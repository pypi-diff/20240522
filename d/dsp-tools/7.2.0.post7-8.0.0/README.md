# Comparing `tmp/dsp_tools-7.2.0.post7.tar.gz` & `tmp/dsp_tools-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsp_tools-7.2.0.post7.tar", max compression
+gzip compressed data, was "dsp_tools-8.0.0.tar", max compression
```

## Comparing `dsp_tools-7.2.0.post7.tar` & `dsp_tools-8.0.0.tar`

### file list

```diff
@@ -1,117 +1,119 @@
--rw-r--r--   0        0        0    35149 2024-05-14 11:55:58.687635 dsp_tools-7.2.0.post7/LICENSE
--rw-r--r--   0        0        0     4941 2024-05-14 11:55:58.703635 dsp_tools-7.2.0.post7/docs/index.md
--rw-r--r--   0        0        0     8406 2024-05-14 11:56:27.899950 dsp_tools-7.2.0.post7/pyproject.toml
--rw-r--r--   0        0        0       41 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/cli/__init__.py
--rw-r--r--   0        0        0     8102 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/cli/call_action.py
--rw-r--r--   0        0        0    13719 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/cli/create_parsers.py
--rw-r--r--   0        0        0     9909 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/cli/entry_point.py
--rw-r--r--   0        0        0        0 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/__init__.py
--rw-r--r--   0        0        0    15987 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/lists.py
--rw-r--r--   0        0        0        0 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/models/__init__.py
--rw-r--r--   0        0        0    14898 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/models/input_error.py
--rw-r--r--   0        0        0     4018 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/models/list_node.py
--rw-r--r--   0        0        0      501 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/models/list_node_name.py
--rw-r--r--   0        0        0    29990 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/new_lists.py
--rw-r--r--   0        0        0     9829 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/project.py
--rw-r--r--   0        0        0    13232 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/properties.py
--rw-r--r--   0        0        0    11887 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/resources.py
--rw-r--r--   0        0        0    11866 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/utils.py
--rw-r--r--   0        0        0      466 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2xml/__init__.py
--rw-r--r--   0        0        0    21361 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2xml/excel2xml_cli.py
--rw-r--r--   0        0        0    80208 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2xml/excel2xml_lib.py
--rw-r--r--   0        0        0     1981 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2xml/propertyelement.py
--rw-r--r--   0        0        0     8275 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/id2iri.py
--rw-r--r--   0        0        0        0 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/ingest_xmlupload/__init__.py
--rw-r--r--   0        0        0     2876 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py
--rw-r--r--   0        0        0     2351 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py
--rw-r--r--   0        0        0     4891 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/ingest_xmlupload/user_information.py
--rw-r--r--   0        0        0        0 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/create/__init__.py
--rw-r--r--   0        0        0    45642 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/create/project_create.py
--rw-r--r--   0        0        0     8243 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/create/project_create_lists.py
--rw-r--r--   0        0        0    19703 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/create/project_validate.py
--rw-r--r--   0        0        0     5743 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/get.py
--rw-r--r--   0        0        0        0 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/__init__.py
--rw-r--r--   0        0        0    12173 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/context.py
--rw-r--r--   0        0        0     8379 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/group.py
--rw-r--r--   0        0        0      850 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/helpers.py
--rw-r--r--   0        0        0    14910 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/listnode.py
--rw-r--r--   0        0        0      245 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/model.py
--rw-r--r--   0        0        0    12710 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/ontology.py
--rw-r--r--   0        0        0    11594 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/project.py
--rw-r--r--   0        0        0      306 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/project_definition.py
--rw-r--r--   0        0        0    17215 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/propertyclass.py
--rw-r--r--   0        0        0    28164 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/resourceclass.py
--rw-r--r--   0        0        0    17030 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/user.py
--rw-r--r--   0        0        0        0 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/resume_xmlupload/__init__.py
--rw-r--r--   0        0        0     3719 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py
--rw-r--r--   0        0        0     4177 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/rosetta.py
--rw-r--r--   0        0        0    16102 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/start_stack.py
--rw-r--r--   0        0        0     1134 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/template.py
--rw-r--r--   0        0        0        0 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/__init__.py
--rw-r--r--   0        0        0     2350 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/ark2iri.py
--rw-r--r--   0        0        0    10356 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py
--rw-r--r--   0        0        0      625 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/iri_resolver.py
--rw-r--r--   0        0        0     3587 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/list_client.py
--rw-r--r--   0        0        0        0 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/deserialise/__init__.py
--rw-r--r--   0        0        0     6448 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/deserialise/deserialise_value.py
--rw-r--r--   0        0        0     3560 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/deserialise/xmlpermission.py
--rw-r--r--   0        0        0     5199 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/deserialise/xmlresource.py
--rw-r--r--   0        0        0     1334 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py
--rw-r--r--   0        0        0     1464 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/namespace_context.py
--rw-r--r--   0        0        0     5549 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py
--rw-r--r--   0        0        0     6752 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py
--rw-r--r--   0        0        0     2388 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/permission.py
--rw-r--r--   0        0        0        0 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/serialise/__init__.py
--rw-r--r--   0        0        0     1302 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/serialise/serialise_value.py
--rw-r--r--   0        0        0      812 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/sipi.py
--rw-r--r--   0        0        0      730 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/upload_state.py
--rw-r--r--   0        0        0     3466 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/ontology_client.py
--rw-r--r--   0        0        0     3140 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/project_client.py
--rw-r--r--   0        0        0     4653 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py
--rw-r--r--   0        0        0    14771 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/resource_create_client.py
--rw-r--r--   0        0        0     4626 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/resource_multimedia.py
--rw-r--r--   0        0        0        0 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/__init__.py
--rw-r--r--   0        0        0    12372 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py
--rw-r--r--   0        0        0     2452 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/graph_models.py
--rw-r--r--   0        0        0     5754 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py
--rw-r--r--   0        0        0     3375 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/stash_models.py
--rw-r--r--   0        0        0     4158 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py
--rw-r--r--   0        0        0     7676 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py
--rw-r--r--   0        0        0     2175 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/upload_config.py
--rw-r--r--   0        0        0      858 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py
--rw-r--r--   0        0        0    19191 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/xmlupload.py
--rw-r--r--   0        0        0        0 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/models/__init__.py
--rw-r--r--   0        0        0      949 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/models/custom_warnings.py
--rw-r--r--   0        0        0     2876 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/models/datetimestamp.py
--rw-r--r--   0        0        0     2785 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/models/exceptions.py
--rw-r--r--   0        0        0     8457 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/models/langstring.py
--rw-r--r--   0        0        0     1777 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/models/projectContext.py
--rw-r--r--   0        0        0        0 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/py.typed
--rw-r--r--   0        0        0     1488 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/0100-template-repo/template.json
--rw-r--r--   0        0        0     1036 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/0100-template-repo/template.xml
--rw-r--r--   0        0        0    29742 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/data.xsd
--rw-r--r--   0        0        0     2770 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/lists-only.json
--rw-r--r--   0        0        0    42680 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/project.json
--rw-r--r--   0        0        0    32411 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/properties-only.json
--rw-r--r--   0        0        0     4240 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/resources-only.json
--rw-r--r--   0        0        0       61 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/start-stack/docker-compose.override.yml
--rw-r--r--   0        0        0     3281 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/start-stack/docker-compose.yml
--rw-r--r--   0        0        0      164 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/start-stack/start-stack-config.yml
--rw-r--r--   0        0        0        0 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/__init__.py
--rw-r--r--   0        0        0     1030 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/connection.py
--rw-r--r--   0        0        0    14126 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/connection_live.py
--rw-r--r--   0        0        0     4554 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/date_util.py
--rw-r--r--   0        0        0      457 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/iri_util.py
--rw-r--r--   0        0        0     1157 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/logger_config.py
--rw-r--r--   0        0        0      705 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/set_encoder.py
--rw-r--r--   0        0        0     5754 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/shared.py
--rw-r--r--   0        0        0      547 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/uri_util.py
--rw-r--r--   0        0        0      978 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/warnings_config.py
--rw-r--r--   0        0        0     4920 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/xml_utils.py
--rw-r--r--   0        0        0     7359 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/xml_validation.py
--rw-r--r--   0        0        0     2312 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/xml_validation_models.py
--rw-r--r--   0        0        0     6388 1970-01-01 00:00:00.000000 dsp_tools-7.2.0.post7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-22 07:20:44.837765 dsp_tools-8.0.0/LICENSE
+-rw-r--r--   0        0        0     4941 2024-05-22 07:20:44.853765 dsp_tools-8.0.0/docs/index.md
+-rw-r--r--   0        0        0     8479 2024-05-22 07:20:44.853765 dsp_tools-8.0.0/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-05-22 07:20:44.853765 dsp_tools-8.0.0/src/dsp_tools/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:20:44.853765 dsp_tools-8.0.0/src/dsp_tools/cli/__init__.py
+-rw-r--r--   0        0        0      237 2024-05-22 07:20:44.853765 dsp_tools-8.0.0/src/dsp_tools/cli/args.py
+-rw-r--r--   0        0        0     7943 2024-05-22 07:20:44.853765 dsp_tools-8.0.0/src/dsp_tools/cli/call_action.py
+-rw-r--r--   0        0        0    13722 2024-05-22 07:20:44.853765 dsp_tools-8.0.0/src/dsp_tools/cli/create_parsers.py
+-rw-r--r--   0        0        0    10116 2024-05-22 07:20:44.853765 dsp_tools-8.0.0/src/dsp_tools/cli/entry_point.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:20:44.853765 dsp_tools-8.0.0/src/dsp_tools/commands/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:20:44.853765 dsp_tools-8.0.0/src/dsp_tools/commands/excel2json/__init__.py
+-rw-r--r--   0        0        0    15987 2024-05-22 07:20:44.853765 dsp_tools-8.0.0/src/dsp_tools/commands/excel2json/lists.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:20:44.853765 dsp_tools-8.0.0/src/dsp_tools/commands/excel2json/models/__init__.py
+-rw-r--r--   0        0        0    14898 2024-05-22 07:20:44.853765 dsp_tools-8.0.0/src/dsp_tools/commands/excel2json/models/input_error.py
+-rw-r--r--   0        0        0     4018 2024-05-22 07:20:44.853765 dsp_tools-8.0.0/src/dsp_tools/commands/excel2json/models/list_node.py
+-rw-r--r--   0        0        0      501 2024-05-22 07:20:44.853765 dsp_tools-8.0.0/src/dsp_tools/commands/excel2json/models/list_node_name.py
+-rw-r--r--   0        0        0    30292 2024-05-22 07:20:44.853765 dsp_tools-8.0.0/src/dsp_tools/commands/excel2json/new_lists.py
+-rw-r--r--   0        0        0     9829 2024-05-22 07:20:44.853765 dsp_tools-8.0.0/src/dsp_tools/commands/excel2json/project.py
+-rw-r--r--   0        0        0    13289 2024-05-22 07:20:44.853765 dsp_tools-8.0.0/src/dsp_tools/commands/excel2json/properties.py
+-rw-r--r--   0        0        0    12292 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/excel2json/resources.py
+-rw-r--r--   0        0        0    12546 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/excel2json/utils.py
+-rw-r--r--   0        0        0      466 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/excel2xml/__init__.py
+-rw-r--r--   0        0        0    21361 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/excel2xml/excel2xml_cli.py
+-rw-r--r--   0        0        0    80218 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/excel2xml/excel2xml_lib.py
+-rw-r--r--   0        0        0     1981 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/excel2xml/propertyelement.py
+-rw-r--r--   0        0        0     8275 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/id2iri.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/ingest_xmlupload/__init__.py
+-rw-r--r--   0        0        0     2817 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py
+-rw-r--r--   0        0        0     4155 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py
+-rw-r--r--   0        0        0     4879 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/ingest_xmlupload/user_information.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/project/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/project/create/__init__.py
+-rw-r--r--   0        0        0    45503 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/project/create/project_create.py
+-rw-r--r--   0        0        0     8170 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/project/create/project_create_lists.py
+-rw-r--r--   0        0        0    19703 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/project/create/project_validate.py
+-rw-r--r--   0        0        0     5590 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/project/get.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/project/models/__init__.py
+-rw-r--r--   0        0        0    12173 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/project/models/context.py
+-rw-r--r--   0        0        0     8379 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/project/models/group.py
+-rw-r--r--   0        0        0      850 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/project/models/helpers.py
+-rw-r--r--   0        0        0    14910 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/project/models/listnode.py
+-rw-r--r--   0        0        0      245 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/project/models/model.py
+-rw-r--r--   0        0        0    12710 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/project/models/ontology.py
+-rw-r--r--   0        0        0    11594 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/project/models/project.py
+-rw-r--r--   0        0        0      306 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/project/models/project_definition.py
+-rw-r--r--   0        0        0    17215 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/project/models/propertyclass.py
+-rw-r--r--   0        0        0    28164 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/project/models/resourceclass.py
+-rw-r--r--   0        0        0    17030 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/project/models/user.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/resume_xmlupload/__init__.py
+-rw-r--r--   0        0        0     3907 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py
+-rw-r--r--   0        0        0     4217 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/rosetta.py
+-rw-r--r--   0        0        0    16105 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/start_stack.py
+-rw-r--r--   0        0        0     1134 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/template.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/__init__.py
+-rw-r--r--   0        0        0     2350 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/ark2iri.py
+-rw-r--r--   0        0        0    10356 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py
+-rw-r--r--   0        0        0      625 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/iri_resolver.py
+-rw-r--r--   0        0        0     3587 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/list_client.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/deserialise/__init__.py
+-rw-r--r--   0        0        0     6448 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/deserialise/deserialise_value.py
+-rw-r--r--   0        0        0     3560 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/deserialise/xmlpermission.py
+-rw-r--r--   0        0        0     4006 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/deserialise/xmlresource.py
+-rw-r--r--   0        0        0     1334 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py
+-rw-r--r--   0        0        0     6234 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/ingest.py
+-rw-r--r--   0        0        0     1551 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/namespace_context.py
+-rw-r--r--   0        0        0     5549 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py
+-rw-r--r--   0        0        0     6752 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py
+-rw-r--r--   0        0        0     2388 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/permission.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/serialise/__init__.py
+-rw-r--r--   0        0        0     1273 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/serialise/jsonld_serialiser.py
+-rw-r--r--   0        0        0     1302 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/serialise/serialise_value.py
+-rw-r--r--   0        0        0      439 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/upload_clients.py
+-rw-r--r--   0        0        0      827 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/upload_state.py
+-rw-r--r--   0        0        0     3466 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/ontology_client.py
+-rw-r--r--   0        0        0     3135 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/project_client.py
+-rw-r--r--   0        0        0     4116 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py
+-rw-r--r--   0        0        0    17002 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/resource_create_client.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/stash/__init__.py
+-rw-r--r--   0        0        0    12372 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py
+-rw-r--r--   0        0        0     2452 2024-05-22 07:20:44.857765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/stash/graph_models.py
+-rw-r--r--   0        0        0     5754 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py
+-rw-r--r--   0        0        0     3375 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/stash/stash_models.py
+-rw-r--r--   0        0        0     4158 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py
+-rw-r--r--   0        0        0     7676 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py
+-rw-r--r--   0        0        0     2175 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/upload_config.py
+-rw-r--r--   0        0        0      858 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py
+-rw-r--r--   0        0        0    19466 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/xmlupload.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/models/__init__.py
+-rw-r--r--   0        0        0      949 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/models/custom_warnings.py
+-rw-r--r--   0        0        0     2876 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/models/datetimestamp.py
+-rw-r--r--   0        0        0     2785 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/models/exceptions.py
+-rw-r--r--   0        0        0     8457 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/models/langstring.py
+-rw-r--r--   0        0        0     1777 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/models/projectContext.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/py.typed
+-rw-r--r--   0        0        0     1488 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/resources/0100-template-repo/template.json
+-rw-r--r--   0        0        0     1036 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/resources/0100-template-repo/template.xml
+-rw-r--r--   0        0        0    29742 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/resources/schema/data.xsd
+-rw-r--r--   0        0        0     2770 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/resources/schema/lists-only.json
+-rw-r--r--   0        0        0    42680 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/resources/schema/project.json
+-rw-r--r--   0        0        0    32411 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/resources/schema/properties-only.json
+-rw-r--r--   0        0        0     4240 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/resources/schema/resources-only.json
+-rw-r--r--   0        0        0       61 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/resources/start-stack/docker-compose.override.yml
+-rw-r--r--   0        0        0     3339 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/resources/start-stack/docker-compose.yml
+-rw-r--r--   0        0        0      164 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/resources/start-stack/start-stack-config.yml
+-rw-r--r--   0        0        0        0 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/utils/__init__.py
+-rw-r--r--   0        0        0     1030 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/utils/connection.py
+-rw-r--r--   0        0        0    14214 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/utils/connection_live.py
+-rw-r--r--   0        0        0     4554 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/utils/date_util.py
+-rw-r--r--   0        0        0      457 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/utils/iri_util.py
+-rw-r--r--   0        0        0     1157 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/utils/logger_config.py
+-rw-r--r--   0        0        0      705 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/utils/set_encoder.py
+-rw-r--r--   0        0        0     5754 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/utils/shared.py
+-rw-r--r--   0        0        0      547 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/utils/uri_util.py
+-rw-r--r--   0        0        0      978 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/utils/warnings_config.py
+-rw-r--r--   0        0        0     4032 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/utils/xml_utils.py
+-rw-r--r--   0        0        0     7358 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/utils/xml_validation.py
+-rw-r--r--   0        0        0     2312 2024-05-22 07:20:44.861765 dsp_tools-8.0.0/src/dsp_tools/utils/xml_validation_models.py
+-rw-r--r--   0        0        0     6382 1970-01-01 00:00:00.000000 dsp_tools-8.0.0/PKG-INFO
```

### Comparing `dsp_tools-7.2.0.post7/LICENSE` & `dsp_tools-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/docs/index.md` & `dsp_tools-8.0.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/pyproject.toml` & `dsp_tools-8.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # See https://packaging.python.org/en/latest/guides/writing-pyproject-toml/#writing-pyproject-toml
 
 [tool.poetry]
 name = "dsp-tools"
-version = "7.2.0.post7"
+version = "8.0.0"
 description = "DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server."
 authors = ["DaSCH - Swiss National Data and Service Center for the Humanities <info@dasch.swiss>"]
 readme = "docs/index.md"
 license = "GPL-3.0-only"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -57,14 +57,15 @@
 types-pyyaml = "^6.0.12.20240311"
 pytest-unordered = "^0.6.0"
 viztracer = "^0.16.2"
 ruff = "^0.4.4"
 pytest-sugar = "^1.0.0"
 pandas-stubs = "^2.2.1.240316"
 types-networkx = "^3.2.1.20240331"
+requests-mock = "^1.12.1"
 
 
 [tool.poetry.scripts]
 dsp-tools = "dsp_tools.cli.entry_point:main"  # definition of the CLI entry point
 
 
 [tool.poetry-exec-plugin.commands]
@@ -130,14 +131,15 @@
 # see https://docs.pytest.org/en/latest/explanation/goodpractices.html#tests-outside-application-code
 pythonpath = [".", "src", "test"]
 
 
 [tool.mypy]
 show_column_numbers = true
 strict = true
+enable_error_code = ["possibly-undefined"]
 exclude = [
     "src/dsp_tools/models/datetimestamp.py",                  # TODO: activate this
     "src/dsp_tools/models/langstring.py",                     # TODO: activate this
     "src/dsp_tools/models/projectContext.py",                 # TODO: activate this
     "src/dsp_tools/commands/project/models/context.py",       # TODO: activate this
     "src/dsp_tools/commands/project/models/group.py",         # TODO: activate this
     "src/dsp_tools/commands/project/models/helpers.py",       # TODO: activate this
@@ -147,15 +149,15 @@
     "src/dsp_tools/commands/project/models/propertyclass.py", # TODO: activate this
     "src/dsp_tools/commands/project/models/resourceclass.py", # TODO: activate this
     "src/dsp_tools/commands/project/models/user.py",          # TODO: activate this
 ]
 
 
 [[tool.mypy.overrides]]
-module = ["jsonpath_ng.*", "viztracer.*"]  # For these packages, no type stubs are available yet
+module = ["jsonpath_ng.*", "viztracer.*", "pyld.*"]  # For these packages, no type stubs are available yet
 ignore_missing_imports = true
 
 
 [tool.ruff]
 line-length = 120
 target-version = "py312"
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/cli/call_action.py` & `dsp_tools-8.0.0/src/dsp_tools/cli/call_action.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 from pathlib import Path
 
 from loguru import logger
 
+from dsp_tools.cli.args import ServerCredentials
 from dsp_tools.commands.excel2json.lists import excel2lists
 from dsp_tools.commands.excel2json.lists import validate_lists_section_with_schema
 from dsp_tools.commands.excel2json.new_lists import new_excel2lists
 from dsp_tools.commands.excel2json.project import excel2json
 from dsp_tools.commands.excel2json.project import new_excel2json
 from dsp_tools.commands.excel2json.properties import excel2properties
 from dsp_tools.commands.excel2json.resources import excel2resources
@@ -20,15 +21,15 @@
 from dsp_tools.commands.resume_xmlupload.resume_xmlupload import resume_xmlupload
 from dsp_tools.commands.rosetta import upload_rosetta
 from dsp_tools.commands.start_stack import StackConfiguration
 from dsp_tools.commands.start_stack import StackHandler
 from dsp_tools.commands.template import generate_template_repo
 from dsp_tools.commands.xmlupload.upload_config import UploadConfig
 from dsp_tools.commands.xmlupload.xmlupload import xmlupload
-from dsp_tools.utils.xml_validation import validate_xml
+from dsp_tools.utils.xml_validation import validate_xml_file
 
 
 def call_requested_action(args: argparse.Namespace) -> bool:
     """
     Call the appropriate method of DSP-TOOLS.
 
     Args:
@@ -164,80 +165,73 @@
         data_model_files=args.excelfolder,
         path_to_output_file=args.project_definition,
     )
 
 
 def _call_ingest_xmlupload(args: argparse.Namespace) -> bool:
     interrupt_after = args.interrupt_after if args.interrupt_after > 0 else None
-    ingest_xmlupload(
+    return ingest_xmlupload(
         xml_file=Path(args.xml_file),
-        user=args.user,
-        password=args.password,
-        dsp_url=args.server,
-        sipi_url=args.sipi_url,
+        creds=_get_creds(args),
         interrupt_after=interrupt_after,
     )
-    return True
 
 
 def _call_xmlupload(args: argparse.Namespace) -> bool:
     if args.validate_only:
-        return validate_xml(args.xmlfile)
+        return validate_xml_file(Path(args.xmlfile))
     else:
         interrupt_after = args.interrupt_after if args.interrupt_after > 0 else None
         return xmlupload(
-            input_file=args.xmlfile,
-            server=args.server,
-            user=args.user,
-            password=args.password,
+            input_file=Path(args.xmlfile),
+            creds=_get_creds(args),
             imgdir=args.imgdir,
-            sipi=args.sipi_url,
             config=UploadConfig(interrupt_after=interrupt_after),
         )
 
 
 def _call_resume_xmlupload(args: argparse.Namespace) -> bool:
     return resume_xmlupload(
-        server=args.server,
-        user=args.user,
-        password=args.password,
-        sipi=args.sipi_url,
+        creds=_get_creds(args),
         skip_first_resource=args.skip_first_resource,
     )
 
 
 def _call_get(args: argparse.Namespace) -> bool:
     return get_project(
         project_identifier=args.project,
         outfile_path=args.project_definition,
-        server=args.server,
-        user=args.user,
-        password=args.password,
+        creds=_get_creds(args),
         verbose=args.verbose,
     )
 
 
 def _call_create(args: argparse.Namespace) -> bool:
     success = False
     match args.lists_only, args.validate_only:
         case True, True:
             success = validate_lists_section_with_schema(args.project_definition)
             print("'Lists' section of the JSON project file is syntactically correct and passed validation.")
         case True, False:
             _, success = create_lists(
                 project_file_as_path_or_parsed=args.project_definition,
-                server=args.server,
-                user=args.user,
-                password=args.password,
+                creds=_get_creds(args),
             )
         case False, True:
             success = validate_project(args.project_definition)
             print("JSON project file is syntactically correct and passed validation.")
         case False, False:
             success = create_project(
                 project_file_as_path_or_parsed=args.project_definition,
-                server=args.server,
-                user_mail=args.user,
-                password=args.password,
+                creds=_get_creds(args),
                 verbose=args.verbose,
             )
     return success
+
+
+def _get_creds(args: argparse.Namespace) -> ServerCredentials:
+    return ServerCredentials(
+        server=args.server,
+        user=args.user,
+        password=args.password,
+        dsp_ingest_url=args.dsp_ingest_url,
+    )
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/cli/create_parsers.py` & `dsp_tools-8.0.0/src/dsp_tools/cli/create_parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
 def _add_start_stack(subparsers: _SubParsersAction[ArgumentParser]) -> None:
     subparser = subparsers.add_parser(name="start-stack", help="Run a local instance of DSP-API and DSP-APP")
     subparser.set_defaults(action="start-stack")
     subparser.add_argument(
         "--max_file_size",
         type=int,
-        help="max. multimedia file size allowed by SIPI, in MB (default: 2000, max: 100'000)",
+        help="max. multimedia file size allowed for ingest, in MB (default: 2000, max: 100'000)",
     )
     subparser.add_argument("--prune", action="store_true", help="execute 'docker system prune' without asking")
     subparser.add_argument(
         "--no-prune", action="store_true", help="don't execute 'docker system prune' (and don't ask)"
     )
     subparser.add_argument(
         "--latest",
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/cli/entry_point.py` & `dsp_tools-8.0.0/src/dsp_tools/cli/entry_point.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     Raises:
         UserError: if user input was wrong
         InputError: if user input was wrong
         InternalError: if the user cannot fix it
     """
     default_dsp_api_url = "http://0.0.0.0:3333"
-    default_sipi_url = "http://0.0.0.0:1024"
+    default_dsp_ingest_url = "http://0.0.0.0:3340"
     root_user_email = "root@example.com"
     root_user_pw = "test"
 
     parser = make_parser(
         default_dsp_api_url=default_dsp_api_url,
         root_user_email=root_user_email,
         root_user_pw=root_user_pw,
@@ -58,18 +58,18 @@
         parser=parser,
     )
     _check_version()
     _log_cli_arguments(parsed_arguments)
     initialize_warnings()
 
     try:
-        parsed_arguments = _derive_sipi_url(
+        parsed_arguments = _derive_dsp_ingest_url(
             parsed_arguments=parsed_arguments,
             default_dsp_api_url=default_dsp_api_url,
-            default_sipi_url=default_sipi_url,
+            default_dsp_ingest_url=default_dsp_ingest_url,
         )
         success = call_requested_action(parsed_arguments)
     except BaseError as err:
         logger.exception("The process was terminated because of an Error:")
         print("\nThe process was terminated because of an Error:")
         print(err.message)
         sys.exit(1)
@@ -197,93 +197,95 @@
     for line in metadata_lines:
         logger.info(line)
     for line in parameter_lines:
         logger.info(line)
     logger.info("*" * asterisk_count)
 
 
-def _get_canonical_server_and_sipi_url(
+def _get_canonical_server_and_dsp_ingest_url(
     server: str,
     default_dsp_api_url: str,
-    default_sipi_url: str,
+    default_dsp_ingest_url: str,
 ) -> tuple[str, str]:
     """
     Based on the DSP server URL passed by the user,
     transform it to its canonical form,
-    and derive the SIPI URL from it.
+    and derive the ingest server URL from it.
 
     If the DSP server URL points to port 3333 on localhost,
-    the SIPI URL will point to port 1024 on localhost.
+    the ingest server will point to port 3340 on localhost.
 
     If the DSP server URL points to a remote server ending in "dasch.swiss",
     modify it (if necessary) to point to the "api" subdomain of that server,
-    and add a new "sipi_url" argument pointing to the "iiif" subdomain of that server.
+    and add a new "dsp_ingest_url" argument pointing to the "ingest" subdomain of that server.
 
     Args:
         server: DSP server URL passed by the user
         default_dsp_api_url: default DSP server on localhost
-        default_sipi_url: default SIPI server on localhost
+        default_dsp_ingest_url: default ingest server on localhost
 
     Raises:
         UserError: if the DSP server URL passed by the user is invalid
 
     Returns:
-        canonical DSP URL and SIPI URL
+        canonical DSP URL and ingest server URL
     """
     localhost_match = regex.search(r"(0\.0\.0\.0|localhost):3333", server)
-    remote_url_match = regex.search(r"^(?:https?:\/\/)?(?:admin\.|api\.|iiif\.|app\.)?((?:.+\.)?dasch)\.swiss", server)
+    remote_url_match = regex.search(
+        r"^(?:https?:\/\/)?(?:admin\.|api\.|ingest\.|app\.)?((?:.+\.)?dasch)\.swiss", server
+    )
 
     if localhost_match:
         server = default_dsp_api_url
-        sipi_url = default_sipi_url
+        dsp_ingest_url = default_dsp_ingest_url
     elif remote_url_match:
         server = f"https://api.{remote_url_match.group(1)}.swiss"
-        sipi_url = f"https://iiif.{remote_url_match.group(1)}.swiss"
+        dsp_ingest_url = f"https://ingest.{remote_url_match.group(1)}.swiss"
     else:
         logger.error(f"Invalid DSP server URL '{server}'")
         raise UserError(f"ERROR: Invalid DSP server URL '{server}'")
 
-    logger.info(f"Using DSP server '{server}' and SIPI server '{sipi_url}'")
-    print(f"Using DSP server '{server}' and SIPI server '{sipi_url}'")
+    logger.info(f"Using DSP server '{server}' and ingest server '{dsp_ingest_url}'")
+    print(f"Using DSP server '{server}' and ingest server '{dsp_ingest_url}'")
 
-    return server, sipi_url
+    return server, dsp_ingest_url
 
 
-def _derive_sipi_url(
+def _derive_dsp_ingest_url(
     parsed_arguments: argparse.Namespace,
     default_dsp_api_url: str,
-    default_sipi_url: str,
+    default_dsp_ingest_url: str,
 ) -> argparse.Namespace:
     """
-    Modify the parsed arguments so that the DSP and SIPI URLs are correct.
+    Modify the parsed arguments so that the DSP and ingest server URLs are correct.
     Based on the DSP server URL passed by the user,
     transform it to its canonical form,
-    and derive the SIPI URL from it.
+    and derive the ingest server URL from it.
 
     Args:
         parsed_arguments: CLI arguments passed by the user, parsed by argparse
         default_dsp_api_url: default DSP server on localhost
-        default_sipi_url: default SIPI server on localhost
+        default_dsp_ingest_url: default ingest server on localhost
 
     Raises:
         UserError: if the DSP server URL passed by the user is invalid
 
     Returns:
         the modified arguments
     """
     if not hasattr(parsed_arguments, "server"):
         # some CLI actions (like excel2json, excel2xml, start-stack, ...) don't have a server at all
         return parsed_arguments
 
-    server, sipi_url = _get_canonical_server_and_sipi_url(
+    server, dsp_ingest_url = _get_canonical_server_and_dsp_ingest_url(
         server=parsed_arguments.server,
         default_dsp_api_url=default_dsp_api_url,
-        default_sipi_url=default_sipi_url,
+        default_dsp_ingest_url=default_dsp_ingest_url,
     )
     parsed_arguments.server = server
-    parsed_arguments.sipi_url = sipi_url
+    parsed_arguments.dsp_ingest_url = dsp_ingest_url
 
     return parsed_arguments
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/lists.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/excel2json/lists.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/models/input_error.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/excel2json/models/input_error.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/models/list_node.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/excel2json/models/list_node.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/new_lists.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/excel2json/new_lists.py`

 * *Files 2% similar despite different names*

```diff
@@ -662,26 +662,30 @@
         list_problems = cast(list[Problem], problems)
         return ListSheetContentProblem(sheet_name, list_problems)
     return None
 
 
 def _check_for_erroneous_node_info_one_df(df: pd.DataFrame, columns: list[str]) -> list[NodesPerRowProblem]:
     problems = []
-    for i, col in enumerate(columns):
-        to_check_cols = columns[i:]
-        problems.extend(_check_for_erroneous_entries_one_column_level(df, to_check_cols))
+    for focus_col_index, col in enumerate(columns):
+        problems.extend(_check_for_erroneous_entries_one_column_level(df, columns, focus_col_index))
     return problems
 
 
-def _check_for_erroneous_entries_one_column_level(df: pd.DataFrame, columns: list[str]) -> list[NodesPerRowProblem]:
+def _check_for_erroneous_entries_one_column_level(
+    df: pd.DataFrame, columns: list[str], focus_col_index: int
+) -> list[NodesPerRowProblem]:
     # column level refers to the hierarchical level of the nodes. eg. "en_1"
-    grouped = df.groupby(columns[0])
+    # we need to group by from the current column all the way back to its ancestors,
+    # otherwise identical values in that column may be interpreted as belonging to the same group
+    grouped = df.groupby(columns[: focus_col_index + 1])
     problems = []
     for name, group in grouped:
-        problems.extend(_check_for_erroneous_entries_one_grouped_df(group, columns))
+        remaining_to_check_columns = columns[focus_col_index:]
+        problems.extend(_check_for_erroneous_entries_one_grouped_df(group, remaining_to_check_columns))
     return problems
 
 
 def _check_for_erroneous_entries_one_grouped_df(
     group: pd.DataFrame, target_cols: list[str]
 ) -> list[NodesPerRowProblem]:
     problems = []
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/project.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/excel2json/project.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/properties.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/excel2json/properties.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from dsp_tools.commands.excel2json.models.input_error import InvalidExcelContentProblem
 from dsp_tools.commands.excel2json.models.input_error import JsonValidationPropertyProblem
 from dsp_tools.commands.excel2json.models.input_error import MissingValuesInRowProblem
 from dsp_tools.commands.excel2json.models.input_error import MoreThanOneSheetProblem
 from dsp_tools.commands.excel2json.models.input_error import PositionInExcel
 from dsp_tools.commands.excel2json.models.input_error import Problem
+from dsp_tools.commands.excel2json.utils import add_optional_columns
 from dsp_tools.commands.excel2json.utils import check_column_for_duplicate
 from dsp_tools.commands.excel2json.utils import check_contains_required_columns
 from dsp_tools.commands.excel2json.utils import check_required_values
 from dsp_tools.commands.excel2json.utils import col_must_or_not_empty_based_on_other_col
 from dsp_tools.commands.excel2json.utils import find_one_full_cell_in_cols
 from dsp_tools.commands.excel2json.utils import get_comments
 from dsp_tools.commands.excel2json.utils import get_labels
@@ -55,15 +56,28 @@
     """
 
     property_df = _read_check_property_df(excelfile)
 
     property_df = _rename_deprecated_columnnames(df=property_df, excelfile=excelfile)
 
     # Not all columns have to be filled, users may delete some for ease of use, but it would generate an error later
-    property_df = _add_optional_columns(df=property_df)
+    optional_col_set = {
+        "label_en",
+        "label_de",
+        "label_fr",
+        "label_it",
+        "label_rm",
+        "comment_en",
+        "comment_de",
+        "comment_fr",
+        "comment_it",
+        "comment_rm",
+        "subject",
+    }
+    property_df = add_optional_columns(property_df, optional_col_set)
 
     _do_property_excel_compliance(df=property_df, excelfile=excelfile)
 
     _check_for_deprecated_syntax(property_df)
 
     # transform every row into a property
     props = [
@@ -150,36 +164,14 @@
         problems.extend(missing_vals_check)
     if any(problems):
         extra = [problem.execute_error_protocol() for problem in problems if problem]
         msg = [f"There is a problem with the excel file: '{excelfile}'", *extra]
         raise InputError("\n\n".join(msg))
 
 
-def _add_optional_columns(df: pd.DataFrame) -> pd.DataFrame:
-    optional_col_set = {
-        "label_en",
-        "label_de",
-        "label_fr",
-        "label_it",
-        "label_rm",
-        "comment_en",
-        "comment_de",
-        "comment_fr",
-        "comment_it",
-        "comment_rm",
-        "subject",
-    }
-    in_df_cols = set(df.columns)
-    if not optional_col_set.issubset(in_df_cols):
-        additional_col = list(optional_col_set.difference(in_df_cols))
-        additional_df = pd.DataFrame(columns=additional_col, index=df.index)
-        df = pd.concat(objs=[df, additional_df], axis=1)
-    return df
-
-
 def _check_missing_values_in_row(df: pd.DataFrame) -> None | list[MissingValuesInRowProblem]:
     required_values = ["name", "super", "object", "gui_element"]
     missing_dict = check_required_values(df=df, required_values_columns=required_values)
     missing_labels = find_one_full_cell_in_cols(df=df, required_columns=language_label_col)
     if missing_labels is not None:
         missing_dict.update({"label": missing_labels})
     missing_gui_attributes = _check_compliance_gui_attributes(df=df)
@@ -205,24 +197,32 @@
     no_attribute_check = col_must_or_not_empty_based_on_other_col(
         df=df,
         substring_list=no_attributes,
         substring_colname="gui_element",
         check_empty_colname="gui_attributes",
         must_have_value=False,
     )
+    final_series = _get_final_series(mandatory_check, no_attribute_check)
+    return {"gui_attributes": final_series} if final_series is not None else None
+
+
+def _get_final_series(
+    mandatory_check: pd.Series[bool] | None, no_attribute_check: pd.Series[bool] | None
+) -> pd.Series[bool] | None:
+    final_series: pd.Series[bool] = pd.Series()
     match mandatory_check, no_attribute_check:
         case None, None:
             return None
         case pd.Series(), pd.Series():
-            final_series: pd.Series[bool] = pd.Series(np.logical_or(mandatory_check, no_attribute_check))  # type: ignore[arg-type]
+            final_series = pd.Series(np.logical_or(mandatory_check, no_attribute_check))  # type: ignore[arg-type]
         case pd.Series(), None:
             final_series = mandatory_check  # type: ignore[assignment]
-        case None, pd.Series:
-            final_series = no_attribute_check
-    return {"gui_attributes": final_series}
+        case None, pd.Series():
+            final_series = no_attribute_check  # type: ignore[assignment]
+    return final_series
 
 
 def _row2prop(df_row: pd.Series[Any], row_num: int, excelfile: str) -> dict[str, Any]:
     _property = {x: df_row[x] for x in mandatory_properties} | {
         "labels": get_labels(df_row=df_row),
         "super": [s.strip() for s in df_row["super"].split(",")],
     }
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/resources.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/excel2json/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import regex
 
 from dsp_tools.commands.excel2json.models.input_error import JsonValidationResourceProblem
 from dsp_tools.commands.excel2json.models.input_error import MissingValuesInRowProblem
 from dsp_tools.commands.excel2json.models.input_error import PositionInExcel
 from dsp_tools.commands.excel2json.models.input_error import Problem
 from dsp_tools.commands.excel2json.models.input_error import ResourcesSheetsNotAsExpected
+from dsp_tools.commands.excel2json.utils import add_optional_columns
 from dsp_tools.commands.excel2json.utils import check_column_for_duplicate
 from dsp_tools.commands.excel2json.utils import read_and_clean_all_sheets
 from dsp_tools.models.exceptions import InputError
 from dsp_tools.utils.shared import check_notna
 from dsp_tools.utils.shared import prepare_dataframe
 
 languages = ["en", "de", "fr", "it", "rm"]
@@ -264,14 +265,29 @@
     else:
         msg = (
             "The excel file 'resources.xlsx' has some problems.\n"
             "There is more than one excel sheet called 'classes'.\n"
             "This is a protected name and cannot be used for other sheets."
         )
         raise InputError(msg)
+    classes_df = add_optional_columns(
+        classes_df,
+        {
+            "label_en",
+            "label_de",
+            "label_fr",
+            "label_it",
+            "label_rm",
+            "comment_en",
+            "comment_de",
+            "comment_fr",
+            "comment_it",
+            "comment_rm",
+        },
+    )
     classes_df = prepare_dataframe(
         df=classes_df,
         required_columns=["name"],
         location_of_sheet="Sheet 'classes' in file 'resources.xlsx'",
     )
     return classes_df, resource_dfs
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/utils.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/excel2json/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -265,7 +265,27 @@
     # This returns True if it finds the substring in the cell, they are joined in a RegEx "|" which denotes "or".
     # If it does not match any of the sub-strings, then the RegEx returns False,
     # which means that the value in the column "check_empty_colname" is not relevant.
     substring_array = df[substring_colname].str.contains("|".join(substring_list), na=False, regex=True)
     # If both are True logical_and returns True otherwise False
     combined_array = np.logical_and(na_series, substring_array)
     return pd.Series(combined_array) if any(combined_array) else None
+
+
+def add_optional_columns(df: pd.DataFrame, optional_col_set: set[str]) -> pd.DataFrame:
+    """
+    Adds columns to a df if they are not already present.
+    The content of the columns is empty.
+
+    Args:
+        df: Dataframe
+        optional_col_set: set of columns that may be added
+
+    Returns:
+        Dataframe with additional columns if they were not present
+    """
+    in_df_cols = set(df.columns)
+    if not optional_col_set.issubset(in_df_cols):
+        additional_col = list(optional_col_set.difference(in_df_cols))
+        additional_df = pd.DataFrame(columns=additional_col, index=df.index)
+        df = pd.concat(objs=[df, additional_df], axis=1)
+    return df
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2xml/excel2xml_cli.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/excel2xml/excel2xml_cli.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2xml/excel2xml_lib.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/excel2xml/excel2xml_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,4970 +44,4971 @@
 000002b0: 2069 6d70 6f72 7420 7369 6d70 6c69 6679   import simplify
 000002c0: 5f6e 616d 650a 6672 6f6d 2064 7370 5f74  _name.from dsp_t
 000002d0: 6f6f 6c73 2e75 7469 6c73 2e75 7269 5f75  ools.utils.uri_u
 000002e0: 7469 6c20 696d 706f 7274 2069 735f 7572  til import is_ur
 000002f0: 690a 6672 6f6d 2064 7370 5f74 6f6f 6c73  i.from dsp_tools
 00000300: 2e75 7469 6c73 2e78 6d6c 5f76 616c 6964  .utils.xml_valid
 00000310: 6174 696f 6e20 696d 706f 7274 2076 616c  ation import val
-00000320: 6964 6174 655f 786d 6c0a 0a23 2072 7566  idate_xml..# ruf
-00000330: 663a 206e 6f71 613a 2045 3530 312c 2055  f: noqa: E501, U
-00000340: 5030 3331 2028 6c69 6e65 2d74 6f6f 2d6c  P031 (line-too-l
-00000350: 6f6e 672c 2075 7365 2066 2d73 7472 696e  ong, use f-strin
-00000360: 6720 6f76 6572 2070 6572 6365 6e74 2066  g over percent f
-00000370: 6f72 6d61 7474 696e 6729 0a0a 0a78 6d6c  ormatting)...xml
-00000380: 5f6e 616d 6573 7061 6365 5f6d 6170 203d  _namespace_map =
-00000390: 207b 4e6f 6e65 3a20 2268 7474 7073 3a2f   {None: "https:/
-000003a0: 2f64 6173 6368 2e73 7769 7373 2f73 6368  /dasch.swiss/sch
-000003b0: 656d 6122 2c20 2278 7369 223a 2022 6874  ema", "xsi": "ht
-000003c0: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
-000003d0: 3230 3031 2f58 4d4c 5363 6865 6d61 2d69  2001/XMLSchema-i
-000003e0: 6e73 7461 6e63 6522 7d0a 0a0a 6465 6620  nstance"}...def 
-000003f0: 6d61 6b65 5f78 7364 5f69 645f 636f 6d70  make_xsd_id_comp
-00000400: 6174 6962 6c65 2873 7472 696e 673a 2073  atible(string: s
-00000410: 7472 2920 2d3e 2073 7472 3a0a 2020 2020  tr) -> str:.    
-00000420: 2222 220a 2020 2020 4d61 6b65 2061 2073  """.    Make a s
-00000430: 7472 696e 6720 636f 6d70 6174 6962 6c65  tring compatible
-00000440: 2077 6974 6820 7468 6520 636f 6e73 7472   with the constr
-00000450: 6169 6e74 7320 6f66 2078 7364 3a49 442c  aints of xsd:ID,
-00000460: 2073 6f20 7468 6174 2069 7420 6361 6e20   so that it can 
-00000470: 6265 2075 7365 6420 6173 2022 6964 2220  be used as "id" 
-00000480: 6174 7472 6962 7574 6520 6f66 2061 203c  attribute of a <
-00000490: 7265 736f 7572 6365 3e0a 2020 2020 7461  resource>.    ta
-000004a0: 672e 2041 6e20 7873 643a 4944 206d 7573  g. An xsd:ID mus
-000004b0: 7420 6e6f 7420 636f 6e74 6169 6e20 7370  t not contain sp
-000004c0: 6563 6961 6c20 6368 6172 6163 7465 7273  ecial characters
-000004d0: 2c20 616e 6420 6974 206d 7573 7420 6265  , and it must be
-000004e0: 2075 6e69 7175 6520 696e 2074 6865 2064   unique in the d
-000004f0: 6f63 756d 656e 742e 0a0a 2020 2020 5468  ocument...    Th
-00000500: 6973 206d 6574 686f 6420 7265 706c 6163  is method replac
-00000510: 6573 2074 6865 2069 6c6c 6567 616c 2063  es the illegal c
-00000520: 6861 7261 6374 6572 7320 6279 2022 5f22  haracters by "_"
-00000530: 2061 6e64 2061 7070 656e 6473 2061 2072   and appends a r
-00000540: 616e 646f 6d20 636f 6d70 6f6e 656e 7420  andom component 
-00000550: 746f 2074 6865 2073 7472 696e 6720 746f  to the string to
-00000560: 206d 616b 6520 6974 2075 6e69 7175 652e   make it unique.
-00000570: 0a0a 2020 2020 5468 6520 7374 7269 6e67  ..    The string
-00000580: 206d 7573 7420 636f 6e74 6169 6e20 6174   must contain at
-00000590: 206c 6561 7374 206f 6e65 2055 6e69 636f   least one Unico
-000005a0: 6465 206c 6574 7465 7220 286d 6174 6368  de letter (match
-000005b0: 696e 6720 7468 6520 7265 6765 7820 6060  ing the regex ``
-000005c0: 5c5c 707b 4c7d 6060 292c 2075 6e64 6572  \\p{L}``), under
-000005d0: 7363 6f72 652c 2021 2c20 3f2c 206f 7220  score, !, ?, or 
-000005e0: 6e75 6d62 6572 2c0a 2020 2020 6275 7420  number,.    but 
-000005f0: 6d75 7374 206e 6f74 2062 6520 224e 6f6e  must not be "Non
-00000600: 6522 2c20 223c 4e41 3e22 2c20 224e 2f41  e", "<NA>", "N/A
-00000610: 222c 206f 7220 222d 222e 204f 7468 6572  ", or "-". Other
-00000620: 7769 7365 2c20 6120 4261 7365 4572 726f  wise, a BaseErro
-00000630: 7220 7769 6c6c 2062 6520 7261 6973 6564  r will be raised
-00000640: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-00000650: 2020 2020 2073 7472 696e 673a 2069 6e70       string: inp
-00000660: 7574 2073 7472 696e 670a 0a20 2020 2052  ut string..    R
-00000670: 6169 7365 733a 0a20 2020 2020 2020 2042  aises:.        B
-00000680: 6173 6545 7272 6f72 3a20 6966 2074 6865  aseError: if the
-00000690: 2069 6e70 7574 2063 616e 6e6f 7420 6265   input cannot be
-000006a0: 2074 7261 6e73 666f 726d 6564 2074 6f20   transformed to 
-000006b0: 616e 2078 7364 3a49 440a 0a20 2020 2052  an xsd:ID..    R
-000006c0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-000006d0: 616e 2078 7364 2049 4420 6261 7365 6420  an xsd ID based 
-000006e0: 6f6e 2074 6865 2069 6e70 7574 2073 7472  on the input str
-000006f0: 696e 670a 2020 2020 2222 220a 0a20 2020  ing.    """..   
-00000700: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
-00000710: 6365 2873 7472 696e 672c 2073 7472 2920  ce(string, str) 
-00000720: 6f72 206e 6f74 2063 6865 636b 5f6e 6f74  or not check_not
-00000730: 6e61 2873 7472 696e 6729 3a0a 2020 2020  na(string):.    
-00000740: 2020 2020 7261 6973 6520 4261 7365 4572      raise BaseEr
-00000750: 726f 7228 6622 5468 6520 696e 7075 7420  ror(f"The input 
-00000760: 277b 7374 7269 6e67 7d27 2063 616e 6e6f  '{string}' canno
-00000770: 7420 6265 2074 7261 6e73 666f 726d 6564  t be transformed
-00000780: 2074 6f20 616e 2078 7364 3a49 4422 290a   to an xsd:ID").
-00000790: 0a20 2020 2023 2069 6620 7374 6172 7420  .    # if start 
-000007a0: 6f66 2073 7472 696e 6720 6973 206e 6569  of string is nei
-000007b0: 7468 6572 206c 6574 7465 7220 6e6f 7220  ther letter nor 
-000007c0: 756e 6465 7273 636f 7265 2c20 6164 6420  underscore, add 
-000007d0: 616e 2075 6e64 6572 7363 6f72 650a 2020  an underscore.  
-000007e0: 2020 7265 7320 3d20 7265 6765 782e 7375    res = regex.su
-000007f0: 6228 7222 5e28 3f3d 5b5e 412d 5a61 2d7a  b(r"^(?=[^A-Za-z
-00000800: 5f5d 2922 2c20 225f 222c 2073 7472 696e  _])", "_", strin
-00000810: 6729 0a0a 2020 2020 2320 7265 706c 6163  g)..    # replac
-00000820: 6520 616c 6c20 696c 6c65 6761 6c20 6368  e all illegal ch
-00000830: 6172 6163 7465 7273 2062 7920 756e 6465  aracters by unde
-00000840: 7273 636f 7265 0a20 2020 2072 6573 203d  rscore.    res =
-00000850: 2072 6567 6578 2e73 7562 2872 225b 5e5c   regex.sub(r"[^\
-00000860: 775f 5c2d 2e5d 222c 2022 5f22 2c20 7265  w_\-.]", "_", re
-00000870: 732c 2066 6c61 6773 3d72 6567 6578 2e41  s, flags=regex.A
-00000880: 5343 4949 290a 0a20 2020 2023 2061 6464  SCII)..    # add
-00000890: 2075 7569 640a 2020 2020 5f75 7569 6420   uuid.    _uuid 
-000008a0: 3d20 7575 6964 2e75 7569 6434 2829 0a20  = uuid.uuid4(). 
-000008b0: 2020 2072 6573 203d 2066 227b 7265 737d     res = f"{res}
-000008c0: 5f7b 5f75 7569 647d 220a 0a20 2020 2072  _{_uuid}"..    r
-000008d0: 6574 7572 6e20 7265 730a 0a0a 6465 6620  eturn res...def 
-000008e0: 5f66 696e 645f 6672 656e 6368 5f62 635f  _find_french_bc_
-000008f0: 6461 7465 280a 2020 2020 7374 7269 6e67  date(.    string
-00000900: 3a20 7374 722c 0a20 2020 206c 6f6f 6b62  : str,.    lookb
-00000910: 6568 696e 643a 2073 7472 2c0a 2020 2020  ehind: str,.    
-00000920: 6c6f 6f6b 6168 6561 643a 2073 7472 2c0a  lookahead: str,.
-00000930: 2920 2d3e 204f 7074 696f 6e61 6c5b 7374  ) -> Optional[st
-00000940: 725d 3a0a 2020 2020 6672 656e 6368 5f62  r]:.    french_b
-00000950: 635f 7265 6765 7820 3d20 7222 6176 283f  c_regex = r"av(?
-00000960: 3a5c 2e20 7c5c 2e7c 2029 4a5c 2e3f 2d3f  :\. |\.| )J\.?-?
-00000970: 435c 2e3f 220a 2020 2020 6966 206e 6f74  C\.?".    if not
-00000980: 2072 6567 6578 2e73 6561 7263 6828 6672   regex.search(fr
-00000990: 656e 6368 5f62 635f 7265 6765 782c 2073  ench_bc_regex, s
-000009a0: 7472 696e 6729 3a0a 2020 2020 2020 2020  tring):.        
-000009b0: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
-000009c0: 2079 6561 725f 7265 6765 7820 3d20 7222   year_regex = r"
-000009d0: 5c64 7b31 2c35 7d22 0a20 2020 2073 6570  \d{1,5}".    sep
-000009e0: 5f72 6567 6578 203d 2072 2220 3f2d 203f  _regex = r" ?- ?
-000009f0: 220a 0a20 2020 2079 6561 725f 7261 6e67  "..    year_rang
-00000a00: 655f 7265 6765 7820 3d20 7266 227b 6c6f  e_regex = rf"{lo
-00000a10: 6f6b 6265 6869 6e64 7d28 7b79 6561 725f  okbehind}({year_
-00000a20: 7265 6765 787d 297b 7365 705f 7265 6765  regex}){sep_rege
-00000a30: 787d 287b 7965 6172 5f72 6567 6578 7d29  x}({year_regex})
-00000a40: 207b 6672 656e 6368 5f62 635f 7265 6765   {french_bc_rege
-00000a50: 787d 7b6c 6f6f 6b61 6865 6164 7d22 0a20  x}{lookahead}". 
-00000a60: 2020 2079 6561 725f 7261 6e67 6520 3d20     year_range = 
-00000a70: 7265 6765 782e 7365 6172 6368 2879 6561  regex.search(yea
-00000a80: 725f 7261 6e67 655f 7265 6765 782c 2073  r_range_regex, s
-00000a90: 7472 696e 6729 0a20 2020 2069 6620 7965  tring).    if ye
-00000aa0: 6172 5f72 616e 6765 3a0a 2020 2020 2020  ar_range:.      
-00000ab0: 2020 7374 6172 745f 7965 6172 203d 2069    start_year = i
-00000ac0: 6e74 2879 6561 725f 7261 6e67 652e 6772  nt(year_range.gr
-00000ad0: 6f75 7028 3129 290a 2020 2020 2020 2020  oup(1)).        
-00000ae0: 656e 645f 7965 6172 203d 2069 6e74 2879  end_year = int(y
-00000af0: 6561 725f 7261 6e67 652e 6772 6f75 7028  ear_range.group(
-00000b00: 3229 290a 2020 2020 2020 2020 6966 2065  2)).        if e
-00000b10: 6e64 5f79 6561 7220 3e20 7374 6172 745f  nd_year > start_
-00000b20: 7965 6172 3a0a 2020 2020 2020 2020 2020  year:.          
-00000b30: 2020 7265 7475 726e 204e 6f6e 650a 2020    return None.  
-00000b40: 2020 2020 2020 7265 7475 726e 2066 2247        return f"G
-00000b50: 5245 474f 5249 414e 3a42 433a 7b73 7461  REGORIAN:BC:{sta
-00000b60: 7274 5f79 6561 727d 3a42 433a 7b65 6e64  rt_year}:BC:{end
-00000b70: 5f79 6561 727d 220a 0a20 2020 2073 696e  _year}"..    sin
-00000b80: 676c 655f 7965 6172 5f72 6567 6578 203d  gle_year_regex =
-00000b90: 2072 6622 7b6c 6f6f 6b62 6568 696e 647d   rf"{lookbehind}
-00000ba0: 287b 7965 6172 5f72 6567 6578 7d29 207b  ({year_regex}) {
-00000bb0: 6672 656e 6368 5f62 635f 7265 6765 787d  french_bc_regex}
-00000bc0: 7b6c 6f6f 6b61 6865 6164 7d22 0a20 2020  {lookahead}".   
-00000bd0: 2073 696e 676c 655f 7965 6172 203d 2072   single_year = r
-00000be0: 6567 6578 2e73 6561 7263 6828 7369 6e67  egex.search(sing
-00000bf0: 6c65 5f79 6561 725f 7265 6765 782c 2073  le_year_regex, s
-00000c00: 7472 696e 6729 0a20 2020 2069 6620 7369  tring).    if si
-00000c10: 6e67 6c65 5f79 6561 723a 0a20 2020 2020  ngle_year:.     
-00000c20: 2020 2073 7461 7274 5f79 6561 7220 3d20     start_year = 
-00000c30: 696e 7428 7369 6e67 6c65 5f79 6561 722e  int(single_year.
-00000c40: 6772 6f75 7028 3129 290a 2020 2020 2020  group(1)).      
-00000c50: 2020 7265 7475 726e 2066 2247 5245 474f    return f"GREGO
-00000c60: 5249 414e 3a42 433a 7b73 7461 7274 5f79  RIAN:BC:{start_y
-00000c70: 6561 727d 3a42 433a 7b73 7461 7274 5f79  ear}:BC:{start_y
-00000c80: 6561 727d 220a 0a20 2020 2072 6574 7572  ear}"..    retur
-00000c90: 6e20 4e6f 6e65 0a0a 0a64 6566 2066 696e  n None...def fin
-00000ca0: 645f 6461 7465 5f69 6e5f 7374 7269 6e67  d_date_in_string
-00000cb0: 2873 7472 696e 673a 2073 7472 2920 2d3e  (string: str) ->
-00000cc0: 204f 7074 696f 6e61 6c5b 7374 725d 3a0a   Optional[str]:.
-00000cd0: 2020 2020 2222 220a 2020 2020 4368 6563      """.    Chec
-00000ce0: 6b73 2069 6620 6120 7374 7269 6e67 2063  ks if a string c
-00000cf0: 6f6e 7461 696e 7320 6120 6461 7465 2076  ontains a date v
-00000d00: 616c 7565 2028 7369 6e67 6c65 2064 6174  alue (single dat
-00000d10: 652c 206f 7220 6461 7465 2072 616e 6765  e, or date range
-00000d20: 292c 0a20 2020 2061 6e64 2072 6574 7572  ),.    and retur
-00000d30: 6e73 2074 6865 2066 6972 7374 2066 6f75  ns the first fou
-00000d40: 6e64 2064 6174 6520 6173 2044 5350 2d66  nd date as DSP-f
-00000d50: 6f72 6d61 7474 6564 2073 7472 696e 672e  ormatted string.
-00000d60: 0a20 2020 2052 6574 7572 6e73 204e 6f6e  .    Returns Non
-00000d70: 6520 6966 206e 6f20 6461 7465 2077 6173  e if no date was
-00000d80: 2066 6f75 6e64 2e0a 0a20 2020 204e 6f74   found...    Not
-00000d90: 6573 3a0a 2020 2020 2020 2020 2d20 416c  es:.        - Al
-00000da0: 6c20 6461 7465 7320 6172 6520 696e 7465  l dates are inte
-00000db0: 7270 7265 7465 6420 696e 2074 6865 2043  rpreted in the C
-00000dc0: 6872 6973 7469 616e 2065 7261 2061 6e64  hristian era and
-00000dd0: 2074 6865 2047 7265 676f 7269 616e 2063   the Gregorian c
-00000de0: 616c 656e 6461 722e 0a20 2020 2020 2020  alendar..       
-00000df0: 202d 2042 4320 6461 7465 7320 6172 6520   - BC dates are 
-00000e00: 6f6e 6c79 2073 7570 706f 7274 6564 2069  only supported i
-00000e10: 6e20 4672 656e 6368 206e 6f74 6174 696f  n French notatio
-00000e20: 6e20 2865 2e67 2e20 3130 3030 2d39 3030  n (e.g. 1000-900
-00000e30: 2061 762e 204a 2e2d 432e 292e 0a20 2020   av. J.-C.)..   
-00000e40: 2020 2020 202d 2054 6865 2079 6561 7273       - The years
-00000e50: 2030 3030 302d 3239 3939 2061 7265 2073   0000-2999 are s
-00000e60: 7570 706f 7274 6564 2c20 696e 2033 2f34  upported, in 3/4
-00000e70: 2d64 6967 6974 2066 6f72 6d2e 0a20 2020  -digit form..   
-00000e80: 2020 2020 202d 2044 6174 6573 2077 7269       - Dates wri
-00000e90: 7474 656e 2077 6974 6820 736c 6173 6865  tten with slashe
-00000ea0: 7320 6172 6520 616c 7761 7973 2069 6e74  s are always int
-00000eb0: 6572 7072 6574 6564 2069 6e20 6120 4575  erpreted in a Eu
-00000ec0: 726f 7065 616e 206d 616e 6e65 723a 2035  ropean manner: 5
-00000ed0: 2f31 312f 3230 3231 2069 7320 7468 6520  /11/2021 is the 
-00000ee0: 3574 6820 6f66 204e 6f76 656d 6265 722e  5th of November.
-00000ef0: 0a20 2020 2020 2020 202d 2049 6e20 7468  .        - In th
-00000f00: 6520 4575 726f 7065 616e 206e 6f74 6174  e European notat
-00000f10: 696f 6e2c 2032 2d64 6967 6974 2079 6561  ion, 2-digit yea
-00000f20: 7273 2061 7265 2065 7870 616e 6465 6420  rs are expanded 
-00000f30: 746f 2034 2064 6967 6974 732c 2077 6974  to 4 digits, wit
-00000f40: 6820 7468 6520 6375 7272 656e 7420 7965  h the current ye
-00000f50: 6172 2061 7320 7761 7465 7273 6865 643a  ar as watershed:
-00000f60: 0a20 2020 2020 2020 2020 2020 202d 2033  .            - 3
-00000f70: 302e 342e 3234 202d 3e20 3330 2e30 342e  0.4.24 -> 30.04.
-00000f80: 3230 3234 0a20 2020 2020 2020 2020 2020  2024.           
-00000f90: 202d 2033 302e 342e 3235 202d 3e20 3330   - 30.4.25 -> 30
-00000fa0: 2e30 342e 3139 3235 0a0a 2020 2020 4375  .04.1925..    Cu
-00000fb0: 7272 656e 746c 7920 7375 7070 6f72 7465  rrently supporte
-00000fc0: 6420 6461 7465 2066 6f72 6d61 7473 3a0a  d date formats:.
-00000fd0: 2020 2020 2020 2020 2d20 3034 3736 2d30          - 0476-0
-00000fe0: 392d 3034 202d 3e20 4752 4547 4f52 4941  9-04 -> GREGORIA
-00000ff0: 4e3a 4345 3a30 3437 362d 3039 2d30 343a  N:CE:0476-09-04:
-00001000: 4345 3a30 3437 362d 3039 2d30 340a 2020  CE:0476-09-04.  
-00001010: 2020 2020 2020 2d20 3034 3736 5f30 395f        - 0476_09_
-00001020: 3034 202d 3e20 4752 4547 4f52 4941 4e3a  04 -> GREGORIAN:
-00001030: 4345 3a30 3437 362d 3039 2d30 343a 4345  CE:0476-09-04:CE
-00001040: 3a30 3437 362d 3039 2d30 340a 2020 2020  :0476-09-04.    
-00001050: 2020 2020 2d20 3330 2e34 2e32 3032 3120      - 30.4.2021 
-00001060: 2d3e 2047 5245 474f 5249 414e 3a43 453a  -> GREGORIAN:CE:
-00001070: 3230 3231 2d30 342d 3330 3a43 453a 3230  2021-04-30:CE:20
-00001080: 3231 2d30 342d 3330 0a20 2020 2020 2020  21-04-30.       
-00001090: 202d 2033 302e 342e 3231 202d 3e20 4752   - 30.4.21 -> GR
-000010a0: 4547 4f52 4941 4e3a 4345 3a32 3032 312d  EGORIAN:CE:2021-
-000010b0: 3034 2d33 303a 4345 3a32 3032 312d 3034  04-30:CE:2021-04
-000010c0: 2d33 300a 2020 2020 2020 2020 2d20 352f  -30.        - 5/
-000010d0: 3131 2f32 3032 3120 2d3e 2047 5245 474f  11/2021 -> GREGO
-000010e0: 5249 414e 3a43 453a 3230 3231 2d31 312d  RIAN:CE:2021-11-
-000010f0: 3035 3a43 453a 3230 3231 2d31 312d 3035  05:CE:2021-11-05
-00001100: 0a20 2020 2020 2020 202d 204a 616e 2032  .        - Jan 2
-00001110: 362c 2031 3939 3320 2d3e 2047 5245 474f  6, 1993 -> GREGO
-00001120: 5249 414e 3a43 453a 3139 3933 2d30 312d  RIAN:CE:1993-01-
-00001130: 3236 3a43 453a 3139 3933 2d30 312d 3236  26:CE:1993-01-26
-00001140: 0a20 2020 2020 2020 202d 2032 382e 322e  .        - 28.2.
-00001150: 2d31 2e31 322e 3135 3135 202d 3e20 4752  -1.12.1515 -> GR
-00001160: 4547 4f52 4941 4e3a 4345 3a31 3531 352d  EGORIAN:CE:1515-
-00001170: 3032 2d32 383a 4345 3a31 3531 352d 3132  02-28:CE:1515-12
-00001180: 2d30 310a 2020 2020 2020 2020 2d20 3235  -01.        - 25
-00001190: 2e2d 3236 2e32 2e30 3830 3020 2d3e 2047  .-26.2.0800 -> G
-000011a0: 5245 474f 5249 414e 3a43 453a 3038 3030  REGORIAN:CE:0800
-000011b0: 2d30 322d 3235 3a43 453a 3038 3030 2d30  -02-25:CE:0800-0
-000011c0: 322d 3236 0a20 2020 2020 2020 202d 2031  2-26.        - 1
-000011d0: 2e39 2e32 3032 322d 332e 312e 3230 3234  .9.2022-3.1.2024
-000011e0: 202d 3e20 4752 4547 4f52 4941 4e3a 4345   -> GREGORIAN:CE
-000011f0: 3a32 3032 322d 3039 2d30 313a 4345 3a32  :2022-09-01:CE:2
-00001200: 3032 342d 3031 2d30 330a 2020 2020 2020  024-01-03.      
-00001210: 2020 2d20 3138 3438 202d 3e20 4752 4547    - 1848 -> GREG
-00001220: 4f52 4941 4e3a 4345 3a31 3834 383a 4345  ORIAN:CE:1848:CE
-00001230: 3a31 3834 380a 2020 2020 2020 2020 2d20  :1848.        - 
-00001240: 3138 3439 2f31 3835 3020 2d3e 2047 5245  1849/1850 -> GRE
-00001250: 474f 5249 414e 3a43 453a 3138 3439 3a43  GORIAN:CE:1849:C
-00001260: 453a 3138 3530 0a20 2020 2020 2020 202d  E:1850.        -
-00001270: 2031 3834 392f 3530 202d 3e20 4752 4547   1849/50 -> GREG
-00001280: 4f52 4941 4e3a 4345 3a31 3834 393a 4345  ORIAN:CE:1849:CE
-00001290: 3a31 3835 300a 2020 2020 2020 2020 2d20  :1850.        - 
-000012a0: 3138 3435 2d35 3020 2d3e 2047 5245 474f  1845-50 -> GREGO
-000012b0: 5249 414e 3a43 453a 3138 3435 3a43 453a  RIAN:CE:1845:CE:
-000012c0: 3138 3530 0a20 2020 2020 2020 202d 2038  1850.        - 8
-000012d0: 3430 2d35 3020 2d3e 2047 5245 474f 5249  40-50 -> GREGORI
-000012e0: 414e 3a43 453a 3834 303a 4345 3a38 3530  AN:CE:840:CE:850
-000012f0: 0a20 2020 2020 2020 202d 2038 3430 2d31  .        - 840-1
-00001300: 202d 3e20 4752 4547 4f52 4941 4e3a 4345   -> GREGORIAN:CE
-00001310: 3a38 3430 3a43 453a 3834 310a 2020 2020  :840:CE:841.    
-00001320: 2020 2020 2d20 3130 3030 2d39 3030 2061      - 1000-900 a
-00001330: 762e 204a 2e2d 432e 202d 3e20 4752 4547  v. J.-C. -> GREG
-00001340: 4f52 4941 4e3a 4243 3a31 3030 303a 4243  ORIAN:BC:1000:BC
-00001350: 3a39 3030 0a20 2020 2020 2020 202d 2034  :900.        - 4
-00001360: 3520 6176 2e20 4a2e 2d43 2e20 2d3e 2047  5 av. J.-C. -> G
-00001370: 5245 474f 5249 414e 3a42 433a 3435 3a42  REGORIAN:BC:45:B
-00001380: 433a 3435 0a0a 2020 2020 4172 6773 3a0a  C:45..    Args:.
-00001390: 2020 2020 2020 2020 7374 7269 6e67 3a20          string: 
-000013a0: 7374 7269 6e67 2074 6f20 6368 6563 6b0a  string to check.
-000013b0: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
-000013c0: 2020 2020 2020 4453 502d 666f 726d 6174        DSP-format
-000013d0: 7465 6420 6461 7465 2073 7472 696e 672c  ted date string,
-000013e0: 206f 7220 4e6f 6e65 0a0a 2020 2020 4578   or None..    Ex
-000013f0: 616d 706c 6573 3a0a 2020 2020 2020 2020  amples:.        
-00001400: 3e3e 3e20 6966 2066 696e 645f 6461 7465  >>> if find_date
-00001410: 5f69 6e5f 7374 7269 6e67 2872 6f77 5b22  _in_string(row["
-00001420: 4570 6f63 6822 5d29 3a0a 2020 2020 2020  Epoch"]):.      
-00001430: 2020 3e3e 3e20 2020 2020 7265 736f 7572    >>>     resour
-00001440: 6365 2e61 7070 656e 6428 6d61 6b65 5f64  ce.append(make_d
-00001450: 6174 655f 7072 6f70 2822 3a68 6173 4461  ate_prop(":hasDa
-00001460: 7465 222c 2066 696e 645f 6461 7465 5f69  te", find_date_i
-00001470: 6e5f 7374 7269 6e67 2872 6f77 5b22 4570  n_string(row["Ep
-00001480: 6f63 6822 5d29 290a 0a20 2020 2053 6565  och"]))..    See
-00001490: 2068 7474 7073 3a2f 2f64 6f63 732e 6461   https://docs.da
-000014a0: 7363 682e 7377 6973 732f 6c61 7465 7374  sch.swiss/latest
-000014b0: 2f44 5350 2d54 4f4f 4c53 2f66 696c 652d  /DSP-TOOLS/file-
-000014c0: 666f 726d 6174 732f 786d 6c2d 6461 7461  formats/xml-data
-000014d0: 2d66 696c 652f 2364 6174 652d 7072 6f70  -file/#date-prop
-000014e0: 0a20 2020 2022 2222 0a0a 2020 2020 2320  .    """..    # 
-000014f0: 7361 6e69 7469 7a65 2069 6e70 7574 2c20  sanitize input, 
-00001500: 6a75 7374 2069 6e20 6361 7365 2074 6861  just in case tha
-00001510: 7420 7468 6520 6d65 7468 6f64 2077 6173  t the method was
-00001520: 2063 616c 6c65 6420 6f6e 2061 6e20 656d   called on an em
-00001530: 7074 7920 6f72 204e 2f41 2063 656c 6c0a  pty or N/A cell.
-00001540: 2020 2020 6966 206e 6f74 2063 6865 636b      if not check
-00001550: 5f6e 6f74 6e61 2873 7472 696e 6729 3a0a  _notna(string):.
-00001560: 2020 2020 2020 2020 7265 7475 726e 204e          return N
-00001570: 6f6e 650a 2020 2020 7472 793a 0a20 2020  one.    try:.   
-00001580: 2020 2020 2072 6574 7572 6e20 5f66 696e       return _fin
-00001590: 645f 6461 7465 5f69 6e5f 7374 7269 6e67  d_date_in_string
-000015a0: 5f74 6872 6f77 696e 6728 7374 7269 6e67  _throwing(string
-000015b0: 290a 2020 2020 6578 6365 7074 2056 616c  ).    except Val
-000015c0: 7565 4572 726f 723a 0a20 2020 2020 2020  ueError:.       
-000015d0: 2072 6574 7572 6e20 4e6f 6e65 0a0a 0a5f   return None..._
-000015e0: 6d6f 6e74 6873 5f64 6963 7420 3d20 7b0a  months_dict = {.
-000015f0: 2020 2020 224a 616e 7561 7279 223a 2031      "January": 1
-00001600: 2c0a 2020 2020 224a 616e 223a 2031 2c0a  ,.    "Jan": 1,.
-00001610: 2020 2020 2246 6562 7275 6172 7922 3a20      "February": 
-00001620: 322c 0a20 2020 2022 4665 6222 3a20 322c  2,.    "Feb": 2,
-00001630: 0a20 2020 2022 4d61 7263 6822 3a20 332c  .    "March": 3,
-00001640: 0a20 2020 2022 4d61 7222 3a20 332c 0a20  .    "Mar": 3,. 
-00001650: 2020 2022 4170 7269 6c22 3a20 342c 0a20     "April": 4,. 
-00001660: 2020 2022 4170 7222 3a20 342c 0a20 2020     "Apr": 4,.   
-00001670: 2022 4d61 7922 3a20 352c 0a20 2020 2022   "May": 5,.    "
-00001680: 4a75 6e65 223a 2036 2c0a 2020 2020 224a  June": 6,.    "J
-00001690: 756e 223a 2036 2c0a 2020 2020 224a 756c  un": 6,.    "Jul
-000016a0: 7922 3a20 372c 0a20 2020 2022 4a75 6c22  y": 7,.    "Jul"
-000016b0: 3a20 372c 0a20 2020 2022 4175 6775 7374  : 7,.    "August
-000016c0: 223a 2038 2c0a 2020 2020 2241 7567 223a  ": 8,.    "Aug":
-000016d0: 2038 2c0a 2020 2020 2253 6570 7465 6d62   8,.    "Septemb
-000016e0: 6572 223a 2039 2c0a 2020 2020 2253 6570  er": 9,.    "Sep
-000016f0: 7422 3a20 392c 0a20 2020 2022 4f63 746f  t": 9,.    "Octo
-00001700: 6265 7222 3a20 3130 2c0a 2020 2020 224f  ber": 10,.    "O
-00001710: 6374 223a 2031 302c 0a20 2020 2022 4e6f  ct": 10,.    "No
-00001720: 7665 6d62 6572 223a 2031 312c 0a20 2020  vember": 11,.   
-00001730: 2022 4e6f 7622 3a20 3131 2c0a 2020 2020   "Nov": 11,.    
-00001740: 2244 6563 656d 6265 7222 3a20 3132 2c0a  "December": 12,.
-00001750: 2020 2020 2244 6563 223a 2031 322c 0a7d      "Dec": 12,.}
-00001760: 0a0a 0a64 6566 205f 6669 6e64 5f64 6174  ...def _find_dat
-00001770: 655f 696e 5f73 7472 696e 675f 7468 726f  e_in_string_thro
-00001780: 7769 6e67 2873 7472 696e 673a 2073 7472  wing(string: str
-00001790: 2920 2d3e 2073 7472 207c 204e 6f6e 653a  ) -> str | None:
-000017a0: 0a20 2020 2022 2222 0a20 2020 2054 6869  .    """.    Thi
-000017b0: 7320 6675 6e63 7469 6f6e 2069 7320 7468  s function is th
-000017c0: 6520 7361 6d65 2061 7320 6669 6e64 5f64  e same as find_d
-000017d0: 6174 655f 696e 5f73 7472 696e 6728 292c  ate_in_string(),
-000017e0: 2062 7574 206d 6179 2072 6169 7365 2061   but may raise a
-000017f0: 2056 616c 7565 4572 726f 7220 696e 7374   ValueError inst
-00001800: 6561 6420 6f66 2072 6574 7572 6e69 6e67  ead of returning
-00001810: 204e 6f6e 652e 0a20 2020 2022 2222 0a20   None..    """. 
-00001820: 2020 2079 6561 725f 7265 6765 7820 3d20     year_regex = 
-00001830: 7222 285b 302d 325d 3f5b 302d 395d 5b30  r"([0-2]?[0-9][0
-00001840: 2d39 5d5b 302d 395d 2922 0a20 2020 2079  -9][0-9])".    y
-00001850: 6561 725f 7265 6765 785f 325f 6f72 5f34  ear_regex_2_or_4
-00001860: 5f64 6967 6974 7320 3d20 7222 2828 3f3a  _digits = r"((?:
-00001870: 5b30 2d32 5d3f 5b30 2d39 5d29 3f5b 302d  [0-2]?[0-9])?[0-
-00001880: 395d 5b30 2d39 5d29 220a 2020 2020 6d6f  9][0-9])".    mo
-00001890: 6e74 685f 7265 6765 7820 3d20 7222 285b  nth_regex = r"([
-000018a0: 302d 315d 3f5b 302d 395d 2922 0a20 2020  0-1]?[0-9])".   
-000018b0: 2064 6179 5f72 6567 6578 203d 2072 2228   day_regex = r"(
-000018c0: 5b30 2d33 5d3f 5b30 2d39 5d29 220a 2020  [0-3]?[0-9])".  
-000018d0: 2020 7365 705f 7265 6765 7820 3d20 7222    sep_regex = r"
-000018e0: 5b5c 2e2f 5d22 0a20 2020 206c 6f6f 6b62  [\./]".    lookb
-000018f0: 6568 696e 6420 3d20 7222 283f 3c21 5b30  ehind = r"(?<![0
-00001900: 2d39 412d 5a61 2d7a 5d29 220a 2020 2020  -9A-Za-z])".    
-00001910: 6c6f 6f6b 6168 6561 6420 3d20 7222 283f  lookahead = r"(?
-00001920: 215b 302d 3941 2d5a 612d 7a5d 2922 0a0a  ![0-9A-Za-z])"..
-00001930: 2020 2020 6966 2066 7265 6e63 685f 6263      if french_bc
-00001940: 5f64 6174 6520 3a3d 205f 6669 6e64 5f66  _date := _find_f
-00001950: 7265 6e63 685f 6263 5f64 6174 6528 7374  rench_bc_date(st
-00001960: 7269 6e67 3d73 7472 696e 672c 206c 6f6f  ring=string, loo
-00001970: 6b62 6568 696e 643d 6c6f 6f6b 6265 6869  kbehind=lookbehi
-00001980: 6e64 2c20 6c6f 6f6b 6168 6561 643d 6c6f  nd, lookahead=lo
-00001990: 6f6b 6168 6561 6429 3a0a 2020 2020 2020  okahead):.      
-000019a0: 2020 7265 7475 726e 2066 7265 6e63 685f    return french_
-000019b0: 6263 5f64 6174 650a 0a20 2020 2023 2074  bc_date..    # t
-000019c0: 656d 706c 6174 653a 2032 3032 312d 3031  emplate: 2021-01
-000019d0: 2d30 3120 7c20 3230 3135 5f30 315f 3032  -01 | 2015_01_02
-000019e0: 0a20 2020 2069 736f 5f64 6174 6520 3d20  .    iso_date = 
-000019f0: 7265 6765 782e 7365 6172 6368 2872 6622  regex.search(rf"
-00001a00: 7b6c 6f6f 6b62 6568 696e 647d 7b79 6561  {lookbehind}{yea
-00001a10: 725f 7265 6765 787d 5b5f 2d5d 285b 302d  r_regex}[_-]([0-
-00001a20: 315d 5b30 2d39 5d29 5b5f 2d5d 285b 302d  1][0-9])[_-]([0-
-00001a30: 335d 5b30 2d39 5d29 7b6c 6f6f 6b61 6865  3][0-9]){lookahe
-00001a40: 6164 7d22 2c20 7374 7269 6e67 290a 0a20  ad}", string).. 
-00001a50: 2020 2023 2074 656d 706c 6174 653a 2036     # template: 6
-00001a60: 2e2d 382e 332e 3139 3438 207c 2036 2f32  .-8.3.1948 | 6/2
-00001a70: 2f31 3934 3720 2d20 3234 2e30 332e 3139  /1947 - 24.03.19
-00001a80: 3438 0a20 2020 2065 7572 5f64 6174 655f  48.    eur_date_
-00001a90: 7261 6e67 655f 7265 6765 7820 3d20 280a  range_regex = (.
-00001aa0: 2020 2020 2020 2020 7266 227b 6c6f 6f6b          rf"{look
-00001ab0: 6265 6869 6e64 7d22 0a20 2020 2020 2020  behind}".       
-00001ac0: 2072 6622 7b64 6179 5f72 6567 6578 7d7b   rf"{day_regex}{
-00001ad0: 7365 705f 7265 6765 787d 283f 3a7b 6d6f  sep_regex}(?:{mo
-00001ae0: 6e74 685f 7265 6765 787d 7b73 6570 5f72  nth_regex}{sep_r
-00001af0: 6567 6578 7d7b 7965 6172 5f72 6567 6578  egex}{year_regex
-00001b00: 5f32 5f6f 725f 345f 6469 6769 7473 7d3f  _2_or_4_digits}?
-00001b10: 293f 203f 283f 3a2d 7c3a 7c74 6f29 203f  )? ?(?:-|:|to) ?
-00001b20: 220a 2020 2020 2020 2020 7266 227b 6461  ".        rf"{da
-00001b30: 795f 7265 6765 787d 7b73 6570 5f72 6567  y_regex}{sep_reg
-00001b40: 6578 7d7b 6d6f 6e74 685f 7265 6765 787d  ex}{month_regex}
-00001b50: 7b73 6570 5f72 6567 6578 7d7b 7965 6172  {sep_regex}{year
-00001b60: 5f72 6567 6578 5f32 5f6f 725f 345f 6469  _regex_2_or_4_di
-00001b70: 6769 7473 7d22 0a20 2020 2020 2020 2072  gits}".        r
-00001b80: 6622 7b6c 6f6f 6b61 6865 6164 7d22 0a20  f"{lookahead}". 
-00001b90: 2020 2029 0a20 2020 2065 7572 5f64 6174     ).    eur_dat
-00001ba0: 655f 7261 6e67 6520 3d20 7265 6765 782e  e_range = regex.
-00001bb0: 7365 6172 6368 2865 7572 5f64 6174 655f  search(eur_date_
-00001bc0: 7261 6e67 655f 7265 6765 782c 2073 7472  range_regex, str
-00001bd0: 696e 6729 0a0a 2020 2020 2320 7465 6d70  ing)..    # temp
-00001be0: 6c61 7465 3a20 312e 342e 3230 3231 207c  late: 1.4.2021 |
-00001bf0: 2035 2f31 312f 3230 3231 0a20 2020 2065   5/11/2021.    e
-00001c00: 7572 5f64 6174 655f 7265 6765 7820 3d20  ur_date_regex = 
-00001c10: 7266 227b 6c6f 6f6b 6265 6869 6e64 7d7b  rf"{lookbehind}{
-00001c20: 6461 795f 7265 6765 787d 7b73 6570 5f72  day_regex}{sep_r
-00001c30: 6567 6578 7d7b 6d6f 6e74 685f 7265 6765  egex}{month_rege
-00001c40: 787d 7b73 6570 5f72 6567 6578 7d7b 7965  x}{sep_regex}{ye
-00001c50: 6172 5f72 6567 6578 5f32 5f6f 725f 345f  ar_regex_2_or_4_
-00001c60: 6469 6769 7473 7d7b 6c6f 6f6b 6168 6561  digits}{lookahea
-00001c70: 647d 220a 2020 2020 6575 725f 6461 7465  d}".    eur_date
-00001c80: 203d 2072 6567 6578 2e73 6561 7263 6828   = regex.search(
-00001c90: 0a20 2020 2020 2020 2065 7572 5f64 6174  .        eur_dat
-00001ca0: 655f 7265 6765 782c 0a20 2020 2020 2020  e_regex,.       
-00001cb0: 2073 7472 696e 672c 0a20 2020 2029 0a0a   string,.    )..
-00001cc0: 2020 2020 2320 7465 6d70 6c61 7465 3a20      # template: 
-00001cd0: 4d61 7263 6820 392c 2031 3930 3820 7c20  March 9, 1908 | 
-00001ce0: 4d61 7263 6835 2c31 3930 3820 7c20 4d61  March5,1908 | Ma
-00001cf0: 7920 3131 2c20 3139 3036 0a20 2020 2061  y 11, 1906.    a
-00001d00: 6c6c 5f6d 6f6e 7468 7320 3d20 227c 222e  ll_months = "|".
-00001d10: 6a6f 696e 285f 6d6f 6e74 6873 5f64 6963  join(_months_dic
-00001d20: 7429 0a20 2020 206d 6f6e 7468 6e61 6d65  t).    monthname
-00001d30: 5f64 6174 655f 7265 6765 7820 3d20 7266  _date_regex = rf
-00001d40: 227b 6c6f 6f6b 6265 6869 6e64 7d28 7b61  "{lookbehind}({a
-00001d50: 6c6c 5f6d 6f6e 7468 737d 2920 3f7b 6461  ll_months}) ?{da
-00001d60: 795f 7265 6765 787d 2c20 3f7b 7965 6172  y_regex}, ?{year
-00001d70: 5f72 6567 6578 7d7b 6c6f 6f6b 6168 6561  _regex}{lookahea
-00001d80: 647d 220a 2020 2020 6d6f 6e74 686e 616d  d}".    monthnam
-00001d90: 655f 6461 7465 203d 2072 6567 6578 2e73  e_date = regex.s
-00001da0: 6561 7263 6828 6d6f 6e74 686e 616d 655f  earch(monthname_
-00001db0: 6461 7465 5f72 6567 6578 2c20 7374 7269  date_regex, stri
-00001dc0: 6e67 290a 0a20 2020 2023 2074 656d 706c  ng)..    # templ
-00001dd0: 6174 653a 2031 3834 392f 3530 207c 2031  ate: 1849/50 | 1
-00001de0: 3834 392d 3530 207c 2031 3834 392f 3138  849-50 | 1849/18
-00001df0: 3530 0a20 2020 2079 6561 725f 7261 6e67  50.    year_rang
-00001e00: 6520 3d20 7265 6765 782e 7365 6172 6368  e = regex.search
-00001e10: 286c 6f6f 6b62 6568 696e 6420 2b20 7965  (lookbehind + ye
-00001e20: 6172 5f72 6567 6578 202b 2072 225b 2f2d  ar_regex + r"[/-
-00001e30: 5d28 5c64 7b31 2c34 7d29 2220 2b20 6c6f  ](\d{1,4})" + lo
-00001e40: 6f6b 6168 6561 642c 2073 7472 696e 6729  okahead, string)
-00001e50: 0a0a 2020 2020 2320 7465 6d70 6c61 7465  ..    # template
-00001e60: 3a20 3139 3037 0a20 2020 2079 6561 725f  : 1907.    year_
-00001e70: 6f6e 6c79 203d 2072 6567 6578 2e73 6561  only = regex.sea
-00001e80: 7263 6828 7266 227b 6c6f 6f6b 6265 6869  rch(rf"{lookbehi
-00001e90: 6e64 7d7b 7965 6172 5f72 6567 6578 7d7b  nd}{year_regex}{
-00001ea0: 6c6f 6f6b 6168 6561 647d 222c 2073 7472  lookahead}", str
-00001eb0: 696e 6729 0a0a 2020 2020 7265 733a 2073  ing)..    res: s
-00001ec0: 7472 207c 204e 6f6e 6520 3d20 4e6f 6e65  tr | None = None
-00001ed0: 0a20 2020 2069 6620 6973 6f5f 6461 7465  .    if iso_date
-00001ee0: 3a0a 2020 2020 2020 2020 7265 7320 3d20  :.        res = 
-00001ef0: 5f66 726f 6d5f 6973 6f5f 6461 7465 2869  _from_iso_date(i
-00001f00: 736f 5f64 6174 6529 0a20 2020 2065 6c69  so_date).    eli
-00001f10: 6620 6575 725f 6461 7465 5f72 616e 6765  f eur_date_range
-00001f20: 3a0a 2020 2020 2020 2020 7265 7320 3d20  :.        res = 
-00001f30: 5f66 726f 6d5f 6575 725f 6461 7465 5f72  _from_eur_date_r
-00001f40: 616e 6765 2865 7572 5f64 6174 655f 7261  ange(eur_date_ra
-00001f50: 6e67 6529 0a20 2020 2065 6c69 6620 6575  nge).    elif eu
-00001f60: 725f 6461 7465 3a0a 2020 2020 2020 2020  r_date:.        
-00001f70: 7265 7320 3d20 5f66 726f 6d5f 6575 725f  res = _from_eur_
-00001f80: 6461 7465 2865 7572 5f64 6174 6529 0a20  date(eur_date). 
-00001f90: 2020 2065 6c69 6620 6d6f 6e74 686e 616d     elif monthnam
-00001fa0: 655f 6461 7465 3a0a 2020 2020 2020 2020  e_date:.        
-00001fb0: 7265 7320 3d20 5f66 726f 6d5f 6d6f 6e74  res = _from_mont
-00001fc0: 686e 616d 655f 6461 7465 286d 6f6e 7468  hname_date(month
-00001fd0: 6e61 6d65 5f64 6174 6529 0a20 2020 2065  name_date).    e
-00001fe0: 6c69 6620 7965 6172 5f72 616e 6765 3a0a  lif year_range:.
-00001ff0: 2020 2020 2020 2020 7265 7320 3d20 5f66          res = _f
-00002000: 726f 6d5f 7965 6172 5f72 616e 6765 2879  rom_year_range(y
-00002010: 6561 725f 7261 6e67 6529 0a20 2020 2065  ear_range).    e
-00002020: 6c69 6620 7965 6172 5f6f 6e6c 793a 0a20  lif year_only:. 
-00002030: 2020 2020 2020 2079 6561 7220 3d20 696e         year = in
-00002040: 7428 7965 6172 5f6f 6e6c 792e 6772 6f75  t(year_only.grou
-00002050: 7028 3029 290a 2020 2020 2020 2020 7265  p(0)).        re
-00002060: 7320 3d20 6622 4752 4547 4f52 4941 4e3a  s = f"GREGORIAN:
-00002070: 4345 3a7b 7965 6172 7d3a 4345 3a7b 7965  CE:{year}:CE:{ye
-00002080: 6172 7d22 0a20 2020 2072 6574 7572 6e20  ar}".    return 
-00002090: 7265 730a 0a0a 6465 6620 5f66 726f 6d5f  res...def _from_
-000020a0: 6973 6f5f 6461 7465 2869 736f 5f64 6174  iso_date(iso_dat
-000020b0: 653a 204d 6174 6368 5b73 7472 5d29 202d  e: Match[str]) -
-000020c0: 3e20 7374 723a 0a20 2020 2079 6561 7220  > str:.    year 
-000020d0: 3d20 696e 7428 6973 6f5f 6461 7465 2e67  = int(iso_date.g
-000020e0: 726f 7570 2831 2929 0a20 2020 206d 6f6e  roup(1)).    mon
-000020f0: 7468 203d 2069 6e74 2869 736f 5f64 6174  th = int(iso_dat
-00002100: 652e 6772 6f75 7028 3229 290a 2020 2020  e.group(2)).    
-00002110: 6461 7920 3d20 696e 7428 6973 6f5f 6461  day = int(iso_da
-00002120: 7465 2e67 726f 7570 2833 2929 0a20 2020  te.group(3)).   
-00002130: 2064 6174 6520 3d20 6461 7465 7469 6d65   date = datetime
-00002140: 2e64 6174 6528 7965 6172 2c20 6d6f 6e74  .date(year, mont
-00002150: 682c 2064 6179 290a 2020 2020 7265 7475  h, day).    retu
-00002160: 726e 2066 2247 5245 474f 5249 414e 3a43  rn f"GREGORIAN:C
-00002170: 453a 7b64 6174 652e 6973 6f66 6f72 6d61  E:{date.isoforma
-00002180: 7428 297d 3a43 453a 7b64 6174 652e 6973  t()}:CE:{date.is
-00002190: 6f66 6f72 6d61 7428 297d 220a 0a0a 6465  oformat()}"...de
-000021a0: 6620 5f65 7870 616e 645f 325f 6469 6769  f _expand_2_digi
-000021b0: 745f 7965 6172 2879 6561 723a 2069 6e74  t_year(year: int
-000021c0: 2920 2d3e 2069 6e74 3a0a 2020 2020 6375  ) -> int:.    cu
-000021d0: 7272 656e 745f 7965 6172 203d 2064 6174  rrent_year = dat
-000021e0: 6574 696d 652e 6461 7465 2e74 6f64 6179  etime.date.today
-000021f0: 2829 2e79 6561 7220 2d20 3230 3030 0a20  ().year - 2000. 
-00002200: 2020 2069 6620 7965 6172 203c 3d20 6375     if year <= cu
-00002210: 7272 656e 745f 7965 6172 3a0a 2020 2020  rrent_year:.    
-00002220: 2020 2020 7265 7475 726e 2079 6561 7220      return year 
-00002230: 2b20 3230 3030 0a20 2020 2065 6c69 6620  + 2000.    elif 
-00002240: 7965 6172 203c 3d20 3939 3a0a 2020 2020  year <= 99:.    
-00002250: 2020 2020 7265 7475 726e 2079 6561 7220      return year 
-00002260: 2b20 3139 3030 0a20 2020 2065 6c73 653a  + 1900.    else:
-00002270: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00002280: 7965 6172 0a0a 0a64 6566 205f 6672 6f6d  year...def _from
-00002290: 5f65 7572 5f64 6174 655f 7261 6e67 6528  _eur_date_range(
-000022a0: 6575 725f 6461 7465 5f72 616e 6765 3a20  eur_date_range: 
-000022b0: 4d61 7463 685b 7374 725d 2920 2d3e 2073  Match[str]) -> s
-000022c0: 7472 3a0a 2020 2020 7374 6172 7464 6179  tr:.    startday
-000022d0: 203d 2069 6e74 2865 7572 5f64 6174 655f   = int(eur_date_
-000022e0: 7261 6e67 652e 6772 6f75 7028 3129 290a  range.group(1)).
-000022f0: 2020 2020 7374 6172 746d 6f6e 7468 203d      startmonth =
-00002300: 2069 6e74 2865 7572 5f64 6174 655f 7261   int(eur_date_ra
-00002310: 6e67 652e 6772 6f75 7028 3229 2920 6966  nge.group(2)) if
-00002320: 2065 7572 5f64 6174 655f 7261 6e67 652e   eur_date_range.
-00002330: 6772 6f75 7028 3229 2065 6c73 6520 696e  group(2) else in
-00002340: 7428 6575 725f 6461 7465 5f72 616e 6765  t(eur_date_range
-00002350: 2e67 726f 7570 2835 2929 0a20 2020 2073  .group(5)).    s
-00002360: 7461 7274 7965 6172 203d 2069 6e74 2865  tartyear = int(e
-00002370: 7572 5f64 6174 655f 7261 6e67 652e 6772  ur_date_range.gr
-00002380: 6f75 7028 3329 2920 6966 2065 7572 5f64  oup(3)) if eur_d
-00002390: 6174 655f 7261 6e67 652e 6772 6f75 7028  ate_range.group(
-000023a0: 3329 2065 6c73 6520 696e 7428 6575 725f  3) else int(eur_
-000023b0: 6461 7465 5f72 616e 6765 2e67 726f 7570  date_range.group
-000023c0: 2836 2929 0a20 2020 2073 7461 7274 7965  (6)).    startye
-000023d0: 6172 203d 205f 6578 7061 6e64 5f32 5f64  ar = _expand_2_d
-000023e0: 6967 6974 5f79 6561 7228 7374 6172 7479  igit_year(starty
-000023f0: 6561 7229 0a20 2020 2065 6e64 6461 7920  ear).    endday 
-00002400: 3d20 696e 7428 6575 725f 6461 7465 5f72  = int(eur_date_r
-00002410: 616e 6765 2e67 726f 7570 2834 2929 0a20  ange.group(4)). 
-00002420: 2020 2065 6e64 6d6f 6e74 6820 3d20 696e     endmonth = in
-00002430: 7428 6575 725f 6461 7465 5f72 616e 6765  t(eur_date_range
-00002440: 2e67 726f 7570 2835 2929 0a20 2020 2065  .group(5)).    e
-00002450: 6e64 7965 6172 203d 2069 6e74 2865 7572  ndyear = int(eur
-00002460: 5f64 6174 655f 7261 6e67 652e 6772 6f75  _date_range.grou
-00002470: 7028 3629 290a 2020 2020 656e 6479 6561  p(6)).    endyea
-00002480: 7220 3d20 5f65 7870 616e 645f 325f 6469  r = _expand_2_di
-00002490: 6769 745f 7965 6172 2865 6e64 7965 6172  git_year(endyear
-000024a0: 290a 2020 2020 7374 6172 7464 6174 6520  ).    startdate 
-000024b0: 3d20 6461 7465 7469 6d65 2e64 6174 6528  = datetime.date(
-000024c0: 7374 6172 7479 6561 722c 2073 7461 7274  startyear, start
-000024d0: 6d6f 6e74 682c 2073 7461 7274 6461 7929  month, startday)
-000024e0: 0a20 2020 2065 6e64 6461 7465 203d 2064  .    enddate = d
-000024f0: 6174 6574 696d 652e 6461 7465 2865 6e64  atetime.date(end
-00002500: 7965 6172 2c20 656e 646d 6f6e 7468 2c20  year, endmonth, 
-00002510: 656e 6464 6179 290a 2020 2020 6966 2065  endday).    if e
-00002520: 6e64 6461 7465 203c 2073 7461 7274 6461  nddate < startda
-00002530: 7465 3a0a 2020 2020 2020 2020 7261 6973  te:.        rais
-00002540: 6520 5661 6c75 6545 7272 6f72 0a20 2020  e ValueError.   
-00002550: 2072 6574 7572 6e20 6622 4752 4547 4f52   return f"GREGOR
-00002560: 4941 4e3a 4345 3a7b 7374 6172 7464 6174  IAN:CE:{startdat
-00002570: 652e 6973 6f66 6f72 6d61 7428 297d 3a43  e.isoformat()}:C
-00002580: 453a 7b65 6e64 6461 7465 2e69 736f 666f  E:{enddate.isofo
-00002590: 726d 6174 2829 7d22 0a0a 0a64 6566 205f  rmat()}"...def _
-000025a0: 6672 6f6d 5f65 7572 5f64 6174 6528 6575  from_eur_date(eu
-000025b0: 725f 6461 7465 3a20 4d61 7463 685b 7374  r_date: Match[st
-000025c0: 725d 2920 2d3e 2073 7472 3a0a 2020 2020  r]) -> str:.    
-000025d0: 7374 6172 7464 6179 203d 2069 6e74 2865  startday = int(e
-000025e0: 7572 5f64 6174 652e 6772 6f75 7028 3129  ur_date.group(1)
-000025f0: 290a 2020 2020 7374 6172 746d 6f6e 7468  ).    startmonth
-00002600: 203d 2069 6e74 2865 7572 5f64 6174 652e   = int(eur_date.
-00002610: 6772 6f75 7028 3229 290a 2020 2020 7374  group(2)).    st
-00002620: 6172 7479 6561 7220 3d20 696e 7428 6575  artyear = int(eu
-00002630: 725f 6461 7465 2e67 726f 7570 2833 2929  r_date.group(3))
-00002640: 0a20 2020 2073 7461 7274 7965 6172 203d  .    startyear =
-00002650: 205f 6578 7061 6e64 5f32 5f64 6967 6974   _expand_2_digit
-00002660: 5f79 6561 7228 7374 6172 7479 6561 7229  _year(startyear)
-00002670: 0a20 2020 2064 6174 6520 3d20 6461 7465  .    date = date
-00002680: 7469 6d65 2e64 6174 6528 7374 6172 7479  time.date(starty
-00002690: 6561 722c 2073 7461 7274 6d6f 6e74 682c  ear, startmonth,
-000026a0: 2073 7461 7274 6461 7929 0a20 2020 2072   startday).    r
-000026b0: 6574 7572 6e20 6622 4752 4547 4f52 4941  eturn f"GREGORIA
-000026c0: 4e3a 4345 3a7b 6461 7465 2e69 736f 666f  N:CE:{date.isofo
-000026d0: 726d 6174 2829 7d3a 4345 3a7b 6461 7465  rmat()}:CE:{date
-000026e0: 2e69 736f 666f 726d 6174 2829 7d22 0a0a  .isoformat()}"..
-000026f0: 0a64 6566 205f 6672 6f6d 5f6d 6f6e 7468  .def _from_month
-00002700: 6e61 6d65 5f64 6174 6528 6d6f 6e74 686e  name_date(monthn
-00002710: 616d 655f 6461 7465 3a20 4d61 7463 685b  ame_date: Match[
-00002720: 7374 725d 2920 2d3e 2073 7472 3a0a 2020  str]) -> str:.  
-00002730: 2020 6461 7920 3d20 696e 7428 6d6f 6e74    day = int(mont
-00002740: 686e 616d 655f 6461 7465 2e67 726f 7570  hname_date.group
-00002750: 2832 2929 0a20 2020 206d 6f6e 7468 203d  (2)).    month =
-00002760: 205f 6d6f 6e74 6873 5f64 6963 745b 6d6f   _months_dict[mo
-00002770: 6e74 686e 616d 655f 6461 7465 2e67 726f  nthname_date.gro
-00002780: 7570 2831 295d 0a20 2020 2079 6561 7220  up(1)].    year 
-00002790: 3d20 696e 7428 6d6f 6e74 686e 616d 655f  = int(monthname_
-000027a0: 6461 7465 2e67 726f 7570 2833 2929 0a20  date.group(3)). 
-000027b0: 2020 2064 6174 6520 3d20 6461 7465 7469     date = dateti
-000027c0: 6d65 2e64 6174 6528 7965 6172 2c20 6d6f  me.date(year, mo
-000027d0: 6e74 682c 2064 6179 290a 2020 2020 7265  nth, day).    re
-000027e0: 7475 726e 2066 2247 5245 474f 5249 414e  turn f"GREGORIAN
-000027f0: 3a43 453a 7b64 6174 652e 6973 6f66 6f72  :CE:{date.isofor
-00002800: 6d61 7428 297d 3a43 453a 7b64 6174 652e  mat()}:CE:{date.
-00002810: 6973 6f66 6f72 6d61 7428 297d 220a 0a0a  isoformat()}"...
-00002820: 6465 6620 5f66 726f 6d5f 7965 6172 5f72  def _from_year_r
-00002830: 616e 6765 2879 6561 725f 7261 6e67 653a  ange(year_range:
-00002840: 204d 6174 6368 5b73 7472 5d29 202d 3e20   Match[str]) -> 
-00002850: 7374 723a 0a20 2020 2073 7461 7274 7965  str:.    startye
-00002860: 6172 203d 2069 6e74 2879 6561 725f 7261  ar = int(year_ra
-00002870: 6e67 652e 6772 6f75 7028 3129 290a 2020  nge.group(1)).  
-00002880: 2020 656e 6479 6561 7220 3d20 696e 7428    endyear = int(
-00002890: 7965 6172 5f72 616e 6765 2e67 726f 7570  year_range.group
-000028a0: 2832 2929 0a20 2020 2069 6620 656e 6479  (2)).    if endy
-000028b0: 6561 7220 2f2f 2031 3020 3d3d 2030 3a0a  ear // 10 == 0:.
-000028c0: 2020 2020 2020 2020 2320 656e 6479 6561          # endyea
-000028d0: 7220 6973 206f 6e6c 7920 312d 6469 6769  r is only 1-digi
-000028e0: 743a 2061 6464 2074 6865 2066 6972 7374  t: add the first
-000028f0: 2032 2d33 2064 6967 6974 7320 6f66 2073   2-3 digits of s
-00002900: 7461 7274 7965 6172 0a20 2020 2020 2020  tartyear.       
-00002910: 2065 6e64 7965 6172 203d 2073 7461 7274   endyear = start
-00002920: 7965 6172 202f 2f20 3130 202a 2031 3020  year // 10 * 10 
-00002930: 2b20 656e 6479 6561 720a 2020 2020 656c  + endyear.    el
-00002940: 6966 2065 6e64 7965 6172 202f 2f20 3130  if endyear // 10
-00002950: 3020 3d3d 2030 3a0a 2020 2020 2020 2020  0 == 0:.        
-00002960: 2320 656e 6479 6561 7220 6973 206f 6e6c  # endyear is onl
-00002970: 7920 322d 6469 6769 743a 2061 6464 2074  y 2-digit: add t
-00002980: 6865 2066 6972 7374 2031 2d32 2064 6967  he first 1-2 dig
-00002990: 6974 7320 6f66 2073 7461 7274 7965 6172  its of startyear
-000029a0: 0a20 2020 2020 2020 2065 6e64 7965 6172  .        endyear
-000029b0: 203d 2073 7461 7274 7965 6172 202f 2f20   = startyear // 
-000029c0: 3130 3020 2a20 3130 3020 2b20 656e 6479  100 * 100 + endy
-000029d0: 6561 720a 2020 2020 6966 2065 6e64 7965  ear.    if endye
-000029e0: 6172 203c 3d20 7374 6172 7479 6561 723a  ar <= startyear:
-000029f0: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
-00002a00: 616c 7565 4572 726f 720a 2020 2020 7265  alueError.    re
-00002a10: 7475 726e 2066 2247 5245 474f 5249 414e  turn f"GREGORIAN
-00002a20: 3a43 453a 7b73 7461 7274 7965 6172 7d3a  :CE:{startyear}:
-00002a30: 4345 3a7b 656e 6479 6561 727d 220a 0a0a  CE:{endyear}"...
-00002a40: 6465 6620 7072 6570 6172 655f 7661 6c75  def prepare_valu
-00002a50: 6528 0a20 2020 2076 616c 7565 3a20 556e  e(.    value: Un
-00002a60: 696f 6e5b 5072 6f70 6572 7479 456c 656d  ion[PropertyElem
-00002a70: 656e 742c 2073 7472 2c20 696e 742c 2066  ent, str, int, f
-00002a80: 6c6f 6174 2c20 626f 6f6c 2c20 4974 6572  loat, bool, Iter
-00002a90: 6162 6c65 5b55 6e69 6f6e 5b50 726f 7065  able[Union[Prope
-00002aa0: 7274 7945 6c65 6d65 6e74 2c20 7374 722c  rtyElement, str,
-00002ab0: 2069 6e74 2c20 666c 6f61 742c 2062 6f6f   int, float, boo
-00002ac0: 6c5d 5d5d 2c0a 2920 2d3e 206c 6973 745b  l]]],.) -> list[
-00002ad0: 5072 6f70 6572 7479 456c 656d 656e 745d  PropertyElement]
-00002ae0: 3a0a 2020 2020 2222 220a 2020 2020 5468  :.    """.    Th
-00002af0: 6973 206d 6574 686f 6420 7472 616e 7366  is method transf
-00002b00: 6f72 6d73 2074 6865 2070 6172 616d 6574  orms the paramet
-00002b10: 6572 2022 7661 6c75 6522 2066 726f 6d20  er "value" from 
-00002b20: 6120 6d61 6b65 5f2a 5f70 726f 7028 2920  a make_*_prop() 
-00002b30: 6d65 7468 6f64 2069 6e74 6f20 6120 6c69  method into a li
-00002b40: 7374 206f 6620 5072 6f70 6572 7479 456c  st of PropertyEl
-00002b50: 656d 656e 7473 2e20 2276 616c 7565 2220  ements. "value" 
-00002b60: 6973 0a20 2020 2070 6173 7365 6420 6f6e  is.    passed on
-00002b70: 2074 6f20 7468 6973 206d 6574 686f 6420   to this method 
-00002b80: 6173 2069 7420 7761 7320 7265 6365 6976  as it was receiv
-00002b90: 6564 2e0a 0a20 2020 2041 7267 733a 0a20  ed...    Args:. 
-00002ba0: 2020 2020 2020 2076 616c 7565 3a20 2276         value: "v
-00002bb0: 616c 7565 2220 6173 2072 6563 6569 7665  alue" as receive
-00002bc0: 6420 6672 6f6d 2074 6865 2063 616c 6c65  d from the calle
-00002bd0: 720a 0a20 2020 2052 6574 7572 6e73 3a0a  r..    Returns:.
-00002be0: 2020 2020 2020 2020 6120 6c69 7374 206f          a list o
-00002bf0: 6620 5072 6f70 6572 7479 456c 656d 656e  f PropertyElemen
-00002c00: 7473 0a20 2020 2022 2222 0a20 2020 2023  ts.    """.    #
-00002c10: 206d 616b 6520 7375 7265 2074 6861 7420   make sure that 
-00002c20: 2276 616c 7565 2220 6973 206c 6973 742d  "value" is list-
-00002c30: 6c69 6b65 0a20 2020 2069 6620 6e6f 7420  like.    if not 
-00002c40: 6973 696e 7374 616e 6365 2876 616c 7565  isinstance(value
-00002c50: 2c20 4974 6572 6162 6c65 2920 6f72 2069  , Iterable) or i
-00002c60: 7369 6e73 7461 6e63 6528 7661 6c75 652c  sinstance(value,
-00002c70: 2073 7472 293a 0a20 2020 2020 2020 2076   str):.        v
-00002c80: 616c 7565 203d 205b 7661 6c75 655d 0a0a  alue = [value]..
-00002c90: 2020 2020 2320 6d61 6b65 2061 2050 726f      # make a Pro
-00002ca0: 7065 7274 7945 6c65 6d65 6e74 206f 7574  pertyElement out
-00002cb0: 206f 6620 6974 7320 656c 656d 656e 7473   of its elements
-00002cc0: 2c20 6966 206e 6563 6573 7361 7279 2e0a  , if necessary..
-00002cd0: 2020 2020 7265 7475 726e 205b 7820 6966      return [x if
-00002ce0: 2069 7369 6e73 7461 6e63 6528 782c 2050   isinstance(x, P
-00002cf0: 726f 7065 7274 7945 6c65 6d65 6e74 2920  ropertyElement) 
-00002d00: 656c 7365 2050 726f 7065 7274 7945 6c65  else PropertyEle
-00002d10: 6d65 6e74 2878 2920 666f 7220 7820 696e  ment(x) for x in
-00002d20: 2076 616c 7565 5d0a 0a0a 6465 6620 6d61   value]...def ma
-00002d30: 6b65 5f72 6f6f 7428 0a20 2020 2073 686f  ke_root(.    sho
-00002d40: 7274 636f 6465 3a20 7374 722c 0a20 2020  rtcode: str,.   
-00002d50: 2064 6566 6175 6c74 5f6f 6e74 6f6c 6f67   default_ontolog
-00002d60: 793a 2073 7472 2c0a 2920 2d3e 2065 7472  y: str,.) -> etr
-00002d70: 6565 2e5f 456c 656d 656e 743a 0a20 2020  ee._Element:.   
-00002d80: 2022 2222 0a20 2020 2053 7461 7274 2062   """.    Start b
-00002d90: 7569 6c64 696e 6720 796f 7572 2058 4d4c  uilding your XML
-00002da0: 2064 6f63 756d 656e 7420 6279 2063 7265   document by cre
-00002db0: 6174 696e 6720 7468 6520 726f 6f74 2065  ating the root e
-00002dc0: 6c65 6d65 6e74 203c 6b6e 6f72 613e 2e0a  lement <knora>..
-00002dd0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-00002de0: 2020 2073 686f 7274 636f 6465 3a20 5468     shortcode: Th
-00002df0: 6520 7368 6f72 7463 6f64 6520 6f66 2074  e shortcode of t
-00002e00: 6869 7320 7072 6f6a 6563 7420 6173 2064  his project as d
-00002e10: 6566 696e 6564 2069 6e20 7468 6520 4a53  efined in the JS
-00002e20: 4f4e 2070 726f 6a65 6374 2066 696c 650a  ON project file.
-00002e30: 2020 2020 2020 2020 6465 6661 756c 745f          default_
-00002e40: 6f6e 746f 6c6f 6779 3a20 6f6e 6520 6f66  ontology: one of
-00002e50: 2074 6865 206f 6e74 6f6c 6f67 6965 7320   the ontologies 
-00002e60: 6f66 2074 6865 204a 534f 4e20 7072 6f6a  of the JSON proj
-00002e70: 6563 7420 6669 6c65 0a0a 2020 2020 5265  ect file..    Re
-00002e80: 7475 726e 733a 0a20 2020 2020 2020 2054  turns:.        T
-00002e90: 6865 2072 6f6f 7420 656c 656d 656e 7420  he root element 
-00002ea0: 3c6b 6e6f 7261 3e2e 0a0a 2020 2020 4578  <knora>...    Ex
-00002eb0: 616d 706c 6573 3a0a 2020 2020 2020 2020  amples:.        
-00002ec0: 3e3e 3e20 726f 6f74 203d 2065 7863 656c  >>> root = excel
-00002ed0: 3278 6d6c 2e6d 616b 655f 726f 6f74 2873  2xml.make_root(s
-00002ee0: 686f 7274 636f 6465 3d73 686f 7274 636f  hortcode=shortco
-00002ef0: 6465 2c20 6465 6661 756c 745f 6f6e 746f  de, default_onto
-00002f00: 6c6f 6779 3d64 6566 6175 6c74 5f6f 6e74  logy=default_ont
-00002f10: 6f6c 6f67 7929 0a20 2020 2020 2020 203e  ology).        >
-00002f20: 3e3e 2072 6f6f 7420 3d20 6578 6365 6c32  >> root = excel2
-00002f30: 786d 6c2e 6170 7065 6e64 5f70 6572 6d69  xml.append_permi
-00002f40: 7373 696f 6e73 2872 6f6f 7429 0a0a 2020  ssions(root)..  
-00002f50: 2020 5365 6520 6874 7470 733a 2f2f 646f    See https://do
-00002f60: 6373 2e64 6173 6368 2e73 7769 7373 2f6c  cs.dasch.swiss/l
-00002f70: 6174 6573 742f 4453 502d 544f 4f4c 532f  atest/DSP-TOOLS/
-00002f80: 6669 6c65 2d66 6f72 6d61 7473 2f78 6d6c  file-formats/xml
-00002f90: 2d64 6174 612d 6669 6c65 2f23 7468 652d  -data-file/#the-
-00002fa0: 726f 6f74 2d65 6c65 6d65 6e74 2d6b 6e6f  root-element-kno
-00002fb0: 7261 0a20 2020 2022 2222 0a20 2020 2073  ra.    """.    s
-00002fc0: 6368 656d 615f 7572 6c20 3d20 2268 7474  chema_url = "htt
-00002fd0: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
-00002fe0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f64  sercontent.com/d
-00002ff0: 6173 6368 2d73 7769 7373 2f64 7370 2d74  asch-swiss/dsp-t
-00003000: 6f6f 6c73 2f6d 6169 6e2f 7372 632f 6473  ools/main/src/ds
-00003010: 705f 746f 6f6c 732f 7265 736f 7572 6365  p_tools/resource
-00003020: 732f 7363 6865 6d61 2f64 6174 612e 7873  s/schema/data.xs
-00003030: 6422 0a20 2020 2073 6368 656d 615f 6c6f  d".    schema_lo
-00003040: 6361 7469 6f6e 5f6b 6579 203d 2073 7472  cation_key = str
-00003050: 2865 7472 6565 2e51 4e61 6d65 2822 6874  (etree.QName("ht
-00003060: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
-00003070: 3230 3031 2f58 4d4c 5363 6865 6d61 2d69  2001/XMLSchema-i
-00003080: 6e73 7461 6e63 6522 2c20 2273 6368 656d  nstance", "schem
-00003090: 614c 6f63 6174 696f 6e22 2929 0a20 2020  aLocation")).   
-000030a0: 2073 6368 656d 615f 6c6f 6361 7469 6f6e   schema_location
-000030b0: 5f76 616c 7565 203d 2066 2268 7474 7073  _value = f"https
-000030c0: 3a2f 2f64 6173 6368 2e73 7769 7373 2f73  ://dasch.swiss/s
-000030d0: 6368 656d 6120 7b73 6368 656d 615f 7572  chema {schema_ur
-000030e0: 6c7d 220a 2020 2020 7265 7475 726e 2065  l}".    return e
-000030f0: 7472 6565 2e45 6c65 6d65 6e74 280a 2020  tree.Element(.  
-00003100: 2020 2020 2020 227b 2573 7d6b 6e6f 7261        "{%s}knora
-00003110: 2220 2520 786d 6c5f 6e61 6d65 7370 6163  " % xml_namespac
-00003120: 655f 6d61 705b 4e6f 6e65 5d2c 0a20 2020  e_map[None],.   
-00003130: 2020 2020 2061 7474 7269 623d 7b0a 2020       attrib={.  
-00003140: 2020 2020 2020 2020 2020 7363 6865 6d61            schema
-00003150: 5f6c 6f63 6174 696f 6e5f 6b65 793a 2073  _location_key: s
-00003160: 6368 656d 615f 6c6f 6361 7469 6f6e 5f76  chema_location_v
-00003170: 616c 7565 2c0a 2020 2020 2020 2020 2020  alue,.          
-00003180: 2020 2273 686f 7274 636f 6465 223a 2073    "shortcode": s
-00003190: 686f 7274 636f 6465 2c0a 2020 2020 2020  hortcode,.      
-000031a0: 2020 2020 2020 2264 6566 6175 6c74 2d6f        "default-o
-000031b0: 6e74 6f6c 6f67 7922 3a20 6465 6661 756c  ntology": defaul
-000031c0: 745f 6f6e 746f 6c6f 6779 2c0a 2020 2020  t_ontology,.    
-000031d0: 2020 2020 7d2c 0a20 2020 2020 2020 206e      },.        n
-000031e0: 736d 6170 3d78 6d6c 5f6e 616d 6573 7061  smap=xml_namespa
-000031f0: 6365 5f6d 6170 2c0a 2020 2020 290a 0a0a  ce_map,.    )...
-00003200: 6465 6620 6170 7065 6e64 5f70 6572 6d69  def append_permi
-00003210: 7373 696f 6e73 2872 6f6f 745f 656c 656d  ssions(root_elem
-00003220: 656e 743a 2065 7472 6565 2e5f 456c 656d  ent: etree._Elem
-00003230: 656e 7429 202d 3e20 6574 7265 652e 5f45  ent) -> etree._E
-00003240: 6c65 6d65 6e74 3a0a 2020 2020 2222 220a  lement:.    """.
-00003250: 2020 2020 4166 7465 7220 6861 7669 6e67      After having
-00003260: 2063 7265 6174 6564 2061 2072 6f6f 7420   created a root 
-00003270: 656c 656d 656e 742c 2063 616c 6c20 7468  element, call th
-00003280: 6973 206d 6574 686f 6420 746f 2061 7070  is method to app
-00003290: 656e 6420 7468 6520 666f 7572 2070 6572  end the four per
-000032a0: 6d69 7373 696f 6e73 2022 7265 732d 6465  missions "res-de
-000032b0: 6661 756c 7422 2c0a 2020 2020 2272 6573  fault",.    "res
-000032c0: 2d72 6573 7472 6963 7465 6422 2c20 2270  -restricted", "p
-000032d0: 726f 702d 6465 6661 756c 7422 2c20 616e  rop-default", an
-000032e0: 6420 2270 726f 702d 7265 7374 7269 6374  d "prop-restrict
-000032f0: 6564 2220 746f 2069 742e 2054 6865 7365  ed" to it. These
-00003300: 2066 6f75 7220 7065 726d 6973 7369 6f6e   four permission
-00003310: 7320 6172 6520 6120 676f 6f64 2062 6173  s are a good bas
-00003320: 6973 2074 6f0a 2020 2020 7374 6172 7420  is to.    start 
-00003330: 7769 7468 2c20 6275 7420 7265 6d65 6d62  with, but rememb
-00003340: 6572 2074 6861 7420 7468 6579 2063 616e  er that they can
-00003350: 2062 6520 6164 6170 7465 642c 2061 6e64   be adapted, and
-00003360: 2074 6861 7420 6f74 6865 7220 7065 726d   that other perm
-00003370: 6973 7369 6f6e 7320 6361 6e20 6265 2064  issions can be d
-00003380: 6566 696e 6564 2069 6e73 7465 6164 206f  efined instead o
-00003390: 6620 7468 6573 652e 0a0a 2020 2020 4172  f these...    Ar
-000033a0: 6773 3a0a 2020 2020 2020 2020 726f 6f74  gs:.        root
-000033b0: 5f65 6c65 6d65 6e74 3a20 5468 6520 584d  _element: The XM
-000033c0: 4c20 726f 6f74 2065 6c65 6d65 6e74 203c  L root element <
-000033d0: 6b6e 6f72 613e 2063 7265 6174 6564 2062  knora> created b
-000033e0: 7920 6d61 6b65 5f72 6f6f 7428 290a 0a20  y make_root().. 
-000033f0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00003400: 2020 2020 5468 6520 726f 6f74 2065 6c65      The root ele
-00003410: 6d65 6e74 2077 6974 6820 7468 6520 666f  ment with the fo
-00003420: 7572 2070 6572 6d69 7373 696f 6e20 626c  ur permission bl
-00003430: 6f63 6b73 2061 7070 656e 6465 640a 0a20  ocks appended.. 
-00003440: 2020 2045 7861 6d70 6c65 733a 0a20 2020     Examples:.   
-00003450: 2020 2020 203e 3e3e 2072 6f6f 7420 3d20       >>> root = 
-00003460: 6578 6365 6c32 786d 6c2e 6d61 6b65 5f72  excel2xml.make_r
-00003470: 6f6f 7428 7368 6f72 7463 6f64 653d 7368  oot(shortcode=sh
-00003480: 6f72 7463 6f64 652c 2064 6566 6175 6c74  ortcode, default
-00003490: 5f6f 6e74 6f6c 6f67 793d 6465 6661 756c  _ontology=defaul
-000034a0: 745f 6f6e 746f 6c6f 6779 290a 2020 2020  t_ontology).    
-000034b0: 2020 2020 3e3e 3e20 726f 6f74 203d 2065      >>> root = e
-000034c0: 7863 656c 3278 6d6c 2e61 7070 656e 645f  xcel2xml.append_
-000034d0: 7065 726d 6973 7369 6f6e 7328 726f 6f74  permissions(root
-000034e0: 290a 0a20 2020 2053 6565 2068 7474 7073  )..    See https
-000034f0: 3a2f 2f64 6f63 732e 6461 7363 682e 7377  ://docs.dasch.sw
-00003500: 6973 732f 6c61 7465 7374 2f44 5350 2d54  iss/latest/DSP-T
-00003510: 4f4f 4c53 2f66 696c 652d 666f 726d 6174  OOLS/file-format
-00003520: 732f 786d 6c2d 6461 7461 2d66 696c 652f  s/xml-data-file/
-00003530: 2364 6573 6372 6962 696e 672d 7065 726d  #describing-perm
-00003540: 6973 7369 6f6e 732d 7769 7468 2d70 6572  issions-with-per
-00003550: 6d69 7373 696f 6e73 2d65 6c65 6d65 6e74  missions-element
-00003560: 730a 2020 2020 2222 220a 0a20 2020 2050  s.    """..    P
-00003570: 4552 4d49 5353 494f 4e53 203d 2045 2e70  ERMISSIONS = E.p
-00003580: 6572 6d69 7373 696f 6e73 0a20 2020 2041  ermissions.    A
-00003590: 4c4c 4f57 203d 2045 2e61 6c6c 6f77 0a20  LLOW = E.allow. 
-000035a0: 2020 2023 206c 786d 6c2e 6275 696c 6465     # lxml.builde
-000035b0: 722e 4520 6973 2061 206d 6f72 6520 736f  r.E is a more so
-000035c0: 7068 6973 7469 6361 7465 6420 656c 656d  phisticated elem
-000035d0: 656e 7420 6661 6374 6f72 7920 7468 616e  ent factory than
-000035e0: 2065 7472 6565 2e45 6c65 6d65 6e74 2e0a   etree.Element..
-000035f0: 2020 2020 2320 452e 7461 6720 6973 2065      # E.tag is e
-00003600: 7175 6976 616c 656e 7420 746f 2045 2822  quivalent to E("
-00003610: 7461 6722 2920 616e 6420 7265 7375 6c74  tag") and result
-00003620: 7320 696e 203c 7461 673e 0a0a 2020 2020  s in <tag>..    
-00003630: 7265 735f 6465 6661 756c 7420 3d20 6574  res_default = et
-00003640: 7265 652e 456c 656d 656e 7428 227b 2573  ree.Element("{%s
-00003650: 7d70 6572 6d69 7373 696f 6e73 2220 2520  }permissions" % 
-00003660: 786d 6c5f 6e61 6d65 7370 6163 655f 6d61  xml_namespace_ma
-00003670: 705b 4e6f 6e65 5d2c 2069 643d 2272 6573  p[None], id="res
-00003680: 2d64 6566 6175 6c74 2229 0a20 2020 2072  -default").    r
-00003690: 6573 5f64 6566 6175 6c74 2e61 7070 656e  es_default.appen
-000036a0: 6428 414c 4c4f 5728 2256 222c 2067 726f  d(ALLOW("V", gro
-000036b0: 7570 3d22 556e 6b6e 6f77 6e55 7365 7222  up="UnknownUser"
-000036c0: 2929 0a20 2020 2072 6573 5f64 6566 6175  )).    res_defau
-000036d0: 6c74 2e61 7070 656e 6428 414c 4c4f 5728  lt.append(ALLOW(
-000036e0: 2256 222c 2067 726f 7570 3d22 4b6e 6f77  "V", group="Know
-000036f0: 6e55 7365 7222 2929 0a20 2020 2072 6573  nUser")).    res
-00003700: 5f64 6566 6175 6c74 2e61 7070 656e 6428  _default.append(
-00003710: 414c 4c4f 5728 2244 222c 2067 726f 7570  ALLOW("D", group
-00003720: 3d22 5072 6f6a 6563 744d 656d 6265 7222  ="ProjectMember"
-00003730: 2929 0a20 2020 2072 6573 5f64 6566 6175  )).    res_defau
-00003740: 6c74 2e61 7070 656e 6428 414c 4c4f 5728  lt.append(ALLOW(
-00003750: 2243 5222 2c20 6772 6f75 703d 2250 726f  "CR", group="Pro
-00003760: 6a65 6374 4164 6d69 6e22 2929 0a20 2020  jectAdmin")).   
-00003770: 2072 6573 5f64 6566 6175 6c74 2e61 7070   res_default.app
-00003780: 656e 6428 414c 4c4f 5728 2243 5222 2c20  end(ALLOW("CR", 
-00003790: 6772 6f75 703d 2243 7265 6174 6f72 2229  group="Creator")
-000037a0: 290a 2020 2020 726f 6f74 5f65 6c65 6d65  ).    root_eleme
-000037b0: 6e74 2e61 7070 656e 6428 7265 735f 6465  nt.append(res_de
-000037c0: 6661 756c 7429 0a0a 2020 2020 7265 735f  fault)..    res_
-000037d0: 7265 7374 7269 6374 6564 203d 2050 4552  restricted = PER
-000037e0: 4d49 5353 494f 4e53 2869 643d 2272 6573  MISSIONS(id="res
-000037f0: 2d72 6573 7472 6963 7465 6422 290a 2020  -restricted").  
-00003800: 2020 7265 735f 7265 7374 7269 6374 6564    res_restricted
-00003810: 2e61 7070 656e 6428 414c 4c4f 5728 224d  .append(ALLOW("M
-00003820: 222c 2067 726f 7570 3d22 5072 6f6a 6563  ", group="Projec
-00003830: 744d 656d 6265 7222 2929 0a20 2020 2072  tMember")).    r
-00003840: 6573 5f72 6573 7472 6963 7465 642e 6170  es_restricted.ap
-00003850: 7065 6e64 2841 4c4c 4f57 2822 4352 222c  pend(ALLOW("CR",
-00003860: 2067 726f 7570 3d22 5072 6f6a 6563 7441   group="ProjectA
-00003870: 646d 696e 2229 290a 2020 2020 7265 735f  dmin")).    res_
-00003880: 7265 7374 7269 6374 6564 2e61 7070 656e  restricted.appen
-00003890: 6428 414c 4c4f 5728 2243 5222 2c20 6772  d(ALLOW("CR", gr
-000038a0: 6f75 703d 2243 7265 6174 6f72 2229 290a  oup="Creator")).
-000038b0: 2020 2020 726f 6f74 5f65 6c65 6d65 6e74      root_element
-000038c0: 2e61 7070 656e 6428 7265 735f 7265 7374  .append(res_rest
-000038d0: 7269 6374 6564 290a 0a20 2020 2070 726f  ricted)..    pro
-000038e0: 705f 6465 6661 756c 7420 3d20 5045 524d  p_default = PERM
-000038f0: 4953 5349 4f4e 5328 6964 3d22 7072 6f70  ISSIONS(id="prop
-00003900: 2d64 6566 6175 6c74 2229 0a20 2020 2070  -default").    p
-00003910: 726f 705f 6465 6661 756c 742e 6170 7065  rop_default.appe
-00003920: 6e64 2841 4c4c 4f57 2822 5622 2c20 6772  nd(ALLOW("V", gr
-00003930: 6f75 703d 2255 6e6b 6e6f 776e 5573 6572  oup="UnknownUser
-00003940: 2229 290a 2020 2020 7072 6f70 5f64 6566  ")).    prop_def
-00003950: 6175 6c74 2e61 7070 656e 6428 414c 4c4f  ault.append(ALLO
-00003960: 5728 2256 222c 2067 726f 7570 3d22 4b6e  W("V", group="Kn
-00003970: 6f77 6e55 7365 7222 2929 0a20 2020 2070  ownUser")).    p
-00003980: 726f 705f 6465 6661 756c 742e 6170 7065  rop_default.appe
-00003990: 6e64 2841 4c4c 4f57 2822 4422 2c20 6772  nd(ALLOW("D", gr
-000039a0: 6f75 703d 2250 726f 6a65 6374 4d65 6d62  oup="ProjectMemb
-000039b0: 6572 2229 290a 2020 2020 7072 6f70 5f64  er")).    prop_d
-000039c0: 6566 6175 6c74 2e61 7070 656e 6428 414c  efault.append(AL
-000039d0: 4c4f 5728 2243 5222 2c20 6772 6f75 703d  LOW("CR", group=
-000039e0: 2250 726f 6a65 6374 4164 6d69 6e22 2929  "ProjectAdmin"))
-000039f0: 0a20 2020 2070 726f 705f 6465 6661 756c  .    prop_defaul
-00003a00: 742e 6170 7065 6e64 2841 4c4c 4f57 2822  t.append(ALLOW("
-00003a10: 4352 222c 2067 726f 7570 3d22 4372 6561  CR", group="Crea
-00003a20: 746f 7222 2929 0a20 2020 2072 6f6f 745f  tor")).    root_
-00003a30: 656c 656d 656e 742e 6170 7065 6e64 2870  element.append(p
-00003a40: 726f 705f 6465 6661 756c 7429 0a0a 2020  rop_default)..  
-00003a50: 2020 7072 6f70 5f72 6573 7472 6963 7465    prop_restricte
-00003a60: 6420 3d20 5045 524d 4953 5349 4f4e 5328  d = PERMISSIONS(
-00003a70: 6964 3d22 7072 6f70 2d72 6573 7472 6963  id="prop-restric
-00003a80: 7465 6422 290a 2020 2020 7072 6f70 5f72  ted").    prop_r
-00003a90: 6573 7472 6963 7465 642e 6170 7065 6e64  estricted.append
-00003aa0: 2841 4c4c 4f57 2822 4d22 2c20 6772 6f75  (ALLOW("M", grou
-00003ab0: 703d 2250 726f 6a65 6374 4d65 6d62 6572  p="ProjectMember
-00003ac0: 2229 290a 2020 2020 7072 6f70 5f72 6573  ")).    prop_res
-00003ad0: 7472 6963 7465 642e 6170 7065 6e64 2841  tricted.append(A
-00003ae0: 4c4c 4f57 2822 4352 222c 2067 726f 7570  LLOW("CR", group
-00003af0: 3d22 5072 6f6a 6563 7441 646d 696e 2229  ="ProjectAdmin")
-00003b00: 290a 2020 2020 7072 6f70 5f72 6573 7472  ).    prop_restr
-00003b10: 6963 7465 642e 6170 7065 6e64 2841 4c4c  icted.append(ALL
-00003b20: 4f57 2822 4352 222c 2067 726f 7570 3d22  OW("CR", group="
-00003b30: 4372 6561 746f 7222 2929 0a20 2020 2072  Creator")).    r
-00003b40: 6f6f 745f 656c 656d 656e 742e 6170 7065  oot_element.appe
-00003b50: 6e64 2870 726f 705f 7265 7374 7269 6374  nd(prop_restrict
-00003b60: 6564 290a 0a20 2020 2072 6574 7572 6e20  ed)..    return 
-00003b70: 726f 6f74 5f65 6c65 6d65 6e74 0a0a 0a64  root_element...d
-00003b80: 6566 206d 616b 655f 7265 736f 7572 6365  ef make_resource
-00003b90: 2820 2023 206e 6f71 613a 2044 3431 3720  (  # noqa: D417 
-00003ba0: 2875 6e64 6f63 756d 656e 7465 642d 7061  (undocumented-pa
-00003bb0: 7261 6d29 0a20 2020 206c 6162 656c 3a20  ram).    label: 
-00003bc0: 7374 722c 0a20 2020 2072 6573 7479 7065  str,.    restype
-00003bd0: 3a20 7374 722c 0a20 2020 2069 643a 2073  : str,.    id: s
-00003be0: 7472 2c0a 2020 2020 7065 726d 6973 7369  tr,.    permissi
-00003bf0: 6f6e 733a 2073 7472 203d 2022 7265 732d  ons: str = "res-
-00003c00: 6465 6661 756c 7422 2c0a 2020 2020 6172  default",.    ar
-00003c10: 6b3a 204f 7074 696f 6e61 6c5b 7374 725d  k: Optional[str]
-00003c20: 203d 204e 6f6e 652c 0a20 2020 2069 7269   = None,.    iri
-00003c30: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-00003c40: 3d20 4e6f 6e65 2c0a 2020 2020 6372 6561  = None,.    crea
-00003c50: 7469 6f6e 5f64 6174 653a 204f 7074 696f  tion_date: Optio
-00003c60: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-00003c70: 0a29 202d 3e20 6574 7265 652e 5f45 6c65  .) -> etree._Ele
-00003c80: 6d65 6e74 3a0a 2020 2020 2222 220a 2020  ment:.    """.  
-00003c90: 2020 4372 6561 7465 7320 616e 2065 6d70    Creates an emp
-00003ca0: 7479 2072 6573 6f75 7263 6520 656c 656d  ty resource elem
-00003cb0: 656e 742c 2077 6974 6820 7468 6520 6174  ent, with the at
-00003cc0: 7472 6962 7574 6573 2061 7320 7370 6563  tributes as spec
-00003cd0: 6966 6965 6420 6279 2074 6865 2061 7267  ified by the arg
-00003ce0: 756d 656e 7473 0a0a 2020 2020 4172 6773  uments..    Args
-00003cf0: 3a0a 2020 2020 2020 2020 5468 6520 6172  :.        The ar
-00003d00: 6775 6d65 6e74 7320 636f 7272 6573 706f  guments correspo
-00003d10: 6e64 2074 6f20 7468 6520 6174 7472 6962  nd to the attrib
-00003d20: 7574 6573 206f 6620 7468 6520 3c72 6573  utes of the <res
-00003d30: 6f75 7263 653e 2065 6c65 6d65 6e74 2e0a  ource> element..
-00003d40: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
-00003d50: 2020 2020 2020 5468 6520 7265 736f 7572        The resour
-00003d60: 6365 2065 6c65 6d65 6e74 2c20 7769 7468  ce element, with
-00003d70: 6f75 7420 616e 7920 6368 696c 6472 656e  out any children
-00003d80: 2c20 6275 7420 7769 7468 2074 6865 2061  , but with the a
-00003d90: 7474 7269 6275 7465 730a 2020 2020 2020  ttributes.      
-00003da0: 2020 6060 3c72 6573 6f75 7263 6520 6c61    ``<resource la
-00003db0: 6265 6c3d 6c61 6265 6c20 7265 7374 7970  bel=label restyp
-00003dc0: 653d 7265 7374 7970 6520 6964 3d69 6420  e=restype id=id 
-00003dd0: 7065 726d 6973 7369 6f6e 733d 7065 726d  permissions=perm
-00003de0: 6973 7369 6f6e 7320 6172 6b3d 6172 6b20  issions ark=ark 
-00003df0: 6972 693d 6972 693e 3c2f 7265 736f 7572  iri=iri></resour
-00003e00: 6365 3e60 600a 0a20 2020 2052 6169 7365  ce>``..    Raise
-00003e10: 733a 0a20 2020 2020 2020 2057 6172 6e69  s:.        Warni
-00003e20: 6e67 3a20 6966 2062 6f74 6820 616e 2041  ng: if both an A
-00003e30: 524b 2061 6e64 2061 6e20 4952 4920 6172  RK and an IRI ar
-00003e40: 6520 7072 6f76 6964 6564 0a20 2020 2020  e provided.     
-00003e50: 2020 2042 6173 6545 7272 6f72 3a20 6966     BaseError: if
-00003e60: 2074 6865 2063 7265 6174 696f 6e20 6461   the creation da
-00003e70: 7465 2069 7320 696e 7661 6c69 640a 0a20  te is invalid.. 
-00003e80: 2020 2045 7861 6d70 6c65 733a 0a20 2020     Examples:.   
-00003e90: 2020 2020 203e 3e3e 2072 6573 6f75 7263       >>> resourc
-00003ea0: 6520 3d20 6578 6365 6c32 786d 6c2e 6d61  e = excel2xml.ma
-00003eb0: 6b65 5f72 6573 6f75 7263 6528 2e2e 2e29  ke_resource(...)
-00003ec0: 0a20 2020 2020 2020 203e 3e3e 2072 6573  .        >>> res
-00003ed0: 6f75 7263 652e 6170 7065 6e64 2865 7863  ource.append(exc
-00003ee0: 656c 3278 6d6c 2e6d 616b 655f 7465 7874  el2xml.make_text
-00003ef0: 5f70 726f 7028 2e2e 2e29 290a 2020 2020  _prop(...)).    
-00003f00: 2020 2020 3e3e 3e20 726f 6f74 2e61 7070      >>> root.app
-00003f10: 656e 6428 7265 736f 7572 6365 290a 0a20  end(resource).. 
-00003f20: 2020 2053 6565 2068 7474 7073 3a2f 2f64     See https://d
-00003f30: 6f63 732e 6461 7363 682e 7377 6973 732f  ocs.dasch.swiss/
-00003f40: 6c61 7465 7374 2f44 5350 2d54 4f4f 4c53  latest/DSP-TOOLS
-00003f50: 2f66 696c 652d 666f 726d 6174 732f 786d  /file-formats/xm
-00003f60: 6c2d 6461 7461 2d66 696c 652f 2364 6573  l-data-file/#des
-00003f70: 6372 6962 696e 672d 7265 736f 7572 6365  cribing-resource
-00003f80: 732d 7769 7468 2d74 6865 2d72 6573 6f75  s-with-the-resou
-00003f90: 7263 652d 656c 656d 656e 740a 2020 2020  rce-element.    
-00003fa0: 2222 220a 2020 2020 6966 206e 6f74 2063  """.    if not c
-00003fb0: 6865 636b 5f6e 6f74 6e61 286c 6162 656c  heck_notna(label
-00003fc0: 293a 0a20 2020 2020 2020 206d 7367 203d  ):.        msg =
-00003fd0: 2066 2259 6f75 7220 7265 736f 7572 6365   f"Your resource
-00003fe0: 2773 206c 6162 656c 206c 6f6f 6b73 2073  's label looks s
-00003ff0: 7573 7069 6369 6f75 7320 2872 6573 6f75  uspicious (resou
-00004000: 7263 6520 7769 7468 2069 6420 277b 6964  rce with id '{id
-00004010: 7d27 2061 6e64 206c 6162 656c 2027 7b6c  }' and label '{l
-00004020: 6162 656c 7d27 2922 0a20 2020 2020 2020  abel}')".       
-00004030: 2077 6172 6e69 6e67 732e 7761 726e 2844   warnings.warn(D
-00004040: 7370 546f 6f6c 7355 7365 7257 6172 6e69  spToolsUserWarni
-00004050: 6e67 286d 7367 2929 0a20 2020 2069 6620  ng(msg)).    if 
-00004060: 6e6f 7420 6368 6563 6b5f 6e6f 746e 6128  not check_notna(
-00004070: 6964 293a 0a20 2020 2020 2020 206d 7367  id):.        msg
-00004080: 203d 2066 2259 6f75 7220 7265 736f 7572   = f"Your resour
-00004090: 6365 2773 2069 6420 6c6f 6f6b 7320 7375  ce's id looks su
-000040a0: 7370 6963 696f 7573 2028 7265 736f 7572  spicious (resour
-000040b0: 6365 2077 6974 6820 6964 2027 7b69 647d  ce with id '{id}
-000040c0: 2720 616e 6420 6c61 6265 6c20 277b 6c61  ' and label '{la
-000040d0: 6265 6c7d 2722 0a20 2020 2020 2020 2077  bel}'".        w
-000040e0: 6172 6e69 6e67 732e 7761 726e 2844 7370  arnings.warn(Dsp
-000040f0: 546f 6f6c 7355 7365 7257 6172 6e69 6e67  ToolsUserWarning
-00004100: 286d 7367 2929 0a20 2020 206b 7761 7267  (msg)).    kwarg
-00004110: 7320 3d20 7b22 6c61 6265 6c22 3a20 6c61  s = {"label": la
-00004120: 6265 6c2c 2022 7265 7374 7970 6522 3a20  bel, "restype": 
-00004130: 7265 7374 7970 652c 2022 6964 223a 2069  restype, "id": i
-00004140: 642c 2022 7065 726d 6973 7369 6f6e 7322  d, "permissions"
-00004150: 3a20 7065 726d 6973 7369 6f6e 732c 2022  : permissions, "
-00004160: 6e73 6d61 7022 3a20 786d 6c5f 6e61 6d65  nsmap": xml_name
-00004170: 7370 6163 655f 6d61 707d 0a20 2020 2069  space_map}.    i
-00004180: 6620 6172 6b3a 0a20 2020 2020 2020 206b  f ark:.        k
-00004190: 7761 7267 735b 2261 726b 225d 203d 2061  wargs["ark"] = a
-000041a0: 726b 0a20 2020 2069 6620 6972 693a 0a20  rk.    if iri:. 
-000041b0: 2020 2020 2020 206b 7761 7267 735b 2269         kwargs["i
-000041c0: 7269 225d 203d 2069 7269 0a20 2020 2069  ri"] = iri.    i
-000041d0: 6620 6172 6b20 616e 6420 6972 693a 0a20  f ark and iri:. 
-000041e0: 2020 2020 2020 206d 7367 203d 2066 2242         msg = f"B
-000041f0: 6f74 6820 4152 4b20 616e 6420 4952 4920  oth ARK and IRI 
-00004200: 7765 7265 2070 726f 7669 6465 6420 666f  were provided fo
-00004210: 7220 7265 736f 7572 6365 2027 7b6c 6162  r resource '{lab
-00004220: 656c 7d27 2028 7b69 647d 292e 2054 6865  el}' ({id}). The
-00004230: 2041 524b 2077 696c 6c20 6f76 6572 7269   ARK will overri
-00004240: 6465 2074 6865 2049 5249 2e22 0a20 2020  de the IRI.".   
-00004250: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
-00004260: 726e 2844 7370 546f 6f6c 7355 7365 7257  rn(DspToolsUserW
-00004270: 6172 6e69 6e67 286d 7367 2929 0a20 2020  arning(msg)).   
-00004280: 2069 6620 6372 6561 7469 6f6e 5f64 6174   if creation_dat
-00004290: 653a 0a20 2020 2020 2020 2074 7279 3a0a  e:.        try:.
-000042a0: 2020 2020 2020 2020 2020 2020 4461 7465              Date
-000042b0: 5469 6d65 5374 616d 7028 6372 6561 7469  TimeStamp(creati
-000042c0: 6f6e 5f64 6174 6529 0a20 2020 2020 2020  on_date).       
-000042d0: 2065 7863 6570 7420 4261 7365 4572 726f   except BaseErro
-000042e0: 723a 0a20 2020 2020 2020 2020 2020 2072  r:.            r
-000042f0: 6169 7365 2042 6173 6545 7272 6f72 280a  aise BaseError(.
-00004300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004310: 6622 5468 6520 7265 736f 7572 6365 2027  f"The resource '
-00004320: 7b6c 6162 656c 7d27 2028 4944 3a20 7b69  {label}' (ID: {i
-00004330: 647d 2920 6861 7320 616e 2069 6e76 616c  d}) has an inval
-00004340: 6964 2063 7265 6174 696f 6e20 6461 7465  id creation date
-00004350: 2027 7b63 7265 6174 696f 6e5f 6461 7465   '{creation_date
-00004360: 7d27 2e20 220a 2020 2020 2020 2020 2020  }'. ".          
-00004370: 2020 2020 2020 6622 4469 6420 796f 7520        f"Did you 
-00004380: 7065 7268 6170 7320 666f 7267 6574 2074  perhaps forget t
-00004390: 6865 2074 696d 657a 6f6e 653f 220a 2020  he timezone?".  
-000043a0: 2020 2020 2020 2020 2020 2920 6672 6f6d            ) from
-000043b0: 204e 6f6e 650a 2020 2020 2020 2020 6b77   None.        kw
-000043c0: 6172 6773 5b22 6372 6561 7469 6f6e 5f64  args["creation_d
-000043d0: 6174 6522 5d20 3d20 6372 6561 7469 6f6e  ate"] = creation
-000043e0: 5f64 6174 650a 0a20 2020 2072 6574 7572  _date..    retur
-000043f0: 6e20 6574 7265 652e 456c 656d 656e 7428  n etree.Element(
-00004400: 227b 2573 7d72 6573 6f75 7263 6522 2025  "{%s}resource" %
-00004410: 2078 6d6c 5f6e 616d 6573 7061 6365 5f6d   xml_namespace_m
-00004420: 6170 5b4e 6f6e 655d 2c20 2a2a 6b77 6172  ap[None], **kwar
-00004430: 6773 2920 2023 2074 7970 653a 2069 676e  gs)  # type: ign
-00004440: 6f72 655b 6172 672d 7479 7065 5d0a 0a0a  ore[arg-type]...
-00004450: 6465 6620 6d61 6b65 5f62 6974 7374 7265  def make_bitstre
-00004460: 616d 5f70 726f 7028 0a20 2020 2070 6174  am_prop(.    pat
-00004470: 683a 2055 6e69 6f6e 5b73 7472 2c20 6f73  h: Union[str, os
-00004480: 2e50 6174 684c 696b 655b 416e 795d 5d2c  .PathLike[Any]],
-00004490: 0a20 2020 2070 6572 6d69 7373 696f 6e73  .    permissions
-000044a0: 3a20 7374 7220 3d20 2270 726f 702d 6465  : str = "prop-de
-000044b0: 6661 756c 7422 2c0a 2020 2020 6368 6563  fault",.    chec
-000044c0: 6b3a 2062 6f6f 6c20 3d20 4661 6c73 652c  k: bool = False,
-000044d0: 0a20 2020 2063 616c 6c69 6e67 5f72 6573  .    calling_res
-000044e0: 6f75 7263 653a 2073 7472 203d 2022 222c  ource: str = "",
-000044f0: 0a29 202d 3e20 6574 7265 652e 5f45 6c65  .) -> etree._Ele
-00004500: 6d65 6e74 3a0a 2020 2020 2222 220a 2020  ment:.    """.  
-00004510: 2020 4372 6561 7465 7320 6120 6269 7473    Creates a bits
-00004520: 7472 6561 6d20 656c 656d 656e 7420 7468  tream element th
-00004530: 6174 2070 6f69 6e74 7320 746f 2022 7061  at points to "pa
-00004540: 7468 222e 0a0a 2020 2020 4172 6773 3a0a  th"...    Args:.
-00004550: 2020 2020 2020 2020 7061 7468 3a20 7061          path: pa
-00004560: 7468 2074 6f20 6120 7661 6c69 6420 6669  th to a valid fi
-00004570: 6c65 2074 6861 7420 7769 6c6c 2062 6520  le that will be 
-00004580: 7570 6c6f 6164 6564 0a20 2020 2020 2020  uploaded.       
-00004590: 2070 6572 6d69 7373 696f 6e73 3a20 7065   permissions: pe
-000045a0: 726d 6973 7369 6f6e 7320 7374 7269 6e67  rmissions string
-000045b0: 0a20 2020 2020 2020 2063 6865 636b 3a20  .        check: 
-000045c0: 6966 2054 7275 652c 2069 7373 7565 2061  if True, issue a
-000045d0: 2077 6172 6e69 6e67 2069 6620 7468 6520   warning if the 
-000045e0: 7061 7468 2064 6f65 736e 2774 2070 6f69  path doesn't poi
-000045f0: 6e74 2074 6f20 616e 2065 7869 7374 696e  nt to an existin
-00004600: 6720 6669 6c65 0a20 2020 2020 2020 2063  g file.        c
-00004610: 616c 6c69 6e67 5f72 6573 6f75 7263 653a  alling_resource:
-00004620: 2074 6865 206e 616d 6520 6f66 2074 6865   the name of the
-00004630: 2070 6172 656e 7420 7265 736f 7572 6365   parent resource
-00004640: 2028 666f 7220 6265 7474 6572 2065 7272   (for better err
-00004650: 6f72 206d 6573 7361 6765 7329 0a0a 2020  or messages)..  
-00004660: 2020 5761 726e 733a 0a20 2020 2020 2020    Warns:.       
-00004670: 2069 6620 7468 6520 7061 7468 2064 6f65   if the path doe
-00004680: 736e 2774 2070 6f69 6e74 2074 6f20 616e  sn't point to an
-00004690: 2065 7869 7374 696e 6720 6669 6c65 2028   existing file (
-000046a0: 6f6e 6c79 2069 6620 6368 6563 6b3d 5472  only if check=Tr
-000046b0: 7565 290a 0a20 2020 2052 6574 7572 6e73  ue)..    Returns
-000046c0: 3a0a 2020 2020 2020 2020 616e 2065 7472  :.        an etr
-000046d0: 6565 2e5f 456c 656d 656e 7420 7468 6174  ee._Element that
-000046e0: 2063 616e 2062 6520 6170 7065 6e64 6564   can be appended
-000046f0: 2074 6f20 7468 6520 7061 7265 6e74 2072   to the parent r
-00004700: 6573 6f75 7263 6520 7769 7468 2072 6573  esource with res
-00004710: 6f75 7263 652e 6170 7065 6e64 286d 616b  ource.append(mak
-00004720: 655f 2a5f 7072 6f70 282e 2e2e 2929 0a0a  e_*_prop(...))..
-00004730: 2020 2020 4578 616d 706c 6573 3a0a 2020      Examples:.  
-00004740: 2020 2020 2020 3e3e 3e20 7265 736f 7572        >>> resour
-00004750: 6365 203d 2065 7863 656c 3278 6d6c 2e6d  ce = excel2xml.m
-00004760: 616b 655f 7265 736f 7572 6365 282e 2e2e  ake_resource(...
-00004770: 290a 2020 2020 2020 2020 3e3e 3e20 7265  ).        >>> re
-00004780: 736f 7572 6365 2e61 7070 656e 6428 6578  source.append(ex
-00004790: 6365 6c32 786d 6c2e 6d61 6b65 5f62 6974  cel2xml.make_bit
-000047a0: 7374 7265 616d 5f70 726f 7028 2264 6174  stream_prop("dat
-000047b0: 612f 696d 6167 6573 2f74 7265 652e 6a70  a/images/tree.jp
-000047c0: 6722 2929 0a20 2020 2020 2020 203e 3e3e  g")).        >>>
-000047d0: 2072 6f6f 742e 6170 7065 6e64 2872 6573   root.append(res
-000047e0: 6f75 7263 6529 0a0a 2020 2020 5365 6520  ource)..    See 
-000047f0: 6874 7470 733a 2f2f 646f 6373 2e64 6173  https://docs.das
-00004800: 6368 2e73 7769 7373 2f6c 6174 6573 742f  ch.swiss/latest/
-00004810: 4453 502d 544f 4f4c 532f 6669 6c65 2d66  DSP-TOOLS/file-f
-00004820: 6f72 6d61 7473 2f78 6d6c 2d64 6174 612d  ormats/xml-data-
-00004830: 6669 6c65 2f23 6269 7473 7472 6561 6d0a  file/#bitstream.
-00004840: 2020 2020 2222 220a 0a20 2020 2069 6620      """..    if 
-00004850: 6368 6563 6b20 616e 6420 6e6f 7420 5061  check and not Pa
-00004860: 7468 2870 6174 6829 2e69 735f 6669 6c65  th(path).is_file
-00004870: 2829 3a0a 2020 2020 2020 2020 6d73 6720  ():.        msg 
-00004880: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-00004890: 6622 4661 696c 6564 2076 616c 6964 6174  f"Failed validat
-000048a0: 696f 6e20 696e 2062 6974 7374 7265 616d  ion in bitstream
-000048b0: 2074 6167 206f 6620 7265 736f 7572 6365   tag of resource
-000048c0: 2027 7b63 616c 6c69 6e67 5f72 6573 6f75   '{calling_resou
-000048d0: 7263 657d 273a 2022 0a20 2020 2020 2020  rce}': ".       
-000048e0: 2020 2020 2066 2254 6865 2066 6f6c 6c6f       f"The follo
-000048f0: 7769 6e67 2070 6174 6820 646f 6573 6e27  wing path doesn'
-00004900: 7420 706f 696e 7420 746f 2061 2066 696c  t point to a fil
-00004910: 653a 207b 7061 7468 7d22 0a20 2020 2020  e: {path}".     
-00004920: 2020 2029 0a20 2020 2020 2020 2077 6172     ).        war
-00004930: 6e69 6e67 732e 7761 726e 2844 7370 546f  nings.warn(DspTo
-00004940: 6f6c 7355 7365 7257 6172 6e69 6e67 286d  olsUserWarning(m
-00004950: 7367 2929 0a20 2020 2070 726f 705f 203d  sg)).    prop_ =
-00004960: 2065 7472 6565 2e45 6c65 6d65 6e74 280a   etree.Element(.
-00004970: 2020 2020 2020 2020 227b 2573 7d62 6974          "{%s}bit
-00004980: 7374 7265 616d 2220 2520 786d 6c5f 6e61  stream" % xml_na
-00004990: 6d65 7370 6163 655f 6d61 705b 4e6f 6e65  mespace_map[None
-000049a0: 5d2c 0a20 2020 2020 2020 2070 6572 6d69  ],.        permi
-000049b0: 7373 696f 6e73 3d70 6572 6d69 7373 696f  ssions=permissio
-000049c0: 6e73 2c0a 2020 2020 2020 2020 6e73 6d61  ns,.        nsma
-000049d0: 703d 786d 6c5f 6e61 6d65 7370 6163 655f  p=xml_namespace_
-000049e0: 6d61 702c 0a20 2020 2029 0a20 2020 2070  map,.    ).    p
-000049f0: 726f 705f 2e74 6578 7420 3d20 7374 7228  rop_.text = str(
-00004a00: 7061 7468 290a 2020 2020 7265 7475 726e  path).    return
-00004a10: 2070 726f 705f 0a0a 0a64 6566 205f 666f   prop_...def _fo
-00004a20: 726d 6174 5f62 6f6f 6c28 0a20 2020 2075  rmat_bool(.    u
-00004a30: 6e66 6f72 6d61 7474 6564 3a20 556e 696f  nformatted: Unio
-00004a40: 6e5b 626f 6f6c 2c20 7374 722c 2069 6e74  n[bool, str, int
-00004a50: 2c20 666c 6f61 745d 2c0a 2020 2020 6e61  , float],.    na
-00004a60: 6d65 3a20 7374 722c 0a20 2020 2063 616c  me: str,.    cal
-00004a70: 6c69 6e67 5f72 6573 6f75 7263 653a 2073  ling_resource: s
-00004a80: 7472 2c0a 2920 2d3e 2073 7472 3a0a 2020  tr,.) -> str:.  
-00004a90: 2020 2222 220a 2020 2020 5468 6973 206d    """.    This m
-00004aa0: 6574 686f 6420 7461 6b65 7320 616e 2075  ethod takes an u
-00004ab0: 6e66 6f72 6d61 7474 6564 2062 6f6f 6c65  nformatted boole
-00004ac0: 616e 2d6c 696b 6520 7661 6c75 652c 2061  an-like value, a
-00004ad0: 6e64 2074 7261 6e73 666f 726d 7320 6974  nd transforms it
-00004ae0: 2069 6e74 6f20 7468 6520 7374 7269 6e67   into the string
-00004af0: 2076 616c 7565 7320 2274 7275 6522 206f   values "true" o
-00004b00: 7220 2266 616c 7365 222e 0a0a 2020 2020  r "false"...    
-00004b10: 4172 6773 3a0a 2020 2020 2020 2020 756e  Args:.        un
-00004b20: 666f 726d 6174 7465 643a 2062 6f6f 6c65  formatted: boole
-00004b30: 616e 2d6c 696b 6520 7661 6c75 650a 2020  an-like value.  
-00004b40: 2020 2020 2020 6e61 6d65 3a20 7072 6f70        name: prop
-00004b50: 6572 7479 206e 616d 652c 2066 6f72 2062  erty name, for b
-00004b60: 6574 7465 7220 6572 726f 7220 6d65 7373  etter error mess
-00004b70: 6167 6573 0a20 2020 2020 2020 2063 616c  ages.        cal
-00004b80: 6c69 6e67 5f72 6573 6f75 7263 653a 2072  ling_resource: r
-00004b90: 6573 6f75 7263 6520 6e61 6d65 2c20 666f  esource name, fo
-00004ba0: 7220 6265 7474 6572 2065 7272 6f72 206d  r better error m
-00004bb0: 6573 7361 6765 730a 0a20 2020 2052 6169  essages..    Rai
-00004bc0: 7365 733a 0a20 2020 2020 2020 2042 6173  ses:.        Bas
-00004bd0: 6545 7272 6f72 3a20 6966 2074 6865 2069  eError: if the i
-00004be0: 6e70 7574 2063 616e 6e6f 7420 6265 2074  nput cannot be t
-00004bf0: 7261 6e73 666f 726d 6564 2069 6e74 6f20  ransformed into 
-00004c00: 2274 7275 6522 2f22 6661 6c73 6522 0a0a  "true"/"false"..
-00004c10: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00004c20: 2020 2020 2022 7472 7565 2220 6966 2074       "true" if t
-00004c30: 6865 2069 6e70 7574 2069 7320 696e 2028  he input is in (
-00004c40: 5472 7565 2c20 2274 7275 6522 2c20 2231  True, "true", "1
-00004c50: 222c 2031 2c20 2279 6573 2229 3b20 2266  ", 1, "yes"); "f
-00004c60: 616c 7365 2220 6966 2069 6e70 7574 2069  alse" if input i
-00004c70: 7320 696e 2028 4661 6c73 652c 2022 6661  s in (False, "fa
-00004c80: 6c73 6522 2c20 2230 222c 2030 2c20 226e  lse", "0", 0, "n
-00004c90: 6f22 290a 2020 2020 2222 220a 2020 2020  o").    """.    
-00004ca0: 6966 2069 7369 6e73 7461 6e63 6528 756e  if isinstance(un
-00004cb0: 666f 726d 6174 7465 642c 2073 7472 293a  formatted, str):
-00004cc0: 0a20 2020 2020 2020 2075 6e66 6f72 6d61  .        unforma
-00004cd0: 7474 6564 203d 2075 6e66 6f72 6d61 7474  tted = unformatt
-00004ce0: 6564 2e6c 6f77 6572 2829 0a20 2020 2069  ed.lower().    i
-00004cf0: 6620 756e 666f 726d 6174 7465 6420 696e  f unformatted in
-00004d00: 2028 4661 6c73 652c 2022 6661 6c73 6522   (False, "false"
-00004d10: 2c20 2230 222c 2030 2c20 302e 302c 2022  , "0", 0, 0.0, "
-00004d20: 6e6f 2229 3a0a 2020 2020 2020 2020 7265  no"):.        re
-00004d30: 7475 726e 2022 6661 6c73 6522 0a20 2020  turn "false".   
-00004d40: 2065 6c69 6620 756e 666f 726d 6174 7465   elif unformatte
-00004d50: 6420 696e 2028 5472 7565 2c20 2274 7275  d in (True, "tru
-00004d60: 6522 2c20 2231 222c 2031 2c20 312e 302c  e", "1", 1, 1.0,
-00004d70: 2022 7965 7322 293a 0a20 2020 2020 2020   "yes"):.       
-00004d80: 2072 6574 7572 6e20 2274 7275 6522 0a20   return "true". 
-00004d90: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00004da0: 2072 6169 7365 2042 6173 6545 7272 6f72   raise BaseError
-00004db0: 280a 2020 2020 2020 2020 2020 2020 6622  (.            f"
-00004dc0: 4661 696c 6564 2076 616c 6964 6174 696f  Failed validatio
-00004dd0: 6e20 696e 2072 6573 6f75 7263 6520 277b  n in resource '{
-00004de0: 6361 6c6c 696e 675f 7265 736f 7572 6365  calling_resource
-00004df0: 7d27 2c20 7072 6f70 6572 7479 2027 7b6e  }', property '{n
-00004e00: 616d 657d 273a 2022 0a20 2020 2020 2020  ame}': ".       
-00004e10: 2020 2020 2066 2227 7b75 6e66 6f72 6d61       f"'{unforma
-00004e20: 7474 6564 7d27 2069 7320 6e6f 7420 6120  tted}' is not a 
-00004e30: 7661 6c69 6420 626f 6f6c 6561 6e2e 220a  valid boolean.".
-00004e40: 2020 2020 2020 2020 290a 0a0a 6465 6620          )...def 
-00004e50: 6d61 6b65 5f62 6f6f 6c65 616e 5f70 726f  make_boolean_pro
-00004e60: 7028 0a20 2020 206e 616d 653a 2073 7472  p(.    name: str
-00004e70: 2c0a 2020 2020 7661 6c75 653a 2055 6e69  ,.    value: Uni
-00004e80: 6f6e 5b50 726f 7065 7274 7945 6c65 6d65  on[PropertyEleme
-00004e90: 6e74 2c20 7374 722c 2069 6e74 2c20 626f  nt, str, int, bo
-00004ea0: 6f6c 5d2c 0a20 2020 2063 616c 6c69 6e67  ol],.    calling
-00004eb0: 5f72 6573 6f75 7263 653a 2073 7472 203d  _resource: str =
-00004ec0: 2022 222c 0a29 202d 3e20 6574 7265 652e   "",.) -> etree.
-00004ed0: 5f45 6c65 6d65 6e74 3a0a 2020 2020 2222  _Element:.    ""
-00004ee0: 220a 2020 2020 4d61 6b65 2061 203c 626f  ".    Make a <bo
-00004ef0: 6f6c 6561 6e2d 7072 6f70 3e20 6672 6f6d  olean-prop> from
-00004f00: 2061 2062 6f6f 6c65 616e 2076 616c 7565   a boolean value
-00004f10: 2e20 5468 6520 7661 6c75 6520 6361 6e20  . The value can 
-00004f20: 6265 2070 726f 7669 6465 6420 6469 7265  be provided dire
-00004f30: 6374 6c79 206f 7220 696e 7369 6465 2061  ctly or inside a
-00004f40: 2050 726f 7065 7274 7945 6c65 6d65 6e74   PropertyElement
-00004f50: 2e20 5468 650a 2020 2020 666f 6c6c 6f77  . The.    follow
-00004f60: 696e 6720 666f 726d 6174 7320 6172 6520  ing formats are 
-00004f70: 7375 7070 6f72 7465 643a 0a20 2020 2020  supported:.     
-00004f80: 2d20 7472 7565 3a20 2854 7275 652c 2022  - true: (True, "
-00004f90: 7472 7565 222c 2022 5472 7565 222c 2022  true", "True", "
-00004fa0: 3122 2c20 312c 2022 7965 7322 2c20 2259  1", 1, "yes", "Y
-00004fb0: 6573 2229 0a20 2020 2020 2d20 6661 6c73  es").     - fals
-00004fc0: 653a 2028 4661 6c73 652c 2022 6661 6c73  e: (False, "fals
-00004fd0: 6522 2c20 2246 616c 7365 222c 2022 3022  e", "False", "0"
-00004fe0: 2c20 302c 2022 6e6f 222c 2022 4e6f 2229  , 0, "no", "No")
-00004ff0: 0a0a 2020 2020 556e 6c65 7373 2070 726f  ..    Unless pro
-00005000: 7669 6465 6420 6173 2050 726f 7065 7274  vided as Propert
-00005010: 7945 6c65 6d65 6e74 2c20 7468 6520 7065  yElement, the pe
-00005020: 726d 6973 7369 6f6e 7320 6f66 2074 6865  rmissions of the
-00005030: 2076 616c 7565 2064 6566 6175 6c74 2074   value default t
-00005040: 6f20 2270 726f 702d 6465 6661 756c 7422  o "prop-default"
-00005050: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-00005060: 2020 2020 206e 616d 653a 2074 6865 206e       name: the n
-00005070: 616d 6520 6f66 2074 6869 7320 7072 6f70  ame of this prop
-00005080: 6572 7479 2061 7320 6465 6669 6e65 6420  erty as defined 
-00005090: 696e 2074 6865 206f 6e74 6f0a 2020 2020  in the onto.    
-000050a0: 2020 2020 7661 6c75 653a 2061 2062 6f6f      value: a boo
-000050b0: 6c65 616e 2076 616c 7565 2061 7320 7374  lean value as st
-000050c0: 722f 626f 6f6c 2f69 6e74 2c20 6f72 2061  r/bool/int, or a
-000050d0: 7320 7374 722f 626f 6f6c 2f69 6e74 2069  s str/bool/int i
-000050e0: 6e73 6964 6520 6120 5072 6f70 6572 7479  nside a Property
-000050f0: 456c 656d 656e 740a 2020 2020 2020 2020  Element.        
-00005100: 6361 6c6c 696e 675f 7265 736f 7572 6365  calling_resource
-00005110: 3a20 7468 6520 6e61 6d65 206f 6620 7468  : the name of th
-00005120: 6520 7061 7265 6e74 2072 6573 6f75 7263  e parent resourc
-00005130: 6520 2866 6f72 2062 6574 7465 7220 6572  e (for better er
-00005140: 726f 7220 6d65 7373 6167 6573 290a 0a20  ror messages).. 
-00005150: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
-00005160: 2020 2042 6173 6545 7272 6f72 3a20 6966     BaseError: if
-00005170: 2074 6865 2076 616c 7565 2069 7320 6e6f   the value is no
-00005180: 7420 6120 7661 6c69 6420 626f 6f6c 6561  t a valid boolea
-00005190: 6e0a 0a20 2020 2052 6574 7572 6e73 3a0a  n..    Returns:.
-000051a0: 2020 2020 2020 2020 616e 2065 7472 6565          an etree
-000051b0: 2e5f 456c 656d 656e 7420 7468 6174 2063  ._Element that c
-000051c0: 616e 2062 6520 6170 7065 6e64 6564 2074  an be appended t
-000051d0: 6f20 7468 6520 7061 7265 6e74 2072 6573  o the parent res
-000051e0: 6f75 7263 6520 7769 7468 2072 6573 6f75  ource with resou
-000051f0: 7263 652e 6170 7065 6e64 286d 616b 655f  rce.append(make_
-00005200: 2a5f 7072 6f70 282e 2e2e 2929 0a0a 2020  *_prop(...))..  
-00005210: 2020 4578 616d 706c 6573 3a0a 2020 2020    Examples:.    
-00005220: 2020 2020 3e3e 3e20 6578 6365 6c32 786d      >>> excel2xm
-00005230: 6c2e 6d61 6b65 5f62 6f6f 6c65 616e 5f70  l.make_boolean_p
-00005240: 726f 7028 223a 7465 7374 7072 6f70 6572  rop(":testproper
-00005250: 7479 222c 2022 6e6f 2229 0a20 2020 2020  ty", "no").     
-00005260: 2020 2020 2020 2020 2020 203c 626f 6f6c             <bool
-00005270: 6561 6e2d 7072 6f70 206e 616d 653d 223a  ean-prop name=":
-00005280: 7465 7374 7072 6f70 6572 7479 223e 0a20  testproperty">. 
-00005290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052a0: 2020 203c 626f 6f6c 6561 6e20 7065 726d     <boolean perm
-000052b0: 6973 7369 6f6e 733d 2270 726f 702d 6465  issions="prop-de
-000052c0: 6661 756c 7422 3e66 616c 7365 3c2f 626f  fault">false</bo
-000052d0: 6f6c 6561 6e3e 0a20 2020 2020 2020 2020  olean>.         
-000052e0: 2020 2020 2020 203c 2f62 6f6f 6c65 616e         </boolean
-000052f0: 2d70 726f 703e 0a20 2020 2020 2020 203e  -prop>.        >
-00005300: 3e3e 2065 7863 656c 3278 6d6c 2e6d 616b  >> excel2xml.mak
-00005310: 655f 626f 6f6c 6561 6e5f 7072 6f70 2822  e_boolean_prop("
-00005320: 3a74 6573 7470 726f 7065 7274 7922 2c20  :testproperty", 
-00005330: 6578 6365 6c32 786d 6c2e 5072 6f70 6572  excel2xml.Proper
-00005340: 7479 456c 656d 656e 7428 2231 222c 2070  tyElement("1", p
-00005350: 6572 6d69 7373 696f 6e73 3d22 7072 6f70  ermissions="prop
-00005360: 2d72 6573 7472 6963 7465 6422 2c20 636f  -restricted", co
-00005370: 6d6d 656e 743d 2265 7861 6d70 6c65 2229  mment="example")
-00005380: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00005390: 2020 3c62 6f6f 6c65 616e 2d70 726f 7020    <boolean-prop 
-000053a0: 6e61 6d65 3d22 3a74 6573 7470 726f 7065  name=":testprope
-000053b0: 7274 7922 3e0a 2020 2020 2020 2020 2020  rty">.          
-000053c0: 2020 2020 2020 2020 2020 3c62 6f6f 6c65            <boole
-000053d0: 616e 2070 6572 6d69 7373 696f 6e73 3d22  an permissions="
-000053e0: 7072 6f70 2d72 6573 7472 6963 7465 6422  prop-restricted"
-000053f0: 2063 6f6d 6d65 6e74 3d22 6578 616d 706c   comment="exampl
-00005400: 6522 3e74 7275 653c 2f62 6f6f 6c65 616e  e">true</boolean
-00005410: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00005420: 2020 3c2f 626f 6f6c 6561 6e2d 7072 6f70    </boolean-prop
-00005430: 3e0a 0a20 2020 2053 6565 2068 7474 7073  >..    See https
-00005440: 3a2f 2f64 6f63 732e 6461 7363 682e 7377  ://docs.dasch.sw
-00005450: 6973 732f 6c61 7465 7374 2f44 5350 2d54  iss/latest/DSP-T
-00005460: 4f4f 4c53 2f66 696c 652d 666f 726d 6174  OOLS/file-format
-00005470: 732f 786d 6c2d 6461 7461 2d66 696c 652f  s/xml-data-file/
-00005480: 2362 6f6f 6c65 616e 2d70 726f 700a 2020  #boolean-prop.  
-00005490: 2020 2222 220a 0a20 2020 2023 2076 616c    """..    # val
-000054a0: 6964 6174 6520 696e 7075 740a 2020 2020  idate input.    
-000054b0: 6966 2069 7369 6e73 7461 6e63 6528 7661  if isinstance(va
-000054c0: 6c75 652c 2050 726f 7065 7274 7945 6c65  lue, PropertyEle
-000054d0: 6d65 6e74 293a 0a20 2020 2020 2020 2076  ment):.        v
-000054e0: 616c 7565 5f6e 6577 203d 2064 6174 6163  alue_new = datac
-000054f0: 6c61 7373 6573 2e72 6570 6c61 6365 2876  lasses.replace(v
-00005500: 616c 7565 2c20 7661 6c75 653d 5f66 6f72  alue, value=_for
-00005510: 6d61 745f 626f 6f6c 2876 616c 7565 2e76  mat_bool(value.v
-00005520: 616c 7565 2c20 6e61 6d65 2c20 6361 6c6c  alue, name, call
-00005530: 696e 675f 7265 736f 7572 6365 2929 0a20  ing_resource)). 
-00005540: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
-00005550: 6365 2876 616c 7565 2c20 2873 7472 2c20  ce(value, (str, 
-00005560: 626f 6f6c 2c20 696e 7429 293a 0a20 2020  bool, int)):.   
-00005570: 2020 2020 2076 616c 7565 5f6e 6577 203d       value_new =
-00005580: 2050 726f 7065 7274 7945 6c65 6d65 6e74   PropertyElement
-00005590: 285f 666f 726d 6174 5f62 6f6f 6c28 7661  (_format_bool(va
-000055a0: 6c75 652c 206e 616d 652c 2063 616c 6c69  lue, name, calli
-000055b0: 6e67 5f72 6573 6f75 7263 6529 290a 2020  ng_resource)).  
-000055c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000055d0: 7261 6973 6520 4261 7365 4572 726f 7228  raise BaseError(
-000055e0: 0a20 2020 2020 2020 2020 2020 2066 2246  .            f"F
-000055f0: 6169 6c65 6420 7661 6c69 6461 7469 6f6e  ailed validation
-00005600: 2069 6e20 7265 736f 7572 6365 2027 7b63   in resource '{c
-00005610: 616c 6c69 6e67 5f72 6573 6f75 7263 657d  alling_resource}
-00005620: 272c 2070 726f 7065 7274 7920 277b 6e61  ', property '{na
-00005630: 6d65 7d27 3a20 277b 7661 6c75 657d 2720  me}': '{value}' 
-00005640: 6973 206e 6f74 2061 2076 616c 6964 2062  is not a valid b
-00005650: 6f6f 6c65 616e 2e22 0a20 2020 2020 2020  oolean.".       
-00005660: 2029 0a0a 2020 2020 2320 6d61 6b65 2078   )..    # make x
-00005670: 6d6c 2073 7472 7563 7475 7265 206f 6620  ml structure of 
-00005680: 7468 6520 7661 6c75 650a 2020 2020 7072  the value.    pr
-00005690: 6f70 5f20 3d20 6574 7265 652e 456c 656d  op_ = etree.Elem
-000056a0: 656e 7428 0a20 2020 2020 2020 2022 7b25  ent(.        "{%
-000056b0: 737d 626f 6f6c 6561 6e2d 7072 6f70 2220  s}boolean-prop" 
-000056c0: 2520 786d 6c5f 6e61 6d65 7370 6163 655f  % xml_namespace_
-000056d0: 6d61 705b 4e6f 6e65 5d2c 0a20 2020 2020  map[None],.     
-000056e0: 2020 206e 616d 653d 6e61 6d65 2c0a 2020     name=name,.  
-000056f0: 2020 2020 2020 6e73 6d61 703d 786d 6c5f        nsmap=xml_
-00005700: 6e61 6d65 7370 6163 655f 6d61 702c 0a20  namespace_map,. 
-00005710: 2020 2029 0a20 2020 206b 7761 7267 7320     ).    kwargs 
-00005720: 3d20 7b22 7065 726d 6973 7369 6f6e 7322  = {"permissions"
-00005730: 3a20 7661 6c75 655f 6e65 772e 7065 726d  : value_new.perm
-00005740: 6973 7369 6f6e 737d 0a20 2020 2069 6620  issions}.    if 
-00005750: 7661 6c75 655f 6e65 772e 636f 6d6d 656e  value_new.commen
-00005760: 7420 616e 6420 6368 6563 6b5f 6e6f 746e  t and check_notn
-00005770: 6128 7661 6c75 655f 6e65 772e 636f 6d6d  a(value_new.comm
-00005780: 656e 7429 3a0a 2020 2020 2020 2020 6b77  ent):.        kw
-00005790: 6172 6773 5b22 636f 6d6d 656e 7422 5d20  args["comment"] 
-000057a0: 3d20 7661 6c75 655f 6e65 772e 636f 6d6d  = value_new.comm
-000057b0: 656e 740a 2020 2020 7661 6c75 655f 203d  ent.    value_ =
-000057c0: 2065 7472 6565 2e45 6c65 6d65 6e74 280a   etree.Element(.
-000057d0: 2020 2020 2020 2020 227b 2573 7d62 6f6f          "{%s}boo
-000057e0: 6c65 616e 2220 2520 786d 6c5f 6e61 6d65  lean" % xml_name
-000057f0: 7370 6163 655f 6d61 705b 4e6f 6e65 5d2c  space_map[None],
-00005800: 0a20 2020 2020 2020 202a 2a6b 7761 7267  .        **kwarg
-00005810: 732c 2020 2320 7479 7065 3a20 6967 6e6f  s,  # type: igno
-00005820: 7265 5b61 7267 2d74 7970 655d 0a20 2020  re[arg-type].   
-00005830: 2020 2020 206e 736d 6170 3d78 6d6c 5f6e       nsmap=xml_n
-00005840: 616d 6573 7061 6365 5f6d 6170 2c0a 2020  amespace_map,.  
-00005850: 2020 290a 2020 2020 7661 6c75 655f 2e74    ).    value_.t
-00005860: 6578 7420 3d20 7374 7228 7661 6c75 655f  ext = str(value_
-00005870: 6e65 772e 7661 6c75 6529 0a20 2020 2070  new.value).    p
-00005880: 726f 705f 2e61 7070 656e 6428 7661 6c75  rop_.append(valu
-00005890: 655f 290a 0a20 2020 2072 6574 7572 6e20  e_)..    return 
-000058a0: 7072 6f70 5f0a 0a0a 6465 6620 6d61 6b65  prop_...def make
-000058b0: 5f63 6f6c 6f72 5f70 726f 7028 0a20 2020  _color_prop(.   
-000058c0: 206e 616d 653a 2073 7472 2c0a 2020 2020   name: str,.    
-000058d0: 7661 6c75 653a 2055 6e69 6f6e 5b50 726f  value: Union[Pro
-000058e0: 7065 7274 7945 6c65 6d65 6e74 2c20 7374  pertyElement, st
-000058f0: 722c 2049 7465 7261 626c 655b 556e 696f  r, Iterable[Unio
-00005900: 6e5b 5072 6f70 6572 7479 456c 656d 656e  n[PropertyElemen
-00005910: 742c 2073 7472 5d5d 5d2c 0a20 2020 2063  t, str]]],.    c
-00005920: 616c 6c69 6e67 5f72 6573 6f75 7263 653a  alling_resource:
-00005930: 2073 7472 203d 2022 222c 0a29 202d 3e20   str = "",.) -> 
-00005940: 6574 7265 652e 5f45 6c65 6d65 6e74 3a0a  etree._Element:.
-00005950: 2020 2020 2222 220a 2020 2020 4d61 6b65      """.    Make
-00005960: 2061 203c 636f 6c6f 722d 7072 6f70 3e20   a <color-prop> 
-00005970: 6672 6f6d 206f 6e65 206f 7220 6d6f 7265  from one or more
-00005980: 2063 6f6c 6f72 732e 2054 6865 2063 6f6c   colors. The col
-00005990: 6f72 2873 2920 6361 6e20 6265 2070 726f  or(s) can be pro
-000059a0: 7669 6465 6420 6173 2073 7472 696e 6720  vided as string 
-000059b0: 6f72 2061 7320 5072 6f70 6572 7479 456c  or as PropertyEl
-000059c0: 656d 656e 7420 7769 7468 2061 0a20 2020  ement with a.   
-000059d0: 2073 7472 696e 6720 696e 7369 6465 2e20   string inside. 
-000059e0: 4966 2070 726f 7669 6465 6420 6173 2073  If provided as s
-000059f0: 7472 696e 672c 2074 6865 2070 6572 6d69  tring, the permi
-00005a00: 7373 696f 6e73 2064 6566 6175 6c74 2074  ssions default t
-00005a10: 6f20 2270 726f 702d 6465 6661 756c 7422  o "prop-default"
-00005a20: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-00005a30: 2020 2020 206e 616d 653a 2074 6865 206e       name: the n
-00005a40: 616d 6520 6f66 2074 6869 7320 7072 6f70  ame of this prop
-00005a50: 6572 7479 2061 7320 6465 6669 6e65 6420  erty as defined 
-00005a60: 696e 2074 6865 206f 6e74 6f0a 2020 2020  in the onto.    
-00005a70: 2020 2020 7661 6c75 653a 206f 6e65 206f      value: one o
-00005a80: 7220 6d6f 7265 2044 5350 2063 6f6c 6f72  r more DSP color
-00005a90: 2873 292c 2061 7320 7374 7269 6e67 2f50  (s), as string/P
-00005aa0: 726f 7065 7274 7945 6c65 6d65 6e74 2c20  ropertyElement, 
-00005ab0: 6f72 2061 7320 6974 6572 6162 6c65 206f  or as iterable o
-00005ac0: 6620 7374 7269 6e67 732f 5072 6f70 6572  f strings/Proper
-00005ad0: 7479 456c 656d 656e 7473 0a20 2020 2020  tyElements.     
-00005ae0: 2020 2063 616c 6c69 6e67 5f72 6573 6f75     calling_resou
-00005af0: 7263 653a 2074 6865 206e 616d 6520 6f66  rce: the name of
-00005b00: 2074 6865 2070 6172 656e 7420 7265 736f   the parent reso
-00005b10: 7572 6365 2028 666f 7220 6265 7474 6572  urce (for better
-00005b20: 2065 7272 6f72 206d 6573 7361 6765 7329   error messages)
-00005b30: 0a0a 2020 2020 5761 726e 733a 0a20 2020  ..    Warns:.   
-00005b40: 2020 2020 2049 6620 7468 6520 7661 6c75       If the valu
-00005b50: 6520 6973 206e 6f74 2061 2076 616c 6964  e is not a valid
-00005b60: 2063 6f6c 6f72 0a0a 2020 2020 5265 7475   color..    Retu
-00005b70: 726e 733a 0a20 2020 2020 2020 2061 6e20  rns:.        an 
-00005b80: 6574 7265 652e 5f45 6c65 6d65 6e74 2074  etree._Element t
-00005b90: 6861 7420 6361 6e20 6265 2061 7070 656e  hat can be appen
-00005ba0: 6465 6420 746f 2074 6865 2070 6172 656e  ded to the paren
-00005bb0: 7420 7265 736f 7572 6365 2077 6974 6820  t resource with 
-00005bc0: 7265 736f 7572 6365 2e61 7070 656e 6428  resource.append(
-00005bd0: 6d61 6b65 5f2a 5f70 726f 7028 2e2e 2e29  make_*_prop(...)
-00005be0: 290a 0a20 2020 2045 7861 6d70 6c65 733a  )..    Examples:
-00005bf0: 0a20 2020 2020 2020 203e 3e3e 2065 7863  .        >>> exc
-00005c00: 656c 3278 6d6c 2e6d 616b 655f 636f 6c6f  el2xml.make_colo
-00005c10: 725f 7072 6f70 2822 3a74 6573 7470 726f  r_prop(":testpro
-00005c20: 7065 7274 7922 2c20 2223 3030 6666 3636  perty", "#00ff66
-00005c30: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00005c40: 2020 203c 636f 6c6f 722d 7072 6f70 206e     <color-prop n
-00005c50: 616d 653d 223a 7465 7374 7072 6f70 6572  ame=":testproper
-00005c60: 7479 223e 0a20 2020 2020 2020 2020 2020  ty">.           
-00005c70: 2020 2020 2020 2020 203c 636f 6c6f 7220           <color 
-00005c80: 7065 726d 6973 7369 6f6e 733d 2270 726f  permissions="pro
-00005c90: 702d 6465 6661 756c 7422 3e23 3030 6666  p-default">#00ff
-00005ca0: 3636 3c2f 636f 6c6f 723e 0a20 2020 2020  66</color>.     
-00005cb0: 2020 2020 2020 2020 2020 203c 2f63 6f6c             </col
-00005cc0: 6f72 2d70 726f 703e 0a20 2020 2020 2020  or-prop>.       
-00005cd0: 203e 3e3e 2065 7863 656c 3278 6d6c 2e6d   >>> excel2xml.m
-00005ce0: 616b 655f 636f 6c6f 725f 7072 6f70 2822  ake_color_prop("
-00005cf0: 3a74 6573 7470 726f 7065 7274 7922 2c20  :testproperty", 
-00005d00: 6578 6365 6c32 786d 6c2e 5072 6f70 6572  excel2xml.Proper
-00005d10: 7479 456c 656d 656e 7428 2223 3030 6666  tyElement("#00ff
-00005d20: 3636 222c 2070 6572 6d69 7373 696f 6e73  66", permissions
-00005d30: 3d22 7072 6f70 2d72 6573 7472 6963 7465  ="prop-restricte
-00005d40: 6422 2c20 636f 6d6d 656e 743d 2265 7861  d", comment="exa
-00005d50: 6d70 6c65 2229 290a 2020 2020 2020 2020  mple")).        
-00005d60: 2020 2020 2020 2020 3c63 6f6c 6f72 2d70          <color-p
-00005d70: 726f 7020 6e61 6d65 3d22 3a74 6573 7470  rop name=":testp
-00005d80: 726f 7065 7274 7922 3e0a 2020 2020 2020  roperty">.      
-00005d90: 2020 2020 2020 2020 2020 2020 2020 3c63                <c
-00005da0: 6f6c 6f72 2070 6572 6d69 7373 696f 6e73  olor permissions
-00005db0: 3d22 7072 6f70 2d72 6573 7472 6963 7465  ="prop-restricte
-00005dc0: 6422 2063 6f6d 6d65 6e74 3d22 6578 616d  d" comment="exam
-00005dd0: 706c 6522 3e23 3030 6666 3636 3c2f 636f  ple">#00ff66</co
-00005de0: 6c6f 723e 0a20 2020 2020 2020 2020 2020  lor>.           
-00005df0: 2020 2020 203c 2f63 6f6c 6f72 2d70 726f       </color-pro
-00005e00: 703e 0a20 2020 2020 2020 203e 3e3e 2065  p>.        >>> e
-00005e10: 7863 656c 3278 6d6c 2e6d 616b 655f 636f  xcel2xml.make_co
-00005e20: 6c6f 725f 7072 6f70 2822 3a74 6573 7470  lor_prop(":testp
-00005e30: 726f 7065 7274 7922 2c20 5b22 2330 3066  roperty", ["#00f
-00005e40: 6636 3622 2c20 2223 3030 3030 3030 225d  f66", "#000000"]
-00005e50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00005e60: 2020 3c63 6f6c 6f72 2d70 726f 7020 6e61    <color-prop na
-00005e70: 6d65 3d22 3a74 6573 7470 726f 7065 7274  me=":testpropert
-00005e80: 7922 3e0a 2020 2020 2020 2020 2020 2020  y">.            
-00005e90: 2020 2020 2020 2020 3c63 6f6c 6f72 2070          <color p
-00005ea0: 6572 6d69 7373 696f 6e73 3d22 7072 6f70  ermissions="prop
-00005eb0: 2d64 6566 6175 6c74 223e 2330 3066 6636  -default">#00ff6
-00005ec0: 363c 2f63 6f6c 6f72 3e0a 2020 2020 2020  6</color>.      
-00005ed0: 2020 2020 2020 2020 2020 2020 2020 3c63                <c
-00005ee0: 6f6c 6f72 2070 6572 6d69 7373 696f 6e73  olor permissions
-00005ef0: 3d22 7072 6f70 2d64 6566 6175 6c74 223e  ="prop-default">
-00005f00: 2330 3030 3030 303c 2f63 6f6c 6f72 3e0a  #000000</color>.
-00005f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f20: 3c2f 636f 6c6f 722d 7072 6f70 3e0a 0a20  </color-prop>.. 
-00005f30: 2020 2053 6565 2068 7474 7073 3a2f 2f64     See https://d
-00005f40: 6f63 732e 6461 7363 682e 7377 6973 732f  ocs.dasch.swiss/
-00005f50: 6c61 7465 7374 2f44 5350 2d54 4f4f 4c53  latest/DSP-TOOLS
-00005f60: 2f66 696c 652d 666f 726d 6174 732f 786d  /file-formats/xm
-00005f70: 6c2d 6461 7461 2d66 696c 652f 2363 6f6c  l-data-file/#col
-00005f80: 6f72 2d70 726f 700a 2020 2020 2222 220a  or-prop.    """.
-00005f90: 0a20 2020 2023 2063 6865 636b 2074 6865  .    # check the
-00005fa0: 2069 6e70 7574 3a20 7072 6570 6172 6520   input: prepare 
-00005fb0: 6120 6c69 7374 2077 6974 6820 7661 6c69  a list with vali
-00005fc0: 6420 7661 6c75 6573 0a20 2020 2076 616c  d values.    val
-00005fd0: 7565 7320 3d20 7072 6570 6172 655f 7661  ues = prepare_va
-00005fe0: 6c75 6528 7661 6c75 6529 0a0a 2020 2020  lue(value)..    
-00005ff0: 2320 6368 6563 6b20 7661 6c75 6520 7479  # check value ty
-00006000: 7065 0a20 2020 2066 6f72 2076 616c 2069  pe.    for val i
-00006010: 6e20 7661 6c75 6573 3a0a 2020 2020 2020  n values:.      
-00006020: 2020 6966 206e 6f74 2072 6567 6578 2e73    if not regex.s
-00006030: 6561 7263 6828 7222 5e23 5b30 2d39 612d  earch(r"^#[0-9a-
-00006040: 665d 7b36 7d24 222c 2073 7472 2876 616c  f]{6}$", str(val
-00006050: 2e76 616c 7565 292e 7374 7269 7028 292c  .value).strip(),
-00006060: 2066 6c61 6773 3d72 6567 6578 2e49 474e   flags=regex.IGN
-00006070: 4f52 4543 4153 4529 3a0a 2020 2020 2020  ORECASE):.      
-00006080: 2020 2020 2020 6d73 6720 3d20 280a 2020        msg = (.  
-00006090: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-000060a0: 4661 696c 6564 2076 616c 6964 6174 696f  Failed validatio
-000060b0: 6e20 696e 2072 6573 6f75 7263 6520 277b  n in resource '{
-000060c0: 6361 6c6c 696e 675f 7265 736f 7572 6365  calling_resource
-000060d0: 7d27 2c20 7072 6f70 6572 7479 2027 7b6e  }', property '{n
-000060e0: 616d 657d 273a 2022 0a20 2020 2020 2020  ame}': ".       
-000060f0: 2020 2020 2020 2020 2066 2227 7b76 616c           f"'{val
-00006100: 2e76 616c 7565 7d27 2069 7320 6e6f 7420  .value}' is not 
-00006110: 6120 7661 6c69 6420 636f 6c6f 722e 220a  a valid color.".
-00006120: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00006130: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
-00006140: 6773 2e77 6172 6e28 4473 7054 6f6f 6c73  gs.warn(DspTools
-00006150: 5573 6572 5761 726e 696e 6728 6d73 6729  UserWarning(msg)
-00006160: 290a 0a20 2020 2023 206d 616b 6520 786d  )..    # make xm
-00006170: 6c20 7374 7275 6374 7572 6520 6f66 2074  l structure of t
-00006180: 6865 2076 616c 6964 2076 616c 7565 730a  he valid values.
-00006190: 2020 2020 7072 6f70 5f20 3d20 6574 7265      prop_ = etre
-000061a0: 652e 456c 656d 656e 7428 0a20 2020 2020  e.Element(.     
-000061b0: 2020 2022 7b25 737d 636f 6c6f 722d 7072     "{%s}color-pr
-000061c0: 6f70 2220 2520 786d 6c5f 6e61 6d65 7370  op" % xml_namesp
-000061d0: 6163 655f 6d61 705b 4e6f 6e65 5d2c 0a20  ace_map[None],. 
-000061e0: 2020 2020 2020 206e 616d 653d 6e61 6d65         name=name
-000061f0: 2c0a 2020 2020 2020 2020 6e73 6d61 703d  ,.        nsmap=
-00006200: 786d 6c5f 6e61 6d65 7370 6163 655f 6d61  xml_namespace_ma
-00006210: 702c 0a20 2020 2029 0a20 2020 2066 6f72  p,.    ).    for
-00006220: 2076 616c 2069 6e20 7661 6c75 6573 3a0a   val in values:.
-00006230: 2020 2020 2020 2020 6b77 6172 6773 203d          kwargs =
-00006240: 207b 2270 6572 6d69 7373 696f 6e73 223a   {"permissions":
-00006250: 2076 616c 2e70 6572 6d69 7373 696f 6e73   val.permissions
-00006260: 7d0a 2020 2020 2020 2020 6966 2076 616c  }.        if val
-00006270: 2e63 6f6d 6d65 6e74 2061 6e64 2063 6865  .comment and che
-00006280: 636b 5f6e 6f74 6e61 2876 616c 2e63 6f6d  ck_notna(val.com
-00006290: 6d65 6e74 293a 0a20 2020 2020 2020 2020  ment):.         
-000062a0: 2020 206b 7761 7267 735b 2263 6f6d 6d65     kwargs["comme
-000062b0: 6e74 225d 203d 2076 616c 2e63 6f6d 6d65  nt"] = val.comme
-000062c0: 6e74 0a20 2020 2020 2020 2076 616c 7565  nt.        value
-000062d0: 5f20 3d20 6574 7265 652e 456c 656d 656e  _ = etree.Elemen
-000062e0: 7428 0a20 2020 2020 2020 2020 2020 2022  t(.            "
-000062f0: 7b25 737d 636f 6c6f 7222 2025 2078 6d6c  {%s}color" % xml
-00006300: 5f6e 616d 6573 7061 6365 5f6d 6170 5b4e  _namespace_map[N
-00006310: 6f6e 655d 2c0a 2020 2020 2020 2020 2020  one],.          
-00006320: 2020 2a2a 6b77 6172 6773 2c20 2023 2074    **kwargs,  # t
-00006330: 7970 653a 2069 676e 6f72 655b 6172 672d  ype: ignore[arg-
-00006340: 7479 7065 5d0a 2020 2020 2020 2020 2020  type].          
-00006350: 2020 6e73 6d61 703d 786d 6c5f 6e61 6d65    nsmap=xml_name
-00006360: 7370 6163 655f 6d61 702c 0a20 2020 2020  space_map,.     
-00006370: 2020 2029 0a20 2020 2020 2020 2076 616c     ).        val
-00006380: 7565 5f2e 7465 7874 203d 2073 7472 2876  ue_.text = str(v
-00006390: 616c 2e76 616c 7565 292e 7374 7269 7028  al.value).strip(
-000063a0: 290a 2020 2020 2020 2020 7072 6f70 5f2e  ).        prop_.
-000063b0: 6170 7065 6e64 2876 616c 7565 5f29 0a0a  append(value_)..
-000063c0: 2020 2020 7265 7475 726e 2070 726f 705f      return prop_
-000063d0: 0a0a 0a64 6566 206d 616b 655f 6461 7465  ...def make_date
-000063e0: 5f70 726f 7028 0a20 2020 206e 616d 653a  _prop(.    name:
-000063f0: 2073 7472 2c0a 2020 2020 7661 6c75 653a   str,.    value:
-00006400: 2055 6e69 6f6e 5b50 726f 7065 7274 7945   Union[PropertyE
-00006410: 6c65 6d65 6e74 2c20 7374 722c 2049 7465  lement, str, Ite
-00006420: 7261 626c 655b 556e 696f 6e5b 5072 6f70  rable[Union[Prop
-00006430: 6572 7479 456c 656d 656e 742c 2073 7472  ertyElement, str
-00006440: 5d5d 5d2c 0a20 2020 2063 616c 6c69 6e67  ]]],.    calling
-00006450: 5f72 6573 6f75 7263 653a 2073 7472 203d  _resource: str =
-00006460: 2022 222c 0a29 202d 3e20 6574 7265 652e   "",.) -> etree.
-00006470: 5f45 6c65 6d65 6e74 3a0a 2020 2020 2222  _Element:.    ""
-00006480: 220a 2020 2020 4d61 6b65 2061 203c 6461  ".    Make a <da
-00006490: 7465 2d70 726f 703e 2066 726f 6d20 6f6e  te-prop> from on
-000064a0: 6520 6f72 206d 6f72 6520 6461 7465 732f  e or more dates/
-000064b0: 6461 7465 2072 616e 6765 732e 2054 6865  date ranges. The
-000064c0: 2064 6174 6528 7329 2063 616e 2062 6520   date(s) can be 
-000064d0: 7072 6f76 6964 6564 2061 7320 7374 7269  provided as stri
-000064e0: 6e67 206f 7220 6173 2050 726f 7065 7274  ng or as Propert
-000064f0: 7945 6c65 6d65 6e74 0a20 2020 2077 6974  yElement.    wit
-00006500: 6820 6120 7374 7269 6e67 2069 6e73 6964  h a string insid
-00006510: 652e 2049 6620 7072 6f76 6964 6564 2061  e. If provided a
-00006520: 7320 7374 7269 6e67 2c20 7468 6520 7065  s string, the pe
-00006530: 726d 6973 7369 6f6e 7320 6465 6661 756c  rmissions defaul
-00006540: 7420 746f 2022 7072 6f70 2d64 6566 6175  t to "prop-defau
-00006550: 6c74 222e 0a0a 2020 2020 4172 6773 3a0a  lt"...    Args:.
-00006560: 2020 2020 2020 2020 6e61 6d65 3a20 7468          name: th
-00006570: 6520 6e61 6d65 206f 6620 7468 6973 2070  e name of this p
-00006580: 726f 7065 7274 7920 6173 2064 6566 696e  roperty as defin
-00006590: 6564 2069 6e20 7468 6520 6f6e 746f 0a20  ed in the onto. 
-000065a0: 2020 2020 2020 2076 616c 7565 3a20 6f6e         value: on
-000065b0: 6520 6f72 206d 6f72 6520 4453 5020 6461  e or more DSP da
-000065c0: 7465 732c 2061 7320 7374 7269 6e67 2f50  tes, as string/P
-000065d0: 726f 7065 7274 7945 6c65 6d65 6e74 2c20  ropertyElement, 
-000065e0: 6f72 2061 7320 6974 6572 6162 6c65 206f  or as iterable o
-000065f0: 6620 7374 7269 6e67 732f 5072 6f70 6572  f strings/Proper
-00006600: 7479 456c 656d 656e 7473 0a20 2020 2020  tyElements.     
-00006610: 2020 2063 616c 6c69 6e67 5f72 6573 6f75     calling_resou
-00006620: 7263 653a 2074 6865 206e 616d 6520 6f66  rce: the name of
-00006630: 2074 6865 2070 6172 656e 7420 7265 736f   the parent reso
-00006640: 7572 6365 2028 666f 7220 6265 7474 6572  urce (for better
-00006650: 2065 7272 6f72 206d 6573 7361 6765 7329   error messages)
-00006660: 0a0a 2020 2020 5761 726e 733a 0a20 2020  ..    Warns:.   
-00006670: 2020 2020 2049 6620 7468 6520 7661 6c75       If the valu
-00006680: 6520 6973 206e 6f74 2061 2076 616c 6964  e is not a valid
-00006690: 2044 5350 2064 6174 650a 0a20 2020 2052   DSP date..    R
-000066a0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-000066b0: 616e 2065 7472 6565 2e5f 456c 656d 656e  an etree._Elemen
-000066c0: 7420 7468 6174 2063 616e 2062 6520 6170  t that can be ap
-000066d0: 7065 6e64 6564 2074 6f20 7468 6520 7061  pended to the pa
-000066e0: 7265 6e74 2072 6573 6f75 7263 6520 7769  rent resource wi
-000066f0: 7468 2072 6573 6f75 7263 652e 6170 7065  th resource.appe
-00006700: 6e64 286d 616b 655f 2a5f 7072 6f70 282e  nd(make_*_prop(.
-00006710: 2e2e 2929 0a0a 2020 2020 4578 616d 706c  ..))..    Exampl
-00006720: 6573 3a0a 2020 2020 2020 2020 3e3e 3e20  es:.        >>> 
-00006730: 6578 6365 6c32 786d 6c2e 6d61 6b65 5f64  excel2xml.make_d
-00006740: 6174 655f 7072 6f70 2822 3a74 6573 7470  ate_prop(":testp
-00006750: 726f 7065 7274 7922 2c20 2247 5245 474f  roperty", "GREGO
-00006760: 5249 414e 3a43 453a 3230 3134 2d30 312d  RIAN:CE:2014-01-
-00006770: 3331 2229 0a20 2020 2020 2020 2020 2020  31").           
-00006780: 2020 2020 203c 6461 7465 2d70 726f 7020       <date-prop 
-00006790: 6e61 6d65 3d22 3a74 6573 7470 726f 7065  name=":testprope
-000067a0: 7274 7922 3e0a 2020 2020 2020 2020 2020  rty">.          
-000067b0: 2020 2020 2020 2020 2020 3c64 6174 6520            <date 
-000067c0: 7065 726d 6973 7369 6f6e 733d 2270 726f  permissions="pro
-000067d0: 702d 6465 6661 756c 7422 3e47 5245 474f  p-default">GREGO
-000067e0: 5249 414e 3a43 453a 3230 3134 2d30 312d  RIAN:CE:2014-01-
-000067f0: 3331 3c2f 6461 7465 3e0a 2020 2020 2020  31</date>.      
-00006800: 2020 2020 2020 2020 2020 3c2f 6461 7465            </date
-00006810: 2d70 726f 703e 0a20 2020 2020 2020 203e  -prop>.        >
-00006820: 3e3e 2065 7863 656c 3278 6d6c 2e6d 616b  >> excel2xml.mak
-00006830: 655f 6461 7465 5f70 726f 7028 223a 7465  e_date_prop(":te
-00006840: 7374 7072 6f70 6572 7479 222c 2065 7863  stproperty", exc
-00006850: 656c 3278 6d6c 2e50 726f 7065 7274 7945  el2xml.PropertyE
-00006860: 6c65 6d65 6e74 2822 4752 4547 4f52 4941  lement("GREGORIA
-00006870: 4e3a 4345 3a32 3031 342d 3031 2d33 3122  N:CE:2014-01-31"
-00006880: 2c20 7065 726d 6973 7369 6f6e 733d 2270  , permissions="p
-00006890: 726f 702d 7265 7374 7269 6374 6564 222c  rop-restricted",
-000068a0: 2063 6f6d 6d65 6e74 3d22 6578 616d 706c   comment="exampl
-000068b0: 6522 2929 0a20 2020 2020 2020 2020 2020  e")).           
-000068c0: 2020 2020 203c 6461 7465 2d70 726f 7020       <date-prop 
-000068d0: 6e61 6d65 3d22 3a74 6573 7470 726f 7065  name=":testprope
-000068e0: 7274 7922 3e0a 2020 2020 2020 2020 2020  rty">.          
-000068f0: 2020 2020 2020 2020 2020 3c64 6174 6520            <date 
-00006900: 7065 726d 6973 7369 6f6e 733d 2270 726f  permissions="pro
-00006910: 702d 7265 7374 7269 6374 6564 2220 636f  p-restricted" co
-00006920: 6d6d 656e 743d 2265 7861 6d70 6c65 223e  mment="example">
-00006930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006940: 2020 2020 2020 2020 2047 5245 474f 5249           GREGORI
-00006950: 414e 3a43 453a 3230 3134 2d30 312d 3331  AN:CE:2014-01-31
-00006960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006970: 2020 2020 203c 2f64 6174 653e 0a20 2020       </date>.   
-00006980: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-00006990: 6174 652d 7072 6f70 3e0a 2020 2020 2020  ate-prop>.      
-000069a0: 2020 3e3e 3e20 6578 6365 6c32 786d 6c2e    >>> excel2xml.
-000069b0: 6d61 6b65 5f64 6174 655f 7072 6f70 2822  make_date_prop("
-000069c0: 3a74 6573 7470 726f 7065 7274 7922 2c20  :testproperty", 
-000069d0: 5b22 4752 4547 4f52 4941 4e3a 4345 3a31  ["GREGORIAN:CE:1
-000069e0: 3933 302d 3039 2d30 323a 4345 3a31 3933  930-09-02:CE:193
-000069f0: 302d 3039 2d30 3322 2c20 2247 5245 474f  0-09-03", "GREGO
-00006a00: 5249 414e 3a43 453a 3139 3330 2d30 392d  RIAN:CE:1930-09-
-00006a10: 3032 3a43 453a 3139 3330 2d30 392d 3033  02:CE:1930-09-03
-00006a20: 225d 290a 2020 2020 2020 2020 2020 2020  "]).            
-00006a30: 2020 2020 3c64 6174 652d 7072 6f70 206e      <date-prop n
-00006a40: 616d 653d 223a 7465 7374 7072 6f70 6572  ame=":testproper
-00006a50: 7479 223e 0a20 2020 2020 2020 2020 2020  ty">.           
-00006a60: 2020 2020 2020 2020 203c 6461 7465 2070           <date p
-00006a70: 6572 6d69 7373 696f 6e73 3d22 7072 6f70  ermissions="prop
-00006a80: 2d64 6566 6175 6c74 223e 0a20 2020 2020  -default">.     
+00000320: 6964 6174 655f 786d 6c5f 6669 6c65 0a0a  idate_xml_file..
+00000330: 2320 7275 6666 3a20 6e6f 7161 3a20 4535  # ruff: noqa: E5
+00000340: 3031 2c20 5550 3033 3120 286c 696e 652d  01, UP031 (line-
+00000350: 746f 6f2d 6c6f 6e67 2c20 7573 6520 662d  too-long, use f-
+00000360: 7374 7269 6e67 206f 7665 7220 7065 7263  string over perc
+00000370: 656e 7420 666f 726d 6174 7469 6e67 290a  ent formatting).
+00000380: 0a0a 786d 6c5f 6e61 6d65 7370 6163 655f  ..xml_namespace_
+00000390: 6d61 7020 3d20 7b4e 6f6e 653a 2022 6874  map = {None: "ht
+000003a0: 7470 733a 2f2f 6461 7363 682e 7377 6973  tps://dasch.swis
+000003b0: 732f 7363 6865 6d61 222c 2022 7873 6922  s/schema", "xsi"
+000003c0: 3a20 2268 7474 703a 2f2f 7777 772e 7733  : "http://www.w3
+000003d0: 2e6f 7267 2f32 3030 312f 584d 4c53 6368  .org/2001/XMLSch
+000003e0: 656d 612d 696e 7374 616e 6365 227d 0a0a  ema-instance"}..
+000003f0: 0a64 6566 206d 616b 655f 7873 645f 6964  .def make_xsd_id
+00000400: 5f63 6f6d 7061 7469 626c 6528 7374 7269  _compatible(stri
+00000410: 6e67 3a20 7374 7229 202d 3e20 7374 723a  ng: str) -> str:
+00000420: 0a20 2020 2022 2222 0a20 2020 204d 616b  .    """.    Mak
+00000430: 6520 6120 7374 7269 6e67 2063 6f6d 7061  e a string compa
+00000440: 7469 626c 6520 7769 7468 2074 6865 2063  tible with the c
+00000450: 6f6e 7374 7261 696e 7473 206f 6620 7873  onstraints of xs
+00000460: 643a 4944 2c20 736f 2074 6861 7420 6974  d:ID, so that it
+00000470: 2063 616e 2062 6520 7573 6564 2061 7320   can be used as 
+00000480: 2269 6422 2061 7474 7269 6275 7465 206f  "id" attribute o
+00000490: 6620 6120 3c72 6573 6f75 7263 653e 0a20  f a <resource>. 
+000004a0: 2020 2074 6167 2e20 416e 2078 7364 3a49     tag. An xsd:I
+000004b0: 4420 6d75 7374 206e 6f74 2063 6f6e 7461  D must not conta
+000004c0: 696e 2073 7065 6369 616c 2063 6861 7261  in special chara
+000004d0: 6374 6572 732c 2061 6e64 2069 7420 6d75  cters, and it mu
+000004e0: 7374 2062 6520 756e 6971 7565 2069 6e20  st be unique in 
+000004f0: 7468 6520 646f 6375 6d65 6e74 2e0a 0a20  the document... 
+00000500: 2020 2054 6869 7320 6d65 7468 6f64 2072     This method r
+00000510: 6570 6c61 6365 7320 7468 6520 696c 6c65  eplaces the ille
+00000520: 6761 6c20 6368 6172 6163 7465 7273 2062  gal characters b
+00000530: 7920 225f 2220 616e 6420 6170 7065 6e64  y "_" and append
+00000540: 7320 6120 7261 6e64 6f6d 2063 6f6d 706f  s a random compo
+00000550: 6e65 6e74 2074 6f20 7468 6520 7374 7269  nent to the stri
+00000560: 6e67 2074 6f20 6d61 6b65 2069 7420 756e  ng to make it un
+00000570: 6971 7565 2e0a 0a20 2020 2054 6865 2073  ique...    The s
+00000580: 7472 696e 6720 6d75 7374 2063 6f6e 7461  tring must conta
+00000590: 696e 2061 7420 6c65 6173 7420 6f6e 6520  in at least one 
+000005a0: 556e 6963 6f64 6520 6c65 7474 6572 2028  Unicode letter (
+000005b0: 6d61 7463 6869 6e67 2074 6865 2072 6567  matching the reg
+000005c0: 6578 2060 605c 5c70 7b4c 7d60 6029 2c20  ex ``\\p{L}``), 
+000005d0: 756e 6465 7273 636f 7265 2c20 212c 203f  underscore, !, ?
+000005e0: 2c20 6f72 206e 756d 6265 722c 0a20 2020  , or number,.   
+000005f0: 2062 7574 206d 7573 7420 6e6f 7420 6265   but must not be
+00000600: 2022 4e6f 6e65 222c 2022 3c4e 413e 222c   "None", "<NA>",
+00000610: 2022 4e2f 4122 2c20 6f72 2022 2d22 2e20   "N/A", or "-". 
+00000620: 4f74 6865 7277 6973 652c 2061 2042 6173  Otherwise, a Bas
+00000630: 6545 7272 6f72 2077 696c 6c20 6265 2072  eError will be r
+00000640: 6169 7365 642e 0a0a 2020 2020 4172 6773  aised...    Args
+00000650: 3a0a 2020 2020 2020 2020 7374 7269 6e67  :.        string
+00000660: 3a20 696e 7075 7420 7374 7269 6e67 0a0a  : input string..
+00000670: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
+00000680: 2020 2020 4261 7365 4572 726f 723a 2069      BaseError: i
+00000690: 6620 7468 6520 696e 7075 7420 6361 6e6e  f the input cann
+000006a0: 6f74 2062 6520 7472 616e 7366 6f72 6d65  ot be transforme
+000006b0: 6420 746f 2061 6e20 7873 643a 4944 0a0a  d to an xsd:ID..
+000006c0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+000006d0: 2020 2020 2061 6e20 7873 6420 4944 2062       an xsd ID b
+000006e0: 6173 6564 206f 6e20 7468 6520 696e 7075  ased on the inpu
+000006f0: 7420 7374 7269 6e67 0a20 2020 2022 2222  t string.    """
+00000700: 0a0a 2020 2020 6966 206e 6f74 2069 7369  ..    if not isi
+00000710: 6e73 7461 6e63 6528 7374 7269 6e67 2c20  nstance(string, 
+00000720: 7374 7229 206f 7220 6e6f 7420 6368 6563  str) or not chec
+00000730: 6b5f 6e6f 746e 6128 7374 7269 6e67 293a  k_notna(string):
+00000740: 0a20 2020 2020 2020 2072 6169 7365 2042  .        raise B
+00000750: 6173 6545 7272 6f72 2866 2254 6865 2069  aseError(f"The i
+00000760: 6e70 7574 2027 7b73 7472 696e 677d 2720  nput '{string}' 
+00000770: 6361 6e6e 6f74 2062 6520 7472 616e 7366  cannot be transf
+00000780: 6f72 6d65 6420 746f 2061 6e20 7873 643a  ormed to an xsd:
+00000790: 4944 2229 0a0a 2020 2020 2320 6966 2073  ID")..    # if s
+000007a0: 7461 7274 206f 6620 7374 7269 6e67 2069  tart of string i
+000007b0: 7320 6e65 6974 6865 7220 6c65 7474 6572  s neither letter
+000007c0: 206e 6f72 2075 6e64 6572 7363 6f72 652c   nor underscore,
+000007d0: 2061 6464 2061 6e20 756e 6465 7273 636f   add an undersco
+000007e0: 7265 0a20 2020 2072 6573 203d 2072 6567  re.    res = reg
+000007f0: 6578 2e73 7562 2872 225e 283f 3d5b 5e41  ex.sub(r"^(?=[^A
+00000800: 2d5a 612d 7a5f 5d29 222c 2022 5f22 2c20  -Za-z_])", "_", 
+00000810: 7374 7269 6e67 290a 0a20 2020 2023 2072  string)..    # r
+00000820: 6570 6c61 6365 2061 6c6c 2069 6c6c 6567  eplace all illeg
+00000830: 616c 2063 6861 7261 6374 6572 7320 6279  al characters by
+00000840: 2075 6e64 6572 7363 6f72 650a 2020 2020   underscore.    
+00000850: 7265 7320 3d20 7265 6765 782e 7375 6228  res = regex.sub(
+00000860: 7222 5b5e 5c77 5f5c 2d2e 5d22 2c20 225f  r"[^\w_\-.]", "_
+00000870: 222c 2072 6573 2c20 666c 6167 733d 7265  ", res, flags=re
+00000880: 6765 782e 4153 4349 4929 0a0a 2020 2020  gex.ASCII)..    
+00000890: 2320 6164 6420 7575 6964 0a20 2020 205f  # add uuid.    _
+000008a0: 7575 6964 203d 2075 7569 642e 7575 6964  uuid = uuid.uuid
+000008b0: 3428 290a 2020 2020 7265 7320 3d20 6622  4().    res = f"
+000008c0: 7b72 6573 7d5f 7b5f 7575 6964 7d22 0a0a  {res}_{_uuid}"..
+000008d0: 2020 2020 7265 7475 726e 2072 6573 0a0a      return res..
+000008e0: 0a64 6566 205f 6669 6e64 5f66 7265 6e63  .def _find_frenc
+000008f0: 685f 6263 5f64 6174 6528 0a20 2020 2073  h_bc_date(.    s
+00000900: 7472 696e 673a 2073 7472 2c0a 2020 2020  tring: str,.    
+00000910: 6c6f 6f6b 6265 6869 6e64 3a20 7374 722c  lookbehind: str,
+00000920: 0a20 2020 206c 6f6f 6b61 6865 6164 3a20  .    lookahead: 
+00000930: 7374 722c 0a29 202d 3e20 4f70 7469 6f6e  str,.) -> Option
+00000940: 616c 5b73 7472 5d3a 0a20 2020 2066 7265  al[str]:.    fre
+00000950: 6e63 685f 6263 5f72 6567 6578 203d 2072  nch_bc_regex = r
+00000960: 2261 7628 3f3a 5c2e 207c 5c2e 7c20 294a  "av(?:\. |\.| )J
+00000970: 5c2e 3f2d 3f43 5c2e 3f22 0a20 2020 2069  \.?-?C\.?".    i
+00000980: 6620 6e6f 7420 7265 6765 782e 7365 6172  f not regex.sear
+00000990: 6368 2866 7265 6e63 685f 6263 5f72 6567  ch(french_bc_reg
+000009a0: 6578 2c20 7374 7269 6e67 293a 0a20 2020  ex, string):.   
+000009b0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+000009c0: 0a0a 2020 2020 7965 6172 5f72 6567 6578  ..    year_regex
+000009d0: 203d 2072 225c 647b 312c 357d 220a 2020   = r"\d{1,5}".  
+000009e0: 2020 7365 705f 7265 6765 7820 3d20 7222    sep_regex = r"
+000009f0: 203f 2d20 3f22 0a0a 2020 2020 7965 6172   ?- ?"..    year
+00000a00: 5f72 616e 6765 5f72 6567 6578 203d 2072  _range_regex = r
+00000a10: 6622 7b6c 6f6f 6b62 6568 696e 647d 287b  f"{lookbehind}({
+00000a20: 7965 6172 5f72 6567 6578 7d29 7b73 6570  year_regex}){sep
+00000a30: 5f72 6567 6578 7d28 7b79 6561 725f 7265  _regex}({year_re
+00000a40: 6765 787d 2920 7b66 7265 6e63 685f 6263  gex}) {french_bc
+00000a50: 5f72 6567 6578 7d7b 6c6f 6f6b 6168 6561  _regex}{lookahea
+00000a60: 647d 220a 2020 2020 7965 6172 5f72 616e  d}".    year_ran
+00000a70: 6765 203d 2072 6567 6578 2e73 6561 7263  ge = regex.searc
+00000a80: 6828 7965 6172 5f72 616e 6765 5f72 6567  h(year_range_reg
+00000a90: 6578 2c20 7374 7269 6e67 290a 2020 2020  ex, string).    
+00000aa0: 6966 2079 6561 725f 7261 6e67 653a 0a20  if year_range:. 
+00000ab0: 2020 2020 2020 2073 7461 7274 5f79 6561         start_yea
+00000ac0: 7220 3d20 696e 7428 7965 6172 5f72 616e  r = int(year_ran
+00000ad0: 6765 2e67 726f 7570 2831 2929 0a20 2020  ge.group(1)).   
+00000ae0: 2020 2020 2065 6e64 5f79 6561 7220 3d20       end_year = 
+00000af0: 696e 7428 7965 6172 5f72 616e 6765 2e67  int(year_range.g
+00000b00: 726f 7570 2832 2929 0a20 2020 2020 2020  roup(2)).       
+00000b10: 2069 6620 656e 645f 7965 6172 203e 2073   if end_year > s
+00000b20: 7461 7274 5f79 6561 723a 0a20 2020 2020  tart_year:.     
+00000b30: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+00000b40: 6e65 0a20 2020 2020 2020 2072 6574 7572  ne.        retur
+00000b50: 6e20 6622 4752 4547 4f52 4941 4e3a 4243  n f"GREGORIAN:BC
+00000b60: 3a7b 7374 6172 745f 7965 6172 7d3a 4243  :{start_year}:BC
+00000b70: 3a7b 656e 645f 7965 6172 7d22 0a0a 2020  :{end_year}"..  
+00000b80: 2020 7369 6e67 6c65 5f79 6561 725f 7265    single_year_re
+00000b90: 6765 7820 3d20 7266 227b 6c6f 6f6b 6265  gex = rf"{lookbe
+00000ba0: 6869 6e64 7d28 7b79 6561 725f 7265 6765  hind}({year_rege
+00000bb0: 787d 2920 7b66 7265 6e63 685f 6263 5f72  x}) {french_bc_r
+00000bc0: 6567 6578 7d7b 6c6f 6f6b 6168 6561 647d  egex}{lookahead}
+00000bd0: 220a 2020 2020 7369 6e67 6c65 5f79 6561  ".    single_yea
+00000be0: 7220 3d20 7265 6765 782e 7365 6172 6368  r = regex.search
+00000bf0: 2873 696e 676c 655f 7965 6172 5f72 6567  (single_year_reg
+00000c00: 6578 2c20 7374 7269 6e67 290a 2020 2020  ex, string).    
+00000c10: 6966 2073 696e 676c 655f 7965 6172 3a0a  if single_year:.
+00000c20: 2020 2020 2020 2020 7374 6172 745f 7965          start_ye
+00000c30: 6172 203d 2069 6e74 2873 696e 676c 655f  ar = int(single_
+00000c40: 7965 6172 2e67 726f 7570 2831 2929 0a20  year.group(1)). 
+00000c50: 2020 2020 2020 2072 6574 7572 6e20 6622         return f"
+00000c60: 4752 4547 4f52 4941 4e3a 4243 3a7b 7374  GREGORIAN:BC:{st
+00000c70: 6172 745f 7965 6172 7d3a 4243 3a7b 7374  art_year}:BC:{st
+00000c80: 6172 745f 7965 6172 7d22 0a0a 2020 2020  art_year}"..    
+00000c90: 7265 7475 726e 204e 6f6e 650a 0a0a 6465  return None...de
+00000ca0: 6620 6669 6e64 5f64 6174 655f 696e 5f73  f find_date_in_s
+00000cb0: 7472 696e 6728 7374 7269 6e67 3a20 7374  tring(string: st
+00000cc0: 7229 202d 3e20 4f70 7469 6f6e 616c 5b73  r) -> Optional[s
+00000cd0: 7472 5d3a 0a20 2020 2022 2222 0a20 2020  tr]:.    """.   
+00000ce0: 2043 6865 636b 7320 6966 2061 2073 7472   Checks if a str
+00000cf0: 696e 6720 636f 6e74 6169 6e73 2061 2064  ing contains a d
+00000d00: 6174 6520 7661 6c75 6520 2873 696e 676c  ate value (singl
+00000d10: 6520 6461 7465 2c20 6f72 2064 6174 6520  e date, or date 
+00000d20: 7261 6e67 6529 2c0a 2020 2020 616e 6420  range),.    and 
+00000d30: 7265 7475 726e 7320 7468 6520 6669 7273  returns the firs
+00000d40: 7420 666f 756e 6420 6461 7465 2061 7320  t found date as 
+00000d50: 4453 502d 666f 726d 6174 7465 6420 7374  DSP-formatted st
+00000d60: 7269 6e67 2e0a 2020 2020 5265 7475 726e  ring..    Return
+00000d70: 7320 4e6f 6e65 2069 6620 6e6f 2064 6174  s None if no dat
+00000d80: 6520 7761 7320 666f 756e 642e 0a0a 2020  e was found...  
+00000d90: 2020 4e6f 7465 733a 0a20 2020 2020 2020    Notes:.       
+00000da0: 202d 2041 6c6c 2064 6174 6573 2061 7265   - All dates are
+00000db0: 2069 6e74 6572 7072 6574 6564 2069 6e20   interpreted in 
+00000dc0: 7468 6520 4368 7269 7374 6961 6e20 6572  the Christian er
+00000dd0: 6120 616e 6420 7468 6520 4772 6567 6f72  a and the Gregor
+00000de0: 6961 6e20 6361 6c65 6e64 6172 2e0a 2020  ian calendar..  
+00000df0: 2020 2020 2020 2d20 4243 2064 6174 6573        - BC dates
+00000e00: 2061 7265 206f 6e6c 7920 7375 7070 6f72   are only suppor
+00000e10: 7465 6420 696e 2046 7265 6e63 6820 6e6f  ted in French no
+00000e20: 7461 7469 6f6e 2028 652e 672e 2031 3030  tation (e.g. 100
+00000e30: 302d 3930 3020 6176 2e20 4a2e 2d43 2e29  0-900 av. J.-C.)
+00000e40: 2e0a 2020 2020 2020 2020 2d20 5468 6520  ..        - The 
+00000e50: 7965 6172 7320 3030 3030 2d32 3939 3920  years 0000-2999 
+00000e60: 6172 6520 7375 7070 6f72 7465 642c 2069  are supported, i
+00000e70: 6e20 332f 342d 6469 6769 7420 666f 726d  n 3/4-digit form
+00000e80: 2e0a 2020 2020 2020 2020 2d20 4461 7465  ..        - Date
+00000e90: 7320 7772 6974 7465 6e20 7769 7468 2073  s written with s
+00000ea0: 6c61 7368 6573 2061 7265 2061 6c77 6179  lashes are alway
+00000eb0: 7320 696e 7465 7270 7265 7465 6420 696e  s interpreted in
+00000ec0: 2061 2045 7572 6f70 6561 6e20 6d61 6e6e   a European mann
+00000ed0: 6572 3a20 352f 3131 2f32 3032 3120 6973  er: 5/11/2021 is
+00000ee0: 2074 6865 2035 7468 206f 6620 4e6f 7665   the 5th of Nove
+00000ef0: 6d62 6572 2e0a 2020 2020 2020 2020 2d20  mber..        - 
+00000f00: 496e 2074 6865 2045 7572 6f70 6561 6e20  In the European 
+00000f10: 6e6f 7461 7469 6f6e 2c20 322d 6469 6769  notation, 2-digi
+00000f20: 7420 7965 6172 7320 6172 6520 6578 7061  t years are expa
+00000f30: 6e64 6564 2074 6f20 3420 6469 6769 7473  nded to 4 digits
+00000f40: 2c20 7769 7468 2074 6865 2063 7572 7265  , with the curre
+00000f50: 6e74 2079 6561 7220 6173 2077 6174 6572  nt year as water
+00000f60: 7368 6564 3a0a 2020 2020 2020 2020 2020  shed:.          
+00000f70: 2020 2d20 3330 2e34 2e32 3420 2d3e 2033    - 30.4.24 -> 3
+00000f80: 302e 3034 2e32 3032 340a 2020 2020 2020  0.04.2024.      
+00000f90: 2020 2020 2020 2d20 3330 2e34 2e32 3520        - 30.4.25 
+00000fa0: 2d3e 2033 302e 3034 2e31 3932 350a 0a20  -> 30.04.1925.. 
+00000fb0: 2020 2043 7572 7265 6e74 6c79 2073 7570     Currently sup
+00000fc0: 706f 7274 6564 2064 6174 6520 666f 726d  ported date form
+00000fd0: 6174 733a 0a20 2020 2020 2020 202d 2030  ats:.        - 0
+00000fe0: 3437 362d 3039 2d30 3420 2d3e 2047 5245  476-09-04 -> GRE
+00000ff0: 474f 5249 414e 3a43 453a 3034 3736 2d30  GORIAN:CE:0476-0
+00001000: 392d 3034 3a43 453a 3034 3736 2d30 392d  9-04:CE:0476-09-
+00001010: 3034 0a20 2020 2020 2020 202d 2030 3437  04.        - 047
+00001020: 365f 3039 5f30 3420 2d3e 2047 5245 474f  6_09_04 -> GREGO
+00001030: 5249 414e 3a43 453a 3034 3736 2d30 392d  RIAN:CE:0476-09-
+00001040: 3034 3a43 453a 3034 3736 2d30 392d 3034  04:CE:0476-09-04
+00001050: 0a20 2020 2020 2020 202d 2033 302e 342e  .        - 30.4.
+00001060: 3230 3231 202d 3e20 4752 4547 4f52 4941  2021 -> GREGORIA
+00001070: 4e3a 4345 3a32 3032 312d 3034 2d33 303a  N:CE:2021-04-30:
+00001080: 4345 3a32 3032 312d 3034 2d33 300a 2020  CE:2021-04-30.  
+00001090: 2020 2020 2020 2d20 3330 2e34 2e32 3120        - 30.4.21 
+000010a0: 2d3e 2047 5245 474f 5249 414e 3a43 453a  -> GREGORIAN:CE:
+000010b0: 3230 3231 2d30 342d 3330 3a43 453a 3230  2021-04-30:CE:20
+000010c0: 3231 2d30 342d 3330 0a20 2020 2020 2020  21-04-30.       
+000010d0: 202d 2035 2f31 312f 3230 3231 202d 3e20   - 5/11/2021 -> 
+000010e0: 4752 4547 4f52 4941 4e3a 4345 3a32 3032  GREGORIAN:CE:202
+000010f0: 312d 3131 2d30 353a 4345 3a32 3032 312d  1-11-05:CE:2021-
+00001100: 3131 2d30 350a 2020 2020 2020 2020 2d20  11-05.        - 
+00001110: 4a61 6e20 3236 2c20 3139 3933 202d 3e20  Jan 26, 1993 -> 
+00001120: 4752 4547 4f52 4941 4e3a 4345 3a31 3939  GREGORIAN:CE:199
+00001130: 332d 3031 2d32 363a 4345 3a31 3939 332d  3-01-26:CE:1993-
+00001140: 3031 2d32 360a 2020 2020 2020 2020 2d20  01-26.        - 
+00001150: 3238 2e32 2e2d 312e 3132 2e31 3531 3520  28.2.-1.12.1515 
+00001160: 2d3e 2047 5245 474f 5249 414e 3a43 453a  -> GREGORIAN:CE:
+00001170: 3135 3135 2d30 322d 3238 3a43 453a 3135  1515-02-28:CE:15
+00001180: 3135 2d31 322d 3031 0a20 2020 2020 2020  15-12-01.       
+00001190: 202d 2032 352e 2d32 362e 322e 3038 3030   - 25.-26.2.0800
+000011a0: 202d 3e20 4752 4547 4f52 4941 4e3a 4345   -> GREGORIAN:CE
+000011b0: 3a30 3830 302d 3032 2d32 353a 4345 3a30  :0800-02-25:CE:0
+000011c0: 3830 302d 3032 2d32 360a 2020 2020 2020  800-02-26.      
+000011d0: 2020 2d20 312e 392e 3230 3232 2d33 2e31    - 1.9.2022-3.1
+000011e0: 2e32 3032 3420 2d3e 2047 5245 474f 5249  .2024 -> GREGORI
+000011f0: 414e 3a43 453a 3230 3232 2d30 392d 3031  AN:CE:2022-09-01
+00001200: 3a43 453a 3230 3234 2d30 312d 3033 0a20  :CE:2024-01-03. 
+00001210: 2020 2020 2020 202d 2031 3834 3820 2d3e         - 1848 ->
+00001220: 2047 5245 474f 5249 414e 3a43 453a 3138   GREGORIAN:CE:18
+00001230: 3438 3a43 453a 3138 3438 0a20 2020 2020  48:CE:1848.     
+00001240: 2020 202d 2031 3834 392f 3138 3530 202d     - 1849/1850 -
+00001250: 3e20 4752 4547 4f52 4941 4e3a 4345 3a31  > GREGORIAN:CE:1
+00001260: 3834 393a 4345 3a31 3835 300a 2020 2020  849:CE:1850.    
+00001270: 2020 2020 2d20 3138 3439 2f35 3020 2d3e      - 1849/50 ->
+00001280: 2047 5245 474f 5249 414e 3a43 453a 3138   GREGORIAN:CE:18
+00001290: 3439 3a43 453a 3138 3530 0a20 2020 2020  49:CE:1850.     
+000012a0: 2020 202d 2031 3834 352d 3530 202d 3e20     - 1845-50 -> 
+000012b0: 4752 4547 4f52 4941 4e3a 4345 3a31 3834  GREGORIAN:CE:184
+000012c0: 353a 4345 3a31 3835 300a 2020 2020 2020  5:CE:1850.      
+000012d0: 2020 2d20 3834 302d 3530 202d 3e20 4752    - 840-50 -> GR
+000012e0: 4547 4f52 4941 4e3a 4345 3a38 3430 3a43  EGORIAN:CE:840:C
+000012f0: 453a 3835 300a 2020 2020 2020 2020 2d20  E:850.        - 
+00001300: 3834 302d 3120 2d3e 2047 5245 474f 5249  840-1 -> GREGORI
+00001310: 414e 3a43 453a 3834 303a 4345 3a38 3431  AN:CE:840:CE:841
+00001320: 0a20 2020 2020 2020 202d 2031 3030 302d  .        - 1000-
+00001330: 3930 3020 6176 2e20 4a2e 2d43 2e20 2d3e  900 av. J.-C. ->
+00001340: 2047 5245 474f 5249 414e 3a42 433a 3130   GREGORIAN:BC:10
+00001350: 3030 3a42 433a 3930 300a 2020 2020 2020  00:BC:900.      
+00001360: 2020 2d20 3435 2061 762e 204a 2e2d 432e    - 45 av. J.-C.
+00001370: 202d 3e20 4752 4547 4f52 4941 4e3a 4243   -> GREGORIAN:BC
+00001380: 3a34 353a 4243 3a34 350a 0a20 2020 2041  :45:BC:45..    A
+00001390: 7267 733a 0a20 2020 2020 2020 2073 7472  rgs:.        str
+000013a0: 696e 673a 2073 7472 696e 6720 746f 2063  ing: string to c
+000013b0: 6865 636b 0a0a 2020 2020 5265 7475 726e  heck..    Return
+000013c0: 733a 0a20 2020 2020 2020 2044 5350 2d66  s:.        DSP-f
+000013d0: 6f72 6d61 7474 6564 2064 6174 6520 7374  ormatted date st
+000013e0: 7269 6e67 2c20 6f72 204e 6f6e 650a 0a20  ring, or None.. 
+000013f0: 2020 2045 7861 6d70 6c65 733a 0a20 2020     Examples:.   
+00001400: 2020 2020 203e 3e3e 2069 6620 6669 6e64       >>> if find
+00001410: 5f64 6174 655f 696e 5f73 7472 696e 6728  _date_in_string(
+00001420: 726f 775b 2245 706f 6368 225d 293a 0a20  row["Epoch"]):. 
+00001430: 2020 2020 2020 203e 3e3e 2020 2020 2072         >>>     r
+00001440: 6573 6f75 7263 652e 6170 7065 6e64 286d  esource.append(m
+00001450: 616b 655f 6461 7465 5f70 726f 7028 223a  ake_date_prop(":
+00001460: 6861 7344 6174 6522 2c20 6669 6e64 5f64  hasDate", find_d
+00001470: 6174 655f 696e 5f73 7472 696e 6728 726f  ate_in_string(ro
+00001480: 775b 2245 706f 6368 225d 2929 0a0a 2020  w["Epoch"]))..  
+00001490: 2020 5365 6520 6874 7470 733a 2f2f 646f    See https://do
+000014a0: 6373 2e64 6173 6368 2e73 7769 7373 2f6c  cs.dasch.swiss/l
+000014b0: 6174 6573 742f 4453 502d 544f 4f4c 532f  atest/DSP-TOOLS/
+000014c0: 6669 6c65 2d66 6f72 6d61 7473 2f78 6d6c  file-formats/xml
+000014d0: 2d64 6174 612d 6669 6c65 2f23 6461 7465  -data-file/#date
+000014e0: 2d70 726f 700a 2020 2020 2222 220a 0a20  -prop.    """.. 
+000014f0: 2020 2023 2073 616e 6974 697a 6520 696e     # sanitize in
+00001500: 7075 742c 206a 7573 7420 696e 2063 6173  put, just in cas
+00001510: 6520 7468 6174 2074 6865 206d 6574 686f  e that the metho
+00001520: 6420 7761 7320 6361 6c6c 6564 206f 6e20  d was called on 
+00001530: 616e 2065 6d70 7479 206f 7220 4e2f 4120  an empty or N/A 
+00001540: 6365 6c6c 0a20 2020 2069 6620 6e6f 7420  cell.    if not 
+00001550: 6368 6563 6b5f 6e6f 746e 6128 7374 7269  check_notna(stri
+00001560: 6e67 293a 0a20 2020 2020 2020 2072 6574  ng):.        ret
+00001570: 7572 6e20 4e6f 6e65 0a20 2020 2074 7279  urn None.    try
+00001580: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00001590: 205f 6669 6e64 5f64 6174 655f 696e 5f73   _find_date_in_s
+000015a0: 7472 696e 675f 7468 726f 7769 6e67 2873  tring_throwing(s
+000015b0: 7472 696e 6729 0a20 2020 2065 7863 6570  tring).    excep
+000015c0: 7420 5661 6c75 6545 7272 6f72 3a0a 2020  t ValueError:.  
+000015d0: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+000015e0: 650a 0a0a 5f6d 6f6e 7468 735f 6469 6374  e..._months_dict
+000015f0: 203d 207b 0a20 2020 2022 4a61 6e75 6172   = {.    "Januar
+00001600: 7922 3a20 312c 0a20 2020 2022 4a61 6e22  y": 1,.    "Jan"
+00001610: 3a20 312c 0a20 2020 2022 4665 6272 7561  : 1,.    "Februa
+00001620: 7279 223a 2032 2c0a 2020 2020 2246 6562  ry": 2,.    "Feb
+00001630: 223a 2032 2c0a 2020 2020 224d 6172 6368  ": 2,.    "March
+00001640: 223a 2033 2c0a 2020 2020 224d 6172 223a  ": 3,.    "Mar":
+00001650: 2033 2c0a 2020 2020 2241 7072 696c 223a   3,.    "April":
+00001660: 2034 2c0a 2020 2020 2241 7072 223a 2034   4,.    "Apr": 4
+00001670: 2c0a 2020 2020 224d 6179 223a 2035 2c0a  ,.    "May": 5,.
+00001680: 2020 2020 224a 756e 6522 3a20 362c 0a20      "June": 6,. 
+00001690: 2020 2022 4a75 6e22 3a20 362c 0a20 2020     "Jun": 6,.   
+000016a0: 2022 4a75 6c79 223a 2037 2c0a 2020 2020   "July": 7,.    
+000016b0: 224a 756c 223a 2037 2c0a 2020 2020 2241  "Jul": 7,.    "A
+000016c0: 7567 7573 7422 3a20 382c 0a20 2020 2022  ugust": 8,.    "
+000016d0: 4175 6722 3a20 382c 0a20 2020 2022 5365  Aug": 8,.    "Se
+000016e0: 7074 656d 6265 7222 3a20 392c 0a20 2020  ptember": 9,.   
+000016f0: 2022 5365 7074 223a 2039 2c0a 2020 2020   "Sept": 9,.    
+00001700: 224f 6374 6f62 6572 223a 2031 302c 0a20  "October": 10,. 
+00001710: 2020 2022 4f63 7422 3a20 3130 2c0a 2020     "Oct": 10,.  
+00001720: 2020 224e 6f76 656d 6265 7222 3a20 3131    "November": 11
+00001730: 2c0a 2020 2020 224e 6f76 223a 2031 312c  ,.    "Nov": 11,
+00001740: 0a20 2020 2022 4465 6365 6d62 6572 223a  .    "December":
+00001750: 2031 322c 0a20 2020 2022 4465 6322 3a20   12,.    "Dec": 
+00001760: 3132 2c0a 7d0a 0a0a 6465 6620 5f66 696e  12,.}...def _fin
+00001770: 645f 6461 7465 5f69 6e5f 7374 7269 6e67  d_date_in_string
+00001780: 5f74 6872 6f77 696e 6728 7374 7269 6e67  _throwing(string
+00001790: 3a20 7374 7229 202d 3e20 7374 7220 7c20  : str) -> str | 
+000017a0: 4e6f 6e65 3a0a 2020 2020 2222 220a 2020  None:.    """.  
+000017b0: 2020 5468 6973 2066 756e 6374 696f 6e20    This function 
+000017c0: 6973 2074 6865 2073 616d 6520 6173 2066  is the same as f
+000017d0: 696e 645f 6461 7465 5f69 6e5f 7374 7269  ind_date_in_stri
+000017e0: 6e67 2829 2c20 6275 7420 6d61 7920 7261  ng(), but may ra
+000017f0: 6973 6520 6120 5661 6c75 6545 7272 6f72  ise a ValueError
+00001800: 2069 6e73 7465 6164 206f 6620 7265 7475   instead of retu
+00001810: 726e 696e 6720 4e6f 6e65 2e0a 2020 2020  rning None..    
+00001820: 2222 220a 2020 2020 7965 6172 5f72 6567  """.    year_reg
+00001830: 6578 203d 2072 2228 5b30 2d32 5d3f 5b30  ex = r"([0-2]?[0
+00001840: 2d39 5d5b 302d 395d 5b30 2d39 5d29 220a  -9][0-9][0-9])".
+00001850: 2020 2020 7965 6172 5f72 6567 6578 5f32      year_regex_2
+00001860: 5f6f 725f 345f 6469 6769 7473 203d 2072  _or_4_digits = r
+00001870: 2228 283f 3a5b 302d 325d 3f5b 302d 395d  "((?:[0-2]?[0-9]
+00001880: 293f 5b30 2d39 5d5b 302d 395d 2922 0a20  )?[0-9][0-9])". 
+00001890: 2020 206d 6f6e 7468 5f72 6567 6578 203d     month_regex =
+000018a0: 2072 2228 5b30 2d31 5d3f 5b30 2d39 5d29   r"([0-1]?[0-9])
+000018b0: 220a 2020 2020 6461 795f 7265 6765 7820  ".    day_regex 
+000018c0: 3d20 7222 285b 302d 335d 3f5b 302d 395d  = r"([0-3]?[0-9]
+000018d0: 2922 0a20 2020 2073 6570 5f72 6567 6578  )".    sep_regex
+000018e0: 203d 2072 225b 5c2e 2f5d 220a 2020 2020   = r"[\./]".    
+000018f0: 6c6f 6f6b 6265 6869 6e64 203d 2072 2228  lookbehind = r"(
+00001900: 3f3c 215b 302d 3941 2d5a 612d 7a5d 2922  ?<![0-9A-Za-z])"
+00001910: 0a20 2020 206c 6f6f 6b61 6865 6164 203d  .    lookahead =
+00001920: 2072 2228 3f21 5b30 2d39 412d 5a61 2d7a   r"(?![0-9A-Za-z
+00001930: 5d29 220a 0a20 2020 2069 6620 6672 656e  ])"..    if fren
+00001940: 6368 5f62 635f 6461 7465 203a 3d20 5f66  ch_bc_date := _f
+00001950: 696e 645f 6672 656e 6368 5f62 635f 6461  ind_french_bc_da
+00001960: 7465 2873 7472 696e 673d 7374 7269 6e67  te(string=string
+00001970: 2c20 6c6f 6f6b 6265 6869 6e64 3d6c 6f6f  , lookbehind=loo
+00001980: 6b62 6568 696e 642c 206c 6f6f 6b61 6865  kbehind, lookahe
+00001990: 6164 3d6c 6f6f 6b61 6865 6164 293a 0a20  ad=lookahead):. 
+000019a0: 2020 2020 2020 2072 6574 7572 6e20 6672         return fr
+000019b0: 656e 6368 5f62 635f 6461 7465 0a0a 2020  ench_bc_date..  
+000019c0: 2020 2320 7465 6d70 6c61 7465 3a20 3230    # template: 20
+000019d0: 3231 2d30 312d 3031 207c 2032 3031 355f  21-01-01 | 2015_
+000019e0: 3031 5f30 320a 2020 2020 6973 6f5f 6461  01_02.    iso_da
+000019f0: 7465 203d 2072 6567 6578 2e73 6561 7263  te = regex.searc
+00001a00: 6828 7266 227b 6c6f 6f6b 6265 6869 6e64  h(rf"{lookbehind
+00001a10: 7d7b 7965 6172 5f72 6567 6578 7d5b 5f2d  }{year_regex}[_-
+00001a20: 5d28 5b30 2d31 5d5b 302d 395d 295b 5f2d  ]([0-1][0-9])[_-
+00001a30: 5d28 5b30 2d33 5d5b 302d 395d 297b 6c6f  ]([0-3][0-9]){lo
+00001a40: 6f6b 6168 6561 647d 222c 2073 7472 696e  okahead}", strin
+00001a50: 6729 0a0a 2020 2020 2320 7465 6d70 6c61  g)..    # templa
+00001a60: 7465 3a20 362e 2d38 2e33 2e31 3934 3820  te: 6.-8.3.1948 
+00001a70: 7c20 362f 322f 3139 3437 202d 2032 342e  | 6/2/1947 - 24.
+00001a80: 3033 2e31 3934 380a 2020 2020 6575 725f  03.1948.    eur_
+00001a90: 6461 7465 5f72 616e 6765 5f72 6567 6578  date_range_regex
+00001aa0: 203d 2028 0a20 2020 2020 2020 2072 6622   = (.        rf"
+00001ab0: 7b6c 6f6f 6b62 6568 696e 647d 220a 2020  {lookbehind}".  
+00001ac0: 2020 2020 2020 7266 227b 6461 795f 7265        rf"{day_re
+00001ad0: 6765 787d 7b73 6570 5f72 6567 6578 7d28  gex}{sep_regex}(
+00001ae0: 3f3a 7b6d 6f6e 7468 5f72 6567 6578 7d7b  ?:{month_regex}{
+00001af0: 7365 705f 7265 6765 787d 7b79 6561 725f  sep_regex}{year_
+00001b00: 7265 6765 785f 325f 6f72 5f34 5f64 6967  regex_2_or_4_dig
+00001b10: 6974 737d 3f29 3f20 3f28 3f3a 2d7c 3a7c  its}?)? ?(?:-|:|
+00001b20: 746f 2920 3f22 0a20 2020 2020 2020 2072  to) ?".        r
+00001b30: 6622 7b64 6179 5f72 6567 6578 7d7b 7365  f"{day_regex}{se
+00001b40: 705f 7265 6765 787d 7b6d 6f6e 7468 5f72  p_regex}{month_r
+00001b50: 6567 6578 7d7b 7365 705f 7265 6765 787d  egex}{sep_regex}
+00001b60: 7b79 6561 725f 7265 6765 785f 325f 6f72  {year_regex_2_or
+00001b70: 5f34 5f64 6967 6974 737d 220a 2020 2020  _4_digits}".    
+00001b80: 2020 2020 7266 227b 6c6f 6f6b 6168 6561      rf"{lookahea
+00001b90: 647d 220a 2020 2020 290a 2020 2020 6575  d}".    ).    eu
+00001ba0: 725f 6461 7465 5f72 616e 6765 203d 2072  r_date_range = r
+00001bb0: 6567 6578 2e73 6561 7263 6828 6575 725f  egex.search(eur_
+00001bc0: 6461 7465 5f72 616e 6765 5f72 6567 6578  date_range_regex
+00001bd0: 2c20 7374 7269 6e67 290a 0a20 2020 2023  , string)..    #
+00001be0: 2074 656d 706c 6174 653a 2031 2e34 2e32   template: 1.4.2
+00001bf0: 3032 3120 7c20 352f 3131 2f32 3032 310a  021 | 5/11/2021.
+00001c00: 2020 2020 6575 725f 6461 7465 5f72 6567      eur_date_reg
+00001c10: 6578 203d 2072 6622 7b6c 6f6f 6b62 6568  ex = rf"{lookbeh
+00001c20: 696e 647d 7b64 6179 5f72 6567 6578 7d7b  ind}{day_regex}{
+00001c30: 7365 705f 7265 6765 787d 7b6d 6f6e 7468  sep_regex}{month
+00001c40: 5f72 6567 6578 7d7b 7365 705f 7265 6765  _regex}{sep_rege
+00001c50: 787d 7b79 6561 725f 7265 6765 785f 325f  x}{year_regex_2_
+00001c60: 6f72 5f34 5f64 6967 6974 737d 7b6c 6f6f  or_4_digits}{loo
+00001c70: 6b61 6865 6164 7d22 0a20 2020 2065 7572  kahead}".    eur
+00001c80: 5f64 6174 6520 3d20 7265 6765 782e 7365  _date = regex.se
+00001c90: 6172 6368 280a 2020 2020 2020 2020 6575  arch(.        eu
+00001ca0: 725f 6461 7465 5f72 6567 6578 2c0a 2020  r_date_regex,.  
+00001cb0: 2020 2020 2020 7374 7269 6e67 2c0a 2020        string,.  
+00001cc0: 2020 290a 0a20 2020 2023 2074 656d 706c    )..    # templ
+00001cd0: 6174 653a 204d 6172 6368 2039 2c20 3139  ate: March 9, 19
+00001ce0: 3038 207c 204d 6172 6368 352c 3139 3038  08 | March5,1908
+00001cf0: 207c 204d 6179 2031 312c 2031 3930 360a   | May 11, 1906.
+00001d00: 2020 2020 616c 6c5f 6d6f 6e74 6873 203d      all_months =
+00001d10: 2022 7c22 2e6a 6f69 6e28 5f6d 6f6e 7468   "|".join(_month
+00001d20: 735f 6469 6374 290a 2020 2020 6d6f 6e74  s_dict).    mont
+00001d30: 686e 616d 655f 6461 7465 5f72 6567 6578  hname_date_regex
+00001d40: 203d 2072 6622 7b6c 6f6f 6b62 6568 696e   = rf"{lookbehin
+00001d50: 647d 287b 616c 6c5f 6d6f 6e74 6873 7d29  d}({all_months})
+00001d60: 203f 7b64 6179 5f72 6567 6578 7d2c 203f   ?{day_regex}, ?
+00001d70: 7b79 6561 725f 7265 6765 787d 7b6c 6f6f  {year_regex}{loo
+00001d80: 6b61 6865 6164 7d22 0a20 2020 206d 6f6e  kahead}".    mon
+00001d90: 7468 6e61 6d65 5f64 6174 6520 3d20 7265  thname_date = re
+00001da0: 6765 782e 7365 6172 6368 286d 6f6e 7468  gex.search(month
+00001db0: 6e61 6d65 5f64 6174 655f 7265 6765 782c  name_date_regex,
+00001dc0: 2073 7472 696e 6729 0a0a 2020 2020 2320   string)..    # 
+00001dd0: 7465 6d70 6c61 7465 3a20 3138 3439 2f35  template: 1849/5
+00001de0: 3020 7c20 3138 3439 2d35 3020 7c20 3138  0 | 1849-50 | 18
+00001df0: 3439 2f31 3835 300a 2020 2020 7965 6172  49/1850.    year
+00001e00: 5f72 616e 6765 203d 2072 6567 6578 2e73  _range = regex.s
+00001e10: 6561 7263 6828 6c6f 6f6b 6265 6869 6e64  earch(lookbehind
+00001e20: 202b 2079 6561 725f 7265 6765 7820 2b20   + year_regex + 
+00001e30: 7222 5b2f 2d5d 285c 647b 312c 347d 2922  r"[/-](\d{1,4})"
+00001e40: 202b 206c 6f6f 6b61 6865 6164 2c20 7374   + lookahead, st
+00001e50: 7269 6e67 290a 0a20 2020 2023 2074 656d  ring)..    # tem
+00001e60: 706c 6174 653a 2031 3930 370a 2020 2020  plate: 1907.    
+00001e70: 7965 6172 5f6f 6e6c 7920 3d20 7265 6765  year_only = rege
+00001e80: 782e 7365 6172 6368 2872 6622 7b6c 6f6f  x.search(rf"{loo
+00001e90: 6b62 6568 696e 647d 7b79 6561 725f 7265  kbehind}{year_re
+00001ea0: 6765 787d 7b6c 6f6f 6b61 6865 6164 7d22  gex}{lookahead}"
+00001eb0: 2c20 7374 7269 6e67 290a 0a20 2020 2072  , string)..    r
+00001ec0: 6573 3a20 7374 7220 7c20 4e6f 6e65 203d  es: str | None =
+00001ed0: 204e 6f6e 650a 2020 2020 6966 2069 736f   None.    if iso
+00001ee0: 5f64 6174 653a 0a20 2020 2020 2020 2072  _date:.        r
+00001ef0: 6573 203d 205f 6672 6f6d 5f69 736f 5f64  es = _from_iso_d
+00001f00: 6174 6528 6973 6f5f 6461 7465 290a 2020  ate(iso_date).  
+00001f10: 2020 656c 6966 2065 7572 5f64 6174 655f    elif eur_date_
+00001f20: 7261 6e67 653a 0a20 2020 2020 2020 2072  range:.        r
+00001f30: 6573 203d 205f 6672 6f6d 5f65 7572 5f64  es = _from_eur_d
+00001f40: 6174 655f 7261 6e67 6528 6575 725f 6461  ate_range(eur_da
+00001f50: 7465 5f72 616e 6765 290a 2020 2020 656c  te_range).    el
+00001f60: 6966 2065 7572 5f64 6174 653a 0a20 2020  if eur_date:.   
+00001f70: 2020 2020 2072 6573 203d 205f 6672 6f6d       res = _from
+00001f80: 5f65 7572 5f64 6174 6528 6575 725f 6461  _eur_date(eur_da
+00001f90: 7465 290a 2020 2020 656c 6966 206d 6f6e  te).    elif mon
+00001fa0: 7468 6e61 6d65 5f64 6174 653a 0a20 2020  thname_date:.   
+00001fb0: 2020 2020 2072 6573 203d 205f 6672 6f6d       res = _from
+00001fc0: 5f6d 6f6e 7468 6e61 6d65 5f64 6174 6528  _monthname_date(
+00001fd0: 6d6f 6e74 686e 616d 655f 6461 7465 290a  monthname_date).
+00001fe0: 2020 2020 656c 6966 2079 6561 725f 7261      elif year_ra
+00001ff0: 6e67 653a 0a20 2020 2020 2020 2072 6573  nge:.        res
+00002000: 203d 205f 6672 6f6d 5f79 6561 725f 7261   = _from_year_ra
+00002010: 6e67 6528 7965 6172 5f72 616e 6765 290a  nge(year_range).
+00002020: 2020 2020 656c 6966 2079 6561 725f 6f6e      elif year_on
+00002030: 6c79 3a0a 2020 2020 2020 2020 7965 6172  ly:.        year
+00002040: 203d 2069 6e74 2879 6561 725f 6f6e 6c79   = int(year_only
+00002050: 2e67 726f 7570 2830 2929 0a20 2020 2020  .group(0)).     
+00002060: 2020 2072 6573 203d 2066 2247 5245 474f     res = f"GREGO
+00002070: 5249 414e 3a43 453a 7b79 6561 727d 3a43  RIAN:CE:{year}:C
+00002080: 453a 7b79 6561 727d 220a 2020 2020 7265  E:{year}".    re
+00002090: 7475 726e 2072 6573 0a0a 0a64 6566 205f  turn res...def _
+000020a0: 6672 6f6d 5f69 736f 5f64 6174 6528 6973  from_iso_date(is
+000020b0: 6f5f 6461 7465 3a20 4d61 7463 685b 7374  o_date: Match[st
+000020c0: 725d 2920 2d3e 2073 7472 3a0a 2020 2020  r]) -> str:.    
+000020d0: 7965 6172 203d 2069 6e74 2869 736f 5f64  year = int(iso_d
+000020e0: 6174 652e 6772 6f75 7028 3129 290a 2020  ate.group(1)).  
+000020f0: 2020 6d6f 6e74 6820 3d20 696e 7428 6973    month = int(is
+00002100: 6f5f 6461 7465 2e67 726f 7570 2832 2929  o_date.group(2))
+00002110: 0a20 2020 2064 6179 203d 2069 6e74 2869  .    day = int(i
+00002120: 736f 5f64 6174 652e 6772 6f75 7028 3329  so_date.group(3)
+00002130: 290a 2020 2020 6461 7465 203d 2064 6174  ).    date = dat
+00002140: 6574 696d 652e 6461 7465 2879 6561 722c  etime.date(year,
+00002150: 206d 6f6e 7468 2c20 6461 7929 0a20 2020   month, day).   
+00002160: 2072 6574 7572 6e20 6622 4752 4547 4f52   return f"GREGOR
+00002170: 4941 4e3a 4345 3a7b 6461 7465 2e69 736f  IAN:CE:{date.iso
+00002180: 666f 726d 6174 2829 7d3a 4345 3a7b 6461  format()}:CE:{da
+00002190: 7465 2e69 736f 666f 726d 6174 2829 7d22  te.isoformat()}"
+000021a0: 0a0a 0a64 6566 205f 6578 7061 6e64 5f32  ...def _expand_2
+000021b0: 5f64 6967 6974 5f79 6561 7228 7965 6172  _digit_year(year
+000021c0: 3a20 696e 7429 202d 3e20 696e 743a 0a20  : int) -> int:. 
+000021d0: 2020 2063 7572 7265 6e74 5f79 6561 7220     current_year 
+000021e0: 3d20 6461 7465 7469 6d65 2e64 6174 652e  = datetime.date.
+000021f0: 746f 6461 7928 292e 7965 6172 202d 2032  today().year - 2
+00002200: 3030 300a 2020 2020 6966 2079 6561 7220  000.    if year 
+00002210: 3c3d 2063 7572 7265 6e74 5f79 6561 723a  <= current_year:
+00002220: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00002230: 7965 6172 202b 2032 3030 300a 2020 2020  year + 2000.    
+00002240: 656c 6966 2079 6561 7220 3c3d 2039 393a  elif year <= 99:
+00002250: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00002260: 7965 6172 202b 2031 3930 300a 2020 2020  year + 1900.    
+00002270: 656c 7365 3a0a 2020 2020 2020 2020 7265  else:.        re
+00002280: 7475 726e 2079 6561 720a 0a0a 6465 6620  turn year...def 
+00002290: 5f66 726f 6d5f 6575 725f 6461 7465 5f72  _from_eur_date_r
+000022a0: 616e 6765 2865 7572 5f64 6174 655f 7261  ange(eur_date_ra
+000022b0: 6e67 653a 204d 6174 6368 5b73 7472 5d29  nge: Match[str])
+000022c0: 202d 3e20 7374 723a 0a20 2020 2073 7461   -> str:.    sta
+000022d0: 7274 6461 7920 3d20 696e 7428 6575 725f  rtday = int(eur_
+000022e0: 6461 7465 5f72 616e 6765 2e67 726f 7570  date_range.group
+000022f0: 2831 2929 0a20 2020 2073 7461 7274 6d6f  (1)).    startmo
+00002300: 6e74 6820 3d20 696e 7428 6575 725f 6461  nth = int(eur_da
+00002310: 7465 5f72 616e 6765 2e67 726f 7570 2832  te_range.group(2
+00002320: 2929 2069 6620 6575 725f 6461 7465 5f72  )) if eur_date_r
+00002330: 616e 6765 2e67 726f 7570 2832 2920 656c  ange.group(2) el
+00002340: 7365 2069 6e74 2865 7572 5f64 6174 655f  se int(eur_date_
+00002350: 7261 6e67 652e 6772 6f75 7028 3529 290a  range.group(5)).
+00002360: 2020 2020 7374 6172 7479 6561 7220 3d20      startyear = 
+00002370: 696e 7428 6575 725f 6461 7465 5f72 616e  int(eur_date_ran
+00002380: 6765 2e67 726f 7570 2833 2929 2069 6620  ge.group(3)) if 
+00002390: 6575 725f 6461 7465 5f72 616e 6765 2e67  eur_date_range.g
+000023a0: 726f 7570 2833 2920 656c 7365 2069 6e74  roup(3) else int
+000023b0: 2865 7572 5f64 6174 655f 7261 6e67 652e  (eur_date_range.
+000023c0: 6772 6f75 7028 3629 290a 2020 2020 7374  group(6)).    st
+000023d0: 6172 7479 6561 7220 3d20 5f65 7870 616e  artyear = _expan
+000023e0: 645f 325f 6469 6769 745f 7965 6172 2873  d_2_digit_year(s
+000023f0: 7461 7274 7965 6172 290a 2020 2020 656e  tartyear).    en
+00002400: 6464 6179 203d 2069 6e74 2865 7572 5f64  dday = int(eur_d
+00002410: 6174 655f 7261 6e67 652e 6772 6f75 7028  ate_range.group(
+00002420: 3429 290a 2020 2020 656e 646d 6f6e 7468  4)).    endmonth
+00002430: 203d 2069 6e74 2865 7572 5f64 6174 655f   = int(eur_date_
+00002440: 7261 6e67 652e 6772 6f75 7028 3529 290a  range.group(5)).
+00002450: 2020 2020 656e 6479 6561 7220 3d20 696e      endyear = in
+00002460: 7428 6575 725f 6461 7465 5f72 616e 6765  t(eur_date_range
+00002470: 2e67 726f 7570 2836 2929 0a20 2020 2065  .group(6)).    e
+00002480: 6e64 7965 6172 203d 205f 6578 7061 6e64  ndyear = _expand
+00002490: 5f32 5f64 6967 6974 5f79 6561 7228 656e  _2_digit_year(en
+000024a0: 6479 6561 7229 0a20 2020 2073 7461 7274  dyear).    start
+000024b0: 6461 7465 203d 2064 6174 6574 696d 652e  date = datetime.
+000024c0: 6461 7465 2873 7461 7274 7965 6172 2c20  date(startyear, 
+000024d0: 7374 6172 746d 6f6e 7468 2c20 7374 6172  startmonth, star
+000024e0: 7464 6179 290a 2020 2020 656e 6464 6174  tday).    enddat
+000024f0: 6520 3d20 6461 7465 7469 6d65 2e64 6174  e = datetime.dat
+00002500: 6528 656e 6479 6561 722c 2065 6e64 6d6f  e(endyear, endmo
+00002510: 6e74 682c 2065 6e64 6461 7929 0a20 2020  nth, endday).   
+00002520: 2069 6620 656e 6464 6174 6520 3c20 7374   if enddate < st
+00002530: 6172 7464 6174 653a 0a20 2020 2020 2020  artdate:.       
+00002540: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00002550: 720a 2020 2020 7265 7475 726e 2066 2247  r.    return f"G
+00002560: 5245 474f 5249 414e 3a43 453a 7b73 7461  REGORIAN:CE:{sta
+00002570: 7274 6461 7465 2e69 736f 666f 726d 6174  rtdate.isoformat
+00002580: 2829 7d3a 4345 3a7b 656e 6464 6174 652e  ()}:CE:{enddate.
+00002590: 6973 6f66 6f72 6d61 7428 297d 220a 0a0a  isoformat()}"...
+000025a0: 6465 6620 5f66 726f 6d5f 6575 725f 6461  def _from_eur_da
+000025b0: 7465 2865 7572 5f64 6174 653a 204d 6174  te(eur_date: Mat
+000025c0: 6368 5b73 7472 5d29 202d 3e20 7374 723a  ch[str]) -> str:
+000025d0: 0a20 2020 2073 7461 7274 6461 7920 3d20  .    startday = 
+000025e0: 696e 7428 6575 725f 6461 7465 2e67 726f  int(eur_date.gro
+000025f0: 7570 2831 2929 0a20 2020 2073 7461 7274  up(1)).    start
+00002600: 6d6f 6e74 6820 3d20 696e 7428 6575 725f  month = int(eur_
+00002610: 6461 7465 2e67 726f 7570 2832 2929 0a20  date.group(2)). 
+00002620: 2020 2073 7461 7274 7965 6172 203d 2069     startyear = i
+00002630: 6e74 2865 7572 5f64 6174 652e 6772 6f75  nt(eur_date.grou
+00002640: 7028 3329 290a 2020 2020 7374 6172 7479  p(3)).    starty
+00002650: 6561 7220 3d20 5f65 7870 616e 645f 325f  ear = _expand_2_
+00002660: 6469 6769 745f 7965 6172 2873 7461 7274  digit_year(start
+00002670: 7965 6172 290a 2020 2020 6461 7465 203d  year).    date =
+00002680: 2064 6174 6574 696d 652e 6461 7465 2873   datetime.date(s
+00002690: 7461 7274 7965 6172 2c20 7374 6172 746d  tartyear, startm
+000026a0: 6f6e 7468 2c20 7374 6172 7464 6179 290a  onth, startday).
+000026b0: 2020 2020 7265 7475 726e 2066 2247 5245      return f"GRE
+000026c0: 474f 5249 414e 3a43 453a 7b64 6174 652e  GORIAN:CE:{date.
+000026d0: 6973 6f66 6f72 6d61 7428 297d 3a43 453a  isoformat()}:CE:
+000026e0: 7b64 6174 652e 6973 6f66 6f72 6d61 7428  {date.isoformat(
+000026f0: 297d 220a 0a0a 6465 6620 5f66 726f 6d5f  )}"...def _from_
+00002700: 6d6f 6e74 686e 616d 655f 6461 7465 286d  monthname_date(m
+00002710: 6f6e 7468 6e61 6d65 5f64 6174 653a 204d  onthname_date: M
+00002720: 6174 6368 5b73 7472 5d29 202d 3e20 7374  atch[str]) -> st
+00002730: 723a 0a20 2020 2064 6179 203d 2069 6e74  r:.    day = int
+00002740: 286d 6f6e 7468 6e61 6d65 5f64 6174 652e  (monthname_date.
+00002750: 6772 6f75 7028 3229 290a 2020 2020 6d6f  group(2)).    mo
+00002760: 6e74 6820 3d20 5f6d 6f6e 7468 735f 6469  nth = _months_di
+00002770: 6374 5b6d 6f6e 7468 6e61 6d65 5f64 6174  ct[monthname_dat
+00002780: 652e 6772 6f75 7028 3129 5d0a 2020 2020  e.group(1)].    
+00002790: 7965 6172 203d 2069 6e74 286d 6f6e 7468  year = int(month
+000027a0: 6e61 6d65 5f64 6174 652e 6772 6f75 7028  name_date.group(
+000027b0: 3329 290a 2020 2020 6461 7465 203d 2064  3)).    date = d
+000027c0: 6174 6574 696d 652e 6461 7465 2879 6561  atetime.date(yea
+000027d0: 722c 206d 6f6e 7468 2c20 6461 7929 0a20  r, month, day). 
+000027e0: 2020 2072 6574 7572 6e20 6622 4752 4547     return f"GREG
+000027f0: 4f52 4941 4e3a 4345 3a7b 6461 7465 2e69  ORIAN:CE:{date.i
+00002800: 736f 666f 726d 6174 2829 7d3a 4345 3a7b  soformat()}:CE:{
+00002810: 6461 7465 2e69 736f 666f 726d 6174 2829  date.isoformat()
+00002820: 7d22 0a0a 0a64 6566 205f 6672 6f6d 5f79  }"...def _from_y
+00002830: 6561 725f 7261 6e67 6528 7965 6172 5f72  ear_range(year_r
+00002840: 616e 6765 3a20 4d61 7463 685b 7374 725d  ange: Match[str]
+00002850: 2920 2d3e 2073 7472 3a0a 2020 2020 7374  ) -> str:.    st
+00002860: 6172 7479 6561 7220 3d20 696e 7428 7965  artyear = int(ye
+00002870: 6172 5f72 616e 6765 2e67 726f 7570 2831  ar_range.group(1
+00002880: 2929 0a20 2020 2065 6e64 7965 6172 203d  )).    endyear =
+00002890: 2069 6e74 2879 6561 725f 7261 6e67 652e   int(year_range.
+000028a0: 6772 6f75 7028 3229 290a 2020 2020 6966  group(2)).    if
+000028b0: 2065 6e64 7965 6172 202f 2f20 3130 203d   endyear // 10 =
+000028c0: 3d20 303a 0a20 2020 2020 2020 2023 2065  = 0:.        # e
+000028d0: 6e64 7965 6172 2069 7320 6f6e 6c79 2031  ndyear is only 1
+000028e0: 2d64 6967 6974 3a20 6164 6420 7468 6520  -digit: add the 
+000028f0: 6669 7273 7420 322d 3320 6469 6769 7473  first 2-3 digits
+00002900: 206f 6620 7374 6172 7479 6561 720a 2020   of startyear.  
+00002910: 2020 2020 2020 656e 6479 6561 7220 3d20        endyear = 
+00002920: 7374 6172 7479 6561 7220 2f2f 2031 3020  startyear // 10 
+00002930: 2a20 3130 202b 2065 6e64 7965 6172 0a20  * 10 + endyear. 
+00002940: 2020 2065 6c69 6620 656e 6479 6561 7220     elif endyear 
+00002950: 2f2f 2031 3030 203d 3d20 303a 0a20 2020  // 100 == 0:.   
+00002960: 2020 2020 2023 2065 6e64 7965 6172 2069       # endyear i
+00002970: 7320 6f6e 6c79 2032 2d64 6967 6974 3a20  s only 2-digit: 
+00002980: 6164 6420 7468 6520 6669 7273 7420 312d  add the first 1-
+00002990: 3220 6469 6769 7473 206f 6620 7374 6172  2 digits of star
+000029a0: 7479 6561 720a 2020 2020 2020 2020 656e  tyear.        en
+000029b0: 6479 6561 7220 3d20 7374 6172 7479 6561  dyear = startyea
+000029c0: 7220 2f2f 2031 3030 202a 2031 3030 202b  r // 100 * 100 +
+000029d0: 2065 6e64 7965 6172 0a20 2020 2069 6620   endyear.    if 
+000029e0: 656e 6479 6561 7220 3c3d 2073 7461 7274  endyear <= start
+000029f0: 7965 6172 3a0a 2020 2020 2020 2020 7261  year:.        ra
+00002a00: 6973 6520 5661 6c75 6545 7272 6f72 0a20  ise ValueError. 
+00002a10: 2020 2072 6574 7572 6e20 6622 4752 4547     return f"GREG
+00002a20: 4f52 4941 4e3a 4345 3a7b 7374 6172 7479  ORIAN:CE:{starty
+00002a30: 6561 727d 3a43 453a 7b65 6e64 7965 6172  ear}:CE:{endyear
+00002a40: 7d22 0a0a 0a64 6566 2070 7265 7061 7265  }"...def prepare
+00002a50: 5f76 616c 7565 280a 2020 2020 7661 6c75  _value(.    valu
+00002a60: 653a 2055 6e69 6f6e 5b50 726f 7065 7274  e: Union[Propert
+00002a70: 7945 6c65 6d65 6e74 2c20 7374 722c 2069  yElement, str, i
+00002a80: 6e74 2c20 666c 6f61 742c 2062 6f6f 6c2c  nt, float, bool,
+00002a90: 2049 7465 7261 626c 655b 556e 696f 6e5b   Iterable[Union[
+00002aa0: 5072 6f70 6572 7479 456c 656d 656e 742c  PropertyElement,
+00002ab0: 2073 7472 2c20 696e 742c 2066 6c6f 6174   str, int, float
+00002ac0: 2c20 626f 6f6c 5d5d 5d2c 0a29 202d 3e20  , bool]]],.) -> 
+00002ad0: 6c69 7374 5b50 726f 7065 7274 7945 6c65  list[PropertyEle
+00002ae0: 6d65 6e74 5d3a 0a20 2020 2022 2222 0a20  ment]:.    """. 
+00002af0: 2020 2054 6869 7320 6d65 7468 6f64 2074     This method t
+00002b00: 7261 6e73 666f 726d 7320 7468 6520 7061  ransforms the pa
+00002b10: 7261 6d65 7465 7220 2276 616c 7565 2220  rameter "value" 
+00002b20: 6672 6f6d 2061 206d 616b 655f 2a5f 7072  from a make_*_pr
+00002b30: 6f70 2829 206d 6574 686f 6420 696e 746f  op() method into
+00002b40: 2061 206c 6973 7420 6f66 2050 726f 7065   a list of Prope
+00002b50: 7274 7945 6c65 6d65 6e74 732e 2022 7661  rtyElements. "va
+00002b60: 6c75 6522 2069 730a 2020 2020 7061 7373  lue" is.    pass
+00002b70: 6564 206f 6e20 746f 2074 6869 7320 6d65  ed on to this me
+00002b80: 7468 6f64 2061 7320 6974 2077 6173 2072  thod as it was r
+00002b90: 6563 6569 7665 642e 0a0a 2020 2020 4172  eceived...    Ar
+00002ba0: 6773 3a0a 2020 2020 2020 2020 7661 6c75  gs:.        valu
+00002bb0: 653a 2022 7661 6c75 6522 2061 7320 7265  e: "value" as re
+00002bc0: 6365 6976 6564 2066 726f 6d20 7468 6520  ceived from the 
+00002bd0: 6361 6c6c 6572 0a0a 2020 2020 5265 7475  caller..    Retu
+00002be0: 726e 733a 0a20 2020 2020 2020 2061 206c  rns:.        a l
+00002bf0: 6973 7420 6f66 2050 726f 7065 7274 7945  ist of PropertyE
+00002c00: 6c65 6d65 6e74 730a 2020 2020 2222 220a  lements.    """.
+00002c10: 2020 2020 2320 6d61 6b65 2073 7572 6520      # make sure 
+00002c20: 7468 6174 2022 7661 6c75 6522 2069 7320  that "value" is 
+00002c30: 6c69 7374 2d6c 696b 650a 2020 2020 6966  list-like.    if
+00002c40: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
+00002c50: 7661 6c75 652c 2049 7465 7261 626c 6529  value, Iterable)
+00002c60: 206f 7220 6973 696e 7374 616e 6365 2876   or isinstance(v
+00002c70: 616c 7565 2c20 7374 7229 3a0a 2020 2020  alue, str):.    
+00002c80: 2020 2020 7661 6c75 6520 3d20 5b76 616c      value = [val
+00002c90: 7565 5d0a 0a20 2020 2023 206d 616b 6520  ue]..    # make 
+00002ca0: 6120 5072 6f70 6572 7479 456c 656d 656e  a PropertyElemen
+00002cb0: 7420 6f75 7420 6f66 2069 7473 2065 6c65  t out of its ele
+00002cc0: 6d65 6e74 732c 2069 6620 6e65 6365 7373  ments, if necess
+00002cd0: 6172 792e 0a20 2020 2072 6574 7572 6e20  ary..    return 
+00002ce0: 5b78 2069 6620 6973 696e 7374 616e 6365  [x if isinstance
+00002cf0: 2878 2c20 5072 6f70 6572 7479 456c 656d  (x, PropertyElem
+00002d00: 656e 7429 2065 6c73 6520 5072 6f70 6572  ent) else Proper
+00002d10: 7479 456c 656d 656e 7428 7829 2066 6f72  tyElement(x) for
+00002d20: 2078 2069 6e20 7661 6c75 655d 0a0a 0a64   x in value]...d
+00002d30: 6566 206d 616b 655f 726f 6f74 280a 2020  ef make_root(.  
+00002d40: 2020 7368 6f72 7463 6f64 653a 2073 7472    shortcode: str
+00002d50: 2c0a 2020 2020 6465 6661 756c 745f 6f6e  ,.    default_on
+00002d60: 746f 6c6f 6779 3a20 7374 722c 0a29 202d  tology: str,.) -
+00002d70: 3e20 6574 7265 652e 5f45 6c65 6d65 6e74  > etree._Element
+00002d80: 3a0a 2020 2020 2222 220a 2020 2020 5374  :.    """.    St
+00002d90: 6172 7420 6275 696c 6469 6e67 2079 6f75  art building you
+00002da0: 7220 584d 4c20 646f 6375 6d65 6e74 2062  r XML document b
+00002db0: 7920 6372 6561 7469 6e67 2074 6865 2072  y creating the r
+00002dc0: 6f6f 7420 656c 656d 656e 7420 3c6b 6e6f  oot element <kno
+00002dd0: 7261 3e2e 0a0a 2020 2020 4172 6773 3a0a  ra>...    Args:.
+00002de0: 2020 2020 2020 2020 7368 6f72 7463 6f64          shortcod
+00002df0: 653a 2054 6865 2073 686f 7274 636f 6465  e: The shortcode
+00002e00: 206f 6620 7468 6973 2070 726f 6a65 6374   of this project
+00002e10: 2061 7320 6465 6669 6e65 6420 696e 2074   as defined in t
+00002e20: 6865 204a 534f 4e20 7072 6f6a 6563 7420  he JSON project 
+00002e30: 6669 6c65 0a20 2020 2020 2020 2064 6566  file.        def
+00002e40: 6175 6c74 5f6f 6e74 6f6c 6f67 793a 206f  ault_ontology: o
+00002e50: 6e65 206f 6620 7468 6520 6f6e 746f 6c6f  ne of the ontolo
+00002e60: 6769 6573 206f 6620 7468 6520 4a53 4f4e  gies of the JSON
+00002e70: 2070 726f 6a65 6374 2066 696c 650a 0a20   project file.. 
+00002e80: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00002e90: 2020 2020 5468 6520 726f 6f74 2065 6c65      The root ele
+00002ea0: 6d65 6e74 203c 6b6e 6f72 613e 2e0a 0a20  ment <knora>... 
+00002eb0: 2020 2045 7861 6d70 6c65 733a 0a20 2020     Examples:.   
+00002ec0: 2020 2020 203e 3e3e 2072 6f6f 7420 3d20       >>> root = 
+00002ed0: 6578 6365 6c32 786d 6c2e 6d61 6b65 5f72  excel2xml.make_r
+00002ee0: 6f6f 7428 7368 6f72 7463 6f64 653d 7368  oot(shortcode=sh
+00002ef0: 6f72 7463 6f64 652c 2064 6566 6175 6c74  ortcode, default
+00002f00: 5f6f 6e74 6f6c 6f67 793d 6465 6661 756c  _ontology=defaul
+00002f10: 745f 6f6e 746f 6c6f 6779 290a 2020 2020  t_ontology).    
+00002f20: 2020 2020 3e3e 3e20 726f 6f74 203d 2065      >>> root = e
+00002f30: 7863 656c 3278 6d6c 2e61 7070 656e 645f  xcel2xml.append_
+00002f40: 7065 726d 6973 7369 6f6e 7328 726f 6f74  permissions(root
+00002f50: 290a 0a20 2020 2053 6565 2068 7474 7073  )..    See https
+00002f60: 3a2f 2f64 6f63 732e 6461 7363 682e 7377  ://docs.dasch.sw
+00002f70: 6973 732f 6c61 7465 7374 2f44 5350 2d54  iss/latest/DSP-T
+00002f80: 4f4f 4c53 2f66 696c 652d 666f 726d 6174  OOLS/file-format
+00002f90: 732f 786d 6c2d 6461 7461 2d66 696c 652f  s/xml-data-file/
+00002fa0: 2374 6865 2d72 6f6f 742d 656c 656d 656e  #the-root-elemen
+00002fb0: 742d 6b6e 6f72 610a 2020 2020 2222 220a  t-knora.    """.
+00002fc0: 2020 2020 7363 6865 6d61 5f75 726c 203d      schema_url =
+00002fd0: 2022 6874 7470 733a 2f2f 7261 772e 6769   "https://raw.gi
+00002fe0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00002ff0: 636f 6d2f 6461 7363 682d 7377 6973 732f  com/dasch-swiss/
+00003000: 6473 702d 746f 6f6c 732f 6d61 696e 2f73  dsp-tools/main/s
+00003010: 7263 2f64 7370 5f74 6f6f 6c73 2f72 6573  rc/dsp_tools/res
+00003020: 6f75 7263 6573 2f73 6368 656d 612f 6461  ources/schema/da
+00003030: 7461 2e78 7364 220a 2020 2020 7363 6865  ta.xsd".    sche
+00003040: 6d61 5f6c 6f63 6174 696f 6e5f 6b65 7920  ma_location_key 
+00003050: 3d20 7374 7228 6574 7265 652e 514e 616d  = str(etree.QNam
+00003060: 6528 2268 7474 703a 2f2f 7777 772e 7733  e("http://www.w3
+00003070: 2e6f 7267 2f32 3030 312f 584d 4c53 6368  .org/2001/XMLSch
+00003080: 656d 612d 696e 7374 616e 6365 222c 2022  ema-instance", "
+00003090: 7363 6865 6d61 4c6f 6361 7469 6f6e 2229  schemaLocation")
+000030a0: 290a 2020 2020 7363 6865 6d61 5f6c 6f63  ).    schema_loc
+000030b0: 6174 696f 6e5f 7661 6c75 6520 3d20 6622  ation_value = f"
+000030c0: 6874 7470 733a 2f2f 6461 7363 682e 7377  https://dasch.sw
+000030d0: 6973 732f 7363 6865 6d61 207b 7363 6865  iss/schema {sche
+000030e0: 6d61 5f75 726c 7d22 0a20 2020 2072 6574  ma_url}".    ret
+000030f0: 7572 6e20 6574 7265 652e 456c 656d 656e  urn etree.Elemen
+00003100: 7428 0a20 2020 2020 2020 2022 7b25 737d  t(.        "{%s}
+00003110: 6b6e 6f72 6122 2025 2078 6d6c 5f6e 616d  knora" % xml_nam
+00003120: 6573 7061 6365 5f6d 6170 5b4e 6f6e 655d  espace_map[None]
+00003130: 2c0a 2020 2020 2020 2020 6174 7472 6962  ,.        attrib
+00003140: 3d7b 0a20 2020 2020 2020 2020 2020 2073  ={.            s
+00003150: 6368 656d 615f 6c6f 6361 7469 6f6e 5f6b  chema_location_k
+00003160: 6579 3a20 7363 6865 6d61 5f6c 6f63 6174  ey: schema_locat
+00003170: 696f 6e5f 7661 6c75 652c 0a20 2020 2020  ion_value,.     
+00003180: 2020 2020 2020 2022 7368 6f72 7463 6f64         "shortcod
+00003190: 6522 3a20 7368 6f72 7463 6f64 652c 0a20  e": shortcode,. 
+000031a0: 2020 2020 2020 2020 2020 2022 6465 6661             "defa
+000031b0: 756c 742d 6f6e 746f 6c6f 6779 223a 2064  ult-ontology": d
+000031c0: 6566 6175 6c74 5f6f 6e74 6f6c 6f67 792c  efault_ontology,
+000031d0: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+000031e0: 2020 2020 6e73 6d61 703d 786d 6c5f 6e61      nsmap=xml_na
+000031f0: 6d65 7370 6163 655f 6d61 702c 0a20 2020  mespace_map,.   
+00003200: 2029 0a0a 0a64 6566 2061 7070 656e 645f   )...def append_
+00003210: 7065 726d 6973 7369 6f6e 7328 726f 6f74  permissions(root
+00003220: 5f65 6c65 6d65 6e74 3a20 6574 7265 652e  _element: etree.
+00003230: 5f45 6c65 6d65 6e74 2920 2d3e 2065 7472  _Element) -> etr
+00003240: 6565 2e5f 456c 656d 656e 743a 0a20 2020  ee._Element:.   
+00003250: 2022 2222 0a20 2020 2041 6674 6572 2068   """.    After h
+00003260: 6176 696e 6720 6372 6561 7465 6420 6120  aving created a 
+00003270: 726f 6f74 2065 6c65 6d65 6e74 2c20 6361  root element, ca
+00003280: 6c6c 2074 6869 7320 6d65 7468 6f64 2074  ll this method t
+00003290: 6f20 6170 7065 6e64 2074 6865 2066 6f75  o append the fou
+000032a0: 7220 7065 726d 6973 7369 6f6e 7320 2272  r permissions "r
+000032b0: 6573 2d64 6566 6175 6c74 222c 0a20 2020  es-default",.   
+000032c0: 2022 7265 732d 7265 7374 7269 6374 6564   "res-restricted
+000032d0: 222c 2022 7072 6f70 2d64 6566 6175 6c74  ", "prop-default
+000032e0: 222c 2061 6e64 2022 7072 6f70 2d72 6573  ", and "prop-res
+000032f0: 7472 6963 7465 6422 2074 6f20 6974 2e20  tricted" to it. 
+00003300: 5468 6573 6520 666f 7572 2070 6572 6d69  These four permi
+00003310: 7373 696f 6e73 2061 7265 2061 2067 6f6f  ssions are a goo
+00003320: 6420 6261 7369 7320 746f 0a20 2020 2073  d basis to.    s
+00003330: 7461 7274 2077 6974 682c 2062 7574 2072  tart with, but r
+00003340: 656d 656d 6265 7220 7468 6174 2074 6865  emember that the
+00003350: 7920 6361 6e20 6265 2061 6461 7074 6564  y can be adapted
+00003360: 2c20 616e 6420 7468 6174 206f 7468 6572  , and that other
+00003370: 2070 6572 6d69 7373 696f 6e73 2063 616e   permissions can
+00003380: 2062 6520 6465 6669 6e65 6420 696e 7374   be defined inst
+00003390: 6561 6420 6f66 2074 6865 7365 2e0a 0a20  ead of these... 
+000033a0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+000033b0: 2072 6f6f 745f 656c 656d 656e 743a 2054   root_element: T
+000033c0: 6865 2058 4d4c 2072 6f6f 7420 656c 656d  he XML root elem
+000033d0: 656e 7420 3c6b 6e6f 7261 3e20 6372 6561  ent <knora> crea
+000033e0: 7465 6420 6279 206d 616b 655f 726f 6f74  ted by make_root
+000033f0: 2829 0a0a 2020 2020 5265 7475 726e 733a  ()..    Returns:
+00003400: 0a20 2020 2020 2020 2054 6865 2072 6f6f  .        The roo
+00003410: 7420 656c 656d 656e 7420 7769 7468 2074  t element with t
+00003420: 6865 2066 6f75 7220 7065 726d 6973 7369  he four permissi
+00003430: 6f6e 2062 6c6f 636b 7320 6170 7065 6e64  on blocks append
+00003440: 6564 0a0a 2020 2020 4578 616d 706c 6573  ed..    Examples
+00003450: 3a0a 2020 2020 2020 2020 3e3e 3e20 726f  :.        >>> ro
+00003460: 6f74 203d 2065 7863 656c 3278 6d6c 2e6d  ot = excel2xml.m
+00003470: 616b 655f 726f 6f74 2873 686f 7274 636f  ake_root(shortco
+00003480: 6465 3d73 686f 7274 636f 6465 2c20 6465  de=shortcode, de
+00003490: 6661 756c 745f 6f6e 746f 6c6f 6779 3d64  fault_ontology=d
+000034a0: 6566 6175 6c74 5f6f 6e74 6f6c 6f67 7929  efault_ontology)
+000034b0: 0a20 2020 2020 2020 203e 3e3e 2072 6f6f  .        >>> roo
+000034c0: 7420 3d20 6578 6365 6c32 786d 6c2e 6170  t = excel2xml.ap
+000034d0: 7065 6e64 5f70 6572 6d69 7373 696f 6e73  pend_permissions
+000034e0: 2872 6f6f 7429 0a0a 2020 2020 5365 6520  (root)..    See 
+000034f0: 6874 7470 733a 2f2f 646f 6373 2e64 6173  https://docs.das
+00003500: 6368 2e73 7769 7373 2f6c 6174 6573 742f  ch.swiss/latest/
+00003510: 4453 502d 544f 4f4c 532f 6669 6c65 2d66  DSP-TOOLS/file-f
+00003520: 6f72 6d61 7473 2f78 6d6c 2d64 6174 612d  ormats/xml-data-
+00003530: 6669 6c65 2f23 6465 7363 7269 6269 6e67  file/#describing
+00003540: 2d70 6572 6d69 7373 696f 6e73 2d77 6974  -permissions-wit
+00003550: 682d 7065 726d 6973 7369 6f6e 732d 656c  h-permissions-el
+00003560: 656d 656e 7473 0a20 2020 2022 2222 0a0a  ements.    """..
+00003570: 2020 2020 5045 524d 4953 5349 4f4e 5320      PERMISSIONS 
+00003580: 3d20 452e 7065 726d 6973 7369 6f6e 730a  = E.permissions.
+00003590: 2020 2020 414c 4c4f 5720 3d20 452e 616c      ALLOW = E.al
+000035a0: 6c6f 770a 2020 2020 2320 6c78 6d6c 2e62  low.    # lxml.b
+000035b0: 7569 6c64 6572 2e45 2069 7320 6120 6d6f  uilder.E is a mo
+000035c0: 7265 2073 6f70 6869 7374 6963 6174 6564  re sophisticated
+000035d0: 2065 6c65 6d65 6e74 2066 6163 746f 7279   element factory
+000035e0: 2074 6861 6e20 6574 7265 652e 456c 656d   than etree.Elem
+000035f0: 656e 742e 0a20 2020 2023 2045 2e74 6167  ent..    # E.tag
+00003600: 2069 7320 6571 7569 7661 6c65 6e74 2074   is equivalent t
+00003610: 6f20 4528 2274 6167 2229 2061 6e64 2072  o E("tag") and r
+00003620: 6573 756c 7473 2069 6e20 3c74 6167 3e0a  esults in <tag>.
+00003630: 0a20 2020 2072 6573 5f64 6566 6175 6c74  .    res_default
+00003640: 203d 2065 7472 6565 2e45 6c65 6d65 6e74   = etree.Element
+00003650: 2822 7b25 737d 7065 726d 6973 7369 6f6e  ("{%s}permission
+00003660: 7322 2025 2078 6d6c 5f6e 616d 6573 7061  s" % xml_namespa
+00003670: 6365 5f6d 6170 5b4e 6f6e 655d 2c20 6964  ce_map[None], id
+00003680: 3d22 7265 732d 6465 6661 756c 7422 290a  ="res-default").
+00003690: 2020 2020 7265 735f 6465 6661 756c 742e      res_default.
+000036a0: 6170 7065 6e64 2841 4c4c 4f57 2822 5622  append(ALLOW("V"
+000036b0: 2c20 6772 6f75 703d 2255 6e6b 6e6f 776e  , group="Unknown
+000036c0: 5573 6572 2229 290a 2020 2020 7265 735f  User")).    res_
+000036d0: 6465 6661 756c 742e 6170 7065 6e64 2841  default.append(A
+000036e0: 4c4c 4f57 2822 5622 2c20 6772 6f75 703d  LLOW("V", group=
+000036f0: 224b 6e6f 776e 5573 6572 2229 290a 2020  "KnownUser")).  
+00003700: 2020 7265 735f 6465 6661 756c 742e 6170    res_default.ap
+00003710: 7065 6e64 2841 4c4c 4f57 2822 4422 2c20  pend(ALLOW("D", 
+00003720: 6772 6f75 703d 2250 726f 6a65 6374 4d65  group="ProjectMe
+00003730: 6d62 6572 2229 290a 2020 2020 7265 735f  mber")).    res_
+00003740: 6465 6661 756c 742e 6170 7065 6e64 2841  default.append(A
+00003750: 4c4c 4f57 2822 4352 222c 2067 726f 7570  LLOW("CR", group
+00003760: 3d22 5072 6f6a 6563 7441 646d 696e 2229  ="ProjectAdmin")
+00003770: 290a 2020 2020 7265 735f 6465 6661 756c  ).    res_defaul
+00003780: 742e 6170 7065 6e64 2841 4c4c 4f57 2822  t.append(ALLOW("
+00003790: 4352 222c 2067 726f 7570 3d22 4372 6561  CR", group="Crea
+000037a0: 746f 7222 2929 0a20 2020 2072 6f6f 745f  tor")).    root_
+000037b0: 656c 656d 656e 742e 6170 7065 6e64 2872  element.append(r
+000037c0: 6573 5f64 6566 6175 6c74 290a 0a20 2020  es_default)..   
+000037d0: 2072 6573 5f72 6573 7472 6963 7465 6420   res_restricted 
+000037e0: 3d20 5045 524d 4953 5349 4f4e 5328 6964  = PERMISSIONS(id
+000037f0: 3d22 7265 732d 7265 7374 7269 6374 6564  ="res-restricted
+00003800: 2229 0a20 2020 2072 6573 5f72 6573 7472  ").    res_restr
+00003810: 6963 7465 642e 6170 7065 6e64 2841 4c4c  icted.append(ALL
+00003820: 4f57 2822 4d22 2c20 6772 6f75 703d 2250  OW("M", group="P
+00003830: 726f 6a65 6374 4d65 6d62 6572 2229 290a  rojectMember")).
+00003840: 2020 2020 7265 735f 7265 7374 7269 6374      res_restrict
+00003850: 6564 2e61 7070 656e 6428 414c 4c4f 5728  ed.append(ALLOW(
+00003860: 2243 5222 2c20 6772 6f75 703d 2250 726f  "CR", group="Pro
+00003870: 6a65 6374 4164 6d69 6e22 2929 0a20 2020  jectAdmin")).   
+00003880: 2072 6573 5f72 6573 7472 6963 7465 642e   res_restricted.
+00003890: 6170 7065 6e64 2841 4c4c 4f57 2822 4352  append(ALLOW("CR
+000038a0: 222c 2067 726f 7570 3d22 4372 6561 746f  ", group="Creato
+000038b0: 7222 2929 0a20 2020 2072 6f6f 745f 656c  r")).    root_el
+000038c0: 656d 656e 742e 6170 7065 6e64 2872 6573  ement.append(res
+000038d0: 5f72 6573 7472 6963 7465 6429 0a0a 2020  _restricted)..  
+000038e0: 2020 7072 6f70 5f64 6566 6175 6c74 203d    prop_default =
+000038f0: 2050 4552 4d49 5353 494f 4e53 2869 643d   PERMISSIONS(id=
+00003900: 2270 726f 702d 6465 6661 756c 7422 290a  "prop-default").
+00003910: 2020 2020 7072 6f70 5f64 6566 6175 6c74      prop_default
+00003920: 2e61 7070 656e 6428 414c 4c4f 5728 2256  .append(ALLOW("V
+00003930: 222c 2067 726f 7570 3d22 556e 6b6e 6f77  ", group="Unknow
+00003940: 6e55 7365 7222 2929 0a20 2020 2070 726f  nUser")).    pro
+00003950: 705f 6465 6661 756c 742e 6170 7065 6e64  p_default.append
+00003960: 2841 4c4c 4f57 2822 5622 2c20 6772 6f75  (ALLOW("V", grou
+00003970: 703d 224b 6e6f 776e 5573 6572 2229 290a  p="KnownUser")).
+00003980: 2020 2020 7072 6f70 5f64 6566 6175 6c74      prop_default
+00003990: 2e61 7070 656e 6428 414c 4c4f 5728 2244  .append(ALLOW("D
+000039a0: 222c 2067 726f 7570 3d22 5072 6f6a 6563  ", group="Projec
+000039b0: 744d 656d 6265 7222 2929 0a20 2020 2070  tMember")).    p
+000039c0: 726f 705f 6465 6661 756c 742e 6170 7065  rop_default.appe
+000039d0: 6e64 2841 4c4c 4f57 2822 4352 222c 2067  nd(ALLOW("CR", g
+000039e0: 726f 7570 3d22 5072 6f6a 6563 7441 646d  roup="ProjectAdm
+000039f0: 696e 2229 290a 2020 2020 7072 6f70 5f64  in")).    prop_d
+00003a00: 6566 6175 6c74 2e61 7070 656e 6428 414c  efault.append(AL
+00003a10: 4c4f 5728 2243 5222 2c20 6772 6f75 703d  LOW("CR", group=
+00003a20: 2243 7265 6174 6f72 2229 290a 2020 2020  "Creator")).    
+00003a30: 726f 6f74 5f65 6c65 6d65 6e74 2e61 7070  root_element.app
+00003a40: 656e 6428 7072 6f70 5f64 6566 6175 6c74  end(prop_default
+00003a50: 290a 0a20 2020 2070 726f 705f 7265 7374  )..    prop_rest
+00003a60: 7269 6374 6564 203d 2050 4552 4d49 5353  ricted = PERMISS
+00003a70: 494f 4e53 2869 643d 2270 726f 702d 7265  IONS(id="prop-re
+00003a80: 7374 7269 6374 6564 2229 0a20 2020 2070  stricted").    p
+00003a90: 726f 705f 7265 7374 7269 6374 6564 2e61  rop_restricted.a
+00003aa0: 7070 656e 6428 414c 4c4f 5728 224d 222c  ppend(ALLOW("M",
+00003ab0: 2067 726f 7570 3d22 5072 6f6a 6563 744d   group="ProjectM
+00003ac0: 656d 6265 7222 2929 0a20 2020 2070 726f  ember")).    pro
+00003ad0: 705f 7265 7374 7269 6374 6564 2e61 7070  p_restricted.app
+00003ae0: 656e 6428 414c 4c4f 5728 2243 5222 2c20  end(ALLOW("CR", 
+00003af0: 6772 6f75 703d 2250 726f 6a65 6374 4164  group="ProjectAd
+00003b00: 6d69 6e22 2929 0a20 2020 2070 726f 705f  min")).    prop_
+00003b10: 7265 7374 7269 6374 6564 2e61 7070 656e  restricted.appen
+00003b20: 6428 414c 4c4f 5728 2243 5222 2c20 6772  d(ALLOW("CR", gr
+00003b30: 6f75 703d 2243 7265 6174 6f72 2229 290a  oup="Creator")).
+00003b40: 2020 2020 726f 6f74 5f65 6c65 6d65 6e74      root_element
+00003b50: 2e61 7070 656e 6428 7072 6f70 5f72 6573  .append(prop_res
+00003b60: 7472 6963 7465 6429 0a0a 2020 2020 7265  tricted)..    re
+00003b70: 7475 726e 2072 6f6f 745f 656c 656d 656e  turn root_elemen
+00003b80: 740a 0a0a 6465 6620 6d61 6b65 5f72 6573  t...def make_res
+00003b90: 6f75 7263 6528 2020 2320 6e6f 7161 3a20  ource(  # noqa: 
+00003ba0: 4434 3137 2028 756e 646f 6375 6d65 6e74  D417 (undocument
+00003bb0: 6564 2d70 6172 616d 290a 2020 2020 6c61  ed-param).    la
+00003bc0: 6265 6c3a 2073 7472 2c0a 2020 2020 7265  bel: str,.    re
+00003bd0: 7374 7970 653a 2073 7472 2c0a 2020 2020  stype: str,.    
+00003be0: 6964 3a20 7374 722c 0a20 2020 2070 6572  id: str,.    per
+00003bf0: 6d69 7373 696f 6e73 3a20 7374 7220 3d20  missions: str = 
+00003c00: 2272 6573 2d64 6566 6175 6c74 222c 0a20  "res-default",. 
+00003c10: 2020 2061 726b 3a20 4f70 7469 6f6e 616c     ark: Optional
+00003c20: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+00003c30: 2020 6972 693a 204f 7074 696f 6e61 6c5b    iri: Optional[
+00003c40: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+00003c50: 2063 7265 6174 696f 6e5f 6461 7465 3a20   creation_date: 
+00003c60: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00003c70: 4e6f 6e65 2c0a 2920 2d3e 2065 7472 6565  None,.) -> etree
+00003c80: 2e5f 456c 656d 656e 743a 0a20 2020 2022  ._Element:.    "
+00003c90: 2222 0a20 2020 2043 7265 6174 6573 2061  "".    Creates a
+00003ca0: 6e20 656d 7074 7920 7265 736f 7572 6365  n empty resource
+00003cb0: 2065 6c65 6d65 6e74 2c20 7769 7468 2074   element, with t
+00003cc0: 6865 2061 7474 7269 6275 7465 7320 6173  he attributes as
+00003cd0: 2073 7065 6369 6669 6564 2062 7920 7468   specified by th
+00003ce0: 6520 6172 6775 6d65 6e74 730a 0a20 2020  e arguments..   
+00003cf0: 2041 7267 733a 0a20 2020 2020 2020 2054   Args:.        T
+00003d00: 6865 2061 7267 756d 656e 7473 2063 6f72  he arguments cor
+00003d10: 7265 7370 6f6e 6420 746f 2074 6865 2061  respond to the a
+00003d20: 7474 7269 6275 7465 7320 6f66 2074 6865  ttributes of the
+00003d30: 203c 7265 736f 7572 6365 3e20 656c 656d   <resource> elem
+00003d40: 656e 742e 0a0a 2020 2020 5265 7475 726e  ent...    Return
+00003d50: 733a 0a20 2020 2020 2020 2054 6865 2072  s:.        The r
+00003d60: 6573 6f75 7263 6520 656c 656d 656e 742c  esource element,
+00003d70: 2077 6974 686f 7574 2061 6e79 2063 6869   without any chi
+00003d80: 6c64 7265 6e2c 2062 7574 2077 6974 6820  ldren, but with 
+00003d90: 7468 6520 6174 7472 6962 7574 6573 0a20  the attributes. 
+00003da0: 2020 2020 2020 2060 603c 7265 736f 7572         ``<resour
+00003db0: 6365 206c 6162 656c 3d6c 6162 656c 2072  ce label=label r
+00003dc0: 6573 7479 7065 3d72 6573 7479 7065 2069  estype=restype i
+00003dd0: 643d 6964 2070 6572 6d69 7373 696f 6e73  d=id permissions
+00003de0: 3d70 6572 6d69 7373 696f 6e73 2061 726b  =permissions ark
+00003df0: 3d61 726b 2069 7269 3d69 7269 3e3c 2f72  =ark iri=iri></r
+00003e00: 6573 6f75 7263 653e 6060 0a0a 2020 2020  esource>``..    
+00003e10: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
+00003e20: 5761 726e 696e 673a 2069 6620 626f 7468  Warning: if both
+00003e30: 2061 6e20 4152 4b20 616e 6420 616e 2049   an ARK and an I
+00003e40: 5249 2061 7265 2070 726f 7669 6465 640a  RI are provided.
+00003e50: 2020 2020 2020 2020 4261 7365 4572 726f          BaseErro
+00003e60: 723a 2069 6620 7468 6520 6372 6561 7469  r: if the creati
+00003e70: 6f6e 2064 6174 6520 6973 2069 6e76 616c  on date is inval
+00003e80: 6964 0a0a 2020 2020 4578 616d 706c 6573  id..    Examples
+00003e90: 3a0a 2020 2020 2020 2020 3e3e 3e20 7265  :.        >>> re
+00003ea0: 736f 7572 6365 203d 2065 7863 656c 3278  source = excel2x
+00003eb0: 6d6c 2e6d 616b 655f 7265 736f 7572 6365  ml.make_resource
+00003ec0: 282e 2e2e 290a 2020 2020 2020 2020 3e3e  (...).        >>
+00003ed0: 3e20 7265 736f 7572 6365 2e61 7070 656e  > resource.appen
+00003ee0: 6428 6578 6365 6c32 786d 6c2e 6d61 6b65  d(excel2xml.make
+00003ef0: 5f74 6578 745f 7072 6f70 282e 2e2e 2929  _text_prop(...))
+00003f00: 0a20 2020 2020 2020 203e 3e3e 2072 6f6f  .        >>> roo
+00003f10: 742e 6170 7065 6e64 2872 6573 6f75 7263  t.append(resourc
+00003f20: 6529 0a0a 2020 2020 5365 6520 6874 7470  e)..    See http
+00003f30: 733a 2f2f 646f 6373 2e64 6173 6368 2e73  s://docs.dasch.s
+00003f40: 7769 7373 2f6c 6174 6573 742f 4453 502d  wiss/latest/DSP-
+00003f50: 544f 4f4c 532f 6669 6c65 2d66 6f72 6d61  TOOLS/file-forma
+00003f60: 7473 2f78 6d6c 2d64 6174 612d 6669 6c65  ts/xml-data-file
+00003f70: 2f23 6465 7363 7269 6269 6e67 2d72 6573  /#describing-res
+00003f80: 6f75 7263 6573 2d77 6974 682d 7468 652d  ources-with-the-
+00003f90: 7265 736f 7572 6365 2d65 6c65 6d65 6e74  resource-element
+00003fa0: 0a20 2020 2022 2222 0a20 2020 2069 6620  .    """.    if 
+00003fb0: 6e6f 7420 6368 6563 6b5f 6e6f 746e 6128  not check_notna(
+00003fc0: 6c61 6265 6c29 3a0a 2020 2020 2020 2020  label):.        
+00003fd0: 6d73 6720 3d20 6622 596f 7572 2072 6573  msg = f"Your res
+00003fe0: 6f75 7263 6527 7320 6c61 6265 6c20 6c6f  ource's label lo
+00003ff0: 6f6b 7320 7375 7370 6963 696f 7573 2028  oks suspicious (
+00004000: 7265 736f 7572 6365 2077 6974 6820 6964  resource with id
+00004010: 2027 7b69 647d 2720 616e 6420 6c61 6265   '{id}' and labe
+00004020: 6c20 277b 6c61 6265 6c7d 2729 220a 2020  l '{label}')".  
+00004030: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
+00004040: 6172 6e28 4473 7054 6f6f 6c73 5573 6572  arn(DspToolsUser
+00004050: 5761 726e 696e 6728 6d73 6729 290a 2020  Warning(msg)).  
+00004060: 2020 6966 206e 6f74 2063 6865 636b 5f6e    if not check_n
+00004070: 6f74 6e61 2869 6429 3a0a 2020 2020 2020  otna(id):.      
+00004080: 2020 6d73 6720 3d20 6622 596f 7572 2072    msg = f"Your r
+00004090: 6573 6f75 7263 6527 7320 6964 206c 6f6f  esource's id loo
+000040a0: 6b73 2073 7573 7069 6369 6f75 7320 2872  ks suspicious (r
+000040b0: 6573 6f75 7263 6520 7769 7468 2069 6420  esource with id 
+000040c0: 277b 6964 7d27 2061 6e64 206c 6162 656c  '{id}' and label
+000040d0: 2027 7b6c 6162 656c 7d27 220a 2020 2020   '{label}'".    
+000040e0: 2020 2020 7761 726e 696e 6773 2e77 6172      warnings.war
+000040f0: 6e28 4473 7054 6f6f 6c73 5573 6572 5761  n(DspToolsUserWa
+00004100: 726e 696e 6728 6d73 6729 290a 2020 2020  rning(msg)).    
+00004110: 6b77 6172 6773 203d 207b 226c 6162 656c  kwargs = {"label
+00004120: 223a 206c 6162 656c 2c20 2272 6573 7479  ": label, "resty
+00004130: 7065 223a 2072 6573 7479 7065 2c20 2269  pe": restype, "i
+00004140: 6422 3a20 6964 2c20 2270 6572 6d69 7373  d": id, "permiss
+00004150: 696f 6e73 223a 2070 6572 6d69 7373 696f  ions": permissio
+00004160: 6e73 2c20 226e 736d 6170 223a 2078 6d6c  ns, "nsmap": xml
+00004170: 5f6e 616d 6573 7061 6365 5f6d 6170 7d0a  _namespace_map}.
+00004180: 2020 2020 6966 2061 726b 3a0a 2020 2020      if ark:.    
+00004190: 2020 2020 6b77 6172 6773 5b22 6172 6b22      kwargs["ark"
+000041a0: 5d20 3d20 6172 6b0a 2020 2020 6966 2069  ] = ark.    if i
+000041b0: 7269 3a0a 2020 2020 2020 2020 6b77 6172  ri:.        kwar
+000041c0: 6773 5b22 6972 6922 5d20 3d20 6972 690a  gs["iri"] = iri.
+000041d0: 2020 2020 6966 2061 726b 2061 6e64 2069      if ark and i
+000041e0: 7269 3a0a 2020 2020 2020 2020 6d73 6720  ri:.        msg 
+000041f0: 3d20 6622 426f 7468 2041 524b 2061 6e64  = f"Both ARK and
+00004200: 2049 5249 2077 6572 6520 7072 6f76 6964   IRI were provid
+00004210: 6564 2066 6f72 2072 6573 6f75 7263 6520  ed for resource 
+00004220: 277b 6c61 6265 6c7d 2720 287b 6964 7d29  '{label}' ({id})
+00004230: 2e20 5468 6520 4152 4b20 7769 6c6c 206f  . The ARK will o
+00004240: 7665 7272 6964 6520 7468 6520 4952 492e  verride the IRI.
+00004250: 220a 2020 2020 2020 2020 7761 726e 696e  ".        warnin
+00004260: 6773 2e77 6172 6e28 4473 7054 6f6f 6c73  gs.warn(DspTools
+00004270: 5573 6572 5761 726e 696e 6728 6d73 6729  UserWarning(msg)
+00004280: 290a 2020 2020 6966 2063 7265 6174 696f  ).    if creatio
+00004290: 6e5f 6461 7465 3a0a 2020 2020 2020 2020  n_date:.        
+000042a0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+000042b0: 2044 6174 6554 696d 6553 7461 6d70 2863   DateTimeStamp(c
+000042c0: 7265 6174 696f 6e5f 6461 7465 290a 2020  reation_date).  
+000042d0: 2020 2020 2020 6578 6365 7074 2042 6173        except Bas
+000042e0: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
+000042f0: 2020 2020 7261 6973 6520 4261 7365 4572      raise BaseEr
+00004300: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+00004310: 2020 2020 2066 2254 6865 2072 6573 6f75       f"The resou
+00004320: 7263 6520 277b 6c61 6265 6c7d 2720 2849  rce '{label}' (I
+00004330: 443a 207b 6964 7d29 2068 6173 2061 6e20  D: {id}) has an 
+00004340: 696e 7661 6c69 6420 6372 6561 7469 6f6e  invalid creation
+00004350: 2064 6174 6520 277b 6372 6561 7469 6f6e   date '{creation
+00004360: 5f64 6174 657d 272e 2022 0a20 2020 2020  _date}'. ".     
+00004370: 2020 2020 2020 2020 2020 2066 2244 6964             f"Did
+00004380: 2079 6f75 2070 6572 6861 7073 2066 6f72   you perhaps for
+00004390: 6765 7420 7468 6520 7469 6d65 7a6f 6e65  get the timezone
+000043a0: 3f22 0a20 2020 2020 2020 2020 2020 2029  ?".            )
+000043b0: 2066 726f 6d20 4e6f 6e65 0a20 2020 2020   from None.     
+000043c0: 2020 206b 7761 7267 735b 2263 7265 6174     kwargs["creat
+000043d0: 696f 6e5f 6461 7465 225d 203d 2063 7265  ion_date"] = cre
+000043e0: 6174 696f 6e5f 6461 7465 0a0a 2020 2020  ation_date..    
+000043f0: 7265 7475 726e 2065 7472 6565 2e45 6c65  return etree.Ele
+00004400: 6d65 6e74 2822 7b25 737d 7265 736f 7572  ment("{%s}resour
+00004410: 6365 2220 2520 786d 6c5f 6e61 6d65 7370  ce" % xml_namesp
+00004420: 6163 655f 6d61 705b 4e6f 6e65 5d2c 202a  ace_map[None], *
+00004430: 2a6b 7761 7267 7329 2020 2320 7479 7065  *kwargs)  # type
+00004440: 3a20 6967 6e6f 7265 5b61 7267 2d74 7970  : ignore[arg-typ
+00004450: 655d 0a0a 0a64 6566 206d 616b 655f 6269  e]...def make_bi
+00004460: 7473 7472 6561 6d5f 7072 6f70 280a 2020  tstream_prop(.  
+00004470: 2020 7061 7468 3a20 556e 696f 6e5b 7374    path: Union[st
+00004480: 722c 206f 732e 5061 7468 4c69 6b65 5b41  r, os.PathLike[A
+00004490: 6e79 5d5d 2c0a 2020 2020 7065 726d 6973  ny]],.    permis
+000044a0: 7369 6f6e 733a 2073 7472 203d 2022 7072  sions: str = "pr
+000044b0: 6f70 2d64 6566 6175 6c74 222c 0a20 2020  op-default",.   
+000044c0: 2063 6865 636b 3a20 626f 6f6c 203d 2046   check: bool = F
+000044d0: 616c 7365 2c0a 2020 2020 6361 6c6c 696e  alse,.    callin
+000044e0: 675f 7265 736f 7572 6365 3a20 7374 7220  g_resource: str 
+000044f0: 3d20 2222 2c0a 2920 2d3e 2065 7472 6565  = "",.) -> etree
+00004500: 2e5f 456c 656d 656e 743a 0a20 2020 2022  ._Element:.    "
+00004510: 2222 0a20 2020 2043 7265 6174 6573 2061  "".    Creates a
+00004520: 2062 6974 7374 7265 616d 2065 6c65 6d65   bitstream eleme
+00004530: 6e74 2074 6861 7420 706f 696e 7473 2074  nt that points t
+00004540: 6f20 2270 6174 6822 2e0a 0a20 2020 2041  o "path"...    A
+00004550: 7267 733a 0a20 2020 2020 2020 2070 6174  rgs:.        pat
+00004560: 683a 2070 6174 6820 746f 2061 2076 616c  h: path to a val
+00004570: 6964 2066 696c 6520 7468 6174 2077 696c  id file that wil
+00004580: 6c20 6265 2075 706c 6f61 6465 640a 2020  l be uploaded.  
+00004590: 2020 2020 2020 7065 726d 6973 7369 6f6e        permission
+000045a0: 733a 2070 6572 6d69 7373 696f 6e73 2073  s: permissions s
+000045b0: 7472 696e 670a 2020 2020 2020 2020 6368  tring.        ch
+000045c0: 6563 6b3a 2069 6620 5472 7565 2c20 6973  eck: if True, is
+000045d0: 7375 6520 6120 7761 726e 696e 6720 6966  sue a warning if
+000045e0: 2074 6865 2070 6174 6820 646f 6573 6e27   the path doesn'
+000045f0: 7420 706f 696e 7420 746f 2061 6e20 6578  t point to an ex
+00004600: 6973 7469 6e67 2066 696c 650a 2020 2020  isting file.    
+00004610: 2020 2020 6361 6c6c 696e 675f 7265 736f      calling_reso
+00004620: 7572 6365 3a20 7468 6520 6e61 6d65 206f  urce: the name o
+00004630: 6620 7468 6520 7061 7265 6e74 2072 6573  f the parent res
+00004640: 6f75 7263 6520 2866 6f72 2062 6574 7465  ource (for bette
+00004650: 7220 6572 726f 7220 6d65 7373 6167 6573  r error messages
+00004660: 290a 0a20 2020 2057 6172 6e73 3a0a 2020  )..    Warns:.  
+00004670: 2020 2020 2020 6966 2074 6865 2070 6174        if the pat
+00004680: 6820 646f 6573 6e27 7420 706f 696e 7420  h doesn't point 
+00004690: 746f 2061 6e20 6578 6973 7469 6e67 2066  to an existing f
+000046a0: 696c 6520 286f 6e6c 7920 6966 2063 6865  ile (only if che
+000046b0: 636b 3d54 7275 6529 0a0a 2020 2020 5265  ck=True)..    Re
+000046c0: 7475 726e 733a 0a20 2020 2020 2020 2061  turns:.        a
+000046d0: 6e20 6574 7265 652e 5f45 6c65 6d65 6e74  n etree._Element
+000046e0: 2074 6861 7420 6361 6e20 6265 2061 7070   that can be app
+000046f0: 656e 6465 6420 746f 2074 6865 2070 6172  ended to the par
+00004700: 656e 7420 7265 736f 7572 6365 2077 6974  ent resource wit
+00004710: 6820 7265 736f 7572 6365 2e61 7070 656e  h resource.appen
+00004720: 6428 6d61 6b65 5f2a 5f70 726f 7028 2e2e  d(make_*_prop(..
+00004730: 2e29 290a 0a20 2020 2045 7861 6d70 6c65  .))..    Example
+00004740: 733a 0a20 2020 2020 2020 203e 3e3e 2072  s:.        >>> r
+00004750: 6573 6f75 7263 6520 3d20 6578 6365 6c32  esource = excel2
+00004760: 786d 6c2e 6d61 6b65 5f72 6573 6f75 7263  xml.make_resourc
+00004770: 6528 2e2e 2e29 0a20 2020 2020 2020 203e  e(...).        >
+00004780: 3e3e 2072 6573 6f75 7263 652e 6170 7065  >> resource.appe
+00004790: 6e64 2865 7863 656c 3278 6d6c 2e6d 616b  nd(excel2xml.mak
+000047a0: 655f 6269 7473 7472 6561 6d5f 7072 6f70  e_bitstream_prop
+000047b0: 2822 6461 7461 2f69 6d61 6765 732f 7472  ("data/images/tr
+000047c0: 6565 2e6a 7067 2229 290a 2020 2020 2020  ee.jpg")).      
+000047d0: 2020 3e3e 3e20 726f 6f74 2e61 7070 656e    >>> root.appen
+000047e0: 6428 7265 736f 7572 6365 290a 0a20 2020  d(resource)..   
+000047f0: 2053 6565 2068 7474 7073 3a2f 2f64 6f63   See https://doc
+00004800: 732e 6461 7363 682e 7377 6973 732f 6c61  s.dasch.swiss/la
+00004810: 7465 7374 2f44 5350 2d54 4f4f 4c53 2f66  test/DSP-TOOLS/f
+00004820: 696c 652d 666f 726d 6174 732f 786d 6c2d  ile-formats/xml-
+00004830: 6461 7461 2d66 696c 652f 2362 6974 7374  data-file/#bitst
+00004840: 7265 616d 0a20 2020 2022 2222 0a0a 2020  ream.    """..  
+00004850: 2020 6966 2063 6865 636b 2061 6e64 206e    if check and n
+00004860: 6f74 2050 6174 6828 7061 7468 292e 6973  ot Path(path).is
+00004870: 5f66 696c 6528 293a 0a20 2020 2020 2020  _file():.       
+00004880: 206d 7367 203d 2028 0a20 2020 2020 2020   msg = (.       
+00004890: 2020 2020 2066 2246 6169 6c65 6420 7661       f"Failed va
+000048a0: 6c69 6461 7469 6f6e 2069 6e20 6269 7473  lidation in bits
+000048b0: 7472 6561 6d20 7461 6720 6f66 2072 6573  tream tag of res
+000048c0: 6f75 7263 6520 277b 6361 6c6c 696e 675f  ource '{calling_
+000048d0: 7265 736f 7572 6365 7d27 3a20 220a 2020  resource}': ".  
+000048e0: 2020 2020 2020 2020 2020 6622 5468 6520            f"The 
+000048f0: 666f 6c6c 6f77 696e 6720 7061 7468 2064  following path d
+00004900: 6f65 736e 2774 2070 6f69 6e74 2074 6f20  oesn't point to 
+00004910: 6120 6669 6c65 3a20 7b70 6174 687d 220a  a file: {path}".
+00004920: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00004930: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
+00004940: 4473 7054 6f6f 6c73 5573 6572 5761 726e  DspToolsUserWarn
+00004950: 696e 6728 6d73 6729 290a 2020 2020 7072  ing(msg)).    pr
+00004960: 6f70 5f20 3d20 6574 7265 652e 456c 656d  op_ = etree.Elem
+00004970: 656e 7428 0a20 2020 2020 2020 2022 7b25  ent(.        "{%
+00004980: 737d 6269 7473 7472 6561 6d22 2025 2078  s}bitstream" % x
+00004990: 6d6c 5f6e 616d 6573 7061 6365 5f6d 6170  ml_namespace_map
+000049a0: 5b4e 6f6e 655d 2c0a 2020 2020 2020 2020  [None],.        
+000049b0: 7065 726d 6973 7369 6f6e 733d 7065 726d  permissions=perm
+000049c0: 6973 7369 6f6e 732c 0a20 2020 2020 2020  issions,.       
+000049d0: 206e 736d 6170 3d78 6d6c 5f6e 616d 6573   nsmap=xml_names
+000049e0: 7061 6365 5f6d 6170 2c0a 2020 2020 290a  pace_map,.    ).
+000049f0: 2020 2020 7072 6f70 5f2e 7465 7874 203d      prop_.text =
+00004a00: 2073 7472 2870 6174 6829 0a20 2020 2072   str(path).    r
+00004a10: 6574 7572 6e20 7072 6f70 5f0a 0a0a 6465  eturn prop_...de
+00004a20: 6620 5f66 6f72 6d61 745f 626f 6f6c 280a  f _format_bool(.
+00004a30: 2020 2020 756e 666f 726d 6174 7465 643a      unformatted:
+00004a40: 2055 6e69 6f6e 5b62 6f6f 6c2c 2073 7472   Union[bool, str
+00004a50: 2c20 696e 742c 2066 6c6f 6174 5d2c 0a20  , int, float],. 
+00004a60: 2020 206e 616d 653a 2073 7472 2c0a 2020     name: str,.  
+00004a70: 2020 6361 6c6c 696e 675f 7265 736f 7572    calling_resour
+00004a80: 6365 3a20 7374 722c 0a29 202d 3e20 7374  ce: str,.) -> st
+00004a90: 723a 0a20 2020 2022 2222 0a20 2020 2054  r:.    """.    T
+00004aa0: 6869 7320 6d65 7468 6f64 2074 616b 6573  his method takes
+00004ab0: 2061 6e20 756e 666f 726d 6174 7465 6420   an unformatted 
+00004ac0: 626f 6f6c 6561 6e2d 6c69 6b65 2076 616c  boolean-like val
+00004ad0: 7565 2c20 616e 6420 7472 616e 7366 6f72  ue, and transfor
+00004ae0: 6d73 2069 7420 696e 746f 2074 6865 2073  ms it into the s
+00004af0: 7472 696e 6720 7661 6c75 6573 2022 7472  tring values "tr
+00004b00: 7565 2220 6f72 2022 6661 6c73 6522 2e0a  ue" or "false"..
+00004b10: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
+00004b20: 2020 2075 6e66 6f72 6d61 7474 6564 3a20     unformatted: 
+00004b30: 626f 6f6c 6561 6e2d 6c69 6b65 2076 616c  boolean-like val
+00004b40: 7565 0a20 2020 2020 2020 206e 616d 653a  ue.        name:
+00004b50: 2070 726f 7065 7274 7920 6e61 6d65 2c20   property name, 
+00004b60: 666f 7220 6265 7474 6572 2065 7272 6f72  for better error
+00004b70: 206d 6573 7361 6765 730a 2020 2020 2020   messages.      
+00004b80: 2020 6361 6c6c 696e 675f 7265 736f 7572    calling_resour
+00004b90: 6365 3a20 7265 736f 7572 6365 206e 616d  ce: resource nam
+00004ba0: 652c 2066 6f72 2062 6574 7465 7220 6572  e, for better er
+00004bb0: 726f 7220 6d65 7373 6167 6573 0a0a 2020  ror messages..  
+00004bc0: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
+00004bd0: 2020 4261 7365 4572 726f 723a 2069 6620    BaseError: if 
+00004be0: 7468 6520 696e 7075 7420 6361 6e6e 6f74  the input cannot
+00004bf0: 2062 6520 7472 616e 7366 6f72 6d65 6420   be transformed 
+00004c00: 696e 746f 2022 7472 7565 222f 2266 616c  into "true"/"fal
+00004c10: 7365 220a 0a20 2020 2052 6574 7572 6e73  se"..    Returns
+00004c20: 3a0a 2020 2020 2020 2020 2274 7275 6522  :.        "true"
+00004c30: 2069 6620 7468 6520 696e 7075 7420 6973   if the input is
+00004c40: 2069 6e20 2854 7275 652c 2022 7472 7565   in (True, "true
+00004c50: 222c 2022 3122 2c20 312c 2022 7965 7322  ", "1", 1, "yes"
+00004c60: 293b 2022 6661 6c73 6522 2069 6620 696e  ); "false" if in
+00004c70: 7075 7420 6973 2069 6e20 2846 616c 7365  put is in (False
+00004c80: 2c20 2266 616c 7365 222c 2022 3022 2c20  , "false", "0", 
+00004c90: 302c 2022 6e6f 2229 0a20 2020 2022 2222  0, "no").    """
+00004ca0: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
+00004cb0: 6365 2875 6e66 6f72 6d61 7474 6564 2c20  ce(unformatted, 
+00004cc0: 7374 7229 3a0a 2020 2020 2020 2020 756e  str):.        un
+00004cd0: 666f 726d 6174 7465 6420 3d20 756e 666f  formatted = unfo
+00004ce0: 726d 6174 7465 642e 6c6f 7765 7228 290a  rmatted.lower().
+00004cf0: 2020 2020 6966 2075 6e66 6f72 6d61 7474      if unformatt
+00004d00: 6564 2069 6e20 2846 616c 7365 2c20 2266  ed in (False, "f
+00004d10: 616c 7365 222c 2022 3022 2c20 302c 2030  alse", "0", 0, 0
+00004d20: 2e30 2c20 226e 6f22 293a 0a20 2020 2020  .0, "no"):.     
+00004d30: 2020 2072 6574 7572 6e20 2266 616c 7365     return "false
+00004d40: 220a 2020 2020 656c 6966 2075 6e66 6f72  ".    elif unfor
+00004d50: 6d61 7474 6564 2069 6e20 2854 7275 652c  matted in (True,
+00004d60: 2022 7472 7565 222c 2022 3122 2c20 312c   "true", "1", 1,
+00004d70: 2031 2e30 2c20 2279 6573 2229 3a0a 2020   1.0, "yes"):.  
+00004d80: 2020 2020 2020 7265 7475 726e 2022 7472        return "tr
+00004d90: 7565 220a 2020 2020 656c 7365 3a0a 2020  ue".    else:.  
+00004da0: 2020 2020 2020 7261 6973 6520 4261 7365        raise Base
+00004db0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+00004dc0: 2020 2066 2246 6169 6c65 6420 7661 6c69     f"Failed vali
+00004dd0: 6461 7469 6f6e 2069 6e20 7265 736f 7572  dation in resour
+00004de0: 6365 2027 7b63 616c 6c69 6e67 5f72 6573  ce '{calling_res
+00004df0: 6f75 7263 657d 272c 2070 726f 7065 7274  ource}', propert
+00004e00: 7920 277b 6e61 6d65 7d27 3a20 220a 2020  y '{name}': ".  
+00004e10: 2020 2020 2020 2020 2020 6622 277b 756e            f"'{un
+00004e20: 666f 726d 6174 7465 647d 2720 6973 206e  formatted}' is n
+00004e30: 6f74 2061 2076 616c 6964 2062 6f6f 6c65  ot a valid boole
+00004e40: 616e 2e22 0a20 2020 2020 2020 2029 0a0a  an.".        )..
+00004e50: 0a64 6566 206d 616b 655f 626f 6f6c 6561  .def make_boolea
+00004e60: 6e5f 7072 6f70 280a 2020 2020 6e61 6d65  n_prop(.    name
+00004e70: 3a20 7374 722c 0a20 2020 2076 616c 7565  : str,.    value
+00004e80: 3a20 556e 696f 6e5b 5072 6f70 6572 7479  : Union[Property
+00004e90: 456c 656d 656e 742c 2073 7472 2c20 696e  Element, str, in
+00004ea0: 742c 2062 6f6f 6c5d 2c0a 2020 2020 6361  t, bool],.    ca
+00004eb0: 6c6c 696e 675f 7265 736f 7572 6365 3a20  lling_resource: 
+00004ec0: 7374 7220 3d20 2222 2c0a 2920 2d3e 2065  str = "",.) -> e
+00004ed0: 7472 6565 2e5f 456c 656d 656e 743a 0a20  tree._Element:. 
+00004ee0: 2020 2022 2222 0a20 2020 204d 616b 6520     """.    Make 
+00004ef0: 6120 3c62 6f6f 6c65 616e 2d70 726f 703e  a <boolean-prop>
+00004f00: 2066 726f 6d20 6120 626f 6f6c 6561 6e20   from a boolean 
+00004f10: 7661 6c75 652e 2054 6865 2076 616c 7565  value. The value
+00004f20: 2063 616e 2062 6520 7072 6f76 6964 6564   can be provided
+00004f30: 2064 6972 6563 746c 7920 6f72 2069 6e73   directly or ins
+00004f40: 6964 6520 6120 5072 6f70 6572 7479 456c  ide a PropertyEl
+00004f50: 656d 656e 742e 2054 6865 0a20 2020 2066  ement. The.    f
+00004f60: 6f6c 6c6f 7769 6e67 2066 6f72 6d61 7473  ollowing formats
+00004f70: 2061 7265 2073 7570 706f 7274 6564 3a0a   are supported:.
+00004f80: 2020 2020 202d 2074 7275 653a 2028 5472       - true: (Tr
+00004f90: 7565 2c20 2274 7275 6522 2c20 2254 7275  ue, "true", "Tru
+00004fa0: 6522 2c20 2231 222c 2031 2c20 2279 6573  e", "1", 1, "yes
+00004fb0: 222c 2022 5965 7322 290a 2020 2020 202d  ", "Yes").     -
+00004fc0: 2066 616c 7365 3a20 2846 616c 7365 2c20   false: (False, 
+00004fd0: 2266 616c 7365 222c 2022 4661 6c73 6522  "false", "False"
+00004fe0: 2c20 2230 222c 2030 2c20 226e 6f22 2c20  , "0", 0, "no", 
+00004ff0: 224e 6f22 290a 0a20 2020 2055 6e6c 6573  "No")..    Unles
+00005000: 7320 7072 6f76 6964 6564 2061 7320 5072  s provided as Pr
+00005010: 6f70 6572 7479 456c 656d 656e 742c 2074  opertyElement, t
+00005020: 6865 2070 6572 6d69 7373 696f 6e73 206f  he permissions o
+00005030: 6620 7468 6520 7661 6c75 6520 6465 6661  f the value defa
+00005040: 756c 7420 746f 2022 7072 6f70 2d64 6566  ult to "prop-def
+00005050: 6175 6c74 222e 0a0a 2020 2020 4172 6773  ault"...    Args
+00005060: 3a0a 2020 2020 2020 2020 6e61 6d65 3a20  :.        name: 
+00005070: 7468 6520 6e61 6d65 206f 6620 7468 6973  the name of this
+00005080: 2070 726f 7065 7274 7920 6173 2064 6566   property as def
+00005090: 696e 6564 2069 6e20 7468 6520 6f6e 746f  ined in the onto
+000050a0: 0a20 2020 2020 2020 2076 616c 7565 3a20  .        value: 
+000050b0: 6120 626f 6f6c 6561 6e20 7661 6c75 6520  a boolean value 
+000050c0: 6173 2073 7472 2f62 6f6f 6c2f 696e 742c  as str/bool/int,
+000050d0: 206f 7220 6173 2073 7472 2f62 6f6f 6c2f   or as str/bool/
+000050e0: 696e 7420 696e 7369 6465 2061 2050 726f  int inside a Pro
+000050f0: 7065 7274 7945 6c65 6d65 6e74 0a20 2020  pertyElement.   
+00005100: 2020 2020 2063 616c 6c69 6e67 5f72 6573       calling_res
+00005110: 6f75 7263 653a 2074 6865 206e 616d 6520  ource: the name 
+00005120: 6f66 2074 6865 2070 6172 656e 7420 7265  of the parent re
+00005130: 736f 7572 6365 2028 666f 7220 6265 7474  source (for bett
+00005140: 6572 2065 7272 6f72 206d 6573 7361 6765  er error message
+00005150: 7329 0a0a 2020 2020 5261 6973 6573 3a0a  s)..    Raises:.
+00005160: 2020 2020 2020 2020 4261 7365 4572 726f          BaseErro
+00005170: 723a 2069 6620 7468 6520 7661 6c75 6520  r: if the value 
+00005180: 6973 206e 6f74 2061 2076 616c 6964 2062  is not a valid b
+00005190: 6f6f 6c65 616e 0a0a 2020 2020 5265 7475  oolean..    Retu
+000051a0: 726e 733a 0a20 2020 2020 2020 2061 6e20  rns:.        an 
+000051b0: 6574 7265 652e 5f45 6c65 6d65 6e74 2074  etree._Element t
+000051c0: 6861 7420 6361 6e20 6265 2061 7070 656e  hat can be appen
+000051d0: 6465 6420 746f 2074 6865 2070 6172 656e  ded to the paren
+000051e0: 7420 7265 736f 7572 6365 2077 6974 6820  t resource with 
+000051f0: 7265 736f 7572 6365 2e61 7070 656e 6428  resource.append(
+00005200: 6d61 6b65 5f2a 5f70 726f 7028 2e2e 2e29  make_*_prop(...)
+00005210: 290a 0a20 2020 2045 7861 6d70 6c65 733a  )..    Examples:
+00005220: 0a20 2020 2020 2020 203e 3e3e 2065 7863  .        >>> exc
+00005230: 656c 3278 6d6c 2e6d 616b 655f 626f 6f6c  el2xml.make_bool
+00005240: 6561 6e5f 7072 6f70 2822 3a74 6573 7470  ean_prop(":testp
+00005250: 726f 7065 7274 7922 2c20 226e 6f22 290a  roperty", "no").
+00005260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005270: 3c62 6f6f 6c65 616e 2d70 726f 7020 6e61  <boolean-prop na
+00005280: 6d65 3d22 3a74 6573 7470 726f 7065 7274  me=":testpropert
+00005290: 7922 3e0a 2020 2020 2020 2020 2020 2020  y">.            
+000052a0: 2020 2020 2020 2020 3c62 6f6f 6c65 616e          <boolean
+000052b0: 2070 6572 6d69 7373 696f 6e73 3d22 7072   permissions="pr
+000052c0: 6f70 2d64 6566 6175 6c74 223e 6661 6c73  op-default">fals
+000052d0: 653c 2f62 6f6f 6c65 616e 3e0a 2020 2020  e</boolean>.    
+000052e0: 2020 2020 2020 2020 2020 2020 3c2f 626f              </bo
+000052f0: 6f6c 6561 6e2d 7072 6f70 3e0a 2020 2020  olean-prop>.    
+00005300: 2020 2020 3e3e 3e20 6578 6365 6c32 786d      >>> excel2xm
+00005310: 6c2e 6d61 6b65 5f62 6f6f 6c65 616e 5f70  l.make_boolean_p
+00005320: 726f 7028 223a 7465 7374 7072 6f70 6572  rop(":testproper
+00005330: 7479 222c 2065 7863 656c 3278 6d6c 2e50  ty", excel2xml.P
+00005340: 726f 7065 7274 7945 6c65 6d65 6e74 2822  ropertyElement("
+00005350: 3122 2c20 7065 726d 6973 7369 6f6e 733d  1", permissions=
+00005360: 2270 726f 702d 7265 7374 7269 6374 6564  "prop-restricted
+00005370: 222c 2063 6f6d 6d65 6e74 3d22 6578 616d  ", comment="exam
+00005380: 706c 6522 2929 0a20 2020 2020 2020 2020  ple")).         
+00005390: 2020 2020 2020 203c 626f 6f6c 6561 6e2d         <boolean-
+000053a0: 7072 6f70 206e 616d 653d 223a 7465 7374  prop name=":test
+000053b0: 7072 6f70 6572 7479 223e 0a20 2020 2020  property">.     
+000053c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000053d0: 626f 6f6c 6561 6e20 7065 726d 6973 7369  boolean permissi
+000053e0: 6f6e 733d 2270 726f 702d 7265 7374 7269  ons="prop-restri
+000053f0: 6374 6564 2220 636f 6d6d 656e 743d 2265  cted" comment="e
+00005400: 7861 6d70 6c65 223e 7472 7565 3c2f 626f  xample">true</bo
+00005410: 6f6c 6561 6e3e 0a20 2020 2020 2020 2020  olean>.         
+00005420: 2020 2020 2020 203c 2f62 6f6f 6c65 616e         </boolean
+00005430: 2d70 726f 703e 0a0a 2020 2020 5365 6520  -prop>..    See 
+00005440: 6874 7470 733a 2f2f 646f 6373 2e64 6173  https://docs.das
+00005450: 6368 2e73 7769 7373 2f6c 6174 6573 742f  ch.swiss/latest/
+00005460: 4453 502d 544f 4f4c 532f 6669 6c65 2d66  DSP-TOOLS/file-f
+00005470: 6f72 6d61 7473 2f78 6d6c 2d64 6174 612d  ormats/xml-data-
+00005480: 6669 6c65 2f23 626f 6f6c 6561 6e2d 7072  file/#boolean-pr
+00005490: 6f70 0a20 2020 2022 2222 0a0a 2020 2020  op.    """..    
+000054a0: 2320 7661 6c69 6461 7465 2069 6e70 7574  # validate input
+000054b0: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
+000054c0: 6365 2876 616c 7565 2c20 5072 6f70 6572  ce(value, Proper
+000054d0: 7479 456c 656d 656e 7429 3a0a 2020 2020  tyElement):.    
+000054e0: 2020 2020 7661 6c75 655f 6e65 7720 3d20      value_new = 
+000054f0: 6461 7461 636c 6173 7365 732e 7265 706c  dataclasses.repl
+00005500: 6163 6528 7661 6c75 652c 2076 616c 7565  ace(value, value
+00005510: 3d5f 666f 726d 6174 5f62 6f6f 6c28 7661  =_format_bool(va
+00005520: 6c75 652e 7661 6c75 652c 206e 616d 652c  lue.value, name,
+00005530: 2063 616c 6c69 6e67 5f72 6573 6f75 7263   calling_resourc
+00005540: 6529 290a 2020 2020 656c 6966 2069 7369  e)).    elif isi
+00005550: 6e73 7461 6e63 6528 7661 6c75 652c 2028  nstance(value, (
+00005560: 7374 722c 2062 6f6f 6c2c 2069 6e74 2929  str, bool, int))
+00005570: 3a0a 2020 2020 2020 2020 7661 6c75 655f  :.        value_
+00005580: 6e65 7720 3d20 5072 6f70 6572 7479 456c  new = PropertyEl
+00005590: 656d 656e 7428 5f66 6f72 6d61 745f 626f  ement(_format_bo
+000055a0: 6f6c 2876 616c 7565 2c20 6e61 6d65 2c20  ol(value, name, 
+000055b0: 6361 6c6c 696e 675f 7265 736f 7572 6365  calling_resource
+000055c0: 2929 0a20 2020 2065 6c73 653a 0a20 2020  )).    else:.   
+000055d0: 2020 2020 2072 6169 7365 2042 6173 6545       raise BaseE
+000055e0: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+000055f0: 2020 6622 4661 696c 6564 2076 616c 6964    f"Failed valid
+00005600: 6174 696f 6e20 696e 2072 6573 6f75 7263  ation in resourc
+00005610: 6520 277b 6361 6c6c 696e 675f 7265 736f  e '{calling_reso
+00005620: 7572 6365 7d27 2c20 7072 6f70 6572 7479  urce}', property
+00005630: 2027 7b6e 616d 657d 273a 2027 7b76 616c   '{name}': '{val
+00005640: 7565 7d27 2069 7320 6e6f 7420 6120 7661  ue}' is not a va
+00005650: 6c69 6420 626f 6f6c 6561 6e2e 220a 2020  lid boolean.".  
+00005660: 2020 2020 2020 290a 0a20 2020 2023 206d        )..    # m
+00005670: 616b 6520 786d 6c20 7374 7275 6374 7572  ake xml structur
+00005680: 6520 6f66 2074 6865 2076 616c 7565 0a20  e of the value. 
+00005690: 2020 2070 726f 705f 203d 2065 7472 6565     prop_ = etree
+000056a0: 2e45 6c65 6d65 6e74 280a 2020 2020 2020  .Element(.      
+000056b0: 2020 227b 2573 7d62 6f6f 6c65 616e 2d70    "{%s}boolean-p
+000056c0: 726f 7022 2025 2078 6d6c 5f6e 616d 6573  rop" % xml_names
+000056d0: 7061 6365 5f6d 6170 5b4e 6f6e 655d 2c0a  pace_map[None],.
+000056e0: 2020 2020 2020 2020 6e61 6d65 3d6e 616d          name=nam
+000056f0: 652c 0a20 2020 2020 2020 206e 736d 6170  e,.        nsmap
+00005700: 3d78 6d6c 5f6e 616d 6573 7061 6365 5f6d  =xml_namespace_m
+00005710: 6170 2c0a 2020 2020 290a 2020 2020 6b77  ap,.    ).    kw
+00005720: 6172 6773 203d 207b 2270 6572 6d69 7373  args = {"permiss
+00005730: 696f 6e73 223a 2076 616c 7565 5f6e 6577  ions": value_new
+00005740: 2e70 6572 6d69 7373 696f 6e73 7d0a 2020  .permissions}.  
+00005750: 2020 6966 2076 616c 7565 5f6e 6577 2e63    if value_new.c
+00005760: 6f6d 6d65 6e74 2061 6e64 2063 6865 636b  omment and check
+00005770: 5f6e 6f74 6e61 2876 616c 7565 5f6e 6577  _notna(value_new
+00005780: 2e63 6f6d 6d65 6e74 293a 0a20 2020 2020  .comment):.     
+00005790: 2020 206b 7761 7267 735b 2263 6f6d 6d65     kwargs["comme
+000057a0: 6e74 225d 203d 2076 616c 7565 5f6e 6577  nt"] = value_new
+000057b0: 2e63 6f6d 6d65 6e74 0a20 2020 2076 616c  .comment.    val
+000057c0: 7565 5f20 3d20 6574 7265 652e 456c 656d  ue_ = etree.Elem
+000057d0: 656e 7428 0a20 2020 2020 2020 2022 7b25  ent(.        "{%
+000057e0: 737d 626f 6f6c 6561 6e22 2025 2078 6d6c  s}boolean" % xml
+000057f0: 5f6e 616d 6573 7061 6365 5f6d 6170 5b4e  _namespace_map[N
+00005800: 6f6e 655d 2c0a 2020 2020 2020 2020 2a2a  one],.        **
+00005810: 6b77 6172 6773 2c20 2023 2074 7970 653a  kwargs,  # type:
+00005820: 2069 676e 6f72 655b 6172 672d 7479 7065   ignore[arg-type
+00005830: 5d0a 2020 2020 2020 2020 6e73 6d61 703d  ].        nsmap=
+00005840: 786d 6c5f 6e61 6d65 7370 6163 655f 6d61  xml_namespace_ma
+00005850: 702c 0a20 2020 2029 0a20 2020 2076 616c  p,.    ).    val
+00005860: 7565 5f2e 7465 7874 203d 2073 7472 2876  ue_.text = str(v
+00005870: 616c 7565 5f6e 6577 2e76 616c 7565 290a  alue_new.value).
+00005880: 2020 2020 7072 6f70 5f2e 6170 7065 6e64      prop_.append
+00005890: 2876 616c 7565 5f29 0a0a 2020 2020 7265  (value_)..    re
+000058a0: 7475 726e 2070 726f 705f 0a0a 0a64 6566  turn prop_...def
+000058b0: 206d 616b 655f 636f 6c6f 725f 7072 6f70   make_color_prop
+000058c0: 280a 2020 2020 6e61 6d65 3a20 7374 722c  (.    name: str,
+000058d0: 0a20 2020 2076 616c 7565 3a20 556e 696f  .    value: Unio
+000058e0: 6e5b 5072 6f70 6572 7479 456c 656d 656e  n[PropertyElemen
+000058f0: 742c 2073 7472 2c20 4974 6572 6162 6c65  t, str, Iterable
+00005900: 5b55 6e69 6f6e 5b50 726f 7065 7274 7945  [Union[PropertyE
+00005910: 6c65 6d65 6e74 2c20 7374 725d 5d5d 2c0a  lement, str]]],.
+00005920: 2020 2020 6361 6c6c 696e 675f 7265 736f      calling_reso
+00005930: 7572 6365 3a20 7374 7220 3d20 2222 2c0a  urce: str = "",.
+00005940: 2920 2d3e 2065 7472 6565 2e5f 456c 656d  ) -> etree._Elem
+00005950: 656e 743a 0a20 2020 2022 2222 0a20 2020  ent:.    """.   
+00005960: 204d 616b 6520 6120 3c63 6f6c 6f72 2d70   Make a <color-p
+00005970: 726f 703e 2066 726f 6d20 6f6e 6520 6f72  rop> from one or
+00005980: 206d 6f72 6520 636f 6c6f 7273 2e20 5468   more colors. Th
+00005990: 6520 636f 6c6f 7228 7329 2063 616e 2062  e color(s) can b
+000059a0: 6520 7072 6f76 6964 6564 2061 7320 7374  e provided as st
+000059b0: 7269 6e67 206f 7220 6173 2050 726f 7065  ring or as Prope
+000059c0: 7274 7945 6c65 6d65 6e74 2077 6974 6820  rtyElement with 
+000059d0: 610a 2020 2020 7374 7269 6e67 2069 6e73  a.    string ins
+000059e0: 6964 652e 2049 6620 7072 6f76 6964 6564  ide. If provided
+000059f0: 2061 7320 7374 7269 6e67 2c20 7468 6520   as string, the 
+00005a00: 7065 726d 6973 7369 6f6e 7320 6465 6661  permissions defa
+00005a10: 756c 7420 746f 2022 7072 6f70 2d64 6566  ult to "prop-def
+00005a20: 6175 6c74 222e 0a0a 2020 2020 4172 6773  ault"...    Args
+00005a30: 3a0a 2020 2020 2020 2020 6e61 6d65 3a20  :.        name: 
+00005a40: 7468 6520 6e61 6d65 206f 6620 7468 6973  the name of this
+00005a50: 2070 726f 7065 7274 7920 6173 2064 6566   property as def
+00005a60: 696e 6564 2069 6e20 7468 6520 6f6e 746f  ined in the onto
+00005a70: 0a20 2020 2020 2020 2076 616c 7565 3a20  .        value: 
+00005a80: 6f6e 6520 6f72 206d 6f72 6520 4453 5020  one or more DSP 
+00005a90: 636f 6c6f 7228 7329 2c20 6173 2073 7472  color(s), as str
+00005aa0: 696e 672f 5072 6f70 6572 7479 456c 656d  ing/PropertyElem
+00005ab0: 656e 742c 206f 7220 6173 2069 7465 7261  ent, or as itera
+00005ac0: 626c 6520 6f66 2073 7472 696e 6773 2f50  ble of strings/P
+00005ad0: 726f 7065 7274 7945 6c65 6d65 6e74 730a  ropertyElements.
+00005ae0: 2020 2020 2020 2020 6361 6c6c 696e 675f          calling_
+00005af0: 7265 736f 7572 6365 3a20 7468 6520 6e61  resource: the na
+00005b00: 6d65 206f 6620 7468 6520 7061 7265 6e74  me of the parent
+00005b10: 2072 6573 6f75 7263 6520 2866 6f72 2062   resource (for b
+00005b20: 6574 7465 7220 6572 726f 7220 6d65 7373  etter error mess
+00005b30: 6167 6573 290a 0a20 2020 2057 6172 6e73  ages)..    Warns
+00005b40: 3a0a 2020 2020 2020 2020 4966 2074 6865  :.        If the
+00005b50: 2076 616c 7565 2069 7320 6e6f 7420 6120   value is not a 
+00005b60: 7661 6c69 6420 636f 6c6f 720a 0a20 2020  valid color..   
+00005b70: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00005b80: 2020 616e 2065 7472 6565 2e5f 456c 656d    an etree._Elem
+00005b90: 656e 7420 7468 6174 2063 616e 2062 6520  ent that can be 
+00005ba0: 6170 7065 6e64 6564 2074 6f20 7468 6520  appended to the 
+00005bb0: 7061 7265 6e74 2072 6573 6f75 7263 6520  parent resource 
+00005bc0: 7769 7468 2072 6573 6f75 7263 652e 6170  with resource.ap
+00005bd0: 7065 6e64 286d 616b 655f 2a5f 7072 6f70  pend(make_*_prop
+00005be0: 282e 2e2e 2929 0a0a 2020 2020 4578 616d  (...))..    Exam
+00005bf0: 706c 6573 3a0a 2020 2020 2020 2020 3e3e  ples:.        >>
+00005c00: 3e20 6578 6365 6c32 786d 6c2e 6d61 6b65  > excel2xml.make
+00005c10: 5f63 6f6c 6f72 5f70 726f 7028 223a 7465  _color_prop(":te
+00005c20: 7374 7072 6f70 6572 7479 222c 2022 2330  stproperty", "#0
+00005c30: 3066 6636 3622 290a 2020 2020 2020 2020  0ff66").        
+00005c40: 2020 2020 2020 2020 3c63 6f6c 6f72 2d70          <color-p
+00005c50: 726f 7020 6e61 6d65 3d22 3a74 6573 7470  rop name=":testp
+00005c60: 726f 7065 7274 7922 3e0a 2020 2020 2020  roperty">.      
+00005c70: 2020 2020 2020 2020 2020 2020 2020 3c63                <c
+00005c80: 6f6c 6f72 2070 6572 6d69 7373 696f 6e73  olor permissions
+00005c90: 3d22 7072 6f70 2d64 6566 6175 6c74 223e  ="prop-default">
+00005ca0: 2330 3066 6636 363c 2f63 6f6c 6f72 3e0a  #00ff66</color>.
+00005cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cc0: 3c2f 636f 6c6f 722d 7072 6f70 3e0a 2020  </color-prop>.  
+00005cd0: 2020 2020 2020 3e3e 3e20 6578 6365 6c32        >>> excel2
+00005ce0: 786d 6c2e 6d61 6b65 5f63 6f6c 6f72 5f70  xml.make_color_p
+00005cf0: 726f 7028 223a 7465 7374 7072 6f70 6572  rop(":testproper
+00005d00: 7479 222c 2065 7863 656c 3278 6d6c 2e50  ty", excel2xml.P
+00005d10: 726f 7065 7274 7945 6c65 6d65 6e74 2822  ropertyElement("
+00005d20: 2330 3066 6636 3622 2c20 7065 726d 6973  #00ff66", permis
+00005d30: 7369 6f6e 733d 2270 726f 702d 7265 7374  sions="prop-rest
+00005d40: 7269 6374 6564 222c 2063 6f6d 6d65 6e74  ricted", comment
+00005d50: 3d22 6578 616d 706c 6522 2929 0a20 2020  ="example")).   
+00005d60: 2020 2020 2020 2020 2020 2020 203c 636f               <co
+00005d70: 6c6f 722d 7072 6f70 206e 616d 653d 223a  lor-prop name=":
+00005d80: 7465 7374 7072 6f70 6572 7479 223e 0a20  testproperty">. 
+00005d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005da0: 2020 203c 636f 6c6f 7220 7065 726d 6973     <color permis
+00005db0: 7369 6f6e 733d 2270 726f 702d 7265 7374  sions="prop-rest
+00005dc0: 7269 6374 6564 2220 636f 6d6d 656e 743d  ricted" comment=
+00005dd0: 2265 7861 6d70 6c65 223e 2330 3066 6636  "example">#00ff6
+00005de0: 363c 2f63 6f6c 6f72 3e0a 2020 2020 2020  6</color>.      
+00005df0: 2020 2020 2020 2020 2020 3c2f 636f 6c6f            </colo
+00005e00: 722d 7072 6f70 3e0a 2020 2020 2020 2020  r-prop>.        
+00005e10: 3e3e 3e20 6578 6365 6c32 786d 6c2e 6d61  >>> excel2xml.ma
+00005e20: 6b65 5f63 6f6c 6f72 5f70 726f 7028 223a  ke_color_prop(":
+00005e30: 7465 7374 7072 6f70 6572 7479 222c 205b  testproperty", [
+00005e40: 2223 3030 6666 3636 222c 2022 2330 3030  "#00ff66", "#000
+00005e50: 3030 3022 5d29 0a20 2020 2020 2020 2020  000"]).         
+00005e60: 2020 2020 2020 203c 636f 6c6f 722d 7072         <color-pr
+00005e70: 6f70 206e 616d 653d 223a 7465 7374 7072  op name=":testpr
+00005e80: 6f70 6572 7479 223e 0a20 2020 2020 2020  operty">.       
+00005e90: 2020 2020 2020 2020 2020 2020 203c 636f               <co
+00005ea0: 6c6f 7220 7065 726d 6973 7369 6f6e 733d  lor permissions=
+00005eb0: 2270 726f 702d 6465 6661 756c 7422 3e23  "prop-default">#
+00005ec0: 3030 6666 3636 3c2f 636f 6c6f 723e 0a20  00ff66</color>. 
+00005ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ee0: 2020 203c 636f 6c6f 7220 7065 726d 6973     <color permis
+00005ef0: 7369 6f6e 733d 2270 726f 702d 6465 6661  sions="prop-defa
+00005f00: 756c 7422 3e23 3030 3030 3030 3c2f 636f  ult">#000000</co
+00005f10: 6c6f 723e 0a20 2020 2020 2020 2020 2020  lor>.           
+00005f20: 2020 2020 203c 2f63 6f6c 6f72 2d70 726f       </color-pro
+00005f30: 703e 0a0a 2020 2020 5365 6520 6874 7470  p>..    See http
+00005f40: 733a 2f2f 646f 6373 2e64 6173 6368 2e73  s://docs.dasch.s
+00005f50: 7769 7373 2f6c 6174 6573 742f 4453 502d  wiss/latest/DSP-
+00005f60: 544f 4f4c 532f 6669 6c65 2d66 6f72 6d61  TOOLS/file-forma
+00005f70: 7473 2f78 6d6c 2d64 6174 612d 6669 6c65  ts/xml-data-file
+00005f80: 2f23 636f 6c6f 722d 7072 6f70 0a20 2020  /#color-prop.   
+00005f90: 2022 2222 0a0a 2020 2020 2320 6368 6563   """..    # chec
+00005fa0: 6b20 7468 6520 696e 7075 743a 2070 7265  k the input: pre
+00005fb0: 7061 7265 2061 206c 6973 7420 7769 7468  pare a list with
+00005fc0: 2076 616c 6964 2076 616c 7565 730a 2020   valid values.  
+00005fd0: 2020 7661 6c75 6573 203d 2070 7265 7061    values = prepa
+00005fe0: 7265 5f76 616c 7565 2876 616c 7565 290a  re_value(value).
+00005ff0: 0a20 2020 2023 2063 6865 636b 2076 616c  .    # check val
+00006000: 7565 2074 7970 650a 2020 2020 666f 7220  ue type.    for 
+00006010: 7661 6c20 696e 2076 616c 7565 733a 0a20  val in values:. 
+00006020: 2020 2020 2020 2069 6620 6e6f 7420 7265         if not re
+00006030: 6765 782e 7365 6172 6368 2872 225e 235b  gex.search(r"^#[
+00006040: 302d 3961 2d66 5d7b 367d 2422 2c20 7374  0-9a-f]{6}$", st
+00006050: 7228 7661 6c2e 7661 6c75 6529 2e73 7472  r(val.value).str
+00006060: 6970 2829 2c20 666c 6167 733d 7265 6765  ip(), flags=rege
+00006070: 782e 4947 4e4f 5245 4341 5345 293a 0a20  x.IGNORECASE):. 
+00006080: 2020 2020 2020 2020 2020 206d 7367 203d             msg =
+00006090: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+000060a0: 2020 2066 2246 6169 6c65 6420 7661 6c69     f"Failed vali
+000060b0: 6461 7469 6f6e 2069 6e20 7265 736f 7572  dation in resour
+000060c0: 6365 2027 7b63 616c 6c69 6e67 5f72 6573  ce '{calling_res
+000060d0: 6f75 7263 657d 272c 2070 726f 7065 7274  ource}', propert
+000060e0: 7920 277b 6e61 6d65 7d27 3a20 220a 2020  y '{name}': ".  
+000060f0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00006100: 277b 7661 6c2e 7661 6c75 657d 2720 6973  '{val.value}' is
+00006110: 206e 6f74 2061 2076 616c 6964 2063 6f6c   not a valid col
+00006120: 6f72 2e22 0a20 2020 2020 2020 2020 2020  or.".           
+00006130: 2029 0a20 2020 2020 2020 2020 2020 2077   ).            w
+00006140: 6172 6e69 6e67 732e 7761 726e 2844 7370  arnings.warn(Dsp
+00006150: 546f 6f6c 7355 7365 7257 6172 6e69 6e67  ToolsUserWarning
+00006160: 286d 7367 2929 0a0a 2020 2020 2320 6d61  (msg))..    # ma
+00006170: 6b65 2078 6d6c 2073 7472 7563 7475 7265  ke xml structure
+00006180: 206f 6620 7468 6520 7661 6c69 6420 7661   of the valid va
+00006190: 6c75 6573 0a20 2020 2070 726f 705f 203d  lues.    prop_ =
+000061a0: 2065 7472 6565 2e45 6c65 6d65 6e74 280a   etree.Element(.
+000061b0: 2020 2020 2020 2020 227b 2573 7d63 6f6c          "{%s}col
+000061c0: 6f72 2d70 726f 7022 2025 2078 6d6c 5f6e  or-prop" % xml_n
+000061d0: 616d 6573 7061 6365 5f6d 6170 5b4e 6f6e  amespace_map[Non
+000061e0: 655d 2c0a 2020 2020 2020 2020 6e61 6d65  e],.        name
+000061f0: 3d6e 616d 652c 0a20 2020 2020 2020 206e  =name,.        n
+00006200: 736d 6170 3d78 6d6c 5f6e 616d 6573 7061  smap=xml_namespa
+00006210: 6365 5f6d 6170 2c0a 2020 2020 290a 2020  ce_map,.    ).  
+00006220: 2020 666f 7220 7661 6c20 696e 2076 616c    for val in val
+00006230: 7565 733a 0a20 2020 2020 2020 206b 7761  ues:.        kwa
+00006240: 7267 7320 3d20 7b22 7065 726d 6973 7369  rgs = {"permissi
+00006250: 6f6e 7322 3a20 7661 6c2e 7065 726d 6973  ons": val.permis
+00006260: 7369 6f6e 737d 0a20 2020 2020 2020 2069  sions}.        i
+00006270: 6620 7661 6c2e 636f 6d6d 656e 7420 616e  f val.comment an
+00006280: 6420 6368 6563 6b5f 6e6f 746e 6128 7661  d check_notna(va
+00006290: 6c2e 636f 6d6d 656e 7429 3a0a 2020 2020  l.comment):.    
+000062a0: 2020 2020 2020 2020 6b77 6172 6773 5b22          kwargs["
+000062b0: 636f 6d6d 656e 7422 5d20 3d20 7661 6c2e  comment"] = val.
+000062c0: 636f 6d6d 656e 740a 2020 2020 2020 2020  comment.        
+000062d0: 7661 6c75 655f 203d 2065 7472 6565 2e45  value_ = etree.E
+000062e0: 6c65 6d65 6e74 280a 2020 2020 2020 2020  lement(.        
+000062f0: 2020 2020 227b 2573 7d63 6f6c 6f72 2220      "{%s}color" 
+00006300: 2520 786d 6c5f 6e61 6d65 7370 6163 655f  % xml_namespace_
+00006310: 6d61 705b 4e6f 6e65 5d2c 0a20 2020 2020  map[None],.     
+00006320: 2020 2020 2020 202a 2a6b 7761 7267 732c         **kwargs,
+00006330: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
+00006340: 5b61 7267 2d74 7970 655d 0a20 2020 2020  [arg-type].     
+00006350: 2020 2020 2020 206e 736d 6170 3d78 6d6c         nsmap=xml
+00006360: 5f6e 616d 6573 7061 6365 5f6d 6170 2c0a  _namespace_map,.
+00006370: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00006380: 2020 7661 6c75 655f 2e74 6578 7420 3d20    value_.text = 
+00006390: 7374 7228 7661 6c2e 7661 6c75 6529 2e73  str(val.value).s
+000063a0: 7472 6970 2829 0a20 2020 2020 2020 2070  trip().        p
+000063b0: 726f 705f 2e61 7070 656e 6428 7661 6c75  rop_.append(valu
+000063c0: 655f 290a 0a20 2020 2072 6574 7572 6e20  e_)..    return 
+000063d0: 7072 6f70 5f0a 0a0a 6465 6620 6d61 6b65  prop_...def make
+000063e0: 5f64 6174 655f 7072 6f70 280a 2020 2020  _date_prop(.    
+000063f0: 6e61 6d65 3a20 7374 722c 0a20 2020 2076  name: str,.    v
+00006400: 616c 7565 3a20 556e 696f 6e5b 5072 6f70  alue: Union[Prop
+00006410: 6572 7479 456c 656d 656e 742c 2073 7472  ertyElement, str
+00006420: 2c20 4974 6572 6162 6c65 5b55 6e69 6f6e  , Iterable[Union
+00006430: 5b50 726f 7065 7274 7945 6c65 6d65 6e74  [PropertyElement
+00006440: 2c20 7374 725d 5d5d 2c0a 2020 2020 6361  , str]]],.    ca
+00006450: 6c6c 696e 675f 7265 736f 7572 6365 3a20  lling_resource: 
+00006460: 7374 7220 3d20 2222 2c0a 2920 2d3e 2065  str = "",.) -> e
+00006470: 7472 6565 2e5f 456c 656d 656e 743a 0a20  tree._Element:. 
+00006480: 2020 2022 2222 0a20 2020 204d 616b 6520     """.    Make 
+00006490: 6120 3c64 6174 652d 7072 6f70 3e20 6672  a <date-prop> fr
+000064a0: 6f6d 206f 6e65 206f 7220 6d6f 7265 2064  om one or more d
+000064b0: 6174 6573 2f64 6174 6520 7261 6e67 6573  ates/date ranges
+000064c0: 2e20 5468 6520 6461 7465 2873 2920 6361  . The date(s) ca
+000064d0: 6e20 6265 2070 726f 7669 6465 6420 6173  n be provided as
+000064e0: 2073 7472 696e 6720 6f72 2061 7320 5072   string or as Pr
+000064f0: 6f70 6572 7479 456c 656d 656e 740a 2020  opertyElement.  
+00006500: 2020 7769 7468 2061 2073 7472 696e 6720    with a string 
+00006510: 696e 7369 6465 2e20 4966 2070 726f 7669  inside. If provi
+00006520: 6465 6420 6173 2073 7472 696e 672c 2074  ded as string, t
+00006530: 6865 2070 6572 6d69 7373 696f 6e73 2064  he permissions d
+00006540: 6566 6175 6c74 2074 6f20 2270 726f 702d  efault to "prop-
+00006550: 6465 6661 756c 7422 2e0a 0a20 2020 2041  default"...    A
+00006560: 7267 733a 0a20 2020 2020 2020 206e 616d  rgs:.        nam
+00006570: 653a 2074 6865 206e 616d 6520 6f66 2074  e: the name of t
+00006580: 6869 7320 7072 6f70 6572 7479 2061 7320  his property as 
+00006590: 6465 6669 6e65 6420 696e 2074 6865 206f  defined in the o
+000065a0: 6e74 6f0a 2020 2020 2020 2020 7661 6c75  nto.        valu
+000065b0: 653a 206f 6e65 206f 7220 6d6f 7265 2044  e: one or more D
+000065c0: 5350 2064 6174 6573 2c20 6173 2073 7472  SP dates, as str
+000065d0: 696e 672f 5072 6f70 6572 7479 456c 656d  ing/PropertyElem
+000065e0: 656e 742c 206f 7220 6173 2069 7465 7261  ent, or as itera
+000065f0: 626c 6520 6f66 2073 7472 696e 6773 2f50  ble of strings/P
+00006600: 726f 7065 7274 7945 6c65 6d65 6e74 730a  ropertyElements.
+00006610: 2020 2020 2020 2020 6361 6c6c 696e 675f          calling_
+00006620: 7265 736f 7572 6365 3a20 7468 6520 6e61  resource: the na
+00006630: 6d65 206f 6620 7468 6520 7061 7265 6e74  me of the parent
+00006640: 2072 6573 6f75 7263 6520 2866 6f72 2062   resource (for b
+00006650: 6574 7465 7220 6572 726f 7220 6d65 7373  etter error mess
+00006660: 6167 6573 290a 0a20 2020 2057 6172 6e73  ages)..    Warns
+00006670: 3a0a 2020 2020 2020 2020 4966 2074 6865  :.        If the
+00006680: 2076 616c 7565 2069 7320 6e6f 7420 6120   value is not a 
+00006690: 7661 6c69 6420 4453 5020 6461 7465 0a0a  valid DSP date..
+000066a0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+000066b0: 2020 2020 2061 6e20 6574 7265 652e 5f45       an etree._E
+000066c0: 6c65 6d65 6e74 2074 6861 7420 6361 6e20  lement that can 
+000066d0: 6265 2061 7070 656e 6465 6420 746f 2074  be appended to t
+000066e0: 6865 2070 6172 656e 7420 7265 736f 7572  he parent resour
+000066f0: 6365 2077 6974 6820 7265 736f 7572 6365  ce with resource
+00006700: 2e61 7070 656e 6428 6d61 6b65 5f2a 5f70  .append(make_*_p
+00006710: 726f 7028 2e2e 2e29 290a 0a20 2020 2045  rop(...))..    E
+00006720: 7861 6d70 6c65 733a 0a20 2020 2020 2020  xamples:.       
+00006730: 203e 3e3e 2065 7863 656c 3278 6d6c 2e6d   >>> excel2xml.m
+00006740: 616b 655f 6461 7465 5f70 726f 7028 223a  ake_date_prop(":
+00006750: 7465 7374 7072 6f70 6572 7479 222c 2022  testproperty", "
+00006760: 4752 4547 4f52 4941 4e3a 4345 3a32 3031  GREGORIAN:CE:201
+00006770: 342d 3031 2d33 3122 290a 2020 2020 2020  4-01-31").      
+00006780: 2020 2020 2020 2020 2020 3c64 6174 652d            <date-
+00006790: 7072 6f70 206e 616d 653d 223a 7465 7374  prop name=":test
+000067a0: 7072 6f70 6572 7479 223e 0a20 2020 2020  property">.     
+000067b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000067c0: 6461 7465 2070 6572 6d69 7373 696f 6e73  date permissions
+000067d0: 3d22 7072 6f70 2d64 6566 6175 6c74 223e  ="prop-default">
+000067e0: 4752 4547 4f52 4941 4e3a 4345 3a32 3031  GREGORIAN:CE:201
+000067f0: 342d 3031 2d33 313c 2f64 6174 653e 0a20  4-01-31</date>. 
+00006800: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00006810: 2f64 6174 652d 7072 6f70 3e0a 2020 2020  /date-prop>.    
+00006820: 2020 2020 3e3e 3e20 6578 6365 6c32 786d      >>> excel2xm
+00006830: 6c2e 6d61 6b65 5f64 6174 655f 7072 6f70  l.make_date_prop
+00006840: 2822 3a74 6573 7470 726f 7065 7274 7922  (":testproperty"
+00006850: 2c20 6578 6365 6c32 786d 6c2e 5072 6f70  , excel2xml.Prop
+00006860: 6572 7479 456c 656d 656e 7428 2247 5245  ertyElement("GRE
+00006870: 474f 5249 414e 3a43 453a 3230 3134 2d30  GORIAN:CE:2014-0
+00006880: 312d 3331 222c 2070 6572 6d69 7373 696f  1-31", permissio
+00006890: 6e73 3d22 7072 6f70 2d72 6573 7472 6963  ns="prop-restric
+000068a0: 7465 6422 2c20 636f 6d6d 656e 743d 2265  ted", comment="e
+000068b0: 7861 6d70 6c65 2229 290a 2020 2020 2020  xample")).      
+000068c0: 2020 2020 2020 2020 2020 3c64 6174 652d            <date-
+000068d0: 7072 6f70 206e 616d 653d 223a 7465 7374  prop name=":test
+000068e0: 7072 6f70 6572 7479 223e 0a20 2020 2020  property">.     
+000068f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00006900: 6461 7465 2070 6572 6d69 7373 696f 6e73  date permissions
+00006910: 3d22 7072 6f70 2d72 6573 7472 6963 7465  ="prop-restricte
+00006920: 6422 2063 6f6d 6d65 6e74 3d22 6578 616d  d" comment="exam
+00006930: 706c 6522 3e0a 2020 2020 2020 2020 2020  ple">.          
+00006940: 2020 2020 2020 2020 2020 2020 2020 4752                GR
+00006950: 4547 4f52 4941 4e3a 4345 3a32 3031 342d  EGORIAN:CE:2014-
+00006960: 3031 2d33 310a 2020 2020 2020 2020 2020  01-31.          
+00006970: 2020 2020 2020 2020 2020 3c2f 6461 7465            </date
+00006980: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00006990: 2020 3c2f 6461 7465 2d70 726f 703e 0a20    </date-prop>. 
+000069a0: 2020 2020 2020 203e 3e3e 2065 7863 656c         >>> excel
+000069b0: 3278 6d6c 2e6d 616b 655f 6461 7465 5f70  2xml.make_date_p
+000069c0: 726f 7028 223a 7465 7374 7072 6f70 6572  rop(":testproper
+000069d0: 7479 222c 205b 2247 5245 474f 5249 414e  ty", ["GREGORIAN
+000069e0: 3a43 453a 3139 3330 2d30 392d 3032 3a43  :CE:1930-09-02:C
+000069f0: 453a 3139 3330 2d30 392d 3033 222c 2022  E:1930-09-03", "
+00006a00: 4752 4547 4f52 4941 4e3a 4345 3a31 3933  GREGORIAN:CE:193
+00006a10: 302d 3039 2d30 323a 4345 3a31 3933 302d  0-09-02:CE:1930-
+00006a20: 3039 2d30 3322 5d29 0a20 2020 2020 2020  09-03"]).       
+00006a30: 2020 2020 2020 2020 203c 6461 7465 2d70           <date-p
+00006a40: 726f 7020 6e61 6d65 3d22 3a74 6573 7470  rop name=":testp
+00006a50: 726f 7065 7274 7922 3e0a 2020 2020 2020  roperty">.      
+00006a60: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00006a70: 6174 6520 7065 726d 6973 7369 6f6e 733d  ate permissions=
+00006a80: 2270 726f 702d 6465 6661 756c 7422 3e0a  "prop-default">.
 00006a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006aa0: 2020 2047 5245 474f 5249 414e 3a43 453a     GREGORIAN:CE:
-00006ab0: 3139 3330 2d30 392d 3032 3a43 453a 3139  1930-09-02:CE:19
-00006ac0: 3330 2d30 392d 3033 0a20 2020 2020 2020  30-09-03.       
-00006ad0: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-00006ae0: 6174 653e 0a20 2020 2020 2020 2020 2020  ate>.           
-00006af0: 2020 2020 2020 2020 203c 6461 7465 2070           <date p
-00006b00: 6572 6d69 7373 696f 6e73 3d22 7072 6f70  ermissions="prop
-00006b10: 2d64 6566 6175 6c74 223e 0a20 2020 2020  -default">.     
+00006aa0: 2020 2020 2020 2020 4752 4547 4f52 4941          GREGORIA
+00006ab0: 4e3a 4345 3a31 3933 302d 3039 2d30 323a  N:CE:1930-09-02:
+00006ac0: 4345 3a31 3933 302d 3039 2d30 330a 2020  CE:1930-09-03.  
+00006ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ae0: 2020 3c2f 6461 7465 3e0a 2020 2020 2020    </date>.      
+00006af0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00006b00: 6174 6520 7065 726d 6973 7369 6f6e 733d  ate permissions=
+00006b10: 2270 726f 702d 6465 6661 756c 7422 3e0a  "prop-default">.
 00006b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b30: 2020 2047 5245 474f 5249 414e 3a43 453a     GREGORIAN:CE:
-00006b40: 3139 3330 2d30 392d 3032 3a43 453a 3139  1930-09-02:CE:19
-00006b50: 3330 2d30 392d 3033 0a20 2020 2020 2020  30-09-03.       
-00006b60: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-00006b70: 6174 653e 0a20 2020 2020 2020 2020 2020  ate>.           
-00006b80: 2020 2020 203c 2f64 6174 652d 7072 6f70       </date-prop
-00006b90: 3e0a 0a20 2020 2053 6565 2068 7474 7073  >..    See https
-00006ba0: 3a2f 2f64 6f63 732e 6461 7363 682e 7377  ://docs.dasch.sw
-00006bb0: 6973 732f 6c61 7465 7374 2f44 5350 2d54  iss/latest/DSP-T
-00006bc0: 4f4f 4c53 2f66 696c 652d 666f 726d 6174  OOLS/file-format
-00006bd0: 732f 786d 6c2d 6461 7461 2d66 696c 652f  s/xml-data-file/
-00006be0: 2364 6174 652d 7072 6f70 0a20 2020 2022  #date-prop.    "
-00006bf0: 2222 0a0a 2020 2020 2320 6368 6563 6b20  ""..    # check 
-00006c00: 7468 6520 696e 7075 743a 2070 7265 7061  the input: prepa
-00006c10: 7265 2061 206c 6973 7420 7769 7468 2076  re a list with v
-00006c20: 616c 6964 2076 616c 7565 730a 2020 2020  alid values.    
-00006c30: 7661 6c75 6573 203d 2070 7265 7061 7265  values = prepare
-00006c40: 5f76 616c 7565 2876 616c 7565 290a 0a20  _value(value).. 
-00006c50: 2020 2023 2063 6865 636b 2076 616c 7565     # check value
-00006c60: 2074 7970 650a 2020 2020 666f 7220 7661   type.    for va
-00006c70: 6c20 696e 2076 616c 7565 733a 0a20 2020  l in values:.   
-00006c80: 2020 2020 2069 6620 6e6f 7420 6973 5f66       if not is_f
-00006c90: 756c 6c5f 6461 7465 2873 7472 2876 616c  ull_date(str(val
-00006ca0: 2e76 616c 7565 292e 7374 7269 7028 2929  .value).strip())
-00006cb0: 3a0a 2020 2020 2020 2020 2020 2020 6d73  :.            ms
-00006cc0: 6720 3d20 280a 2020 2020 2020 2020 2020  g = (.          
-00006cd0: 2020 2020 2020 6622 4661 696c 6564 2076        f"Failed v
-00006ce0: 616c 6964 6174 696f 6e20 696e 2072 6573  alidation in res
-00006cf0: 6f75 7263 6520 277b 6361 6c6c 696e 675f  ource '{calling_
-00006d00: 7265 736f 7572 6365 7d27 2c20 7072 6f70  resource}', prop
-00006d10: 6572 7479 2027 7b6e 616d 657d 273a 2022  erty '{name}': "
-00006d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006d30: 2066 2227 7b76 616c 2e76 616c 7565 7d27   f"'{val.value}'
-00006d40: 2069 7320 6e6f 7420 6120 7661 6c69 6420   is not a valid 
-00006d50: 4453 5020 6461 7465 2e22 0a20 2020 2020  DSP date.".     
-00006d60: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00006d70: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
-00006d80: 726e 2844 7370 546f 6f6c 7355 7365 7257  rn(DspToolsUserW
-00006d90: 6172 6e69 6e67 286d 7367 2929 0a0a 2020  arning(msg))..  
-00006da0: 2020 2320 6d61 6b65 2078 6d6c 2073 7472    # make xml str
-00006db0: 7563 7475 7265 206f 6620 7468 6520 7661  ucture of the va
-00006dc0: 6c69 6420 7661 6c75 6573 0a20 2020 2070  lid values.    p
-00006dd0: 726f 705f 203d 2065 7472 6565 2e45 6c65  rop_ = etree.Ele
-00006de0: 6d65 6e74 280a 2020 2020 2020 2020 227b  ment(.        "{
-00006df0: 2573 7d64 6174 652d 7072 6f70 2220 2520  %s}date-prop" % 
-00006e00: 786d 6c5f 6e61 6d65 7370 6163 655f 6d61  xml_namespace_ma
-00006e10: 705b 4e6f 6e65 5d2c 0a20 2020 2020 2020  p[None],.       
-00006e20: 206e 616d 653d 6e61 6d65 2c0a 2020 2020   name=name,.    
-00006e30: 2020 2020 6e73 6d61 703d 786d 6c5f 6e61      nsmap=xml_na
-00006e40: 6d65 7370 6163 655f 6d61 702c 0a20 2020  mespace_map,.   
-00006e50: 2029 0a20 2020 2066 6f72 2076 616c 2069   ).    for val i
-00006e60: 6e20 7661 6c75 6573 3a0a 2020 2020 2020  n values:.      
-00006e70: 2020 6b77 6172 6773 203d 207b 2270 6572    kwargs = {"per
-00006e80: 6d69 7373 696f 6e73 223a 2076 616c 2e70  missions": val.p
-00006e90: 6572 6d69 7373 696f 6e73 7d0a 2020 2020  ermissions}.    
-00006ea0: 2020 2020 6966 2076 616c 2e63 6f6d 6d65      if val.comme
-00006eb0: 6e74 2061 6e64 2063 6865 636b 5f6e 6f74  nt and check_not
-00006ec0: 6e61 2876 616c 2e63 6f6d 6d65 6e74 293a  na(val.comment):
-00006ed0: 0a20 2020 2020 2020 2020 2020 206b 7761  .            kwa
-00006ee0: 7267 735b 2263 6f6d 6d65 6e74 225d 203d  rgs["comment"] =
-00006ef0: 2076 616c 2e63 6f6d 6d65 6e74 0a20 2020   val.comment.   
-00006f00: 2020 2020 2076 616c 7565 5f20 3d20 6574       value_ = et
-00006f10: 7265 652e 456c 656d 656e 7428 0a20 2020  ree.Element(.   
-00006f20: 2020 2020 2020 2020 2022 7b25 737d 6461           "{%s}da
-00006f30: 7465 2220 2520 786d 6c5f 6e61 6d65 7370  te" % xml_namesp
-00006f40: 6163 655f 6d61 705b 4e6f 6e65 5d2c 0a20  ace_map[None],. 
-00006f50: 2020 2020 2020 2020 2020 202a 2a6b 7761             **kwa
-00006f60: 7267 732c 2020 2320 7479 7065 3a20 6967  rgs,  # type: ig
-00006f70: 6e6f 7265 5b61 7267 2d74 7970 655d 0a20  nore[arg-type]. 
-00006f80: 2020 2020 2020 2020 2020 206e 736d 6170             nsmap
-00006f90: 3d78 6d6c 5f6e 616d 6573 7061 6365 5f6d  =xml_namespace_m
-00006fa0: 6170 2c0a 2020 2020 2020 2020 290a 2020  ap,.        ).  
-00006fb0: 2020 2020 2020 7661 6c75 655f 2e74 6578        value_.tex
-00006fc0: 7420 3d20 7374 7228 7661 6c2e 7661 6c75  t = str(val.valu
-00006fd0: 6529 2e73 7472 6970 2829 0a20 2020 2020  e).strip().     
-00006fe0: 2020 2070 726f 705f 2e61 7070 656e 6428     prop_.append(
-00006ff0: 7661 6c75 655f 290a 0a20 2020 2072 6574  value_)..    ret
-00007000: 7572 6e20 7072 6f70 5f0a 0a0a 6465 6620  urn prop_...def 
-00007010: 6d61 6b65 5f64 6563 696d 616c 5f70 726f  make_decimal_pro
-00007020: 7028 0a20 2020 206e 616d 653a 2073 7472  p(.    name: str
-00007030: 2c0a 2020 2020 7661 6c75 653a 2055 6e69  ,.    value: Uni
-00007040: 6f6e 5b50 726f 7065 7274 7945 6c65 6d65  on[PropertyEleme
-00007050: 6e74 2c20 7374 722c 2049 7465 7261 626c  nt, str, Iterabl
-00007060: 655b 556e 696f 6e5b 5072 6f70 6572 7479  e[Union[Property
-00007070: 456c 656d 656e 742c 2073 7472 5d5d 5d2c  Element, str]]],
-00007080: 0a20 2020 2063 616c 6c69 6e67 5f72 6573  .    calling_res
-00007090: 6f75 7263 653a 2073 7472 203d 2022 222c  ource: str = "",
-000070a0: 0a29 202d 3e20 6574 7265 652e 5f45 6c65  .) -> etree._Ele
-000070b0: 6d65 6e74 3a0a 2020 2020 2222 220a 2020  ment:.    """.  
-000070c0: 2020 4d61 6b65 2061 203c 6465 6369 6d61    Make a <decima
-000070d0: 6c2d 7072 6f70 3e20 6672 6f6d 206f 6e65  l-prop> from one
-000070e0: 206f 7220 6d6f 7265 2064 6563 696d 616c   or more decimal
-000070f0: 206e 756d 6265 7273 2e20 5468 6520 6465   numbers. The de
-00007100: 6369 6d61 6c28 7329 2063 616e 2062 6520  cimal(s) can be 
-00007110: 7072 6f76 6964 6564 2061 7320 7374 7269  provided as stri
-00007120: 6e67 2c20 666c 6f61 742c 206f 7220 6173  ng, float, or as
-00007130: 0a20 2020 2050 726f 7065 7274 7945 6c65  .    PropertyEle
-00007140: 6d65 6e74 2077 6974 6820 6120 7374 7269  ment with a stri
-00007150: 6e67 2f66 6c6f 6174 2069 6e73 6964 652e  ng/float inside.
-00007160: 2049 6620 7072 6f76 6964 6564 2061 7320   If provided as 
-00007170: 7374 7269 6e67 2f66 6c6f 6174 2c20 7468  string/float, th
-00007180: 6520 7065 726d 6973 7369 6f6e 7320 6465  e permissions de
-00007190: 6661 756c 7420 746f 0a20 2020 2022 7072  fault to.    "pr
-000071a0: 6f70 2d64 6566 6175 6c74 222e 0a0a 2020  op-default"...  
-000071b0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-000071c0: 6e61 6d65 3a20 7468 6520 6e61 6d65 206f  name: the name o
-000071d0: 6620 7468 6973 2070 726f 7065 7274 7920  f this property 
-000071e0: 6173 2064 6566 696e 6564 2069 6e20 7468  as defined in th
-000071f0: 6520 6f6e 746f 0a20 2020 2020 2020 2076  e onto.        v
-00007200: 616c 7565 3a20 6f6e 6520 6f72 206d 6f72  alue: one or mor
-00007210: 6520 6465 6369 6d61 6c20 6e75 6d62 6572  e decimal number
-00007220: 732c 2061 7320 7374 7269 6e67 2f66 6c6f  s, as string/flo
-00007230: 6174 2f50 726f 7065 7274 7945 6c65 6d65  at/PropertyEleme
-00007240: 6e74 2c20 6f72 2061 7320 6974 6572 6162  nt, or as iterab
-00007250: 6c65 206f 6620 7374 7269 6e67 732f 5072  le of strings/Pr
-00007260: 6f70 6572 7479 456c 656d 656e 7473 0a20  opertyElements. 
-00007270: 2020 2020 2020 2063 616c 6c69 6e67 5f72         calling_r
-00007280: 6573 6f75 7263 653a 2074 6865 206e 616d  esource: the nam
-00007290: 6520 6f66 2074 6865 2070 6172 656e 7420  e of the parent 
-000072a0: 7265 736f 7572 6365 2028 666f 7220 6265  resource (for be
-000072b0: 7474 6572 2065 7272 6f72 206d 6573 7361  tter error messa
-000072c0: 6765 7329 0a0a 2020 2020 5761 726e 733a  ges)..    Warns:
-000072d0: 0a20 2020 2020 2020 2049 6620 7468 6520  .        If the 
-000072e0: 7661 6c75 6520 6973 206e 6f74 2061 2076  value is not a v
-000072f0: 616c 6964 2064 6563 696d 616c 206e 756d  alid decimal num
-00007300: 6265 720a 0a20 2020 2052 6574 7572 6e73  ber..    Returns
-00007310: 3a0a 2020 2020 2020 2020 616e 2065 7472  :.        an etr
-00007320: 6565 2e5f 456c 656d 656e 7420 7468 6174  ee._Element that
-00007330: 2063 616e 2062 6520 6170 7065 6e64 6564   can be appended
-00007340: 2074 6f20 7468 6520 7061 7265 6e74 2072   to the parent r
-00007350: 6573 6f75 7263 6520 7769 7468 2072 6573  esource with res
-00007360: 6f75 7263 652e 6170 7065 6e64 286d 616b  ource.append(mak
-00007370: 655f 2a5f 7072 6f70 282e 2e2e 2929 0a0a  e_*_prop(...))..
-00007380: 2020 2020 4578 616d 706c 6573 3a0a 2020      Examples:.  
-00007390: 2020 2020 2020 3e3e 3e20 6578 6365 6c32        >>> excel2
-000073a0: 786d 6c2e 6d61 6b65 5f64 6563 696d 616c  xml.make_decimal
-000073b0: 5f70 726f 7028 223a 7465 7374 7072 6f70  _prop(":testprop
-000073c0: 6572 7479 222c 2022 332e 3134 3135 3922  erty", "3.14159"
-000073d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000073e0: 2020 3c64 6563 696d 616c 2d70 726f 7020    <decimal-prop 
-000073f0: 6e61 6d65 3d22 3a74 6573 7470 726f 7065  name=":testprope
-00007400: 7274 7922 3e0a 2020 2020 2020 2020 2020  rty">.          
-00007410: 2020 2020 2020 2020 2020 3c64 6563 696d            <decim
-00007420: 616c 2070 6572 6d69 7373 696f 6e73 3d22  al permissions="
-00007430: 7072 6f70 2d64 6566 6175 6c74 223e 332e  prop-default">3.
-00007440: 3134 3135 393c 2f64 6563 696d 616c 3e0a  14159</decimal>.
-00007450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007460: 3c2f 6465 6369 6d61 6c2d 7072 6f70 3e0a  </decimal-prop>.
-00007470: 2020 2020 2020 2020 3e3e 3e20 6578 6365          >>> exce
-00007480: 6c32 786d 6c2e 6d61 6b65 5f64 6563 696d  l2xml.make_decim
-00007490: 616c 5f70 726f 7028 223a 7465 7374 7072  al_prop(":testpr
-000074a0: 6f70 6572 7479 222c 2065 7863 656c 3278  operty", excel2x
-000074b0: 6d6c 2e50 726f 7065 7274 7945 6c65 6d65  ml.PropertyEleme
-000074c0: 6e74 2822 332e 3134 3135 3922 2c20 7065  nt("3.14159", pe
-000074d0: 726d 6973 7369 6f6e 733d 2270 726f 702d  rmissions="prop-
-000074e0: 7265 7374 7269 6374 6564 222c 2063 6f6d  restricted", com
-000074f0: 6d65 6e74 3d22 6578 616d 706c 6522 2929  ment="example"))
-00007500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007510: 203c 6465 6369 6d61 6c2d 7072 6f70 206e   <decimal-prop n
-00007520: 616d 653d 223a 7465 7374 7072 6f70 6572  ame=":testproper
-00007530: 7479 223e 0a20 2020 2020 2020 2020 2020  ty">.           
-00007540: 2020 2020 2020 2020 203c 6465 6369 6d61           <decima
-00007550: 6c20 7065 726d 6973 7369 6f6e 733d 2270  l permissions="p
-00007560: 726f 702d 7265 7374 7269 6374 6564 2220  rop-restricted" 
-00007570: 636f 6d6d 656e 743d 2265 7861 6d70 6c65  comment="example
-00007580: 223e 332e 3134 3135 393c 2f64 6563 696d  ">3.14159</decim
-00007590: 616c 3e0a 2020 2020 2020 2020 2020 2020  al>.            
-000075a0: 2020 2020 3c2f 6465 6369 6d61 6c2d 7072      </decimal-pr
-000075b0: 6f70 3e0a 2020 2020 2020 2020 3e3e 3e20  op>.        >>> 
-000075c0: 6578 6365 6c32 786d 6c2e 6d61 6b65 5f64  excel2xml.make_d
-000075d0: 6563 696d 616c 5f70 726f 7028 223a 7465  ecimal_prop(":te
-000075e0: 7374 7072 6f70 6572 7479 222c 205b 2233  stproperty", ["3
-000075f0: 2e31 3431 3539 222c 2022 322e 3731 3822  .14159", "2.718"
-00007600: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-00007610: 2020 203c 6465 6369 6d61 6c2d 7072 6f70     <decimal-prop
-00007620: 206e 616d 653d 223a 7465 7374 7072 6f70   name=":testprop
-00007630: 6572 7479 223e 0a20 2020 2020 2020 2020  erty">.         
-00007640: 2020 2020 2020 2020 2020 203c 6465 6369             <deci
-00007650: 6d61 6c20 7065 726d 6973 7369 6f6e 733d  mal permissions=
-00007660: 2270 726f 702d 6465 6661 756c 7422 3e33  "prop-default">3
-00007670: 2e31 3431 3539 3c2f 6465 6369 6d61 6c3e  .14159</decimal>
-00007680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007690: 2020 2020 203c 6465 6369 6d61 6c20 7065       <decimal pe
-000076a0: 726d 6973 7369 6f6e 733d 2270 726f 702d  rmissions="prop-
-000076b0: 6465 6661 756c 7422 3e32 2e37 3138 3c2f  default">2.718</
-000076c0: 6465 6369 6d61 6c3e 0a20 2020 2020 2020  decimal>.       
-000076d0: 2020 2020 2020 2020 203c 2f64 6563 696d           </decim
-000076e0: 616c 2d70 726f 703e 0a0a 2020 2020 5365  al-prop>..    Se
-000076f0: 6520 6874 7470 733a 2f2f 646f 6373 2e64  e https://docs.d
-00007700: 6173 6368 2e73 7769 7373 2f6c 6174 6573  asch.swiss/lates
-00007710: 742f 4453 502d 544f 4f4c 532f 6669 6c65  t/DSP-TOOLS/file
-00007720: 2d66 6f72 6d61 7473 2f78 6d6c 2d64 6174  -formats/xml-dat
-00007730: 612d 6669 6c65 2f23 6465 6369 6d61 6c2d  a-file/#decimal-
-00007740: 7072 6f70 0a20 2020 2022 2222 0a0a 2020  prop.    """..  
-00007750: 2020 2320 6368 6563 6b20 7468 6520 696e    # check the in
-00007760: 7075 743a 2070 7265 7061 7265 2061 206c  put: prepare a l
-00007770: 6973 7420 7769 7468 2076 616c 6964 2076  ist with valid v
-00007780: 616c 7565 730a 2020 2020 7661 6c75 6573  alues.    values
-00007790: 203d 2070 7265 7061 7265 5f76 616c 7565   = prepare_value
-000077a0: 2876 616c 7565 290a 0a20 2020 2023 2063  (value)..    # c
-000077b0: 6865 636b 2076 616c 7565 2074 7970 650a  heck value type.
-000077c0: 2020 2020 666f 7220 7661 6c20 696e 2076      for val in v
-000077d0: 616c 7565 733a 0a20 2020 2020 2020 2074  alues:.        t
-000077e0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-000077f0: 666c 6f61 7428 7661 6c2e 7661 6c75 6529  float(val.value)
-00007800: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-00007810: 5661 6c75 6545 7272 6f72 3a0a 2020 2020  ValueError:.    
-00007820: 2020 2020 2020 2020 6d73 6720 3d20 280a          msg = (.
-00007830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007840: 6622 4661 696c 6564 2076 616c 6964 6174  f"Failed validat
-00007850: 696f 6e20 696e 2072 6573 6f75 7263 6520  ion in resource 
-00007860: 277b 6361 6c6c 696e 675f 7265 736f 7572  '{calling_resour
-00007870: 6365 7d27 2c20 7072 6f70 6572 7479 2027  ce}', property '
-00007880: 7b6e 616d 657d 273a 2022 0a20 2020 2020  {name}': ".     
-00007890: 2020 2020 2020 2020 2020 2066 2227 7b76             f"'{v
-000078a0: 616c 2e76 616c 7565 7d27 2069 7320 6e6f  al.value}' is no
-000078b0: 7420 6120 7661 6c69 6420 6465 6369 6d61  t a valid decima
-000078c0: 6c20 6e75 6d62 6572 2e22 0a20 2020 2020  l number.".     
-000078d0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000078e0: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
-000078f0: 726e 2844 7370 546f 6f6c 7355 7365 7257  rn(DspToolsUserW
-00007900: 6172 6e69 6e67 286d 7367 2929 0a0a 2020  arning(msg))..  
-00007910: 2020 2320 6d61 6b65 2078 6d6c 2073 7472    # make xml str
-00007920: 7563 7475 7265 206f 6620 7468 6520 7661  ucture of the va
-00007930: 6c69 6420 7661 6c75 6573 0a20 2020 2070  lid values.    p
-00007940: 726f 705f 203d 2065 7472 6565 2e45 6c65  rop_ = etree.Ele
-00007950: 6d65 6e74 280a 2020 2020 2020 2020 227b  ment(.        "{
-00007960: 2573 7d64 6563 696d 616c 2d70 726f 7022  %s}decimal-prop"
-00007970: 2025 2078 6d6c 5f6e 616d 6573 7061 6365   % xml_namespace
-00007980: 5f6d 6170 5b4e 6f6e 655d 2c0a 2020 2020  _map[None],.    
-00007990: 2020 2020 6e61 6d65 3d6e 616d 652c 0a20      name=name,. 
-000079a0: 2020 2020 2020 206e 736d 6170 3d78 6d6c         nsmap=xml
-000079b0: 5f6e 616d 6573 7061 6365 5f6d 6170 2c0a  _namespace_map,.
-000079c0: 2020 2020 290a 2020 2020 666f 7220 7661      ).    for va
-000079d0: 6c20 696e 2076 616c 7565 733a 0a20 2020  l in values:.   
-000079e0: 2020 2020 206b 7761 7267 7320 3d20 7b22       kwargs = {"
-000079f0: 7065 726d 6973 7369 6f6e 7322 3a20 7661  permissions": va
-00007a00: 6c2e 7065 726d 6973 7369 6f6e 737d 0a20  l.permissions}. 
-00007a10: 2020 2020 2020 2069 6620 7661 6c2e 636f         if val.co
-00007a20: 6d6d 656e 7420 616e 6420 6368 6563 6b5f  mment and check_
-00007a30: 6e6f 746e 6128 7661 6c2e 636f 6d6d 656e  notna(val.commen
-00007a40: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-00007a50: 6b77 6172 6773 5b22 636f 6d6d 656e 7422  kwargs["comment"
-00007a60: 5d20 3d20 7661 6c2e 636f 6d6d 656e 740a  ] = val.comment.
-00007a70: 2020 2020 2020 2020 7661 6c75 655f 203d          value_ =
-00007a80: 2065 7472 6565 2e45 6c65 6d65 6e74 280a   etree.Element(.
-00007a90: 2020 2020 2020 2020 2020 2020 227b 2573              "{%s
-00007aa0: 7d64 6563 696d 616c 2220 2520 786d 6c5f  }decimal" % xml_
-00007ab0: 6e61 6d65 7370 6163 655f 6d61 705b 4e6f  namespace_map[No
-00007ac0: 6e65 5d2c 0a20 2020 2020 2020 2020 2020  ne],.           
-00007ad0: 202a 2a6b 7761 7267 732c 2020 2320 7479   **kwargs,  # ty
-00007ae0: 7065 3a20 6967 6e6f 7265 5b61 7267 2d74  pe: ignore[arg-t
-00007af0: 7970 655d 0a20 2020 2020 2020 2020 2020  ype].           
-00007b00: 206e 736d 6170 3d78 6d6c 5f6e 616d 6573   nsmap=xml_names
-00007b10: 7061 6365 5f6d 6170 2c0a 2020 2020 2020  pace_map,.      
-00007b20: 2020 290a 2020 2020 2020 2020 7661 6c75    ).        valu
-00007b30: 655f 2e74 6578 7420 3d20 7374 7228 7661  e_.text = str(va
-00007b40: 6c2e 7661 6c75 6529 0a20 2020 2020 2020  l.value).       
-00007b50: 2070 726f 705f 2e61 7070 656e 6428 7661   prop_.append(va
-00007b60: 6c75 655f 290a 0a20 2020 2072 6574 7572  lue_)..    retur
-00007b70: 6e20 7072 6f70 5f0a 0a0a 6465 6620 6d61  n prop_...def ma
-00007b80: 6b65 5f67 656f 6d65 7472 795f 7072 6f70  ke_geometry_prop
-00007b90: 280a 2020 2020 6e61 6d65 3a20 7374 722c  (.    name: str,
-00007ba0: 0a20 2020 2076 616c 7565 3a20 556e 696f  .    value: Unio
-00007bb0: 6e5b 5072 6f70 6572 7479 456c 656d 656e  n[PropertyElemen
-00007bc0: 742c 2073 7472 2c20 4974 6572 6162 6c65  t, str, Iterable
-00007bd0: 5b55 6e69 6f6e 5b50 726f 7065 7274 7945  [Union[PropertyE
-00007be0: 6c65 6d65 6e74 2c20 7374 725d 5d5d 2c0a  lement, str]]],.
-00007bf0: 2020 2020 6361 6c6c 696e 675f 7265 736f      calling_reso
-00007c00: 7572 6365 3a20 7374 7220 3d20 2222 2c0a  urce: str = "",.
-00007c10: 2920 2d3e 2065 7472 6565 2e5f 456c 656d  ) -> etree._Elem
-00007c20: 656e 743a 0a20 2020 2022 2222 0a20 2020  ent:.    """.   
-00007c30: 204d 616b 6520 6120 3c67 656f 6d65 7472   Make a <geometr
-00007c40: 792d 7072 6f70 3e20 6672 6f6d 206f 6e65  y-prop> from one
-00007c50: 206f 7220 6d6f 7265 2061 7265 6173 206f   or more areas o
-00007c60: 6620 616e 2069 6d61 6765 2e20 5468 6520  f an image. The 
-00007c70: 6172 6561 2873 2920 6361 6e20 6265 2070  area(s) can be p
-00007c80: 726f 7669 6465 6420 6173 204a 534f 4e2d  rovided as JSON-
-00007c90: 7374 7269 6e67 206f 7220 6173 0a20 2020  string or as.   
-00007ca0: 2050 726f 7065 7274 7945 6c65 6d65 6e74   PropertyElement
-00007cb0: 2077 6974 6820 7468 6520 4a53 4f4e 2d73   with the JSON-s
-00007cc0: 7472 696e 6720 696e 7369 6465 2e20 4966  tring inside. If
-00007cd0: 2070 726f 7669 6465 6420 6173 2073 7472   provided as str
-00007ce0: 696e 672c 2074 6865 2070 6572 6d69 7373  ing, the permiss
-00007cf0: 696f 6e73 2064 6566 6175 6c74 2074 6f20  ions default to 
-00007d00: 2270 726f 702d 6465 6661 756c 7422 2e0a  "prop-default"..
-00007d10: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-00007d20: 2020 206e 616d 653a 2074 6865 206e 616d     name: the nam
-00007d30: 6520 6f66 2074 6869 7320 7072 6f70 6572  e of this proper
-00007d40: 7479 2061 7320 6465 6669 6e65 6420 696e  ty as defined in
-00007d50: 2074 6865 206f 6e74 6f0a 2020 2020 2020   the onto.      
-00007d60: 2020 7661 6c75 653a 206f 6e65 206f 7220    value: one or 
-00007d70: 6d6f 7265 204a 534f 4e20 6765 6f6d 6574  more JSON geomet
-00007d80: 7279 206f 626a 6563 7473 2c20 6173 2073  ry objects, as s
-00007d90: 7472 696e 672f 5072 6f70 6572 7479 456c  tring/PropertyEl
-00007da0: 656d 656e 742c 206f 7220 6173 2069 7465  ement, or as ite
-00007db0: 7261 626c 6520 6f66 2073 7472 696e 6773  rable of strings
-00007dc0: 2f50 726f 7065 7274 7945 6c65 6d65 6e74  /PropertyElement
-00007dd0: 730a 2020 2020 2020 2020 6361 6c6c 696e  s.        callin
-00007de0: 675f 7265 736f 7572 6365 3a20 7468 6520  g_resource: the 
-00007df0: 6e61 6d65 206f 6620 7468 6520 7061 7265  name of the pare
-00007e00: 6e74 2072 6573 6f75 7263 6520 2866 6f72  nt resource (for
-00007e10: 2062 6574 7465 7220 6572 726f 7220 6d65   better error me
-00007e20: 7373 6167 6573 290a 0a20 2020 2057 6172  ssages)..    War
-00007e30: 6e73 3a0a 2020 2020 2020 2020 4966 2074  ns:.        If t
-00007e40: 6865 2076 616c 7565 2069 7320 6e6f 7420  he value is not 
-00007e50: 6120 7661 6c69 6420 4a53 4f4e 2067 656f  a valid JSON geo
-00007e60: 6d65 7472 7920 6f62 6a65 6374 0a0a 2020  metry object..  
-00007e70: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00007e80: 2020 2061 6e20 6574 7265 652e 5f45 6c65     an etree._Ele
-00007e90: 6d65 6e74 2074 6861 7420 6361 6e20 6265  ment that can be
-00007ea0: 2061 7070 656e 6465 6420 746f 2074 6865   appended to the
-00007eb0: 2070 6172 656e 7420 7265 736f 7572 6365   parent resource
-00007ec0: 2077 6974 6820 7265 736f 7572 6365 2e61   with resource.a
-00007ed0: 7070 656e 6428 6d61 6b65 5f2a 5f70 726f  ppend(make_*_pro
-00007ee0: 7028 2e2e 2e29 290a 0a20 2020 2045 7861  p(...))..    Exa
-00007ef0: 6d70 6c65 733a 0a20 2020 2020 2020 203e  mples:.        >
-00007f00: 3e3e 2065 7863 656c 3278 6d6c 2e6d 616b  >> excel2xml.mak
-00007f10: 655f 6765 6f6d 6574 7279 5f70 726f 7028  e_geometry_prop(
-00007f20: 223a 7465 7374 7072 6f70 6572 7479 222c  ":testproperty",
-00007f30: 206a 736f 6e5f 7374 7269 6e67 290a 2020   json_string).  
-00007f40: 2020 2020 2020 2020 2020 2020 2020 3c67                <g
-00007f50: 656f 6d65 7472 792d 7072 6f70 206e 616d  eometry-prop nam
-00007f60: 653d 223a 7465 7374 7072 6f70 6572 7479  e=":testproperty
-00007f70: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00007f80: 2020 2020 2020 203c 6765 6f6d 6574 7279         <geometry
-00007f90: 2070 6572 6d69 7373 696f 6e73 3d22 7072   permissions="pr
-00007fa0: 6f70 2d64 6566 6175 6c74 223e 7b4a 534f  op-default">{JSO
-00007fb0: 4e7d 3c2f 6765 6f6d 6574 7279 3e0a 2020  N}</geometry>.  
-00007fc0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00007fd0: 6765 6f6d 6574 7279 2d70 726f 703e 0a20  geometry-prop>. 
-00007fe0: 2020 2020 2020 203e 3e3e 2065 7863 656c         >>> excel
-00007ff0: 3278 6d6c 2e6d 616b 655f 6765 6f6d 6574  2xml.make_geomet
-00008000: 7279 5f70 726f 7028 223a 7465 7374 7072  ry_prop(":testpr
-00008010: 6f70 6572 7479 222c 2065 7863 656c 3278  operty", excel2x
-00008020: 6d6c 2e50 726f 7065 7274 7945 6c65 6d65  ml.PropertyEleme
-00008030: 6e74 286a 736f 6e5f 7374 7269 6e67 2c20  nt(json_string, 
-00008040: 7065 726d 6973 7369 6f6e 733d 2270 726f  permissions="pro
-00008050: 702d 7265 7374 7269 6374 6564 222c 2063  p-restricted", c
-00008060: 6f6d 6d65 6e74 3d22 6578 616d 706c 6522  omment="example"
-00008070: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00008080: 2020 203c 6765 6f6d 6574 7279 2d70 726f     <geometry-pro
-00008090: 7020 6e61 6d65 3d22 3a74 6573 7470 726f  p name=":testpro
-000080a0: 7065 7274 7922 3e0a 2020 2020 2020 2020  perty">.        
-000080b0: 2020 2020 2020 2020 2020 2020 3c67 656f              <geo
-000080c0: 6d65 7472 7920 7065 726d 6973 7369 6f6e  metry permission
-000080d0: 733d 2270 726f 702d 7265 7374 7269 6374  s="prop-restrict
-000080e0: 6564 2220 636f 6d6d 656e 743d 2265 7861  ed" comment="exa
-000080f0: 6d70 6c65 223e 7b4a 534f 4e7d 3c2f 6765  mple">{JSON}</ge
-00008100: 6f6d 6574 7279 3e0a 2020 2020 2020 2020  ometry>.        
-00008110: 2020 2020 2020 2020 3c2f 6765 6f6d 6574          </geomet
-00008120: 7279 2d70 726f 703e 0a20 2020 2020 2020  ry-prop>.       
-00008130: 203e 3e3e 2065 7863 656c 3278 6d6c 2e6d   >>> excel2xml.m
-00008140: 616b 655f 6765 6f6d 6574 7279 5f70 726f  ake_geometry_pro
-00008150: 7028 223a 7465 7374 7072 6f70 6572 7479  p(":testproperty
-00008160: 222c 205b 6a73 6f6e 5f73 7472 696e 6731  ", [json_string1
-00008170: 2c20 6a73 6f6e 5f73 7472 696e 6732 5d29  , json_string2])
-00008180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008190: 203c 6765 6f6d 6574 7279 2d70 726f 7020   <geometry-prop 
-000081a0: 6e61 6d65 3d22 3a74 6573 7470 726f 7065  name=":testprope
-000081b0: 7274 7922 3e0a 2020 2020 2020 2020 2020  rty">.          
-000081c0: 2020 2020 2020 2020 2020 3c67 656f 6d65            <geome
-000081d0: 7472 7920 7065 726d 6973 7369 6f6e 733d  try permissions=
-000081e0: 2270 726f 702d 6465 6661 756c 7422 3e7b  "prop-default">{
-000081f0: 4a53 4f4e 7d3c 2f67 656f 6d65 7472 793e  JSON}</geometry>
-00008200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008210: 2020 2020 203c 6765 6f6d 6574 7279 2070       <geometry p
-00008220: 6572 6d69 7373 696f 6e73 3d22 7072 6f70  ermissions="prop
-00008230: 2d64 6566 6175 6c74 223e 7b4a 534f 4e7d  -default">{JSON}
-00008240: 3c2f 6765 6f6d 6574 7279 3e0a 2020 2020  </geometry>.    
-00008250: 2020 2020 2020 2020 2020 2020 3c2f 6765              </ge
-00008260: 6f6d 6574 7279 2d70 726f 703e 0a0a 2020  ometry-prop>..  
-00008270: 2020 5365 6520 6874 7470 733a 2f2f 646f    See https://do
-00008280: 6373 2e64 6173 6368 2e73 7769 7373 2f6c  cs.dasch.swiss/l
-00008290: 6174 6573 742f 4453 502d 544f 4f4c 532f  atest/DSP-TOOLS/
-000082a0: 6669 6c65 2d66 6f72 6d61 7473 2f78 6d6c  file-formats/xml
-000082b0: 2d64 6174 612d 6669 6c65 2f23 6765 6f6d  -data-file/#geom
-000082c0: 6574 7279 2d70 726f 700a 2020 2020 2222  etry-prop.    ""
-000082d0: 220a 0a20 2020 2023 2063 6865 636b 2074  "..    # check t
-000082e0: 6865 2069 6e70 7574 3a20 7072 6570 6172  he input: prepar
-000082f0: 6520 6120 6c69 7374 2077 6974 6820 7661  e a list with va
-00008300: 6c69 6420 7661 6c75 6573 0a20 2020 2076  lid values.    v
-00008310: 616c 7565 7320 3d20 7072 6570 6172 655f  alues = prepare_
-00008320: 7661 6c75 6528 7661 6c75 6529 0a0a 2020  value(value)..  
-00008330: 2020 2320 6368 6563 6b20 7661 6c75 6520    # check value 
-00008340: 7479 7065 0a20 2020 2066 6f72 2076 616c  type.    for val
-00008350: 2069 6e20 7661 6c75 6573 3a0a 2020 2020   in values:.    
-00008360: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00008370: 2020 2020 2076 616c 7565 5f61 735f 6469       value_as_di
-00008380: 6374 203d 206a 736f 6e2e 6c6f 6164 7328  ct = json.loads(
-00008390: 7374 7228 7661 6c2e 7661 6c75 6529 290a  str(val.value)).
-000083a0: 2020 2020 2020 2020 2020 2020 6966 2076              if v
-000083b0: 616c 7565 5f61 735f 6469 6374 5b22 7479  alue_as_dict["ty
-000083c0: 7065 225d 206e 6f74 2069 6e20 5b22 7265  pe"] not in ["re
-000083d0: 6374 616e 676c 6522 2c20 2263 6972 636c  ctangle", "circl
-000083e0: 6522 2c20 2270 6f6c 7967 6f6e 225d 3a0a  e", "polygon"]:.
-000083f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008400: 6d73 6720 3d20 280a 2020 2020 2020 2020  msg = (.        
-00008410: 2020 2020 2020 2020 2020 2020 6622 4661              f"Fa
-00008420: 696c 6564 2076 616c 6964 6174 696f 6e20  iled validation 
-00008430: 696e 2072 6573 6f75 7263 6520 277b 6361  in resource '{ca
-00008440: 6c6c 696e 675f 7265 736f 7572 6365 7d27  lling_resource}'
-00008450: 2c20 7072 6f70 6572 7479 2027 7b6e 616d  , property '{nam
-00008460: 657d 273a 2022 0a20 2020 2020 2020 2020  e}': ".         
-00008470: 2020 2020 2020 2020 2020 2066 2254 6865             f"The
-00008480: 2027 7479 7065 2720 6f66 2074 6865 204a   'type' of the J
-00008490: 534f 4e20 6765 6f6d 6574 7279 206f 626a  SON geometry obj
-000084a0: 6563 7420 6d75 7374 2062 6520 2772 6563  ect must be 'rec
-000084b0: 7461 6e67 6c65 272c 2027 6369 7263 6c65  tangle', 'circle
-000084c0: 272c 206f 7220 2770 6f6c 7967 6f6e 272e  ', or 'polygon'.
-000084d0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000084e0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-000084f0: 2020 2020 7761 726e 696e 6773 2e77 6172      warnings.war
-00008500: 6e28 4473 7054 6f6f 6c73 5573 6572 5761  n(DspToolsUserWa
-00008510: 726e 696e 6728 6d73 6729 290a 2020 2020  rning(msg)).    
-00008520: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-00008530: 7369 6e73 7461 6e63 6528 7661 6c75 655f  sinstance(value_
-00008540: 6173 5f64 6963 745b 2270 6f69 6e74 7322  as_dict["points"
-00008550: 5d2c 206c 6973 7429 3a0a 2020 2020 2020  ], list):.      
-00008560: 2020 2020 2020 2020 2020 6d73 6720 3d20            msg = 
-00008570: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00008580: 2020 2020 2020 6622 4661 696c 6564 2076        f"Failed v
-00008590: 616c 6964 6174 696f 6e20 696e 2072 6573  alidation in res
-000085a0: 6f75 7263 6520 277b 6361 6c6c 696e 675f  ource '{calling_
-000085b0: 7265 736f 7572 6365 7d27 2c20 7072 6f70  resource}', prop
-000085c0: 6572 7479 2027 7b6e 616d 657d 273a 2022  erty '{name}': "
-000085d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000085e0: 2020 2020 2066 2254 6865 2027 706f 696e       f"The 'poin
-000085f0: 7473 276f 6620 7468 6520 4a53 4f4e 2067  ts'of the JSON g
-00008600: 656f 6d65 7472 7920 6f62 6a65 6374 206d  eometry object m
-00008610: 7573 7420 6265 2061 206c 6973 7420 6f66  ust be a list of
-00008620: 2070 6f69 6e74 732e 220a 2020 2020 2020   points.".      
-00008630: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00008640: 2020 2020 2020 2020 2020 2020 7761 726e              warn
-00008650: 696e 6773 2e77 6172 6e28 4473 7054 6f6f  ings.warn(DspToo
-00008660: 6c73 5573 6572 5761 726e 696e 6728 6d73  lsUserWarning(ms
-00008670: 6729 290a 2020 2020 2020 2020 6578 6365  g)).        exce
-00008680: 7074 2028 6a73 6f6e 2e4a 534f 4e44 6563  pt (json.JSONDec
-00008690: 6f64 6545 7272 6f72 2c20 5479 7065 4572  odeError, TypeEr
-000086a0: 726f 722c 2049 6e64 6578 4572 726f 722c  ror, IndexError,
-000086b0: 204b 6579 4572 726f 722c 2041 7373 6572   KeyError, Asser
-000086c0: 7469 6f6e 4572 726f 7229 3a0a 2020 2020  tionError):.    
-000086d0: 2020 2020 2020 2020 6d73 6720 3d20 280a          msg = (.
-000086e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086f0: 6622 4661 696c 6564 2076 616c 6964 6174  f"Failed validat
-00008700: 696f 6e20 696e 2072 6573 6f75 7263 6520  ion in resource 
-00008710: 277b 6361 6c6c 696e 675f 7265 736f 7572  '{calling_resour
-00008720: 6365 7d27 2c20 7072 6f70 6572 7479 2027  ce}', property '
-00008730: 7b6e 616d 657d 273a 2022 0a20 2020 2020  {name}': ".     
-00008740: 2020 2020 2020 2020 2020 2066 2227 7b76             f"'{v
-00008750: 616c 2e76 616c 7565 7d27 2069 7320 6e6f  al.value}' is no
-00008760: 7420 6120 7661 6c69 6420 4a53 4f4e 2067  t a valid JSON g
-00008770: 656f 6d65 7472 7920 6f62 6a65 6374 2e22  eometry object."
-00008780: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00008790: 2020 2020 2020 2020 2020 2077 6172 6e69             warni
-000087a0: 6e67 732e 7761 726e 2844 7370 546f 6f6c  ngs.warn(DspTool
-000087b0: 7355 7365 7257 6172 6e69 6e67 286d 7367  sUserWarning(msg
-000087c0: 2929 0a0a 2020 2020 2320 6d61 6b65 2078  ))..    # make x
-000087d0: 6d6c 2073 7472 7563 7475 7265 206f 6620  ml structure of 
-000087e0: 7468 6520 7661 6c69 6420 7661 6c75 6573  the valid values
-000087f0: 0a20 2020 2070 726f 705f 203d 2065 7472  .    prop_ = etr
-00008800: 6565 2e45 6c65 6d65 6e74 280a 2020 2020  ee.Element(.    
-00008810: 2020 2020 227b 2573 7d67 656f 6d65 7472      "{%s}geometr
-00008820: 792d 7072 6f70 2220 2520 786d 6c5f 6e61  y-prop" % xml_na
-00008830: 6d65 7370 6163 655f 6d61 705b 4e6f 6e65  mespace_map[None
-00008840: 5d2c 0a20 2020 2020 2020 206e 616d 653d  ],.        name=
-00008850: 6e61 6d65 2c0a 2020 2020 2020 2020 6e73  name,.        ns
-00008860: 6d61 703d 786d 6c5f 6e61 6d65 7370 6163  map=xml_namespac
-00008870: 655f 6d61 702c 0a20 2020 2029 0a20 2020  e_map,.    ).   
-00008880: 2066 6f72 2076 616c 2069 6e20 7661 6c75   for val in valu
-00008890: 6573 3a0a 2020 2020 2020 2020 6b77 6172  es:.        kwar
-000088a0: 6773 203d 207b 2270 6572 6d69 7373 696f  gs = {"permissio
-000088b0: 6e73 223a 2076 616c 2e70 6572 6d69 7373  ns": val.permiss
-000088c0: 696f 6e73 7d0a 2020 2020 2020 2020 6966  ions}.        if
-000088d0: 2076 616c 2e63 6f6d 6d65 6e74 2061 6e64   val.comment and
-000088e0: 2063 6865 636b 5f6e 6f74 6e61 2876 616c   check_notna(val
-000088f0: 2e63 6f6d 6d65 6e74 293a 0a20 2020 2020  .comment):.     
-00008900: 2020 2020 2020 206b 7761 7267 735b 2263         kwargs["c
-00008910: 6f6d 6d65 6e74 225d 203d 2076 616c 2e63  omment"] = val.c
-00008920: 6f6d 6d65 6e74 0a20 2020 2020 2020 2076  omment.        v
-00008930: 616c 7565 5f20 3d20 6574 7265 652e 456c  alue_ = etree.El
-00008940: 656d 656e 7428 0a20 2020 2020 2020 2020  ement(.         
-00008950: 2020 2022 7b25 737d 6765 6f6d 6574 7279     "{%s}geometry
-00008960: 2220 2520 786d 6c5f 6e61 6d65 7370 6163  " % xml_namespac
-00008970: 655f 6d61 705b 4e6f 6e65 5d2c 0a20 2020  e_map[None],.   
-00008980: 2020 2020 2020 2020 202a 2a6b 7761 7267           **kwarg
-00008990: 732c 2020 2320 7479 7065 3a20 6967 6e6f  s,  # type: igno
-000089a0: 7265 5b61 7267 2d74 7970 655d 0a20 2020  re[arg-type].   
-000089b0: 2020 2020 2020 2020 206e 736d 6170 3d78           nsmap=x
-000089c0: 6d6c 5f6e 616d 6573 7061 6365 5f6d 6170  ml_namespace_map
-000089d0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-000089e0: 2020 2020 7661 6c75 655f 2e74 6578 7420      value_.text 
-000089f0: 3d20 7374 7228 7661 6c2e 7661 6c75 6529  = str(val.value)
-00008a00: 0a20 2020 2020 2020 2070 726f 705f 2e61  .        prop_.a
-00008a10: 7070 656e 6428 7661 6c75 655f 290a 2020  ppend(value_).  
-00008a20: 2020 7265 7475 726e 2070 726f 705f 0a0a    return prop_..
-00008a30: 0a64 6566 206d 616b 655f 6765 6f6e 616d  .def make_geonam
-00008a40: 655f 7072 6f70 280a 2020 2020 6e61 6d65  e_prop(.    name
-00008a50: 3a20 7374 722c 0a20 2020 2076 616c 7565  : str,.    value
-00008a60: 3a20 556e 696f 6e5b 5072 6f70 6572 7479  : Union[Property
-00008a70: 456c 656d 656e 742c 2073 7472 2c20 696e  Element, str, in
-00008a80: 742c 2049 7465 7261 626c 655b 556e 696f  t, Iterable[Unio
-00008a90: 6e5b 5072 6f70 6572 7479 456c 656d 656e  n[PropertyElemen
-00008aa0: 742c 2073 7472 2c20 696e 745d 5d5d 2c0a  t, str, int]]],.
-00008ab0: 2020 2020 6361 6c6c 696e 675f 7265 736f      calling_reso
-00008ac0: 7572 6365 3a20 7374 7220 3d20 2222 2c0a  urce: str = "",.
-00008ad0: 2920 2d3e 2065 7472 6565 2e5f 456c 656d  ) -> etree._Elem
-00008ae0: 656e 743a 0a20 2020 2022 2222 0a20 2020  ent:.    """.   
-00008af0: 204d 616b 6520 6120 3c67 656f 6e61 6d65   Make a <geoname
-00008b00: 2d70 726f 703e 2066 726f 6d20 6f6e 6520  -prop> from one 
-00008b10: 6f72 206d 6f72 6520 6765 6f6e 616d 6573  or more geonames
-00008b20: 2e6f 7267 2049 4473 2e20 5468 6520 4944  .org IDs. The ID
-00008b30: 2873 2920 6361 6e20 6265 2070 726f 7669  (s) can be provi
-00008b40: 6465 6420 6173 2073 7472 696e 672c 2069  ded as string, i
-00008b50: 6e74 6567 6572 2c20 6f72 2061 730a 2020  nteger, or as.  
-00008b60: 2020 5072 6f70 6572 7479 456c 656d 656e    PropertyElemen
-00008b70: 7420 7769 7468 2061 2073 7472 696e 672f  t with a string/
-00008b80: 696e 7465 6765 7220 696e 7369 6465 2e20  integer inside. 
-00008b90: 4966 2070 726f 7669 6465 6420 6173 2073  If provided as s
-00008ba0: 7472 696e 672f 696e 7465 6765 722c 2074  tring/integer, t
-00008bb0: 6865 2070 6572 6d69 7373 696f 6e73 2064  he permissions d
-00008bc0: 6566 6175 6c74 2074 6f0a 2020 2020 2270  efault to.    "p
-00008bd0: 726f 702d 6465 6661 756c 7422 2e0a 0a20  rop-default"... 
-00008be0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00008bf0: 206e 616d 653a 2074 6865 206e 616d 6520   name: the name 
-00008c00: 6f66 2074 6869 7320 7072 6f70 6572 7479  of this property
-00008c10: 2061 7320 6465 6669 6e65 6420 696e 2074   as defined in t
-00008c20: 6865 206f 6e74 6f0a 2020 2020 2020 2020  he onto.        
-00008c30: 7661 6c75 653a 206f 6e65 206f 7220 6d6f  value: one or mo
-00008c40: 7265 2067 656f 6e61 6d65 732e 6f72 6720  re geonames.org 
-00008c50: 4944 732c 2061 7320 7374 722f 696e 742f  IDs, as str/int/
-00008c60: 5072 6f70 6572 7479 456c 656d 656e 742c  PropertyElement,
-00008c70: 206f 7220 6173 2069 7465 7261 626c 6520   or as iterable 
-00008c80: 6f66 2073 7472 2f69 6e74 2f50 726f 7065  of str/int/Prope
-00008c90: 7274 7945 6c65 6d65 6e74 0a20 2020 2020  rtyElement.     
-00008ca0: 2020 2063 616c 6c69 6e67 5f72 6573 6f75     calling_resou
-00008cb0: 7263 653a 2074 6865 206e 616d 6520 6f66  rce: the name of
-00008cc0: 2074 6865 2070 6172 656e 7420 7265 736f   the parent reso
-00008cd0: 7572 6365 2028 666f 7220 6265 7474 6572  urce (for better
-00008ce0: 2065 7272 6f72 206d 6573 7361 6765 7329   error messages)
-00008cf0: 0a0a 2020 2020 5761 726e 733a 0a20 2020  ..    Warns:.   
-00008d00: 2020 2020 2049 6620 7468 6520 7661 6c75       If the valu
-00008d10: 6520 6973 206e 6f74 2061 2076 616c 6964  e is not a valid
-00008d20: 2067 656f 6e61 6d65 732e 6f72 6720 6964   geonames.org id
-00008d30: 656e 7469 6669 6572 0a0a 2020 2020 5265  entifier..    Re
-00008d40: 7475 726e 733a 0a20 2020 2020 2020 2061  turns:.        a
-00008d50: 6e20 6574 7265 652e 5f45 6c65 6d65 6e74  n etree._Element
-00008d60: 2074 6861 7420 6361 6e20 6265 2061 7070   that can be app
-00008d70: 656e 6465 6420 746f 2074 6865 2070 6172  ended to the par
-00008d80: 656e 7420 7265 736f 7572 6365 2077 6974  ent resource wit
-00008d90: 6820 7265 736f 7572 6365 2e61 7070 656e  h resource.appen
-00008da0: 6428 6d61 6b65 5f2a 5f70 726f 7028 2e2e  d(make_*_prop(..
-00008db0: 2e29 290a 0a20 2020 2045 7861 6d70 6c65  .))..    Example
-00008dc0: 733a 0a20 2020 2020 2020 203e 3e3e 2065  s:.        >>> e
-00008dd0: 7863 656c 3278 6d6c 2e6d 616b 655f 6765  xcel2xml.make_ge
-00008de0: 6f6e 616d 655f 7072 6f70 2822 3a74 6573  oname_prop(":tes
-00008df0: 7470 726f 7065 7274 7922 2c20 2232 3736  tproperty", "276
-00008e00: 3133 3639 2229 0a20 2020 2020 2020 2020  1369").         
-00008e10: 2020 2020 2020 203c 6765 6f6e 616d 652d         <geoname-
-00008e20: 7072 6f70 206e 616d 653d 223a 7465 7374  prop name=":test
-00008e30: 7072 6f70 6572 7479 223e 0a20 2020 2020  property">.     
-00008e40: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00008e50: 6765 6f6e 616d 6520 7065 726d 6973 7369  geoname permissi
-00008e60: 6f6e 733d 2270 726f 702d 6465 6661 756c  ons="prop-defaul
-00008e70: 7422 3e32 3736 3133 3639 3c2f 6765 6f6e  t">2761369</geon
-00008e80: 616d 653e 0a20 2020 2020 2020 2020 2020  ame>.           
-00008e90: 2020 2020 203c 2f67 656f 6e61 6d65 2d70       </geoname-p
-00008ea0: 726f 703e 0a20 2020 2020 2020 203e 3e3e  rop>.        >>>
-00008eb0: 2065 7863 656c 3278 6d6c 2e6d 616b 655f   excel2xml.make_
-00008ec0: 6765 6f6e 616d 655f 7072 6f70 2822 3a74  geoname_prop(":t
-00008ed0: 6573 7470 726f 7065 7274 7922 2c20 6578  estproperty", ex
-00008ee0: 6365 6c32 786d 6c2e 5072 6f70 6572 7479  cel2xml.Property
-00008ef0: 456c 656d 656e 7428 2232 3736 3133 3639  Element("2761369
-00008f00: 222c 2070 6572 6d69 7373 696f 6e73 3d22  ", permissions="
-00008f10: 7072 6f70 2d72 6573 7472 6963 7465 6422  prop-restricted"
-00008f20: 2c20 636f 6d6d 656e 743d 2265 7861 6d70  , comment="examp
-00008f30: 6c65 2229 290a 2020 2020 2020 2020 2020  le")).          
-00008f40: 2020 2020 2020 3c67 656f 6e61 6d65 2d70        <geoname-p
-00008f50: 726f 7020 6e61 6d65 3d22 3a74 6573 7470  rop name=":testp
-00008f60: 726f 7065 7274 7922 3e0a 2020 2020 2020  roperty">.      
-00008f70: 2020 2020 2020 2020 2020 2020 2020 3c67                <g
-00008f80: 656f 6e61 6d65 2070 6572 6d69 7373 696f  eoname permissio
-00008f90: 6e73 3d22 7072 6f70 2d72 6573 7472 6963  ns="prop-restric
-00008fa0: 7465 6422 2063 6f6d 6d65 6e74 3d22 6578  ted" comment="ex
-00008fb0: 616d 706c 6522 3e32 3736 3133 3639 3c2f  ample">2761369</
-00008fc0: 6765 6f6e 616d 653e 0a20 2020 2020 2020  geoname>.       
-00008fd0: 2020 2020 2020 2020 203c 2f67 656f 6e61           </geona
-00008fe0: 6d65 2d70 726f 703e 0a20 2020 2020 2020  me-prop>.       
-00008ff0: 203e 3e3e 2065 7863 656c 3278 6d6c 2e6d   >>> excel2xml.m
-00009000: 616b 655f 6765 6f6e 616d 655f 7072 6f70  ake_geoname_prop
-00009010: 2822 3a74 6573 7470 726f 7065 7274 7922  (":testproperty"
-00009020: 2c20 5b22 3237 3631 3336 3922 2c20 2231  , ["2761369", "1
-00009030: 3031 3031 3031 225d 290a 2020 2020 2020  010101"]).      
-00009040: 2020 2020 2020 2020 2020 3c67 656f 6e61            <geona
-00009050: 6d65 2d70 726f 7020 6e61 6d65 3d22 3a74  me-prop name=":t
-00009060: 6573 7470 726f 7065 7274 7922 3e0a 2020  estproperty">.  
-00009070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009080: 2020 3c67 656f 6e61 6d65 2070 6572 6d69    <geoname permi
-00009090: 7373 696f 6e73 3d22 7072 6f70 2d64 6566  ssions="prop-def
-000090a0: 6175 6c74 223e 3237 3631 3336 393c 2f67  ault">2761369</g
-000090b0: 656f 6e61 6d65 3e0a 2020 2020 2020 2020  eoname>.        
-000090c0: 2020 2020 2020 2020 2020 2020 3c67 656f              <geo
-000090d0: 6e61 6d65 2070 6572 6d69 7373 696f 6e73  name permissions
-000090e0: 3d22 7072 6f70 2d64 6566 6175 6c74 223e  ="prop-default">
-000090f0: 3130 3130 3130 313c 2f67 656f 6e61 6d65  1010101</geoname
-00009100: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00009110: 2020 3c2f 6765 6f6e 616d 652d 7072 6f70    </geoname-prop
-00009120: 3e0a 0a20 2020 2053 6565 2068 7474 7073  >..    See https
-00009130: 3a2f 2f64 6f63 732e 6461 7363 682e 7377  ://docs.dasch.sw
-00009140: 6973 732f 6c61 7465 7374 2f44 5350 2d54  iss/latest/DSP-T
-00009150: 4f4f 4c53 2f66 696c 652d 666f 726d 6174  OOLS/file-format
-00009160: 732f 786d 6c2d 6461 7461 2d66 696c 652f  s/xml-data-file/
-00009170: 2367 656f 6e61 6d65 2d70 726f 700a 2020  #geoname-prop.  
-00009180: 2020 2222 220a 0a20 2020 2023 2063 6865    """..    # che
-00009190: 636b 2074 6865 2069 6e70 7574 3a20 7072  ck the input: pr
-000091a0: 6570 6172 6520 6120 6c69 7374 2077 6974  epare a list wit
-000091b0: 6820 7661 6c69 6420 7661 6c75 6573 0a20  h valid values. 
-000091c0: 2020 2076 616c 7565 7320 3d20 7072 6570     values = prep
-000091d0: 6172 655f 7661 6c75 6528 7661 6c75 6529  are_value(value)
-000091e0: 0a0a 2020 2020 2320 6368 6563 6b20 7661  ..    # check va
-000091f0: 6c75 6520 7479 7065 0a20 2020 2066 6f72  lue type.    for
-00009200: 2076 616c 2069 6e20 7661 6c75 6573 3a0a   val in values:.
-00009210: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
-00009220: 6567 6578 2e73 6561 7263 6828 7222 5e5b  egex.search(r"^[
-00009230: 302d 395d 2b24 222c 2073 7472 2876 616c  0-9]+$", str(val
-00009240: 2e76 616c 7565 2929 3a0a 2020 2020 2020  .value)):.      
-00009250: 2020 2020 2020 6d73 6720 3d20 280a 2020        msg = (.  
-00009260: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-00009270: 4661 696c 6564 2076 616c 6964 6174 696f  Failed validatio
-00009280: 6e20 696e 2072 6573 6f75 7263 6520 277b  n in resource '{
-00009290: 6361 6c6c 696e 675f 7265 736f 7572 6365  calling_resource
-000092a0: 7d27 2c20 7072 6f70 6572 7479 2027 7b6e  }', property '{n
-000092b0: 616d 657d 273a 2022 0a20 2020 2020 2020  ame}': ".       
-000092c0: 2020 2020 2020 2020 2066 2227 7b76 616c           f"'{val
-000092d0: 2e76 616c 7565 7d27 2069 7320 6e6f 7420  .value}' is not 
-000092e0: 6120 6765 6f6e 616d 6573 2e6f 7267 2069  a geonames.org i
-000092f0: 6465 6e74 6966 6965 722e 220a 2020 2020  dentifier.".    
-00009300: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00009310: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
-00009320: 6172 6e28 4473 7054 6f6f 6c73 5573 6572  arn(DspToolsUser
-00009330: 5761 726e 696e 6728 6d73 6729 290a 0a20  Warning(msg)).. 
-00009340: 2020 2023 206d 616b 6520 786d 6c20 7374     # make xml st
-00009350: 7275 6374 7572 6520 6f66 2074 6865 2076  ructure of the v
-00009360: 616c 6964 2076 616c 7565 730a 2020 2020  alid values.    
-00009370: 7072 6f70 5f20 3d20 6574 7265 652e 456c  prop_ = etree.El
-00009380: 656d 656e 7428 0a20 2020 2020 2020 2022  ement(.        "
-00009390: 7b25 737d 6765 6f6e 616d 652d 7072 6f70  {%s}geoname-prop
-000093a0: 2220 2520 786d 6c5f 6e61 6d65 7370 6163  " % xml_namespac
-000093b0: 655f 6d61 705b 4e6f 6e65 5d2c 0a20 2020  e_map[None],.   
-000093c0: 2020 2020 206e 616d 653d 6e61 6d65 2c0a       name=name,.
-000093d0: 2020 2020 2020 2020 6e73 6d61 703d 786d          nsmap=xm
-000093e0: 6c5f 6e61 6d65 7370 6163 655f 6d61 702c  l_namespace_map,
-000093f0: 0a20 2020 2029 0a20 2020 2066 6f72 2076  .    ).    for v
-00009400: 616c 2069 6e20 7661 6c75 6573 3a0a 2020  al in values:.  
-00009410: 2020 2020 2020 6b77 6172 6773 203d 207b        kwargs = {
-00009420: 2270 6572 6d69 7373 696f 6e73 223a 2076  "permissions": v
-00009430: 616c 2e70 6572 6d69 7373 696f 6e73 7d0a  al.permissions}.
-00009440: 2020 2020 2020 2020 6966 2076 616c 2e63          if val.c
-00009450: 6f6d 6d65 6e74 2061 6e64 2063 6865 636b  omment and check
-00009460: 5f6e 6f74 6e61 2876 616c 2e63 6f6d 6d65  _notna(val.comme
-00009470: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
-00009480: 206b 7761 7267 735b 2263 6f6d 6d65 6e74   kwargs["comment
-00009490: 225d 203d 2076 616c 2e63 6f6d 6d65 6e74  "] = val.comment
-000094a0: 0a20 2020 2020 2020 2076 616c 7565 5f20  .        value_ 
-000094b0: 3d20 6574 7265 652e 456c 656d 656e 7428  = etree.Element(
-000094c0: 0a20 2020 2020 2020 2020 2020 2022 7b25  .            "{%
-000094d0: 737d 6765 6f6e 616d 6522 2025 2078 6d6c  s}geoname" % xml
-000094e0: 5f6e 616d 6573 7061 6365 5f6d 6170 5b4e  _namespace_map[N
-000094f0: 6f6e 655d 2c0a 2020 2020 2020 2020 2020  one],.          
-00009500: 2020 2a2a 6b77 6172 6773 2c20 2023 2074    **kwargs,  # t
-00009510: 7970 653a 2069 676e 6f72 655b 6172 672d  ype: ignore[arg-
-00009520: 7479 7065 5d0a 2020 2020 2020 2020 2020  type].          
-00009530: 2020 6e73 6d61 703d 786d 6c5f 6e61 6d65    nsmap=xml_name
-00009540: 7370 6163 655f 6d61 702c 0a20 2020 2020  space_map,.     
-00009550: 2020 2029 0a20 2020 2020 2020 2076 616c     ).        val
-00009560: 7565 5f2e 7465 7874 203d 2073 7472 2876  ue_.text = str(v
-00009570: 616c 2e76 616c 7565 290a 2020 2020 2020  al.value).      
-00009580: 2020 7072 6f70 5f2e 6170 7065 6e64 2876    prop_.append(v
-00009590: 616c 7565 5f29 0a0a 2020 2020 7265 7475  alue_)..    retu
-000095a0: 726e 2070 726f 705f 0a0a 0a64 6566 206d  rn prop_...def m
-000095b0: 616b 655f 696e 7465 6765 725f 7072 6f70  ake_integer_prop
-000095c0: 280a 2020 2020 6e61 6d65 3a20 7374 722c  (.    name: str,
-000095d0: 0a20 2020 2076 616c 7565 3a20 556e 696f  .    value: Unio
-000095e0: 6e5b 5072 6f70 6572 7479 456c 656d 656e  n[PropertyElemen
-000095f0: 742c 2073 7472 2c20 696e 742c 2049 7465  t, str, int, Ite
-00009600: 7261 626c 655b 556e 696f 6e5b 5072 6f70  rable[Union[Prop
-00009610: 6572 7479 456c 656d 656e 742c 2073 7472  ertyElement, str
-00009620: 2c20 696e 745d 5d5d 2c0a 2020 2020 6361  , int]]],.    ca
-00009630: 6c6c 696e 675f 7265 736f 7572 6365 3a20  lling_resource: 
-00009640: 7374 7220 3d20 2222 2c0a 2920 2d3e 2065  str = "",.) -> e
-00009650: 7472 6565 2e5f 456c 656d 656e 743a 0a20  tree._Element:. 
-00009660: 2020 2022 2222 0a20 2020 204d 616b 6520     """.    Make 
-00009670: 6120 3c69 6e74 6567 6572 2d70 726f 703e  a <integer-prop>
-00009680: 2066 726f 6d20 6f6e 6520 6f72 206d 6f72   from one or mor
-00009690: 6520 696e 7465 6765 7273 2e20 5468 6520  e integers. The 
-000096a0: 696e 7465 6765 7273 2063 616e 2062 6520  integers can be 
-000096b0: 7072 6f76 6964 6564 2061 7320 7374 7269  provided as stri
-000096c0: 6e67 2c20 696e 7465 6765 722c 206f 7220  ng, integer, or 
-000096d0: 6173 0a20 2020 2050 726f 7065 7274 7945  as.    PropertyE
-000096e0: 6c65 6d65 6e74 2077 6974 6820 6120 7374  lement with a st
-000096f0: 7269 6e67 2f69 6e74 6567 6572 2069 6e73  ring/integer ins
-00009700: 6964 652e 2049 6620 7072 6f76 6964 6564  ide. If provided
-00009710: 2061 7320 7374 7269 6e67 2f69 6e74 6567   as string/integ
-00009720: 6572 2c20 7468 6520 7065 726d 6973 7369  er, the permissi
-00009730: 6f6e 7320 6465 6661 756c 7420 746f 0a20  ons default to. 
-00009740: 2020 2022 7072 6f70 2d64 6566 6175 6c74     "prop-default
-00009750: 222e 0a0a 2020 2020 4172 6773 3a0a 2020  "...    Args:.  
-00009760: 2020 2020 2020 6e61 6d65 3a20 7468 6520        name: the 
-00009770: 6e61 6d65 206f 6620 7468 6973 2070 726f  name of this pro
-00009780: 7065 7274 7920 6173 2064 6566 696e 6564  perty as defined
-00009790: 2069 6e20 7468 6520 6f6e 746f 0a20 2020   in the onto.   
-000097a0: 2020 2020 2076 616c 7565 3a20 6f6e 6520       value: one 
-000097b0: 6f72 206d 6f72 6520 696e 7465 6765 7273  or more integers
-000097c0: 2c20 6173 2073 7472 696e 672f 696e 742f  , as string/int/
-000097d0: 5072 6f70 6572 7479 456c 656d 656e 742c  PropertyElement,
-000097e0: 206f 7220 6173 2069 7465 7261 626c 6520   or as iterable 
-000097f0: 6f66 2073 7472 696e 6773 2f69 6e74 732f  of strings/ints/
-00009800: 5072 6f70 6572 7479 456c 656d 656e 7473  PropertyElements
-00009810: 0a20 2020 2020 2020 2063 616c 6c69 6e67  .        calling
-00009820: 5f72 6573 6f75 7263 653a 2074 6865 206e  _resource: the n
-00009830: 616d 6520 6f66 2074 6865 2070 6172 656e  ame of the paren
-00009840: 7420 7265 736f 7572 6365 2028 666f 7220  t resource (for 
-00009850: 6265 7474 6572 2065 7272 6f72 206d 6573  better error mes
-00009860: 7361 6765 7329 0a0a 2020 2020 5761 726e  sages)..    Warn
-00009870: 733a 0a20 2020 2020 2020 2049 6620 7468  s:.        If th
-00009880: 6520 7661 6c75 6520 6973 206e 6f74 2061  e value is not a
-00009890: 2076 616c 6964 2069 6e74 6567 6572 0a0a   valid integer..
-000098a0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-000098b0: 2020 2020 2061 6e20 6574 7265 652e 5f45       an etree._E
-000098c0: 6c65 6d65 6e74 2074 6861 7420 6361 6e20  lement that can 
-000098d0: 6265 2061 7070 656e 6465 6420 746f 2074  be appended to t
-000098e0: 6865 2070 6172 656e 7420 7265 736f 7572  he parent resour
-000098f0: 6365 2077 6974 6820 7265 736f 7572 6365  ce with resource
-00009900: 2e61 7070 656e 6428 6d61 6b65 5f2a 5f70  .append(make_*_p
-00009910: 726f 7028 2e2e 2e29 290a 0a20 2020 2045  rop(...))..    E
-00009920: 7861 6d70 6c65 733a 0a20 2020 2020 2020  xamples:.       
-00009930: 203e 3e3e 2065 7863 656c 3278 6d6c 2e6d   >>> excel2xml.m
-00009940: 616b 655f 696e 7465 6765 725f 7072 6f70  ake_integer_prop
-00009950: 2822 3a74 6573 7470 726f 7065 7274 7922  (":testproperty"
-00009960: 2c20 2232 3736 3133 3639 2229 0a20 2020  , "2761369").   
-00009970: 2020 2020 2020 2020 2020 2020 203c 696e               <in
-00009980: 7465 6765 722d 7072 6f70 206e 616d 653d  teger-prop name=
-00009990: 223a 7465 7374 7072 6f70 6572 7479 223e  ":testproperty">
-000099a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000099b0: 2020 2020 203c 696e 7465 6765 7220 7065       <integer pe
-000099c0: 726d 6973 7369 6f6e 733d 2270 726f 702d  rmissions="prop-
-000099d0: 6465 6661 756c 7422 3e32 3736 3133 3639  default">2761369
-000099e0: 3c2f 696e 7465 6765 723e 0a20 2020 2020  </integer>.     
-000099f0: 2020 2020 2020 2020 2020 203c 2f69 6e74             </int
-00009a00: 6567 6572 2d70 726f 703e 0a20 2020 2020  eger-prop>.     
-00009a10: 2020 203e 3e3e 2065 7863 656c 3278 6d6c     >>> excel2xml
-00009a20: 2e6d 616b 655f 696e 7465 6765 725f 7072  .make_integer_pr
-00009a30: 6f70 2822 3a74 6573 7470 726f 7065 7274  op(":testpropert
-00009a40: 7922 2c20 6578 6365 6c32 786d 6c2e 5072  y", excel2xml.Pr
-00009a50: 6f70 6572 7479 456c 656d 656e 7428 2232  opertyElement("2
-00009a60: 3736 3133 3639 222c 2070 6572 6d69 7373  761369", permiss
-00009a70: 696f 6e73 3d22 7072 6f70 2d72 6573 7472  ions="prop-restr
-00009a80: 6963 7465 6422 2c20 636f 6d6d 656e 743d  icted", comment=
-00009a90: 2265 7861 6d70 6c65 2229 290a 2020 2020  "example")).    
-00009aa0: 2020 2020 2020 2020 2020 2020 3c69 6e74              <int
-00009ab0: 6567 6572 2d70 726f 7020 6e61 6d65 3d22  eger-prop name="
-00009ac0: 3a74 6573 7470 726f 7065 7274 7922 3e0a  :testproperty">.
-00009ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ae0: 2020 2020 3c69 6e74 6567 6572 2070 6572      <integer per
-00009af0: 6d69 7373 696f 6e73 3d22 7072 6f70 2d72  missions="prop-r
-00009b00: 6573 7472 6963 7465 6422 2063 6f6d 6d65  estricted" comme
-00009b10: 6e74 3d22 6578 616d 706c 6522 3e32 3736  nt="example">276
-00009b20: 3133 3639 3c2f 696e 7465 6765 723e 0a20  1369</integer>. 
-00009b30: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00009b40: 2f69 6e74 6567 6572 2d70 726f 703e 0a20  /integer-prop>. 
-00009b50: 2020 2020 2020 203e 3e3e 2065 7863 656c         >>> excel
-00009b60: 3278 6d6c 2e6d 616b 655f 696e 7465 6765  2xml.make_intege
-00009b70: 725f 7072 6f70 2822 3a74 6573 7470 726f  r_prop(":testpro
-00009b80: 7065 7274 7922 2c20 5b22 3237 3631 3336  perty", ["276136
-00009b90: 3922 2c20 2231 3031 3031 3031 225d 290a  9", "1010101"]).
-00009ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bb0: 3c69 6e74 6567 6572 2d70 726f 7020 6e61  <integer-prop na
-00009bc0: 6d65 3d22 3a74 6573 7470 726f 7065 7274  me=":testpropert
-00009bd0: 7922 3e0a 2020 2020 2020 2020 2020 2020  y">.            
-00009be0: 2020 2020 2020 2020 3c69 6e74 6567 6572          <integer
-00009bf0: 2070 6572 6d69 7373 696f 6e73 3d22 7072   permissions="pr
-00009c00: 6f70 2d64 6566 6175 6c74 223e 3237 3631  op-default">2761
-00009c10: 3336 393c 2f69 6e74 6567 6572 3e0a 2020  369</integer>.  
-00009c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c30: 2020 3c69 6e74 6567 6572 2070 6572 6d69    <integer permi
-00009c40: 7373 696f 6e73 3d22 7072 6f70 2d64 6566  ssions="prop-def
-00009c50: 6175 6c74 223e 3130 3130 3130 313c 2f69  ault">1010101</i
-00009c60: 6e74 6567 6572 3e0a 2020 2020 2020 2020  nteger>.        
-00009c70: 2020 2020 2020 2020 3c2f 696e 7465 6765          </intege
-00009c80: 722d 7072 6f70 3e0a 0a20 2020 2053 6565  r-prop>..    See
-00009c90: 2068 7474 7073 3a2f 2f64 6f63 732e 6461   https://docs.da
-00009ca0: 7363 682e 7377 6973 732f 6c61 7465 7374  sch.swiss/latest
-00009cb0: 2f44 5350 2d54 4f4f 4c53 2f66 696c 652d  /DSP-TOOLS/file-
-00009cc0: 666f 726d 6174 732f 786d 6c2d 6461 7461  formats/xml-data
-00009cd0: 2d66 696c 652f 2369 6e74 6567 6572 2d70  -file/#integer-p
-00009ce0: 726f 700a 2020 2020 2222 220a 0a20 2020  rop.    """..   
-00009cf0: 2023 2063 6865 636b 2074 6865 2069 6e70   # check the inp
-00009d00: 7574 3a20 7072 6570 6172 6520 6120 6c69  ut: prepare a li
-00009d10: 7374 2077 6974 6820 7661 6c69 6420 7661  st with valid va
-00009d20: 6c75 6573 0a20 2020 2076 616c 7565 7320  lues.    values 
-00009d30: 3d20 7072 6570 6172 655f 7661 6c75 6528  = prepare_value(
-00009d40: 7661 6c75 6529 0a0a 2020 2020 2320 6368  value)..    # ch
-00009d50: 6563 6b20 7661 6c75 6520 7479 7065 0a20  eck value type. 
-00009d60: 2020 2066 6f72 2076 616c 2069 6e20 7661     for val in va
-00009d70: 6c75 6573 3a0a 2020 2020 2020 2020 7472  lues:.        tr
-00009d80: 793a 0a20 2020 2020 2020 2020 2020 2069  y:.            i
-00009d90: 6e74 2876 616c 2e76 616c 7565 290a 2020  nt(val.value).  
-00009da0: 2020 2020 2020 6578 6365 7074 2056 616c        except Val
-00009db0: 7565 4572 726f 723a 0a20 2020 2020 2020  ueError:.       
-00009dc0: 2020 2020 206d 7367 203d 2028 0a20 2020       msg = (.   
-00009dd0: 2020 2020 2020 2020 2020 2020 2066 2246               f"F
-00009de0: 6169 6c65 6420 7661 6c69 6461 7469 6f6e  ailed validation
-00009df0: 2069 6e20 7265 736f 7572 6365 2027 7b63   in resource '{c
-00009e00: 616c 6c69 6e67 5f72 6573 6f75 7263 657d  alling_resource}
-00009e10: 272c 2070 726f 7065 7274 7920 277b 6e61  ', property '{na
-00009e20: 6d65 7d27 3a20 220a 2020 2020 2020 2020  me}': ".        
-00009e30: 2020 2020 2020 2020 6622 277b 7661 6c2e          f"'{val.
-00009e40: 7661 6c75 657d 2720 6973 206e 6f74 2061  value}' is not a
-00009e50: 2076 616c 6964 2069 6e74 6567 6572 2e22   valid integer."
-00009e60: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00009e70: 2020 2020 2020 2020 2020 2077 6172 6e69             warni
-00009e80: 6e67 732e 7761 726e 2844 7370 546f 6f6c  ngs.warn(DspTool
-00009e90: 7355 7365 7257 6172 6e69 6e67 286d 7367  sUserWarning(msg
-00009ea0: 2929 0a0a 2020 2020 2320 6d61 6b65 2078  ))..    # make x
-00009eb0: 6d6c 2073 7472 7563 7475 7265 206f 6620  ml structure of 
-00009ec0: 7468 6520 7661 6c69 6420 7661 6c75 6573  the valid values
-00009ed0: 0a20 2020 2070 726f 705f 203d 2065 7472  .    prop_ = etr
-00009ee0: 6565 2e45 6c65 6d65 6e74 280a 2020 2020  ee.Element(.    
-00009ef0: 2020 2020 227b 2573 7d69 6e74 6567 6572      "{%s}integer
-00009f00: 2d70 726f 7022 2025 2078 6d6c 5f6e 616d  -prop" % xml_nam
-00009f10: 6573 7061 6365 5f6d 6170 5b4e 6f6e 655d  espace_map[None]
-00009f20: 2c0a 2020 2020 2020 2020 6e61 6d65 3d6e  ,.        name=n
-00009f30: 616d 652c 0a20 2020 2020 2020 206e 736d  ame,.        nsm
-00009f40: 6170 3d78 6d6c 5f6e 616d 6573 7061 6365  ap=xml_namespace
-00009f50: 5f6d 6170 2c0a 2020 2020 290a 2020 2020  _map,.    ).    
-00009f60: 666f 7220 7661 6c20 696e 2076 616c 7565  for val in value
-00009f70: 733a 0a20 2020 2020 2020 206b 7761 7267  s:.        kwarg
-00009f80: 7320 3d20 7b22 7065 726d 6973 7369 6f6e  s = {"permission
-00009f90: 7322 3a20 7661 6c2e 7065 726d 6973 7369  s": val.permissi
-00009fa0: 6f6e 737d 0a20 2020 2020 2020 2069 6620  ons}.        if 
-00009fb0: 7661 6c2e 636f 6d6d 656e 7420 616e 6420  val.comment and 
-00009fc0: 6368 6563 6b5f 6e6f 746e 6128 7661 6c2e  check_notna(val.
-00009fd0: 636f 6d6d 656e 7429 3a0a 2020 2020 2020  comment):.      
-00009fe0: 2020 2020 2020 6b77 6172 6773 5b22 636f        kwargs["co
-00009ff0: 6d6d 656e 7422 5d20 3d20 7661 6c2e 636f  mment"] = val.co
-0000a000: 6d6d 656e 740a 2020 2020 2020 2020 7661  mment.        va
-0000a010: 6c75 655f 203d 2065 7472 6565 2e45 6c65  lue_ = etree.Ele
-0000a020: 6d65 6e74 280a 2020 2020 2020 2020 2020  ment(.          
-0000a030: 2020 227b 2573 7d69 6e74 6567 6572 2220    "{%s}integer" 
-0000a040: 2520 786d 6c5f 6e61 6d65 7370 6163 655f  % xml_namespace_
-0000a050: 6d61 705b 4e6f 6e65 5d2c 0a20 2020 2020  map[None],.     
-0000a060: 2020 2020 2020 202a 2a6b 7761 7267 732c         **kwargs,
-0000a070: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
-0000a080: 5b61 7267 2d74 7970 655d 0a20 2020 2020  [arg-type].     
-0000a090: 2020 2020 2020 206e 736d 6170 3d78 6d6c         nsmap=xml
-0000a0a0: 5f6e 616d 6573 7061 6365 5f6d 6170 2c0a  _namespace_map,.
-0000a0b0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000a0c0: 2020 7661 6c75 655f 2e74 6578 7420 3d20    value_.text = 
-0000a0d0: 7374 7228 7661 6c2e 7661 6c75 6529 0a20  str(val.value). 
-0000a0e0: 2020 2020 2020 2070 726f 705f 2e61 7070         prop_.app
-0000a0f0: 656e 6428 7661 6c75 655f 290a 0a20 2020  end(value_)..   
-0000a100: 2072 6574 7572 6e20 7072 6f70 5f0a 0a0a   return prop_...
-0000a110: 6465 6620 6d61 6b65 5f69 6e74 6572 7661  def make_interva
-0000a120: 6c5f 7072 6f70 286e 616d 653a 2073 7472  l_prop(name: str
-0000a130: 2c20 7661 6c75 653a 2055 6e69 6f6e 5b50  , value: Union[P
-0000a140: 726f 7065 7274 7945 6c65 6d65 6e74 2c20  ropertyElement, 
-0000a150: 7374 725d 2c20 6361 6c6c 696e 675f 7265  str], calling_re
-0000a160: 736f 7572 6365 3a20 7374 7220 3d20 2222  source: str = ""
-0000a170: 2920 2d3e 2065 7472 6565 2e5f 456c 656d  ) -> etree._Elem
-0000a180: 656e 743a 0a20 2020 2022 2222 0a20 2020  ent:.    """.   
-0000a190: 204d 616b 6520 6120 3c69 6e74 6572 7661   Make a <interva
-0000a1a0: 6c2d 7072 6f70 206e 616d 653d 2268 6173  l-prop name="has
-0000a1b0: 5365 676d 656e 7442 6f75 6e64 7322 3e20  SegmentBounds"> 
-0000a1c0: 666f 7220 6120 3c76 6964 656f 2d73 6567  for a <video-seg
-0000a1d0: 6d65 6e74 3e20 6f72 203c 6175 6469 6f2d  ment> or <audio-
-0000a1e0: 7365 676d 656e 743e 2e0a 2020 2020 5468  segment>..    Th
-0000a1f0: 6520 696e 7465 7276 616c 2063 616e 2062  e interval can b
-0000a200: 6520 7072 6f76 6964 6564 2061 7320 7374  e provided as st
-0000a210: 7269 6e67 206f 7220 6173 2050 726f 7065  ring or as Prope
-0000a220: 7274 7945 6c65 6d65 6e74 2077 6974 6820  rtyElement with 
-0000a230: 6120 7374 7269 6e67 2069 6e73 6964 652e  a string inside.
-0000a240: 0a20 2020 2049 6620 7072 6f76 6964 6564  .    If provided
-0000a250: 2061 7320 7374 7269 6e67 2c20 7468 6520   as string, the 
-0000a260: 7065 726d 6973 7369 6f6e 7320 6465 6661  permissions defa
-0000a270: 756c 7420 746f 2022 7072 6f70 2d64 6566  ult to "prop-def
-0000a280: 6175 6c74 222e 0a20 2020 2044 5350 2069  ault"..    DSP i
-0000a290: 6e74 6572 7661 6c20 7661 6c75 6573 2061  nterval values a
-0000a2a0: 7265 2066 6f72 6d61 7474 6564 2061 7320  re formatted as 
-0000a2b0: 2273 7461 7274 5f73 6563 6f6e 6473 3a65  "start_seconds:e
-0000a2c0: 6e64 5f73 6563 6f6e 6473 222e 0a20 2020  nd_seconds"..   
-0000a2d0: 2042 6f74 6820 6e75 6d62 6572 7320 6361   Both numbers ca
-0000a2e0: 6e20 6861 7665 2061 2064 6563 696d 616c  n have a decimal
-0000a2f0: 2070 6f69 6e74 2c20 666f 7220 6672 6163   point, for frac
-0000a300: 7469 6f6e 7320 6f66 2073 6563 6f6e 6473  tions of seconds
-0000a310: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-0000a320: 2020 2020 206e 616d 653a 2074 6865 206e       name: the n
-0000a330: 616d 6520 6f66 2074 6869 7320 7072 6f70  ame of this prop
-0000a340: 6572 7479 2e20 5468 6520 6f6e 6c79 2061  erty. The only a
-0000a350: 6363 6570 7465 6420 7661 6c75 6520 6973  ccepted value is
-0000a360: 2022 6861 7353 6567 6d65 6e74 426f 756e   "hasSegmentBoun
-0000a370: 6473 220a 2020 2020 2020 2020 7661 6c75  ds".        valu
-0000a380: 653a 2061 2044 5350 2069 6e74 6572 7661  e: a DSP interva
-0000a390: 6c2c 2061 7320 7374 7269 6e67 206f 7220  l, as string or 
-0000a3a0: 5072 6f70 6572 7479 456c 656d 656e 740a  PropertyElement.
-0000a3b0: 2020 2020 2020 2020 6361 6c6c 696e 675f          calling_
-0000a3c0: 7265 736f 7572 6365 3a20 7468 6520 6e61  resource: the na
-0000a3d0: 6d65 206f 6620 7468 6520 7061 7265 6e74  me of the parent
-0000a3e0: 2072 6573 6f75 7263 6520 2866 6f72 2062   resource (for b
-0000a3f0: 6574 7465 7220 6572 726f 7220 6d65 7373  etter error mess
-0000a400: 6167 6573 290a 0a20 2020 2057 6172 6e73  ages)..    Warns
-0000a410: 3a0a 2020 2020 2020 2020 2d20 4966 2074  :.        - If t
-0000a420: 6865 2076 616c 7565 2069 7320 6e6f 7420  he value is not 
-0000a430: 6120 7661 6c69 6420 4453 5020 696e 7465  a valid DSP inte
-0000a440: 7276 616c 0a20 2020 2020 2020 202d 2049  rval.        - I
-0000a450: 6620 7468 6520 6e61 6d65 2069 7320 6e6f  f the name is no
-0000a460: 7420 2268 6173 5365 676d 656e 7442 6f75  t "hasSegmentBou
-0000a470: 6e64 7322 0a0a 2020 2020 5265 7475 726e  nds"..    Return
-0000a480: 733a 0a20 2020 2020 2020 2061 6e20 6574  s:.        an et
-0000a490: 7265 652e 5f45 6c65 6d65 6e74 2074 6861  ree._Element tha
-0000a4a0: 7420 6361 6e20 6265 2061 7070 656e 6465  t can be appende
-0000a4b0: 6420 746f 2074 6865 2070 6172 656e 7420  d to the parent 
-0000a4c0: 7265 736f 7572 6365 2077 6974 6820 7265  resource with re
-0000a4d0: 736f 7572 6365 2e61 7070 656e 6428 6d61  source.append(ma
-0000a4e0: 6b65 5f2a 5f70 726f 7028 2e2e 2e29 290a  ke_*_prop(...)).
-0000a4f0: 0a20 2020 2045 7861 6d70 6c65 733a 0a20  .    Examples:. 
-0000a500: 2020 2020 2020 203e 3e3e 2069 6e74 6572         >>> inter
-0000a510: 7661 6c20 3d20 6578 6365 6c32 786d 6c2e  val = excel2xml.
-0000a520: 6372 6561 7465 5f69 6e74 6572 7661 6c5f  create_interval_
-0000a530: 7661 6c75 6528 7374 6172 743d 2230 3a30  value(start="0:0
-0000a540: 313a 3030 222c 2065 6e64 3d22 303a 3032  1:00", end="0:02
-0000a550: 3a30 3022 2920 2023 2072 6573 756c 743a  :00")  # result:
-0000a560: 2022 3630 3a31 3230 220a 2020 2020 2020   "60:120".      
-0000a570: 2020 3e3e 3e20 6578 6365 6c32 786d 6c2e    >>> excel2xml.
-0000a580: 6d61 6b65 5f69 6e74 6572 7661 6c5f 7072  make_interval_pr
-0000a590: 6f70 2822 6861 7353 6567 6d65 6e74 426f  op("hasSegmentBo
-0000a5a0: 756e 6473 222c 2069 6e76 6572 7661 6c29  unds", inverval)
-0000a5b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a5c0: 203c 696e 7465 7276 616c 2d70 726f 7020   <interval-prop 
-0000a5d0: 6e61 6d65 3d22 6861 7353 6567 6d65 6e74  name="hasSegment
-0000a5e0: 426f 756e 6473 223e 0a20 2020 2020 2020  Bounds">.       
-0000a5f0: 2020 2020 2020 2020 2020 2020 203c 696e               <in
-0000a600: 7465 7276 616c 2070 6572 6d69 7373 696f  terval permissio
-0000a610: 6e73 3d22 7072 6f70 2d64 6566 6175 6c74  ns="prop-default
-0000a620: 223e 3630 3a31 3230 3c2f 696e 7465 7276  ">60:120</interv
-0000a630: 616c 3e0a 2020 2020 2020 2020 2020 2020  al>.            
-0000a640: 2020 2020 3c2f 696e 7465 7276 616c 2d70      </interval-p
-0000a650: 726f 703e 0a20 2020 2020 2020 203e 3e3e  rop>.        >>>
-0000a660: 2069 6e74 6572 7661 6c20 3d20 6578 6365   interval = exce
-0000a670: 6c32 786d 6c2e 6372 6561 7465 5f69 6e74  l2xml.create_int
-0000a680: 6572 7661 6c5f 7661 6c75 6528 7374 6172  erval_value(star
-0000a690: 743d 2230 3a33 303a 3030 222c 2065 6e64  t="0:30:00", end
-0000a6a0: 3d22 313a 3030 3a30 3022 2920 2023 2072  ="1:00:00")  # r
-0000a6b0: 6573 756c 743a 2022 3138 3030 3a33 3630  esult: "1800:360
-0000a6c0: 3022 0a20 2020 2020 2020 203e 3e3e 2065  0".        >>> e
-0000a6d0: 7863 656c 3278 6d6c 2e6d 616b 655f 696e  xcel2xml.make_in
-0000a6e0: 7465 7276 616c 5f70 726f 7028 2268 6173  terval_prop("has
-0000a6f0: 5365 676d 656e 7442 6f75 6e64 7322 2c20  SegmentBounds", 
-0000a700: 6578 6365 6c32 786d 6c2e 5072 6f70 6572  excel2xml.Proper
-0000a710: 7479 456c 656d 656e 7428 696e 7465 7276  tyElement(interv
-0000a720: 616c 2c20 7065 726d 6973 7369 6f6e 733d  al, permissions=
-0000a730: 2270 726f 702d 7265 7374 7269 6374 6564  "prop-restricted
-0000a740: 222c 2063 6f6d 6d65 6e74 3d22 6578 616d  ", comment="exam
-0000a750: 706c 6522 2929 0a20 2020 2020 2020 2020  ple")).         
-0000a760: 2020 2020 2020 203c 696e 7465 7276 616c         <interval
-0000a770: 2d70 726f 7020 6e61 6d65 3d22 6861 7353  -prop name="hasS
-0000a780: 6567 6d65 6e74 426f 756e 6473 3e0a 2020  egmentBounds>.  
-0000a790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a7a0: 2020 3c69 6e74 6572 7661 6c20 7065 726d    <interval perm
-0000a7b0: 6973 7369 6f6e 733d 2270 726f 702d 7265  issions="prop-re
-0000a7c0: 7374 7269 6374 6564 2220 636f 6d6d 656e  stricted" commen
-0000a7d0: 743d 2265 7861 6d70 6c65 223e 3138 3030  t="example">1800
-0000a7e0: 3a33 3630 303c 2f69 6e74 6572 7661 6c3e  :3600</interval>
-0000a7f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a800: 203c 2f69 6e74 6572 7661 6c2d 7072 6f70   </interval-prop
-0000a810: 3e0a 0a20 2020 2053 6565 2068 7474 7073  >..    See https
-0000a820: 3a2f 2f64 6f63 732e 6461 7363 682e 7377  ://docs.dasch.sw
-0000a830: 6973 732f 6c61 7465 7374 2f44 5350 2d54  iss/latest/DSP-T
-0000a840: 4f4f 4c53 2f66 696c 652d 666f 726d 6174  OOLS/file-format
-0000a850: 732f 786d 6c2d 6461 7461 2d66 696c 652f  s/xml-data-file/
-0000a860: 2376 6964 656f 2d73 6567 6d65 6e74 2d61  #video-segment-a
-0000a870: 7564 696f 2d73 6567 6d65 6e74 0a20 2020  udio-segment.   
-0000a880: 2022 2222 0a0a 2020 2020 6966 206e 616d   """..    if nam
-0000a890: 6520 213d 2022 6861 7353 6567 6d65 6e74  e != "hasSegment
-0000a8a0: 426f 756e 6473 223a 0a20 2020 2020 2020  Bounds":.       
-0000a8b0: 206d 7367 203d 2028 0a20 2020 2020 2020   msg = (.       
-0000a8c0: 2020 2020 2066 2246 6169 6c65 6420 7661       f"Failed va
-0000a8d0: 6c69 6461 7469 6f6e 2069 6e20 7265 736f  lidation in reso
-0000a8e0: 7572 6365 2027 7b63 616c 6c69 6e67 5f72  urce '{calling_r
-0000a8f0: 6573 6f75 7263 657d 272c 2070 726f 7065  esource}', prope
-0000a900: 7274 7920 277b 6e61 6d65 7d27 3a20 220a  rty '{name}': ".
-0000a910: 2020 2020 2020 2020 2020 2020 6622 5468              f"Th
-0000a920: 6520 6f6e 6c79 2061 6363 6570 7465 6420  e only accepted 
-0000a930: 7661 6c75 6520 666f 7220 276e 616d 6527  value for 'name'
-0000a940: 2069 7320 2768 6173 5365 676d 656e 7442   is 'hasSegmentB
-0000a950: 6f75 6e64 7327 2e22 0a20 2020 2020 2020  ounds'.".       
-0000a960: 2029 0a20 2020 2020 2020 2077 6172 6e69   ).        warni
-0000a970: 6e67 732e 7761 726e 2844 7370 546f 6f6c  ngs.warn(DspTool
-0000a980: 7355 7365 7257 6172 6e69 6e67 286d 7367  sUserWarning(msg
-0000a990: 2929 0a0a 2020 2020 7661 6c75 6520 3d20  ))..    value = 
-0000a9a0: 7661 6c75 6520 6966 2069 7369 6e73 7461  value if isinsta
-0000a9b0: 6e63 6528 7661 6c75 652c 2050 726f 7065  nce(value, Prope
-0000a9c0: 7274 7945 6c65 6d65 6e74 2920 656c 7365  rtyElement) else
-0000a9d0: 2050 726f 7065 7274 7945 6c65 6d65 6e74   PropertyElement
-0000a9e0: 2876 616c 7565 290a 0a20 2020 2023 2063  (value)..    # c
-0000a9f0: 6865 636b 2076 616c 7565 2074 7970 650a  heck value type.
-0000aa00: 2020 2020 6966 206e 6f74 2072 6567 6578      if not regex
-0000aa10: 2e6d 6174 6368 2872 225c 642b 285c 2e5c  .match(r"\d+(\.\
-0000aa20: 642b 293f 3a5c 642b 285c 2e5c 642b 293f  d+)?:\d+(\.\d+)?
-0000aa30: 222c 2073 7472 2876 616c 7565 2e76 616c  ", str(value.val
-0000aa40: 7565 2929 3a0a 2020 2020 2020 2020 6d73  ue)):.        ms
-0000aa50: 6720 3d20 280a 2020 2020 2020 2020 2020  g = (.          
-0000aa60: 2020 6622 4661 696c 6564 2076 616c 6964    f"Failed valid
-0000aa70: 6174 696f 6e20 696e 2072 6573 6f75 7263  ation in resourc
-0000aa80: 6520 277b 6361 6c6c 696e 675f 7265 736f  e '{calling_reso
-0000aa90: 7572 6365 7d27 2c20 7072 6f70 6572 7479  urce}', property
-0000aaa0: 2027 7b6e 616d 657d 273a 2022 0a20 2020   '{name}': ".   
-0000aab0: 2020 2020 2020 2020 2066 2227 7b76 616c           f"'{val
-0000aac0: 7565 2e76 616c 7565 7d27 2069 7320 6e6f  ue.value}' is no
-0000aad0: 7420 6120 7661 6c69 6420 4453 5020 696e  t a valid DSP in
-0000aae0: 7465 7276 616c 2e22 0a20 2020 2020 2020  terval.".       
-0000aaf0: 2029 0a20 2020 2020 2020 2077 6172 6e69   ).        warni
-0000ab00: 6e67 732e 7761 726e 2844 7370 546f 6f6c  ngs.warn(DspTool
-0000ab10: 7355 7365 7257 6172 6e69 6e67 286d 7367  sUserWarning(msg
-0000ab20: 2929 0a0a 2020 2020 2320 6d61 6b65 2078  ))..    # make x
-0000ab30: 6d6c 2073 7472 7563 7475 7265 206f 6620  ml structure of 
-0000ab40: 7468 6520 7661 6c69 6420 7661 6c75 6573  the valid values
-0000ab50: 0a20 2020 2070 726f 705f 203d 2065 7472  .    prop_ = etr
-0000ab60: 6565 2e45 6c65 6d65 6e74 280a 2020 2020  ee.Element(.    
-0000ab70: 2020 2020 227b 2573 7d69 6e74 6572 7661      "{%s}interva
-0000ab80: 6c2d 7072 6f70 2220 2520 786d 6c5f 6e61  l-prop" % xml_na
-0000ab90: 6d65 7370 6163 655f 6d61 705b 4e6f 6e65  mespace_map[None
-0000aba0: 5d2c 0a20 2020 2020 2020 206e 616d 653d  ],.        name=
-0000abb0: 6e61 6d65 2c0a 2020 2020 2020 2020 6e73  name,.        ns
-0000abc0: 6d61 703d 786d 6c5f 6e61 6d65 7370 6163  map=xml_namespac
-0000abd0: 655f 6d61 702c 0a20 2020 2029 0a20 2020  e_map,.    ).   
-0000abe0: 206b 7761 7267 7320 3d20 7b22 7065 726d   kwargs = {"perm
-0000abf0: 6973 7369 6f6e 7322 3a20 7661 6c75 652e  issions": value.
-0000ac00: 7065 726d 6973 7369 6f6e 737d 0a20 2020  permissions}.   
-0000ac10: 2069 6620 7661 6c75 652e 636f 6d6d 656e   if value.commen
-0000ac20: 7420 616e 6420 6368 6563 6b5f 6e6f 746e  t and check_notn
-0000ac30: 6128 7661 6c75 652e 636f 6d6d 656e 7429  a(value.comment)
-0000ac40: 3a0a 2020 2020 2020 2020 6b77 6172 6773  :.        kwargs
-0000ac50: 5b22 636f 6d6d 656e 7422 5d20 3d20 7661  ["comment"] = va
-0000ac60: 6c75 652e 636f 6d6d 656e 740a 2020 2020  lue.comment.    
-0000ac70: 7661 6c75 655f 203d 2065 7472 6565 2e45  value_ = etree.E
-0000ac80: 6c65 6d65 6e74 280a 2020 2020 2020 2020  lement(.        
-0000ac90: 227b 2573 7d69 6e74 6572 7661 6c22 2025  "{%s}interval" %
-0000aca0: 2078 6d6c 5f6e 616d 6573 7061 6365 5f6d   xml_namespace_m
-0000acb0: 6170 5b4e 6f6e 655d 2c0a 2020 2020 2020  ap[None],.      
-0000acc0: 2020 2a2a 6b77 6172 6773 2c20 2023 2074    **kwargs,  # t
-0000acd0: 7970 653a 2069 676e 6f72 655b 6172 672d  ype: ignore[arg-
-0000ace0: 7479 7065 5d0a 2020 2020 2020 2020 6e73  type].        ns
-0000acf0: 6d61 703d 786d 6c5f 6e61 6d65 7370 6163  map=xml_namespac
-0000ad00: 655f 6d61 702c 0a20 2020 2029 0a20 2020  e_map,.    ).   
-0000ad10: 2076 616c 7565 5f2e 7465 7874 203d 2073   value_.text = s
-0000ad20: 7472 2876 616c 7565 2e76 616c 7565 290a  tr(value.value).
-0000ad30: 2020 2020 7072 6f70 5f2e 6170 7065 6e64      prop_.append
-0000ad40: 2876 616c 7565 5f29 0a0a 2020 2020 7265  (value_)..    re
-0000ad50: 7475 726e 2070 726f 705f 0a0a 0a64 6566  turn prop_...def
-0000ad60: 206d 616b 655f 6c69 7374 5f70 726f 7028   make_list_prop(
-0000ad70: 0a20 2020 206c 6973 745f 6e61 6d65 3a20  .    list_name: 
-0000ad80: 7374 722c 0a20 2020 206e 616d 653a 2073  str,.    name: s
-0000ad90: 7472 2c0a 2020 2020 7661 6c75 653a 2055  tr,.    value: U
-0000ada0: 6e69 6f6e 5b50 726f 7065 7274 7945 6c65  nion[PropertyEle
-0000adb0: 6d65 6e74 2c20 7374 722c 2049 7465 7261  ment, str, Itera
-0000adc0: 626c 655b 556e 696f 6e5b 5072 6f70 6572  ble[Union[Proper
-0000add0: 7479 456c 656d 656e 742c 2073 7472 5d5d  tyElement, str]]
-0000ade0: 5d2c 0a20 2020 2063 616c 6c69 6e67 5f72  ],.    calling_r
-0000adf0: 6573 6f75 7263 653a 2073 7472 203d 2022  esource: str = "
-0000ae00: 222c 0a29 202d 3e20 6574 7265 652e 5f45  ",.) -> etree._E
-0000ae10: 6c65 6d65 6e74 3a0a 2020 2020 2222 220a  lement:.    """.
-0000ae20: 2020 2020 4d61 6b65 2061 203c 6c69 7374      Make a <list
-0000ae30: 2d70 726f 703e 2066 726f 6d20 6f6e 6520  -prop> from one 
-0000ae40: 6f72 206d 6f72 6520 6c69 7374 206e 6f64  or more list nod
-0000ae50: 6573 2e20 5468 6520 6e61 6d65 2873 2920  es. The name(s) 
-0000ae60: 6f66 2074 6865 206c 6973 7420 6e6f 6465  of the list node
-0000ae70: 2873 2920 6361 6e20 6265 2070 726f 7669  (s) can be provi
-0000ae80: 6465 6420 6173 2073 7472 696e 6720 6f72  ded as string or
-0000ae90: 2061 730a 2020 2020 5072 6f70 6572 7479   as.    Property
-0000aea0: 456c 656d 656e 7420 7769 7468 2061 2073  Element with a s
-0000aeb0: 7472 696e 6720 696e 7369 6465 2e20 4966  tring inside. If
-0000aec0: 2070 726f 7669 6465 6420 6173 2073 7472   provided as str
-0000aed0: 696e 672c 2074 6865 2070 6572 6d69 7373  ing, the permiss
-0000aee0: 696f 6e73 2064 6566 6175 6c74 2074 6f20  ions default to 
-0000aef0: 2270 726f 702d 6465 6661 756c 7422 2e0a  "prop-default"..
-0000af00: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-0000af10: 2020 206c 6973 745f 6e61 6d65 3a20 7468     list_name: th
-0000af20: 6520 6e61 6d65 206f 6620 7468 6520 6c69  e name of the li
-0000af30: 7374 2061 7320 6465 6669 6e65 6420 696e  st as defined in
-0000af40: 2074 6865 206f 6e74 6f0a 2020 2020 2020   the onto.      
-0000af50: 2020 6e61 6d65 3a20 7468 6520 6e61 6d65    name: the name
-0000af60: 206f 6620 7468 6973 2070 726f 7065 7274   of this propert
-0000af70: 7920 6173 2064 6566 696e 6564 2069 6e20  y as defined in 
-0000af80: 7468 6520 6f6e 746f 0a20 2020 2020 2020  the onto.       
-0000af90: 2076 616c 7565 3a20 6f6e 6520 6f72 206d   value: one or m
-0000afa0: 6f72 6520 6e6f 6465 206e 616d 6573 2c20  ore node names, 
-0000afb0: 6173 2073 7472 696e 672f 5072 6f70 6572  as string/Proper
-0000afc0: 7479 456c 656d 656e 742c 206f 7220 6173  tyElement, or as
-0000afd0: 2069 7465 7261 626c 6520 6f66 2073 7472   iterable of str
-0000afe0: 696e 6773 2f50 726f 7065 7274 7945 6c65  ings/PropertyEle
-0000aff0: 6d65 6e74 730a 2020 2020 2020 2020 6361  ments.        ca
-0000b000: 6c6c 696e 675f 7265 736f 7572 6365 3a20  lling_resource: 
-0000b010: 7468 6520 6e61 6d65 206f 6620 7468 6520  the name of the 
-0000b020: 7061 7265 6e74 2072 6573 6f75 7263 6520  parent resource 
-0000b030: 2866 6f72 2062 6574 7465 7220 6572 726f  (for better erro
-0000b040: 7220 6d65 7373 6167 6573 290a 0a20 2020  r messages)..   
-0000b050: 2057 6172 6e73 3a0a 2020 2020 2020 2020   Warns:.        
-0000b060: 4966 2074 6865 206e 616d 6520 6f66 206f  If the name of o
-0000b070: 6e65 206f 6620 7468 6520 6c69 7374 206e  ne of the list n
-0000b080: 6f64 6573 2069 7320 6e6f 7420 6120 7661  odes is not a va
-0000b090: 6c69 6420 7374 7269 6e67 0a0a 2020 2020  lid string..    
-0000b0a0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-0000b0b0: 2061 6e20 6574 7265 652e 5f45 6c65 6d65   an etree._Eleme
-0000b0c0: 6e74 2074 6861 7420 6361 6e20 6265 2061  nt that can be a
-0000b0d0: 7070 656e 6465 6420 746f 2074 6865 2070  ppended to the p
-0000b0e0: 6172 656e 7420 7265 736f 7572 6365 2077  arent resource w
-0000b0f0: 6974 6820 7265 736f 7572 6365 2e61 7070  ith resource.app
-0000b100: 656e 6428 6d61 6b65 5f2a 5f70 726f 7028  end(make_*_prop(
-0000b110: 2e2e 2e29 290a 0a20 2020 2045 7861 6d70  ...))..    Examp
-0000b120: 6c65 733a 0a20 2020 2020 2020 203e 3e3e  les:.        >>>
-0000b130: 2065 7863 656c 3278 6d6c 2e6d 616b 655f   excel2xml.make_
-0000b140: 6c69 7374 5f70 726f 7028 226d 796c 6973  list_prop("mylis
-0000b150: 7422 2c20 223a 7465 7374 7072 6f70 6572  t", ":testproper
-0000b160: 7479 222c 2022 6669 7273 745f 6e6f 6465  ty", "first_node
-0000b170: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-0000b180: 2020 203c 6c69 7374 2d70 726f 7020 6c69     <list-prop li
-0000b190: 7374 3d22 6d79 6c69 7374 2220 6e61 6d65  st="mylist" name
-0000b1a0: 3d22 3a74 6573 7470 726f 7065 7274 7922  =":testproperty"
-0000b1b0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-0000b1c0: 2020 2020 2020 3c6c 6973 7420 7065 726d        <list perm
-0000b1d0: 6973 7369 6f6e 733d 2270 726f 702d 6465  issions="prop-de
-0000b1e0: 6661 756c 7422 3e66 6972 7374 5f6e 6f64  fault">first_nod
-0000b1f0: 653c 2f6c 6973 743e 0a20 2020 2020 2020  e</list>.       
-0000b200: 2020 2020 2020 2020 203c 2f6c 6973 742d           </list-
-0000b210: 7072 6f70 3e0a 2020 2020 2020 2020 3e3e  prop>.        >>
-0000b220: 3e20 6578 6365 6c32 786d 6c2e 6d61 6b65  > excel2xml.make
-0000b230: 5f6c 6973 745f 7072 6f70 2822 6d79 6c69  _list_prop("myli
-0000b240: 7374 222c 2022 3a74 6573 7470 726f 7065  st", ":testprope
-0000b250: 7274 7922 2c20 6578 6365 6c32 786d 6c2e  rty", excel2xml.
-0000b260: 5072 6f70 6572 7479 456c 656d 656e 7428  PropertyElement(
-0000b270: 2266 6972 7374 5f6e 6f64 6522 2c20 7065  "first_node", pe
-0000b280: 726d 6973 7369 6f6e 733d 2270 726f 702d  rmissions="prop-
-0000b290: 7265 7374 7269 6374 6564 222c 2063 6f6d  restricted", com
-0000b2a0: 6d65 6e74 3d22 6578 616d 706c 6522 2929  ment="example"))
-0000b2b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b2c0: 203c 6c69 7374 2d70 726f 7020 6c69 7374   <list-prop list
-0000b2d0: 3d22 6d79 6c69 7374 2220 6e61 6d65 3d22  ="mylist" name="
-0000b2e0: 3a74 6573 7470 726f 7065 7274 7922 3e0a  :testproperty">.
-0000b2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b300: 2020 2020 3c6c 6973 7420 7065 726d 6973      <list permis
-0000b310: 7369 6f6e 733d 2270 726f 702d 7265 7374  sions="prop-rest
-0000b320: 7269 6374 6564 2220 636f 6d6d 656e 743d  ricted" comment=
-0000b330: 2265 7861 6d70 6c65 223e 6669 7273 745f  "example">first_
-0000b340: 6e6f 6465 3c2f 6c69 7374 3e0a 2020 2020  node</list>.    
-0000b350: 2020 2020 2020 2020 2020 2020 3c2f 6c69              </li
-0000b360: 7374 2d70 726f 703e 0a20 2020 2020 2020  st-prop>.       
-0000b370: 203e 3e3e 2065 7863 656c 3278 6d6c 2e6d   >>> excel2xml.m
-0000b380: 616b 655f 6c69 7374 5f70 726f 7028 226d  ake_list_prop("m
-0000b390: 796c 6973 7422 2c20 223a 7465 7374 7072  ylist", ":testpr
-0000b3a0: 6f70 6572 7479 222c 205b 2266 6972 7374  operty", ["first
-0000b3b0: 5f6e 6f64 6522 2c20 2273 6563 6f6e 645f  _node", "second_
-0000b3c0: 6e6f 6465 225d 290a 2020 2020 2020 2020  node"]).        
-0000b3d0: 2020 2020 2020 2020 3c6c 6973 742d 7072          <list-pr
-0000b3e0: 6f70 206c 6973 743d 226d 796c 6973 7422  op list="mylist"
-0000b3f0: 206e 616d 653d 223a 7465 7374 7072 6f70   name=":testprop
-0000b400: 6572 7479 223e 0a20 2020 2020 2020 2020  erty">.         
-0000b410: 2020 2020 2020 2020 2020 203c 6c69 7374             <list
-0000b420: 2070 6572 6d69 7373 696f 6e73 3d22 7072   permissions="pr
-0000b430: 6f70 2d64 6566 6175 6c74 223e 6669 7273  op-default">firs
-0000b440: 745f 6e6f 6465 3c2f 6c69 7374 3e0a 2020  t_node</list>.  
-0000b450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b460: 2020 3c6c 6973 7420 7065 726d 6973 7369    <list permissi
-0000b470: 6f6e 733d 2270 726f 702d 6465 6661 756c  ons="prop-defaul
-0000b480: 7422 3e73 6563 6f6e 645f 6e6f 6465 3c2f  t">second_node</
-0000b490: 6c69 7374 3e0a 2020 2020 2020 2020 2020  list>.          
-0000b4a0: 2020 2020 2020 3c2f 6c69 7374 2d70 726f        </list-pro
-0000b4b0: 703e 0a0a 2020 2020 5365 6520 6874 7470  p>..    See http
-0000b4c0: 733a 2f2f 646f 6373 2e64 6173 6368 2e73  s://docs.dasch.s
-0000b4d0: 7769 7373 2f6c 6174 6573 742f 4453 502d  wiss/latest/DSP-
-0000b4e0: 544f 4f4c 532f 6669 6c65 2d66 6f72 6d61  TOOLS/file-forma
-0000b4f0: 7473 2f78 6d6c 2d64 6174 612d 6669 6c65  ts/xml-data-file
-0000b500: 2f23 6c69 7374 2d70 726f 700a 2020 2020  /#list-prop.    
-0000b510: 2222 220a 0a20 2020 2023 2063 6865 636b  """..    # check
-0000b520: 2074 6865 2069 6e70 7574 3a20 7072 6570   the input: prep
-0000b530: 6172 6520 6120 6c69 7374 2077 6974 6820  are a list with 
-0000b540: 7661 6c69 6420 7661 6c75 6573 0a20 2020  valid values.   
-0000b550: 2076 616c 7565 7320 3d20 7072 6570 6172   values = prepar
-0000b560: 655f 7661 6c75 6528 7661 6c75 6529 0a0a  e_value(value)..
-0000b570: 2020 2020 2320 6368 6563 6b20 7661 6c75      # check valu
-0000b580: 6520 7479 7065 0a20 2020 2066 6f72 2076  e type.    for v
-0000b590: 616c 2069 6e20 7661 6c75 6573 3a0a 2020  al in values:.  
-0000b5a0: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
-0000b5b0: 6e73 7461 6e63 6528 7661 6c2e 7661 6c75  nstance(val.valu
-0000b5c0: 652c 2073 7472 2920 6f72 206e 6f74 2063  e, str) or not c
-0000b5d0: 6865 636b 5f6e 6f74 6e61 2876 616c 2e76  heck_notna(val.v
-0000b5e0: 616c 7565 293a 0a20 2020 2020 2020 2020  alue):.         
-0000b5f0: 2020 206d 7367 203d 2028 0a20 2020 2020     msg = (.     
-0000b600: 2020 2020 2020 2020 2020 2066 2246 6169             f"Fai
-0000b610: 6c65 6420 7661 6c69 6461 7469 6f6e 2069  led validation i
-0000b620: 6e20 7265 736f 7572 6365 2027 7b63 616c  n resource '{cal
-0000b630: 6c69 6e67 5f72 6573 6f75 7263 657d 272c  ling_resource}',
-0000b640: 2070 726f 7065 7274 7920 277b 6e61 6d65   property '{name
-0000b650: 7d27 3a20 220a 2020 2020 2020 2020 2020  }': ".          
-0000b660: 2020 2020 2020 6622 277b 7661 6c2e 7661        f"'{val.va
-0000b670: 6c75 657d 2720 6973 206e 6f74 2061 2076  lue}' is not a v
-0000b680: 616c 6964 206e 616d 6520 6f66 2061 206c  alid name of a l
-0000b690: 6973 7420 6e6f 6465 2e22 0a20 2020 2020  ist node.".     
-0000b6a0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000b6b0: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
-0000b6c0: 726e 2844 7370 546f 6f6c 7355 7365 7257  rn(DspToolsUserW
-0000b6d0: 6172 6e69 6e67 286d 7367 2929 0a0a 2020  arning(msg))..  
-0000b6e0: 2020 2320 6d61 6b65 2078 6d6c 2073 7472    # make xml str
-0000b6f0: 7563 7475 7265 206f 6620 7468 6520 7661  ucture of the va
-0000b700: 6c69 6420 7661 6c75 6573 0a20 2020 2070  lid values.    p
-0000b710: 726f 705f 203d 2065 7472 6565 2e45 6c65  rop_ = etree.Ele
-0000b720: 6d65 6e74 280a 2020 2020 2020 2020 227b  ment(.        "{
-0000b730: 2573 7d6c 6973 742d 7072 6f70 2220 2520  %s}list-prop" % 
-0000b740: 786d 6c5f 6e61 6d65 7370 6163 655f 6d61  xml_namespace_ma
-0000b750: 705b 4e6f 6e65 5d2c 0a20 2020 2020 2020  p[None],.       
-0000b760: 206c 6973 743d 6c69 7374 5f6e 616d 652c   list=list_name,
-0000b770: 0a20 2020 2020 2020 206e 616d 653d 6e61  .        name=na
-0000b780: 6d65 2c0a 2020 2020 2020 2020 6e73 6d61  me,.        nsma
-0000b790: 703d 786d 6c5f 6e61 6d65 7370 6163 655f  p=xml_namespace_
-0000b7a0: 6d61 702c 0a20 2020 2029 0a20 2020 2066  map,.    ).    f
-0000b7b0: 6f72 2076 616c 2069 6e20 7661 6c75 6573  or val in values
-0000b7c0: 3a0a 2020 2020 2020 2020 6b77 6172 6773  :.        kwargs
-0000b7d0: 203d 207b 2270 6572 6d69 7373 696f 6e73   = {"permissions
-0000b7e0: 223a 2076 616c 2e70 6572 6d69 7373 696f  ": val.permissio
-0000b7f0: 6e73 7d0a 2020 2020 2020 2020 6966 2076  ns}.        if v
-0000b800: 616c 2e63 6f6d 6d65 6e74 2061 6e64 2063  al.comment and c
-0000b810: 6865 636b 5f6e 6f74 6e61 2876 616c 2e63  heck_notna(val.c
-0000b820: 6f6d 6d65 6e74 293a 0a20 2020 2020 2020  omment):.       
-0000b830: 2020 2020 206b 7761 7267 735b 2263 6f6d       kwargs["com
-0000b840: 6d65 6e74 225d 203d 2076 616c 2e63 6f6d  ment"] = val.com
-0000b850: 6d65 6e74 0a20 2020 2020 2020 2076 616c  ment.        val
-0000b860: 7565 5f20 3d20 6574 7265 652e 456c 656d  ue_ = etree.Elem
-0000b870: 656e 7428 0a20 2020 2020 2020 2020 2020  ent(.           
-0000b880: 2022 7b25 737d 6c69 7374 2220 2520 786d   "{%s}list" % xm
-0000b890: 6c5f 6e61 6d65 7370 6163 655f 6d61 705b  l_namespace_map[
-0000b8a0: 4e6f 6e65 5d2c 0a20 2020 2020 2020 2020  None],.         
-0000b8b0: 2020 202a 2a6b 7761 7267 732c 2020 2320     **kwargs,  # 
-0000b8c0: 7479 7065 3a20 6967 6e6f 7265 5b61 7267  type: ignore[arg
-0000b8d0: 2d74 7970 655d 0a20 2020 2020 2020 2020  -type].         
-0000b8e0: 2020 206e 736d 6170 3d78 6d6c 5f6e 616d     nsmap=xml_nam
-0000b8f0: 6573 7061 6365 5f6d 6170 2c0a 2020 2020  espace_map,.    
-0000b900: 2020 2020 290a 2020 2020 2020 2020 7661      ).        va
-0000b910: 6c75 655f 2e74 6578 7420 3d20 7374 7228  lue_.text = str(
-0000b920: 7661 6c2e 7661 6c75 6529 0a20 2020 2020  val.value).     
-0000b930: 2020 2070 726f 705f 2e61 7070 656e 6428     prop_.append(
-0000b940: 7661 6c75 655f 290a 0a20 2020 2072 6574  value_)..    ret
-0000b950: 7572 6e20 7072 6f70 5f0a 0a0a 6465 6620  urn prop_...def 
-0000b960: 6d61 6b65 5f72 6573 7074 725f 7072 6f70  make_resptr_prop
-0000b970: 280a 2020 2020 6e61 6d65 3a20 7374 722c  (.    name: str,
-0000b980: 0a20 2020 2076 616c 7565 3a20 556e 696f  .    value: Unio
-0000b990: 6e5b 5072 6f70 6572 7479 456c 656d 656e  n[PropertyElemen
-0000b9a0: 742c 2073 7472 2c20 4974 6572 6162 6c65  t, str, Iterable
-0000b9b0: 5b55 6e69 6f6e 5b50 726f 7065 7274 7945  [Union[PropertyE
-0000b9c0: 6c65 6d65 6e74 2c20 7374 725d 5d5d 2c0a  lement, str]]],.
-0000b9d0: 2020 2020 6361 6c6c 696e 675f 7265 736f      calling_reso
-0000b9e0: 7572 6365 3a20 7374 7220 3d20 2222 2c0a  urce: str = "",.
-0000b9f0: 2920 2d3e 2065 7472 6565 2e5f 456c 656d  ) -> etree._Elem
-0000ba00: 656e 743a 0a20 2020 2022 2222 0a20 2020  ent:.    """.   
-0000ba10: 204d 616b 6520 6120 3c72 6573 7074 722d   Make a <resptr-
-0000ba20: 7072 6f70 3e20 6672 6f6d 206f 6e65 206f  prop> from one o
-0000ba30: 7220 6d6f 7265 2049 4473 206f 6620 6f74  r more IDs of ot
-0000ba40: 6865 7220 7265 736f 7572 6365 732e 2054  her resources. T
-0000ba50: 6865 2049 4428 7329 2063 616e 2062 6520  he ID(s) can be 
-0000ba60: 7072 6f76 6964 6564 2061 7320 7374 7269  provided as stri
-0000ba70: 6e67 206f 7220 6173 0a20 2020 2050 726f  ng or as.    Pro
-0000ba80: 7065 7274 7945 6c65 6d65 6e74 2077 6974  pertyElement wit
-0000ba90: 6820 6120 7374 7269 6e67 2069 6e73 6964  h a string insid
-0000baa0: 652e 2049 6620 7072 6f76 6964 6564 2061  e. If provided a
-0000bab0: 7320 7374 7269 6e67 2c20 7468 6520 7065  s string, the pe
-0000bac0: 726d 6973 7369 6f6e 7320 6465 6661 756c  rmissions defaul
-0000bad0: 7420 746f 2022 7072 6f70 2d64 6566 6175  t to "prop-defau
-0000bae0: 6c74 222e 0a0a 2020 2020 4172 6773 3a0a  lt"...    Args:.
-0000baf0: 2020 2020 2020 2020 6e61 6d65 3a20 7468          name: th
-0000bb00: 6520 6e61 6d65 206f 6620 7468 6973 2070  e name of this p
-0000bb10: 726f 7065 7274 7920 6173 2064 6566 696e  roperty as defin
-0000bb20: 6564 2069 6e20 7468 6520 6f6e 746f 0a20  ed in the onto. 
-0000bb30: 2020 2020 2020 2076 616c 7565 3a20 6f6e         value: on
-0000bb40: 6520 6f72 206d 6f72 6520 7265 736f 7572  e or more resour
-0000bb50: 6365 2069 6465 6e74 6966 6965 7273 2c20  ce identifiers, 
-0000bb60: 6173 2073 7472 696e 672f 5072 6f70 6572  as string/Proper
-0000bb70: 7479 456c 656d 656e 742c 206f 7220 6173  tyElement, or as
-0000bb80: 2069 7465 7261 626c 6520 6f66 2073 7472   iterable of str
-0000bb90: 696e 6773 2f50 726f 7065 7274 7945 6c65  ings/PropertyEle
-0000bba0: 6d65 6e74 730a 2020 2020 2020 2020 6361  ments.        ca
-0000bbb0: 6c6c 696e 675f 7265 736f 7572 6365 3a20  lling_resource: 
-0000bbc0: 7468 6520 6e61 6d65 206f 6620 7468 6520  the name of the 
-0000bbd0: 7061 7265 6e74 2072 6573 6f75 7263 6520  parent resource 
-0000bbe0: 2866 6f72 2062 6574 7465 7220 6572 726f  (for better erro
-0000bbf0: 7220 6d65 7373 6167 6573 290a 0a20 2020  r messages)..   
-0000bc00: 2057 6172 6e73 3a0a 2020 2020 2020 2020   Warns:.        
-0000bc10: 4966 2074 6865 2049 4420 6f66 206f 6e65  If the ID of one
-0000bc20: 206f 6620 7468 6520 7461 7267 6574 2072   of the target r
-0000bc30: 6573 6f75 7263 6573 2069 7320 6e6f 7420  esources is not 
-0000bc40: 6120 7661 6c69 6420 7374 7269 6e67 0a0a  a valid string..
-0000bc50: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-0000bc60: 2020 2020 2061 6e20 6574 7265 652e 5f45       an etree._E
-0000bc70: 6c65 6d65 6e74 2074 6861 7420 6361 6e20  lement that can 
-0000bc80: 6265 2061 7070 656e 6465 6420 746f 2074  be appended to t
-0000bc90: 6865 2070 6172 656e 7420 7265 736f 7572  he parent resour
-0000bca0: 6365 2077 6974 6820 7265 736f 7572 6365  ce with resource
-0000bcb0: 2e61 7070 656e 6428 6d61 6b65 5f2a 5f70  .append(make_*_p
-0000bcc0: 726f 7028 2e2e 2e29 290a 0a20 2020 2045  rop(...))..    E
-0000bcd0: 7861 6d70 6c65 733a 0a20 2020 2020 2020  xamples:.       
-0000bce0: 203e 3e3e 2065 7863 656c 3278 6d6c 2e6d   >>> excel2xml.m
-0000bcf0: 616b 655f 7265 7370 7472 5f70 726f 7028  ake_resptr_prop(
-0000bd00: 223a 7465 7374 7072 6f70 6572 7479 222c  ":testproperty",
-0000bd10: 2022 7265 736f 7572 6365 5f31 2229 0a20   "resource_1"). 
-0000bd20: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000bd30: 7265 7370 7472 2d70 726f 7020 6e61 6d65  resptr-prop name
-0000bd40: 3d22 3a74 6573 7470 726f 7065 7274 7922  =":testproperty"
-0000bd50: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-0000bd60: 2020 2020 2020 3c72 6573 7074 7220 7065        <resptr pe
-0000bd70: 726d 6973 7369 6f6e 733d 2270 726f 702d  rmissions="prop-
-0000bd80: 6465 6661 756c 7422 3e72 6573 6f75 7263  default">resourc
-0000bd90: 655f 313c 2f72 6573 7074 723e 0a20 2020  e_1</resptr>.   
-0000bda0: 2020 2020 2020 2020 2020 2020 203c 2f72               </r
-0000bdb0: 6573 7074 722d 7072 6f70 3e0a 2020 2020  esptr-prop>.    
-0000bdc0: 2020 2020 3e3e 3e20 6578 6365 6c32 786d      >>> excel2xm
-0000bdd0: 6c2e 6d61 6b65 5f72 6573 7074 725f 7072  l.make_resptr_pr
-0000bde0: 6f70 2822 3a74 6573 7470 726f 7065 7274  op(":testpropert
-0000bdf0: 7922 2c20 6578 6365 6c32 786d 6c2e 5072  y", excel2xml.Pr
-0000be00: 6f70 6572 7479 456c 656d 656e 7428 2272  opertyElement("r
-0000be10: 6573 6f75 7263 655f 3122 2c20 7065 726d  esource_1", perm
-0000be20: 6973 7369 6f6e 733d 2270 726f 702d 7265  issions="prop-re
-0000be30: 7374 7269 6374 6564 222c 2063 6f6d 6d65  stricted", comme
-0000be40: 6e74 3d22 6578 616d 706c 6522 2929 0a20  nt="example")). 
-0000be50: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000be60: 7265 7370 7472 2d70 726f 7020 6e61 6d65  resptr-prop name
-0000be70: 3d22 3a74 6573 7470 726f 7065 7274 7922  =":testproperty"
-0000be80: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-0000be90: 2020 2020 2020 3c72 6573 7074 7220 7065        <resptr pe
-0000bea0: 726d 6973 7369 6f6e 733d 2270 726f 702d  rmissions="prop-
-0000beb0: 7265 7374 7269 6374 6564 2220 636f 6d6d  restricted" comm
-0000bec0: 656e 743d 2265 7861 6d70 6c65 223e 7265  ent="example">re
-0000bed0: 736f 7572 6365 5f31 3c2f 7265 7370 7472  source_1</resptr
-0000bee0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-0000bef0: 2020 3c2f 7265 7370 7472 2d70 726f 703e    </resptr-prop>
-0000bf00: 0a20 2020 2020 2020 203e 3e3e 2065 7863  .        >>> exc
-0000bf10: 656c 3278 6d6c 2e6d 616b 655f 7265 7370  el2xml.make_resp
-0000bf20: 7472 5f70 726f 7028 223a 7465 7374 7072  tr_prop(":testpr
-0000bf30: 6f70 6572 7479 222c 205b 2272 6573 6f75  operty", ["resou
-0000bf40: 7263 655f 3122 2c20 2272 6573 6f75 7263  rce_1", "resourc
-0000bf50: 655f 3222 5d29 0a20 2020 2020 2020 2020  e_2"]).         
-0000bf60: 2020 2020 2020 203c 7265 7370 7472 2d70         <resptr-p
-0000bf70: 726f 7020 6e61 6d65 3d22 3a74 6573 7470  rop name=":testp
-0000bf80: 726f 7065 7274 7922 3e0a 2020 2020 2020  roperty">.      
-0000bf90: 2020 2020 2020 2020 2020 2020 2020 3c72                <r
-0000bfa0: 6573 7074 7220 7065 726d 6973 7369 6f6e  esptr permission
-0000bfb0: 733d 2270 726f 702d 6465 6661 756c 7422  s="prop-default"
-0000bfc0: 3e72 6573 6f75 7263 655f 313c 2f72 6573  >resource_1</res
-0000bfd0: 7074 723e 0a20 2020 2020 2020 2020 2020  ptr>.           
-0000bfe0: 2020 2020 2020 2020 203c 7265 7370 7472           <resptr
-0000bff0: 2070 6572 6d69 7373 696f 6e73 3d22 7072   permissions="pr
-0000c000: 6f70 2d64 6566 6175 6c74 223e 7265 736f  op-default">reso
-0000c010: 7572 6365 5f32 3c2f 7265 7370 7472 3e0a  urce_2</resptr>.
-0000c020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c030: 3c2f 7265 7370 7472 2d70 726f 703e 0a0a  </resptr-prop>..
-0000c040: 2020 2020 5365 6520 6874 7470 733a 2f2f      See https://
-0000c050: 646f 6373 2e64 6173 6368 2e73 7769 7373  docs.dasch.swiss
-0000c060: 2f6c 6174 6573 742f 4453 502d 544f 4f4c  /latest/DSP-TOOL
-0000c070: 532f 6669 6c65 2d66 6f72 6d61 7473 2f78  S/file-formats/x
-0000c080: 6d6c 2d64 6174 612d 6669 6c65 2f23 7265  ml-data-file/#re
-0000c090: 7370 7472 2d70 726f 700a 2020 2020 2222  sptr-prop.    ""
-0000c0a0: 220a 0a20 2020 2023 2063 6865 636b 2074  "..    # check t
-0000c0b0: 6865 2069 6e70 7574 3a20 7072 6570 6172  he input: prepar
-0000c0c0: 6520 6120 6c69 7374 2077 6974 6820 7661  e a list with va
-0000c0d0: 6c69 6420 7661 6c75 6573 0a20 2020 2076  lid values.    v
-0000c0e0: 616c 7565 7320 3d20 7072 6570 6172 655f  alues = prepare_
-0000c0f0: 7661 6c75 6528 7661 6c75 6529 0a0a 2020  value(value)..  
-0000c100: 2020 2320 6368 6563 6b20 7661 6c75 6520    # check value 
-0000c110: 7479 7065 0a20 2020 2066 6f72 2076 616c  type.    for val
-0000c120: 2069 6e20 7661 6c75 6573 3a0a 2020 2020   in values:.    
-0000c130: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
-0000c140: 7461 6e63 6528 7661 6c2e 7661 6c75 652c  tance(val.value,
-0000c150: 2073 7472 2920 6f72 206e 6f74 2063 6865   str) or not che
-0000c160: 636b 5f6e 6f74 6e61 2876 616c 2e76 616c  ck_notna(val.val
-0000c170: 7565 293a 0a20 2020 2020 2020 2020 2020  ue):.           
-0000c180: 206d 7367 203d 2028 0a20 2020 2020 2020   msg = (.       
-0000c190: 2020 2020 2020 2020 2066 2256 616c 6964           f"Valid
-0000c1a0: 6174 696f 6e20 4572 726f 7220 696e 2072  ation Error in r
-0000c1b0: 6573 6f75 7263 6520 277b 6361 6c6c 696e  esource '{callin
-0000c1c0: 675f 7265 736f 7572 6365 7d27 2c20 7072  g_resource}', pr
-0000c1d0: 6f70 6572 7479 2027 7b6e 616d 657d 273a  operty '{name}':
-0000c1e0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-0000c1f0: 2020 2066 2254 6865 2066 6f6c 6c6f 7769     f"The followi
-0000c200: 6e67 2064 6f65 736e 2774 2073 6565 6d20  ng doesn't seem 
-0000c210: 746f 2062 6520 6120 7661 6c69 6420 4944  to be a valid ID
-0000c220: 206f 6620 6120 7461 7267 6574 2072 6573   of a target res
-0000c230: 6f75 7263 653a 2027 7b76 616c 2e76 616c  ource: '{val.val
-0000c240: 7565 7d27 220a 2020 2020 2020 2020 2020  ue}'".          
-0000c250: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0000c260: 7761 726e 696e 6773 2e77 6172 6e28 4473  warnings.warn(Ds
-0000c270: 7054 6f6f 6c73 5573 6572 5761 726e 696e  pToolsUserWarnin
-0000c280: 6728 6d73 6729 290a 0a20 2020 2023 206d  g(msg))..    # m
-0000c290: 616b 6520 786d 6c20 7374 7275 6374 7572  ake xml structur
-0000c2a0: 6520 6f66 2074 6865 2076 616c 6964 2076  e of the valid v
-0000c2b0: 616c 7565 730a 2020 2020 7072 6f70 5f20  alues.    prop_ 
-0000c2c0: 3d20 6574 7265 652e 456c 656d 656e 7428  = etree.Element(
-0000c2d0: 0a20 2020 2020 2020 2022 7b25 737d 7265  .        "{%s}re
-0000c2e0: 7370 7472 2d70 726f 7022 2025 2078 6d6c  sptr-prop" % xml
-0000c2f0: 5f6e 616d 6573 7061 6365 5f6d 6170 5b4e  _namespace_map[N
-0000c300: 6f6e 655d 2c0a 2020 2020 2020 2020 6e61  one],.        na
-0000c310: 6d65 3d6e 616d 652c 0a20 2020 2020 2020  me=name,.       
-0000c320: 206e 736d 6170 3d78 6d6c 5f6e 616d 6573   nsmap=xml_names
-0000c330: 7061 6365 5f6d 6170 2c0a 2020 2020 290a  pace_map,.    ).
-0000c340: 2020 2020 666f 7220 7661 6c20 696e 2076      for val in v
-0000c350: 616c 7565 733a 0a20 2020 2020 2020 206b  alues:.        k
-0000c360: 7761 7267 7320 3d20 7b22 7065 726d 6973  wargs = {"permis
-0000c370: 7369 6f6e 7322 3a20 7661 6c2e 7065 726d  sions": val.perm
-0000c380: 6973 7369 6f6e 737d 0a20 2020 2020 2020  issions}.       
-0000c390: 2069 6620 7661 6c2e 636f 6d6d 656e 7420   if val.comment 
-0000c3a0: 616e 6420 6368 6563 6b5f 6e6f 746e 6128  and check_notna(
-0000c3b0: 7661 6c2e 636f 6d6d 656e 7429 3a0a 2020  val.comment):.  
-0000c3c0: 2020 2020 2020 2020 2020 6b77 6172 6773            kwargs
-0000c3d0: 5b22 636f 6d6d 656e 7422 5d20 3d20 7661  ["comment"] = va
-0000c3e0: 6c2e 636f 6d6d 656e 740a 2020 2020 2020  l.comment.      
-0000c3f0: 2020 7661 6c75 655f 203d 2065 7472 6565    value_ = etree
-0000c400: 2e45 6c65 6d65 6e74 280a 2020 2020 2020  .Element(.      
-0000c410: 2020 2020 2020 227b 2573 7d72 6573 7074        "{%s}respt
-0000c420: 7222 2025 2078 6d6c 5f6e 616d 6573 7061  r" % xml_namespa
-0000c430: 6365 5f6d 6170 5b4e 6f6e 655d 2c0a 2020  ce_map[None],.  
-0000c440: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
-0000c450: 6773 2c20 2023 2074 7970 653a 2069 676e  gs,  # type: ign
-0000c460: 6f72 655b 6172 672d 7479 7065 5d0a 2020  ore[arg-type].  
-0000c470: 2020 2020 2020 2020 2020 6e73 6d61 703d            nsmap=
-0000c480: 786d 6c5f 6e61 6d65 7370 6163 655f 6d61  xml_namespace_ma
-0000c490: 702c 0a20 2020 2020 2020 2029 0a20 2020  p,.        ).   
-0000c4a0: 2020 2020 2076 616c 7565 5f2e 7465 7874       value_.text
-0000c4b0: 203d 2073 7472 2876 616c 2e76 616c 7565   = str(val.value
-0000c4c0: 290a 2020 2020 2020 2020 7072 6f70 5f2e  ).        prop_.
-0000c4d0: 6170 7065 6e64 2876 616c 7565 5f29 0a0a  append(value_)..
-0000c4e0: 2020 2020 7265 7475 726e 2070 726f 705f      return prop_
-0000c4f0: 0a0a 0a64 6566 206d 616b 655f 7465 7874  ...def make_text
-0000c500: 5f70 726f 7028 0a20 2020 206e 616d 653a  _prop(.    name:
-0000c510: 2073 7472 2c0a 2020 2020 7661 6c75 653a   str,.    value:
-0000c520: 2055 6e69 6f6e 5b50 726f 7065 7274 7945   Union[PropertyE
-0000c530: 6c65 6d65 6e74 2c20 7374 722c 2049 7465  lement, str, Ite
-0000c540: 7261 626c 655b 556e 696f 6e5b 5072 6f70  rable[Union[Prop
-0000c550: 6572 7479 456c 656d 656e 742c 2073 7472  ertyElement, str
-0000c560: 5d5d 5d2c 0a20 2020 2063 616c 6c69 6e67  ]]],.    calling
-0000c570: 5f72 6573 6f75 7263 653a 2073 7472 203d  _resource: str =
-0000c580: 2022 222c 0a29 202d 3e20 6574 7265 652e   "",.) -> etree.
-0000c590: 5f45 6c65 6d65 6e74 3a0a 2020 2020 2222  _Element:.    ""
-0000c5a0: 220a 2020 2020 4d61 6b65 2061 203c 7465  ".    Make a <te
-0000c5b0: 7874 2d70 726f 703e 2066 726f 6d20 6f6e  xt-prop> from on
-0000c5c0: 6520 6f72 206d 6f72 6520 7374 7269 6e67  e or more string
-0000c5d0: 732e 2054 6865 2073 7472 696e 6728 7329  s. The string(s)
-0000c5e0: 2063 616e 2062 6520 7072 6f76 6964 6564   can be provided
-0000c5f0: 2061 7320 7374 7269 6e67 206f 7220 6173   as string or as
-0000c600: 2050 726f 7065 7274 7945 6c65 6d65 6e74   PropertyElement
-0000c610: 2077 6974 6820 610a 2020 2020 7374 7269   with a.    stri
-0000c620: 6e67 2069 6e73 6964 652e 2049 6620 7072  ng inside. If pr
-0000c630: 6f76 6964 6564 2061 7320 7374 7269 6e67  ovided as string
-0000c640: 2c20 7468 6520 656e 636f 6469 6e67 2064  , the encoding d
-0000c650: 6566 6175 6c74 7320 746f 2075 7466 382c  efaults to utf8,
-0000c660: 2061 6e64 2074 6865 2070 6572 6d69 7373   and the permiss
-0000c670: 696f 6e73 2074 6f20 2270 726f 702d 6465  ions to "prop-de
-0000c680: 6661 756c 7422 2e0a 0a20 2020 2041 7267  fault"...    Arg
-0000c690: 733a 0a20 2020 2020 2020 206e 616d 653a  s:.        name:
-0000c6a0: 2074 6865 206e 616d 6520 6f66 2074 6869   the name of thi
-0000c6b0: 7320 7072 6f70 6572 7479 2061 7320 6465  s property as de
-0000c6c0: 6669 6e65 6420 696e 2074 6865 206f 6e74  fined in the ont
-0000c6d0: 6f0a 2020 2020 2020 2020 7661 6c75 653a  o.        value:
-0000c6e0: 206f 6e65 206f 7220 6d6f 7265 2073 7472   one or more str
-0000c6f0: 696e 6773 2c20 6173 2073 7472 696e 672f  ings, as string/
-0000c700: 5072 6f70 6572 7479 456c 656d 656e 742c  PropertyElement,
-0000c710: 206f 7220 6173 2069 7465 7261 626c 6520   or as iterable 
-0000c720: 6f66 2073 7472 696e 6773 2f50 726f 7065  of strings/Prope
-0000c730: 7274 7945 6c65 6d65 6e74 730a 2020 2020  rtyElements.    
-0000c740: 2020 2020 6361 6c6c 696e 675f 7265 736f      calling_reso
-0000c750: 7572 6365 3a20 7468 6520 6e61 6d65 206f  urce: the name o
-0000c760: 6620 7468 6520 7061 7265 6e74 2072 6573  f the parent res
-0000c770: 6f75 7263 6520 2866 6f72 2062 6574 7465  ource (for bette
-0000c780: 7220 6572 726f 7220 6d65 7373 6167 6573  r error messages
-0000c790: 290a 0a20 2020 2052 6169 7365 733a 0a20  )..    Raises:. 
-0000c7a0: 2020 2020 2020 2042 6173 6545 7272 6f72         BaseError
-0000c7b0: 3a20 6966 2074 6865 2058 4d4c 2074 6167  : if the XML tag
-0000c7c0: 7320 696e 2061 2072 6963 6874 6578 7420  s in a richtext 
-0000c7d0: 7072 6f70 6572 7479 2028 656e 636f 6469  property (encodi
-0000c7e0: 6e67 3d78 6d6c 2920 6172 6520 6e6f 7420  ng=xml) are not 
-0000c7f0: 7765 6c6c 2d66 6f72 6d65 640a 2020 2020  well-formed.    
-0000c800: 2020 2020 5761 726e 696e 673a 2069 6620      Warning: if 
-0000c810: 6f6e 6520 6f66 2074 6865 2076 616c 7565  one of the value
-0000c820: 7320 646f 6573 6e27 7420 6c6f 6f6b 206c  s doesn't look l
-0000c830: 696b 6520 6120 7265 6173 6f6e 6162 6c65  ike a reasonable
-0000c840: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
-0000c850: 2020 2020 2865 2e67 2e20 223c 4e41 3e22      (e.g. "<NA>"
-0000c860: 2069 7320 6120 7661 6c69 6420 7374 7269   is a valid stri
-0000c870: 6e67 2c20 6275 7420 7072 6f62 6162 6c79  ng, but probably
-0000c880: 206e 6f74 2069 6e74 656e 6465 6429 0a0a   not intended)..
-0000c890: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-0000c8a0: 2020 2020 2061 6e20 6574 7265 652e 5f45       an etree._E
-0000c8b0: 6c65 6d65 6e74 2074 6861 7420 6361 6e20  lement that can 
-0000c8c0: 6265 2061 7070 656e 6465 6420 746f 2074  be appended to t
-0000c8d0: 6865 2070 6172 656e 7420 7265 736f 7572  he parent resour
-0000c8e0: 6365 2077 6974 6820 7265 736f 7572 6365  ce with resource
-0000c8f0: 2e61 7070 656e 6428 6d61 6b65 5f2a 5f70  .append(make_*_p
-0000c900: 726f 7028 2e2e 2e29 290a 0a20 2020 2045  rop(...))..    E
-0000c910: 7861 6d70 6c65 733a 0a20 2020 2020 2020  xamples:.       
-0000c920: 203e 3e3e 2065 7863 656c 3278 6d6c 2e6d   >>> excel2xml.m
-0000c930: 616b 655f 7465 7874 5f70 726f 7028 223a  ake_text_prop(":
-0000c940: 7465 7374 7072 6f70 6572 7479 222c 2022  testproperty", "
-0000c950: 6669 7273 7420 7465 7874 2229 0a20 2020  first text").   
-0000c960: 2020 2020 2020 2020 2020 2020 203c 7465               <te
-0000c970: 7874 2d70 726f 7020 6e61 6d65 3d22 3a74  xt-prop name=":t
-0000c980: 6573 7470 726f 7065 7274 7922 3e0a 2020  estproperty">.  
-0000c990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9a0: 2020 3c74 6578 7420 656e 636f 6469 6e67    <text encoding
-0000c9b0: 3d22 7574 6638 2220 7065 726d 6973 7369  ="utf8" permissi
-0000c9c0: 6f6e 733d 2270 726f 702d 6465 6661 756c  ons="prop-defaul
-0000c9d0: 7422 3e66 6972 7374 2074 6578 743c 2f74  t">first text</t
-0000c9e0: 6578 743e 0a20 2020 2020 2020 2020 2020  ext>.           
-0000c9f0: 2020 2020 203c 2f74 6578 742d 7072 6f70       </text-prop
-0000ca00: 3e0a 2020 2020 2020 2020 3e3e 3e20 6578  >.        >>> ex
-0000ca10: 6365 6c32 786d 6c2e 6d61 6b65 5f74 6578  cel2xml.make_tex
-0000ca20: 745f 7072 6f70 2822 3a74 6573 7470 726f  t_prop(":testpro
-0000ca30: 7065 7274 7922 2c20 6578 6365 6c32 786d  perty", excel2xm
-0000ca40: 6c2e 5072 6f70 6572 7479 456c 656d 656e  l.PropertyElemen
-0000ca50: 7428 2266 6972 7374 2074 6578 7422 2c20  t("first text", 
-0000ca60: 7065 726d 6973 7369 6f6e 733d 2270 726f  permissions="pro
-0000ca70: 702d 7265 7374 7269 6374 6564 222c 2065  p-restricted", e
-0000ca80: 6e63 6f64 696e 673d 2278 6d6c 2229 290a  ncoding="xml")).
-0000ca90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000caa0: 3c74 6578 742d 7072 6f70 206e 616d 653d  <text-prop name=
-0000cab0: 223a 7465 7374 7072 6f70 6572 7479 223e  ":testproperty">
-0000cac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cad0: 2020 2020 203c 7465 7874 2065 6e63 6f64       <text encod
-0000cae0: 696e 673d 2278 6d6c 2220 7065 726d 6973  ing="xml" permis
-0000caf0: 7369 6f6e 733d 2270 726f 702d 7265 7374  sions="prop-rest
-0000cb00: 7269 6374 6564 223e 6669 7273 7420 7465  ricted">first te
-0000cb10: 7874 3c2f 7465 7874 3e0a 2020 2020 2020  xt</text>.      
-0000cb20: 2020 2020 2020 2020 2020 3c2f 7465 7874            </text
-0000cb30: 2d70 726f 703e 0a20 2020 2020 2020 203e  -prop>.        >
-0000cb40: 3e3e 2065 7863 656c 3278 6d6c 2e6d 616b  >> excel2xml.mak
-0000cb50: 655f 7465 7874 5f70 726f 7028 223a 7465  e_text_prop(":te
-0000cb60: 7374 7072 6f70 6572 7479 222c 205b 2266  stproperty", ["f
-0000cb70: 6972 7374 2074 6578 7422 2c20 2273 6563  irst text", "sec
-0000cb80: 6f6e 6420 7465 7874 225d 290a 2020 2020  ond text"]).    
-0000cb90: 2020 2020 2020 2020 2020 2020 3c74 6578              <tex
-0000cba0: 742d 7072 6f70 206e 616d 653d 223a 7465  t-prop name=":te
-0000cbb0: 7374 7072 6f70 6572 7479 223e 0a20 2020  stproperty">.   
-0000cbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cbd0: 203c 7465 7874 2065 6e63 6f64 696e 673d   <text encoding=
-0000cbe0: 2275 7466 3822 2070 6572 6d69 7373 696f  "utf8" permissio
-0000cbf0: 6e73 3d22 7072 6f70 2d64 6566 6175 6c74  ns="prop-default
-0000cc00: 223e 6669 7273 7420 7465 7874 3c2f 7465  ">first text</te
-0000cc10: 7874 3e0a 2020 2020 2020 2020 2020 2020  xt>.            
-0000cc20: 2020 2020 2020 2020 3c74 6578 7420 656e          <text en
-0000cc30: 636f 6469 6e67 3d22 7574 6638 2220 7065  coding="utf8" pe
-0000cc40: 726d 6973 7369 6f6e 733d 2270 726f 702d  rmissions="prop-
-0000cc50: 6465 6661 756c 7422 3e73 6563 6f6e 6420  default">second 
-0000cc60: 7465 7874 3c2f 7465 7874 3e0a 2020 2020  text</text>.    
-0000cc70: 2020 2020 2020 2020 2020 2020 3c2f 7465              </te
-0000cc80: 7874 2d70 726f 703e 0a0a 2020 2020 5365  xt-prop>..    Se
-0000cc90: 6520 6874 7470 733a 2f2f 646f 6373 2e64  e https://docs.d
-0000cca0: 6173 6368 2e73 7769 7373 2f6c 6174 6573  asch.swiss/lates
-0000ccb0: 742f 4453 502d 544f 4f4c 532f 6669 6c65  t/DSP-TOOLS/file
-0000ccc0: 2d66 6f72 6d61 7473 2f78 6d6c 2d64 6174  -formats/xml-dat
-0000ccd0: 612d 6669 6c65 2f23 7465 7874 2d70 726f  a-file/#text-pro
-0000cce0: 700a 2020 2020 2222 220a 0a20 2020 2023  p.    """..    #
-0000ccf0: 2063 6865 636b 2074 6865 2069 6e70 7574   check the input
-0000cd00: 3a20 7072 6570 6172 6520 6120 6c69 7374  : prepare a list
-0000cd10: 2077 6974 6820 7661 6c69 6420 7661 6c75   with valid valu
-0000cd20: 6573 0a20 2020 2076 616c 7565 7320 3d20  es.    values = 
-0000cd30: 7072 6570 6172 655f 7661 6c75 6528 7661  prepare_value(va
-0000cd40: 6c75 6529 0a0a 2020 2020 2320 6368 6563  lue)..    # chec
-0000cd50: 6b20 7661 6c75 6520 7479 7065 0a20 2020  k value type.   
-0000cd60: 2066 6f72 2076 616c 2069 6e20 7661 6c75   for val in valu
-0000cd70: 6573 3a0a 2020 2020 2020 2020 6966 206e  es:.        if n
-0000cd80: 6f74 2069 7369 6e73 7461 6e63 6528 7661  ot isinstance(va
-0000cd90: 6c2e 7661 6c75 652c 2073 7472 2920 6f72  l.value, str) or
-0000cda0: 206e 6f74 2063 6865 636b 5f6e 6f74 6e61   not check_notna
-0000cdb0: 2876 616c 2e76 616c 7565 293a 0a20 2020  (val.value):.   
-0000cdc0: 2020 2020 2020 2020 206d 7367 203d 2028           msg = (
-0000cdd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cde0: 2066 2246 6169 6c65 6420 7661 6c69 6461   f"Failed valida
-0000cdf0: 7469 6f6e 2069 6e20 7265 736f 7572 6365  tion in resource
-0000ce00: 2027 7b63 616c 6c69 6e67 5f72 6573 6f75   '{calling_resou
-0000ce10: 7263 657d 272c 2070 726f 7065 7274 7920  rce}', property 
-0000ce20: 277b 6e61 6d65 7d27 3a20 220a 2020 2020  '{name}': ".    
-0000ce30: 2020 2020 2020 2020 2020 2020 6622 277b              f"'{
-0000ce40: 7661 6c2e 7661 6c75 657d 2720 6973 2070  val.value}' is p
-0000ce50: 726f 6261 626c 7920 6e6f 7420 6120 7573  robably not a us
-0000ce60: 6162 6c65 2073 7472 696e 672e 220a 2020  able string.".  
-0000ce70: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000ce80: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
-0000ce90: 2e77 6172 6e28 4473 7054 6f6f 6c73 5573  .warn(DspToolsUs
-0000cea0: 6572 5761 726e 696e 6728 6d73 6729 290a  erWarning(msg)).
-0000ceb0: 0a20 2020 2023 206d 616b 6520 786d 6c20  .    # make xml 
-0000cec0: 7374 7275 6374 7572 6520 6f66 2074 6865  structure of the
-0000ced0: 2076 616c 6964 2076 616c 7565 730a 2020   valid values.  
-0000cee0: 2020 7072 6f70 5f20 3d20 6574 7265 652e    prop_ = etree.
-0000cef0: 456c 656d 656e 7428 0a20 2020 2020 2020  Element(.       
-0000cf00: 2022 7b25 737d 7465 7874 2d70 726f 7022   "{%s}text-prop"
-0000cf10: 2025 2078 6d6c 5f6e 616d 6573 7061 6365   % xml_namespace
-0000cf20: 5f6d 6170 5b4e 6f6e 655d 2c0a 2020 2020  _map[None],.    
-0000cf30: 2020 2020 6e61 6d65 3d6e 616d 652c 0a20      name=name,. 
-0000cf40: 2020 2020 2020 206e 736d 6170 3d78 6d6c         nsmap=xml
-0000cf50: 5f6e 616d 6573 7061 6365 5f6d 6170 2c0a  _namespace_map,.
-0000cf60: 2020 2020 290a 2020 2020 666f 7220 7661      ).    for va
-0000cf70: 6c20 696e 2076 616c 7565 733a 0a20 2020  l in values:.   
-0000cf80: 2020 2020 206b 7761 7267 7320 3d20 7b22       kwargs = {"
-0000cf90: 7065 726d 6973 7369 6f6e 7322 3a20 7661  permissions": va
-0000cfa0: 6c2e 7065 726d 6973 7369 6f6e 737d 0a20  l.permissions}. 
-0000cfb0: 2020 2020 2020 2069 6620 6368 6563 6b5f         if check_
-0000cfc0: 6e6f 746e 6128 7661 6c2e 636f 6d6d 656e  notna(val.commen
-0000cfd0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-0000cfe0: 6b77 6172 6773 5b22 636f 6d6d 656e 7422  kwargs["comment"
-0000cff0: 5d20 3d20 7661 6c2e 636f 6d6d 656e 740a  ] = val.comment.
-0000d000: 2020 2020 2020 2020 6b77 6172 6773 5b22          kwargs["
-0000d010: 656e 636f 6469 6e67 225d 203d 2076 616c  encoding"] = val
-0000d020: 2e65 6e63 6f64 696e 6720 6966 2063 6865  .encoding if che
-0000d030: 636b 5f6e 6f74 6e61 2876 616c 2e65 6e63  ck_notna(val.enc
-0000d040: 6f64 696e 6729 2065 6c73 6520 2275 7466  oding) else "utf
-0000d050: 3822 0a20 2020 2020 2020 2076 616c 7565  8".        value
-0000d060: 5f20 3d20 6574 7265 652e 456c 656d 656e  _ = etree.Elemen
-0000d070: 7428 0a20 2020 2020 2020 2020 2020 2022  t(.            "
-0000d080: 7b25 737d 7465 7874 2220 2520 786d 6c5f  {%s}text" % xml_
-0000d090: 6e61 6d65 7370 6163 655f 6d61 705b 4e6f  namespace_map[No
-0000d0a0: 6e65 5d2c 0a20 2020 2020 2020 2020 2020  ne],.           
-0000d0b0: 202a 2a6b 7761 7267 732c 2020 2320 7479   **kwargs,  # ty
-0000d0c0: 7065 3a20 6967 6e6f 7265 5b61 7267 2d74  pe: ignore[arg-t
-0000d0d0: 7970 655d 0a20 2020 2020 2020 2020 2020  ype].           
-0000d0e0: 206e 736d 6170 3d78 6d6c 5f6e 616d 6573   nsmap=xml_names
-0000d0f0: 7061 6365 5f6d 6170 2c0a 2020 2020 2020  pace_map,.      
-0000d100: 2020 290a 2020 2020 2020 2020 6966 206b    ).        if k
-0000d110: 7761 7267 735b 2265 6e63 6f64 696e 6722  wargs["encoding"
-0000d120: 5d20 3d3d 2022 7574 6638 223a 0a20 2020  ] == "utf8":.   
-0000d130: 2020 2020 2020 2020 2023 2077 7269 7465           # write
-0000d140: 2074 6865 2074 6578 7420 696e 746f 2074   the text into t
-0000d150: 6865 2074 6167 2c20 7769 7468 6f75 7420  he tag, without 
-0000d160: 7661 6c69 6461 7469 6f6e 0a20 2020 2020  validation.     
-0000d170: 2020 2020 2020 2076 616c 7565 5f2e 7465         value_.te
-0000d180: 7874 203d 2073 7472 2876 616c 2e76 616c  xt = str(val.val
-0000d190: 7565 290a 2020 2020 2020 2020 656c 7365  ue).        else
-0000d1a0: 3a0a 2020 2020 2020 2020 2020 2020 6573  :.            es
-0000d1b0: 6361 7065 645f 7465 7874 203d 205f 6573  caped_text = _es
-0000d1c0: 6361 7065 5f72 6573 6572 7665 645f 6368  cape_reserved_ch
-0000d1d0: 6172 7328 7374 7228 7661 6c2e 7661 6c75  ars(str(val.valu
-0000d1e0: 6529 290a 2020 2020 2020 2020 2020 2020  e)).            
-0000d1f0: 2320 656e 666f 7263 6520 7468 6174 2074  # enforce that t
-0000d200: 6865 2074 6578 7420 6973 2077 656c 6c2d  he text is well-
-0000d210: 666f 726d 6564 2058 4d4c 3a20 7365 7269  formed XML: seri
-0000d220: 616c 697a 6520 7461 6720 2e2e 2e0a 2020  alize tag ....  
-0000d230: 2020 2020 2020 2020 2020 7365 7269 616c            serial
-0000d240: 697a 6564 203d 2065 7472 6565 2e74 6f73  ized = etree.tos
-0000d250: 7472 696e 6728 7661 6c75 655f 2c20 656e  tring(value_, en
-0000d260: 636f 6469 6e67 3d22 756e 6963 6f64 6522  coding="unicode"
-0000d270: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
-0000d280: 2e2e 2e20 696e 7365 7274 2074 6578 7420  ... insert text 
-0000d290: 6174 2074 6865 2076 6572 7920 656e 6420  at the very end 
-0000d2a0: 6f66 2074 6865 2073 7472 696e 672c 2061  of the string, a
-0000d2b0: 6e64 2061 6464 2065 6e64 696e 6720 7461  nd add ending ta
-0000d2c0: 6720 746f 2074 6865 2070 7265 7669 6f75  g to the previou
-0000d2d0: 736c 7920 7369 6e67 6c65 203c 7465 7874  sly single <text
-0000d2e0: 2f3e 2074 6167 202e 2e2e 0a20 2020 2020  /> tag ....     
-0000d2f0: 2020 2020 2020 2073 6572 6961 6c69 7a65         serialize
-0000d300: 6420 3d20 7265 6765 782e 7375 6228 7222  d = regex.sub(r"
-0000d310: 2f3e 2422 2c20 6622 3e7b 6573 6361 7065  />$", f">{escape
-0000d320: 645f 7465 7874 7d3c 2f74 6578 743e 222c  d_text}</text>",
-0000d330: 2073 6572 6961 6c69 7a65 6429 0a20 2020   serialized).   
-0000d340: 2020 2020 2020 2020 2023 202e 2e2e 2074           # ... t
-0000d350: 7279 2074 6f20 7061 7273 6520 6974 2061  ry to parse it a
-0000d360: 6761 696e 0a20 2020 2020 2020 2020 2020  gain.           
-0000d370: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-0000d380: 2020 2020 2020 7661 6c75 655f 203d 2065        value_ = e
-0000d390: 7472 6565 2e66 726f 6d73 7472 696e 6728  tree.fromstring(
-0000d3a0: 7365 7269 616c 697a 6564 290a 2020 2020  serialized).    
-0000d3b0: 2020 2020 2020 2020 6578 6365 7074 2065          except e
-0000d3c0: 7472 6565 2e58 4d4c 5379 6e74 6178 4572  tree.XMLSyntaxEr
-0000d3d0: 726f 7220 6173 2065 7272 3a0a 2020 2020  ror as err:.    
-0000d3e0: 2020 2020 2020 2020 2020 2020 6d73 6720              msg 
-0000d3f0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-0000d400: 2020 2020 2020 2020 2254 6865 2058 4d4c          "The XML
-0000d410: 2074 6167 7320 636f 6e74 6169 6e65 6420   tags contained 
-0000d420: 696e 2061 2072 6963 6874 6578 7420 7072  in a richtext pr
-0000d430: 6f70 6572 7479 2028 656e 636f 6469 6e67  operty (encoding
-0000d440: 3d78 6d6c 2920 6d75 7374 2062 6520 7765  =xml) must be we
-0000d450: 6c6c 2d66 6f72 6d65 642e 2022 0a20 2020  ll-formed. ".   
-0000d460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d470: 2022 5468 6520 7370 6563 6961 6c20 6368   "The special ch
-0000d480: 6172 6163 7465 7273 203c 2c20 3e20 616e  aracters <, > an
-0000d490: 6420 2620 6172 6520 6f6e 6c79 2061 6c6c  d & are only all
-0000d4a0: 6f77 6564 2074 6f20 636f 6e73 7472 7563  owed to construc
-0000d4b0: 7420 6120 7461 672e 2022 0a20 2020 2020  t a tag. ".     
-0000d4c0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000d4d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000d4e0: 6361 6c6c 696e 675f 7265 736f 7572 6365  calling_resource
-0000d4f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000d500: 2020 2020 2020 6d73 6720 2b3d 2066 2254        msg += f"T
-0000d510: 6865 2065 7272 6f72 206f 6363 7572 7265  he error occurre
-0000d520: 6420 696e 2072 6573 6f75 7263 6520 7b63  d in resource {c
-0000d530: 616c 6c69 6e67 5f72 6573 6f75 7263 657d  alling_resource}
-0000d540: 2c20 7072 6f70 6572 7479 207b 6e61 6d65  , property {name
-0000d550: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
-0000d560: 2020 206d 7367 202b 3d20 6622 5c6e 4f72     msg += f"\nOr
-0000d570: 6967 696e 616c 2065 7272 6f72 206d 6573  iginal error mes
-0000d580: 7361 6765 3a20 7b65 7272 2e6d 7367 7d22  sage: {err.msg}"
-0000d590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d5a0: 206d 7367 202b 3d20 6622 5c6e 4576 656e   msg += f"\nEven
-0000d5b0: 7475 616c 206c 696e 652f 636f 6c75 6d6e  tual line/column
-0000d5c0: 206e 756d 6265 7273 2061 7265 2072 656c   numbers are rel
-0000d5d0: 6174 6976 6520 746f 2074 6869 7320 7365  ative to this se
-0000d5e0: 7269 616c 697a 6564 2074 6578 743a 207b  rialized text: {
-0000d5f0: 7365 7269 616c 697a 6564 7d22 0a20 2020  serialized}".   
-0000d600: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-0000d610: 7365 2042 6173 6545 7272 6f72 286d 7367  se BaseError(msg
-0000d620: 2920 6672 6f6d 204e 6f6e 650a 2020 2020  ) from None.    
-0000d630: 2020 2020 7072 6f70 5f2e 6170 7065 6e64      prop_.append
-0000d640: 2876 616c 7565 5f29 0a0a 2020 2020 7265  (value_)..    re
-0000d650: 7475 726e 2070 726f 705f 0a0a 0a64 6566  turn prop_...def
-0000d660: 205f 6573 6361 7065 5f72 6573 6572 7665   _escape_reserve
-0000d670: 645f 6368 6172 7328 7465 7874 3a20 7374  d_chars(text: st
-0000d680: 7229 202d 3e20 7374 723a 0a20 2020 2022  r) -> str:.    "
-0000d690: 2222 0a20 2020 2046 726f 6d20 7269 6368  "".    From rich
-0000d6a0: 7465 7874 2073 7472 696e 6773 2028 656e  text strings (en
-0000d6b0: 636f 6469 6e67 3d22 786d 6c22 292c 2065  coding="xml"), e
-0000d6c0: 7363 6170 6520 7468 6520 7265 7365 7276  scape the reserv
-0000d6d0: 6564 2063 6861 7261 6374 6572 7320 3c2c  ed characters <,
-0000d6e0: 203e 2061 6e64 2026 2c0a 2020 2020 6275   > and &,.    bu
-0000d6f0: 7420 6f6e 6c79 2069 6620 7468 6579 2061  t only if they a
-0000d700: 7265 206e 6f74 2070 6172 7420 6f66 2061  re not part of a
-0000d710: 2073 7461 6e64 6172 6420 7374 616e 646f   standard stando
-0000d720: 6666 2074 6167 206f 7220 6573 6361 7065  ff tag or escape
-0000d730: 2073 6571 7565 6e63 652e 0a20 2020 2054   sequence..    T
-0000d740: 6865 2073 7461 6e64 6172 6420 7374 616e  he standard stan
-0000d750: 646f 6666 2074 6167 7320 616c 6c6f 7765  doff tags allowe
-0000d760: 6420 6279 2044 5350 2d41 5049 2061 7265  d by DSP-API are
-0000d770: 2064 6f63 756d 656e 7465 6420 6865 7265   documented here
-0000d780: 3a0a 2020 2020 6874 7470 733a 2f2f 646f  :.    https://do
-0000d790: 6373 2e64 6173 6368 2e73 7769 7373 2f32  cs.dasch.swiss/2
-0000d7a0: 3032 332e 3132 2e30 312f 4453 502d 4150  023.12.01/DSP-AP
-0000d7b0: 492f 3033 2d65 6e64 706f 696e 7473 2f61  I/03-endpoints/a
-0000d7c0: 7069 2d76 322f 7465 7874 2f73 7461 6e64  pi-v2/text/stand
-0000d7d0: 6172 642d 7374 616e 646f 6666 2f0a 0a20  ard-standoff/.. 
-0000d7e0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-0000d7f0: 2074 6578 743a 2074 6865 2072 6963 6874   text: the richt
-0000d800: 6578 7420 7374 7269 6e67 2074 6f20 6265  ext string to be
-0000d810: 2065 7363 6170 6564 0a0a 2020 2020 5265   escaped..    Re
-0000d820: 7475 726e 733a 0a20 2020 2020 2020 2074  turns:.        t
-0000d830: 6865 2065 7363 6170 6564 2072 6963 6874  he escaped richt
-0000d840: 6578 7420 7374 7269 6e67 0a20 2020 2022  ext string.    "
-0000d850: 2222 0a20 2020 2061 6c6c 6f77 6564 5f74  "".    allowed_t
-0000d860: 6167 7320 3d20 5b0a 2020 2020 2020 2020  ags = [.        
-0000d870: 2261 2820 5b5e 3e5d 2b29 3f22 2c20 2023  "a( [^>]+)?",  #
-0000d880: 203c 613e 2069 7320 7468 6520 6f6e 6c79   <a> is the only
-0000d890: 2074 6167 2074 6861 7420 6361 6e20 6861   tag that can ha
-0000d8a0: 7665 2061 7474 7269 6275 7465 730a 2020  ve attributes.  
-0000d8b0: 2020 2020 2020 2270 222c 0a20 2020 2020        "p",.     
-0000d8c0: 2020 2022 656d 222c 0a20 2020 2020 2020     "em",.       
-0000d8d0: 2022 7374 726f 6e67 222c 0a20 2020 2020   "strong",.     
-0000d8e0: 2020 2022 7522 2c0a 2020 2020 2020 2020     "u",.        
-0000d8f0: 2273 7562 222c 0a20 2020 2020 2020 2022  "sub",.        "
-0000d900: 7375 7022 2c0a 2020 2020 2020 2020 2273  sup",.        "s
-0000d910: 7472 696b 6522 2c0a 2020 2020 2020 2020  trike",.        
-0000d920: 2268 3122 2c0a 2020 2020 2020 2020 226f  "h1",.        "o
-0000d930: 6c22 2c0a 2020 2020 2020 2020 2275 6c22  l",.        "ul"
-0000d940: 2c0a 2020 2020 2020 2020 226c 6922 2c0a  ,.        "li",.
-0000d950: 2020 2020 2020 2020 2274 626f 6479 222c          "tbody",
-0000d960: 0a20 2020 2020 2020 2022 7461 626c 6522  .        "table"
-0000d970: 2c0a 2020 2020 2020 2020 2274 7222 2c0a  ,.        "tr",.
-0000d980: 2020 2020 2020 2020 2274 6422 2c0a 2020          "td",.  
-0000d990: 2020 2020 2020 2262 7222 2c0a 2020 2020        "br",.    
-0000d9a0: 2020 2020 2268 7222 2c0a 2020 2020 2020      "hr",.      
-0000d9b0: 2020 2270 7265 222c 0a20 2020 2020 2020    "pre",.       
-0000d9c0: 2022 6369 7465 222c 0a20 2020 2020 2020   "cite",.       
-0000d9d0: 2022 626c 6f63 6b71 756f 7465 222c 0a20   "blockquote",. 
-0000d9e0: 2020 2020 2020 2022 636f 6465 222c 0a20         "code",. 
-0000d9f0: 2020 205d 0a20 2020 2061 6c6c 6f77 6564     ].    allowed
-0000da00: 5f74 6167 735f 7265 6765 7820 3d20 227c  _tags_regex = "|
-0000da10: 222e 6a6f 696e 2861 6c6c 6f77 6564 5f74  ".join(allowed_t
-0000da20: 6167 7329 0a20 2020 206c 6f6f 6b61 6865  ags).    lookahe
-0000da30: 6164 203d 2072 6622 283f 212f 3f28 7b61  ad = rf"(?!/?({a
-0000da40: 6c6c 6f77 6564 5f74 6167 735f 7265 6765  llowed_tags_rege
-0000da50: 787d 292f 3f3e 2922 0a20 2020 2069 6c6c  x})/?>)".    ill
-0000da60: 6567 616c 5f6c 7420 3d20 7266 223c 7b6c  egal_lt = rf"<{l
-0000da70: 6f6f 6b61 6865 6164 7d22 0a20 2020 206c  ookahead}".    l
-0000da80: 6f6f 6b62 6568 696e 6420 3d20 7266 2228  ookbehind = rf"(
-0000da90: 3f3c 213c 2f3f 287b 616c 6c6f 7765 645f  ?<!</?({allowed_
-0000daa0: 7461 6773 5f72 6567 6578 7d29 2f3f 2922  tags_regex})/?)"
-0000dab0: 0a20 2020 2069 6c6c 6567 616c 5f67 7420  .    illegal_gt 
-0000dac0: 3d20 7266 227b 6c6f 6f6b 6265 6869 6e64  = rf"{lookbehind
-0000dad0: 7d3e 220a 2020 2020 696c 6c65 6761 6c5f  }>".    illegal_
-0000dae0: 616d 7020 3d20 7222 2628 3f21 5b23 612d  amp = r"&(?![#a-
-0000daf0: 7a41 2d5a 302d 395d 2b3b 2922 0a20 2020  zA-Z0-9]+;)".   
-0000db00: 2074 6578 7420 3d20 7265 6765 782e 7375   text = regex.su
-0000db10: 6228 696c 6c65 6761 6c5f 6c74 2c20 2226  b(illegal_lt, "&
-0000db20: 6c74 3b22 2c20 7465 7874 290a 2020 2020  lt;", text).    
-0000db30: 7465 7874 203d 2072 6567 6578 2e73 7562  text = regex.sub
-0000db40: 2869 6c6c 6567 616c 5f67 742c 2022 2667  (illegal_gt, "&g
-0000db50: 743b 222c 2074 6578 7429 0a20 2020 2074  t;", text).    t
-0000db60: 6578 7420 3d20 7265 6765 782e 7375 6228  ext = regex.sub(
-0000db70: 696c 6c65 6761 6c5f 616d 702c 2022 2661  illegal_amp, "&a
-0000db80: 6d70 3b22 2c20 7465 7874 290a 2020 2020  mp;", text).    
-0000db90: 7265 7475 726e 2074 6578 740a 0a0a 6465  return text...de
-0000dba0: 6620 6d61 6b65 5f74 696d 655f 7072 6f70  f make_time_prop
-0000dbb0: 280a 2020 2020 6e61 6d65 3a20 7374 722c  (.    name: str,
-0000dbc0: 0a20 2020 2076 616c 7565 3a20 556e 696f  .    value: Unio
-0000dbd0: 6e5b 5072 6f70 6572 7479 456c 656d 656e  n[PropertyElemen
-0000dbe0: 742c 2073 7472 2c20 4974 6572 6162 6c65  t, str, Iterable
-0000dbf0: 5b55 6e69 6f6e 5b50 726f 7065 7274 7945  [Union[PropertyE
-0000dc00: 6c65 6d65 6e74 2c20 7374 725d 5d5d 2c0a  lement, str]]],.
-0000dc10: 2020 2020 6361 6c6c 696e 675f 7265 736f      calling_reso
-0000dc20: 7572 6365 3a20 7374 7220 3d20 2222 2c0a  urce: str = "",.
-0000dc30: 2920 2d3e 2065 7472 6565 2e5f 456c 656d  ) -> etree._Elem
-0000dc40: 656e 743a 0a20 2020 2022 2222 0a20 2020  ent:.    """.   
-0000dc50: 204d 616b 6520 6120 3c74 696d 652d 7072   Make a <time-pr
-0000dc60: 6f70 3e20 6672 6f6d 206f 6e65 206f 7220  op> from one or 
-0000dc70: 6d6f 7265 2064 6174 6574 696d 6520 7661  more datetime va
-0000dc80: 6c75 6573 206f 6620 7468 6520 666f 726d  lues of the form
-0000dc90: 2022 3230 3039 2d31 302d 3130 5431 323a   "2009-10-10T12:
-0000dca0: 3030 3a30 302d 3035 3a30 3022 2e20 5468  00:00-05:00". Th
-0000dcb0: 6520 7469 6d65 2873 2920 6361 6e20 6265  e time(s) can be
-0000dcc0: 0a20 2020 2070 726f 7669 6465 6420 6173  .    provided as
-0000dcd0: 2073 7472 696e 6720 6f72 2061 7320 5072   string or as Pr
-0000dce0: 6f70 6572 7479 456c 656d 656e 7420 7769  opertyElement wi
-0000dcf0: 7468 2061 2073 7472 696e 6720 696e 7369  th a string insi
-0000dd00: 6465 2e20 4966 2070 726f 7669 6465 6420  de. If provided 
-0000dd10: 6173 2073 7472 696e 672c 2074 6865 2070  as string, the p
-0000dd20: 6572 6d69 7373 696f 6e73 2064 6566 6175  ermissions defau
-0000dd30: 6c74 2074 6f0a 2020 2020 2270 726f 702d  lt to.    "prop-
-0000dd40: 6465 6661 756c 7422 2e0a 0a20 2020 2041  default"...    A
-0000dd50: 7267 733a 0a20 2020 2020 2020 206e 616d  rgs:.        nam
-0000dd60: 653a 2074 6865 206e 616d 6520 6f66 2074  e: the name of t
-0000dd70: 6869 7320 7072 6f70 6572 7479 2061 7320  his property as 
-0000dd80: 6465 6669 6e65 6420 696e 2074 6865 206f  defined in the o
-0000dd90: 6e74 6f0a 2020 2020 2020 2020 7661 6c75  nto.        valu
-0000dda0: 653a 206f 6e65 206f 7220 6d6f 7265 2044  e: one or more D
-0000ddb0: 5350 2074 696d 6573 2c20 6173 2073 7472  SP times, as str
-0000ddc0: 696e 672f 5072 6f70 6572 7479 456c 656d  ing/PropertyElem
-0000ddd0: 656e 742c 206f 7220 6173 2069 7465 7261  ent, or as itera
-0000dde0: 626c 6520 6f66 2073 7472 696e 6773 2f50  ble of strings/P
-0000ddf0: 726f 7065 7274 7945 6c65 6d65 6e74 730a  ropertyElements.
-0000de00: 2020 2020 2020 2020 6361 6c6c 696e 675f          calling_
-0000de10: 7265 736f 7572 6365 3a20 7468 6520 6e61  resource: the na
-0000de20: 6d65 206f 6620 7468 6520 7061 7265 6e74  me of the parent
-0000de30: 2072 6573 6f75 7263 6520 2866 6f72 2062   resource (for b
-0000de40: 6574 7465 7220 6572 726f 7220 6d65 7373  etter error mess
-0000de50: 6167 6573 290a 0a20 2020 2057 6172 6e73  ages)..    Warns
-0000de60: 3a0a 2020 2020 2020 2020 4966 206f 6e65  :.        If one
-0000de70: 206f 6620 7468 6520 7661 6c75 6573 2069   of the values i
-0000de80: 7320 6e6f 7420 6120 7661 6c69 6420 4453  s not a valid DS
-0000de90: 5020 7469 6d65 2073 7472 696e 670a 0a20  P time string.. 
-0000dea0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-0000deb0: 2020 2020 616e 2065 7472 6565 2e5f 456c      an etree._El
-0000dec0: 656d 656e 7420 7468 6174 2063 616e 2062  ement that can b
-0000ded0: 6520 6170 7065 6e64 6564 2074 6f20 7468  e appended to th
-0000dee0: 6520 7061 7265 6e74 2072 6573 6f75 7263  e parent resourc
-0000def0: 6520 7769 7468 2072 6573 6f75 7263 652e  e with resource.
-0000df00: 6170 7065 6e64 286d 616b 655f 2a5f 7072  append(make_*_pr
-0000df10: 6f70 282e 2e2e 2929 0a0a 2020 2020 4578  op(...))..    Ex
-0000df20: 616d 706c 6573 3a0a 2020 2020 2020 2020  amples:.        
-0000df30: 3e3e 3e20 6578 6365 6c32 786d 6c2e 6d61  >>> excel2xml.ma
-0000df40: 6b65 5f74 696d 655f 7072 6f70 2822 3a74  ke_time_prop(":t
-0000df50: 6573 7470 726f 7065 7274 7922 2c20 2232  estproperty", "2
-0000df60: 3030 392d 3130 2d31 3054 3132 3a30 303a  009-10-10T12:00:
-0000df70: 3030 2d30 353a 3030 2229 0a20 2020 2020  00-05:00").     
-0000df80: 2020 2020 2020 2020 2020 203c 7469 6d65             <time
-0000df90: 2d70 726f 7020 6e61 6d65 3d22 3a74 6573  -prop name=":tes
-0000dfa0: 7470 726f 7065 7274 7922 3e0a 2020 2020  tproperty">.    
-0000dfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dfc0: 3c74 696d 6520 7065 726d 6973 7369 6f6e  <time permission
-0000dfd0: 733d 2270 726f 702d 6465 6661 756c 7422  s="prop-default"
-0000dfe0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-0000dff0: 2020 2020 2020 2020 2020 3230 3039 2d31            2009-1
-0000e000: 302d 3130 5431 323a 3030 3a30 302d 3035  0-10T12:00:00-05
-0000e010: 3a30 300a 2020 2020 2020 2020 2020 2020  :00.            
-0000e020: 2020 2020 2020 2020 3c2f 7469 6d65 3e0a          </time>.
-0000e030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e040: 3c2f 7469 6d65 2d70 726f 703e 0a20 2020  </time-prop>.   
-0000e050: 2020 2020 203e 3e3e 2065 7863 656c 3278       >>> excel2x
-0000e060: 6d6c 2e6d 616b 655f 7469 6d65 5f70 726f  ml.make_time_pro
-0000e070: 7028 223a 7465 7374 7072 6f70 6572 7479  p(":testproperty
-0000e080: 222c 2065 7863 656c 3278 6d6c 2e50 726f  ", excel2xml.Pro
-0000e090: 7065 7274 7945 6c65 6d65 6e74 2822 3230  pertyElement("20
-0000e0a0: 3039 2d31 302d 3130 5431 323a 3030 3a30  09-10-10T12:00:0
-0000e0b0: 302d 3035 3a30 3022 2c20 7065 726d 6973  0-05:00", permis
-0000e0c0: 7369 6f6e 733d 2270 726f 702d 7265 7374  sions="prop-rest
-0000e0d0: 7269 6374 6564 222c 2063 6f6d 6d65 6e74  ricted", comment
-0000e0e0: 3d22 6578 616d 706c 6522 2929 0a20 2020  ="example")).   
-0000e0f0: 2020 2020 2020 2020 2020 2020 203c 7469               <ti
-0000e100: 6d65 2d70 726f 7020 6e61 6d65 3d22 3a74  me-prop name=":t
-0000e110: 6573 7470 726f 7065 7274 7922 3e0a 2020  estproperty">.  
-0000e120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e130: 2020 3c74 696d 6520 7065 726d 6973 7369    <time permissi
-0000e140: 6f6e 733d 2270 726f 702d 7265 7374 7269  ons="prop-restri
-0000e150: 6374 6564 2220 636f 6d6d 656e 743d 2265  cted" comment="e
-0000e160: 7861 6d70 6c65 223e 0a20 2020 2020 2020  xample">.       
+00006b30: 2020 2020 2020 2020 4752 4547 4f52 4941          GREGORIA
+00006b40: 4e3a 4345 3a31 3933 302d 3039 2d30 323a  N:CE:1930-09-02:
+00006b50: 4345 3a31 3933 302d 3039 2d30 330a 2020  CE:1930-09-03.  
+00006b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b70: 2020 3c2f 6461 7465 3e0a 2020 2020 2020    </date>.      
+00006b80: 2020 2020 2020 2020 2020 3c2f 6461 7465            </date
+00006b90: 2d70 726f 703e 0a0a 2020 2020 5365 6520  -prop>..    See 
+00006ba0: 6874 7470 733a 2f2f 646f 6373 2e64 6173  https://docs.das
+00006bb0: 6368 2e73 7769 7373 2f6c 6174 6573 742f  ch.swiss/latest/
+00006bc0: 4453 502d 544f 4f4c 532f 6669 6c65 2d66  DSP-TOOLS/file-f
+00006bd0: 6f72 6d61 7473 2f78 6d6c 2d64 6174 612d  ormats/xml-data-
+00006be0: 6669 6c65 2f23 6461 7465 2d70 726f 700a  file/#date-prop.
+00006bf0: 2020 2020 2222 220a 0a20 2020 2023 2063      """..    # c
+00006c00: 6865 636b 2074 6865 2069 6e70 7574 3a20  heck the input: 
+00006c10: 7072 6570 6172 6520 6120 6c69 7374 2077  prepare a list w
+00006c20: 6974 6820 7661 6c69 6420 7661 6c75 6573  ith valid values
+00006c30: 0a20 2020 2076 616c 7565 7320 3d20 7072  .    values = pr
+00006c40: 6570 6172 655f 7661 6c75 6528 7661 6c75  epare_value(valu
+00006c50: 6529 0a0a 2020 2020 2320 6368 6563 6b20  e)..    # check 
+00006c60: 7661 6c75 6520 7479 7065 0a20 2020 2066  value type.    f
+00006c70: 6f72 2076 616c 2069 6e20 7661 6c75 6573  or val in values
+00006c80: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
+00006c90: 2069 735f 6675 6c6c 5f64 6174 6528 7374   is_full_date(st
+00006ca0: 7228 7661 6c2e 7661 6c75 6529 2e73 7472  r(val.value).str
+00006cb0: 6970 2829 293a 0a20 2020 2020 2020 2020  ip()):.         
+00006cc0: 2020 206d 7367 203d 2028 0a20 2020 2020     msg = (.     
+00006cd0: 2020 2020 2020 2020 2020 2066 2246 6169             f"Fai
+00006ce0: 6c65 6420 7661 6c69 6461 7469 6f6e 2069  led validation i
+00006cf0: 6e20 7265 736f 7572 6365 2027 7b63 616c  n resource '{cal
+00006d00: 6c69 6e67 5f72 6573 6f75 7263 657d 272c  ling_resource}',
+00006d10: 2070 726f 7065 7274 7920 277b 6e61 6d65   property '{name
+00006d20: 7d27 3a20 220a 2020 2020 2020 2020 2020  }': ".          
+00006d30: 2020 2020 2020 6622 277b 7661 6c2e 7661        f"'{val.va
+00006d40: 6c75 657d 2720 6973 206e 6f74 2061 2076  lue}' is not a v
+00006d50: 616c 6964 2044 5350 2064 6174 652e 220a  alid DSP date.".
+00006d60: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00006d70: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
+00006d80: 6773 2e77 6172 6e28 4473 7054 6f6f 6c73  gs.warn(DspTools
+00006d90: 5573 6572 5761 726e 696e 6728 6d73 6729  UserWarning(msg)
+00006da0: 290a 0a20 2020 2023 206d 616b 6520 786d  )..    # make xm
+00006db0: 6c20 7374 7275 6374 7572 6520 6f66 2074  l structure of t
+00006dc0: 6865 2076 616c 6964 2076 616c 7565 730a  he valid values.
+00006dd0: 2020 2020 7072 6f70 5f20 3d20 6574 7265      prop_ = etre
+00006de0: 652e 456c 656d 656e 7428 0a20 2020 2020  e.Element(.     
+00006df0: 2020 2022 7b25 737d 6461 7465 2d70 726f     "{%s}date-pro
+00006e00: 7022 2025 2078 6d6c 5f6e 616d 6573 7061  p" % xml_namespa
+00006e10: 6365 5f6d 6170 5b4e 6f6e 655d 2c0a 2020  ce_map[None],.  
+00006e20: 2020 2020 2020 6e61 6d65 3d6e 616d 652c        name=name,
+00006e30: 0a20 2020 2020 2020 206e 736d 6170 3d78  .        nsmap=x
+00006e40: 6d6c 5f6e 616d 6573 7061 6365 5f6d 6170  ml_namespace_map
+00006e50: 2c0a 2020 2020 290a 2020 2020 666f 7220  ,.    ).    for 
+00006e60: 7661 6c20 696e 2076 616c 7565 733a 0a20  val in values:. 
+00006e70: 2020 2020 2020 206b 7761 7267 7320 3d20         kwargs = 
+00006e80: 7b22 7065 726d 6973 7369 6f6e 7322 3a20  {"permissions": 
+00006e90: 7661 6c2e 7065 726d 6973 7369 6f6e 737d  val.permissions}
+00006ea0: 0a20 2020 2020 2020 2069 6620 7661 6c2e  .        if val.
+00006eb0: 636f 6d6d 656e 7420 616e 6420 6368 6563  comment and chec
+00006ec0: 6b5f 6e6f 746e 6128 7661 6c2e 636f 6d6d  k_notna(val.comm
+00006ed0: 656e 7429 3a0a 2020 2020 2020 2020 2020  ent):.          
+00006ee0: 2020 6b77 6172 6773 5b22 636f 6d6d 656e    kwargs["commen
+00006ef0: 7422 5d20 3d20 7661 6c2e 636f 6d6d 656e  t"] = val.commen
+00006f00: 740a 2020 2020 2020 2020 7661 6c75 655f  t.        value_
+00006f10: 203d 2065 7472 6565 2e45 6c65 6d65 6e74   = etree.Element
+00006f20: 280a 2020 2020 2020 2020 2020 2020 227b  (.            "{
+00006f30: 2573 7d64 6174 6522 2025 2078 6d6c 5f6e  %s}date" % xml_n
+00006f40: 616d 6573 7061 6365 5f6d 6170 5b4e 6f6e  amespace_map[Non
+00006f50: 655d 2c0a 2020 2020 2020 2020 2020 2020  e],.            
+00006f60: 2a2a 6b77 6172 6773 2c20 2023 2074 7970  **kwargs,  # typ
+00006f70: 653a 2069 676e 6f72 655b 6172 672d 7479  e: ignore[arg-ty
+00006f80: 7065 5d0a 2020 2020 2020 2020 2020 2020  pe].            
+00006f90: 6e73 6d61 703d 786d 6c5f 6e61 6d65 7370  nsmap=xml_namesp
+00006fa0: 6163 655f 6d61 702c 0a20 2020 2020 2020  ace_map,.       
+00006fb0: 2029 0a20 2020 2020 2020 2076 616c 7565   ).        value
+00006fc0: 5f2e 7465 7874 203d 2073 7472 2876 616c  _.text = str(val
+00006fd0: 2e76 616c 7565 292e 7374 7269 7028 290a  .value).strip().
+00006fe0: 2020 2020 2020 2020 7072 6f70 5f2e 6170          prop_.ap
+00006ff0: 7065 6e64 2876 616c 7565 5f29 0a0a 2020  pend(value_)..  
+00007000: 2020 7265 7475 726e 2070 726f 705f 0a0a    return prop_..
+00007010: 0a64 6566 206d 616b 655f 6465 6369 6d61  .def make_decima
+00007020: 6c5f 7072 6f70 280a 2020 2020 6e61 6d65  l_prop(.    name
+00007030: 3a20 7374 722c 0a20 2020 2076 616c 7565  : str,.    value
+00007040: 3a20 556e 696f 6e5b 5072 6f70 6572 7479  : Union[Property
+00007050: 456c 656d 656e 742c 2073 7472 2c20 4974  Element, str, It
+00007060: 6572 6162 6c65 5b55 6e69 6f6e 5b50 726f  erable[Union[Pro
+00007070: 7065 7274 7945 6c65 6d65 6e74 2c20 7374  pertyElement, st
+00007080: 725d 5d5d 2c0a 2020 2020 6361 6c6c 696e  r]]],.    callin
+00007090: 675f 7265 736f 7572 6365 3a20 7374 7220  g_resource: str 
+000070a0: 3d20 2222 2c0a 2920 2d3e 2065 7472 6565  = "",.) -> etree
+000070b0: 2e5f 456c 656d 656e 743a 0a20 2020 2022  ._Element:.    "
+000070c0: 2222 0a20 2020 204d 616b 6520 6120 3c64  "".    Make a <d
+000070d0: 6563 696d 616c 2d70 726f 703e 2066 726f  ecimal-prop> fro
+000070e0: 6d20 6f6e 6520 6f72 206d 6f72 6520 6465  m one or more de
+000070f0: 6369 6d61 6c20 6e75 6d62 6572 732e 2054  cimal numbers. T
+00007100: 6865 2064 6563 696d 616c 2873 2920 6361  he decimal(s) ca
+00007110: 6e20 6265 2070 726f 7669 6465 6420 6173  n be provided as
+00007120: 2073 7472 696e 672c 2066 6c6f 6174 2c20   string, float, 
+00007130: 6f72 2061 730a 2020 2020 5072 6f70 6572  or as.    Proper
+00007140: 7479 456c 656d 656e 7420 7769 7468 2061  tyElement with a
+00007150: 2073 7472 696e 672f 666c 6f61 7420 696e   string/float in
+00007160: 7369 6465 2e20 4966 2070 726f 7669 6465  side. If provide
+00007170: 6420 6173 2073 7472 696e 672f 666c 6f61  d as string/floa
+00007180: 742c 2074 6865 2070 6572 6d69 7373 696f  t, the permissio
+00007190: 6e73 2064 6566 6175 6c74 2074 6f0a 2020  ns default to.  
+000071a0: 2020 2270 726f 702d 6465 6661 756c 7422    "prop-default"
+000071b0: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
+000071c0: 2020 2020 206e 616d 653a 2074 6865 206e       name: the n
+000071d0: 616d 6520 6f66 2074 6869 7320 7072 6f70  ame of this prop
+000071e0: 6572 7479 2061 7320 6465 6669 6e65 6420  erty as defined 
+000071f0: 696e 2074 6865 206f 6e74 6f0a 2020 2020  in the onto.    
+00007200: 2020 2020 7661 6c75 653a 206f 6e65 206f      value: one o
+00007210: 7220 6d6f 7265 2064 6563 696d 616c 206e  r more decimal n
+00007220: 756d 6265 7273 2c20 6173 2073 7472 696e  umbers, as strin
+00007230: 672f 666c 6f61 742f 5072 6f70 6572 7479  g/float/Property
+00007240: 456c 656d 656e 742c 206f 7220 6173 2069  Element, or as i
+00007250: 7465 7261 626c 6520 6f66 2073 7472 696e  terable of strin
+00007260: 6773 2f50 726f 7065 7274 7945 6c65 6d65  gs/PropertyEleme
+00007270: 6e74 730a 2020 2020 2020 2020 6361 6c6c  nts.        call
+00007280: 696e 675f 7265 736f 7572 6365 3a20 7468  ing_resource: th
+00007290: 6520 6e61 6d65 206f 6620 7468 6520 7061  e name of the pa
+000072a0: 7265 6e74 2072 6573 6f75 7263 6520 2866  rent resource (f
+000072b0: 6f72 2062 6574 7465 7220 6572 726f 7220  or better error 
+000072c0: 6d65 7373 6167 6573 290a 0a20 2020 2057  messages)..    W
+000072d0: 6172 6e73 3a0a 2020 2020 2020 2020 4966  arns:.        If
+000072e0: 2074 6865 2076 616c 7565 2069 7320 6e6f   the value is no
+000072f0: 7420 6120 7661 6c69 6420 6465 6369 6d61  t a valid decima
+00007300: 6c20 6e75 6d62 6572 0a0a 2020 2020 5265  l number..    Re
+00007310: 7475 726e 733a 0a20 2020 2020 2020 2061  turns:.        a
+00007320: 6e20 6574 7265 652e 5f45 6c65 6d65 6e74  n etree._Element
+00007330: 2074 6861 7420 6361 6e20 6265 2061 7070   that can be app
+00007340: 656e 6465 6420 746f 2074 6865 2070 6172  ended to the par
+00007350: 656e 7420 7265 736f 7572 6365 2077 6974  ent resource wit
+00007360: 6820 7265 736f 7572 6365 2e61 7070 656e  h resource.appen
+00007370: 6428 6d61 6b65 5f2a 5f70 726f 7028 2e2e  d(make_*_prop(..
+00007380: 2e29 290a 0a20 2020 2045 7861 6d70 6c65  .))..    Example
+00007390: 733a 0a20 2020 2020 2020 203e 3e3e 2065  s:.        >>> e
+000073a0: 7863 656c 3278 6d6c 2e6d 616b 655f 6465  xcel2xml.make_de
+000073b0: 6369 6d61 6c5f 7072 6f70 2822 3a74 6573  cimal_prop(":tes
+000073c0: 7470 726f 7065 7274 7922 2c20 2233 2e31  tproperty", "3.1
+000073d0: 3431 3539 2229 0a20 2020 2020 2020 2020  4159").         
+000073e0: 2020 2020 2020 203c 6465 6369 6d61 6c2d         <decimal-
+000073f0: 7072 6f70 206e 616d 653d 223a 7465 7374  prop name=":test
+00007400: 7072 6f70 6572 7479 223e 0a20 2020 2020  property">.     
+00007410: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00007420: 6465 6369 6d61 6c20 7065 726d 6973 7369  decimal permissi
+00007430: 6f6e 733d 2270 726f 702d 6465 6661 756c  ons="prop-defaul
+00007440: 7422 3e33 2e31 3431 3539 3c2f 6465 6369  t">3.14159</deci
+00007450: 6d61 6c3e 0a20 2020 2020 2020 2020 2020  mal>.           
+00007460: 2020 2020 203c 2f64 6563 696d 616c 2d70       </decimal-p
+00007470: 726f 703e 0a20 2020 2020 2020 203e 3e3e  rop>.        >>>
+00007480: 2065 7863 656c 3278 6d6c 2e6d 616b 655f   excel2xml.make_
+00007490: 6465 6369 6d61 6c5f 7072 6f70 2822 3a74  decimal_prop(":t
+000074a0: 6573 7470 726f 7065 7274 7922 2c20 6578  estproperty", ex
+000074b0: 6365 6c32 786d 6c2e 5072 6f70 6572 7479  cel2xml.Property
+000074c0: 456c 656d 656e 7428 2233 2e31 3431 3539  Element("3.14159
+000074d0: 222c 2070 6572 6d69 7373 696f 6e73 3d22  ", permissions="
+000074e0: 7072 6f70 2d72 6573 7472 6963 7465 6422  prop-restricted"
+000074f0: 2c20 636f 6d6d 656e 743d 2265 7861 6d70  , comment="examp
+00007500: 6c65 2229 290a 2020 2020 2020 2020 2020  le")).          
+00007510: 2020 2020 2020 3c64 6563 696d 616c 2d70        <decimal-p
+00007520: 726f 7020 6e61 6d65 3d22 3a74 6573 7470  rop name=":testp
+00007530: 726f 7065 7274 7922 3e0a 2020 2020 2020  roperty">.      
+00007540: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00007550: 6563 696d 616c 2070 6572 6d69 7373 696f  ecimal permissio
+00007560: 6e73 3d22 7072 6f70 2d72 6573 7472 6963  ns="prop-restric
+00007570: 7465 6422 2063 6f6d 6d65 6e74 3d22 6578  ted" comment="ex
+00007580: 616d 706c 6522 3e33 2e31 3431 3539 3c2f  ample">3.14159</
+00007590: 6465 6369 6d61 6c3e 0a20 2020 2020 2020  decimal>.       
+000075a0: 2020 2020 2020 2020 203c 2f64 6563 696d           </decim
+000075b0: 616c 2d70 726f 703e 0a20 2020 2020 2020  al-prop>.       
+000075c0: 203e 3e3e 2065 7863 656c 3278 6d6c 2e6d   >>> excel2xml.m
+000075d0: 616b 655f 6465 6369 6d61 6c5f 7072 6f70  ake_decimal_prop
+000075e0: 2822 3a74 6573 7470 726f 7065 7274 7922  (":testproperty"
+000075f0: 2c20 5b22 332e 3134 3135 3922 2c20 2232  , ["3.14159", "2
+00007600: 2e37 3138 225d 290a 2020 2020 2020 2020  .718"]).        
+00007610: 2020 2020 2020 2020 3c64 6563 696d 616c          <decimal
+00007620: 2d70 726f 7020 6e61 6d65 3d22 3a74 6573  -prop name=":tes
+00007630: 7470 726f 7065 7274 7922 3e0a 2020 2020  tproperty">.    
+00007640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007650: 3c64 6563 696d 616c 2070 6572 6d69 7373  <decimal permiss
+00007660: 696f 6e73 3d22 7072 6f70 2d64 6566 6175  ions="prop-defau
+00007670: 6c74 223e 332e 3134 3135 393c 2f64 6563  lt">3.14159</dec
+00007680: 696d 616c 3e0a 2020 2020 2020 2020 2020  imal>.          
+00007690: 2020 2020 2020 2020 2020 3c64 6563 696d            <decim
+000076a0: 616c 2070 6572 6d69 7373 696f 6e73 3d22  al permissions="
+000076b0: 7072 6f70 2d64 6566 6175 6c74 223e 322e  prop-default">2.
+000076c0: 3731 383c 2f64 6563 696d 616c 3e0a 2020  718</decimal>.  
+000076d0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+000076e0: 6465 6369 6d61 6c2d 7072 6f70 3e0a 0a20  decimal-prop>.. 
+000076f0: 2020 2053 6565 2068 7474 7073 3a2f 2f64     See https://d
+00007700: 6f63 732e 6461 7363 682e 7377 6973 732f  ocs.dasch.swiss/
+00007710: 6c61 7465 7374 2f44 5350 2d54 4f4f 4c53  latest/DSP-TOOLS
+00007720: 2f66 696c 652d 666f 726d 6174 732f 786d  /file-formats/xm
+00007730: 6c2d 6461 7461 2d66 696c 652f 2364 6563  l-data-file/#dec
+00007740: 696d 616c 2d70 726f 700a 2020 2020 2222  imal-prop.    ""
+00007750: 220a 0a20 2020 2023 2063 6865 636b 2074  "..    # check t
+00007760: 6865 2069 6e70 7574 3a20 7072 6570 6172  he input: prepar
+00007770: 6520 6120 6c69 7374 2077 6974 6820 7661  e a list with va
+00007780: 6c69 6420 7661 6c75 6573 0a20 2020 2076  lid values.    v
+00007790: 616c 7565 7320 3d20 7072 6570 6172 655f  alues = prepare_
+000077a0: 7661 6c75 6528 7661 6c75 6529 0a0a 2020  value(value)..  
+000077b0: 2020 2320 6368 6563 6b20 7661 6c75 6520    # check value 
+000077c0: 7479 7065 0a20 2020 2066 6f72 2076 616c  type.    for val
+000077d0: 2069 6e20 7661 6c75 6573 3a0a 2020 2020   in values:.    
+000077e0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+000077f0: 2020 2020 2066 6c6f 6174 2876 616c 2e76       float(val.v
+00007800: 616c 7565 290a 2020 2020 2020 2020 6578  alue).        ex
+00007810: 6365 7074 2056 616c 7565 4572 726f 723a  cept ValueError:
+00007820: 0a20 2020 2020 2020 2020 2020 206d 7367  .            msg
+00007830: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+00007840: 2020 2020 2066 2246 6169 6c65 6420 7661       f"Failed va
+00007850: 6c69 6461 7469 6f6e 2069 6e20 7265 736f  lidation in reso
+00007860: 7572 6365 2027 7b63 616c 6c69 6e67 5f72  urce '{calling_r
+00007870: 6573 6f75 7263 657d 272c 2070 726f 7065  esource}', prope
+00007880: 7274 7920 277b 6e61 6d65 7d27 3a20 220a  rty '{name}': ".
+00007890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078a0: 6622 277b 7661 6c2e 7661 6c75 657d 2720  f"'{val.value}' 
+000078b0: 6973 206e 6f74 2061 2076 616c 6964 2064  is not a valid d
+000078c0: 6563 696d 616c 206e 756d 6265 722e 220a  ecimal number.".
+000078d0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000078e0: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
+000078f0: 6773 2e77 6172 6e28 4473 7054 6f6f 6c73  gs.warn(DspTools
+00007900: 5573 6572 5761 726e 696e 6728 6d73 6729  UserWarning(msg)
+00007910: 290a 0a20 2020 2023 206d 616b 6520 786d  )..    # make xm
+00007920: 6c20 7374 7275 6374 7572 6520 6f66 2074  l structure of t
+00007930: 6865 2076 616c 6964 2076 616c 7565 730a  he valid values.
+00007940: 2020 2020 7072 6f70 5f20 3d20 6574 7265      prop_ = etre
+00007950: 652e 456c 656d 656e 7428 0a20 2020 2020  e.Element(.     
+00007960: 2020 2022 7b25 737d 6465 6369 6d61 6c2d     "{%s}decimal-
+00007970: 7072 6f70 2220 2520 786d 6c5f 6e61 6d65  prop" % xml_name
+00007980: 7370 6163 655f 6d61 705b 4e6f 6e65 5d2c  space_map[None],
+00007990: 0a20 2020 2020 2020 206e 616d 653d 6e61  .        name=na
+000079a0: 6d65 2c0a 2020 2020 2020 2020 6e73 6d61  me,.        nsma
+000079b0: 703d 786d 6c5f 6e61 6d65 7370 6163 655f  p=xml_namespace_
+000079c0: 6d61 702c 0a20 2020 2029 0a20 2020 2066  map,.    ).    f
+000079d0: 6f72 2076 616c 2069 6e20 7661 6c75 6573  or val in values
+000079e0: 3a0a 2020 2020 2020 2020 6b77 6172 6773  :.        kwargs
+000079f0: 203d 207b 2270 6572 6d69 7373 696f 6e73   = {"permissions
+00007a00: 223a 2076 616c 2e70 6572 6d69 7373 696f  ": val.permissio
+00007a10: 6e73 7d0a 2020 2020 2020 2020 6966 2076  ns}.        if v
+00007a20: 616c 2e63 6f6d 6d65 6e74 2061 6e64 2063  al.comment and c
+00007a30: 6865 636b 5f6e 6f74 6e61 2876 616c 2e63  heck_notna(val.c
+00007a40: 6f6d 6d65 6e74 293a 0a20 2020 2020 2020  omment):.       
+00007a50: 2020 2020 206b 7761 7267 735b 2263 6f6d       kwargs["com
+00007a60: 6d65 6e74 225d 203d 2076 616c 2e63 6f6d  ment"] = val.com
+00007a70: 6d65 6e74 0a20 2020 2020 2020 2076 616c  ment.        val
+00007a80: 7565 5f20 3d20 6574 7265 652e 456c 656d  ue_ = etree.Elem
+00007a90: 656e 7428 0a20 2020 2020 2020 2020 2020  ent(.           
+00007aa0: 2022 7b25 737d 6465 6369 6d61 6c22 2025   "{%s}decimal" %
+00007ab0: 2078 6d6c 5f6e 616d 6573 7061 6365 5f6d   xml_namespace_m
+00007ac0: 6170 5b4e 6f6e 655d 2c0a 2020 2020 2020  ap[None],.      
+00007ad0: 2020 2020 2020 2a2a 6b77 6172 6773 2c20        **kwargs, 
+00007ae0: 2023 2074 7970 653a 2069 676e 6f72 655b   # type: ignore[
+00007af0: 6172 672d 7479 7065 5d0a 2020 2020 2020  arg-type].      
+00007b00: 2020 2020 2020 6e73 6d61 703d 786d 6c5f        nsmap=xml_
+00007b10: 6e61 6d65 7370 6163 655f 6d61 702c 0a20  namespace_map,. 
+00007b20: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00007b30: 2076 616c 7565 5f2e 7465 7874 203d 2073   value_.text = s
+00007b40: 7472 2876 616c 2e76 616c 7565 290a 2020  tr(val.value).  
+00007b50: 2020 2020 2020 7072 6f70 5f2e 6170 7065        prop_.appe
+00007b60: 6e64 2876 616c 7565 5f29 0a0a 2020 2020  nd(value_)..    
+00007b70: 7265 7475 726e 2070 726f 705f 0a0a 0a64  return prop_...d
+00007b80: 6566 206d 616b 655f 6765 6f6d 6574 7279  ef make_geometry
+00007b90: 5f70 726f 7028 0a20 2020 206e 616d 653a  _prop(.    name:
+00007ba0: 2073 7472 2c0a 2020 2020 7661 6c75 653a   str,.    value:
+00007bb0: 2055 6e69 6f6e 5b50 726f 7065 7274 7945   Union[PropertyE
+00007bc0: 6c65 6d65 6e74 2c20 7374 722c 2049 7465  lement, str, Ite
+00007bd0: 7261 626c 655b 556e 696f 6e5b 5072 6f70  rable[Union[Prop
+00007be0: 6572 7479 456c 656d 656e 742c 2073 7472  ertyElement, str
+00007bf0: 5d5d 5d2c 0a20 2020 2063 616c 6c69 6e67  ]]],.    calling
+00007c00: 5f72 6573 6f75 7263 653a 2073 7472 203d  _resource: str =
+00007c10: 2022 222c 0a29 202d 3e20 6574 7265 652e   "",.) -> etree.
+00007c20: 5f45 6c65 6d65 6e74 3a0a 2020 2020 2222  _Element:.    ""
+00007c30: 220a 2020 2020 4d61 6b65 2061 203c 6765  ".    Make a <ge
+00007c40: 6f6d 6574 7279 2d70 726f 703e 2066 726f  ometry-prop> fro
+00007c50: 6d20 6f6e 6520 6f72 206d 6f72 6520 6172  m one or more ar
+00007c60: 6561 7320 6f66 2061 6e20 696d 6167 652e  eas of an image.
+00007c70: 2054 6865 2061 7265 6128 7329 2063 616e   The area(s) can
+00007c80: 2062 6520 7072 6f76 6964 6564 2061 7320   be provided as 
+00007c90: 4a53 4f4e 2d73 7472 696e 6720 6f72 2061  JSON-string or a
+00007ca0: 730a 2020 2020 5072 6f70 6572 7479 456c  s.    PropertyEl
+00007cb0: 656d 656e 7420 7769 7468 2074 6865 204a  ement with the J
+00007cc0: 534f 4e2d 7374 7269 6e67 2069 6e73 6964  SON-string insid
+00007cd0: 652e 2049 6620 7072 6f76 6964 6564 2061  e. If provided a
+00007ce0: 7320 7374 7269 6e67 2c20 7468 6520 7065  s string, the pe
+00007cf0: 726d 6973 7369 6f6e 7320 6465 6661 756c  rmissions defaul
+00007d00: 7420 746f 2022 7072 6f70 2d64 6566 6175  t to "prop-defau
+00007d10: 6c74 222e 0a0a 2020 2020 4172 6773 3a0a  lt"...    Args:.
+00007d20: 2020 2020 2020 2020 6e61 6d65 3a20 7468          name: th
+00007d30: 6520 6e61 6d65 206f 6620 7468 6973 2070  e name of this p
+00007d40: 726f 7065 7274 7920 6173 2064 6566 696e  roperty as defin
+00007d50: 6564 2069 6e20 7468 6520 6f6e 746f 0a20  ed in the onto. 
+00007d60: 2020 2020 2020 2076 616c 7565 3a20 6f6e         value: on
+00007d70: 6520 6f72 206d 6f72 6520 4a53 4f4e 2067  e or more JSON g
+00007d80: 656f 6d65 7472 7920 6f62 6a65 6374 732c  eometry objects,
+00007d90: 2061 7320 7374 7269 6e67 2f50 726f 7065   as string/Prope
+00007da0: 7274 7945 6c65 6d65 6e74 2c20 6f72 2061  rtyElement, or a
+00007db0: 7320 6974 6572 6162 6c65 206f 6620 7374  s iterable of st
+00007dc0: 7269 6e67 732f 5072 6f70 6572 7479 456c  rings/PropertyEl
+00007dd0: 656d 656e 7473 0a20 2020 2020 2020 2063  ements.        c
+00007de0: 616c 6c69 6e67 5f72 6573 6f75 7263 653a  alling_resource:
+00007df0: 2074 6865 206e 616d 6520 6f66 2074 6865   the name of the
+00007e00: 2070 6172 656e 7420 7265 736f 7572 6365   parent resource
+00007e10: 2028 666f 7220 6265 7474 6572 2065 7272   (for better err
+00007e20: 6f72 206d 6573 7361 6765 7329 0a0a 2020  or messages)..  
+00007e30: 2020 5761 726e 733a 0a20 2020 2020 2020    Warns:.       
+00007e40: 2049 6620 7468 6520 7661 6c75 6520 6973   If the value is
+00007e50: 206e 6f74 2061 2076 616c 6964 204a 534f   not a valid JSO
+00007e60: 4e20 6765 6f6d 6574 7279 206f 626a 6563  N geometry objec
+00007e70: 740a 0a20 2020 2052 6574 7572 6e73 3a0a  t..    Returns:.
+00007e80: 2020 2020 2020 2020 616e 2065 7472 6565          an etree
+00007e90: 2e5f 456c 656d 656e 7420 7468 6174 2063  ._Element that c
+00007ea0: 616e 2062 6520 6170 7065 6e64 6564 2074  an be appended t
+00007eb0: 6f20 7468 6520 7061 7265 6e74 2072 6573  o the parent res
+00007ec0: 6f75 7263 6520 7769 7468 2072 6573 6f75  ource with resou
+00007ed0: 7263 652e 6170 7065 6e64 286d 616b 655f  rce.append(make_
+00007ee0: 2a5f 7072 6f70 282e 2e2e 2929 0a0a 2020  *_prop(...))..  
+00007ef0: 2020 4578 616d 706c 6573 3a0a 2020 2020    Examples:.    
+00007f00: 2020 2020 3e3e 3e20 6578 6365 6c32 786d      >>> excel2xm
+00007f10: 6c2e 6d61 6b65 5f67 656f 6d65 7472 795f  l.make_geometry_
+00007f20: 7072 6f70 2822 3a74 6573 7470 726f 7065  prop(":testprope
+00007f30: 7274 7922 2c20 6a73 6f6e 5f73 7472 696e  rty", json_strin
+00007f40: 6729 0a20 2020 2020 2020 2020 2020 2020  g).             
+00007f50: 2020 203c 6765 6f6d 6574 7279 2d70 726f     <geometry-pro
+00007f60: 7020 6e61 6d65 3d22 3a74 6573 7470 726f  p name=":testpro
+00007f70: 7065 7274 7922 3e0a 2020 2020 2020 2020  perty">.        
+00007f80: 2020 2020 2020 2020 2020 2020 3c67 656f              <geo
+00007f90: 6d65 7472 7920 7065 726d 6973 7369 6f6e  metry permission
+00007fa0: 733d 2270 726f 702d 6465 6661 756c 7422  s="prop-default"
+00007fb0: 3e7b 4a53 4f4e 7d3c 2f67 656f 6d65 7472  >{JSON}</geometr
+00007fc0: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
+00007fd0: 2020 203c 2f67 656f 6d65 7472 792d 7072     </geometry-pr
+00007fe0: 6f70 3e0a 2020 2020 2020 2020 3e3e 3e20  op>.        >>> 
+00007ff0: 6578 6365 6c32 786d 6c2e 6d61 6b65 5f67  excel2xml.make_g
+00008000: 656f 6d65 7472 795f 7072 6f70 2822 3a74  eometry_prop(":t
+00008010: 6573 7470 726f 7065 7274 7922 2c20 6578  estproperty", ex
+00008020: 6365 6c32 786d 6c2e 5072 6f70 6572 7479  cel2xml.Property
+00008030: 456c 656d 656e 7428 6a73 6f6e 5f73 7472  Element(json_str
+00008040: 696e 672c 2070 6572 6d69 7373 696f 6e73  ing, permissions
+00008050: 3d22 7072 6f70 2d72 6573 7472 6963 7465  ="prop-restricte
+00008060: 6422 2c20 636f 6d6d 656e 743d 2265 7861  d", comment="exa
+00008070: 6d70 6c65 2229 290a 2020 2020 2020 2020  mple")).        
+00008080: 2020 2020 2020 2020 3c67 656f 6d65 7472          <geometr
+00008090: 792d 7072 6f70 206e 616d 653d 223a 7465  y-prop name=":te
+000080a0: 7374 7072 6f70 6572 7479 223e 0a20 2020  stproperty">.   
+000080b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080c0: 203c 6765 6f6d 6574 7279 2070 6572 6d69   <geometry permi
+000080d0: 7373 696f 6e73 3d22 7072 6f70 2d72 6573  ssions="prop-res
+000080e0: 7472 6963 7465 6422 2063 6f6d 6d65 6e74  tricted" comment
+000080f0: 3d22 6578 616d 706c 6522 3e7b 4a53 4f4e  ="example">{JSON
+00008100: 7d3c 2f67 656f 6d65 7472 793e 0a20 2020  }</geometry>.   
+00008110: 2020 2020 2020 2020 2020 2020 203c 2f67               </g
+00008120: 656f 6d65 7472 792d 7072 6f70 3e0a 2020  eometry-prop>.  
+00008130: 2020 2020 2020 3e3e 3e20 6578 6365 6c32        >>> excel2
+00008140: 786d 6c2e 6d61 6b65 5f67 656f 6d65 7472  xml.make_geometr
+00008150: 795f 7072 6f70 2822 3a74 6573 7470 726f  y_prop(":testpro
+00008160: 7065 7274 7922 2c20 5b6a 736f 6e5f 7374  perty", [json_st
+00008170: 7269 6e67 312c 206a 736f 6e5f 7374 7269  ring1, json_stri
+00008180: 6e67 325d 290a 2020 2020 2020 2020 2020  ng2]).          
+00008190: 2020 2020 2020 3c67 656f 6d65 7472 792d        <geometry-
+000081a0: 7072 6f70 206e 616d 653d 223a 7465 7374  prop name=":test
+000081b0: 7072 6f70 6572 7479 223e 0a20 2020 2020  property">.     
+000081c0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000081d0: 6765 6f6d 6574 7279 2070 6572 6d69 7373  geometry permiss
+000081e0: 696f 6e73 3d22 7072 6f70 2d64 6566 6175  ions="prop-defau
+000081f0: 6c74 223e 7b4a 534f 4e7d 3c2f 6765 6f6d  lt">{JSON}</geom
+00008200: 6574 7279 3e0a 2020 2020 2020 2020 2020  etry>.          
+00008210: 2020 2020 2020 2020 2020 3c67 656f 6d65            <geome
+00008220: 7472 7920 7065 726d 6973 7369 6f6e 733d  try permissions=
+00008230: 2270 726f 702d 6465 6661 756c 7422 3e7b  "prop-default">{
+00008240: 4a53 4f4e 7d3c 2f67 656f 6d65 7472 793e  JSON}</geometry>
+00008250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008260: 203c 2f67 656f 6d65 7472 792d 7072 6f70   </geometry-prop
+00008270: 3e0a 0a20 2020 2053 6565 2068 7474 7073  >..    See https
+00008280: 3a2f 2f64 6f63 732e 6461 7363 682e 7377  ://docs.dasch.sw
+00008290: 6973 732f 6c61 7465 7374 2f44 5350 2d54  iss/latest/DSP-T
+000082a0: 4f4f 4c53 2f66 696c 652d 666f 726d 6174  OOLS/file-format
+000082b0: 732f 786d 6c2d 6461 7461 2d66 696c 652f  s/xml-data-file/
+000082c0: 2367 656f 6d65 7472 792d 7072 6f70 0a20  #geometry-prop. 
+000082d0: 2020 2022 2222 0a0a 2020 2020 2320 6368     """..    # ch
+000082e0: 6563 6b20 7468 6520 696e 7075 743a 2070  eck the input: p
+000082f0: 7265 7061 7265 2061 206c 6973 7420 7769  repare a list wi
+00008300: 7468 2076 616c 6964 2076 616c 7565 730a  th valid values.
+00008310: 2020 2020 7661 6c75 6573 203d 2070 7265      values = pre
+00008320: 7061 7265 5f76 616c 7565 2876 616c 7565  pare_value(value
+00008330: 290a 0a20 2020 2023 2063 6865 636b 2076  )..    # check v
+00008340: 616c 7565 2074 7970 650a 2020 2020 666f  alue type.    fo
+00008350: 7220 7661 6c20 696e 2076 616c 7565 733a  r val in values:
+00008360: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+00008370: 2020 2020 2020 2020 2020 7661 6c75 655f            value_
+00008380: 6173 5f64 6963 7420 3d20 6a73 6f6e 2e6c  as_dict = json.l
+00008390: 6f61 6473 2873 7472 2876 616c 2e76 616c  oads(str(val.val
+000083a0: 7565 2929 0a20 2020 2020 2020 2020 2020  ue)).           
+000083b0: 2069 6620 7661 6c75 655f 6173 5f64 6963   if value_as_dic
+000083c0: 745b 2274 7970 6522 5d20 6e6f 7420 696e  t["type"] not in
+000083d0: 205b 2272 6563 7461 6e67 6c65 222c 2022   ["rectangle", "
+000083e0: 6369 7263 6c65 222c 2022 706f 6c79 676f  circle", "polygo
+000083f0: 6e22 5d3a 0a20 2020 2020 2020 2020 2020  n"]:.           
+00008400: 2020 2020 206d 7367 203d 2028 0a20 2020       msg = (.   
+00008410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008420: 2066 2246 6169 6c65 6420 7661 6c69 6461   f"Failed valida
+00008430: 7469 6f6e 2069 6e20 7265 736f 7572 6365  tion in resource
+00008440: 2027 7b63 616c 6c69 6e67 5f72 6573 6f75   '{calling_resou
+00008450: 7263 657d 272c 2070 726f 7065 7274 7920  rce}', property 
+00008460: 277b 6e61 6d65 7d27 3a20 220a 2020 2020  '{name}': ".    
+00008470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008480: 6622 5468 6520 2774 7970 6527 206f 6620  f"The 'type' of 
+00008490: 7468 6520 4a53 4f4e 2067 656f 6d65 7472  the JSON geometr
+000084a0: 7920 6f62 6a65 6374 206d 7573 7420 6265  y object must be
+000084b0: 2027 7265 6374 616e 676c 6527 2c20 2763   'rectangle', 'c
+000084c0: 6972 636c 6527 2c20 6f72 2027 706f 6c79  ircle', or 'poly
+000084d0: 676f 6e27 2e22 0a20 2020 2020 2020 2020  gon'.".         
+000084e0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000084f0: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
+00008500: 732e 7761 726e 2844 7370 546f 6f6c 7355  s.warn(DspToolsU
+00008510: 7365 7257 6172 6e69 6e67 286d 7367 2929  serWarning(msg))
+00008520: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00008530: 6e6f 7420 6973 696e 7374 616e 6365 2876  not isinstance(v
+00008540: 616c 7565 5f61 735f 6469 6374 5b22 706f  alue_as_dict["po
+00008550: 696e 7473 225d 2c20 6c69 7374 293a 0a20  ints"], list):. 
+00008560: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00008570: 7367 203d 2028 0a20 2020 2020 2020 2020  sg = (.         
+00008580: 2020 2020 2020 2020 2020 2066 2246 6169             f"Fai
+00008590: 6c65 6420 7661 6c69 6461 7469 6f6e 2069  led validation i
+000085a0: 6e20 7265 736f 7572 6365 2027 7b63 616c  n resource '{cal
+000085b0: 6c69 6e67 5f72 6573 6f75 7263 657d 272c  ling_resource}',
+000085c0: 2070 726f 7065 7274 7920 277b 6e61 6d65   property '{name
+000085d0: 7d27 3a20 220a 2020 2020 2020 2020 2020  }': ".          
+000085e0: 2020 2020 2020 2020 2020 6622 5468 6520            f"The 
+000085f0: 2770 6f69 6e74 7327 6f66 2074 6865 204a  'points'of the J
+00008600: 534f 4e20 6765 6f6d 6574 7279 206f 626a  SON geometry obj
+00008610: 6563 7420 6d75 7374 2062 6520 6120 6c69  ect must be a li
+00008620: 7374 206f 6620 706f 696e 7473 2e22 0a20  st of points.". 
+00008630: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00008640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008650: 2077 6172 6e69 6e67 732e 7761 726e 2844   warnings.warn(D
+00008660: 7370 546f 6f6c 7355 7365 7257 6172 6e69  spToolsUserWarni
+00008670: 6e67 286d 7367 2929 0a20 2020 2020 2020  ng(msg)).       
+00008680: 2065 7863 6570 7420 286a 736f 6e2e 4a53   except (json.JS
+00008690: 4f4e 4465 636f 6465 4572 726f 722c 2054  ONDecodeError, T
+000086a0: 7970 6545 7272 6f72 2c20 496e 6465 7845  ypeError, IndexE
+000086b0: 7272 6f72 2c20 4b65 7945 7272 6f72 2c20  rror, KeyError, 
+000086c0: 4173 7365 7274 696f 6e45 7272 6f72 293a  AssertionError):
+000086d0: 0a20 2020 2020 2020 2020 2020 206d 7367  .            msg
+000086e0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+000086f0: 2020 2020 2066 2246 6169 6c65 6420 7661       f"Failed va
+00008700: 6c69 6461 7469 6f6e 2069 6e20 7265 736f  lidation in reso
+00008710: 7572 6365 2027 7b63 616c 6c69 6e67 5f72  urce '{calling_r
+00008720: 6573 6f75 7263 657d 272c 2070 726f 7065  esource}', prope
+00008730: 7274 7920 277b 6e61 6d65 7d27 3a20 220a  rty '{name}': ".
+00008740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008750: 6622 277b 7661 6c2e 7661 6c75 657d 2720  f"'{val.value}' 
+00008760: 6973 206e 6f74 2061 2076 616c 6964 204a  is not a valid J
+00008770: 534f 4e20 6765 6f6d 6574 7279 206f 626a  SON geometry obj
+00008780: 6563 742e 220a 2020 2020 2020 2020 2020  ect.".          
+00008790: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+000087a0: 7761 726e 696e 6773 2e77 6172 6e28 4473  warnings.warn(Ds
+000087b0: 7054 6f6f 6c73 5573 6572 5761 726e 696e  pToolsUserWarnin
+000087c0: 6728 6d73 6729 290a 0a20 2020 2023 206d  g(msg))..    # m
+000087d0: 616b 6520 786d 6c20 7374 7275 6374 7572  ake xml structur
+000087e0: 6520 6f66 2074 6865 2076 616c 6964 2076  e of the valid v
+000087f0: 616c 7565 730a 2020 2020 7072 6f70 5f20  alues.    prop_ 
+00008800: 3d20 6574 7265 652e 456c 656d 656e 7428  = etree.Element(
+00008810: 0a20 2020 2020 2020 2022 7b25 737d 6765  .        "{%s}ge
+00008820: 6f6d 6574 7279 2d70 726f 7022 2025 2078  ometry-prop" % x
+00008830: 6d6c 5f6e 616d 6573 7061 6365 5f6d 6170  ml_namespace_map
+00008840: 5b4e 6f6e 655d 2c0a 2020 2020 2020 2020  [None],.        
+00008850: 6e61 6d65 3d6e 616d 652c 0a20 2020 2020  name=name,.     
+00008860: 2020 206e 736d 6170 3d78 6d6c 5f6e 616d     nsmap=xml_nam
+00008870: 6573 7061 6365 5f6d 6170 2c0a 2020 2020  espace_map,.    
+00008880: 290a 2020 2020 666f 7220 7661 6c20 696e  ).    for val in
+00008890: 2076 616c 7565 733a 0a20 2020 2020 2020   values:.       
+000088a0: 206b 7761 7267 7320 3d20 7b22 7065 726d   kwargs = {"perm
+000088b0: 6973 7369 6f6e 7322 3a20 7661 6c2e 7065  issions": val.pe
+000088c0: 726d 6973 7369 6f6e 737d 0a20 2020 2020  rmissions}.     
+000088d0: 2020 2069 6620 7661 6c2e 636f 6d6d 656e     if val.commen
+000088e0: 7420 616e 6420 6368 6563 6b5f 6e6f 746e  t and check_notn
+000088f0: 6128 7661 6c2e 636f 6d6d 656e 7429 3a0a  a(val.comment):.
+00008900: 2020 2020 2020 2020 2020 2020 6b77 6172              kwar
+00008910: 6773 5b22 636f 6d6d 656e 7422 5d20 3d20  gs["comment"] = 
+00008920: 7661 6c2e 636f 6d6d 656e 740a 2020 2020  val.comment.    
+00008930: 2020 2020 7661 6c75 655f 203d 2065 7472      value_ = etr
+00008940: 6565 2e45 6c65 6d65 6e74 280a 2020 2020  ee.Element(.    
+00008950: 2020 2020 2020 2020 227b 2573 7d67 656f          "{%s}geo
+00008960: 6d65 7472 7922 2025 2078 6d6c 5f6e 616d  metry" % xml_nam
+00008970: 6573 7061 6365 5f6d 6170 5b4e 6f6e 655d  espace_map[None]
+00008980: 2c0a 2020 2020 2020 2020 2020 2020 2a2a  ,.            **
+00008990: 6b77 6172 6773 2c20 2023 2074 7970 653a  kwargs,  # type:
+000089a0: 2069 676e 6f72 655b 6172 672d 7479 7065   ignore[arg-type
+000089b0: 5d0a 2020 2020 2020 2020 2020 2020 6e73  ].            ns
+000089c0: 6d61 703d 786d 6c5f 6e61 6d65 7370 6163  map=xml_namespac
+000089d0: 655f 6d61 702c 0a20 2020 2020 2020 2029  e_map,.        )
+000089e0: 0a20 2020 2020 2020 2076 616c 7565 5f2e  .        value_.
+000089f0: 7465 7874 203d 2073 7472 2876 616c 2e76  text = str(val.v
+00008a00: 616c 7565 290a 2020 2020 2020 2020 7072  alue).        pr
+00008a10: 6f70 5f2e 6170 7065 6e64 2876 616c 7565  op_.append(value
+00008a20: 5f29 0a20 2020 2072 6574 7572 6e20 7072  _).    return pr
+00008a30: 6f70 5f0a 0a0a 6465 6620 6d61 6b65 5f67  op_...def make_g
+00008a40: 656f 6e61 6d65 5f70 726f 7028 0a20 2020  eoname_prop(.   
+00008a50: 206e 616d 653a 2073 7472 2c0a 2020 2020   name: str,.    
+00008a60: 7661 6c75 653a 2055 6e69 6f6e 5b50 726f  value: Union[Pro
+00008a70: 7065 7274 7945 6c65 6d65 6e74 2c20 7374  pertyElement, st
+00008a80: 722c 2069 6e74 2c20 4974 6572 6162 6c65  r, int, Iterable
+00008a90: 5b55 6e69 6f6e 5b50 726f 7065 7274 7945  [Union[PropertyE
+00008aa0: 6c65 6d65 6e74 2c20 7374 722c 2069 6e74  lement, str, int
+00008ab0: 5d5d 5d2c 0a20 2020 2063 616c 6c69 6e67  ]]],.    calling
+00008ac0: 5f72 6573 6f75 7263 653a 2073 7472 203d  _resource: str =
+00008ad0: 2022 222c 0a29 202d 3e20 6574 7265 652e   "",.) -> etree.
+00008ae0: 5f45 6c65 6d65 6e74 3a0a 2020 2020 2222  _Element:.    ""
+00008af0: 220a 2020 2020 4d61 6b65 2061 203c 6765  ".    Make a <ge
+00008b00: 6f6e 616d 652d 7072 6f70 3e20 6672 6f6d  oname-prop> from
+00008b10: 206f 6e65 206f 7220 6d6f 7265 2067 656f   one or more geo
+00008b20: 6e61 6d65 732e 6f72 6720 4944 732e 2054  names.org IDs. T
+00008b30: 6865 2049 4428 7329 2063 616e 2062 6520  he ID(s) can be 
+00008b40: 7072 6f76 6964 6564 2061 7320 7374 7269  provided as stri
+00008b50: 6e67 2c20 696e 7465 6765 722c 206f 7220  ng, integer, or 
+00008b60: 6173 0a20 2020 2050 726f 7065 7274 7945  as.    PropertyE
+00008b70: 6c65 6d65 6e74 2077 6974 6820 6120 7374  lement with a st
+00008b80: 7269 6e67 2f69 6e74 6567 6572 2069 6e73  ring/integer ins
+00008b90: 6964 652e 2049 6620 7072 6f76 6964 6564  ide. If provided
+00008ba0: 2061 7320 7374 7269 6e67 2f69 6e74 6567   as string/integ
+00008bb0: 6572 2c20 7468 6520 7065 726d 6973 7369  er, the permissi
+00008bc0: 6f6e 7320 6465 6661 756c 7420 746f 0a20  ons default to. 
+00008bd0: 2020 2022 7072 6f70 2d64 6566 6175 6c74     "prop-default
+00008be0: 222e 0a0a 2020 2020 4172 6773 3a0a 2020  "...    Args:.  
+00008bf0: 2020 2020 2020 6e61 6d65 3a20 7468 6520        name: the 
+00008c00: 6e61 6d65 206f 6620 7468 6973 2070 726f  name of this pro
+00008c10: 7065 7274 7920 6173 2064 6566 696e 6564  perty as defined
+00008c20: 2069 6e20 7468 6520 6f6e 746f 0a20 2020   in the onto.   
+00008c30: 2020 2020 2076 616c 7565 3a20 6f6e 6520       value: one 
+00008c40: 6f72 206d 6f72 6520 6765 6f6e 616d 6573  or more geonames
+00008c50: 2e6f 7267 2049 4473 2c20 6173 2073 7472  .org IDs, as str
+00008c60: 2f69 6e74 2f50 726f 7065 7274 7945 6c65  /int/PropertyEle
+00008c70: 6d65 6e74 2c20 6f72 2061 7320 6974 6572  ment, or as iter
+00008c80: 6162 6c65 206f 6620 7374 722f 696e 742f  able of str/int/
+00008c90: 5072 6f70 6572 7479 456c 656d 656e 740a  PropertyElement.
+00008ca0: 2020 2020 2020 2020 6361 6c6c 696e 675f          calling_
+00008cb0: 7265 736f 7572 6365 3a20 7468 6520 6e61  resource: the na
+00008cc0: 6d65 206f 6620 7468 6520 7061 7265 6e74  me of the parent
+00008cd0: 2072 6573 6f75 7263 6520 2866 6f72 2062   resource (for b
+00008ce0: 6574 7465 7220 6572 726f 7220 6d65 7373  etter error mess
+00008cf0: 6167 6573 290a 0a20 2020 2057 6172 6e73  ages)..    Warns
+00008d00: 3a0a 2020 2020 2020 2020 4966 2074 6865  :.        If the
+00008d10: 2076 616c 7565 2069 7320 6e6f 7420 6120   value is not a 
+00008d20: 7661 6c69 6420 6765 6f6e 616d 6573 2e6f  valid geonames.o
+00008d30: 7267 2069 6465 6e74 6966 6965 720a 0a20  rg identifier.. 
+00008d40: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00008d50: 2020 2020 616e 2065 7472 6565 2e5f 456c      an etree._El
+00008d60: 656d 656e 7420 7468 6174 2063 616e 2062  ement that can b
+00008d70: 6520 6170 7065 6e64 6564 2074 6f20 7468  e appended to th
+00008d80: 6520 7061 7265 6e74 2072 6573 6f75 7263  e parent resourc
+00008d90: 6520 7769 7468 2072 6573 6f75 7263 652e  e with resource.
+00008da0: 6170 7065 6e64 286d 616b 655f 2a5f 7072  append(make_*_pr
+00008db0: 6f70 282e 2e2e 2929 0a0a 2020 2020 4578  op(...))..    Ex
+00008dc0: 616d 706c 6573 3a0a 2020 2020 2020 2020  amples:.        
+00008dd0: 3e3e 3e20 6578 6365 6c32 786d 6c2e 6d61  >>> excel2xml.ma
+00008de0: 6b65 5f67 656f 6e61 6d65 5f70 726f 7028  ke_geoname_prop(
+00008df0: 223a 7465 7374 7072 6f70 6572 7479 222c  ":testproperty",
+00008e00: 2022 3237 3631 3336 3922 290a 2020 2020   "2761369").    
+00008e10: 2020 2020 2020 2020 2020 2020 3c67 656f              <geo
+00008e20: 6e61 6d65 2d70 726f 7020 6e61 6d65 3d22  name-prop name="
+00008e30: 3a74 6573 7470 726f 7065 7274 7922 3e0a  :testproperty">.
+00008e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e50: 2020 2020 3c67 656f 6e61 6d65 2070 6572      <geoname per
+00008e60: 6d69 7373 696f 6e73 3d22 7072 6f70 2d64  missions="prop-d
+00008e70: 6566 6175 6c74 223e 3237 3631 3336 393c  efault">2761369<
+00008e80: 2f67 656f 6e61 6d65 3e0a 2020 2020 2020  /geoname>.      
+00008e90: 2020 2020 2020 2020 2020 3c2f 6765 6f6e            </geon
+00008ea0: 616d 652d 7072 6f70 3e0a 2020 2020 2020  ame-prop>.      
+00008eb0: 2020 3e3e 3e20 6578 6365 6c32 786d 6c2e    >>> excel2xml.
+00008ec0: 6d61 6b65 5f67 656f 6e61 6d65 5f70 726f  make_geoname_pro
+00008ed0: 7028 223a 7465 7374 7072 6f70 6572 7479  p(":testproperty
+00008ee0: 222c 2065 7863 656c 3278 6d6c 2e50 726f  ", excel2xml.Pro
+00008ef0: 7065 7274 7945 6c65 6d65 6e74 2822 3237  pertyElement("27
+00008f00: 3631 3336 3922 2c20 7065 726d 6973 7369  61369", permissi
+00008f10: 6f6e 733d 2270 726f 702d 7265 7374 7269  ons="prop-restri
+00008f20: 6374 6564 222c 2063 6f6d 6d65 6e74 3d22  cted", comment="
+00008f30: 6578 616d 706c 6522 2929 0a20 2020 2020  example")).     
+00008f40: 2020 2020 2020 2020 2020 203c 6765 6f6e             <geon
+00008f50: 616d 652d 7072 6f70 206e 616d 653d 223a  ame-prop name=":
+00008f60: 7465 7374 7072 6f70 6572 7479 223e 0a20  testproperty">. 
+00008f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f80: 2020 203c 6765 6f6e 616d 6520 7065 726d     <geoname perm
+00008f90: 6973 7369 6f6e 733d 2270 726f 702d 7265  issions="prop-re
+00008fa0: 7374 7269 6374 6564 2220 636f 6d6d 656e  stricted" commen
+00008fb0: 743d 2265 7861 6d70 6c65 223e 3237 3631  t="example">2761
+00008fc0: 3336 393c 2f67 656f 6e61 6d65 3e0a 2020  369</geoname>.  
+00008fd0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00008fe0: 6765 6f6e 616d 652d 7072 6f70 3e0a 2020  geoname-prop>.  
+00008ff0: 2020 2020 2020 3e3e 3e20 6578 6365 6c32        >>> excel2
+00009000: 786d 6c2e 6d61 6b65 5f67 656f 6e61 6d65  xml.make_geoname
+00009010: 5f70 726f 7028 223a 7465 7374 7072 6f70  _prop(":testprop
+00009020: 6572 7479 222c 205b 2232 3736 3133 3639  erty", ["2761369
+00009030: 222c 2022 3130 3130 3130 3122 5d29 0a20  ", "1010101"]). 
+00009040: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00009050: 6765 6f6e 616d 652d 7072 6f70 206e 616d  geoname-prop nam
+00009060: 653d 223a 7465 7374 7072 6f70 6572 7479  e=":testproperty
+00009070: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00009080: 2020 2020 2020 203c 6765 6f6e 616d 6520         <geoname 
+00009090: 7065 726d 6973 7369 6f6e 733d 2270 726f  permissions="pro
+000090a0: 702d 6465 6661 756c 7422 3e32 3736 3133  p-default">27613
+000090b0: 3639 3c2f 6765 6f6e 616d 653e 0a20 2020  69</geoname>.   
+000090c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000090d0: 203c 6765 6f6e 616d 6520 7065 726d 6973   <geoname permis
+000090e0: 7369 6f6e 733d 2270 726f 702d 6465 6661  sions="prop-defa
+000090f0: 756c 7422 3e31 3031 3031 3031 3c2f 6765  ult">1010101</ge
+00009100: 6f6e 616d 653e 0a20 2020 2020 2020 2020  oname>.         
+00009110: 2020 2020 2020 203c 2f67 656f 6e61 6d65         </geoname
+00009120: 2d70 726f 703e 0a0a 2020 2020 5365 6520  -prop>..    See 
+00009130: 6874 7470 733a 2f2f 646f 6373 2e64 6173  https://docs.das
+00009140: 6368 2e73 7769 7373 2f6c 6174 6573 742f  ch.swiss/latest/
+00009150: 4453 502d 544f 4f4c 532f 6669 6c65 2d66  DSP-TOOLS/file-f
+00009160: 6f72 6d61 7473 2f78 6d6c 2d64 6174 612d  ormats/xml-data-
+00009170: 6669 6c65 2f23 6765 6f6e 616d 652d 7072  file/#geoname-pr
+00009180: 6f70 0a20 2020 2022 2222 0a0a 2020 2020  op.    """..    
+00009190: 2320 6368 6563 6b20 7468 6520 696e 7075  # check the inpu
+000091a0: 743a 2070 7265 7061 7265 2061 206c 6973  t: prepare a lis
+000091b0: 7420 7769 7468 2076 616c 6964 2076 616c  t with valid val
+000091c0: 7565 730a 2020 2020 7661 6c75 6573 203d  ues.    values =
+000091d0: 2070 7265 7061 7265 5f76 616c 7565 2876   prepare_value(v
+000091e0: 616c 7565 290a 0a20 2020 2023 2063 6865  alue)..    # che
+000091f0: 636b 2076 616c 7565 2074 7970 650a 2020  ck value type.  
+00009200: 2020 666f 7220 7661 6c20 696e 2076 616c    for val in val
+00009210: 7565 733a 0a20 2020 2020 2020 2069 6620  ues:.        if 
+00009220: 6e6f 7420 7265 6765 782e 7365 6172 6368  not regex.search
+00009230: 2872 225e 5b30 2d39 5d2b 2422 2c20 7374  (r"^[0-9]+$", st
+00009240: 7228 7661 6c2e 7661 6c75 6529 293a 0a20  r(val.value)):. 
+00009250: 2020 2020 2020 2020 2020 206d 7367 203d             msg =
+00009260: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00009270: 2020 2066 2246 6169 6c65 6420 7661 6c69     f"Failed vali
+00009280: 6461 7469 6f6e 2069 6e20 7265 736f 7572  dation in resour
+00009290: 6365 2027 7b63 616c 6c69 6e67 5f72 6573  ce '{calling_res
+000092a0: 6f75 7263 657d 272c 2070 726f 7065 7274  ource}', propert
+000092b0: 7920 277b 6e61 6d65 7d27 3a20 220a 2020  y '{name}': ".  
+000092c0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+000092d0: 277b 7661 6c2e 7661 6c75 657d 2720 6973  '{val.value}' is
+000092e0: 206e 6f74 2061 2067 656f 6e61 6d65 732e   not a geonames.
+000092f0: 6f72 6720 6964 656e 7469 6669 6572 2e22  org identifier."
+00009300: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00009310: 2020 2020 2020 2020 2020 2077 6172 6e69             warni
+00009320: 6e67 732e 7761 726e 2844 7370 546f 6f6c  ngs.warn(DspTool
+00009330: 7355 7365 7257 6172 6e69 6e67 286d 7367  sUserWarning(msg
+00009340: 2929 0a0a 2020 2020 2320 6d61 6b65 2078  ))..    # make x
+00009350: 6d6c 2073 7472 7563 7475 7265 206f 6620  ml structure of 
+00009360: 7468 6520 7661 6c69 6420 7661 6c75 6573  the valid values
+00009370: 0a20 2020 2070 726f 705f 203d 2065 7472  .    prop_ = etr
+00009380: 6565 2e45 6c65 6d65 6e74 280a 2020 2020  ee.Element(.    
+00009390: 2020 2020 227b 2573 7d67 656f 6e61 6d65      "{%s}geoname
+000093a0: 2d70 726f 7022 2025 2078 6d6c 5f6e 616d  -prop" % xml_nam
+000093b0: 6573 7061 6365 5f6d 6170 5b4e 6f6e 655d  espace_map[None]
+000093c0: 2c0a 2020 2020 2020 2020 6e61 6d65 3d6e  ,.        name=n
+000093d0: 616d 652c 0a20 2020 2020 2020 206e 736d  ame,.        nsm
+000093e0: 6170 3d78 6d6c 5f6e 616d 6573 7061 6365  ap=xml_namespace
+000093f0: 5f6d 6170 2c0a 2020 2020 290a 2020 2020  _map,.    ).    
+00009400: 666f 7220 7661 6c20 696e 2076 616c 7565  for val in value
+00009410: 733a 0a20 2020 2020 2020 206b 7761 7267  s:.        kwarg
+00009420: 7320 3d20 7b22 7065 726d 6973 7369 6f6e  s = {"permission
+00009430: 7322 3a20 7661 6c2e 7065 726d 6973 7369  s": val.permissi
+00009440: 6f6e 737d 0a20 2020 2020 2020 2069 6620  ons}.        if 
+00009450: 7661 6c2e 636f 6d6d 656e 7420 616e 6420  val.comment and 
+00009460: 6368 6563 6b5f 6e6f 746e 6128 7661 6c2e  check_notna(val.
+00009470: 636f 6d6d 656e 7429 3a0a 2020 2020 2020  comment):.      
+00009480: 2020 2020 2020 6b77 6172 6773 5b22 636f        kwargs["co
+00009490: 6d6d 656e 7422 5d20 3d20 7661 6c2e 636f  mment"] = val.co
+000094a0: 6d6d 656e 740a 2020 2020 2020 2020 7661  mment.        va
+000094b0: 6c75 655f 203d 2065 7472 6565 2e45 6c65  lue_ = etree.Ele
+000094c0: 6d65 6e74 280a 2020 2020 2020 2020 2020  ment(.          
+000094d0: 2020 227b 2573 7d67 656f 6e61 6d65 2220    "{%s}geoname" 
+000094e0: 2520 786d 6c5f 6e61 6d65 7370 6163 655f  % xml_namespace_
+000094f0: 6d61 705b 4e6f 6e65 5d2c 0a20 2020 2020  map[None],.     
+00009500: 2020 2020 2020 202a 2a6b 7761 7267 732c         **kwargs,
+00009510: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
+00009520: 5b61 7267 2d74 7970 655d 0a20 2020 2020  [arg-type].     
+00009530: 2020 2020 2020 206e 736d 6170 3d78 6d6c         nsmap=xml
+00009540: 5f6e 616d 6573 7061 6365 5f6d 6170 2c0a  _namespace_map,.
+00009550: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00009560: 2020 7661 6c75 655f 2e74 6578 7420 3d20    value_.text = 
+00009570: 7374 7228 7661 6c2e 7661 6c75 6529 0a20  str(val.value). 
+00009580: 2020 2020 2020 2070 726f 705f 2e61 7070         prop_.app
+00009590: 656e 6428 7661 6c75 655f 290a 0a20 2020  end(value_)..   
+000095a0: 2072 6574 7572 6e20 7072 6f70 5f0a 0a0a   return prop_...
+000095b0: 6465 6620 6d61 6b65 5f69 6e74 6567 6572  def make_integer
+000095c0: 5f70 726f 7028 0a20 2020 206e 616d 653a  _prop(.    name:
+000095d0: 2073 7472 2c0a 2020 2020 7661 6c75 653a   str,.    value:
+000095e0: 2055 6e69 6f6e 5b50 726f 7065 7274 7945   Union[PropertyE
+000095f0: 6c65 6d65 6e74 2c20 7374 722c 2069 6e74  lement, str, int
+00009600: 2c20 4974 6572 6162 6c65 5b55 6e69 6f6e  , Iterable[Union
+00009610: 5b50 726f 7065 7274 7945 6c65 6d65 6e74  [PropertyElement
+00009620: 2c20 7374 722c 2069 6e74 5d5d 5d2c 0a20  , str, int]]],. 
+00009630: 2020 2063 616c 6c69 6e67 5f72 6573 6f75     calling_resou
+00009640: 7263 653a 2073 7472 203d 2022 222c 0a29  rce: str = "",.)
+00009650: 202d 3e20 6574 7265 652e 5f45 6c65 6d65   -> etree._Eleme
+00009660: 6e74 3a0a 2020 2020 2222 220a 2020 2020  nt:.    """.    
+00009670: 4d61 6b65 2061 203c 696e 7465 6765 722d  Make a <integer-
+00009680: 7072 6f70 3e20 6672 6f6d 206f 6e65 206f  prop> from one o
+00009690: 7220 6d6f 7265 2069 6e74 6567 6572 732e  r more integers.
+000096a0: 2054 6865 2069 6e74 6567 6572 7320 6361   The integers ca
+000096b0: 6e20 6265 2070 726f 7669 6465 6420 6173  n be provided as
+000096c0: 2073 7472 696e 672c 2069 6e74 6567 6572   string, integer
+000096d0: 2c20 6f72 2061 730a 2020 2020 5072 6f70  , or as.    Prop
+000096e0: 6572 7479 456c 656d 656e 7420 7769 7468  ertyElement with
+000096f0: 2061 2073 7472 696e 672f 696e 7465 6765   a string/intege
+00009700: 7220 696e 7369 6465 2e20 4966 2070 726f  r inside. If pro
+00009710: 7669 6465 6420 6173 2073 7472 696e 672f  vided as string/
+00009720: 696e 7465 6765 722c 2074 6865 2070 6572  integer, the per
+00009730: 6d69 7373 696f 6e73 2064 6566 6175 6c74  missions default
+00009740: 2074 6f0a 2020 2020 2270 726f 702d 6465   to.    "prop-de
+00009750: 6661 756c 7422 2e0a 0a20 2020 2041 7267  fault"...    Arg
+00009760: 733a 0a20 2020 2020 2020 206e 616d 653a  s:.        name:
+00009770: 2074 6865 206e 616d 6520 6f66 2074 6869   the name of thi
+00009780: 7320 7072 6f70 6572 7479 2061 7320 6465  s property as de
+00009790: 6669 6e65 6420 696e 2074 6865 206f 6e74  fined in the ont
+000097a0: 6f0a 2020 2020 2020 2020 7661 6c75 653a  o.        value:
+000097b0: 206f 6e65 206f 7220 6d6f 7265 2069 6e74   one or more int
+000097c0: 6567 6572 732c 2061 7320 7374 7269 6e67  egers, as string
+000097d0: 2f69 6e74 2f50 726f 7065 7274 7945 6c65  /int/PropertyEle
+000097e0: 6d65 6e74 2c20 6f72 2061 7320 6974 6572  ment, or as iter
+000097f0: 6162 6c65 206f 6620 7374 7269 6e67 732f  able of strings/
+00009800: 696e 7473 2f50 726f 7065 7274 7945 6c65  ints/PropertyEle
+00009810: 6d65 6e74 730a 2020 2020 2020 2020 6361  ments.        ca
+00009820: 6c6c 696e 675f 7265 736f 7572 6365 3a20  lling_resource: 
+00009830: 7468 6520 6e61 6d65 206f 6620 7468 6520  the name of the 
+00009840: 7061 7265 6e74 2072 6573 6f75 7263 6520  parent resource 
+00009850: 2866 6f72 2062 6574 7465 7220 6572 726f  (for better erro
+00009860: 7220 6d65 7373 6167 6573 290a 0a20 2020  r messages)..   
+00009870: 2057 6172 6e73 3a0a 2020 2020 2020 2020   Warns:.        
+00009880: 4966 2074 6865 2076 616c 7565 2069 7320  If the value is 
+00009890: 6e6f 7420 6120 7661 6c69 6420 696e 7465  not a valid inte
+000098a0: 6765 720a 0a20 2020 2052 6574 7572 6e73  ger..    Returns
+000098b0: 3a0a 2020 2020 2020 2020 616e 2065 7472  :.        an etr
+000098c0: 6565 2e5f 456c 656d 656e 7420 7468 6174  ee._Element that
+000098d0: 2063 616e 2062 6520 6170 7065 6e64 6564   can be appended
+000098e0: 2074 6f20 7468 6520 7061 7265 6e74 2072   to the parent r
+000098f0: 6573 6f75 7263 6520 7769 7468 2072 6573  esource with res
+00009900: 6f75 7263 652e 6170 7065 6e64 286d 616b  ource.append(mak
+00009910: 655f 2a5f 7072 6f70 282e 2e2e 2929 0a0a  e_*_prop(...))..
+00009920: 2020 2020 4578 616d 706c 6573 3a0a 2020      Examples:.  
+00009930: 2020 2020 2020 3e3e 3e20 6578 6365 6c32        >>> excel2
+00009940: 786d 6c2e 6d61 6b65 5f69 6e74 6567 6572  xml.make_integer
+00009950: 5f70 726f 7028 223a 7465 7374 7072 6f70  _prop(":testprop
+00009960: 6572 7479 222c 2022 3237 3631 3336 3922  erty", "2761369"
+00009970: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00009980: 2020 3c69 6e74 6567 6572 2d70 726f 7020    <integer-prop 
+00009990: 6e61 6d65 3d22 3a74 6573 7470 726f 7065  name=":testprope
+000099a0: 7274 7922 3e0a 2020 2020 2020 2020 2020  rty">.          
+000099b0: 2020 2020 2020 2020 2020 3c69 6e74 6567            <integ
+000099c0: 6572 2070 6572 6d69 7373 696f 6e73 3d22  er permissions="
+000099d0: 7072 6f70 2d64 6566 6175 6c74 223e 3237  prop-default">27
+000099e0: 3631 3336 393c 2f69 6e74 6567 6572 3e0a  61369</integer>.
+000099f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a00: 3c2f 696e 7465 6765 722d 7072 6f70 3e0a  </integer-prop>.
+00009a10: 2020 2020 2020 2020 3e3e 3e20 6578 6365          >>> exce
+00009a20: 6c32 786d 6c2e 6d61 6b65 5f69 6e74 6567  l2xml.make_integ
+00009a30: 6572 5f70 726f 7028 223a 7465 7374 7072  er_prop(":testpr
+00009a40: 6f70 6572 7479 222c 2065 7863 656c 3278  operty", excel2x
+00009a50: 6d6c 2e50 726f 7065 7274 7945 6c65 6d65  ml.PropertyEleme
+00009a60: 6e74 2822 3237 3631 3336 3922 2c20 7065  nt("2761369", pe
+00009a70: 726d 6973 7369 6f6e 733d 2270 726f 702d  rmissions="prop-
+00009a80: 7265 7374 7269 6374 6564 222c 2063 6f6d  restricted", com
+00009a90: 6d65 6e74 3d22 6578 616d 706c 6522 2929  ment="example"))
+00009aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009ab0: 203c 696e 7465 6765 722d 7072 6f70 206e   <integer-prop n
+00009ac0: 616d 653d 223a 7465 7374 7072 6f70 6572  ame=":testproper
+00009ad0: 7479 223e 0a20 2020 2020 2020 2020 2020  ty">.           
+00009ae0: 2020 2020 2020 2020 203c 696e 7465 6765           <intege
+00009af0: 7220 7065 726d 6973 7369 6f6e 733d 2270  r permissions="p
+00009b00: 726f 702d 7265 7374 7269 6374 6564 2220  rop-restricted" 
+00009b10: 636f 6d6d 656e 743d 2265 7861 6d70 6c65  comment="example
+00009b20: 223e 3237 3631 3336 393c 2f69 6e74 6567  ">2761369</integ
+00009b30: 6572 3e0a 2020 2020 2020 2020 2020 2020  er>.            
+00009b40: 2020 2020 3c2f 696e 7465 6765 722d 7072      </integer-pr
+00009b50: 6f70 3e0a 2020 2020 2020 2020 3e3e 3e20  op>.        >>> 
+00009b60: 6578 6365 6c32 786d 6c2e 6d61 6b65 5f69  excel2xml.make_i
+00009b70: 6e74 6567 6572 5f70 726f 7028 223a 7465  nteger_prop(":te
+00009b80: 7374 7072 6f70 6572 7479 222c 205b 2232  stproperty", ["2
+00009b90: 3736 3133 3639 222c 2022 3130 3130 3130  761369", "101010
+00009ba0: 3122 5d29 0a20 2020 2020 2020 2020 2020  1"]).           
+00009bb0: 2020 2020 203c 696e 7465 6765 722d 7072       <integer-pr
+00009bc0: 6f70 206e 616d 653d 223a 7465 7374 7072  op name=":testpr
+00009bd0: 6f70 6572 7479 223e 0a20 2020 2020 2020  operty">.       
+00009be0: 2020 2020 2020 2020 2020 2020 203c 696e               <in
+00009bf0: 7465 6765 7220 7065 726d 6973 7369 6f6e  teger permission
+00009c00: 733d 2270 726f 702d 6465 6661 756c 7422  s="prop-default"
+00009c10: 3e32 3736 3133 3639 3c2f 696e 7465 6765  >2761369</intege
+00009c20: 723e 0a20 2020 2020 2020 2020 2020 2020  r>.             
+00009c30: 2020 2020 2020 203c 696e 7465 6765 7220         <integer 
+00009c40: 7065 726d 6973 7369 6f6e 733d 2270 726f  permissions="pro
+00009c50: 702d 6465 6661 756c 7422 3e31 3031 3031  p-default">10101
+00009c60: 3031 3c2f 696e 7465 6765 723e 0a20 2020  01</integer>.   
+00009c70: 2020 2020 2020 2020 2020 2020 203c 2f69               </i
+00009c80: 6e74 6567 6572 2d70 726f 703e 0a0a 2020  nteger-prop>..  
+00009c90: 2020 5365 6520 6874 7470 733a 2f2f 646f    See https://do
+00009ca0: 6373 2e64 6173 6368 2e73 7769 7373 2f6c  cs.dasch.swiss/l
+00009cb0: 6174 6573 742f 4453 502d 544f 4f4c 532f  atest/DSP-TOOLS/
+00009cc0: 6669 6c65 2d66 6f72 6d61 7473 2f78 6d6c  file-formats/xml
+00009cd0: 2d64 6174 612d 6669 6c65 2f23 696e 7465  -data-file/#inte
+00009ce0: 6765 722d 7072 6f70 0a20 2020 2022 2222  ger-prop.    """
+00009cf0: 0a0a 2020 2020 2320 6368 6563 6b20 7468  ..    # check th
+00009d00: 6520 696e 7075 743a 2070 7265 7061 7265  e input: prepare
+00009d10: 2061 206c 6973 7420 7769 7468 2076 616c   a list with val
+00009d20: 6964 2076 616c 7565 730a 2020 2020 7661  id values.    va
+00009d30: 6c75 6573 203d 2070 7265 7061 7265 5f76  lues = prepare_v
+00009d40: 616c 7565 2876 616c 7565 290a 0a20 2020  alue(value)..   
+00009d50: 2023 2063 6865 636b 2076 616c 7565 2074   # check value t
+00009d60: 7970 650a 2020 2020 666f 7220 7661 6c20  ype.    for val 
+00009d70: 696e 2076 616c 7565 733a 0a20 2020 2020  in values:.     
+00009d80: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00009d90: 2020 2020 696e 7428 7661 6c2e 7661 6c75      int(val.valu
+00009da0: 6529 0a20 2020 2020 2020 2065 7863 6570  e).        excep
+00009db0: 7420 5661 6c75 6545 7272 6f72 3a0a 2020  t ValueError:.  
+00009dc0: 2020 2020 2020 2020 2020 6d73 6720 3d20            msg = 
+00009dd0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00009de0: 2020 6622 4661 696c 6564 2076 616c 6964    f"Failed valid
+00009df0: 6174 696f 6e20 696e 2072 6573 6f75 7263  ation in resourc
+00009e00: 6520 277b 6361 6c6c 696e 675f 7265 736f  e '{calling_reso
+00009e10: 7572 6365 7d27 2c20 7072 6f70 6572 7479  urce}', property
+00009e20: 2027 7b6e 616d 657d 273a 2022 0a20 2020   '{name}': ".   
+00009e30: 2020 2020 2020 2020 2020 2020 2066 2227               f"'
+00009e40: 7b76 616c 2e76 616c 7565 7d27 2069 7320  {val.value}' is 
+00009e50: 6e6f 7420 6120 7661 6c69 6420 696e 7465  not a valid inte
+00009e60: 6765 722e 220a 2020 2020 2020 2020 2020  ger.".          
+00009e70: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00009e80: 7761 726e 696e 6773 2e77 6172 6e28 4473  warnings.warn(Ds
+00009e90: 7054 6f6f 6c73 5573 6572 5761 726e 696e  pToolsUserWarnin
+00009ea0: 6728 6d73 6729 290a 0a20 2020 2023 206d  g(msg))..    # m
+00009eb0: 616b 6520 786d 6c20 7374 7275 6374 7572  ake xml structur
+00009ec0: 6520 6f66 2074 6865 2076 616c 6964 2076  e of the valid v
+00009ed0: 616c 7565 730a 2020 2020 7072 6f70 5f20  alues.    prop_ 
+00009ee0: 3d20 6574 7265 652e 456c 656d 656e 7428  = etree.Element(
+00009ef0: 0a20 2020 2020 2020 2022 7b25 737d 696e  .        "{%s}in
+00009f00: 7465 6765 722d 7072 6f70 2220 2520 786d  teger-prop" % xm
+00009f10: 6c5f 6e61 6d65 7370 6163 655f 6d61 705b  l_namespace_map[
+00009f20: 4e6f 6e65 5d2c 0a20 2020 2020 2020 206e  None],.        n
+00009f30: 616d 653d 6e61 6d65 2c0a 2020 2020 2020  ame=name,.      
+00009f40: 2020 6e73 6d61 703d 786d 6c5f 6e61 6d65    nsmap=xml_name
+00009f50: 7370 6163 655f 6d61 702c 0a20 2020 2029  space_map,.    )
+00009f60: 0a20 2020 2066 6f72 2076 616c 2069 6e20  .    for val in 
+00009f70: 7661 6c75 6573 3a0a 2020 2020 2020 2020  values:.        
+00009f80: 6b77 6172 6773 203d 207b 2270 6572 6d69  kwargs = {"permi
+00009f90: 7373 696f 6e73 223a 2076 616c 2e70 6572  ssions": val.per
+00009fa0: 6d69 7373 696f 6e73 7d0a 2020 2020 2020  missions}.      
+00009fb0: 2020 6966 2076 616c 2e63 6f6d 6d65 6e74    if val.comment
+00009fc0: 2061 6e64 2063 6865 636b 5f6e 6f74 6e61   and check_notna
+00009fd0: 2876 616c 2e63 6f6d 6d65 6e74 293a 0a20  (val.comment):. 
+00009fe0: 2020 2020 2020 2020 2020 206b 7761 7267             kwarg
+00009ff0: 735b 2263 6f6d 6d65 6e74 225d 203d 2076  s["comment"] = v
+0000a000: 616c 2e63 6f6d 6d65 6e74 0a20 2020 2020  al.comment.     
+0000a010: 2020 2076 616c 7565 5f20 3d20 6574 7265     value_ = etre
+0000a020: 652e 456c 656d 656e 7428 0a20 2020 2020  e.Element(.     
+0000a030: 2020 2020 2020 2022 7b25 737d 696e 7465         "{%s}inte
+0000a040: 6765 7222 2025 2078 6d6c 5f6e 616d 6573  ger" % xml_names
+0000a050: 7061 6365 5f6d 6170 5b4e 6f6e 655d 2c0a  pace_map[None],.
+0000a060: 2020 2020 2020 2020 2020 2020 2a2a 6b77              **kw
+0000a070: 6172 6773 2c20 2023 2074 7970 653a 2069  args,  # type: i
+0000a080: 676e 6f72 655b 6172 672d 7479 7065 5d0a  gnore[arg-type].
+0000a090: 2020 2020 2020 2020 2020 2020 6e73 6d61              nsma
+0000a0a0: 703d 786d 6c5f 6e61 6d65 7370 6163 655f  p=xml_namespace_
+0000a0b0: 6d61 702c 0a20 2020 2020 2020 2029 0a20  map,.        ). 
+0000a0c0: 2020 2020 2020 2076 616c 7565 5f2e 7465         value_.te
+0000a0d0: 7874 203d 2073 7472 2876 616c 2e76 616c  xt = str(val.val
+0000a0e0: 7565 290a 2020 2020 2020 2020 7072 6f70  ue).        prop
+0000a0f0: 5f2e 6170 7065 6e64 2876 616c 7565 5f29  _.append(value_)
+0000a100: 0a0a 2020 2020 7265 7475 726e 2070 726f  ..    return pro
+0000a110: 705f 0a0a 0a64 6566 206d 616b 655f 696e  p_...def make_in
+0000a120: 7465 7276 616c 5f70 726f 7028 6e61 6d65  terval_prop(name
+0000a130: 3a20 7374 722c 2076 616c 7565 3a20 556e  : str, value: Un
+0000a140: 696f 6e5b 5072 6f70 6572 7479 456c 656d  ion[PropertyElem
+0000a150: 656e 742c 2073 7472 5d2c 2063 616c 6c69  ent, str], calli
+0000a160: 6e67 5f72 6573 6f75 7263 653a 2073 7472  ng_resource: str
+0000a170: 203d 2022 2229 202d 3e20 6574 7265 652e   = "") -> etree.
+0000a180: 5f45 6c65 6d65 6e74 3a0a 2020 2020 2222  _Element:.    ""
+0000a190: 220a 2020 2020 4d61 6b65 2061 203c 696e  ".    Make a <in
+0000a1a0: 7465 7276 616c 2d70 726f 7020 6e61 6d65  terval-prop name
+0000a1b0: 3d22 6861 7353 6567 6d65 6e74 426f 756e  ="hasSegmentBoun
+0000a1c0: 6473 223e 2066 6f72 2061 203c 7669 6465  ds"> for a <vide
+0000a1d0: 6f2d 7365 676d 656e 743e 206f 7220 3c61  o-segment> or <a
+0000a1e0: 7564 696f 2d73 6567 6d65 6e74 3e2e 0a20  udio-segment>.. 
+0000a1f0: 2020 2054 6865 2069 6e74 6572 7661 6c20     The interval 
+0000a200: 6361 6e20 6265 2070 726f 7669 6465 6420  can be provided 
+0000a210: 6173 2073 7472 696e 6720 6f72 2061 7320  as string or as 
+0000a220: 5072 6f70 6572 7479 456c 656d 656e 7420  PropertyElement 
+0000a230: 7769 7468 2061 2073 7472 696e 6720 696e  with a string in
+0000a240: 7369 6465 2e0a 2020 2020 4966 2070 726f  side..    If pro
+0000a250: 7669 6465 6420 6173 2073 7472 696e 672c  vided as string,
+0000a260: 2074 6865 2070 6572 6d69 7373 696f 6e73   the permissions
+0000a270: 2064 6566 6175 6c74 2074 6f20 2270 726f   default to "pro
+0000a280: 702d 6465 6661 756c 7422 2e0a 2020 2020  p-default"..    
+0000a290: 4453 5020 696e 7465 7276 616c 2076 616c  DSP interval val
+0000a2a0: 7565 7320 6172 6520 666f 726d 6174 7465  ues are formatte
+0000a2b0: 6420 6173 2022 7374 6172 745f 7365 636f  d as "start_seco
+0000a2c0: 6e64 733a 656e 645f 7365 636f 6e64 7322  nds:end_seconds"
+0000a2d0: 2e0a 2020 2020 426f 7468 206e 756d 6265  ..    Both numbe
+0000a2e0: 7273 2063 616e 2068 6176 6520 6120 6465  rs can have a de
+0000a2f0: 6369 6d61 6c20 706f 696e 742c 2066 6f72  cimal point, for
+0000a300: 2066 7261 6374 696f 6e73 206f 6620 7365   fractions of se
+0000a310: 636f 6e64 732e 0a0a 2020 2020 4172 6773  conds...    Args
+0000a320: 3a0a 2020 2020 2020 2020 6e61 6d65 3a20  :.        name: 
+0000a330: 7468 6520 6e61 6d65 206f 6620 7468 6973  the name of this
+0000a340: 2070 726f 7065 7274 792e 2054 6865 206f   property. The o
+0000a350: 6e6c 7920 6163 6365 7074 6564 2076 616c  nly accepted val
+0000a360: 7565 2069 7320 2268 6173 5365 676d 656e  ue is "hasSegmen
+0000a370: 7442 6f75 6e64 7322 0a20 2020 2020 2020  tBounds".       
+0000a380: 2076 616c 7565 3a20 6120 4453 5020 696e   value: a DSP in
+0000a390: 7465 7276 616c 2c20 6173 2073 7472 696e  terval, as strin
+0000a3a0: 6720 6f72 2050 726f 7065 7274 7945 6c65  g or PropertyEle
+0000a3b0: 6d65 6e74 0a20 2020 2020 2020 2063 616c  ment.        cal
+0000a3c0: 6c69 6e67 5f72 6573 6f75 7263 653a 2074  ling_resource: t
+0000a3d0: 6865 206e 616d 6520 6f66 2074 6865 2070  he name of the p
+0000a3e0: 6172 656e 7420 7265 736f 7572 6365 2028  arent resource (
+0000a3f0: 666f 7220 6265 7474 6572 2065 7272 6f72  for better error
+0000a400: 206d 6573 7361 6765 7329 0a0a 2020 2020   messages)..    
+0000a410: 5761 726e 733a 0a20 2020 2020 2020 202d  Warns:.        -
+0000a420: 2049 6620 7468 6520 7661 6c75 6520 6973   If the value is
+0000a430: 206e 6f74 2061 2076 616c 6964 2044 5350   not a valid DSP
+0000a440: 2069 6e74 6572 7661 6c0a 2020 2020 2020   interval.      
+0000a450: 2020 2d20 4966 2074 6865 206e 616d 6520    - If the name 
+0000a460: 6973 206e 6f74 2022 6861 7353 6567 6d65  is not "hasSegme
+0000a470: 6e74 426f 756e 6473 220a 0a20 2020 2052  ntBounds"..    R
+0000a480: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+0000a490: 616e 2065 7472 6565 2e5f 456c 656d 656e  an etree._Elemen
+0000a4a0: 7420 7468 6174 2063 616e 2062 6520 6170  t that can be ap
+0000a4b0: 7065 6e64 6564 2074 6f20 7468 6520 7061  pended to the pa
+0000a4c0: 7265 6e74 2072 6573 6f75 7263 6520 7769  rent resource wi
+0000a4d0: 7468 2072 6573 6f75 7263 652e 6170 7065  th resource.appe
+0000a4e0: 6e64 286d 616b 655f 2a5f 7072 6f70 282e  nd(make_*_prop(.
+0000a4f0: 2e2e 2929 0a0a 2020 2020 4578 616d 706c  ..))..    Exampl
+0000a500: 6573 3a0a 2020 2020 2020 2020 3e3e 3e20  es:.        >>> 
+0000a510: 696e 7465 7276 616c 203d 2065 7863 656c  interval = excel
+0000a520: 3278 6d6c 2e63 7265 6174 655f 696e 7465  2xml.create_inte
+0000a530: 7276 616c 5f76 616c 7565 2873 7461 7274  rval_value(start
+0000a540: 3d22 303a 3031 3a30 3022 2c20 656e 643d  ="0:01:00", end=
+0000a550: 2230 3a30 323a 3030 2229 2020 2320 7265  "0:02:00")  # re
+0000a560: 7375 6c74 3a20 2236 303a 3132 3022 0a20  sult: "60:120". 
+0000a570: 2020 2020 2020 203e 3e3e 2065 7863 656c         >>> excel
+0000a580: 3278 6d6c 2e6d 616b 655f 696e 7465 7276  2xml.make_interv
+0000a590: 616c 5f70 726f 7028 2268 6173 5365 676d  al_prop("hasSegm
+0000a5a0: 656e 7442 6f75 6e64 7322 2c20 696e 7665  entBounds", inve
+0000a5b0: 7276 616c 290a 2020 2020 2020 2020 2020  rval).          
+0000a5c0: 2020 2020 2020 3c69 6e74 6572 7661 6c2d        <interval-
+0000a5d0: 7072 6f70 206e 616d 653d 2268 6173 5365  prop name="hasSe
+0000a5e0: 676d 656e 7442 6f75 6e64 7322 3e0a 2020  gmentBounds">.  
+0000a5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a600: 2020 3c69 6e74 6572 7661 6c20 7065 726d    <interval perm
+0000a610: 6973 7369 6f6e 733d 2270 726f 702d 6465  issions="prop-de
+0000a620: 6661 756c 7422 3e36 303a 3132 303c 2f69  fault">60:120</i
+0000a630: 6e74 6572 7661 6c3e 0a20 2020 2020 2020  nterval>.       
+0000a640: 2020 2020 2020 2020 203c 2f69 6e74 6572           </inter
+0000a650: 7661 6c2d 7072 6f70 3e0a 2020 2020 2020  val-prop>.      
+0000a660: 2020 3e3e 3e20 696e 7465 7276 616c 203d    >>> interval =
+0000a670: 2065 7863 656c 3278 6d6c 2e63 7265 6174   excel2xml.creat
+0000a680: 655f 696e 7465 7276 616c 5f76 616c 7565  e_interval_value
+0000a690: 2873 7461 7274 3d22 303a 3330 3a30 3022  (start="0:30:00"
+0000a6a0: 2c20 656e 643d 2231 3a30 303a 3030 2229  , end="1:00:00")
+0000a6b0: 2020 2320 7265 7375 6c74 3a20 2231 3830    # result: "180
+0000a6c0: 303a 3336 3030 220a 2020 2020 2020 2020  0:3600".        
+0000a6d0: 3e3e 3e20 6578 6365 6c32 786d 6c2e 6d61  >>> excel2xml.ma
+0000a6e0: 6b65 5f69 6e74 6572 7661 6c5f 7072 6f70  ke_interval_prop
+0000a6f0: 2822 6861 7353 6567 6d65 6e74 426f 756e  ("hasSegmentBoun
+0000a700: 6473 222c 2065 7863 656c 3278 6d6c 2e50  ds", excel2xml.P
+0000a710: 726f 7065 7274 7945 6c65 6d65 6e74 2869  ropertyElement(i
+0000a720: 6e74 6572 7661 6c2c 2070 6572 6d69 7373  nterval, permiss
+0000a730: 696f 6e73 3d22 7072 6f70 2d72 6573 7472  ions="prop-restr
+0000a740: 6963 7465 6422 2c20 636f 6d6d 656e 743d  icted", comment=
+0000a750: 2265 7861 6d70 6c65 2229 290a 2020 2020  "example")).    
+0000a760: 2020 2020 2020 2020 2020 2020 3c69 6e74              <int
+0000a770: 6572 7661 6c2d 7072 6f70 206e 616d 653d  erval-prop name=
+0000a780: 2268 6173 5365 676d 656e 7442 6f75 6e64  "hasSegmentBound
+0000a790: 733e 0a20 2020 2020 2020 2020 2020 2020  s>.             
+0000a7a0: 2020 2020 2020 203c 696e 7465 7276 616c         <interval
+0000a7b0: 2070 6572 6d69 7373 696f 6e73 3d22 7072   permissions="pr
+0000a7c0: 6f70 2d72 6573 7472 6963 7465 6422 2063  op-restricted" c
+0000a7d0: 6f6d 6d65 6e74 3d22 6578 616d 706c 6522  omment="example"
+0000a7e0: 3e31 3830 303a 3336 3030 3c2f 696e 7465  >1800:3600</inte
+0000a7f0: 7276 616c 3e0a 2020 2020 2020 2020 2020  rval>.          
+0000a800: 2020 2020 2020 3c2f 696e 7465 7276 616c        </interval
+0000a810: 2d70 726f 703e 0a0a 2020 2020 5365 6520  -prop>..    See 
+0000a820: 6874 7470 733a 2f2f 646f 6373 2e64 6173  https://docs.das
+0000a830: 6368 2e73 7769 7373 2f6c 6174 6573 742f  ch.swiss/latest/
+0000a840: 4453 502d 544f 4f4c 532f 6669 6c65 2d66  DSP-TOOLS/file-f
+0000a850: 6f72 6d61 7473 2f78 6d6c 2d64 6174 612d  ormats/xml-data-
+0000a860: 6669 6c65 2f23 7669 6465 6f2d 7365 676d  file/#video-segm
+0000a870: 656e 742d 6175 6469 6f2d 7365 676d 656e  ent-audio-segmen
+0000a880: 740a 2020 2020 2222 220a 0a20 2020 2069  t.    """..    i
+0000a890: 6620 6e61 6d65 2021 3d20 2268 6173 5365  f name != "hasSe
+0000a8a0: 676d 656e 7442 6f75 6e64 7322 3a0a 2020  gmentBounds":.  
+0000a8b0: 2020 2020 2020 6d73 6720 3d20 280a 2020        msg = (.  
+0000a8c0: 2020 2020 2020 2020 2020 6622 4661 696c            f"Fail
+0000a8d0: 6564 2076 616c 6964 6174 696f 6e20 696e  ed validation in
+0000a8e0: 2072 6573 6f75 7263 6520 277b 6361 6c6c   resource '{call
+0000a8f0: 696e 675f 7265 736f 7572 6365 7d27 2c20  ing_resource}', 
+0000a900: 7072 6f70 6572 7479 2027 7b6e 616d 657d  property '{name}
+0000a910: 273a 2022 0a20 2020 2020 2020 2020 2020  ': ".           
+0000a920: 2066 2254 6865 206f 6e6c 7920 6163 6365   f"The only acce
+0000a930: 7074 6564 2076 616c 7565 2066 6f72 2027  pted value for '
+0000a940: 6e61 6d65 2720 6973 2027 6861 7353 6567  name' is 'hasSeg
+0000a950: 6d65 6e74 426f 756e 6473 272e 220a 2020  mentBounds'.".  
+0000a960: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000a970: 7761 726e 696e 6773 2e77 6172 6e28 4473  warnings.warn(Ds
+0000a980: 7054 6f6f 6c73 5573 6572 5761 726e 696e  pToolsUserWarnin
+0000a990: 6728 6d73 6729 290a 0a20 2020 2076 616c  g(msg))..    val
+0000a9a0: 7565 203d 2076 616c 7565 2069 6620 6973  ue = value if is
+0000a9b0: 696e 7374 616e 6365 2876 616c 7565 2c20  instance(value, 
+0000a9c0: 5072 6f70 6572 7479 456c 656d 656e 7429  PropertyElement)
+0000a9d0: 2065 6c73 6520 5072 6f70 6572 7479 456c   else PropertyEl
+0000a9e0: 656d 656e 7428 7661 6c75 6529 0a0a 2020  ement(value)..  
+0000a9f0: 2020 2320 6368 6563 6b20 7661 6c75 6520    # check value 
+0000aa00: 7479 7065 0a20 2020 2069 6620 6e6f 7420  type.    if not 
+0000aa10: 7265 6765 782e 6d61 7463 6828 7222 5c64  regex.match(r"\d
+0000aa20: 2b28 5c2e 5c64 2b29 3f3a 5c64 2b28 5c2e  +(\.\d+)?:\d+(\.
+0000aa30: 5c64 2b29 3f22 2c20 7374 7228 7661 6c75  \d+)?", str(valu
+0000aa40: 652e 7661 6c75 6529 293a 0a20 2020 2020  e.value)):.     
+0000aa50: 2020 206d 7367 203d 2028 0a20 2020 2020     msg = (.     
+0000aa60: 2020 2020 2020 2066 2246 6169 6c65 6420         f"Failed 
+0000aa70: 7661 6c69 6461 7469 6f6e 2069 6e20 7265  validation in re
+0000aa80: 736f 7572 6365 2027 7b63 616c 6c69 6e67  source '{calling
+0000aa90: 5f72 6573 6f75 7263 657d 272c 2070 726f  _resource}', pro
+0000aaa0: 7065 7274 7920 277b 6e61 6d65 7d27 3a20  perty '{name}': 
+0000aab0: 220a 2020 2020 2020 2020 2020 2020 6622  ".            f"
+0000aac0: 277b 7661 6c75 652e 7661 6c75 657d 2720  '{value.value}' 
+0000aad0: 6973 206e 6f74 2061 2076 616c 6964 2044  is not a valid D
+0000aae0: 5350 2069 6e74 6572 7661 6c2e 220a 2020  SP interval.".  
+0000aaf0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000ab00: 7761 726e 696e 6773 2e77 6172 6e28 4473  warnings.warn(Ds
+0000ab10: 7054 6f6f 6c73 5573 6572 5761 726e 696e  pToolsUserWarnin
+0000ab20: 6728 6d73 6729 290a 0a20 2020 2023 206d  g(msg))..    # m
+0000ab30: 616b 6520 786d 6c20 7374 7275 6374 7572  ake xml structur
+0000ab40: 6520 6f66 2074 6865 2076 616c 6964 2076  e of the valid v
+0000ab50: 616c 7565 730a 2020 2020 7072 6f70 5f20  alues.    prop_ 
+0000ab60: 3d20 6574 7265 652e 456c 656d 656e 7428  = etree.Element(
+0000ab70: 0a20 2020 2020 2020 2022 7b25 737d 696e  .        "{%s}in
+0000ab80: 7465 7276 616c 2d70 726f 7022 2025 2078  terval-prop" % x
+0000ab90: 6d6c 5f6e 616d 6573 7061 6365 5f6d 6170  ml_namespace_map
+0000aba0: 5b4e 6f6e 655d 2c0a 2020 2020 2020 2020  [None],.        
+0000abb0: 6e61 6d65 3d6e 616d 652c 0a20 2020 2020  name=name,.     
+0000abc0: 2020 206e 736d 6170 3d78 6d6c 5f6e 616d     nsmap=xml_nam
+0000abd0: 6573 7061 6365 5f6d 6170 2c0a 2020 2020  espace_map,.    
+0000abe0: 290a 2020 2020 6b77 6172 6773 203d 207b  ).    kwargs = {
+0000abf0: 2270 6572 6d69 7373 696f 6e73 223a 2076  "permissions": v
+0000ac00: 616c 7565 2e70 6572 6d69 7373 696f 6e73  alue.permissions
+0000ac10: 7d0a 2020 2020 6966 2076 616c 7565 2e63  }.    if value.c
+0000ac20: 6f6d 6d65 6e74 2061 6e64 2063 6865 636b  omment and check
+0000ac30: 5f6e 6f74 6e61 2876 616c 7565 2e63 6f6d  _notna(value.com
+0000ac40: 6d65 6e74 293a 0a20 2020 2020 2020 206b  ment):.        k
+0000ac50: 7761 7267 735b 2263 6f6d 6d65 6e74 225d  wargs["comment"]
+0000ac60: 203d 2076 616c 7565 2e63 6f6d 6d65 6e74   = value.comment
+0000ac70: 0a20 2020 2076 616c 7565 5f20 3d20 6574  .    value_ = et
+0000ac80: 7265 652e 456c 656d 656e 7428 0a20 2020  ree.Element(.   
+0000ac90: 2020 2020 2022 7b25 737d 696e 7465 7276       "{%s}interv
+0000aca0: 616c 2220 2520 786d 6c5f 6e61 6d65 7370  al" % xml_namesp
+0000acb0: 6163 655f 6d61 705b 4e6f 6e65 5d2c 0a20  ace_map[None],. 
+0000acc0: 2020 2020 2020 202a 2a6b 7761 7267 732c         **kwargs,
+0000acd0: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
+0000ace0: 5b61 7267 2d74 7970 655d 0a20 2020 2020  [arg-type].     
+0000acf0: 2020 206e 736d 6170 3d78 6d6c 5f6e 616d     nsmap=xml_nam
+0000ad00: 6573 7061 6365 5f6d 6170 2c0a 2020 2020  espace_map,.    
+0000ad10: 290a 2020 2020 7661 6c75 655f 2e74 6578  ).    value_.tex
+0000ad20: 7420 3d20 7374 7228 7661 6c75 652e 7661  t = str(value.va
+0000ad30: 6c75 6529 0a20 2020 2070 726f 705f 2e61  lue).    prop_.a
+0000ad40: 7070 656e 6428 7661 6c75 655f 290a 0a20  ppend(value_).. 
+0000ad50: 2020 2072 6574 7572 6e20 7072 6f70 5f0a     return prop_.
+0000ad60: 0a0a 6465 6620 6d61 6b65 5f6c 6973 745f  ..def make_list_
+0000ad70: 7072 6f70 280a 2020 2020 6c69 7374 5f6e  prop(.    list_n
+0000ad80: 616d 653a 2073 7472 2c0a 2020 2020 6e61  ame: str,.    na
+0000ad90: 6d65 3a20 7374 722c 0a20 2020 2076 616c  me: str,.    val
+0000ada0: 7565 3a20 556e 696f 6e5b 5072 6f70 6572  ue: Union[Proper
+0000adb0: 7479 456c 656d 656e 742c 2073 7472 2c20  tyElement, str, 
+0000adc0: 4974 6572 6162 6c65 5b55 6e69 6f6e 5b50  Iterable[Union[P
+0000add0: 726f 7065 7274 7945 6c65 6d65 6e74 2c20  ropertyElement, 
+0000ade0: 7374 725d 5d5d 2c0a 2020 2020 6361 6c6c  str]]],.    call
+0000adf0: 696e 675f 7265 736f 7572 6365 3a20 7374  ing_resource: st
+0000ae00: 7220 3d20 2222 2c0a 2920 2d3e 2065 7472  r = "",.) -> etr
+0000ae10: 6565 2e5f 456c 656d 656e 743a 0a20 2020  ee._Element:.   
+0000ae20: 2022 2222 0a20 2020 204d 616b 6520 6120   """.    Make a 
+0000ae30: 3c6c 6973 742d 7072 6f70 3e20 6672 6f6d  <list-prop> from
+0000ae40: 206f 6e65 206f 7220 6d6f 7265 206c 6973   one or more lis
+0000ae50: 7420 6e6f 6465 732e 2054 6865 206e 616d  t nodes. The nam
+0000ae60: 6528 7329 206f 6620 7468 6520 6c69 7374  e(s) of the list
+0000ae70: 206e 6f64 6528 7329 2063 616e 2062 6520   node(s) can be 
+0000ae80: 7072 6f76 6964 6564 2061 7320 7374 7269  provided as stri
+0000ae90: 6e67 206f 7220 6173 0a20 2020 2050 726f  ng or as.    Pro
+0000aea0: 7065 7274 7945 6c65 6d65 6e74 2077 6974  pertyElement wit
+0000aeb0: 6820 6120 7374 7269 6e67 2069 6e73 6964  h a string insid
+0000aec0: 652e 2049 6620 7072 6f76 6964 6564 2061  e. If provided a
+0000aed0: 7320 7374 7269 6e67 2c20 7468 6520 7065  s string, the pe
+0000aee0: 726d 6973 7369 6f6e 7320 6465 6661 756c  rmissions defaul
+0000aef0: 7420 746f 2022 7072 6f70 2d64 6566 6175  t to "prop-defau
+0000af00: 6c74 222e 0a0a 2020 2020 4172 6773 3a0a  lt"...    Args:.
+0000af10: 2020 2020 2020 2020 6c69 7374 5f6e 616d          list_nam
+0000af20: 653a 2074 6865 206e 616d 6520 6f66 2074  e: the name of t
+0000af30: 6865 206c 6973 7420 6173 2064 6566 696e  he list as defin
+0000af40: 6564 2069 6e20 7468 6520 6f6e 746f 0a20  ed in the onto. 
+0000af50: 2020 2020 2020 206e 616d 653a 2074 6865         name: the
+0000af60: 206e 616d 6520 6f66 2074 6869 7320 7072   name of this pr
+0000af70: 6f70 6572 7479 2061 7320 6465 6669 6e65  operty as define
+0000af80: 6420 696e 2074 6865 206f 6e74 6f0a 2020  d in the onto.  
+0000af90: 2020 2020 2020 7661 6c75 653a 206f 6e65        value: one
+0000afa0: 206f 7220 6d6f 7265 206e 6f64 6520 6e61   or more node na
+0000afb0: 6d65 732c 2061 7320 7374 7269 6e67 2f50  mes, as string/P
+0000afc0: 726f 7065 7274 7945 6c65 6d65 6e74 2c20  ropertyElement, 
+0000afd0: 6f72 2061 7320 6974 6572 6162 6c65 206f  or as iterable o
+0000afe0: 6620 7374 7269 6e67 732f 5072 6f70 6572  f strings/Proper
+0000aff0: 7479 456c 656d 656e 7473 0a20 2020 2020  tyElements.     
+0000b000: 2020 2063 616c 6c69 6e67 5f72 6573 6f75     calling_resou
+0000b010: 7263 653a 2074 6865 206e 616d 6520 6f66  rce: the name of
+0000b020: 2074 6865 2070 6172 656e 7420 7265 736f   the parent reso
+0000b030: 7572 6365 2028 666f 7220 6265 7474 6572  urce (for better
+0000b040: 2065 7272 6f72 206d 6573 7361 6765 7329   error messages)
+0000b050: 0a0a 2020 2020 5761 726e 733a 0a20 2020  ..    Warns:.   
+0000b060: 2020 2020 2049 6620 7468 6520 6e61 6d65       If the name
+0000b070: 206f 6620 6f6e 6520 6f66 2074 6865 206c   of one of the l
+0000b080: 6973 7420 6e6f 6465 7320 6973 206e 6f74  ist nodes is not
+0000b090: 2061 2076 616c 6964 2073 7472 696e 670a   a valid string.
+0000b0a0: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
+0000b0b0: 2020 2020 2020 616e 2065 7472 6565 2e5f        an etree._
+0000b0c0: 456c 656d 656e 7420 7468 6174 2063 616e  Element that can
+0000b0d0: 2062 6520 6170 7065 6e64 6564 2074 6f20   be appended to 
+0000b0e0: 7468 6520 7061 7265 6e74 2072 6573 6f75  the parent resou
+0000b0f0: 7263 6520 7769 7468 2072 6573 6f75 7263  rce with resourc
+0000b100: 652e 6170 7065 6e64 286d 616b 655f 2a5f  e.append(make_*_
+0000b110: 7072 6f70 282e 2e2e 2929 0a0a 2020 2020  prop(...))..    
+0000b120: 4578 616d 706c 6573 3a0a 2020 2020 2020  Examples:.      
+0000b130: 2020 3e3e 3e20 6578 6365 6c32 786d 6c2e    >>> excel2xml.
+0000b140: 6d61 6b65 5f6c 6973 745f 7072 6f70 2822  make_list_prop("
+0000b150: 6d79 6c69 7374 222c 2022 3a74 6573 7470  mylist", ":testp
+0000b160: 726f 7065 7274 7922 2c20 2266 6972 7374  roperty", "first
+0000b170: 5f6e 6f64 6522 290a 2020 2020 2020 2020  _node").        
+0000b180: 2020 2020 2020 2020 3c6c 6973 742d 7072          <list-pr
+0000b190: 6f70 206c 6973 743d 226d 796c 6973 7422  op list="mylist"
+0000b1a0: 206e 616d 653d 223a 7465 7374 7072 6f70   name=":testprop
+0000b1b0: 6572 7479 223e 0a20 2020 2020 2020 2020  erty">.         
+0000b1c0: 2020 2020 2020 2020 2020 203c 6c69 7374             <list
+0000b1d0: 2070 6572 6d69 7373 696f 6e73 3d22 7072   permissions="pr
+0000b1e0: 6f70 2d64 6566 6175 6c74 223e 6669 7273  op-default">firs
+0000b1f0: 745f 6e6f 6465 3c2f 6c69 7374 3e0a 2020  t_node</list>.  
+0000b200: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+0000b210: 6c69 7374 2d70 726f 703e 0a20 2020 2020  list-prop>.     
+0000b220: 2020 203e 3e3e 2065 7863 656c 3278 6d6c     >>> excel2xml
+0000b230: 2e6d 616b 655f 6c69 7374 5f70 726f 7028  .make_list_prop(
+0000b240: 226d 796c 6973 7422 2c20 223a 7465 7374  "mylist", ":test
+0000b250: 7072 6f70 6572 7479 222c 2065 7863 656c  property", excel
+0000b260: 3278 6d6c 2e50 726f 7065 7274 7945 6c65  2xml.PropertyEle
+0000b270: 6d65 6e74 2822 6669 7273 745f 6e6f 6465  ment("first_node
+0000b280: 222c 2070 6572 6d69 7373 696f 6e73 3d22  ", permissions="
+0000b290: 7072 6f70 2d72 6573 7472 6963 7465 6422  prop-restricted"
+0000b2a0: 2c20 636f 6d6d 656e 743d 2265 7861 6d70  , comment="examp
+0000b2b0: 6c65 2229 290a 2020 2020 2020 2020 2020  le")).          
+0000b2c0: 2020 2020 2020 3c6c 6973 742d 7072 6f70        <list-prop
+0000b2d0: 206c 6973 743d 226d 796c 6973 7422 206e   list="mylist" n
+0000b2e0: 616d 653d 223a 7465 7374 7072 6f70 6572  ame=":testproper
+0000b2f0: 7479 223e 0a20 2020 2020 2020 2020 2020  ty">.           
+0000b300: 2020 2020 2020 2020 203c 6c69 7374 2070           <list p
+0000b310: 6572 6d69 7373 696f 6e73 3d22 7072 6f70  ermissions="prop
+0000b320: 2d72 6573 7472 6963 7465 6422 2063 6f6d  -restricted" com
+0000b330: 6d65 6e74 3d22 6578 616d 706c 6522 3e66  ment="example">f
+0000b340: 6972 7374 5f6e 6f64 653c 2f6c 6973 743e  irst_node</list>
+0000b350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b360: 203c 2f6c 6973 742d 7072 6f70 3e0a 2020   </list-prop>.  
+0000b370: 2020 2020 2020 3e3e 3e20 6578 6365 6c32        >>> excel2
+0000b380: 786d 6c2e 6d61 6b65 5f6c 6973 745f 7072  xml.make_list_pr
+0000b390: 6f70 2822 6d79 6c69 7374 222c 2022 3a74  op("mylist", ":t
+0000b3a0: 6573 7470 726f 7065 7274 7922 2c20 5b22  estproperty", ["
+0000b3b0: 6669 7273 745f 6e6f 6465 222c 2022 7365  first_node", "se
+0000b3c0: 636f 6e64 5f6e 6f64 6522 5d29 0a20 2020  cond_node"]).   
+0000b3d0: 2020 2020 2020 2020 2020 2020 203c 6c69               <li
+0000b3e0: 7374 2d70 726f 7020 6c69 7374 3d22 6d79  st-prop list="my
+0000b3f0: 6c69 7374 2220 6e61 6d65 3d22 3a74 6573  list" name=":tes
+0000b400: 7470 726f 7065 7274 7922 3e0a 2020 2020  tproperty">.    
+0000b410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b420: 3c6c 6973 7420 7065 726d 6973 7369 6f6e  <list permission
+0000b430: 733d 2270 726f 702d 6465 6661 756c 7422  s="prop-default"
+0000b440: 3e66 6972 7374 5f6e 6f64 653c 2f6c 6973  >first_node</lis
+0000b450: 743e 0a20 2020 2020 2020 2020 2020 2020  t>.             
+0000b460: 2020 2020 2020 203c 6c69 7374 2070 6572         <list per
+0000b470: 6d69 7373 696f 6e73 3d22 7072 6f70 2d64  missions="prop-d
+0000b480: 6566 6175 6c74 223e 7365 636f 6e64 5f6e  efault">second_n
+0000b490: 6f64 653c 2f6c 6973 743e 0a20 2020 2020  ode</list>.     
+0000b4a0: 2020 2020 2020 2020 2020 203c 2f6c 6973             </lis
+0000b4b0: 742d 7072 6f70 3e0a 0a20 2020 2053 6565  t-prop>..    See
+0000b4c0: 2068 7474 7073 3a2f 2f64 6f63 732e 6461   https://docs.da
+0000b4d0: 7363 682e 7377 6973 732f 6c61 7465 7374  sch.swiss/latest
+0000b4e0: 2f44 5350 2d54 4f4f 4c53 2f66 696c 652d  /DSP-TOOLS/file-
+0000b4f0: 666f 726d 6174 732f 786d 6c2d 6461 7461  formats/xml-data
+0000b500: 2d66 696c 652f 236c 6973 742d 7072 6f70  -file/#list-prop
+0000b510: 0a20 2020 2022 2222 0a0a 2020 2020 2320  .    """..    # 
+0000b520: 6368 6563 6b20 7468 6520 696e 7075 743a  check the input:
+0000b530: 2070 7265 7061 7265 2061 206c 6973 7420   prepare a list 
+0000b540: 7769 7468 2076 616c 6964 2076 616c 7565  with valid value
+0000b550: 730a 2020 2020 7661 6c75 6573 203d 2070  s.    values = p
+0000b560: 7265 7061 7265 5f76 616c 7565 2876 616c  repare_value(val
+0000b570: 7565 290a 0a20 2020 2023 2063 6865 636b  ue)..    # check
+0000b580: 2076 616c 7565 2074 7970 650a 2020 2020   value type.    
+0000b590: 666f 7220 7661 6c20 696e 2076 616c 7565  for val in value
+0000b5a0: 733a 0a20 2020 2020 2020 2069 6620 6e6f  s:.        if no
+0000b5b0: 7420 6973 696e 7374 616e 6365 2876 616c  t isinstance(val
+0000b5c0: 2e76 616c 7565 2c20 7374 7229 206f 7220  .value, str) or 
+0000b5d0: 6e6f 7420 6368 6563 6b5f 6e6f 746e 6128  not check_notna(
+0000b5e0: 7661 6c2e 7661 6c75 6529 3a0a 2020 2020  val.value):.    
+0000b5f0: 2020 2020 2020 2020 6d73 6720 3d20 280a          msg = (.
+0000b600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b610: 6622 4661 696c 6564 2076 616c 6964 6174  f"Failed validat
+0000b620: 696f 6e20 696e 2072 6573 6f75 7263 6520  ion in resource 
+0000b630: 277b 6361 6c6c 696e 675f 7265 736f 7572  '{calling_resour
+0000b640: 6365 7d27 2c20 7072 6f70 6572 7479 2027  ce}', property '
+0000b650: 7b6e 616d 657d 273a 2022 0a20 2020 2020  {name}': ".     
+0000b660: 2020 2020 2020 2020 2020 2066 2227 7b76             f"'{v
+0000b670: 616c 2e76 616c 7565 7d27 2069 7320 6e6f  al.value}' is no
+0000b680: 7420 6120 7661 6c69 6420 6e61 6d65 206f  t a valid name o
+0000b690: 6620 6120 6c69 7374 206e 6f64 652e 220a  f a list node.".
+0000b6a0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000b6b0: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
+0000b6c0: 6773 2e77 6172 6e28 4473 7054 6f6f 6c73  gs.warn(DspTools
+0000b6d0: 5573 6572 5761 726e 696e 6728 6d73 6729  UserWarning(msg)
+0000b6e0: 290a 0a20 2020 2023 206d 616b 6520 786d  )..    # make xm
+0000b6f0: 6c20 7374 7275 6374 7572 6520 6f66 2074  l structure of t
+0000b700: 6865 2076 616c 6964 2076 616c 7565 730a  he valid values.
+0000b710: 2020 2020 7072 6f70 5f20 3d20 6574 7265      prop_ = etre
+0000b720: 652e 456c 656d 656e 7428 0a20 2020 2020  e.Element(.     
+0000b730: 2020 2022 7b25 737d 6c69 7374 2d70 726f     "{%s}list-pro
+0000b740: 7022 2025 2078 6d6c 5f6e 616d 6573 7061  p" % xml_namespa
+0000b750: 6365 5f6d 6170 5b4e 6f6e 655d 2c0a 2020  ce_map[None],.  
+0000b760: 2020 2020 2020 6c69 7374 3d6c 6973 745f        list=list_
+0000b770: 6e61 6d65 2c0a 2020 2020 2020 2020 6e61  name,.        na
+0000b780: 6d65 3d6e 616d 652c 0a20 2020 2020 2020  me=name,.       
+0000b790: 206e 736d 6170 3d78 6d6c 5f6e 616d 6573   nsmap=xml_names
+0000b7a0: 7061 6365 5f6d 6170 2c0a 2020 2020 290a  pace_map,.    ).
+0000b7b0: 2020 2020 666f 7220 7661 6c20 696e 2076      for val in v
+0000b7c0: 616c 7565 733a 0a20 2020 2020 2020 206b  alues:.        k
+0000b7d0: 7761 7267 7320 3d20 7b22 7065 726d 6973  wargs = {"permis
+0000b7e0: 7369 6f6e 7322 3a20 7661 6c2e 7065 726d  sions": val.perm
+0000b7f0: 6973 7369 6f6e 737d 0a20 2020 2020 2020  issions}.       
+0000b800: 2069 6620 7661 6c2e 636f 6d6d 656e 7420   if val.comment 
+0000b810: 616e 6420 6368 6563 6b5f 6e6f 746e 6128  and check_notna(
+0000b820: 7661 6c2e 636f 6d6d 656e 7429 3a0a 2020  val.comment):.  
+0000b830: 2020 2020 2020 2020 2020 6b77 6172 6773            kwargs
+0000b840: 5b22 636f 6d6d 656e 7422 5d20 3d20 7661  ["comment"] = va
+0000b850: 6c2e 636f 6d6d 656e 740a 2020 2020 2020  l.comment.      
+0000b860: 2020 7661 6c75 655f 203d 2065 7472 6565    value_ = etree
+0000b870: 2e45 6c65 6d65 6e74 280a 2020 2020 2020  .Element(.      
+0000b880: 2020 2020 2020 227b 2573 7d6c 6973 7422        "{%s}list"
+0000b890: 2025 2078 6d6c 5f6e 616d 6573 7061 6365   % xml_namespace
+0000b8a0: 5f6d 6170 5b4e 6f6e 655d 2c0a 2020 2020  _map[None],.    
+0000b8b0: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
+0000b8c0: 2c20 2023 2074 7970 653a 2069 676e 6f72  ,  # type: ignor
+0000b8d0: 655b 6172 672d 7479 7065 5d0a 2020 2020  e[arg-type].    
+0000b8e0: 2020 2020 2020 2020 6e73 6d61 703d 786d          nsmap=xm
+0000b8f0: 6c5f 6e61 6d65 7370 6163 655f 6d61 702c  l_namespace_map,
+0000b900: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0000b910: 2020 2076 616c 7565 5f2e 7465 7874 203d     value_.text =
+0000b920: 2073 7472 2876 616c 2e76 616c 7565 290a   str(val.value).
+0000b930: 2020 2020 2020 2020 7072 6f70 5f2e 6170          prop_.ap
+0000b940: 7065 6e64 2876 616c 7565 5f29 0a0a 2020  pend(value_)..  
+0000b950: 2020 7265 7475 726e 2070 726f 705f 0a0a    return prop_..
+0000b960: 0a64 6566 206d 616b 655f 7265 7370 7472  .def make_resptr
+0000b970: 5f70 726f 7028 0a20 2020 206e 616d 653a  _prop(.    name:
+0000b980: 2073 7472 2c0a 2020 2020 7661 6c75 653a   str,.    value:
+0000b990: 2055 6e69 6f6e 5b50 726f 7065 7274 7945   Union[PropertyE
+0000b9a0: 6c65 6d65 6e74 2c20 7374 722c 2049 7465  lement, str, Ite
+0000b9b0: 7261 626c 655b 556e 696f 6e5b 5072 6f70  rable[Union[Prop
+0000b9c0: 6572 7479 456c 656d 656e 742c 2073 7472  ertyElement, str
+0000b9d0: 5d5d 5d2c 0a20 2020 2063 616c 6c69 6e67  ]]],.    calling
+0000b9e0: 5f72 6573 6f75 7263 653a 2073 7472 203d  _resource: str =
+0000b9f0: 2022 222c 0a29 202d 3e20 6574 7265 652e   "",.) -> etree.
+0000ba00: 5f45 6c65 6d65 6e74 3a0a 2020 2020 2222  _Element:.    ""
+0000ba10: 220a 2020 2020 4d61 6b65 2061 203c 7265  ".    Make a <re
+0000ba20: 7370 7472 2d70 726f 703e 2066 726f 6d20  sptr-prop> from 
+0000ba30: 6f6e 6520 6f72 206d 6f72 6520 4944 7320  one or more IDs 
+0000ba40: 6f66 206f 7468 6572 2072 6573 6f75 7263  of other resourc
+0000ba50: 6573 2e20 5468 6520 4944 2873 2920 6361  es. The ID(s) ca
+0000ba60: 6e20 6265 2070 726f 7669 6465 6420 6173  n be provided as
+0000ba70: 2073 7472 696e 6720 6f72 2061 730a 2020   string or as.  
+0000ba80: 2020 5072 6f70 6572 7479 456c 656d 656e    PropertyElemen
+0000ba90: 7420 7769 7468 2061 2073 7472 696e 6720  t with a string 
+0000baa0: 696e 7369 6465 2e20 4966 2070 726f 7669  inside. If provi
+0000bab0: 6465 6420 6173 2073 7472 696e 672c 2074  ded as string, t
+0000bac0: 6865 2070 6572 6d69 7373 696f 6e73 2064  he permissions d
+0000bad0: 6566 6175 6c74 2074 6f20 2270 726f 702d  efault to "prop-
+0000bae0: 6465 6661 756c 7422 2e0a 0a20 2020 2041  default"...    A
+0000baf0: 7267 733a 0a20 2020 2020 2020 206e 616d  rgs:.        nam
+0000bb00: 653a 2074 6865 206e 616d 6520 6f66 2074  e: the name of t
+0000bb10: 6869 7320 7072 6f70 6572 7479 2061 7320  his property as 
+0000bb20: 6465 6669 6e65 6420 696e 2074 6865 206f  defined in the o
+0000bb30: 6e74 6f0a 2020 2020 2020 2020 7661 6c75  nto.        valu
+0000bb40: 653a 206f 6e65 206f 7220 6d6f 7265 2072  e: one or more r
+0000bb50: 6573 6f75 7263 6520 6964 656e 7469 6669  esource identifi
+0000bb60: 6572 732c 2061 7320 7374 7269 6e67 2f50  ers, as string/P
+0000bb70: 726f 7065 7274 7945 6c65 6d65 6e74 2c20  ropertyElement, 
+0000bb80: 6f72 2061 7320 6974 6572 6162 6c65 206f  or as iterable o
+0000bb90: 6620 7374 7269 6e67 732f 5072 6f70 6572  f strings/Proper
+0000bba0: 7479 456c 656d 656e 7473 0a20 2020 2020  tyElements.     
+0000bbb0: 2020 2063 616c 6c69 6e67 5f72 6573 6f75     calling_resou
+0000bbc0: 7263 653a 2074 6865 206e 616d 6520 6f66  rce: the name of
+0000bbd0: 2074 6865 2070 6172 656e 7420 7265 736f   the parent reso
+0000bbe0: 7572 6365 2028 666f 7220 6265 7474 6572  urce (for better
+0000bbf0: 2065 7272 6f72 206d 6573 7361 6765 7329   error messages)
+0000bc00: 0a0a 2020 2020 5761 726e 733a 0a20 2020  ..    Warns:.   
+0000bc10: 2020 2020 2049 6620 7468 6520 4944 206f       If the ID o
+0000bc20: 6620 6f6e 6520 6f66 2074 6865 2074 6172  f one of the tar
+0000bc30: 6765 7420 7265 736f 7572 6365 7320 6973  get resources is
+0000bc40: 206e 6f74 2061 2076 616c 6964 2073 7472   not a valid str
+0000bc50: 696e 670a 0a20 2020 2052 6574 7572 6e73  ing..    Returns
+0000bc60: 3a0a 2020 2020 2020 2020 616e 2065 7472  :.        an etr
+0000bc70: 6565 2e5f 456c 656d 656e 7420 7468 6174  ee._Element that
+0000bc80: 2063 616e 2062 6520 6170 7065 6e64 6564   can be appended
+0000bc90: 2074 6f20 7468 6520 7061 7265 6e74 2072   to the parent r
+0000bca0: 6573 6f75 7263 6520 7769 7468 2072 6573  esource with res
+0000bcb0: 6f75 7263 652e 6170 7065 6e64 286d 616b  ource.append(mak
+0000bcc0: 655f 2a5f 7072 6f70 282e 2e2e 2929 0a0a  e_*_prop(...))..
+0000bcd0: 2020 2020 4578 616d 706c 6573 3a0a 2020      Examples:.  
+0000bce0: 2020 2020 2020 3e3e 3e20 6578 6365 6c32        >>> excel2
+0000bcf0: 786d 6c2e 6d61 6b65 5f72 6573 7074 725f  xml.make_resptr_
+0000bd00: 7072 6f70 2822 3a74 6573 7470 726f 7065  prop(":testprope
+0000bd10: 7274 7922 2c20 2272 6573 6f75 7263 655f  rty", "resource_
+0000bd20: 3122 290a 2020 2020 2020 2020 2020 2020  1").            
+0000bd30: 2020 2020 3c72 6573 7074 722d 7072 6f70      <resptr-prop
+0000bd40: 206e 616d 653d 223a 7465 7374 7072 6f70   name=":testprop
+0000bd50: 6572 7479 223e 0a20 2020 2020 2020 2020  erty">.         
+0000bd60: 2020 2020 2020 2020 2020 203c 7265 7370             <resp
+0000bd70: 7472 2070 6572 6d69 7373 696f 6e73 3d22  tr permissions="
+0000bd80: 7072 6f70 2d64 6566 6175 6c74 223e 7265  prop-default">re
+0000bd90: 736f 7572 6365 5f31 3c2f 7265 7370 7472  source_1</resptr
+0000bda0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+0000bdb0: 2020 3c2f 7265 7370 7472 2d70 726f 703e    </resptr-prop>
+0000bdc0: 0a20 2020 2020 2020 203e 3e3e 2065 7863  .        >>> exc
+0000bdd0: 656c 3278 6d6c 2e6d 616b 655f 7265 7370  el2xml.make_resp
+0000bde0: 7472 5f70 726f 7028 223a 7465 7374 7072  tr_prop(":testpr
+0000bdf0: 6f70 6572 7479 222c 2065 7863 656c 3278  operty", excel2x
+0000be00: 6d6c 2e50 726f 7065 7274 7945 6c65 6d65  ml.PropertyEleme
+0000be10: 6e74 2822 7265 736f 7572 6365 5f31 222c  nt("resource_1",
+0000be20: 2070 6572 6d69 7373 696f 6e73 3d22 7072   permissions="pr
+0000be30: 6f70 2d72 6573 7472 6963 7465 6422 2c20  op-restricted", 
+0000be40: 636f 6d6d 656e 743d 2265 7861 6d70 6c65  comment="example
+0000be50: 2229 290a 2020 2020 2020 2020 2020 2020  ")).            
+0000be60: 2020 2020 3c72 6573 7074 722d 7072 6f70      <resptr-prop
+0000be70: 206e 616d 653d 223a 7465 7374 7072 6f70   name=":testprop
+0000be80: 6572 7479 223e 0a20 2020 2020 2020 2020  erty">.         
+0000be90: 2020 2020 2020 2020 2020 203c 7265 7370             <resp
+0000bea0: 7472 2070 6572 6d69 7373 696f 6e73 3d22  tr permissions="
+0000beb0: 7072 6f70 2d72 6573 7472 6963 7465 6422  prop-restricted"
+0000bec0: 2063 6f6d 6d65 6e74 3d22 6578 616d 706c   comment="exampl
+0000bed0: 6522 3e72 6573 6f75 7263 655f 313c 2f72  e">resource_1</r
+0000bee0: 6573 7074 723e 0a20 2020 2020 2020 2020  esptr>.         
+0000bef0: 2020 2020 2020 203c 2f72 6573 7074 722d         </resptr-
+0000bf00: 7072 6f70 3e0a 2020 2020 2020 2020 3e3e  prop>.        >>
+0000bf10: 3e20 6578 6365 6c32 786d 6c2e 6d61 6b65  > excel2xml.make
+0000bf20: 5f72 6573 7074 725f 7072 6f70 2822 3a74  _resptr_prop(":t
+0000bf30: 6573 7470 726f 7065 7274 7922 2c20 5b22  estproperty", ["
+0000bf40: 7265 736f 7572 6365 5f31 222c 2022 7265  resource_1", "re
+0000bf50: 736f 7572 6365 5f32 225d 290a 2020 2020  source_2"]).    
+0000bf60: 2020 2020 2020 2020 2020 2020 3c72 6573              <res
+0000bf70: 7074 722d 7072 6f70 206e 616d 653d 223a  ptr-prop name=":
+0000bf80: 7465 7374 7072 6f70 6572 7479 223e 0a20  testproperty">. 
+0000bf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfa0: 2020 203c 7265 7370 7472 2070 6572 6d69     <resptr permi
+0000bfb0: 7373 696f 6e73 3d22 7072 6f70 2d64 6566  ssions="prop-def
+0000bfc0: 6175 6c74 223e 7265 736f 7572 6365 5f31  ault">resource_1
+0000bfd0: 3c2f 7265 7370 7472 3e0a 2020 2020 2020  </resptr>.      
+0000bfe0: 2020 2020 2020 2020 2020 2020 2020 3c72                <r
+0000bff0: 6573 7074 7220 7065 726d 6973 7369 6f6e  esptr permission
+0000c000: 733d 2270 726f 702d 6465 6661 756c 7422  s="prop-default"
+0000c010: 3e72 6573 6f75 7263 655f 323c 2f72 6573  >resource_2</res
+0000c020: 7074 723e 0a20 2020 2020 2020 2020 2020  ptr>.           
+0000c030: 2020 2020 203c 2f72 6573 7074 722d 7072       </resptr-pr
+0000c040: 6f70 3e0a 0a20 2020 2053 6565 2068 7474  op>..    See htt
+0000c050: 7073 3a2f 2f64 6f63 732e 6461 7363 682e  ps://docs.dasch.
+0000c060: 7377 6973 732f 6c61 7465 7374 2f44 5350  swiss/latest/DSP
+0000c070: 2d54 4f4f 4c53 2f66 696c 652d 666f 726d  -TOOLS/file-form
+0000c080: 6174 732f 786d 6c2d 6461 7461 2d66 696c  ats/xml-data-fil
+0000c090: 652f 2372 6573 7074 722d 7072 6f70 0a20  e/#resptr-prop. 
+0000c0a0: 2020 2022 2222 0a0a 2020 2020 2320 6368     """..    # ch
+0000c0b0: 6563 6b20 7468 6520 696e 7075 743a 2070  eck the input: p
+0000c0c0: 7265 7061 7265 2061 206c 6973 7420 7769  repare a list wi
+0000c0d0: 7468 2076 616c 6964 2076 616c 7565 730a  th valid values.
+0000c0e0: 2020 2020 7661 6c75 6573 203d 2070 7265      values = pre
+0000c0f0: 7061 7265 5f76 616c 7565 2876 616c 7565  pare_value(value
+0000c100: 290a 0a20 2020 2023 2063 6865 636b 2076  )..    # check v
+0000c110: 616c 7565 2074 7970 650a 2020 2020 666f  alue type.    fo
+0000c120: 7220 7661 6c20 696e 2076 616c 7565 733a  r val in values:
+0000c130: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0000c140: 6973 696e 7374 616e 6365 2876 616c 2e76  isinstance(val.v
+0000c150: 616c 7565 2c20 7374 7229 206f 7220 6e6f  alue, str) or no
+0000c160: 7420 6368 6563 6b5f 6e6f 746e 6128 7661  t check_notna(va
+0000c170: 6c2e 7661 6c75 6529 3a0a 2020 2020 2020  l.value):.      
+0000c180: 2020 2020 2020 6d73 6720 3d20 280a 2020        msg = (.  
+0000c190: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+0000c1a0: 5661 6c69 6461 7469 6f6e 2045 7272 6f72  Validation Error
+0000c1b0: 2069 6e20 7265 736f 7572 6365 2027 7b63   in resource '{c
+0000c1c0: 616c 6c69 6e67 5f72 6573 6f75 7263 657d  alling_resource}
+0000c1d0: 272c 2070 726f 7065 7274 7920 277b 6e61  ', property '{na
+0000c1e0: 6d65 7d27 3a20 220a 2020 2020 2020 2020  me}': ".        
+0000c1f0: 2020 2020 2020 2020 6622 5468 6520 666f          f"The fo
+0000c200: 6c6c 6f77 696e 6720 646f 6573 6e27 7420  llowing doesn't 
+0000c210: 7365 656d 2074 6f20 6265 2061 2076 616c  seem to be a val
+0000c220: 6964 2049 4420 6f66 2061 2074 6172 6765  id ID of a targe
+0000c230: 7420 7265 736f 7572 6365 3a20 277b 7661  t resource: '{va
+0000c240: 6c2e 7661 6c75 657d 2722 0a20 2020 2020  l.value}'".     
+0000c250: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000c260: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
+0000c270: 726e 2844 7370 546f 6f6c 7355 7365 7257  rn(DspToolsUserW
+0000c280: 6172 6e69 6e67 286d 7367 2929 0a0a 2020  arning(msg))..  
+0000c290: 2020 2320 6d61 6b65 2078 6d6c 2073 7472    # make xml str
+0000c2a0: 7563 7475 7265 206f 6620 7468 6520 7661  ucture of the va
+0000c2b0: 6c69 6420 7661 6c75 6573 0a20 2020 2070  lid values.    p
+0000c2c0: 726f 705f 203d 2065 7472 6565 2e45 6c65  rop_ = etree.Ele
+0000c2d0: 6d65 6e74 280a 2020 2020 2020 2020 227b  ment(.        "{
+0000c2e0: 2573 7d72 6573 7074 722d 7072 6f70 2220  %s}resptr-prop" 
+0000c2f0: 2520 786d 6c5f 6e61 6d65 7370 6163 655f  % xml_namespace_
+0000c300: 6d61 705b 4e6f 6e65 5d2c 0a20 2020 2020  map[None],.     
+0000c310: 2020 206e 616d 653d 6e61 6d65 2c0a 2020     name=name,.  
+0000c320: 2020 2020 2020 6e73 6d61 703d 786d 6c5f        nsmap=xml_
+0000c330: 6e61 6d65 7370 6163 655f 6d61 702c 0a20  namespace_map,. 
+0000c340: 2020 2029 0a20 2020 2066 6f72 2076 616c     ).    for val
+0000c350: 2069 6e20 7661 6c75 6573 3a0a 2020 2020   in values:.    
+0000c360: 2020 2020 6b77 6172 6773 203d 207b 2270      kwargs = {"p
+0000c370: 6572 6d69 7373 696f 6e73 223a 2076 616c  ermissions": val
+0000c380: 2e70 6572 6d69 7373 696f 6e73 7d0a 2020  .permissions}.  
+0000c390: 2020 2020 2020 6966 2076 616c 2e63 6f6d        if val.com
+0000c3a0: 6d65 6e74 2061 6e64 2063 6865 636b 5f6e  ment and check_n
+0000c3b0: 6f74 6e61 2876 616c 2e63 6f6d 6d65 6e74  otna(val.comment
+0000c3c0: 293a 0a20 2020 2020 2020 2020 2020 206b  ):.            k
+0000c3d0: 7761 7267 735b 2263 6f6d 6d65 6e74 225d  wargs["comment"]
+0000c3e0: 203d 2076 616c 2e63 6f6d 6d65 6e74 0a20   = val.comment. 
+0000c3f0: 2020 2020 2020 2076 616c 7565 5f20 3d20         value_ = 
+0000c400: 6574 7265 652e 456c 656d 656e 7428 0a20  etree.Element(. 
+0000c410: 2020 2020 2020 2020 2020 2022 7b25 737d             "{%s}
+0000c420: 7265 7370 7472 2220 2520 786d 6c5f 6e61  resptr" % xml_na
+0000c430: 6d65 7370 6163 655f 6d61 705b 4e6f 6e65  mespace_map[None
+0000c440: 5d2c 0a20 2020 2020 2020 2020 2020 202a  ],.            *
+0000c450: 2a6b 7761 7267 732c 2020 2320 7479 7065  *kwargs,  # type
+0000c460: 3a20 6967 6e6f 7265 5b61 7267 2d74 7970  : ignore[arg-typ
+0000c470: 655d 0a20 2020 2020 2020 2020 2020 206e  e].            n
+0000c480: 736d 6170 3d78 6d6c 5f6e 616d 6573 7061  smap=xml_namespa
+0000c490: 6365 5f6d 6170 2c0a 2020 2020 2020 2020  ce_map,.        
+0000c4a0: 290a 2020 2020 2020 2020 7661 6c75 655f  ).        value_
+0000c4b0: 2e74 6578 7420 3d20 7374 7228 7661 6c2e  .text = str(val.
+0000c4c0: 7661 6c75 6529 0a20 2020 2020 2020 2070  value).        p
+0000c4d0: 726f 705f 2e61 7070 656e 6428 7661 6c75  rop_.append(valu
+0000c4e0: 655f 290a 0a20 2020 2072 6574 7572 6e20  e_)..    return 
+0000c4f0: 7072 6f70 5f0a 0a0a 6465 6620 6d61 6b65  prop_...def make
+0000c500: 5f74 6578 745f 7072 6f70 280a 2020 2020  _text_prop(.    
+0000c510: 6e61 6d65 3a20 7374 722c 0a20 2020 2076  name: str,.    v
+0000c520: 616c 7565 3a20 556e 696f 6e5b 5072 6f70  alue: Union[Prop
+0000c530: 6572 7479 456c 656d 656e 742c 2073 7472  ertyElement, str
+0000c540: 2c20 4974 6572 6162 6c65 5b55 6e69 6f6e  , Iterable[Union
+0000c550: 5b50 726f 7065 7274 7945 6c65 6d65 6e74  [PropertyElement
+0000c560: 2c20 7374 725d 5d5d 2c0a 2020 2020 6361  , str]]],.    ca
+0000c570: 6c6c 696e 675f 7265 736f 7572 6365 3a20  lling_resource: 
+0000c580: 7374 7220 3d20 2222 2c0a 2920 2d3e 2065  str = "",.) -> e
+0000c590: 7472 6565 2e5f 456c 656d 656e 743a 0a20  tree._Element:. 
+0000c5a0: 2020 2022 2222 0a20 2020 204d 616b 6520     """.    Make 
+0000c5b0: 6120 3c74 6578 742d 7072 6f70 3e20 6672  a <text-prop> fr
+0000c5c0: 6f6d 206f 6e65 206f 7220 6d6f 7265 2073  om one or more s
+0000c5d0: 7472 696e 6773 2e20 5468 6520 7374 7269  trings. The stri
+0000c5e0: 6e67 2873 2920 6361 6e20 6265 2070 726f  ng(s) can be pro
+0000c5f0: 7669 6465 6420 6173 2073 7472 696e 6720  vided as string 
+0000c600: 6f72 2061 7320 5072 6f70 6572 7479 456c  or as PropertyEl
+0000c610: 656d 656e 7420 7769 7468 2061 0a20 2020  ement with a.   
+0000c620: 2073 7472 696e 6720 696e 7369 6465 2e20   string inside. 
+0000c630: 4966 2070 726f 7669 6465 6420 6173 2073  If provided as s
+0000c640: 7472 696e 672c 2074 6865 2065 6e63 6f64  tring, the encod
+0000c650: 696e 6720 6465 6661 756c 7473 2074 6f20  ing defaults to 
+0000c660: 7574 6638 2c20 616e 6420 7468 6520 7065  utf8, and the pe
+0000c670: 726d 6973 7369 6f6e 7320 746f 2022 7072  rmissions to "pr
+0000c680: 6f70 2d64 6566 6175 6c74 222e 0a0a 2020  op-default"...  
+0000c690: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+0000c6a0: 6e61 6d65 3a20 7468 6520 6e61 6d65 206f  name: the name o
+0000c6b0: 6620 7468 6973 2070 726f 7065 7274 7920  f this property 
+0000c6c0: 6173 2064 6566 696e 6564 2069 6e20 7468  as defined in th
+0000c6d0: 6520 6f6e 746f 0a20 2020 2020 2020 2076  e onto.        v
+0000c6e0: 616c 7565 3a20 6f6e 6520 6f72 206d 6f72  alue: one or mor
+0000c6f0: 6520 7374 7269 6e67 732c 2061 7320 7374  e strings, as st
+0000c700: 7269 6e67 2f50 726f 7065 7274 7945 6c65  ring/PropertyEle
+0000c710: 6d65 6e74 2c20 6f72 2061 7320 6974 6572  ment, or as iter
+0000c720: 6162 6c65 206f 6620 7374 7269 6e67 732f  able of strings/
+0000c730: 5072 6f70 6572 7479 456c 656d 656e 7473  PropertyElements
+0000c740: 0a20 2020 2020 2020 2063 616c 6c69 6e67  .        calling
+0000c750: 5f72 6573 6f75 7263 653a 2074 6865 206e  _resource: the n
+0000c760: 616d 6520 6f66 2074 6865 2070 6172 656e  ame of the paren
+0000c770: 7420 7265 736f 7572 6365 2028 666f 7220  t resource (for 
+0000c780: 6265 7474 6572 2065 7272 6f72 206d 6573  better error mes
+0000c790: 7361 6765 7329 0a0a 2020 2020 5261 6973  sages)..    Rais
+0000c7a0: 6573 3a0a 2020 2020 2020 2020 4261 7365  es:.        Base
+0000c7b0: 4572 726f 723a 2069 6620 7468 6520 584d  Error: if the XM
+0000c7c0: 4c20 7461 6773 2069 6e20 6120 7269 6368  L tags in a rich
+0000c7d0: 7465 7874 2070 726f 7065 7274 7920 2865  text property (e
+0000c7e0: 6e63 6f64 696e 673d 786d 6c29 2061 7265  ncoding=xml) are
+0000c7f0: 206e 6f74 2077 656c 6c2d 666f 726d 6564   not well-formed
+0000c800: 0a20 2020 2020 2020 2057 6172 6e69 6e67  .        Warning
+0000c810: 3a20 6966 206f 6e65 206f 6620 7468 6520  : if one of the 
+0000c820: 7661 6c75 6573 2064 6f65 736e 2774 206c  values doesn't l
+0000c830: 6f6f 6b20 6c69 6b65 2061 2072 6561 736f  ook like a reaso
+0000c840: 6e61 626c 6520 7374 7269 6e67 0a20 2020  nable string.   
+0000c850: 2020 2020 2020 2020 2028 652e 672e 2022           (e.g. "
+0000c860: 3c4e 413e 2220 6973 2061 2076 616c 6964  <NA>" is a valid
+0000c870: 2073 7472 696e 672c 2062 7574 2070 726f   string, but pro
+0000c880: 6261 626c 7920 6e6f 7420 696e 7465 6e64  bably not intend
+0000c890: 6564 290a 0a20 2020 2052 6574 7572 6e73  ed)..    Returns
+0000c8a0: 3a0a 2020 2020 2020 2020 616e 2065 7472  :.        an etr
+0000c8b0: 6565 2e5f 456c 656d 656e 7420 7468 6174  ee._Element that
+0000c8c0: 2063 616e 2062 6520 6170 7065 6e64 6564   can be appended
+0000c8d0: 2074 6f20 7468 6520 7061 7265 6e74 2072   to the parent r
+0000c8e0: 6573 6f75 7263 6520 7769 7468 2072 6573  esource with res
+0000c8f0: 6f75 7263 652e 6170 7065 6e64 286d 616b  ource.append(mak
+0000c900: 655f 2a5f 7072 6f70 282e 2e2e 2929 0a0a  e_*_prop(...))..
+0000c910: 2020 2020 4578 616d 706c 6573 3a0a 2020      Examples:.  
+0000c920: 2020 2020 2020 3e3e 3e20 6578 6365 6c32        >>> excel2
+0000c930: 786d 6c2e 6d61 6b65 5f74 6578 745f 7072  xml.make_text_pr
+0000c940: 6f70 2822 3a74 6573 7470 726f 7065 7274  op(":testpropert
+0000c950: 7922 2c20 2266 6972 7374 2074 6578 7422  y", "first text"
+0000c960: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000c970: 2020 3c74 6578 742d 7072 6f70 206e 616d    <text-prop nam
+0000c980: 653d 223a 7465 7374 7072 6f70 6572 7479  e=":testproperty
+0000c990: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+0000c9a0: 2020 2020 2020 203c 7465 7874 2065 6e63         <text enc
+0000c9b0: 6f64 696e 673d 2275 7466 3822 2070 6572  oding="utf8" per
+0000c9c0: 6d69 7373 696f 6e73 3d22 7072 6f70 2d64  missions="prop-d
+0000c9d0: 6566 6175 6c74 223e 6669 7273 7420 7465  efault">first te
+0000c9e0: 7874 3c2f 7465 7874 3e0a 2020 2020 2020  xt</text>.      
+0000c9f0: 2020 2020 2020 2020 2020 3c2f 7465 7874            </text
+0000ca00: 2d70 726f 703e 0a20 2020 2020 2020 203e  -prop>.        >
+0000ca10: 3e3e 2065 7863 656c 3278 6d6c 2e6d 616b  >> excel2xml.mak
+0000ca20: 655f 7465 7874 5f70 726f 7028 223a 7465  e_text_prop(":te
+0000ca30: 7374 7072 6f70 6572 7479 222c 2065 7863  stproperty", exc
+0000ca40: 656c 3278 6d6c 2e50 726f 7065 7274 7945  el2xml.PropertyE
+0000ca50: 6c65 6d65 6e74 2822 6669 7273 7420 7465  lement("first te
+0000ca60: 7874 222c 2070 6572 6d69 7373 696f 6e73  xt", permissions
+0000ca70: 3d22 7072 6f70 2d72 6573 7472 6963 7465  ="prop-restricte
+0000ca80: 6422 2c20 656e 636f 6469 6e67 3d22 786d  d", encoding="xm
+0000ca90: 6c22 2929 0a20 2020 2020 2020 2020 2020  l")).           
+0000caa0: 2020 2020 203c 7465 7874 2d70 726f 7020       <text-prop 
+0000cab0: 6e61 6d65 3d22 3a74 6573 7470 726f 7065  name=":testprope
+0000cac0: 7274 7922 3e0a 2020 2020 2020 2020 2020  rty">.          
+0000cad0: 2020 2020 2020 2020 2020 3c74 6578 7420            <text 
+0000cae0: 656e 636f 6469 6e67 3d22 786d 6c22 2070  encoding="xml" p
+0000caf0: 6572 6d69 7373 696f 6e73 3d22 7072 6f70  ermissions="prop
+0000cb00: 2d72 6573 7472 6963 7465 6422 3e66 6972  -restricted">fir
+0000cb10: 7374 2074 6578 743c 2f74 6578 743e 0a20  st text</text>. 
+0000cb20: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+0000cb30: 2f74 6578 742d 7072 6f70 3e0a 2020 2020  /text-prop>.    
+0000cb40: 2020 2020 3e3e 3e20 6578 6365 6c32 786d      >>> excel2xm
+0000cb50: 6c2e 6d61 6b65 5f74 6578 745f 7072 6f70  l.make_text_prop
+0000cb60: 2822 3a74 6573 7470 726f 7065 7274 7922  (":testproperty"
+0000cb70: 2c20 5b22 6669 7273 7420 7465 7874 222c  , ["first text",
+0000cb80: 2022 7365 636f 6e64 2074 6578 7422 5d29   "second text"])
+0000cb90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cba0: 203c 7465 7874 2d70 726f 7020 6e61 6d65   <text-prop name
+0000cbb0: 3d22 3a74 6573 7470 726f 7065 7274 7922  =":testproperty"
+0000cbc0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+0000cbd0: 2020 2020 2020 3c74 6578 7420 656e 636f        <text enco
+0000cbe0: 6469 6e67 3d22 7574 6638 2220 7065 726d  ding="utf8" perm
+0000cbf0: 6973 7369 6f6e 733d 2270 726f 702d 6465  issions="prop-de
+0000cc00: 6661 756c 7422 3e66 6972 7374 2074 6578  fault">first tex
+0000cc10: 743c 2f74 6578 743e 0a20 2020 2020 2020  t</text>.       
+0000cc20: 2020 2020 2020 2020 2020 2020 203c 7465               <te
+0000cc30: 7874 2065 6e63 6f64 696e 673d 2275 7466  xt encoding="utf
+0000cc40: 3822 2070 6572 6d69 7373 696f 6e73 3d22  8" permissions="
+0000cc50: 7072 6f70 2d64 6566 6175 6c74 223e 7365  prop-default">se
+0000cc60: 636f 6e64 2074 6578 743c 2f74 6578 743e  cond text</text>
+0000cc70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cc80: 203c 2f74 6578 742d 7072 6f70 3e0a 0a20   </text-prop>.. 
+0000cc90: 2020 2053 6565 2068 7474 7073 3a2f 2f64     See https://d
+0000cca0: 6f63 732e 6461 7363 682e 7377 6973 732f  ocs.dasch.swiss/
+0000ccb0: 6c61 7465 7374 2f44 5350 2d54 4f4f 4c53  latest/DSP-TOOLS
+0000ccc0: 2f66 696c 652d 666f 726d 6174 732f 786d  /file-formats/xm
+0000ccd0: 6c2d 6461 7461 2d66 696c 652f 2374 6578  l-data-file/#tex
+0000cce0: 742d 7072 6f70 0a20 2020 2022 2222 0a0a  t-prop.    """..
+0000ccf0: 2020 2020 2320 6368 6563 6b20 7468 6520      # check the 
+0000cd00: 696e 7075 743a 2070 7265 7061 7265 2061  input: prepare a
+0000cd10: 206c 6973 7420 7769 7468 2076 616c 6964   list with valid
+0000cd20: 2076 616c 7565 730a 2020 2020 7661 6c75   values.    valu
+0000cd30: 6573 203d 2070 7265 7061 7265 5f76 616c  es = prepare_val
+0000cd40: 7565 2876 616c 7565 290a 0a20 2020 2023  ue(value)..    #
+0000cd50: 2063 6865 636b 2076 616c 7565 2074 7970   check value typ
+0000cd60: 650a 2020 2020 666f 7220 7661 6c20 696e  e.    for val in
+0000cd70: 2076 616c 7565 733a 0a20 2020 2020 2020   values:.       
+0000cd80: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
+0000cd90: 6365 2876 616c 2e76 616c 7565 2c20 7374  ce(val.value, st
+0000cda0: 7229 206f 7220 6e6f 7420 6368 6563 6b5f  r) or not check_
+0000cdb0: 6e6f 746e 6128 7661 6c2e 7661 6c75 6529  notna(val.value)
+0000cdc0: 3a0a 2020 2020 2020 2020 2020 2020 6d73  :.            ms
+0000cdd0: 6720 3d20 280a 2020 2020 2020 2020 2020  g = (.          
+0000cde0: 2020 2020 2020 6622 4661 696c 6564 2076        f"Failed v
+0000cdf0: 616c 6964 6174 696f 6e20 696e 2072 6573  alidation in res
+0000ce00: 6f75 7263 6520 277b 6361 6c6c 696e 675f  ource '{calling_
+0000ce10: 7265 736f 7572 6365 7d27 2c20 7072 6f70  resource}', prop
+0000ce20: 6572 7479 2027 7b6e 616d 657d 273a 2022  erty '{name}': "
+0000ce30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ce40: 2066 2227 7b76 616c 2e76 616c 7565 7d27   f"'{val.value}'
+0000ce50: 2069 7320 7072 6f62 6162 6c79 206e 6f74   is probably not
+0000ce60: 2061 2075 7361 626c 6520 7374 7269 6e67   a usable string
+0000ce70: 2e22 0a20 2020 2020 2020 2020 2020 2029  .".            )
+0000ce80: 0a20 2020 2020 2020 2020 2020 2077 6172  .            war
+0000ce90: 6e69 6e67 732e 7761 726e 2844 7370 546f  nings.warn(DspTo
+0000cea0: 6f6c 7355 7365 7257 6172 6e69 6e67 286d  olsUserWarning(m
+0000ceb0: 7367 2929 0a0a 2020 2020 2320 6d61 6b65  sg))..    # make
+0000cec0: 2078 6d6c 2073 7472 7563 7475 7265 206f   xml structure o
+0000ced0: 6620 7468 6520 7661 6c69 6420 7661 6c75  f the valid valu
+0000cee0: 6573 0a20 2020 2070 726f 705f 203d 2065  es.    prop_ = e
+0000cef0: 7472 6565 2e45 6c65 6d65 6e74 280a 2020  tree.Element(.  
+0000cf00: 2020 2020 2020 227b 2573 7d74 6578 742d        "{%s}text-
+0000cf10: 7072 6f70 2220 2520 786d 6c5f 6e61 6d65  prop" % xml_name
+0000cf20: 7370 6163 655f 6d61 705b 4e6f 6e65 5d2c  space_map[None],
+0000cf30: 0a20 2020 2020 2020 206e 616d 653d 6e61  .        name=na
+0000cf40: 6d65 2c0a 2020 2020 2020 2020 6e73 6d61  me,.        nsma
+0000cf50: 703d 786d 6c5f 6e61 6d65 7370 6163 655f  p=xml_namespace_
+0000cf60: 6d61 702c 0a20 2020 2029 0a20 2020 2066  map,.    ).    f
+0000cf70: 6f72 2076 616c 2069 6e20 7661 6c75 6573  or val in values
+0000cf80: 3a0a 2020 2020 2020 2020 6b77 6172 6773  :.        kwargs
+0000cf90: 203d 207b 2270 6572 6d69 7373 696f 6e73   = {"permissions
+0000cfa0: 223a 2076 616c 2e70 6572 6d69 7373 696f  ": val.permissio
+0000cfb0: 6e73 7d0a 2020 2020 2020 2020 6966 2063  ns}.        if c
+0000cfc0: 6865 636b 5f6e 6f74 6e61 2876 616c 2e63  heck_notna(val.c
+0000cfd0: 6f6d 6d65 6e74 293a 0a20 2020 2020 2020  omment):.       
+0000cfe0: 2020 2020 206b 7761 7267 735b 2263 6f6d       kwargs["com
+0000cff0: 6d65 6e74 225d 203d 2076 616c 2e63 6f6d  ment"] = val.com
+0000d000: 6d65 6e74 0a20 2020 2020 2020 206b 7761  ment.        kwa
+0000d010: 7267 735b 2265 6e63 6f64 696e 6722 5d20  rgs["encoding"] 
+0000d020: 3d20 7661 6c2e 656e 636f 6469 6e67 2069  = val.encoding i
+0000d030: 6620 6368 6563 6b5f 6e6f 746e 6128 7661  f check_notna(va
+0000d040: 6c2e 656e 636f 6469 6e67 2920 656c 7365  l.encoding) else
+0000d050: 2022 7574 6638 220a 2020 2020 2020 2020   "utf8".        
+0000d060: 7661 6c75 655f 203d 2065 7472 6565 2e45  value_ = etree.E
+0000d070: 6c65 6d65 6e74 280a 2020 2020 2020 2020  lement(.        
+0000d080: 2020 2020 227b 2573 7d74 6578 7422 2025      "{%s}text" %
+0000d090: 2078 6d6c 5f6e 616d 6573 7061 6365 5f6d   xml_namespace_m
+0000d0a0: 6170 5b4e 6f6e 655d 2c0a 2020 2020 2020  ap[None],.      
+0000d0b0: 2020 2020 2020 2a2a 6b77 6172 6773 2c20        **kwargs, 
+0000d0c0: 2023 2074 7970 653a 2069 676e 6f72 655b   # type: ignore[
+0000d0d0: 6172 672d 7479 7065 5d0a 2020 2020 2020  arg-type].      
+0000d0e0: 2020 2020 2020 6e73 6d61 703d 786d 6c5f        nsmap=xml_
+0000d0f0: 6e61 6d65 7370 6163 655f 6d61 702c 0a20  namespace_map,. 
+0000d100: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000d110: 2069 6620 6b77 6172 6773 5b22 656e 636f   if kwargs["enco
+0000d120: 6469 6e67 225d 203d 3d20 2275 7466 3822  ding"] == "utf8"
+0000d130: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+0000d140: 7772 6974 6520 7468 6520 7465 7874 2069  write the text i
+0000d150: 6e74 6f20 7468 6520 7461 672c 2077 6974  nto the tag, wit
+0000d160: 686f 7574 2076 616c 6964 6174 696f 6e0a  hout validation.
+0000d170: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+0000d180: 655f 2e74 6578 7420 3d20 7374 7228 7661  e_.text = str(va
+0000d190: 6c2e 7661 6c75 6529 0a20 2020 2020 2020  l.value).       
+0000d1a0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000d1b0: 2020 2065 7363 6170 6564 5f74 6578 7420     escaped_text 
+0000d1c0: 3d20 5f65 7363 6170 655f 7265 7365 7276  = _escape_reserv
+0000d1d0: 6564 5f63 6861 7273 2873 7472 2876 616c  ed_chars(str(val
+0000d1e0: 2e76 616c 7565 2929 0a20 2020 2020 2020  .value)).       
+0000d1f0: 2020 2020 2023 2065 6e66 6f72 6365 2074       # enforce t
+0000d200: 6861 7420 7468 6520 7465 7874 2069 7320  hat the text is 
+0000d210: 7765 6c6c 2d66 6f72 6d65 6420 584d 4c3a  well-formed XML:
+0000d220: 2073 6572 6961 6c69 7a65 2074 6167 202e   serialize tag .
+0000d230: 2e2e 0a20 2020 2020 2020 2020 2020 2073  ...            s
+0000d240: 6572 6961 6c69 7a65 6420 3d20 6574 7265  erialized = etre
+0000d250: 652e 746f 7374 7269 6e67 2876 616c 7565  e.tostring(value
+0000d260: 5f2c 2065 6e63 6f64 696e 673d 2275 6e69  _, encoding="uni
+0000d270: 636f 6465 2229 0a20 2020 2020 2020 2020  code").         
+0000d280: 2020 2023 202e 2e2e 2069 6e73 6572 7420     # ... insert 
+0000d290: 7465 7874 2061 7420 7468 6520 7665 7279  text at the very
+0000d2a0: 2065 6e64 206f 6620 7468 6520 7374 7269   end of the stri
+0000d2b0: 6e67 2c20 616e 6420 6164 6420 656e 6469  ng, and add endi
+0000d2c0: 6e67 2074 6167 2074 6f20 7468 6520 7072  ng tag to the pr
+0000d2d0: 6576 696f 7573 6c79 2073 696e 676c 6520  eviously single 
+0000d2e0: 3c74 6578 742f 3e20 7461 6720 2e2e 2e0a  <text/> tag ....
+0000d2f0: 2020 2020 2020 2020 2020 2020 7365 7269              seri
+0000d300: 616c 697a 6564 203d 2072 6567 6578 2e73  alized = regex.s
+0000d310: 7562 2872 222f 3e24 222c 2066 223e 7b65  ub(r"/>$", f">{e
+0000d320: 7363 6170 6564 5f74 6578 747d 3c2f 7465  scaped_text}</te
+0000d330: 7874 3e22 2c20 7365 7269 616c 697a 6564  xt>", serialized
+0000d340: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
+0000d350: 2e2e 2e20 7472 7920 746f 2070 6172 7365  ... try to parse
+0000d360: 2069 7420 6167 6169 6e0a 2020 2020 2020   it again.      
+0000d370: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+0000d380: 2020 2020 2020 2020 2020 2076 616c 7565             value
+0000d390: 5f20 3d20 6574 7265 652e 6672 6f6d 7374  _ = etree.fromst
+0000d3a0: 7269 6e67 2873 6572 6961 6c69 7a65 6429  ring(serialized)
+0000d3b0: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+0000d3c0: 6570 7420 6574 7265 652e 584d 4c53 796e  ept etree.XMLSyn
+0000d3d0: 7461 7845 7272 6f72 2061 7320 6572 723a  taxError as err:
+0000d3e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d3f0: 206d 7367 203d 2028 0a20 2020 2020 2020   msg = (.       
+0000d400: 2020 2020 2020 2020 2020 2020 2022 5468               "Th
+0000d410: 6520 584d 4c20 7461 6773 2063 6f6e 7461  e XML tags conta
+0000d420: 696e 6564 2069 6e20 6120 7269 6368 7465  ined in a richte
+0000d430: 7874 2070 726f 7065 7274 7920 2865 6e63  xt property (enc
+0000d440: 6f64 696e 673d 786d 6c29 206d 7573 7420  oding=xml) must 
+0000d450: 6265 2077 656c 6c2d 666f 726d 6564 2e20  be well-formed. 
+0000d460: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000d470: 2020 2020 2020 2254 6865 2073 7065 6369        "The speci
+0000d480: 616c 2063 6861 7261 6374 6572 7320 3c2c  al characters <,
+0000d490: 203e 2061 6e64 2026 2061 7265 206f 6e6c   > and & are onl
+0000d4a0: 7920 616c 6c6f 7765 6420 746f 2063 6f6e  y allowed to con
+0000d4b0: 7374 7275 6374 2061 2074 6167 2e20 220a  struct a tag. ".
+0000d4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d4d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000d4e0: 2020 6966 2063 616c 6c69 6e67 5f72 6573    if calling_res
+0000d4f0: 6f75 7263 653a 0a20 2020 2020 2020 2020  ource:.         
+0000d500: 2020 2020 2020 2020 2020 206d 7367 202b             msg +
+0000d510: 3d20 6622 5468 6520 6572 726f 7220 6f63  = f"The error oc
+0000d520: 6375 7272 6564 2069 6e20 7265 736f 7572  curred in resour
+0000d530: 6365 207b 6361 6c6c 696e 675f 7265 736f  ce {calling_reso
+0000d540: 7572 6365 7d2c 2070 726f 7065 7274 7920  urce}, property 
+0000d550: 7b6e 616d 657d 220a 2020 2020 2020 2020  {name}".        
+0000d560: 2020 2020 2020 2020 6d73 6720 2b3d 2066          msg += f
+0000d570: 225c 6e4f 7269 6769 6e61 6c20 6572 726f  "\nOriginal erro
+0000d580: 7220 6d65 7373 6167 653a 207b 6572 722e  r message: {err.
+0000d590: 6d73 677d 220a 2020 2020 2020 2020 2020  msg}".          
+0000d5a0: 2020 2020 2020 6d73 6720 2b3d 2066 225c        msg += f"\
+0000d5b0: 6e45 7665 6e74 7561 6c20 6c69 6e65 2f63  nEventual line/c
+0000d5c0: 6f6c 756d 6e20 6e75 6d62 6572 7320 6172  olumn numbers ar
+0000d5d0: 6520 7265 6c61 7469 7665 2074 6f20 7468  e relative to th
+0000d5e0: 6973 2073 6572 6961 6c69 7a65 6420 7465  is serialized te
+0000d5f0: 7874 3a20 7b73 6572 6961 6c69 7a65 647d  xt: {serialized}
+0000d600: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000d610: 2020 7261 6973 6520 4261 7365 4572 726f    raise BaseErro
+0000d620: 7228 6d73 6729 2066 726f 6d20 4e6f 6e65  r(msg) from None
+0000d630: 0a20 2020 2020 2020 2070 726f 705f 2e61  .        prop_.a
+0000d640: 7070 656e 6428 7661 6c75 655f 290a 0a20  ppend(value_).. 
+0000d650: 2020 2072 6574 7572 6e20 7072 6f70 5f0a     return prop_.
+0000d660: 0a0a 6465 6620 5f65 7363 6170 655f 7265  ..def _escape_re
+0000d670: 7365 7276 6564 5f63 6861 7273 2874 6578  served_chars(tex
+0000d680: 743a 2073 7472 2920 2d3e 2073 7472 3a0a  t: str) -> str:.
+0000d690: 2020 2020 2222 220a 2020 2020 4672 6f6d      """.    From
+0000d6a0: 2072 6963 6874 6578 7420 7374 7269 6e67   richtext string
+0000d6b0: 7320 2865 6e63 6f64 696e 673d 2278 6d6c  s (encoding="xml
+0000d6c0: 2229 2c20 6573 6361 7065 2074 6865 2072  "), escape the r
+0000d6d0: 6573 6572 7665 6420 6368 6172 6163 7465  eserved characte
+0000d6e0: 7273 203c 2c20 3e20 616e 6420 262c 0a20  rs <, > and &,. 
+0000d6f0: 2020 2062 7574 206f 6e6c 7920 6966 2074     but only if t
+0000d700: 6865 7920 6172 6520 6e6f 7420 7061 7274  hey are not part
+0000d710: 206f 6620 6120 7374 616e 6461 7264 2073   of a standard s
+0000d720: 7461 6e64 6f66 6620 7461 6720 6f72 2065  tandoff tag or e
+0000d730: 7363 6170 6520 7365 7175 656e 6365 2e0a  scape sequence..
+0000d740: 2020 2020 5468 6520 7374 616e 6461 7264      The standard
+0000d750: 2073 7461 6e64 6f66 6620 7461 6773 2061   standoff tags a
+0000d760: 6c6c 6f77 6564 2062 7920 4453 502d 4150  llowed by DSP-AP
+0000d770: 4920 6172 6520 646f 6375 6d65 6e74 6564  I are documented
+0000d780: 2068 6572 653a 0a20 2020 2068 7474 7073   here:.    https
+0000d790: 3a2f 2f64 6f63 732e 6461 7363 682e 7377  ://docs.dasch.sw
+0000d7a0: 6973 732f 3230 3233 2e31 322e 3031 2f44  iss/2023.12.01/D
+0000d7b0: 5350 2d41 5049 2f30 332d 656e 6470 6f69  SP-API/03-endpoi
+0000d7c0: 6e74 732f 6170 692d 7632 2f74 6578 742f  nts/api-v2/text/
+0000d7d0: 7374 616e 6461 7264 2d73 7461 6e64 6f66  standard-standof
+0000d7e0: 662f 0a0a 2020 2020 4172 6773 3a0a 2020  f/..    Args:.  
+0000d7f0: 2020 2020 2020 7465 7874 3a20 7468 6520        text: the 
+0000d800: 7269 6368 7465 7874 2073 7472 696e 6720  richtext string 
+0000d810: 746f 2062 6520 6573 6361 7065 640a 0a20  to be escaped.. 
+0000d820: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+0000d830: 2020 2020 7468 6520 6573 6361 7065 6420      the escaped 
+0000d840: 7269 6368 7465 7874 2073 7472 696e 670a  richtext string.
+0000d850: 2020 2020 2222 220a 2020 2020 616c 6c6f      """.    allo
+0000d860: 7765 645f 7461 6773 203d 205b 0a20 2020  wed_tags = [.   
+0000d870: 2020 2020 2022 6128 205b 5e3e 5d2b 293f       "a( [^>]+)?
+0000d880: 222c 2020 2320 3c61 3e20 6973 2074 6865  ",  # <a> is the
+0000d890: 206f 6e6c 7920 7461 6720 7468 6174 2063   only tag that c
+0000d8a0: 616e 2068 6176 6520 6174 7472 6962 7574  an have attribut
+0000d8b0: 6573 0a20 2020 2020 2020 2022 7022 2c0a  es.        "p",.
+0000d8c0: 2020 2020 2020 2020 2265 6d22 2c0a 2020          "em",.  
+0000d8d0: 2020 2020 2020 2273 7472 6f6e 6722 2c0a        "strong",.
+0000d8e0: 2020 2020 2020 2020 2275 222c 0a20 2020          "u",.   
+0000d8f0: 2020 2020 2022 7375 6222 2c0a 2020 2020       "sub",.    
+0000d900: 2020 2020 2273 7570 222c 0a20 2020 2020      "sup",.     
+0000d910: 2020 2022 7374 7269 6b65 222c 0a20 2020     "strike",.   
+0000d920: 2020 2020 2022 6831 222c 0a20 2020 2020       "h1",.     
+0000d930: 2020 2022 6f6c 222c 0a20 2020 2020 2020     "ol",.       
+0000d940: 2022 756c 222c 0a20 2020 2020 2020 2022   "ul",.        "
+0000d950: 6c69 222c 0a20 2020 2020 2020 2022 7462  li",.        "tb
+0000d960: 6f64 7922 2c0a 2020 2020 2020 2020 2274  ody",.        "t
+0000d970: 6162 6c65 222c 0a20 2020 2020 2020 2022  able",.        "
+0000d980: 7472 222c 0a20 2020 2020 2020 2022 7464  tr",.        "td
+0000d990: 222c 0a20 2020 2020 2020 2022 6272 222c  ",.        "br",
+0000d9a0: 0a20 2020 2020 2020 2022 6872 222c 0a20  .        "hr",. 
+0000d9b0: 2020 2020 2020 2022 7072 6522 2c0a 2020         "pre",.  
+0000d9c0: 2020 2020 2020 2263 6974 6522 2c0a 2020        "cite",.  
+0000d9d0: 2020 2020 2020 2262 6c6f 636b 7175 6f74        "blockquot
+0000d9e0: 6522 2c0a 2020 2020 2020 2020 2263 6f64  e",.        "cod
+0000d9f0: 6522 2c0a 2020 2020 5d0a 2020 2020 616c  e",.    ].    al
+0000da00: 6c6f 7765 645f 7461 6773 5f72 6567 6578  lowed_tags_regex
+0000da10: 203d 2022 7c22 2e6a 6f69 6e28 616c 6c6f   = "|".join(allo
+0000da20: 7765 645f 7461 6773 290a 2020 2020 6c6f  wed_tags).    lo
+0000da30: 6f6b 6168 6561 6420 3d20 7266 2228 3f21  okahead = rf"(?!
+0000da40: 2f3f 287b 616c 6c6f 7765 645f 7461 6773  /?({allowed_tags
+0000da50: 5f72 6567 6578 7d29 2f3f 3e29 220a 2020  _regex})/?>)".  
+0000da60: 2020 696c 6c65 6761 6c5f 6c74 203d 2072    illegal_lt = r
+0000da70: 6622 3c7b 6c6f 6f6b 6168 6561 647d 220a  f"<{lookahead}".
+0000da80: 2020 2020 6c6f 6f6b 6265 6869 6e64 203d      lookbehind =
+0000da90: 2072 6622 283f 3c21 3c2f 3f28 7b61 6c6c   rf"(?<!</?({all
+0000daa0: 6f77 6564 5f74 6167 735f 7265 6765 787d  owed_tags_regex}
+0000dab0: 292f 3f29 220a 2020 2020 696c 6c65 6761  )/?)".    illega
+0000dac0: 6c5f 6774 203d 2072 6622 7b6c 6f6f 6b62  l_gt = rf"{lookb
+0000dad0: 6568 696e 647d 3e22 0a20 2020 2069 6c6c  ehind}>".    ill
+0000dae0: 6567 616c 5f61 6d70 203d 2072 2226 283f  egal_amp = r"&(?
+0000daf0: 215b 2361 2d7a 412d 5a30 2d39 5d2b 3b29  ![#a-zA-Z0-9]+;)
+0000db00: 220a 2020 2020 7465 7874 203d 2072 6567  ".    text = reg
+0000db10: 6578 2e73 7562 2869 6c6c 6567 616c 5f6c  ex.sub(illegal_l
+0000db20: 742c 2022 266c 743b 222c 2074 6578 7429  t, "&lt;", text)
+0000db30: 0a20 2020 2074 6578 7420 3d20 7265 6765  .    text = rege
+0000db40: 782e 7375 6228 696c 6c65 6761 6c5f 6774  x.sub(illegal_gt
+0000db50: 2c20 2226 6774 3b22 2c20 7465 7874 290a  , "&gt;", text).
+0000db60: 2020 2020 7465 7874 203d 2072 6567 6578      text = regex
+0000db70: 2e73 7562 2869 6c6c 6567 616c 5f61 6d70  .sub(illegal_amp
+0000db80: 2c20 2226 616d 703b 222c 2074 6578 7429  , "&amp;", text)
+0000db90: 0a20 2020 2072 6574 7572 6e20 7465 7874  .    return text
+0000dba0: 0a0a 0a64 6566 206d 616b 655f 7469 6d65  ...def make_time
+0000dbb0: 5f70 726f 7028 0a20 2020 206e 616d 653a  _prop(.    name:
+0000dbc0: 2073 7472 2c0a 2020 2020 7661 6c75 653a   str,.    value:
+0000dbd0: 2055 6e69 6f6e 5b50 726f 7065 7274 7945   Union[PropertyE
+0000dbe0: 6c65 6d65 6e74 2c20 7374 722c 2049 7465  lement, str, Ite
+0000dbf0: 7261 626c 655b 556e 696f 6e5b 5072 6f70  rable[Union[Prop
+0000dc00: 6572 7479 456c 656d 656e 742c 2073 7472  ertyElement, str
+0000dc10: 5d5d 5d2c 0a20 2020 2063 616c 6c69 6e67  ]]],.    calling
+0000dc20: 5f72 6573 6f75 7263 653a 2073 7472 203d  _resource: str =
+0000dc30: 2022 222c 0a29 202d 3e20 6574 7265 652e   "",.) -> etree.
+0000dc40: 5f45 6c65 6d65 6e74 3a0a 2020 2020 2222  _Element:.    ""
+0000dc50: 220a 2020 2020 4d61 6b65 2061 203c 7469  ".    Make a <ti
+0000dc60: 6d65 2d70 726f 703e 2066 726f 6d20 6f6e  me-prop> from on
+0000dc70: 6520 6f72 206d 6f72 6520 6461 7465 7469  e or more dateti
+0000dc80: 6d65 2076 616c 7565 7320 6f66 2074 6865  me values of the
+0000dc90: 2066 6f72 6d20 2232 3030 392d 3130 2d31   form "2009-10-1
+0000dca0: 3054 3132 3a30 303a 3030 2d30 353a 3030  0T12:00:00-05:00
+0000dcb0: 222e 2054 6865 2074 696d 6528 7329 2063  ". The time(s) c
+0000dcc0: 616e 2062 650a 2020 2020 7072 6f76 6964  an be.    provid
+0000dcd0: 6564 2061 7320 7374 7269 6e67 206f 7220  ed as string or 
+0000dce0: 6173 2050 726f 7065 7274 7945 6c65 6d65  as PropertyEleme
+0000dcf0: 6e74 2077 6974 6820 6120 7374 7269 6e67  nt with a string
+0000dd00: 2069 6e73 6964 652e 2049 6620 7072 6f76   inside. If prov
+0000dd10: 6964 6564 2061 7320 7374 7269 6e67 2c20  ided as string, 
+0000dd20: 7468 6520 7065 726d 6973 7369 6f6e 7320  the permissions 
+0000dd30: 6465 6661 756c 7420 746f 0a20 2020 2022  default to.    "
+0000dd40: 7072 6f70 2d64 6566 6175 6c74 222e 0a0a  prop-default"...
+0000dd50: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0000dd60: 2020 6e61 6d65 3a20 7468 6520 6e61 6d65    name: the name
+0000dd70: 206f 6620 7468 6973 2070 726f 7065 7274   of this propert
+0000dd80: 7920 6173 2064 6566 696e 6564 2069 6e20  y as defined in 
+0000dd90: 7468 6520 6f6e 746f 0a20 2020 2020 2020  the onto.       
+0000dda0: 2076 616c 7565 3a20 6f6e 6520 6f72 206d   value: one or m
+0000ddb0: 6f72 6520 4453 5020 7469 6d65 732c 2061  ore DSP times, a
+0000ddc0: 7320 7374 7269 6e67 2f50 726f 7065 7274  s string/Propert
+0000ddd0: 7945 6c65 6d65 6e74 2c20 6f72 2061 7320  yElement, or as 
+0000dde0: 6974 6572 6162 6c65 206f 6620 7374 7269  iterable of stri
+0000ddf0: 6e67 732f 5072 6f70 6572 7479 456c 656d  ngs/PropertyElem
+0000de00: 656e 7473 0a20 2020 2020 2020 2063 616c  ents.        cal
+0000de10: 6c69 6e67 5f72 6573 6f75 7263 653a 2074  ling_resource: t
+0000de20: 6865 206e 616d 6520 6f66 2074 6865 2070  he name of the p
+0000de30: 6172 656e 7420 7265 736f 7572 6365 2028  arent resource (
+0000de40: 666f 7220 6265 7474 6572 2065 7272 6f72  for better error
+0000de50: 206d 6573 7361 6765 7329 0a0a 2020 2020   messages)..    
+0000de60: 5761 726e 733a 0a20 2020 2020 2020 2049  Warns:.        I
+0000de70: 6620 6f6e 6520 6f66 2074 6865 2076 616c  f one of the val
+0000de80: 7565 7320 6973 206e 6f74 2061 2076 616c  ues is not a val
+0000de90: 6964 2044 5350 2074 696d 6520 7374 7269  id DSP time stri
+0000dea0: 6e67 0a0a 2020 2020 5265 7475 726e 733a  ng..    Returns:
+0000deb0: 0a20 2020 2020 2020 2061 6e20 6574 7265  .        an etre
+0000dec0: 652e 5f45 6c65 6d65 6e74 2074 6861 7420  e._Element that 
+0000ded0: 6361 6e20 6265 2061 7070 656e 6465 6420  can be appended 
+0000dee0: 746f 2074 6865 2070 6172 656e 7420 7265  to the parent re
+0000def0: 736f 7572 6365 2077 6974 6820 7265 736f  source with reso
+0000df00: 7572 6365 2e61 7070 656e 6428 6d61 6b65  urce.append(make
+0000df10: 5f2a 5f70 726f 7028 2e2e 2e29 290a 0a20  _*_prop(...)).. 
+0000df20: 2020 2045 7861 6d70 6c65 733a 0a20 2020     Examples:.   
+0000df30: 2020 2020 203e 3e3e 2065 7863 656c 3278       >>> excel2x
+0000df40: 6d6c 2e6d 616b 655f 7469 6d65 5f70 726f  ml.make_time_pro
+0000df50: 7028 223a 7465 7374 7072 6f70 6572 7479  p(":testproperty
+0000df60: 222c 2022 3230 3039 2d31 302d 3130 5431  ", "2009-10-10T1
+0000df70: 323a 3030 3a30 302d 3035 3a30 3022 290a  2:00:00-05:00").
+0000df80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df90: 3c74 696d 652d 7072 6f70 206e 616d 653d  <time-prop name=
+0000dfa0: 223a 7465 7374 7072 6f70 6572 7479 223e  ":testproperty">
+0000dfb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dfc0: 2020 2020 203c 7469 6d65 2070 6572 6d69       <time permi
+0000dfd0: 7373 696f 6e73 3d22 7072 6f70 2d64 6566  ssions="prop-def
+0000dfe0: 6175 6c74 223e 0a20 2020 2020 2020 2020  ault">.         
+0000dff0: 2020 2020 2020 2020 2020 2020 2020 2032                 2
+0000e000: 3030 392d 3130 2d31 3054 3132 3a30 303a  009-10-10T12:00:
+0000e010: 3030 2d30 353a 3030 0a20 2020 2020 2020  00-05:00.       
+0000e020: 2020 2020 2020 2020 2020 2020 203c 2f74               </t
+0000e030: 696d 653e 0a20 2020 2020 2020 2020 2020  ime>.           
+0000e040: 2020 2020 203c 2f74 696d 652d 7072 6f70       </time-prop
+0000e050: 3e0a 2020 2020 2020 2020 3e3e 3e20 6578  >.        >>> ex
+0000e060: 6365 6c32 786d 6c2e 6d61 6b65 5f74 696d  cel2xml.make_tim
+0000e070: 655f 7072 6f70 2822 3a74 6573 7470 726f  e_prop(":testpro
+0000e080: 7065 7274 7922 2c20 6578 6365 6c32 786d  perty", excel2xm
+0000e090: 6c2e 5072 6f70 6572 7479 456c 656d 656e  l.PropertyElemen
+0000e0a0: 7428 2232 3030 392d 3130 2d31 3054 3132  t("2009-10-10T12
+0000e0b0: 3a30 303a 3030 2d30 353a 3030 222c 2070  :00:00-05:00", p
+0000e0c0: 6572 6d69 7373 696f 6e73 3d22 7072 6f70  ermissions="prop
+0000e0d0: 2d72 6573 7472 6963 7465 6422 2c20 636f  -restricted", co
+0000e0e0: 6d6d 656e 743d 2265 7861 6d70 6c65 2229  mment="example")
+0000e0f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000e100: 2020 3c74 696d 652d 7072 6f70 206e 616d    <time-prop nam
+0000e110: 653d 223a 7465 7374 7072 6f70 6572 7479  e=":testproperty
+0000e120: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+0000e130: 2020 2020 2020 203c 7469 6d65 2070 6572         <time per
+0000e140: 6d69 7373 696f 6e73 3d22 7072 6f70 2d72  missions="prop-r
+0000e150: 6573 7472 6963 7465 6422 2063 6f6d 6d65  estricted" comme
+0000e160: 6e74 3d22 6578 616d 706c 6522 3e0a 2020  nt="example">.  
 0000e170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e180: 2032 3030 392d 3130 2d31 3054 3132 3a30   2009-10-10T12:0
-0000e190: 303a 3030 2d30 353a 3030 0a20 2020 2020  0:00-05:00.     
-0000e1a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000e1b0: 2f74 696d 653e 0a20 2020 2020 2020 2020  /time>.         
-0000e1c0: 2020 2020 2020 203c 2f74 696d 652d 7072         </time-pr
-0000e1d0: 6f70 3e0a 2020 2020 2020 2020 3e3e 3e20  op>.        >>> 
-0000e1e0: 6578 6365 6c32 786d 6c2e 6d61 6b65 5f74  excel2xml.make_t
-0000e1f0: 696d 655f 7072 6f70 2822 3a74 6573 7470  ime_prop(":testp
-0000e200: 726f 7065 7274 7922 2c20 5b22 3230 3039  roperty", ["2009
-0000e210: 2d31 302d 3130 5431 323a 3030 3a30 302d  -10-10T12:00:00-
-0000e220: 3035 3a30 3022 2c20 2231 3930 312d 3031  05:00", "1901-01
-0000e230: 2d30 3154 3031 3a30 303a 3030 2d30 303a  -01T01:00:00-00:
-0000e240: 3030 225d 290a 2020 2020 2020 2020 2020  00"]).          
-0000e250: 2020 2020 2020 3c74 696d 652d 7072 6f70        <time-prop
-0000e260: 206e 616d 653d 223a 7465 7374 7072 6f70   name=":testprop
-0000e270: 6572 7479 223e 0a20 2020 2020 2020 2020  erty">.         
-0000e280: 2020 2020 2020 2020 2020 203c 7469 6d65             <time
-0000e290: 2070 6572 6d69 7373 696f 6e73 3d22 7072   permissions="pr
-0000e2a0: 6f70 2d64 6566 6175 6c74 223e 0a20 2020  op-default">.   
-0000e2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2c0: 2020 2020 2032 3030 392d 3130 2d31 3054       2009-10-10T
-0000e2d0: 3132 3a30 303a 3030 2d30 353a 3030 0a20  12:00:00-05:00. 
-0000e2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e2f0: 2020 203c 2f74 696d 653e 0a20 2020 2020     </time>.     
-0000e300: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000e310: 7469 6d65 2070 6572 6d69 7373 696f 6e73  time permissions
-0000e320: 3d22 7072 6f70 2d64 6566 6175 6c74 223e  ="prop-default">
-0000e330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e340: 2020 2020 2020 2020 2031 3930 312d 3031           1901-01
-0000e350: 2d30 3154 3031 3a30 303a 3030 2d30 303a  -01T01:00:00-00:
-0000e360: 3030 320a 2020 2020 2020 2020 2020 2020  002.            
-0000e370: 2020 2020 2020 2020 3c2f 7469 6d65 3e0a          </time>.
-0000e380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e390: 3c2f 7469 6d65 2d70 726f 703e 0a0a 2020  </time-prop>..  
-0000e3a0: 2020 5365 6520 6874 7470 733a 2f2f 646f    See https://do
-0000e3b0: 6373 2e64 6173 6368 2e73 7769 7373 2f6c  cs.dasch.swiss/l
-0000e3c0: 6174 6573 742f 4453 502d 544f 4f4c 532f  atest/DSP-TOOLS/
-0000e3d0: 6669 6c65 2d66 6f72 6d61 7473 2f78 6d6c  file-formats/xml
-0000e3e0: 2d64 6174 612d 6669 6c65 2f23 7469 6d65  -data-file/#time
-0000e3f0: 2d70 726f 700a 2020 2020 2222 220a 0a20  -prop.    """.. 
-0000e400: 2020 2023 2063 6865 636b 2074 6865 2069     # check the i
-0000e410: 6e70 7574 3a20 7072 6570 6172 6520 6120  nput: prepare a 
-0000e420: 6c69 7374 2077 6974 6820 7661 6c69 6420  list with valid 
-0000e430: 7661 6c75 6573 0a20 2020 2076 616c 7565  values.    value
-0000e440: 7320 3d20 7072 6570 6172 655f 7661 6c75  s = prepare_valu
-0000e450: 6528 7661 6c75 6529 0a0a 2020 2020 2320  e(value)..    # 
-0000e460: 6368 6563 6b20 7661 6c75 6520 7479 7065  check value type
-0000e470: 0a20 2020 2076 616c 6964 6174 696f 6e5f  .    validation_
-0000e480: 7265 6765 7820 3d20 7222 5e5c 647b 347d  regex = r"^\d{4}
-0000e490: 2d5b 302d 315d 5c64 2d5b 302d 335d 5c64  -[0-1]\d-[0-3]\d
-0000e4a0: 545b 302d 325d 5c64 3a5b 302d 355d 5c64  T[0-2]\d:[0-5]\d
-0000e4b0: 3a5b 302d 355d 5c64 282e 5c64 7b31 2c31  :[0-5]\d(.\d{1,1
-0000e4c0: 327d 293f 285a 7c5b 2b2d 5d5b 302d 315d  2})?(Z|[+-][0-1]
-0000e4d0: 5c64 3a5b 302d 355d 5c64 2924 220a 2020  \d:[0-5]\d)$".  
-0000e4e0: 2020 666f 7220 7661 6c20 696e 2076 616c    for val in val
-0000e4f0: 7565 733a 0a20 2020 2020 2020 2069 6620  ues:.        if 
-0000e500: 6e6f 7420 7265 6765 782e 7365 6172 6368  not regex.search
-0000e510: 2876 616c 6964 6174 696f 6e5f 7265 6765  (validation_rege
-0000e520: 782c 2073 7472 2876 616c 2e76 616c 7565  x, str(val.value
-0000e530: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-0000e540: 6d73 6720 3d20 280a 2020 2020 2020 2020  msg = (.        
-0000e550: 2020 2020 2020 2020 6622 4661 696c 6564          f"Failed
-0000e560: 2076 616c 6964 6174 696f 6e20 696e 2072   validation in r
-0000e570: 6573 6f75 7263 6520 277b 6361 6c6c 696e  esource '{callin
-0000e580: 675f 7265 736f 7572 6365 7d27 2c20 7072  g_resource}', pr
-0000e590: 6f70 6572 7479 2027 7b6e 616d 657d 273a  operty '{name}':
-0000e5a0: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-0000e5b0: 2020 2066 2227 7b76 616c 2e76 616c 7565     f"'{val.value
-0000e5c0: 7d27 2069 7320 6e6f 7420 6120 7661 6c69  }' is not a vali
-0000e5d0: 6420 4453 5020 7469 6d65 2e22 0a20 2020  d DSP time.".   
-0000e5e0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000e5f0: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
-0000e600: 7761 726e 2844 7370 546f 6f6c 7355 7365  warn(DspToolsUse
-0000e610: 7257 6172 6e69 6e67 286d 7367 2929 0a0a  rWarning(msg))..
-0000e620: 2020 2020 2320 6d61 6b65 2078 6d6c 2073      # make xml s
-0000e630: 7472 7563 7475 7265 206f 6620 7468 6520  tructure of the 
-0000e640: 7661 6c69 6420 7661 6c75 6573 0a20 2020  valid values.   
-0000e650: 2070 726f 705f 203d 2065 7472 6565 2e45   prop_ = etree.E
-0000e660: 6c65 6d65 6e74 280a 2020 2020 2020 2020  lement(.        
-0000e670: 227b 2573 7d74 696d 652d 7072 6f70 2220  "{%s}time-prop" 
-0000e680: 2520 786d 6c5f 6e61 6d65 7370 6163 655f  % xml_namespace_
-0000e690: 6d61 705b 4e6f 6e65 5d2c 0a20 2020 2020  map[None],.     
-0000e6a0: 2020 206e 616d 653d 6e61 6d65 2c0a 2020     name=name,.  
-0000e6b0: 2020 2020 2020 6e73 6d61 703d 786d 6c5f        nsmap=xml_
-0000e6c0: 6e61 6d65 7370 6163 655f 6d61 702c 0a20  namespace_map,. 
-0000e6d0: 2020 2029 0a20 2020 2066 6f72 2076 616c     ).    for val
-0000e6e0: 2069 6e20 7661 6c75 6573 3a0a 2020 2020   in values:.    
-0000e6f0: 2020 2020 6b77 6172 6773 203d 207b 2270      kwargs = {"p
-0000e700: 6572 6d69 7373 696f 6e73 223a 2076 616c  ermissions": val
-0000e710: 2e70 6572 6d69 7373 696f 6e73 7d0a 2020  .permissions}.  
-0000e720: 2020 2020 2020 6966 2076 616c 2e63 6f6d        if val.com
-0000e730: 6d65 6e74 2061 6e64 2063 6865 636b 5f6e  ment and check_n
-0000e740: 6f74 6e61 2876 616c 2e63 6f6d 6d65 6e74  otna(val.comment
-0000e750: 293a 0a20 2020 2020 2020 2020 2020 206b  ):.            k
-0000e760: 7761 7267 735b 2263 6f6d 6d65 6e74 225d  wargs["comment"]
-0000e770: 203d 2076 616c 2e63 6f6d 6d65 6e74 0a20   = val.comment. 
-0000e780: 2020 2020 2020 2076 616c 7565 5f20 3d20         value_ = 
-0000e790: 6574 7265 652e 456c 656d 656e 7428 0a20  etree.Element(. 
-0000e7a0: 2020 2020 2020 2020 2020 2022 7b25 737d             "{%s}
-0000e7b0: 7469 6d65 2220 2520 786d 6c5f 6e61 6d65  time" % xml_name
-0000e7c0: 7370 6163 655f 6d61 705b 4e6f 6e65 5d2c  space_map[None],
-0000e7d0: 0a20 2020 2020 2020 2020 2020 202a 2a6b  .            **k
-0000e7e0: 7761 7267 732c 2020 2320 7479 7065 3a20  wargs,  # type: 
-0000e7f0: 6967 6e6f 7265 5b61 7267 2d74 7970 655d  ignore[arg-type]
-0000e800: 0a20 2020 2020 2020 2020 2020 206e 736d  .            nsm
-0000e810: 6170 3d78 6d6c 5f6e 616d 6573 7061 6365  ap=xml_namespace
-0000e820: 5f6d 6170 2c0a 2020 2020 2020 2020 290a  _map,.        ).
-0000e830: 2020 2020 2020 2020 7661 6c75 655f 2e74          value_.t
-0000e840: 6578 7420 3d20 7374 7228 7661 6c2e 7661  ext = str(val.va
-0000e850: 6c75 6529 0a20 2020 2020 2020 2070 726f  lue).        pro
-0000e860: 705f 2e61 7070 656e 6428 7661 6c75 655f  p_.append(value_
-0000e870: 290a 0a20 2020 2072 6574 7572 6e20 7072  )..    return pr
-0000e880: 6f70 5f0a 0a0a 6465 6620 6d61 6b65 5f75  op_...def make_u
-0000e890: 7269 5f70 726f 7028 0a20 2020 206e 616d  ri_prop(.    nam
-0000e8a0: 653a 2073 7472 2c0a 2020 2020 7661 6c75  e: str,.    valu
-0000e8b0: 653a 2055 6e69 6f6e 5b50 726f 7065 7274  e: Union[Propert
-0000e8c0: 7945 6c65 6d65 6e74 2c20 7374 722c 2049  yElement, str, I
-0000e8d0: 7465 7261 626c 655b 556e 696f 6e5b 5072  terable[Union[Pr
-0000e8e0: 6f70 6572 7479 456c 656d 656e 742c 2073  opertyElement, s
-0000e8f0: 7472 5d5d 5d2c 0a20 2020 2063 616c 6c69  tr]]],.    calli
-0000e900: 6e67 5f72 6573 6f75 7263 653a 2073 7472  ng_resource: str
-0000e910: 203d 2022 222c 0a29 202d 3e20 6574 7265   = "",.) -> etre
-0000e920: 652e 5f45 6c65 6d65 6e74 3a0a 2020 2020  e._Element:.    
-0000e930: 2222 220a 2020 2020 4d61 6b65 2061 6e20  """.    Make an 
-0000e940: 3c75 7269 2d70 726f 703e 2066 726f 6d20  <uri-prop> from 
-0000e950: 6f6e 6520 6f72 206d 6f72 6520 5552 4973  one or more URIs
-0000e960: 2e20 5468 6520 5552 4928 7329 2063 616e  . The URI(s) can
-0000e970: 2062 6520 7072 6f76 6964 6564 2061 7320   be provided as 
-0000e980: 7374 7269 6e67 206f 7220 6173 2050 726f  string or as Pro
-0000e990: 7065 7274 7945 6c65 6d65 6e74 2077 6974  pertyElement wit
-0000e9a0: 6820 6120 7374 7269 6e67 0a20 2020 2069  h a string.    i
-0000e9b0: 6e73 6964 652e 2049 6620 7072 6f76 6964  nside. If provid
-0000e9c0: 6564 2061 7320 7374 7269 6e67 2c20 7468  ed as string, th
-0000e9d0: 6520 7065 726d 6973 7369 6f6e 7320 6465  e permissions de
-0000e9e0: 6661 756c 7420 746f 2022 7072 6f70 2d64  fault to "prop-d
-0000e9f0: 6566 6175 6c74 222e 0a0a 2020 2020 4172  efault"...    Ar
-0000ea00: 6773 3a0a 2020 2020 2020 2020 6e61 6d65  gs:.        name
-0000ea10: 3a20 7468 6520 6e61 6d65 206f 6620 7468  : the name of th
-0000ea20: 6973 2070 726f 7065 7274 7920 6173 2064  is property as d
-0000ea30: 6566 696e 6564 2069 6e20 7468 6520 6f6e  efined in the on
-0000ea40: 746f 0a20 2020 2020 2020 2076 616c 7565  to.        value
-0000ea50: 3a20 6f6e 6520 6f72 206d 6f72 6520 5552  : one or more UR
-0000ea60: 4973 2c20 6173 2073 7472 696e 672f 5072  Is, as string/Pr
-0000ea70: 6f70 6572 7479 456c 656d 656e 742c 206f  opertyElement, o
-0000ea80: 7220 6173 2069 7465 7261 626c 6520 6f66  r as iterable of
-0000ea90: 2073 7472 696e 6773 2f50 726f 7065 7274   strings/Propert
-0000eaa0: 7945 6c65 6d65 6e74 730a 2020 2020 2020  yElements.      
-0000eab0: 2020 6361 6c6c 696e 675f 7265 736f 7572    calling_resour
-0000eac0: 6365 3a20 7468 6520 6e61 6d65 206f 6620  ce: the name of 
-0000ead0: 7468 6520 7061 7265 6e74 2072 6573 6f75  the parent resou
-0000eae0: 7263 6520 2866 6f72 2062 6574 7465 7220  rce (for better 
-0000eaf0: 6572 726f 7220 6d65 7373 6167 6573 290a  error messages).
-0000eb00: 0a20 2020 2057 6172 6e73 3a0a 2020 2020  .    Warns:.    
-0000eb10: 2020 2020 4966 206f 6e65 206f 6620 7468      If one of th
-0000eb20: 6520 7661 6c75 6573 2069 7320 6e6f 7420  e values is not 
-0000eb30: 6120 7661 6c69 6420 5552 490a 0a20 2020  a valid URI..   
-0000eb40: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-0000eb50: 2020 616e 2065 7472 6565 2e5f 456c 656d    an etree._Elem
-0000eb60: 656e 7420 7468 6174 2063 616e 2062 6520  ent that can be 
-0000eb70: 6170 7065 6e64 6564 2074 6f20 7468 6520  appended to the 
-0000eb80: 7061 7265 6e74 2072 6573 6f75 7263 6520  parent resource 
-0000eb90: 7769 7468 2072 6573 6f75 7263 652e 6170  with resource.ap
-0000eba0: 7065 6e64 286d 616b 655f 2a5f 7072 6f70  pend(make_*_prop
-0000ebb0: 282e 2e2e 2929 0a0a 2020 2020 4578 616d  (...))..    Exam
-0000ebc0: 706c 6573 3a0a 2020 2020 2020 2020 3e3e  ples:.        >>
-0000ebd0: 3e20 6578 6365 6c32 786d 6c2e 6d61 6b65  > excel2xml.make
-0000ebe0: 5f75 7269 5f70 726f 7028 223a 7465 7374  _uri_prop(":test
-0000ebf0: 7072 6f70 6572 7479 222c 2022 7777 772e  property", "www.
-0000ec00: 7465 7374 2e63 6f6d 2229 0a20 2020 2020  test.com").     
-0000ec10: 2020 2020 2020 2020 2020 203c 7572 692d             <uri-
-0000ec20: 7072 6f70 206e 616d 653d 223a 7465 7374  prop name=":test
-0000ec30: 7072 6f70 6572 7479 223e 0a20 2020 2020  property">.     
-0000ec40: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-0000ec50: 7572 6920 7065 726d 6973 7369 6f6e 733d  uri permissions=
-0000ec60: 2270 726f 702d 6465 6661 756c 7422 3e77  "prop-default">w
-0000ec70: 7777 2e74 6573 742e 636f 6d3c 2f75 7269  ww.test.com</uri
-0000ec80: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-0000ec90: 2020 3c2f 7572 692d 7072 6f70 3e0a 2020    </uri-prop>.  
-0000eca0: 2020 2020 2020 3e3e 3e20 6578 6365 6c32        >>> excel2
-0000ecb0: 786d 6c2e 6d61 6b65 5f75 7269 5f70 726f  xml.make_uri_pro
-0000ecc0: 7028 223a 7465 7374 7072 6f70 6572 7479  p(":testproperty
-0000ecd0: 222c 2065 7863 656c 3278 6d6c 2e50 726f  ", excel2xml.Pro
-0000ece0: 7065 7274 7945 6c65 6d65 6e74 2822 7777  pertyElement("ww
-0000ecf0: 772e 7465 7374 2e63 6f6d 222c 2070 6572  w.test.com", per
-0000ed00: 6d69 7373 696f 6e73 3d22 7072 6f70 2d72  missions="prop-r
-0000ed10: 6573 7472 6963 7465 6422 2c20 636f 6d6d  estricted", comm
-0000ed20: 656e 743d 2265 7861 6d70 6c65 2229 290a  ent="example")).
-0000ed30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed40: 3c75 7269 2d70 726f 7020 6e61 6d65 3d22  <uri-prop name="
-0000ed50: 3a74 6573 7470 726f 7065 7274 7922 3e0a  :testproperty">.
-0000ed60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ed70: 2020 2020 3c75 7269 2070 6572 6d69 7373      <uri permiss
-0000ed80: 696f 6e73 3d22 7072 6f70 2d72 6573 7472  ions="prop-restr
-0000ed90: 6963 7465 6422 2063 6f6d 6d65 6e74 3d22  icted" comment="
-0000eda0: 6578 616d 706c 6522 3e77 7777 2e74 6573  example">www.tes
-0000edb0: 742e 636f 6d3c 2f75 7269 3e0a 2020 2020  t.com</uri>.    
-0000edc0: 2020 2020 2020 2020 2020 2020 3c2f 7572              </ur
-0000edd0: 692d 7072 6f70 3e0a 2020 2020 2020 2020  i-prop>.        
-0000ede0: 3e3e 3e20 6578 6365 6c32 786d 6c2e 6d61  >>> excel2xml.ma
-0000edf0: 6b65 5f75 7269 5f70 726f 7028 223a 7465  ke_uri_prop(":te
-0000ee00: 7374 7072 6f70 6572 7479 222c 205b 2277  stproperty", ["w
-0000ee10: 7777 2e31 2e63 6f6d 222c 2022 7777 772e  ww.1.com", "www.
-0000ee20: 322e 636f 6d22 5d29 0a20 2020 2020 2020  2.com"]).       
-0000ee30: 2020 2020 2020 2020 203c 7572 692d 7072           <uri-pr
-0000ee40: 6f70 206e 616d 653d 223a 7465 7374 7072  op name=":testpr
-0000ee50: 6f70 6572 7479 223e 0a20 2020 2020 2020  operty">.       
-0000ee60: 2020 2020 2020 2020 2020 2020 203c 7572               <ur
-0000ee70: 6920 7065 726d 6973 7369 6f6e 733d 2270  i permissions="p
-0000ee80: 726f 702d 6465 6661 756c 7422 3e77 7777  rop-default">www
-0000ee90: 2e31 2e63 6f6d 3c2f 7572 693e 0a20 2020  .1.com</uri>.   
-0000eea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eeb0: 203c 7572 6920 7065 726d 6973 7369 6f6e   <uri permission
-0000eec0: 733d 2270 726f 702d 6465 6661 756c 7422  s="prop-default"
-0000eed0: 3e77 7777 2e32 2e63 6f6d 3c2f 7572 693e  >www.2.com</uri>
-0000eee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000eef0: 203c 2f75 7269 2d70 726f 703e 0a0a 2020   </uri-prop>..  
-0000ef00: 2020 5365 6520 6874 7470 733a 2f2f 646f    See https://do
-0000ef10: 6373 2e64 6173 6368 2e73 7769 7373 2f6c  cs.dasch.swiss/l
-0000ef20: 6174 6573 742f 4453 502d 544f 4f4c 532f  atest/DSP-TOOLS/
-0000ef30: 6669 6c65 2d66 6f72 6d61 7473 2f78 6d6c  file-formats/xml
-0000ef40: 2d64 6174 612d 6669 6c65 2f23 7572 692d  -data-file/#uri-
-0000ef50: 7072 6f70 0a20 2020 2022 2222 0a0a 2020  prop.    """..  
-0000ef60: 2020 2320 6368 6563 6b20 7468 6520 696e    # check the in
-0000ef70: 7075 743a 2070 7265 7061 7265 2061 206c  put: prepare a l
-0000ef80: 6973 7420 7769 7468 2076 616c 6964 2076  ist with valid v
-0000ef90: 616c 7565 730a 2020 2020 7661 6c75 6573  alues.    values
-0000efa0: 203d 2070 7265 7061 7265 5f76 616c 7565   = prepare_value
-0000efb0: 2876 616c 7565 290a 0a20 2020 2023 2063  (value)..    # c
-0000efc0: 6865 636b 2076 616c 7565 2074 7970 650a  heck value type.
-0000efd0: 2020 2020 666f 7220 7661 6c20 696e 2076      for val in v
-0000efe0: 616c 7565 733a 0a20 2020 2020 2020 2069  alues:.        i
-0000eff0: 6620 6e6f 7420 6973 5f75 7269 2873 7472  f not is_uri(str
-0000f000: 2876 616c 2e76 616c 7565 2929 3a0a 2020  (val.value)):.  
-0000f010: 2020 2020 2020 2020 2020 6d73 6720 3d20            msg = 
-0000f020: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000f030: 2020 6622 4661 696c 6564 2076 616c 6964    f"Failed valid
-0000f040: 6174 696f 6e20 696e 2072 6573 6f75 7263  ation in resourc
-0000f050: 6520 277b 6361 6c6c 696e 675f 7265 736f  e '{calling_reso
-0000f060: 7572 6365 7d27 2c20 7072 6f70 6572 7479  urce}', property
-0000f070: 2027 7b6e 616d 657d 273a 2022 0a20 2020   '{name}': ".   
-0000f080: 2020 2020 2020 2020 2020 2020 2066 2227               f"'
-0000f090: 7b76 616c 2e76 616c 7565 7d27 2069 7320  {val.value}' is 
-0000f0a0: 6e6f 7420 6120 7661 6c69 6420 5552 492e  not a valid URI.
-0000f0b0: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
-0000f0c0: 2020 2020 2020 2020 2020 2020 7761 726e              warn
-0000f0d0: 696e 6773 2e77 6172 6e28 4473 7054 6f6f  ings.warn(DspToo
-0000f0e0: 6c73 5573 6572 5761 726e 696e 6728 6d73  lsUserWarning(ms
-0000f0f0: 6729 290a 0a20 2020 2023 206d 616b 6520  g))..    # make 
-0000f100: 786d 6c20 7374 7275 6374 7572 6520 6f66  xml structure of
-0000f110: 2074 6865 2076 616c 6964 2076 616c 7565   the valid value
-0000f120: 730a 2020 2020 7072 6f70 5f20 3d20 6574  s.    prop_ = et
-0000f130: 7265 652e 456c 656d 656e 7428 0a20 2020  ree.Element(.   
-0000f140: 2020 2020 2022 7b25 737d 7572 692d 7072       "{%s}uri-pr
-0000f150: 6f70 2220 2520 786d 6c5f 6e61 6d65 7370  op" % xml_namesp
-0000f160: 6163 655f 6d61 705b 4e6f 6e65 5d2c 0a20  ace_map[None],. 
-0000f170: 2020 2020 2020 206e 616d 653d 6e61 6d65         name=name
-0000f180: 2c0a 2020 2020 2020 2020 6e73 6d61 703d  ,.        nsmap=
-0000f190: 786d 6c5f 6e61 6d65 7370 6163 655f 6d61  xml_namespace_ma
-0000f1a0: 702c 0a20 2020 2029 0a20 2020 2066 6f72  p,.    ).    for
-0000f1b0: 2076 616c 2069 6e20 7661 6c75 6573 3a0a   val in values:.
-0000f1c0: 2020 2020 2020 2020 6b77 6172 6773 203d          kwargs =
-0000f1d0: 207b 2270 6572 6d69 7373 696f 6e73 223a   {"permissions":
-0000f1e0: 2076 616c 2e70 6572 6d69 7373 696f 6e73   val.permissions
-0000f1f0: 7d0a 2020 2020 2020 2020 6966 2076 616c  }.        if val
-0000f200: 2e63 6f6d 6d65 6e74 2061 6e64 2063 6865  .comment and che
-0000f210: 636b 5f6e 6f74 6e61 2876 616c 2e63 6f6d  ck_notna(val.com
-0000f220: 6d65 6e74 293a 0a20 2020 2020 2020 2020  ment):.         
-0000f230: 2020 206b 7761 7267 735b 2263 6f6d 6d65     kwargs["comme
-0000f240: 6e74 225d 203d 2076 616c 2e63 6f6d 6d65  nt"] = val.comme
-0000f250: 6e74 0a20 2020 2020 2020 2076 616c 7565  nt.        value
-0000f260: 5f20 3d20 6574 7265 652e 456c 656d 656e  _ = etree.Elemen
-0000f270: 7428 0a20 2020 2020 2020 2020 2020 2022  t(.            "
-0000f280: 7b25 737d 7572 6922 2025 2078 6d6c 5f6e  {%s}uri" % xml_n
-0000f290: 616d 6573 7061 6365 5f6d 6170 5b4e 6f6e  amespace_map[Non
-0000f2a0: 655d 2c0a 2020 2020 2020 2020 2020 2020  e],.            
-0000f2b0: 2a2a 6b77 6172 6773 2c20 2023 2074 7970  **kwargs,  # typ
-0000f2c0: 653a 2069 676e 6f72 655b 6172 672d 7479  e: ignore[arg-ty
-0000f2d0: 7065 5d0a 2020 2020 2020 2020 2020 2020  pe].            
-0000f2e0: 6e73 6d61 703d 786d 6c5f 6e61 6d65 7370  nsmap=xml_namesp
-0000f2f0: 6163 655f 6d61 702c 0a20 2020 2020 2020  ace_map,.       
-0000f300: 2029 0a20 2020 2020 2020 2076 616c 7565   ).        value
-0000f310: 5f2e 7465 7874 203d 2073 7472 2876 616c  _.text = str(val
-0000f320: 2e76 616c 7565 290a 2020 2020 2020 2020  .value).        
-0000f330: 7072 6f70 5f2e 6170 7065 6e64 2876 616c  prop_.append(val
-0000f340: 7565 5f29 0a0a 2020 2020 7265 7475 726e  ue_)..    return
-0000f350: 2070 726f 705f 0a0a 0a64 6566 206d 616b   prop_...def mak
-0000f360: 655f 7265 6769 6f6e 2820 2023 206e 6f71  e_region(  # noq
-0000f370: 613a 2044 3431 3720 2875 6e64 6f63 756d  a: D417 (undocum
-0000f380: 656e 7465 642d 7061 7261 6d29 0a20 2020  ented-param).   
-0000f390: 206c 6162 656c 3a20 7374 722c 0a20 2020   label: str,.   
-0000f3a0: 2069 643a 2073 7472 2c0a 2020 2020 7065   id: str,.    pe
-0000f3b0: 726d 6973 7369 6f6e 733a 2073 7472 203d  rmissions: str =
-0000f3c0: 2022 7265 732d 6465 6661 756c 7422 2c0a   "res-default",.
-0000f3d0: 2020 2020 6172 6b3a 204f 7074 696f 6e61      ark: Optiona
-0000f3e0: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
-0000f3f0: 2020 2069 7269 3a20 4f70 7469 6f6e 616c     iri: Optional
-0000f400: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-0000f410: 2020 6372 6561 7469 6f6e 5f64 6174 653a    creation_date:
-0000f420: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-0000f430: 204e 6f6e 652c 0a29 202d 3e20 6574 7265   None,.) -> etre
-0000f440: 652e 5f45 6c65 6d65 6e74 3a0a 2020 2020  e._Element:.    
-0000f450: 2222 220a 2020 2020 4372 6561 7465 7320  """.    Creates 
-0000f460: 616e 2065 6d70 7479 2072 6567 696f 6e20  an empty region 
-0000f470: 656c 656d 656e 742c 2077 6974 6820 7468  element, with th
-0000f480: 6520 6174 7472 6962 7574 6573 2061 7320  e attributes as 
-0000f490: 7370 6563 6966 6965 6420 6279 2074 6865  specified by the
-0000f4a0: 2061 7267 756d 656e 7473 0a0a 2020 2020   arguments..    
-0000f4b0: 4172 6773 3a0a 2020 2020 2020 2020 5468  Args:.        Th
-0000f4c0: 6520 6172 6775 6d65 6e74 7320 636f 7272  e arguments corr
-0000f4d0: 6573 706f 6e64 2031 3a31 2074 6f20 7468  espond 1:1 to th
-0000f4e0: 6520 6174 7472 6962 7574 6573 206f 6620  e attributes of 
-0000f4f0: 7468 6520 3c72 6567 696f 6e3e 2065 6c65  the <region> ele
-0000f500: 6d65 6e74 2e0a 0a20 2020 2052 6169 7365  ment...    Raise
-0000f510: 733a 0a20 2020 2020 2020 2057 6172 6e69  s:.        Warni
-0000f520: 6e67 3a20 6966 2062 6f74 6820 616e 2041  ng: if both an A
-0000f530: 524b 2061 6e64 2061 6e20 4952 4920 6172  RK and an IRI ar
-0000f540: 6520 7072 6f76 6964 6564 0a20 2020 2020  e provided.     
-0000f550: 2020 2042 6173 6545 7272 6f72 3a20 6966     BaseError: if
-0000f560: 2074 6865 2063 7265 6174 696f 6e20 6461   the creation da
-0000f570: 7465 2069 7320 696e 7661 6c69 640a 0a20  te is invalid.. 
-0000f580: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-0000f590: 2020 2020 5468 6520 7265 6769 6f6e 2065      The region e
-0000f5a0: 6c65 6d65 6e74 2c20 7769 7468 6f75 7420  lement, without 
-0000f5b0: 616e 7920 6368 696c 6472 656e 2c20 6275  any children, bu
-0000f5c0: 7420 7769 7468 2074 6865 2061 7474 7269  t with the attri
-0000f5d0: 6275 7465 733a 0a20 2020 2020 2020 203c  butes:.        <
-0000f5e0: 7265 6769 6f6e 206c 6162 656c 3d6c 6162  region label=lab
-0000f5f0: 656c 2069 643d 6964 2070 6572 6d69 7373  el id=id permiss
-0000f600: 696f 6e73 3d70 6572 6d69 7373 696f 6e73  ions=permissions
-0000f610: 2061 726b 3d61 726b 2069 7269 3d69 7269   ark=ark iri=iri
-0000f620: 3e3c 2f72 6567 696f 6e3e 0a0a 2020 2020  ></region>..    
-0000f630: 4578 616d 706c 6573 3a0a 2020 2020 2020  Examples:.      
-0000f640: 2020 3e3e 3e20 7265 6769 6f6e 203d 2065    >>> region = e
-0000f650: 7863 656c 3278 6d6c 2e6d 616b 655f 7265  xcel2xml.make_re
-0000f660: 6769 6f6e 2822 6c61 6265 6c22 2c20 2269  gion("label", "i
-0000f670: 6422 290a 2020 2020 2020 2020 3e3e 3e20  d").        >>> 
-0000f680: 7265 6769 6f6e 2e61 7070 656e 6428 6578  region.append(ex
-0000f690: 6365 6c32 786d 6c2e 6d61 6b65 5f74 6578  cel2xml.make_tex
-0000f6a0: 745f 7072 6f70 2822 6861 7343 6f6d 6d65  t_prop("hasComme
-0000f6b0: 6e74 222c 2022 5468 6973 2069 7320 6120  nt", "This is a 
-0000f6c0: 636f 6d6d 656e 7422 2929 0a20 2020 2020  comment")).     
-0000f6d0: 2020 203e 3e3e 2072 6567 696f 6e2e 6170     >>> region.ap
-0000f6e0: 7065 6e64 2865 7863 656c 3278 6d6c 2e6d  pend(excel2xml.m
-0000f6f0: 616b 655f 636f 6c6f 725f 7072 6f70 2822  ake_color_prop("
-0000f700: 6861 7343 6f6c 6f72 222c 2022 2335 6431  hasColor", "#5d1
-0000f710: 6631 6522 2929 0a20 2020 2020 2020 203e  f1e")).        >
-0000f720: 3e3e 2072 6567 696f 6e2e 6170 7065 6e64  >> region.append
-0000f730: 2865 7863 656c 3278 6d6c 2e6d 616b 655f  (excel2xml.make_
-0000f740: 7265 7370 7472 5f70 726f 7028 2269 7352  resptr_prop("isR
-0000f750: 6567 696f 6e4f 6622 2c20 2269 6d61 6765  egionOf", "image
-0000f760: 5f30 2229 290a 2020 2020 2020 2020 3e3e  _0")).        >>
-0000f770: 3e20 7265 6769 6f6e 2e61 7070 656e 6428  > region.append(
-0000f780: 6578 6365 6c32 786d 6c2e 6d61 6b65 5f67  excel2xml.make_g
-0000f790: 656f 6d65 7472 795f 7072 6f70 2822 6861  eometry_prop("ha
-0000f7a0: 7347 656f 6d65 7472 7922 2c20 227b 2e2e  sGeometry", "{..
-0000f7b0: 2e7d 2229 290a 2020 2020 2020 2020 3e3e  .}")).        >>
-0000f7c0: 3e20 726f 6f74 2e61 7070 656e 6428 7265  > root.append(re
-0000f7d0: 6769 6f6e 290a 0a20 2020 2053 6565 2068  gion)..    See h
-0000f7e0: 7474 7073 3a2f 2f64 6f63 732e 6461 7363  ttps://docs.dasc
-0000f7f0: 682e 7377 6973 732f 6c61 7465 7374 2f44  h.swiss/latest/D
-0000f800: 5350 2d54 4f4f 4c53 2f66 696c 652d 666f  SP-TOOLS/file-fo
-0000f810: 726d 6174 732f 786d 6c2d 6461 7461 2d66  rmats/xml-data-f
-0000f820: 696c 652f 2372 6567 696f 6e0a 2020 2020  ile/#region.    
-0000f830: 2222 220a 0a20 2020 206b 7761 7267 7320  """..    kwargs 
-0000f840: 3d20 7b22 6c61 6265 6c22 3a20 6c61 6265  = {"label": labe
-0000f850: 6c2c 2022 6964 223a 2069 642c 2022 7065  l, "id": id, "pe
-0000f860: 726d 6973 7369 6f6e 7322 3a20 7065 726d  rmissions": perm
-0000f870: 6973 7369 6f6e 732c 2022 6e73 6d61 7022  issions, "nsmap"
-0000f880: 3a20 786d 6c5f 6e61 6d65 7370 6163 655f  : xml_namespace_
-0000f890: 6d61 707d 0a20 2020 2069 6620 6172 6b3a  map}.    if ark:
-0000f8a0: 0a20 2020 2020 2020 206b 7761 7267 735b  .        kwargs[
-0000f8b0: 2261 726b 225d 203d 2061 726b 0a20 2020  "ark"] = ark.   
-0000f8c0: 2069 6620 6972 693a 0a20 2020 2020 2020   if iri:.       
-0000f8d0: 206b 7761 7267 735b 2269 7269 225d 203d   kwargs["iri"] =
-0000f8e0: 2069 7269 0a20 2020 2069 6620 6172 6b20   iri.    if ark 
-0000f8f0: 616e 6420 6972 693a 0a20 2020 2020 2020  and iri:.       
-0000f900: 206d 7367 203d 2066 2242 6f74 6820 4152   msg = f"Both AR
-0000f910: 4b20 616e 6420 4952 4920 7765 7265 2070  K and IRI were p
-0000f920: 726f 7669 6465 6420 666f 7220 7265 736f  rovided for reso
-0000f930: 7572 6365 2027 7b6c 6162 656c 7d27 2028  urce '{label}' (
-0000f940: 7b69 647d 292e 2054 6865 2041 524b 2077  {id}). The ARK w
-0000f950: 696c 6c20 6f76 6572 7269 6465 2074 6865  ill override the
-0000f960: 2049 5249 2e22 0a20 2020 2020 2020 2077   IRI.".        w
-0000f970: 6172 6e69 6e67 732e 7761 726e 2844 7370  arnings.warn(Dsp
-0000f980: 546f 6f6c 7355 7365 7257 6172 6e69 6e67  ToolsUserWarning
-0000f990: 286d 7367 2929 0a20 2020 2069 6620 6372  (msg)).    if cr
-0000f9a0: 6561 7469 6f6e 5f64 6174 653a 0a20 2020  eation_date:.   
-0000f9b0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-0000f9c0: 2020 2020 2020 4461 7465 5469 6d65 5374        DateTimeSt
-0000f9d0: 616d 7028 6372 6561 7469 6f6e 5f64 6174  amp(creation_dat
-0000f9e0: 6529 0a20 2020 2020 2020 2065 7863 6570  e).        excep
-0000f9f0: 7420 4261 7365 4572 726f 723a 0a20 2020  t BaseError:.   
-0000fa00: 2020 2020 2020 2020 2072 6169 7365 2042           raise B
-0000fa10: 6173 6545 7272 6f72 280a 2020 2020 2020  aseError(.      
-0000fa20: 2020 2020 2020 2020 2020 6622 5468 6520            f"The 
-0000fa30: 7265 6769 6f6e 2027 7b6c 6162 656c 7d27  region '{label}'
-0000fa40: 2028 4944 3a20 7b69 647d 2920 6861 7320   (ID: {id}) has 
-0000fa50: 616e 2069 6e76 616c 6964 2063 7265 6174  an invalid creat
-0000fa60: 696f 6e20 6461 7465 2027 7b63 7265 6174  ion date '{creat
-0000fa70: 696f 6e5f 6461 7465 7d27 2e20 220a 2020  ion_date}'. ".  
-0000fa80: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-0000fa90: 4469 6420 796f 7520 7065 7268 6170 7320  Did you perhaps 
-0000faa0: 666f 7267 6574 2074 6865 2074 696d 657a  forget the timez
-0000fab0: 6f6e 653f 220a 2020 2020 2020 2020 2020  one?".          
-0000fac0: 2020 2920 6672 6f6d 204e 6f6e 650a 2020    ) from None.  
-0000fad0: 2020 2020 2020 6b77 6172 6773 5b22 6372        kwargs["cr
-0000fae0: 6561 7469 6f6e 5f64 6174 6522 5d20 3d20  eation_date"] = 
-0000faf0: 6372 6561 7469 6f6e 5f64 6174 650a 0a20  creation_date.. 
-0000fb00: 2020 2072 6574 7572 6e20 6574 7265 652e     return etree.
-0000fb10: 456c 656d 656e 7428 0a20 2020 2020 2020  Element(.       
-0000fb20: 2022 7b25 737d 7265 6769 6f6e 2220 2520   "{%s}region" % 
-0000fb30: 786d 6c5f 6e61 6d65 7370 6163 655f 6d61  xml_namespace_ma
-0000fb40: 705b 4e6f 6e65 5d2c 0a20 2020 2020 2020  p[None],.       
-0000fb50: 202a 2a6b 7761 7267 732c 2020 2320 7479   **kwargs,  # ty
-0000fb60: 7065 3a20 6967 6e6f 7265 5b61 7267 2d74  pe: ignore[arg-t
-0000fb70: 7970 655d 0a20 2020 2029 0a0a 0a64 6566  ype].    )...def
-0000fb80: 206d 616b 655f 616e 6e6f 7461 7469 6f6e   make_annotation
-0000fb90: 2820 2023 206e 6f71 613a 2044 3431 3720  (  # noqa: D417 
-0000fba0: 2875 6e64 6f63 756d 656e 7465 642d 7061  (undocumented-pa
-0000fbb0: 7261 6d29 0a20 2020 206c 6162 656c 3a20  ram).    label: 
-0000fbc0: 7374 722c 0a20 2020 2069 643a 2073 7472  str,.    id: str
-0000fbd0: 2c0a 2020 2020 7065 726d 6973 7369 6f6e  ,.    permission
-0000fbe0: 733a 2073 7472 203d 2022 7265 732d 6465  s: str = "res-de
-0000fbf0: 6661 756c 7422 2c0a 2020 2020 6172 6b3a  fault",.    ark:
-0000fc00: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-0000fc10: 204e 6f6e 652c 0a20 2020 2069 7269 3a20   None,.    iri: 
-0000fc20: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-0000fc30: 4e6f 6e65 2c0a 2020 2020 6372 6561 7469  None,.    creati
-0000fc40: 6f6e 5f64 6174 653a 204f 7074 696f 6e61  on_date: Optiona
-0000fc50: 6c5b 7374 725d 203d 204e 6f6e 652c 0a29  l[str] = None,.)
-0000fc60: 202d 3e20 6574 7265 652e 5f45 6c65 6d65   -> etree._Eleme
-0000fc70: 6e74 3a0a 2020 2020 2222 220a 2020 2020  nt:.    """.    
-0000fc80: 4372 6561 7465 7320 616e 2065 6d70 7479  Creates an empty
-0000fc90: 2061 6e6e 6f74 6174 696f 6e20 656c 656d   annotation elem
-0000fca0: 656e 742c 2077 6974 6820 7468 6520 6174  ent, with the at
-0000fcb0: 7472 6962 7574 6573 2061 7320 7370 6563  tributes as spec
-0000fcc0: 6966 6965 6420 6279 2074 6865 2061 7267  ified by the arg
-0000fcd0: 756d 656e 7473 0a0a 2020 2020 4172 6773  uments..    Args
-0000fce0: 3a0a 2020 2020 2020 2020 5468 6520 6172  :.        The ar
-0000fcf0: 6775 6d65 6e74 7320 636f 7272 6573 706f  guments correspo
-0000fd00: 6e64 2031 3a31 2074 6f20 7468 6520 6174  nd 1:1 to the at
-0000fd10: 7472 6962 7574 6573 206f 6620 7468 6520  tributes of the 
-0000fd20: 3c61 6e6e 6f74 6174 696f 6e3e 2065 6c65  <annotation> ele
-0000fd30: 6d65 6e74 2e0a 0a20 2020 2052 6169 7365  ment...    Raise
-0000fd40: 733a 0a20 2020 2020 2020 2057 6172 6e69  s:.        Warni
-0000fd50: 6e67 3a20 6966 2062 6f74 6820 616e 2041  ng: if both an A
-0000fd60: 524b 2061 6e64 2061 6e20 4952 4920 6172  RK and an IRI ar
-0000fd70: 6520 7072 6f76 6964 6564 0a20 2020 2020  e provided.     
-0000fd80: 2020 2042 6173 6545 7272 6f72 3a20 6966     BaseError: if
-0000fd90: 2074 6865 2063 7265 6174 696f 6e20 6461   the creation da
-0000fda0: 7465 2069 7320 696e 7661 6c69 640a 0a20  te is invalid.. 
-0000fdb0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-0000fdc0: 2020 2020 5468 6520 616e 6e6f 7461 7469      The annotati
-0000fdd0: 6f6e 2065 6c65 6d65 6e74 2c20 7769 7468  on element, with
-0000fde0: 6f75 7420 616e 7920 6368 696c 6472 656e  out any children
-0000fdf0: 2c20 6275 7420 7769 7468 2074 6865 2061  , but with the a
-0000fe00: 7474 7269 6275 7465 733a 0a20 2020 2020  ttributes:.     
-0000fe10: 2020 203c 616e 6e6f 7461 7469 6f6e 206c     <annotation l
-0000fe20: 6162 656c 3d6c 6162 656c 2069 643d 6964  abel=label id=id
-0000fe30: 2070 6572 6d69 7373 696f 6e73 3d70 6572   permissions=per
-0000fe40: 6d69 7373 696f 6e73 2061 726b 3d61 726b  missions ark=ark
-0000fe50: 2069 7269 3d69 7269 3e3c 2f61 6e6e 6f74   iri=iri></annot
-0000fe60: 6174 696f 6e3e 0a0a 2020 2020 4578 616d  ation>..    Exam
-0000fe70: 706c 6573 3a0a 2020 2020 2020 2020 3e3e  ples:.        >>
-0000fe80: 3e20 616e 6e6f 7461 7469 6f6e 203d 2065  > annotation = e
-0000fe90: 7863 656c 3278 6d6c 2e6d 616b 655f 616e  xcel2xml.make_an
-0000fea0: 6e6f 7461 7469 6f6e 2822 6c61 6265 6c22  notation("label"
-0000feb0: 2c20 2269 6422 290a 2020 2020 2020 2020  , "id").        
-0000fec0: 3e3e 3e20 616e 6e6f 7461 7469 6f6e 2e61  >>> annotation.a
-0000fed0: 7070 656e 6428 6578 6365 6c32 786d 6c2e  ppend(excel2xml.
-0000fee0: 6d61 6b65 5f74 6578 745f 7072 6f70 2822  make_text_prop("
-0000fef0: 6861 7343 6f6d 6d65 6e74 222c 2022 5468  hasComment", "Th
-0000ff00: 6973 2069 7320 6120 636f 6d6d 656e 7422  is is a comment"
-0000ff10: 2929 0a20 2020 2020 2020 203e 3e3e 2061  )).        >>> a
-0000ff20: 6e6e 6f74 6174 696f 6e2e 6170 7065 6e64  nnotation.append
-0000ff30: 2865 7863 656c 3278 6d6c 2e6d 616b 655f  (excel2xml.make_
-0000ff40: 7265 7370 7472 5f70 726f 7028 2269 7341  resptr_prop("isA
-0000ff50: 6e6e 6f74 6174 696f 6e4f 6622 2c20 2272  nnotationOf", "r
-0000ff60: 6573 6f75 7263 655f 3022 2929 0a20 2020  esource_0")).   
-0000ff70: 2020 2020 203e 3e3e 2072 6f6f 742e 6170       >>> root.ap
-0000ff80: 7065 6e64 2861 6e6e 6f74 6174 696f 6e29  pend(annotation)
-0000ff90: 0a0a 2020 2020 5365 6520 6874 7470 733a  ..    See https:
-0000ffa0: 2f2f 646f 6373 2e64 6173 6368 2e73 7769  //docs.dasch.swi
-0000ffb0: 7373 2f6c 6174 6573 742f 4453 502d 544f  ss/latest/DSP-TO
-0000ffc0: 4f4c 532f 6669 6c65 2d66 6f72 6d61 7473  OLS/file-formats
-0000ffd0: 2f78 6d6c 2d64 6174 612d 6669 6c65 2f23  /xml-data-file/#
-0000ffe0: 616e 6e6f 7461 7469 6f6e 0a20 2020 2022  annotation.    "
-0000fff0: 2222 0a0a 2020 2020 6b77 6172 6773 203d  ""..    kwargs =
-00010000: 207b 226c 6162 656c 223a 206c 6162 656c   {"label": label
-00010010: 2c20 2269 6422 3a20 6964 2c20 2270 6572  , "id": id, "per
-00010020: 6d69 7373 696f 6e73 223a 2070 6572 6d69  missions": permi
-00010030: 7373 696f 6e73 2c20 226e 736d 6170 223a  ssions, "nsmap":
-00010040: 2078 6d6c 5f6e 616d 6573 7061 6365 5f6d   xml_namespace_m
-00010050: 6170 7d0a 2020 2020 6966 2061 726b 3a0a  ap}.    if ark:.
-00010060: 2020 2020 2020 2020 6b77 6172 6773 5b22          kwargs["
-00010070: 6172 6b22 5d20 3d20 6172 6b0a 2020 2020  ark"] = ark.    
-00010080: 6966 2069 7269 3a0a 2020 2020 2020 2020  if iri:.        
-00010090: 6b77 6172 6773 5b22 6972 6922 5d20 3d20  kwargs["iri"] = 
-000100a0: 6972 690a 2020 2020 6966 2061 726b 2061  iri.    if ark a
-000100b0: 6e64 2069 7269 3a0a 2020 2020 2020 2020  nd iri:.        
-000100c0: 7761 726e 696e 6720 3d20 6622 426f 7468  warning = f"Both
-000100d0: 2041 524b 2061 6e64 2049 5249 2077 6572   ARK and IRI wer
-000100e0: 6520 7072 6f76 6964 6564 2066 6f72 2072  e provided for r
-000100f0: 6573 6f75 7263 6520 277b 6c61 6265 6c7d  esource '{label}
-00010100: 2720 287b 6964 7d29 2e20 5468 6520 4152  ' ({id}). The AR
-00010110: 4b20 7769 6c6c 206f 7665 7272 6964 6520  K will override 
-00010120: 7468 6520 4952 492e 220a 2020 2020 2020  the IRI.".      
-00010130: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
-00010140: 4473 7054 6f6f 6c73 5573 6572 5761 726e  DspToolsUserWarn
-00010150: 696e 6728 7761 726e 696e 6729 290a 2020  ing(warning)).  
-00010160: 2020 6966 2063 7265 6174 696f 6e5f 6461    if creation_da
-00010170: 7465 3a0a 2020 2020 2020 2020 7472 793a  te:.        try:
-00010180: 0a20 2020 2020 2020 2020 2020 2044 6174  .            Dat
-00010190: 6554 696d 6553 7461 6d70 2863 7265 6174  eTimeStamp(creat
-000101a0: 696f 6e5f 6461 7465 290a 2020 2020 2020  ion_date).      
-000101b0: 2020 6578 6365 7074 2042 6173 6545 7272    except BaseErr
-000101c0: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
-000101d0: 7261 6973 6520 4261 7365 4572 726f 7228  raise BaseError(
-000101e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000101f0: 2066 2254 6865 2061 6e6e 6f74 6174 696f   f"The annotatio
-00010200: 6e20 277b 6c61 6265 6c7d 2720 2849 443a  n '{label}' (ID:
-00010210: 207b 6964 7d29 2068 6173 2061 6e20 696e   {id}) has an in
-00010220: 7661 6c69 6420 6372 6561 7469 6f6e 2064  valid creation d
-00010230: 6174 6520 277b 6372 6561 7469 6f6e 5f64  ate '{creation_d
-00010240: 6174 657d 272e 2022 0a20 2020 2020 2020  ate}'. ".       
-00010250: 2020 2020 2020 2020 2066 2244 6964 2079           f"Did y
-00010260: 6f75 2070 6572 6861 7073 2066 6f72 6765  ou perhaps forge
-00010270: 7420 7468 6520 7469 6d65 7a6f 6e65 3f22  t the timezone?"
-00010280: 0a20 2020 2020 2020 2020 2020 2029 2066  .            ) f
-00010290: 726f 6d20 4e6f 6e65 0a20 2020 2020 2020  rom None.       
-000102a0: 206b 7761 7267 735b 2263 7265 6174 696f   kwargs["creatio
-000102b0: 6e5f 6461 7465 225d 203d 2063 7265 6174  n_date"] = creat
-000102c0: 696f 6e5f 6461 7465 0a0a 2020 2020 7265  ion_date..    re
-000102d0: 7475 726e 2065 7472 6565 2e45 6c65 6d65  turn etree.Eleme
-000102e0: 6e74 280a 2020 2020 2020 2020 227b 2573  nt(.        "{%s
-000102f0: 7d61 6e6e 6f74 6174 696f 6e22 2025 2078  }annotation" % x
-00010300: 6d6c 5f6e 616d 6573 7061 6365 5f6d 6170  ml_namespace_map
-00010310: 5b4e 6f6e 655d 2c0a 2020 2020 2020 2020  [None],.        
-00010320: 2a2a 6b77 6172 6773 2c20 2023 2074 7970  **kwargs,  # typ
-00010330: 653a 2069 676e 6f72 655b 6172 672d 7479  e: ignore[arg-ty
-00010340: 7065 5d0a 2020 2020 290a 0a0a 6465 6620  pe].    )...def 
-00010350: 6d61 6b65 5f6c 696e 6b28 2020 2320 6e6f  make_link(  # no
-00010360: 7161 3a20 4434 3137 2028 756e 646f 6375  qa: D417 (undocu
-00010370: 6d65 6e74 6564 2d70 6172 616d 290a 2020  mented-param).  
-00010380: 2020 6c61 6265 6c3a 2073 7472 2c0a 2020    label: str,.  
-00010390: 2020 6964 3a20 7374 722c 0a20 2020 2070    id: str,.    p
-000103a0: 6572 6d69 7373 696f 6e73 3a20 7374 7220  ermissions: str 
-000103b0: 3d20 2272 6573 2d64 6566 6175 6c74 222c  = "res-default",
-000103c0: 0a20 2020 2061 726b 3a20 4f70 7469 6f6e  .    ark: Option
-000103d0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
-000103e0: 2020 2020 6972 693a 204f 7074 696f 6e61      iri: Optiona
-000103f0: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
-00010400: 2020 2063 7265 6174 696f 6e5f 6461 7465     creation_date
-00010410: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-00010420: 3d20 4e6f 6e65 2c0a 2920 2d3e 2065 7472  = None,.) -> etr
-00010430: 6565 2e5f 456c 656d 656e 743a 0a20 2020  ee._Element:.   
-00010440: 2022 2222 0a20 2020 2043 7265 6174 6573   """.    Creates
-00010450: 2061 6e20 656d 7074 7920 6c69 6e6b 2065   an empty link e
-00010460: 6c65 6d65 6e74 2c20 7769 7468 2074 6865  lement, with the
-00010470: 2061 7474 7269 6275 7465 7320 6173 2073   attributes as s
-00010480: 7065 6369 6669 6564 2062 7920 7468 6520  pecified by the 
-00010490: 6172 6775 6d65 6e74 730a 0a20 2020 2041  arguments..    A
-000104a0: 7267 733a 0a20 2020 2020 2020 2054 6865  rgs:.        The
-000104b0: 2061 7267 756d 656e 7473 2063 6f72 7265   arguments corre
-000104c0: 7370 6f6e 6420 313a 3120 746f 2074 6865  spond 1:1 to the
-000104d0: 2061 7474 7269 6275 7465 7320 6f66 2074   attributes of t
-000104e0: 6865 203c 6c69 6e6b 3e20 656c 656d 656e  he <link> elemen
-000104f0: 742e 0a0a 2020 2020 5261 6973 6573 3a0a  t...    Raises:.
-00010500: 2020 2020 2020 2020 5761 726e 696e 673a          Warning:
-00010510: 2069 6620 626f 7468 2061 6e20 4152 4b20   if both an ARK 
-00010520: 616e 6420 616e 2049 5249 2061 7265 2070  and an IRI are p
-00010530: 726f 7669 6465 640a 2020 2020 2020 2020  rovided.        
-00010540: 4261 7365 4572 726f 723a 2069 6620 7468  BaseError: if th
-00010550: 6520 6372 6561 7469 6f6e 2064 6174 6520  e creation date 
-00010560: 6973 2069 6e76 616c 6964 0a0a 2020 2020  is invalid..    
-00010570: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00010580: 2054 6865 206c 696e 6b20 656c 656d 656e   The link elemen
-00010590: 742c 2077 6974 686f 7574 2061 6e79 2063  t, without any c
-000105a0: 6869 6c64 7265 6e2c 2062 7574 2077 6974  hildren, but wit
-000105b0: 6820 7468 6520 6174 7472 6962 7574 6573  h the attributes
-000105c0: 3a0a 2020 2020 2020 2020 3c6c 696e 6b20  :.        <link 
-000105d0: 6c61 6265 6c3d 6c61 6265 6c20 6964 3d69  label=label id=i
-000105e0: 6420 7065 726d 6973 7369 6f6e 733d 7065  d permissions=pe
-000105f0: 726d 6973 7369 6f6e 7320 6172 6b3d 6172  rmissions ark=ar
-00010600: 6b20 6972 693d 6972 693e 3c2f 6c69 6e6b  k iri=iri></link
-00010610: 3e0a 0a20 2020 2045 7861 6d70 6c65 733a  >..    Examples:
-00010620: 0a20 2020 2020 2020 203e 3e3e 206c 696e  .        >>> lin
-00010630: 6b20 3d20 6578 6365 6c32 786d 6c2e 6d61  k = excel2xml.ma
-00010640: 6b65 5f6c 696e 6b28 226c 6162 656c 222c  ke_link("label",
-00010650: 2022 6964 2229 0a20 2020 2020 2020 203e   "id").        >
-00010660: 3e3e 206c 696e 6b2e 6170 7065 6e64 2865  >> link.append(e
-00010670: 7863 656c 3278 6d6c 2e6d 616b 655f 7465  xcel2xml.make_te
-00010680: 7874 5f70 726f 7028 2268 6173 436f 6d6d  xt_prop("hasComm
-00010690: 656e 7422 2c20 2254 6869 7320 6973 2061  ent", "This is a
-000106a0: 2063 6f6d 6d65 6e74 2229 290a 2020 2020   comment")).    
-000106b0: 2020 2020 3e3e 3e20 6c69 6e6b 2e61 7070      >>> link.app
-000106c0: 656e 6428 6578 6365 6c32 786d 6c2e 6d61  end(excel2xml.ma
-000106d0: 6b65 5f72 6573 7074 725f 7072 6f70 2822  ke_resptr_prop("
-000106e0: 6861 734c 696e 6b54 6f22 2c20 5b22 7265  hasLinkTo", ["re
-000106f0: 736f 7572 6365 5f30 222c 2022 7265 736f  source_0", "reso
-00010700: 7572 6365 5f31 225d 2929 0a20 2020 2020  urce_1"])).     
-00010710: 2020 203e 3e3e 2072 6f6f 742e 6170 7065     >>> root.appe
-00010720: 6e64 286c 696e 6b29 0a0a 2020 2020 5365  nd(link)..    Se
-00010730: 6520 6874 7470 733a 2f2f 646f 6373 2e64  e https://docs.d
-00010740: 6173 6368 2e73 7769 7373 2f6c 6174 6573  asch.swiss/lates
-00010750: 742f 4453 502d 544f 4f4c 532f 6669 6c65  t/DSP-TOOLS/file
-00010760: 2d66 6f72 6d61 7473 2f78 6d6c 2d64 6174  -formats/xml-dat
-00010770: 612d 6669 6c65 2f23 6c69 6e6b 0a20 2020  a-file/#link.   
-00010780: 2022 2222 0a0a 2020 2020 6b77 6172 6773   """..    kwargs
-00010790: 203d 207b 226c 6162 656c 223a 206c 6162   = {"label": lab
-000107a0: 656c 2c20 2269 6422 3a20 6964 2c20 2270  el, "id": id, "p
-000107b0: 6572 6d69 7373 696f 6e73 223a 2070 6572  ermissions": per
-000107c0: 6d69 7373 696f 6e73 2c20 226e 736d 6170  missions, "nsmap
-000107d0: 223a 2078 6d6c 5f6e 616d 6573 7061 6365  ": xml_namespace
-000107e0: 5f6d 6170 7d0a 2020 2020 6966 2061 726b  _map}.    if ark
-000107f0: 3a0a 2020 2020 2020 2020 6b77 6172 6773  :.        kwargs
-00010800: 5b22 6172 6b22 5d20 3d20 6172 6b0a 2020  ["ark"] = ark.  
-00010810: 2020 6966 2069 7269 3a0a 2020 2020 2020    if iri:.      
-00010820: 2020 6b77 6172 6773 5b22 6972 6922 5d20    kwargs["iri"] 
-00010830: 3d20 6972 690a 2020 2020 6966 2061 726b  = iri.    if ark
-00010840: 2061 6e64 2069 7269 3a0a 2020 2020 2020   and iri:.      
-00010850: 2020 6d73 6720 3d20 6622 426f 7468 2041    msg = f"Both A
-00010860: 524b 2061 6e64 2049 5249 2077 6572 6520  RK and IRI were 
-00010870: 7072 6f76 6964 6564 2066 6f72 2072 6573  provided for res
-00010880: 6f75 7263 6520 277b 6c61 6265 6c7d 2720  ource '{label}' 
-00010890: 287b 6964 7d29 2e20 5468 6520 4152 4b20  ({id}). The ARK 
-000108a0: 7769 6c6c 206f 7665 7272 6964 6520 7468  will override th
-000108b0: 6520 4952 492e 220a 2020 2020 2020 2020  e IRI.".        
-000108c0: 7761 726e 696e 6773 2e77 6172 6e28 4473  warnings.warn(Ds
-000108d0: 7054 6f6f 6c73 5573 6572 5761 726e 696e  pToolsUserWarnin
-000108e0: 6728 6d73 6729 290a 2020 2020 6966 2063  g(msg)).    if c
-000108f0: 7265 6174 696f 6e5f 6461 7465 3a0a 2020  reation_date:.  
-00010900: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00010910: 2020 2020 2020 2044 6174 6554 696d 6553         DateTimeS
-00010920: 7461 6d70 2863 7265 6174 696f 6e5f 6461  tamp(creation_da
-00010930: 7465 290a 2020 2020 2020 2020 6578 6365  te).        exce
-00010940: 7074 2042 6173 6545 7272 6f72 3a0a 2020  pt BaseError:.  
-00010950: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00010960: 4261 7365 4572 726f 7228 0a20 2020 2020  BaseError(.     
-00010970: 2020 2020 2020 2020 2020 2066 2254 6865             f"The
-00010980: 206c 696e 6b20 277b 6c61 6265 6c7d 2720   link '{label}' 
-00010990: 2849 443a 207b 6964 7d29 2068 6173 2061  (ID: {id}) has a
-000109a0: 6e20 696e 7661 6c69 6420 6372 6561 7469  n invalid creati
-000109b0: 6f6e 2064 6174 6520 277b 6372 6561 7469  on date '{creati
-000109c0: 6f6e 5f64 6174 657d 272e 2022 0a20 2020  on_date}'. ".   
-000109d0: 2020 2020 2020 2020 2020 2020 2066 2244               f"D
-000109e0: 6964 2079 6f75 2070 6572 6861 7073 2066  id you perhaps f
-000109f0: 6f72 6765 7420 7468 6520 7469 6d65 7a6f  orget the timezo
-00010a00: 6e65 3f22 0a20 2020 2020 2020 2020 2020  ne?".           
-00010a10: 2029 2066 726f 6d20 4e6f 6e65 0a20 2020   ) from None.   
-00010a20: 2020 2020 206b 7761 7267 735b 2263 7265       kwargs["cre
-00010a30: 6174 696f 6e5f 6461 7465 225d 203d 2063  ation_date"] = c
-00010a40: 7265 6174 696f 6e5f 6461 7465 0a0a 2020  reation_date..  
-00010a50: 2020 7265 7475 726e 2065 7472 6565 2e45    return etree.E
-00010a60: 6c65 6d65 6e74 280a 2020 2020 2020 2020  lement(.        
-00010a70: 227b 2573 7d6c 696e 6b22 2025 2078 6d6c  "{%s}link" % xml
-00010a80: 5f6e 616d 6573 7061 6365 5f6d 6170 5b4e  _namespace_map[N
-00010a90: 6f6e 655d 2c0a 2020 2020 2020 2020 2a2a  one],.        **
-00010aa0: 6b77 6172 6773 2c20 2023 2074 7970 653a  kwargs,  # type:
-00010ab0: 2069 676e 6f72 655b 6172 672d 7479 7065   ignore[arg-type
-00010ac0: 5d0a 2020 2020 290a 0a0a 6465 6620 6d61  ].    )...def ma
-00010ad0: 6b65 5f61 7564 696f 5f73 6567 6d65 6e74  ke_audio_segment
-00010ae0: 2820 2023 206e 6f71 613a 2044 3431 3720  (  # noqa: D417 
-00010af0: 2875 6e64 6f63 756d 656e 7465 642d 7061  (undocumented-pa
-00010b00: 7261 6d29 0a20 2020 206c 6162 656c 3a20  ram).    label: 
-00010b10: 7374 722c 0a20 2020 2069 643a 2073 7472  str,.    id: str
-00010b20: 2c0a 2020 2020 7065 726d 6973 7369 6f6e  ,.    permission
-00010b30: 733a 2073 7472 203d 2022 7265 732d 6465  s: str = "res-de
-00010b40: 6661 756c 7422 2c0a 2920 2d3e 2065 7472  fault",.) -> etr
-00010b50: 6565 2e5f 456c 656d 656e 743a 0a20 2020  ee._Element:.   
-00010b60: 2022 2222 0a20 2020 2043 7265 6174 6573   """.    Creates
-00010b70: 2061 6e20 656d 7074 7920 3c61 7564 696f   an empty <audio
-00010b80: 2d73 6567 6d65 6e74 3e20 656c 656d 656e  -segment> elemen
-00010b90: 742c 2077 6974 6820 7468 6520 6174 7472  t, with the attr
-00010ba0: 6962 7574 6573 2061 7320 7370 6563 6966  ibutes as specif
-00010bb0: 6965 6420 6279 2074 6865 2061 7267 756d  ied by the argum
-00010bc0: 656e 7473 0a0a 2020 2020 4172 6773 3a0a  ents..    Args:.
-00010bd0: 2020 2020 2020 2020 5468 6520 6172 6775          The argu
-00010be0: 6d65 6e74 7320 636f 7272 6573 706f 6e64  ments correspond
-00010bf0: 2031 3a31 2074 6f20 7468 6520 6174 7472   1:1 to the attr
-00010c00: 6962 7574 6573 206f 6620 7468 6520 3c61  ibutes of the <a
-00010c10: 7564 696f 2d73 6567 6d65 6e74 3e20 656c  udio-segment> el
-00010c20: 656d 656e 742e 0a0a 2020 2020 5265 7475  ement...    Retu
-00010c30: 726e 733a 0a20 2020 2020 2020 2054 6865  rns:.        The
-00010c40: 2061 7564 696f 2d73 6567 6d65 6e74 2065   audio-segment e
-00010c50: 6c65 6d65 6e74 2c20 7769 7468 6f75 7420  lement, without 
-00010c60: 616e 7920 6368 696c 6472 656e 2c20 6275  any children, bu
-00010c70: 7420 7769 7468 2074 6865 2061 7474 7269  t with the attri
-00010c80: 6275 7465 733a 0a20 2020 2020 2020 203c  butes:.        <
-00010c90: 6175 6469 6f2d 7365 676d 656e 7420 6c61  audio-segment la
-00010ca0: 6265 6c3d 6c61 6265 6c20 6964 3d69 6420  bel=label id=id 
-00010cb0: 7065 726d 6973 7369 6f6e 733d 7065 726d  permissions=perm
-00010cc0: 6973 7369 6f6e 733e 3c2f 6175 6469 6f2d  issions></audio-
-00010cd0: 7365 676d 656e 743e 0a0a 2020 2020 4578  segment>..    Ex
-00010ce0: 616d 706c 6573 3a0a 2020 2020 2020 2020  amples:.        
-00010cf0: 3e3e 3e20 6175 6469 6f5f 7365 676d 656e  >>> audio_segmen
-00010d00: 7420 3d20 6578 6365 6c32 786d 6c2e 6d61  t = excel2xml.ma
-00010d10: 6b65 5f61 7564 696f 5f73 6567 6d65 6e74  ke_audio_segment
-00010d20: 2822 6c61 6265 6c22 2c20 2269 6422 290a  ("label", "id").
-00010d30: 2020 2020 2020 2020 3e3e 3e20 6175 6469          >>> audi
-00010d40: 6f5f 7365 676d 656e 742e 6170 7065 6e64  o_segment.append
-00010d50: 2865 7863 656c 3278 6d6c 2e6d 616b 655f  (excel2xml.make_
-00010d60: 7265 7370 7472 5f70 726f 7028 2269 7353  resptr_prop("isS
-00010d70: 6567 6d65 6e74 4f66 222c 2022 6175 6469  egmentOf", "audi
-00010d80: 6f5f 7265 736f 7572 6365 5f69 6422 2929  o_resource_id"))
-00010d90: 0a20 2020 2020 2020 203e 3e3e 2061 7564  .        >>> aud
-00010da0: 696f 5f73 6567 6d65 6e74 2e61 7070 656e  io_segment.appen
-00010db0: 6428 6578 6365 6c32 786d 6c2e 6d61 6b65  d(excel2xml.make
-00010dc0: 5f69 6e74 6572 7661 6c5f 7072 6f70 2822  _interval_prop("
-00010dd0: 6861 7353 6567 6d65 6e74 426f 756e 6473  hasSegmentBounds
-00010de0: 222c 2022 3630 3a31 3230 2229 0a20 2020  ", "60:120").   
-00010df0: 2020 2020 203e 3e3e 2072 6f6f 742e 6170       >>> root.ap
-00010e00: 7065 6e64 2861 7564 696f 5f73 6567 6d65  pend(audio_segme
-00010e10: 6e74 290a 0a20 2020 2053 6565 2068 7474  nt)..    See htt
-00010e20: 7073 3a2f 2f64 6f63 732e 6461 7363 682e  ps://docs.dasch.
-00010e30: 7377 6973 732f 6c61 7465 7374 2f44 5350  swiss/latest/DSP
-00010e40: 2d54 4f4f 4c53 2f66 696c 652d 666f 726d  -TOOLS/file-form
-00010e50: 6174 732f 786d 6c2d 6461 7461 2d66 696c  ats/xml-data-fil
-00010e60: 652f 2376 6964 656f 2d73 6567 6d65 6e74  e/#video-segment
-00010e70: 2d61 7564 696f 2d73 6567 6d65 6e74 0a20  -audio-segment. 
-00010e80: 2020 2022 2222 0a20 2020 2072 6574 7572     """.    retur
-00010e90: 6e20 6574 7265 652e 456c 656d 656e 7428  n etree.Element(
-00010ea0: 0a20 2020 2020 2020 2022 7b25 737d 6175  .        "{%s}au
-00010eb0: 6469 6f2d 7365 676d 656e 7422 2025 2078  dio-segment" % x
-00010ec0: 6d6c 5f6e 616d 6573 7061 6365 5f6d 6170  ml_namespace_map
-00010ed0: 5b4e 6f6e 655d 2c0a 2020 2020 2020 2020  [None],.        
-00010ee0: 6c61 6265 6c3d 6c61 6265 6c2c 0a20 2020  label=label,.   
-00010ef0: 2020 2020 2069 643d 6964 2c0a 2020 2020       id=id,.    
-00010f00: 2020 2020 7065 726d 6973 7369 6f6e 733d      permissions=
-00010f10: 7065 726d 6973 7369 6f6e 732c 0a20 2020  permissions,.   
-00010f20: 2020 2020 206e 736d 6170 3d78 6d6c 5f6e       nsmap=xml_n
-00010f30: 616d 6573 7061 6365 5f6d 6170 2c0a 2020  amespace_map,.  
-00010f40: 2020 290a 0a0a 6465 6620 6d61 6b65 5f76    )...def make_v
-00010f50: 6964 656f 5f73 6567 6d65 6e74 2820 2023  ideo_segment(  #
-00010f60: 206e 6f71 613a 2044 3431 3720 2875 6e64   noqa: D417 (und
-00010f70: 6f63 756d 656e 7465 642d 7061 7261 6d29  ocumented-param)
-00010f80: 0a20 2020 206c 6162 656c 3a20 7374 722c  .    label: str,
-00010f90: 0a20 2020 2069 643a 2073 7472 2c0a 2020  .    id: str,.  
-00010fa0: 2020 7065 726d 6973 7369 6f6e 733a 2073    permissions: s
-00010fb0: 7472 203d 2022 7265 732d 6465 6661 756c  tr = "res-defaul
-00010fc0: 7422 2c0a 2920 2d3e 2065 7472 6565 2e5f  t",.) -> etree._
-00010fd0: 456c 656d 656e 743a 0a20 2020 2022 2222  Element:.    """
-00010fe0: 0a20 2020 2043 7265 6174 6573 2061 6e20  .    Creates an 
-00010ff0: 656d 7074 7920 3c76 6964 656f 2d73 6567  empty <video-seg
-00011000: 6d65 6e74 3e20 656c 656d 656e 742c 2077  ment> element, w
-00011010: 6974 6820 7468 6520 6174 7472 6962 7574  ith the attribut
-00011020: 6573 2061 7320 7370 6563 6966 6965 6420  es as specified 
-00011030: 6279 2074 6865 2061 7267 756d 656e 7473  by the arguments
-00011040: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
-00011050: 2020 2020 5468 6520 6172 6775 6d65 6e74      The argument
-00011060: 7320 636f 7272 6573 706f 6e64 2031 3a31  s correspond 1:1
-00011070: 2074 6f20 7468 6520 6174 7472 6962 7574   to the attribut
-00011080: 6573 206f 6620 7468 6520 3c76 6964 656f  es of the <video
-00011090: 2d73 6567 6d65 6e74 3e20 656c 656d 656e  -segment> elemen
-000110a0: 742e 0a0a 2020 2020 5265 7475 726e 733a  t...    Returns:
-000110b0: 0a20 2020 2020 2020 2054 6865 2076 6964  .        The vid
-000110c0: 656f 2d73 6567 6d65 6e74 2065 6c65 6d65  eo-segment eleme
-000110d0: 6e74 2c20 7769 7468 6f75 7420 616e 7920  nt, without any 
-000110e0: 6368 696c 6472 656e 2c20 6275 7420 7769  children, but wi
-000110f0: 7468 2074 6865 2061 7474 7269 6275 7465  th the attribute
-00011100: 733a 0a20 2020 2020 2020 203c 7669 6465  s:.        <vide
-00011110: 6f2d 7365 676d 656e 7420 6c61 6265 6c3d  o-segment label=
-00011120: 6c61 6265 6c20 6964 3d69 6420 7065 726d  label id=id perm
-00011130: 6973 7369 6f6e 733d 7065 726d 6973 7369  issions=permissi
-00011140: 6f6e 733e 3c2f 7669 6465 6f2d 7365 676d  ons></video-segm
-00011150: 656e 743e 0a0a 2020 2020 4578 616d 706c  ent>..    Exampl
-00011160: 6573 3a0a 2020 2020 2020 2020 3e3e 3e20  es:.        >>> 
-00011170: 7669 6465 6f5f 7365 676d 656e 7420 3d20  video_segment = 
-00011180: 6578 6365 6c32 786d 6c2e 6d61 6b65 5f76  excel2xml.make_v
-00011190: 6964 656f 5f73 6567 6d65 6e74 2822 6c61  ideo_segment("la
-000111a0: 6265 6c22 2c20 2269 6422 290a 2020 2020  bel", "id").    
-000111b0: 2020 2020 3e3e 3e20 7669 6465 6f5f 7365      >>> video_se
-000111c0: 676d 656e 742e 6170 7065 6e64 2865 7863  gment.append(exc
-000111d0: 656c 3278 6d6c 2e6d 616b 655f 7265 7370  el2xml.make_resp
-000111e0: 7472 5f70 726f 7028 2269 7353 6567 6d65  tr_prop("isSegme
-000111f0: 6e74 4f66 222c 2022 7669 6465 6f5f 7265  ntOf", "video_re
-00011200: 736f 7572 6365 5f69 6422 2929 0a20 2020  source_id")).   
-00011210: 2020 2020 203e 3e3e 2076 6964 656f 5f73       >>> video_s
-00011220: 6567 6d65 6e74 2e61 7070 656e 6428 6578  egment.append(ex
-00011230: 6365 6c32 786d 6c2e 6d61 6b65 5f69 6e74  cel2xml.make_int
-00011240: 6572 7661 6c5f 7072 6f70 2822 6861 7353  erval_prop("hasS
-00011250: 6567 6d65 6e74 426f 756e 6473 222c 2022  egmentBounds", "
-00011260: 3630 3a31 3230 2229 0a20 2020 2020 2020  60:120").       
-00011270: 203e 3e3e 2072 6f6f 742e 6170 7065 6e64   >>> root.append
-00011280: 2876 6964 656f 5f73 6567 6d65 6e74 290a  (video_segment).
-00011290: 0a20 2020 2053 6565 2068 7474 7073 3a2f  .    See https:/
-000112a0: 2f64 6f63 732e 6461 7363 682e 7377 6973  /docs.dasch.swis
-000112b0: 732f 6c61 7465 7374 2f44 5350 2d54 4f4f  s/latest/DSP-TOO
-000112c0: 4c53 2f66 696c 652d 666f 726d 6174 732f  LS/file-formats/
-000112d0: 786d 6c2d 6461 7461 2d66 696c 652f 2376  xml-data-file/#v
-000112e0: 6964 656f 2d73 6567 6d65 6e74 2d61 7564  ideo-segment-aud
-000112f0: 696f 2d73 6567 6d65 6e74 0a20 2020 2022  io-segment.    "
-00011300: 2222 0a20 2020 2072 6574 7572 6e20 6574  "".    return et
-00011310: 7265 652e 456c 656d 656e 7428 0a20 2020  ree.Element(.   
-00011320: 2020 2020 2022 7b25 737d 7669 6465 6f2d       "{%s}video-
-00011330: 7365 676d 656e 7422 2025 2078 6d6c 5f6e  segment" % xml_n
-00011340: 616d 6573 7061 6365 5f6d 6170 5b4e 6f6e  amespace_map[Non
-00011350: 655d 2c0a 2020 2020 2020 2020 6c61 6265  e],.        labe
-00011360: 6c3d 6c61 6265 6c2c 0a20 2020 2020 2020  l=label,.       
-00011370: 2069 643d 6964 2c0a 2020 2020 2020 2020   id=id,.        
-00011380: 7065 726d 6973 7369 6f6e 733d 7065 726d  permissions=perm
-00011390: 6973 7369 6f6e 732c 0a20 2020 2020 2020  issions,.       
-000113a0: 206e 736d 6170 3d78 6d6c 5f6e 616d 6573   nsmap=xml_names
-000113b0: 7061 6365 5f6d 6170 2c0a 2020 2020 290a  pace_map,.    ).
-000113c0: 0a0a 6465 6620 6372 6561 7465 5f69 6e74  ..def create_int
-000113d0: 6572 7661 6c5f 7661 6c75 6528 7374 6172  erval_value(star
-000113e0: 743a 2073 7472 2c20 656e 643a 2073 7472  t: str, end: str
-000113f0: 2920 2d3e 2073 7472 3a0a 2020 2020 2222  ) -> str:.    ""
-00011400: 220a 2020 2020 5472 616e 7366 6f72 6d20  ".    Transform 
-00011410: 6120 7374 6172 7420 616e 6420 656e 6420  a start and end 
-00011420: 7469 6d65 2069 6e74 6f20 6120 7661 6c69  time into a vali
-00011430: 6420 4453 5020 696e 7465 7276 616c 2076  d DSP interval v
-00011440: 616c 7565 2c0a 2020 2020 7768 6963 6820  alue,.    which 
-00011450: 7468 656e 2063 616e 2062 6520 7573 6564  then can be used
-00011460: 2069 6e20 616e 203c 696e 7465 7276 616c   in an <interval
-00011470: 206e 616d 653d 2268 6173 5365 676d 656e   name="hasSegmen
-00011480: 7442 6f75 6e64 7322 3e20 7461 672c 0a20  tBounds"> tag,. 
-00011490: 2020 2077 6869 6368 2069 7320 7573 6564     which is used
-000114a0: 2069 6e20 3c61 7564 696f 2d73 6567 6d65   in <audio-segme
-000114b0: 6e74 3e20 616e 6420 3c76 6964 656f 2d73  nt> and <video-s
-000114c0: 6567 6d65 6e74 3e20 656c 656d 656e 7473  egment> elements
-000114d0: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-000114e0: 2020 2020 2073 7461 7274 3a20 7374 6172       start: star
-000114f0: 7420 7469 6d65 206f 6620 7468 6520 7669  t time of the vi
-00011500: 6465 6f2f 6175 6469 6f20 7365 676d 656e  deo/audio segmen
-00011510: 742c 2069 6e20 7468 6520 666f 726d 6174  t, in the format
-00011520: 2027 4828 4829 3a4d 4d3a 5353 282e 7329   'H(H):MM:SS(.s)
-00011530: 270a 2020 2020 2020 2020 656e 643a 2065  '.        end: e
-00011540: 6e64 2074 696d 6520 6f66 2074 6865 2076  nd time of the v
-00011550: 6964 656f 2f61 7564 696f 2073 6567 6d65  ideo/audio segme
-00011560: 6e74 2c20 696e 2074 6865 2066 6f72 6d61  nt, in the forma
-00011570: 7420 2748 2848 293a 4d4d 3a53 5328 2e73  t 'H(H):MM:SS(.s
-00011580: 2927 0a0a 2020 2020 5261 6973 6573 3a0a  )'..    Raises:.
-00011590: 2020 2020 2020 2020 5661 6c75 6545 7272          ValueErr
-000115a0: 6f72 3a20 6966 2074 6865 2070 726f 7669  or: if the provi
-000115b0: 6465 6420 6172 6775 6d65 6e74 7320 6172  ded arguments ar
-000115c0: 6520 6e6f 7420 696e 2074 6865 2063 6f72  e not in the cor
-000115d0: 7265 6374 2066 6f72 6d61 742c 206f 7220  rect format, or 
-000115e0: 6966 2074 6865 2073 7461 7274 2074 696d  if the start tim
-000115f0: 6520 6973 2067 7265 6174 6572 2074 6861  e is greater tha
-00011600: 6e20 7468 6520 656e 6420 7469 6d65 0a0a  n the end time..
-00011610: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00011620: 2020 2020 2061 2044 5350 2069 6e74 6572       a DSP inter
-00011630: 7661 6c20 7661 6c75 6520 696e 2074 6865  val value in the
-00011640: 2066 6f72 6d61 7420 2773 7461 7274 5f73   format 'start_s
-00011650: 6563 6f6e 6473 3a65 6e64 5f73 6563 6f6e  econds:end_secon
-00011660: 6473 270a 0a20 2020 2045 7861 6d70 6c65  ds'..    Example
-00011670: 733a 0a20 2020 2020 2020 203e 3e3e 2065  s:.        >>> e
-00011680: 7863 656c 3278 6d6c 2e63 7265 6174 655f  xcel2xml.create_
-00011690: 696e 7465 7276 616c 5f76 616c 7565 2822  interval_value("
-000116a0: 303a 3031 3a30 3022 2c20 2230 3a30 323a  0:01:00", "0:02:
-000116b0: 3030 2229 0a20 2020 2020 2020 2022 3630  00").        "60
-000116c0: 3a31 3230 220a 2020 2020 2020 2020 3e3e  :120".        >>
-000116d0: 3e20 6578 6365 6c32 786d 6c2e 6372 6561  > excel2xml.crea
-000116e0: 7465 5f69 6e74 6572 7661 6c5f 7661 6c75  te_interval_valu
-000116f0: 6528 2230 3a30 313a 3030 2e35 222c 2022  e("0:01:00.5", "
-00011700: 303a 3031 3a30 302e 3622 290a 2020 2020  0:01:00.6").    
-00011710: 2020 2020 2236 302e 353a 3630 2e36 220a      "60.5:60.6".
-00011720: 2020 2020 2222 220a 2020 2020 7374 6172      """.    star
-00011730: 745f 6d61 7463 6820 3d20 7265 6765 782e  t_match = regex.
-00011740: 7365 6172 6368 2872 225e 285c 642b 293a  search(r"^(\d+):
-00011750: 285b 302d 355d 5b30 2d39 5d29 3a28 5b30  ([0-5][0-9]):([0
-00011760: 2d35 5d5b 302d 395d 283f 3a5c 2e5b 302d  -5][0-9](?:\.[0-
-00011770: 395d 2b29 3f29 2422 2c20 7374 6172 7429  9]+)?)$", start)
-00011780: 0a20 2020 2065 6e64 5f6d 6174 6368 203d  .    end_match =
-00011790: 2072 6567 6578 2e6d 6174 6368 2872 225e   regex.match(r"^
-000117a0: 285c 642b 293a 285b 302d 355d 5b30 2d39  (\d+):([0-5][0-9
-000117b0: 5d29 3a28 5b30 2d35 5d5b 302d 395d 283f  ]):([0-5][0-9](?
-000117c0: 3a5c 2e5b 302d 395d 2b29 3f29 2422 2c20  :\.[0-9]+)?)$", 
-000117d0: 656e 6429 0a20 2020 2069 6620 6e6f 7420  end).    if not 
-000117e0: 7374 6172 745f 6d61 7463 6820 6f72 206e  start_match or n
-000117f0: 6f74 2065 6e64 5f6d 6174 6368 3a0a 2020  ot end_match:.  
-00011800: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00011810: 6545 7272 6f72 2822 5468 6520 7374 6172  eError("The star
-00011820: 7420 616e 6420 656e 6420 7661 6c75 6573  t and end values
-00011830: 206d 7573 7420 6265 2069 6e20 7468 6520   must be in the 
-00011840: 666f 726d 6174 2027 4828 4829 3a4d 4d3a  format 'H(H):MM:
-00011850: 5353 282e 7329 2722 290a 2020 2020 7374  SS(.s)'").    st
-00011860: 6172 745f 682c 2073 7461 7274 5f6d 2c20  art_h, start_m, 
-00011870: 7374 6172 745f 7320 3d20 7374 6172 745f  start_s = start_
-00011880: 6d61 7463 682e 6772 6f75 7073 2829 0a20  match.groups(). 
-00011890: 2020 2065 6e64 5f68 2c20 656e 645f 6d2c     end_h, end_m,
-000118a0: 2065 6e64 5f73 203d 2065 6e64 5f6d 6174   end_s = end_mat
-000118b0: 6368 2e67 726f 7570 7328 290a 2020 2020  ch.groups().    
-000118c0: 7374 6172 745f 7365 636f 6e64 7320 3d20  start_seconds = 
-000118d0: 696e 7428 7374 6172 745f 6829 202a 2033  int(start_h) * 3
-000118e0: 3630 3020 2b20 696e 7428 7374 6172 745f  600 + int(start_
-000118f0: 6d29 202a 2036 3020 2b20 666c 6f61 7428  m) * 60 + float(
-00011900: 7374 6172 745f 7329 0a20 2020 2065 6e64  start_s).    end
-00011910: 5f73 6563 6f6e 6473 203d 2069 6e74 2865  _seconds = int(e
-00011920: 6e64 5f68 2920 2a20 3336 3030 202b 2069  nd_h) * 3600 + i
-00011930: 6e74 2865 6e64 5f6d 2920 2a20 3630 202b  nt(end_m) * 60 +
-00011940: 2066 6c6f 6174 2865 6e64 5f73 290a 2020   float(end_s).  
-00011950: 2020 7374 6172 745f 7365 636f 6e64 7320    start_seconds 
-00011960: 3d20 696e 7428 7374 6172 745f 7365 636f  = int(start_seco
-00011970: 6e64 7329 2069 6620 7374 6172 745f 7365  nds) if start_se
-00011980: 636f 6e64 732e 6973 5f69 6e74 6567 6572  conds.is_integer
-00011990: 2829 2065 6c73 6520 7374 6172 745f 7365  () else start_se
-000119a0: 636f 6e64 730a 2020 2020 656e 645f 7365  conds.    end_se
-000119b0: 636f 6e64 7320 3d20 696e 7428 656e 645f  conds = int(end_
-000119c0: 7365 636f 6e64 7329 2069 6620 656e 645f  seconds) if end_
-000119d0: 7365 636f 6e64 732e 6973 5f69 6e74 6567  seconds.is_integ
-000119e0: 6572 2829 2065 6c73 6520 656e 645f 7365  er() else end_se
-000119f0: 636f 6e64 730a 2020 2020 6966 2073 7461  conds.    if sta
-00011a00: 7274 5f73 6563 6f6e 6473 203e 2065 6e64  rt_seconds > end
-00011a10: 5f73 6563 6f6e 6473 3a0a 2020 2020 2020  _seconds:.      
-00011a20: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00011a30: 6f72 2822 5468 6520 7374 6172 7420 7661  or("The start va
-00011a40: 6c75 6520 6d75 7374 2062 6520 736d 616c  lue must be smal
-00011a50: 6c65 7220 7468 616e 2074 6865 2065 6e64  ler than the end
-00011a60: 2076 616c 7565 2229 0a20 2020 2072 6574   value").    ret
-00011a70: 7572 6e20 6622 7b73 7461 7274 5f73 6563  urn f"{start_sec
-00011a80: 6f6e 6473 7d3a 7b65 6e64 5f73 6563 6f6e  onds}:{end_secon
-00011a90: 6473 7d22 0a0a 0a64 6566 2063 7265 6174  ds}"...def creat
-00011aa0: 655f 6a73 6f6e 5f65 7863 656c 5f6c 6973  e_json_excel_lis
-00011ab0: 745f 6d61 7070 696e 6728 0a20 2020 2070  t_mapping(.    p
-00011ac0: 6174 685f 746f 5f6a 736f 6e3a 2073 7472  ath_to_json: str
-00011ad0: 2c0a 2020 2020 6c69 7374 5f6e 616d 653a  ,.    list_name:
-00011ae0: 2073 7472 2c0a 2020 2020 6578 6365 6c5f   str,.    excel_
-00011af0: 7661 6c75 6573 3a20 4974 6572 6162 6c65  values: Iterable
-00011b00: 5b73 7472 5d2c 0a20 2020 2073 6570 3a20  [str],.    sep: 
-00011b10: 7374 7220 3d20 272b 222a c3a7 2526 2f28  str = '+"*..%&/(
-00011b20: 293d 272c 0a20 2020 2063 6f72 7265 6374  )=',.    correct
-00011b30: 696f 6e73 3a20 4f70 7469 6f6e 616c 5b64  ions: Optional[d
-00011b40: 6963 745b 7374 722c 2073 7472 5d5d 203d  ict[str, str]] =
-00011b50: 204e 6f6e 652c 0a29 202d 3e20 6469 6374   None,.) -> dict
-00011b60: 5b73 7472 2c20 7374 725d 3a0a 2020 2020  [str, str]:.    
-00011b70: 2222 220a 2020 2020 4f66 7465 6e2c 2064  """.    Often, d
-00011b80: 6174 6120 736f 7572 6365 7320 636f 6e74  ata sources cont
-00011b90: 6169 6e20 6c69 7374 2076 616c 7565 7320  ain list values 
-00011ba0: 7468 6174 2061 7265 6e27 7420 6964 656e  that aren't iden
-00011bb0: 7469 6361 6c20 746f 2074 6865 206e 616d  tical to the nam
-00011bc0: 6520 6f66 2074 6865 206e 6f64 6520 696e  e of the node in
-00011bd0: 2074 6865 206c 6973 7420 6f66 2074 6865   the list of the
-00011be0: 204a 534f 4e0a 2020 2020 7072 6f6a 6563   JSON.    projec
-00011bf0: 7420 6669 6c65 2028 636f 6c6c 6f71 7569  t file (colloqui
-00011c00: 616c 6c79 3a20 6f6e 746f 6c6f 6779 292e  ally: ontology).
-00011c10: 2049 6e20 6f72 6465 7220 746f 2063 7265   In order to cre
-00011c20: 6174 6520 6120 636f 7272 6563 7420 584d  ate a correct XM
-00011c30: 4c20 666f 7220 7468 6520 6064 7370 2d74  L for the `dsp-t
-00011c40: 6f6f 6c73 2078 6d6c 7570 6c6f 6164 602c  ools xmlupload`,
-00011c50: 2061 206d 6170 7069 6e67 2069 730a 2020   a mapping is.  
-00011c60: 2020 6e65 6365 7373 6172 792e 2054 6869    necessary. Thi
-00011c70: 7320 6675 6e63 7469 6f6e 2074 616b 6573  s function takes
-00011c80: 2061 204a 534f 4e20 6c69 7374 2061 6e64   a JSON list and
-00011c90: 2061 6e20 4578 6365 6c20 636f 6c75 6d6e   an Excel column
-00011ca0: 2063 6f6e 7461 696e 696e 6720 6c69 7374   containing list
-00011cb0: 2d76 616c 7565 732c 2061 6e64 2074 7269  -values, and tri
-00011cc0: 6573 2074 6f20 6d61 7463 6820 7468 656d  es to match them
-00011cd0: 0a20 2020 2061 7574 6f6d 6174 6963 616c  .    automatical
-00011ce0: 6c79 2062 6173 6564 206f 6e20 7369 6d69  ly based on simi
-00011cf0: 6c61 7269 7479 2e20 5468 6520 7265 7375  larity. The resu
-00011d00: 6c74 2069 7320 6120 6469 6374 206f 6620  lt is a dict of 
-00011d10: 7468 6520 666f 726d 207b 6578 6365 6c5f  the form {excel_
-00011d20: 7661 6c75 653a 206c 6973 745f 6e6f 6465  value: list_node
-00011d30: 5f6e 616d 657d 2e0a 0a20 2020 2041 6c74  _name}...    Alt
-00011d40: 6572 6e61 7469 7665 6c79 2c20 636f 6e73  ernatively, cons
-00011d50: 6964 6572 2075 7369 6e67 2074 6865 2066  ider using the f
-00011d60: 756e 6374 696f 6e20 6372 6561 7465 5f6a  unction create_j
-00011d70: 736f 6e5f 6c69 7374 5f6d 6170 7069 6e67  son_list_mapping
-00011d80: 2829 2c20 7768 6963 6820 616c 736f 2062  (), which also b
-00011d90: 7569 6c64 7320 6120 6469 6374 696f 6e61  uilds a dictiona
-00011da0: 7279 2c0a 2020 2020 6275 7420 6672 6f6d  ry,.    but from
-00011db0: 2074 6865 206e 616d 6573 2061 6e64 206c   the names and l
-00011dc0: 6162 656c 7320 696e 2074 6865 204a 534f  abels in the JSO
-00011dd0: 4e20 6c69 7374 2c20 7768 6963 6820 6973  N list, which is
-00011de0: 206c 6573 7320 6572 726f 722d 7072 6f6e   less error-pron
-00011df0: 6520 7468 616e 2074 6869 7320 6675 6e63  e than this func
-00011e00: 7469 6f6e 2773 2061 7070 726f 6163 682e  tion's approach.
-00011e10: 2048 6f77 6576 6572 2c0a 2020 2020 7468   However,.    th
-00011e20: 6973 2066 756e 6374 696f 6e20 6861 7320  is function has 
-00011e30: 7468 6520 6164 7661 6e74 6167 6520 7468  the advantage th
-00011e40: 6174 2069 7420 6576 656e 2077 6f72 6b73  at it even works
-00011e50: 2077 6865 6e20 796f 7572 2064 6174 6120   when your data 
-00011e60: 736f 7572 6365 2064 6f65 736e 2774 2075  source doesn't u
-00011e70: 7365 2074 6865 206c 6973 7420 6c61 6265  se the list labe
-00011e80: 6c73 2063 6f72 7265 6374 6c79 2e0a 0a20  ls correctly... 
-00011e90: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00011ea0: 2070 6174 685f 746f 5f6a 736f 6e3a 2070   path_to_json: p
-00011eb0: 6174 6820 746f 2074 6865 204a 534f 4e20  ath to the JSON 
-00011ec0: 7072 6f6a 6563 7420 6669 6c65 0a20 2020  project file.   
-00011ed0: 2020 2020 206c 6973 745f 6e61 6d65 3a20       list_name: 
-00011ee0: 6e61 6d65 206f 6620 7468 6520 6c69 7374  name of the list
-00011ef0: 2069 6e20 7468 6520 4a53 4f4e 2070 726f   in the JSON pro
-00011f00: 6a65 6374 2066 696c 6520 2863 616e 2061  ject file (can a
-00011f10: 6c73 6f20 6265 2061 206e 6573 7465 6420  lso be a nested 
-00011f20: 6c69 7374 290a 2020 2020 2020 2020 6578  list).        ex
-00011f30: 6365 6c5f 7661 6c75 6573 3a20 7468 6520  cel_values: the 
-00011f40: 4578 6365 6c20 636f 6c75 6d6e 2028 652e  Excel column (e.
-00011f50: 672e 2061 7320 6c69 7374 2920 7769 7468  g. as list) with
-00011f60: 2074 6865 206c 6973 7420 7661 6c75 6573   the list values
-00011f70: 2069 6e20 6974 0a20 2020 2020 2020 2073   in it.        s
-00011f80: 6570 3a20 7365 7061 7261 746f 7220 7374  ep: separator st
-00011f90: 7269 6e67 2c20 6966 2074 6865 2063 656c  ring, if the cel
-00011fa0: 6c73 2069 6e20 7468 6520 4578 6365 6c20  ls in the Excel 
-00011fb0: 636f 6e74 6169 6e20 6d6f 7265 2074 6861  contain more tha
-00011fc0: 6e20 6f6e 6520 6c69 7374 2065 6e74 7279  n one list entry
-00011fd0: 0a20 2020 2020 2020 2063 6f72 7265 6374  .        correct
-00011fe0: 696f 6e73 3a20 6469 6374 2077 6974 6820  ions: dict with 
-00011ff0: 7772 6f6e 6720 656e 7472 6965 732c 2065  wrong entries, e
-00012000: 6163 6820 706f 696e 7469 6e67 2074 6f20  ach pointing to 
-00012010: 6974 7320 636f 7272 6563 7420 636f 756e  its correct coun
-00012020: 7465 7270 6172 740a 0a20 2020 2052 6169  terpart..    Rai
-00012030: 7365 733a 0a20 2020 2020 2020 2057 6172  ses:.        War
-00012040: 6e69 6e67 3a20 6966 2074 6865 7265 2069  ning: if there i
-00012050: 7320 616e 2045 7863 656c 2076 616c 7565  s an Excel value
-00012060: 2074 6861 7420 636f 756c 646e 2774 2062   that couldn't b
-00012070: 6520 6d61 7463 6865 640a 2020 2020 2020  e matched.      
-00012080: 2020 4578 6365 7074 696f 6e3a 2069 6620    Exception: if 
-00012090: 7468 6520 7061 7468 2064 6f65 736e 2774  the path doesn't
-000120a0: 2070 6f69 6e74 2074 6f20 6120 4a53 4f4e   point to a JSON
-000120b0: 2070 726f 6a65 6374 2066 696c 650a 0a20   project file.. 
-000120c0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-000120d0: 2020 2020 6469 6374 206f 6620 7468 6520      dict of the 
-000120e0: 666f 726d 2060 607b 6578 6365 6c5f 7661  form ``{excel_va
-000120f0: 6c75 653a 206c 6973 745f 6e6f 6465 5f6e  lue: list_node_n
-00012100: 616d 657d 6060 2e0a 2020 2020 2020 2020  ame}``..        
-00012110: 2020 2020 4576 6572 7920 6578 6365 6c5f      Every excel_
-00012120: 7661 6c75 6520 6973 2073 7472 6970 7065  value is strippe
-00012130: 642c 2061 6e64 2061 6c73 6f20 7072 6573  d, and also pres
-00012140: 656e 7420 696e 2061 206c 6f77 6572 6361  ent in a lowerca
-00012150: 7365 2066 6f72 6d2e 0a0a 2020 2020 4578  se form...    Ex
-00012160: 616d 706c 6573 3a0a 2020 2020 2020 2020  amples:.        
-00012170: 3e3e 3e20 6a73 6f6e 5f6c 6973 745f 6e6f  >>> json_list_no
-00012180: 6465 7320 3d20 5b0a 2020 2020 2020 2020  des = [.        
-00012190: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-000121a0: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-000121b0: 616d 6522 3a20 2267 6972 6166 6665 222c  ame": "giraffe",
-000121c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000121d0: 2020 2020 2022 6c61 6265 6c73 223a 207b       "labels": {
-000121e0: 2265 6e22 3a20 2267 6972 6166 6665 227d  "en": "giraffe"}
-000121f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012200: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00012210: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00012220: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
-00012230: 3a20 2261 6e74 656c 6f70 6522 2c0a 2020  : "antelope",.  
-00012240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012250: 2020 226c 6162 656c 7322 3a20 7b22 656e    "labels": {"en
-00012260: 223a 2022 616e 7465 6c6f 7065 227d 0a20  ": "antelope"}. 
-00012270: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00012280: 0a20 2020 2020 2020 2020 2020 205d 0a20  .            ]. 
-00012290: 2020 2020 2020 203e 3e3e 2065 7863 656c         >>> excel
-000122a0: 5f72 6f77 5f31 203d 205b 2247 6972 6166  _row_1 = ["Giraf
-000122b0: 6665 6568 2022 2c20 2220 416e 7469 6c6f  feeh ", " Antilo
-000122c0: 7570 6522 2c20 2247 6972 7261 6666 6520  upe", "Girraffe 
-000122d0: 2c20 416e 7469 6c6f 7570 6520 225d 0a20  , Antiloupe "]. 
-000122e0: 2020 2020 2020 203e 3e3e 206a 736f 6e5f         >>> json_
-000122f0: 6578 6365 6c5f 6c69 7374 5f6d 6170 7069  excel_list_mappi
-00012300: 6e67 203d 207b 0a20 2020 2020 2020 2020  ng = {.         
-00012310: 2020 2020 2020 2022 4769 7261 6666 6565         "Giraffee
-00012320: 6822 3a20 2267 6972 6166 6665 222c 0a20  h": "giraffe",. 
-00012330: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00012340: 6769 7261 6666 6565 6822 3a20 2267 6972  giraffeeh": "gir
-00012350: 6166 6665 222c 0a20 2020 2020 2020 2020  affe",.         
-00012360: 2020 2020 2020 2022 4769 7272 6166 6665         "Girraffe
-00012370: 223a 2022 6769 7261 6666 6522 2c0a 2020  ": "giraffe",.  
-00012380: 2020 2020 2020 2020 2020 2020 2020 2267                "g
-00012390: 6972 7261 6666 6522 3a20 2267 6972 6166  irraffe": "giraf
-000123a0: 6665 222c 0a20 2020 2020 2020 2020 2020  fe",.           
-000123b0: 2020 2020 2022 416e 7469 6c6f 7570 6522       "Antiloupe"
-000123c0: 3a20 2261 6e74 656c 6f70 6522 2c0a 2020  : "antelope",.  
-000123d0: 2020 2020 2020 2020 2020 2020 2020 2261                "a
-000123e0: 6e74 696c 6f75 7065 223a 2022 616e 7465  ntiloupe": "ante
-000123f0: 6c6f 7065 220a 2020 2020 2020 2020 2020  lope".          
-00012400: 2020 7d0a 2020 2020 2222 220a 0a20 2020    }.    """..   
-00012410: 2023 2061 766f 6964 206d 7574 6162 6c65   # avoid mutable
-00012420: 2064 6566 6175 6c74 2061 7267 756d 656e   default argumen
-00012430: 740a 2020 2020 636f 7272 6563 7469 6f6e  t.    correction
-00012440: 7320 3d20 636f 7272 6563 7469 6f6e 7320  s = corrections 
-00012450: 6f72 207b 7d0a 0a20 2020 2023 2073 706c  or {}..    # spl
-00012460: 6974 2074 6865 2076 616c 7565 732c 2069  it the values, i
-00012470: 6620 6e65 6365 7373 6172 790a 2020 2020  f necessary.    
-00012480: 6578 6365 6c5f 7661 6c75 6573 5f6e 6577  excel_values_new
-00012490: 203d 205b 5d0a 2020 2020 666f 7220 7661   = [].    for va
-000124a0: 6c20 696e 2065 7863 656c 5f76 616c 7565  l in excel_value
-000124b0: 733a 0a20 2020 2020 2020 2069 6620 6973  s:.        if is
-000124c0: 696e 7374 616e 6365 2876 616c 2c20 7374  instance(val, st
-000124d0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-000124e0: 6578 6365 6c5f 7661 6c75 6573 5f6e 6577  excel_values_new
-000124f0: 2e65 7874 656e 6428 5b78 2e73 7472 6970  .extend([x.strip
-00012500: 2829 2066 6f72 2078 2069 6e20 7661 6c2e  () for x in val.
-00012510: 7370 6c69 7428 7365 7029 2069 6620 785d  split(sep) if x]
-00012520: 290a 0a20 2020 2023 2072 6561 6420 7468  )..    # read th
-00012530: 6520 6c69 7374 206f 6620 7468 6520 4a53  e list of the JS
-00012540: 4f4e 2070 726f 6a65 6374 2028 776f 726b  ON project (work
-00012550: 7320 616c 736f 2066 6f72 206e 6573 7465  s also for neste
-00012560: 6420 6c69 7374 7329 0a20 2020 2077 6974  d lists).    wit
-00012570: 6820 6f70 656e 2870 6174 685f 746f 5f6a  h open(path_to_j
-00012580: 736f 6e2c 2065 6e63 6f64 696e 673d 2275  son, encoding="u
-00012590: 7466 2d38 2229 2061 7320 663a 0a20 2020  tf-8") as f:.   
-000125a0: 2020 2020 206a 736f 6e5f 6669 6c65 203d       json_file =
-000125b0: 206a 736f 6e2e 6c6f 6164 2866 290a 2020   json.load(f).  
-000125c0: 2020 6a73 6f6e 5f73 7562 7365 7420 3d20    json_subset = 
-000125d0: 5b5d 0a20 2020 2066 6f72 2065 6c65 6d20  [].    for elem 
-000125e0: 696e 206a 736f 6e5f 6669 6c65 5b22 7072  in json_file["pr
-000125f0: 6f6a 6563 7422 5d5b 226c 6973 7473 225d  oject"]["lists"]
-00012600: 3a0a 2020 2020 2020 2020 6966 2065 6c65  :.        if ele
-00012610: 6d5b 226e 616d 6522 5d20 3d3d 206c 6973  m["name"] == lis
-00012620: 745f 6e61 6d65 3a0a 2020 2020 2020 2020  t_name:.        
-00012630: 2020 2020 6a73 6f6e 5f73 7562 7365 7420      json_subset 
-00012640: 3d20 656c 656d 5b22 6e6f 6465 7322 5d0a  = elem["nodes"].
-00012650: 2020 2020 6a73 6f6e 5f76 616c 7565 7320      json_values 
-00012660: 3d20 7365 7428 5f6e 6573 7465 645f 6469  = set(_nested_di
-00012670: 6374 5f76 616c 7565 735f 6974 6572 6174  ct_values_iterat
-00012680: 6f72 286a 736f 6e5f 7375 6273 6574 2929  or(json_subset))
-00012690: 0a0a 2020 2020 2320 6275 696c 6420 6469  ..    # build di
-000126a0: 6374 696f 6e61 7279 2077 6974 6820 7468  ctionary with th
-000126b0: 6520 6d61 7070 696e 672c 2062 6173 6564  e mapping, based
-000126c0: 206f 6e20 7374 7269 6e67 2073 696d 696c   on string simil
-000126d0: 6172 6974 790a 2020 2020 7265 7320 3d20  arity.    res = 
-000126e0: 7b7d 0a20 2020 2066 6f72 2065 7863 656c  {}.    for excel
-000126f0: 5f76 616c 7565 2069 6e20 6578 6365 6c5f  _value in excel_
-00012700: 7661 6c75 6573 5f6e 6577 3a0a 2020 2020  values_new:.    
-00012710: 2020 2020 6578 6365 6c5f 7661 6c75 655f      excel_value_
-00012720: 636f 7272 6563 7465 6420 3d20 636f 7272  corrected = corr
-00012730: 6563 7469 6f6e 732e 6765 7428 6578 6365  ections.get(exce
-00012740: 6c5f 7661 6c75 652c 2065 7863 656c 5f76  l_value, excel_v
-00012750: 616c 7565 290a 2020 2020 2020 2020 6578  alue).        ex
-00012760: 6365 6c5f 7661 6c75 655f 7369 6d70 6c20  cel_value_simpl 
-00012770: 3d20 7369 6d70 6c69 6679 5f6e 616d 6528  = simplify_name(
-00012780: 6578 6365 6c5f 7661 6c75 655f 636f 7272  excel_value_corr
-00012790: 6563 7465 6429 2020 2320 696e 6372 6561  ected)  # increa
-000127a0: 7365 206d 6174 6368 2070 726f 6261 6269  se match probabi
-000127b0: 6c69 7479 2062 7920 7265 6d6f 7669 6e67  lity by removing
-000127c0: 2069 6c6c 6567 616c 2063 6861 7273 0a20   illegal chars. 
-000127d0: 2020 2020 2020 2069 6620 6d61 7463 6865         if matche
-000127e0: 7320 3a3d 2064 6966 666c 6962 2e67 6574  s := difflib.get
-000127f0: 5f63 6c6f 7365 5f6d 6174 6368 6573 280a  _close_matches(.
-00012800: 2020 2020 2020 2020 2020 2020 776f 7264              word
-00012810: 3d65 7863 656c 5f76 616c 7565 5f73 696d  =excel_value_sim
-00012820: 706c 2c0a 2020 2020 2020 2020 2020 2020  pl,.            
-00012830: 706f 7373 6962 696c 6974 6965 733d 6a73  possibilities=js
-00012840: 6f6e 5f76 616c 7565 732c 0a20 2020 2020  on_values,.     
-00012850: 2020 2020 2020 206e 3d31 2c0a 2020 2020         n=1,.    
-00012860: 2020 2020 2020 2020 6375 746f 6666 3d30          cutoff=0
-00012870: 2e36 2c0a 2020 2020 2020 2020 293a 0a20  .6,.        ):. 
-00012880: 2020 2020 2020 2020 2020 2072 6573 5b65             res[e
-00012890: 7863 656c 5f76 616c 7565 5d20 3d20 6d61  xcel_value] = ma
-000128a0: 7463 6865 735b 305d 0a20 2020 2020 2020  tches[0].       
-000128b0: 2020 2020 2072 6573 5b65 7863 656c 5f76       res[excel_v
-000128c0: 616c 7565 2e6c 6f77 6572 2829 5d20 3d20  alue.lower()] = 
-000128d0: 6d61 7463 6865 735b 305d 0a20 2020 2020  matches[0].     
-000128e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000128f0: 2020 2020 206d 7367 203d 2028 0a20 2020       msg = (.   
-00012900: 2020 2020 2020 2020 2020 2020 2066 2244               f"D
-00012910: 6964 206e 6f74 2066 696e 6420 6120 636c  id not find a cl
-00012920: 6f73 6520 6d61 7463 6820 746f 2074 6865  ose match to the
-00012930: 2065 7863 656c 206c 6973 7420 656e 7472   excel list entr
-00012940: 7920 277b 6578 6365 6c5f 7661 6c75 657d  y '{excel_value}
-00012950: 2720 220a 2020 2020 2020 2020 2020 2020  ' ".            
-00012960: 2020 2020 6622 616d 6f6e 6720 7468 6520      f"among the 
-00012970: 7661 6c75 6573 2069 6e20 7468 6520 4a53  values in the JS
-00012980: 4f4e 2070 726f 6a65 6374 206c 6973 7420  ON project list 
-00012990: 277b 6c69 7374 5f6e 616d 657d 2722 0a20  '{list_name}'". 
-000129a0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-000129b0: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
-000129c0: 732e 7761 726e 2844 7370 546f 6f6c 7355  s.warn(DspToolsU
-000129d0: 7365 7257 6172 6e69 6e67 286d 7367 2929  serWarning(msg))
-000129e0: 0a0a 2020 2020 7265 7475 726e 2072 6573  ..    return res
-000129f0: 0a0a 0a64 6566 205f 6e65 7374 6564 5f64  ...def _nested_d
-00012a00: 6963 745f 7661 6c75 6573 5f69 7465 7261  ict_values_itera
-00012a10: 746f 7228 6469 6374 733a 206c 6973 745b  tor(dicts: list[
-00012a20: 6469 6374 5b73 7472 2c20 416e 795d 5d29  dict[str, Any]])
-00012a30: 202d 3e20 4974 6572 6162 6c65 5b73 7472   -> Iterable[str
-00012a40: 5d3a 0a20 2020 2022 2222 0a20 2020 2059  ]:.    """.    Y
-00012a50: 6965 6c64 2061 6c6c 2076 616c 7565 7320  ield all values 
-00012a60: 6f66 2061 206e 6573 7465 6420 6469 6374  of a nested dict
-00012a70: 696f 6e61 7279 2e0a 0a20 2020 2041 7267  ionary...    Arg
-00012a80: 733a 0a20 2020 2020 2020 2064 6963 7473  s:.        dicts
-00012a90: 3a20 6c69 7374 206f 6620 6e65 7374 6564  : list of nested
-00012aa0: 2064 6963 7469 6f6e 6172 6965 730a 0a20   dictionaries.. 
-00012ab0: 2020 2059 6965 6c64 733a 0a20 2020 2020     Yields:.     
-00012ac0: 2020 2076 616c 7565 7320 6f66 2074 6865     values of the
-00012ad0: 206e 6573 7465 6420 6469 6374 696f 6e61   nested dictiona
-00012ae0: 7269 6573 0a20 2020 2022 2222 0a20 2020  ries.    """.   
-00012af0: 2023 2043 7265 6469 7473 3a20 6874 7470   # Credits: http
-00012b00: 733a 2f2f 7468 6973 706f 696e 7465 722e  s://thispointer.
-00012b10: 636f 6d2f 7079 7468 6f6e 2d69 7465 7261  com/python-itera
-00012b20: 7465 2d6c 6f6f 702d 6f76 6572 2d61 6c6c  te-loop-over-all
-00012b30: 2d6e 6573 7465 642d 6469 6374 696f 6e61  -nested-dictiona
-00012b40: 7279 2d76 616c 7565 732f 0a20 2020 2066  ry-values/.    f
-00012b50: 6f72 205f 6469 6374 2069 6e20 6469 6374  or _dict in dict
-00012b60: 733a 0a20 2020 2020 2020 2069 6620 226e  s:.        if "n
-00012b70: 6f64 6573 2220 696e 205f 6469 6374 3a0a  odes" in _dict:.
-00012b80: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
-00012b90: 6420 6672 6f6d 205f 6e65 7374 6564 5f64  d from _nested_d
-00012ba0: 6963 745f 7661 6c75 6573 5f69 7465 7261  ict_values_itera
-00012bb0: 746f 7228 5f64 6963 745b 226e 6f64 6573  tor(_dict["nodes
-00012bc0: 225d 290a 2020 2020 2020 2020 6966 2022  "]).        if "
-00012bd0: 6e61 6d65 2220 696e 205f 6469 6374 3a0a  name" in _dict:.
-00012be0: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
-00012bf0: 6420 5f64 6963 745b 226e 616d 6522 5d0a  d _dict["name"].
-00012c00: 0a0a 6465 6620 6372 6561 7465 5f6a 736f  ..def create_jso
-00012c10: 6e5f 6c69 7374 5f6d 6170 7069 6e67 280a  n_list_mapping(.
-00012c20: 2020 2020 7061 7468 5f74 6f5f 6a73 6f6e      path_to_json
-00012c30: 3a20 7374 722c 0a20 2020 206c 6973 745f  : str,.    list_
-00012c40: 6e61 6d65 3a20 7374 722c 0a20 2020 206c  name: str,.    l
-00012c50: 616e 6775 6167 655f 6c61 6265 6c3a 2073  anguage_label: s
-00012c60: 7472 2c0a 2920 2d3e 2064 6963 745b 7374  tr,.) -> dict[st
-00012c70: 722c 2073 7472 5d3a 0a20 2020 2022 2222  r, str]:.    """
-00012c80: 0a20 2020 204f 6674 656e 2c20 6461 7461  .    Often, data
-00012c90: 2073 6f75 7263 6573 2063 6f6e 7461 696e   sources contain
-00012ca0: 206c 6973 7420 7661 6c75 6573 206e 616d   list values nam
-00012cb0: 6564 2061 6674 6572 2074 6865 2022 6c61  ed after the "la
-00012cc0: 6265 6c22 206f 6620 7468 6520 4a53 4f4e  bel" of the JSON
-00012cd0: 2070 726f 6a65 6374 206c 6973 7420 6e6f   project list no
-00012ce0: 6465 2c20 696e 7374 6561 6420 6f66 2074  de, instead of t
-00012cf0: 6865 2022 6e61 6d65 220a 2020 2020 7768  he "name".    wh
-00012d00: 6963 6820 6973 206e 6565 6465 6420 666f  ich is needed fo
-00012d10: 7220 7468 6520 6064 7370 2d74 6f6f 6c73  r the `dsp-tools
-00012d20: 2078 6d6c 7570 6c6f 6164 602e 2049 6e20   xmlupload`. In 
-00012d30: 6f72 6465 7220 746f 2063 7265 6174 6520  order to create 
-00012d40: 6120 636f 7272 6563 7420 584d 4c2c 2079  a correct XML, y
-00012d50: 6f75 206e 6565 6420 6120 6469 6374 696f  ou need a dictio
-00012d60: 6e61 7279 2074 6861 7420 6d61 7073 2074  nary that maps t
-00012d70: 6865 0a20 2020 2022 6c61 6265 6c73 2220  he.    "labels" 
-00012d80: 746f 2074 6865 6972 2063 6f72 7265 6374  to their correct
-00012d90: 2022 6e61 6d65 7322 2e0a 0a20 2020 2041   "names"...    A
-00012da0: 6c74 6572 6e61 7469 7665 6c79 2c20 636f  lternatively, co
-00012db0: 6e73 6964 6572 2075 7369 6e67 2074 6865  nsider using the
-00012dc0: 206d 6574 686f 6420 6372 6561 7465 5f6a   method create_j
-00012dd0: 736f 6e5f 6578 6365 6c5f 6c69 7374 5f6d  son_excel_list_m
-00012de0: 6170 7069 6e67 2829 2c20 7768 6963 6820  apping(), which 
-00012df0: 616c 736f 2063 7265 6174 6573 2061 2064  also creates a d
-00012e00: 6963 7469 6f6e 6172 792c 2062 7574 206d  ictionary, but m
-00012e10: 6170 730a 2020 2020 7661 6c75 6573 2066  aps.    values f
-00012e20: 726f 6d20 796f 7572 2064 6174 6120 736f  rom your data so
-00012e30: 7572 6365 2074 6f20 6c69 7374 206e 6f64  urce to list nod
-00012e40: 6520 6e61 6d65 7320 6672 6f6d 2074 6865  e names from the
-00012e50: 204a 534f 4e20 7072 6f6a 6563 7420 6669   JSON project fi
-00012e60: 6c65 2c20 6261 7365 6420 6f6e 2073 696d  le, based on sim
-00012e70: 696c 6172 6974 792e 0a0a 2020 2020 4172  ilarity...    Ar
-00012e80: 6773 3a0a 2020 2020 2020 2020 7061 7468  gs:.        path
-00012e90: 5f74 6f5f 6a73 6f6e 3a20 7061 7468 2074  _to_json: path t
-00012ea0: 6f20 6120 4a53 4f4e 2070 726f 6a65 6374  o a JSON project
-00012eb0: 2066 696c 6520 2861 2e6b 2e61 2e20 6f6e   file (a.k.a. on
-00012ec0: 746f 6c6f 6779 290a 2020 2020 2020 2020  tology).        
-00012ed0: 6c69 7374 5f6e 616d 653a 206e 616d 6520  list_name: name 
-00012ee0: 6f66 2061 206c 6973 7420 696e 2074 6865  of a list in the
-00012ef0: 204a 534f 4e20 7072 6f6a 6563 7420 2877   JSON project (w
-00012f00: 6f72 6b73 2061 6c73 6f20 666f 7220 6e65  orks also for ne
-00012f10: 7374 6564 206c 6973 7473 290a 2020 2020  sted lists).    
-00012f20: 2020 2020 6c61 6e67 7561 6765 5f6c 6162      language_lab
-00012f30: 656c 3a20 7768 6963 6820 6c61 6e67 7561  el: which langua
-00012f40: 6765 206f 6620 7468 6520 6c61 6265 6c20  ge of the label 
-00012f50: 746f 2063 686f 6f73 650a 0a20 2020 2052  to choose..    R
-00012f60: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00012f70: 6120 6469 6374 696f 6e61 7279 206f 6620  a dictionary of 
-00012f80: 7468 6520 666f 726d 207b 6c61 6265 6c3a  the form {label:
-00012f90: 206e 616d 657d 0a20 2020 2022 2222 0a20   name}.    """. 
-00012fa0: 2020 2077 6974 6820 6f70 656e 2870 6174     with open(pat
-00012fb0: 685f 746f 5f6a 736f 6e2c 2065 6e63 6f64  h_to_json, encod
-00012fc0: 696e 673d 2275 7466 2d38 2229 2061 7320  ing="utf-8") as 
-00012fd0: 663a 0a20 2020 2020 2020 206a 736f 6e5f  f:.        json_
-00012fe0: 6669 6c65 203d 206a 736f 6e2e 6c6f 6164  file = json.load
-00012ff0: 2866 290a 2020 2020 6a73 6f6e 5f73 7562  (f).    json_sub
-00013000: 7365 7420 3d20 5b78 2066 6f72 2078 2069  set = [x for x i
-00013010: 6e20 6a73 6f6e 5f66 696c 655b 2270 726f  n json_file["pro
-00013020: 6a65 6374 225d 5b22 6c69 7374 7322 5d20  ject"]["lists"] 
-00013030: 6966 2078 5b22 6e61 6d65 225d 203d 3d20  if x["name"] == 
-00013040: 6c69 7374 5f6e 616d 655d 0a20 2020 2023  list_name].    #
-00013050: 206a 736f 6e5f 7375 6273 6574 2069 7320   json_subset is 
-00013060: 6120 6c69 7374 2063 6f6e 7461 696e 696e  a list containin
-00013070: 6720 6f6e 6520 6974 656d 2c20 6e61 6d65  g one item, name
-00013080: 6c79 2074 6865 206a 736f 6e20 6f62 6a65  ly the json obje
-00013090: 6374 2063 6f6e 7461 696e 696e 6720 7468  ct containing th
-000130a0: 6520 656e 7469 7265 206a 736f 6e2d 6c69  e entire json-li
-000130b0: 7374 0a0a 2020 2020 7265 7320 3d20 7b7d  st..    res = {}
-000130c0: 0a20 2020 2066 6f72 206c 6162 656c 2c20  .    for label, 
-000130d0: 6e61 6d65 2069 6e20 5f6e 616d 655f 6c61  name in _name_la
-000130e0: 6265 6c5f 6d61 7070 6572 5f69 7465 7261  bel_mapper_itera
-000130f0: 746f 7228 6a73 6f6e 5f73 7562 7365 742c  tor(json_subset,
-00013100: 206c 616e 6775 6167 655f 6c61 6265 6c29   language_label)
-00013110: 3a0a 2020 2020 2020 2020 6966 206e 616d  :.        if nam
-00013120: 6520 213d 206c 6973 745f 6e61 6d65 3a0a  e != list_name:.
-00013130: 2020 2020 2020 2020 2020 2020 7265 735b              res[
-00013140: 6c61 6265 6c5d 203d 206e 616d 650a 2020  label] = name.  
-00013150: 2020 2020 2020 2020 2020 7265 735b 6c61            res[la
-00013160: 6265 6c2e 7374 7269 7028 292e 6c6f 7765  bel.strip().lowe
-00013170: 7228 295d 203d 206e 616d 650a 0a20 2020  r()] = name..   
-00013180: 2072 6574 7572 6e20 7265 730a 0a0a 6465   return res...de
-00013190: 6620 5f6e 616d 655f 6c61 6265 6c5f 6d61  f _name_label_ma
-000131a0: 7070 6572 5f69 7465 7261 746f 7228 0a20  pper_iterator(. 
-000131b0: 2020 206a 736f 6e5f 7375 6273 6574 3a20     json_subset: 
-000131c0: 6c69 7374 5b64 6963 745b 7374 722c 2041  list[dict[str, A
-000131d0: 6e79 5d5d 2c0a 2020 2020 6c61 6e67 7561  ny]],.    langua
-000131e0: 6765 5f6c 6162 656c 3a20 7374 722c 0a29  ge_label: str,.)
-000131f0: 202d 3e20 4974 6572 6162 6c65 5b74 7570   -> Iterable[tup
-00013200: 6c65 5b73 7472 2c20 7374 725d 5d3a 0a20  le[str, str]]:. 
-00013210: 2020 2022 2222 0a20 2020 2047 6f20 7468     """.    Go th
-00013220: 726f 7567 6820 6c69 7374 206e 6f64 6573  rough list nodes
-00013230: 206f 6620 6120 4a53 4f4e 2070 726f 6a65   of a JSON proje
-00013240: 6374 2061 6e64 2079 6965 6c64 2028 6c61  ct and yield (la
-00013250: 6265 6c2c 206e 616d 6529 2070 6169 7273  bel, name) pairs
-00013260: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-00013270: 2020 2020 206a 736f 6e5f 7375 6273 6574       json_subset
-00013280: 3a20 6c69 7374 206f 6620 4453 5020 6c69  : list of DSP li
-00013290: 7374 7320 2861 2044 5350 206c 6973 7420  sts (a DSP list 
-000132a0: 6265 696e 6720 6120 6469 6374 696f 6e61  being a dictiona
-000132b0: 7279 2077 6974 6820 7468 6520 6b65 7973  ry with the keys
-000132c0: 2022 6e61 6d65 222c 2022 6c61 6265 6c73   "name", "labels
-000132d0: 2220 616e 6420 226e 6f64 6573 2229 0a20  " and "nodes"). 
-000132e0: 2020 2020 2020 206c 616e 6775 6167 655f         language_
-000132f0: 6c61 6265 6c3a 2077 6869 6368 206c 616e  label: which lan
-00013300: 6775 6167 6520 6f66 2074 6865 206c 6162  guage of the lab
-00013310: 656c 2074 6f20 6368 6f6f 7365 0a0a 2020  el to choose..  
-00013320: 2020 5969 656c 6473 3a0a 2020 2020 2020    Yields:.      
-00013330: 2020 286c 6162 656c 2c20 6e61 6d65 2920    (label, name) 
-00013340: 7061 6972 730a 2020 2020 2222 220a 2020  pairs.    """.  
-00013350: 2020 666f 7220 6e6f 6465 2069 6e20 6a73    for node in js
-00013360: 6f6e 5f73 7562 7365 743a 0a20 2020 2020  on_subset:.     
-00013370: 2020 2023 206e 6f64 6520 6973 2074 6865     # node is the
-00013380: 206a 736f 6e20 6f62 6a65 6374 2063 6f6e   json object con
-00013390: 7461 696e 696e 6720 7468 6520 656e 7469  taining the enti
-000133a0: 7265 206a 736f 6e2d 6c69 7374 0a20 2020  re json-list.   
-000133b0: 2020 2020 2069 6620 226e 6f64 6573 2220       if "nodes" 
-000133c0: 696e 206e 6f64 653a 0a20 2020 2020 2020  in node:.       
-000133d0: 2020 2020 2023 2022 6e6f 6465 7322 2069       # "nodes" i
-000133e0: 7320 7468 6520 6a73 6f6e 2073 7562 2d6f  s the json sub-o
-000133f0: 626a 6563 7420 636f 6e74 6169 6e69 6e67  bject containing
-00013400: 2074 6865 2065 6e74 7269 6573 206f 6620   the entries of 
-00013410: 7468 6520 6a73 6f6e 2d6c 6973 740a 2020  the json-list.  
-00013420: 2020 2020 2020 2020 2020 7969 656c 6420            yield 
-00013430: 6672 6f6d 205f 6e61 6d65 5f6c 6162 656c  from _name_label
-00013440: 5f6d 6170 7065 725f 6974 6572 6174 6f72  _mapper_iterator
-00013450: 286e 6f64 655b 226e 6f64 6573 225d 2c20  (node["nodes"], 
-00013460: 6c61 6e67 7561 6765 5f6c 6162 656c 290a  language_label).
-00013470: 2020 2020 2020 2020 2020 2020 2320 6561              # ea
-00013480: 6368 2079 6965 6c64 6564 2076 616c 7565  ch yielded value
-00013490: 2069 7320 6120 286c 6162 656c 2c20 6e61   is a (label, na
-000134a0: 6d65 2920 7061 6972 206f 6620 6120 7369  me) pair of a si
-000134b0: 6e67 6c65 206c 6973 7420 656e 7472 790a  ngle list entry.
-000134c0: 2020 2020 2020 2020 6966 2022 6e61 6d65          if "name
-000134d0: 2220 696e 206e 6f64 653a 0a20 2020 2020  " in node:.     
-000134e0: 2020 2020 2020 2079 6965 6c64 2028 6e6f         yield (no
-000134f0: 6465 5b22 6c61 6265 6c73 225d 5b6c 616e  de["labels"][lan
-00013500: 6775 6167 655f 6c61 6265 6c5d 2c20 6e6f  guage_label], no
-00013510: 6465 5b22 6e61 6d65 225d 290a 2020 2020  de["name"]).    
-00013520: 2020 2020 2020 2020 2320 7468 6520 6163          # the ac
-00013530: 7475 616c 2076 616c 7565 7320 6f66 2074  tual values of t
-00013540: 6865 206e 616d 6520 616e 6420 7468 6520  he name and the 
-00013550: 6c61 6265 6c0a 0a0a 6465 6620 7772 6974  label...def writ
-00013560: 655f 786d 6c28 0a20 2020 2072 6f6f 743a  e_xml(.    root:
-00013570: 2065 7472 6565 2e5f 456c 656d 656e 742c   etree._Element,
-00013580: 0a20 2020 2066 696c 6570 6174 683a 2073  .    filepath: s
-00013590: 7472 207c 2050 6174 682c 0a29 202d 3e20  tr | Path,.) -> 
-000135a0: 4e6f 6e65 3a0a 2020 2020 2222 220a 2020  None:.    """.  
-000135b0: 2020 5772 6974 6520 7468 6520 6669 6e69    Write the fini
-000135c0: 7368 6564 2058 4d4c 2074 6f20 6120 6669  shed XML to a fi
-000135d0: 6c65 2e0a 0a20 2020 2041 7267 733a 0a20  le...    Args:. 
-000135e0: 2020 2020 2020 2072 6f6f 743a 2065 7472         root: etr
-000135f0: 6565 2045 6c65 6d65 6e74 2077 6974 6820  ee Element with 
-00013600: 7468 6520 656e 7469 7265 2058 4d4c 2064  the entire XML d
-00013610: 6f63 756d 656e 740a 2020 2020 2020 2020  ocument.        
-00013620: 6669 6c65 7061 7468 3a20 7768 6572 6520  filepath: where 
-00013630: 746f 2073 6176 6520 7468 6520 6669 6c65  to save the file
-00013640: 0a0a 2020 2020 5761 726e 696e 673a 0a20  ..    Warning:. 
-00013650: 2020 2020 2020 2069 6620 7468 6520 584d         if the XM
-00013660: 4c20 6973 206e 6f74 2076 616c 6964 2061  L is not valid a
-00013670: 6363 6f72 6469 6e67 2074 6f20 7468 6520  ccording to the 
-00013680: 7363 6865 6d61 0a20 2020 2022 2222 0a20  schema.    """. 
-00013690: 2020 2065 7472 6565 2e69 6e64 656e 7428     etree.indent(
-000136a0: 726f 6f74 2c20 7370 6163 653d 2220 2020  root, space="   
-000136b0: 2022 290a 2020 2020 786d 6c5f 7374 7269   ").    xml_stri
-000136c0: 6e67 203d 2065 7472 6565 2e74 6f73 7472  ng = etree.tostr
-000136d0: 696e 6728 0a20 2020 2020 2020 2072 6f6f  ing(.        roo
-000136e0: 742c 0a20 2020 2020 2020 2065 6e63 6f64  t,.        encod
-000136f0: 696e 673d 2275 6e69 636f 6465 222c 0a20  ing="unicode",. 
-00013700: 2020 2020 2020 2070 7265 7474 795f 7072         pretty_pr
-00013710: 696e 743d 5472 7565 2c0a 2020 2020 2020  int=True,.      
-00013720: 2020 646f 6374 7970 653d 273c 3f78 6d6c    doctype='<?xml
-00013730: 2076 6572 7369 6f6e 3d22 312e 3022 2065   version="1.0" e
-00013740: 6e63 6f64 696e 673d 2255 5446 2d38 223f  ncoding="UTF-8"?
-00013750: 3e27 2c0a 2020 2020 290a 2020 2020 786d  >',.    ).    xm
-00013760: 6c5f 7374 7269 6e67 203d 2078 6d6c 5f73  l_string = xml_s
-00013770: 7472 696e 672e 7265 706c 6163 6528 7222  tring.replace(r"
-00013780: 5c27 222c 2022 2722 290a 2020 2020 7769  \'", "'").    wi
-00013790: 7468 206f 7065 6e28 6669 6c65 7061 7468  th open(filepath
-000137a0: 2c20 2277 222c 2065 6e63 6f64 696e 673d  , "w", encoding=
-000137b0: 2275 7466 2d38 2229 2061 7320 663a 0a20  "utf-8") as f:. 
-000137c0: 2020 2020 2020 2066 2e77 7269 7465 2878         f.write(x
-000137d0: 6d6c 5f73 7472 696e 6729 0a20 2020 2074  ml_string).    t
-000137e0: 7279 3a0a 2020 2020 2020 2020 7661 6c69  ry:.        vali
-000137f0: 6461 7465 5f78 6d6c 2869 6e70 7574 5f66  date_xml(input_f
-00013800: 696c 653d 6669 6c65 7061 7468 290a 2020  ile=filepath).  
-00013810: 2020 2020 2020 7072 696e 7428 6622 5468        print(f"Th
-00013820: 6520 584d 4c20 6669 6c65 2077 6173 2073  e XML file was s
-00013830: 7563 6365 7373 6675 6c6c 7920 7361 7665  uccessfully save
-00013840: 6420 746f 207b 6669 6c65 7061 7468 7d22  d to {filepath}"
-00013850: 290a 2020 2020 6578 6365 7074 2042 6173  ).    except Bas
-00013860: 6545 7272 6f72 2061 7320 6572 723a 0a20  eError as err:. 
-00013870: 2020 2020 2020 206d 7367 203d 2028 0a20         msg = (. 
-00013880: 2020 2020 2020 2020 2020 2066 2254 6865             f"The
-00013890: 2058 4d4c 2066 696c 6520 7761 7320 7375   XML file was su
-000138a0: 6363 6573 7366 756c 6c79 2073 6176 6564  ccessfully saved
-000138b0: 2074 6f20 7b66 696c 6570 6174 687d 2c20   to {filepath}, 
-000138c0: 220a 2020 2020 2020 2020 2020 2020 6622  ".            f"
-000138d0: 6275 7420 7468 6520 666f 6c6c 6f77 696e  but the followin
-000138e0: 6720 5363 6865 6d61 2076 616c 6964 6174  g Schema validat
-000138f0: 696f 6e20 6572 726f 7228 7329 206f 6363  ion error(s) occ
-00013900: 7572 7265 643a 207b 6572 722e 6d65 7373  urred: {err.mess
-00013910: 6167 657d 220a 2020 2020 2020 2020 290a  age}".        ).
-00013920: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
-00013930: 2e77 6172 6e28 4473 7054 6f6f 6c73 5573  .warn(DspToolsUs
-00013940: 6572 5761 726e 696e 6728 6d73 6729 290a  erWarning(msg)).
+0000e180: 2020 2020 2020 3230 3039 2d31 302d 3130        2009-10-10
+0000e190: 5431 323a 3030 3a30 302d 3035 3a30 300a  T12:00:00-05:00.
+0000e1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1b0: 2020 2020 3c2f 7469 6d65 3e0a 2020 2020      </time>.    
+0000e1c0: 2020 2020 2020 2020 2020 2020 3c2f 7469              </ti
+0000e1d0: 6d65 2d70 726f 703e 0a20 2020 2020 2020  me-prop>.       
+0000e1e0: 203e 3e3e 2065 7863 656c 3278 6d6c 2e6d   >>> excel2xml.m
+0000e1f0: 616b 655f 7469 6d65 5f70 726f 7028 223a  ake_time_prop(":
+0000e200: 7465 7374 7072 6f70 6572 7479 222c 205b  testproperty", [
+0000e210: 2232 3030 392d 3130 2d31 3054 3132 3a30  "2009-10-10T12:0
+0000e220: 303a 3030 2d30 353a 3030 222c 2022 3139  0:00-05:00", "19
+0000e230: 3031 2d30 312d 3031 5430 313a 3030 3a30  01-01-01T01:00:0
+0000e240: 302d 3030 3a30 3022 5d29 0a20 2020 2020  0-00:00"]).     
+0000e250: 2020 2020 2020 2020 2020 203c 7469 6d65             <time
+0000e260: 2d70 726f 7020 6e61 6d65 3d22 3a74 6573  -prop name=":tes
+0000e270: 7470 726f 7065 7274 7922 3e0a 2020 2020  tproperty">.    
+0000e280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e290: 3c74 696d 6520 7065 726d 6973 7369 6f6e  <time permission
+0000e2a0: 733d 2270 726f 702d 6465 6661 756c 7422  s="prop-default"
+0000e2b0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+0000e2c0: 2020 2020 2020 2020 2020 3230 3039 2d31            2009-1
+0000e2d0: 302d 3130 5431 323a 3030 3a30 302d 3035  0-10T12:00:00-05
+0000e2e0: 3a30 300a 2020 2020 2020 2020 2020 2020  :00.            
+0000e2f0: 2020 2020 2020 2020 3c2f 7469 6d65 3e0a          </time>.
+0000e300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e310: 2020 2020 3c74 696d 6520 7065 726d 6973      <time permis
+0000e320: 7369 6f6e 733d 2270 726f 702d 6465 6661  sions="prop-defa
+0000e330: 756c 7422 3e0a 2020 2020 2020 2020 2020  ult">.          
+0000e340: 2020 2020 2020 2020 2020 2020 2020 3139                19
+0000e350: 3031 2d30 312d 3031 5430 313a 3030 3a30  01-01-01T01:00:0
+0000e360: 302d 3030 3a30 3032 0a20 2020 2020 2020  0-00:002.       
+0000e370: 2020 2020 2020 2020 2020 2020 203c 2f74               </t
+0000e380: 696d 653e 0a20 2020 2020 2020 2020 2020  ime>.           
+0000e390: 2020 2020 203c 2f74 696d 652d 7072 6f70       </time-prop
+0000e3a0: 3e0a 0a20 2020 2053 6565 2068 7474 7073  >..    See https
+0000e3b0: 3a2f 2f64 6f63 732e 6461 7363 682e 7377  ://docs.dasch.sw
+0000e3c0: 6973 732f 6c61 7465 7374 2f44 5350 2d54  iss/latest/DSP-T
+0000e3d0: 4f4f 4c53 2f66 696c 652d 666f 726d 6174  OOLS/file-format
+0000e3e0: 732f 786d 6c2d 6461 7461 2d66 696c 652f  s/xml-data-file/
+0000e3f0: 2374 696d 652d 7072 6f70 0a20 2020 2022  #time-prop.    "
+0000e400: 2222 0a0a 2020 2020 2320 6368 6563 6b20  ""..    # check 
+0000e410: 7468 6520 696e 7075 743a 2070 7265 7061  the input: prepa
+0000e420: 7265 2061 206c 6973 7420 7769 7468 2076  re a list with v
+0000e430: 616c 6964 2076 616c 7565 730a 2020 2020  alid values.    
+0000e440: 7661 6c75 6573 203d 2070 7265 7061 7265  values = prepare
+0000e450: 5f76 616c 7565 2876 616c 7565 290a 0a20  _value(value).. 
+0000e460: 2020 2023 2063 6865 636b 2076 616c 7565     # check value
+0000e470: 2074 7970 650a 2020 2020 7661 6c69 6461   type.    valida
+0000e480: 7469 6f6e 5f72 6567 6578 203d 2072 225e  tion_regex = r"^
+0000e490: 5c64 7b34 7d2d 5b30 2d31 5d5c 642d 5b30  \d{4}-[0-1]\d-[0
+0000e4a0: 2d33 5d5c 6454 5b30 2d32 5d5c 643a 5b30  -3]\dT[0-2]\d:[0
+0000e4b0: 2d35 5d5c 643a 5b30 2d35 5d5c 6428 2e5c  -5]\d:[0-5]\d(.\
+0000e4c0: 647b 312c 3132 7d29 3f28 5a7c 5b2b 2d5d  d{1,12})?(Z|[+-]
+0000e4d0: 5b30 2d31 5d5c 643a 5b30 2d35 5d5c 6429  [0-1]\d:[0-5]\d)
+0000e4e0: 2422 0a20 2020 2066 6f72 2076 616c 2069  $".    for val i
+0000e4f0: 6e20 7661 6c75 6573 3a0a 2020 2020 2020  n values:.      
+0000e500: 2020 6966 206e 6f74 2072 6567 6578 2e73    if not regex.s
+0000e510: 6561 7263 6828 7661 6c69 6461 7469 6f6e  earch(validation
+0000e520: 5f72 6567 6578 2c20 7374 7228 7661 6c2e  _regex, str(val.
+0000e530: 7661 6c75 6529 293a 0a20 2020 2020 2020  value)):.       
+0000e540: 2020 2020 206d 7367 203d 2028 0a20 2020       msg = (.   
+0000e550: 2020 2020 2020 2020 2020 2020 2066 2246               f"F
+0000e560: 6169 6c65 6420 7661 6c69 6461 7469 6f6e  ailed validation
+0000e570: 2069 6e20 7265 736f 7572 6365 2027 7b63   in resource '{c
+0000e580: 616c 6c69 6e67 5f72 6573 6f75 7263 657d  alling_resource}
+0000e590: 272c 2070 726f 7065 7274 7920 277b 6e61  ', property '{na
+0000e5a0: 6d65 7d27 3a20 220a 2020 2020 2020 2020  me}': ".        
+0000e5b0: 2020 2020 2020 2020 6622 277b 7661 6c2e          f"'{val.
+0000e5c0: 7661 6c75 657d 2720 6973 206e 6f74 2061  value}' is not a
+0000e5d0: 2076 616c 6964 2044 5350 2074 696d 652e   valid DSP time.
+0000e5e0: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
+0000e5f0: 2020 2020 2020 2020 2020 2020 7761 726e              warn
+0000e600: 696e 6773 2e77 6172 6e28 4473 7054 6f6f  ings.warn(DspToo
+0000e610: 6c73 5573 6572 5761 726e 696e 6728 6d73  lsUserWarning(ms
+0000e620: 6729 290a 0a20 2020 2023 206d 616b 6520  g))..    # make 
+0000e630: 786d 6c20 7374 7275 6374 7572 6520 6f66  xml structure of
+0000e640: 2074 6865 2076 616c 6964 2076 616c 7565   the valid value
+0000e650: 730a 2020 2020 7072 6f70 5f20 3d20 6574  s.    prop_ = et
+0000e660: 7265 652e 456c 656d 656e 7428 0a20 2020  ree.Element(.   
+0000e670: 2020 2020 2022 7b25 737d 7469 6d65 2d70       "{%s}time-p
+0000e680: 726f 7022 2025 2078 6d6c 5f6e 616d 6573  rop" % xml_names
+0000e690: 7061 6365 5f6d 6170 5b4e 6f6e 655d 2c0a  pace_map[None],.
+0000e6a0: 2020 2020 2020 2020 6e61 6d65 3d6e 616d          name=nam
+0000e6b0: 652c 0a20 2020 2020 2020 206e 736d 6170  e,.        nsmap
+0000e6c0: 3d78 6d6c 5f6e 616d 6573 7061 6365 5f6d  =xml_namespace_m
+0000e6d0: 6170 2c0a 2020 2020 290a 2020 2020 666f  ap,.    ).    fo
+0000e6e0: 7220 7661 6c20 696e 2076 616c 7565 733a  r val in values:
+0000e6f0: 0a20 2020 2020 2020 206b 7761 7267 7320  .        kwargs 
+0000e700: 3d20 7b22 7065 726d 6973 7369 6f6e 7322  = {"permissions"
+0000e710: 3a20 7661 6c2e 7065 726d 6973 7369 6f6e  : val.permission
+0000e720: 737d 0a20 2020 2020 2020 2069 6620 7661  s}.        if va
+0000e730: 6c2e 636f 6d6d 656e 7420 616e 6420 6368  l.comment and ch
+0000e740: 6563 6b5f 6e6f 746e 6128 7661 6c2e 636f  eck_notna(val.co
+0000e750: 6d6d 656e 7429 3a0a 2020 2020 2020 2020  mment):.        
+0000e760: 2020 2020 6b77 6172 6773 5b22 636f 6d6d      kwargs["comm
+0000e770: 656e 7422 5d20 3d20 7661 6c2e 636f 6d6d  ent"] = val.comm
+0000e780: 656e 740a 2020 2020 2020 2020 7661 6c75  ent.        valu
+0000e790: 655f 203d 2065 7472 6565 2e45 6c65 6d65  e_ = etree.Eleme
+0000e7a0: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
+0000e7b0: 227b 2573 7d74 696d 6522 2025 2078 6d6c  "{%s}time" % xml
+0000e7c0: 5f6e 616d 6573 7061 6365 5f6d 6170 5b4e  _namespace_map[N
+0000e7d0: 6f6e 655d 2c0a 2020 2020 2020 2020 2020  one],.          
+0000e7e0: 2020 2a2a 6b77 6172 6773 2c20 2023 2074    **kwargs,  # t
+0000e7f0: 7970 653a 2069 676e 6f72 655b 6172 672d  ype: ignore[arg-
+0000e800: 7479 7065 5d0a 2020 2020 2020 2020 2020  type].          
+0000e810: 2020 6e73 6d61 703d 786d 6c5f 6e61 6d65    nsmap=xml_name
+0000e820: 7370 6163 655f 6d61 702c 0a20 2020 2020  space_map,.     
+0000e830: 2020 2029 0a20 2020 2020 2020 2076 616c     ).        val
+0000e840: 7565 5f2e 7465 7874 203d 2073 7472 2876  ue_.text = str(v
+0000e850: 616c 2e76 616c 7565 290a 2020 2020 2020  al.value).      
+0000e860: 2020 7072 6f70 5f2e 6170 7065 6e64 2876    prop_.append(v
+0000e870: 616c 7565 5f29 0a0a 2020 2020 7265 7475  alue_)..    retu
+0000e880: 726e 2070 726f 705f 0a0a 0a64 6566 206d  rn prop_...def m
+0000e890: 616b 655f 7572 695f 7072 6f70 280a 2020  ake_uri_prop(.  
+0000e8a0: 2020 6e61 6d65 3a20 7374 722c 0a20 2020    name: str,.   
+0000e8b0: 2076 616c 7565 3a20 556e 696f 6e5b 5072   value: Union[Pr
+0000e8c0: 6f70 6572 7479 456c 656d 656e 742c 2073  opertyElement, s
+0000e8d0: 7472 2c20 4974 6572 6162 6c65 5b55 6e69  tr, Iterable[Uni
+0000e8e0: 6f6e 5b50 726f 7065 7274 7945 6c65 6d65  on[PropertyEleme
+0000e8f0: 6e74 2c20 7374 725d 5d5d 2c0a 2020 2020  nt, str]]],.    
+0000e900: 6361 6c6c 696e 675f 7265 736f 7572 6365  calling_resource
+0000e910: 3a20 7374 7220 3d20 2222 2c0a 2920 2d3e  : str = "",.) ->
+0000e920: 2065 7472 6565 2e5f 456c 656d 656e 743a   etree._Element:
+0000e930: 0a20 2020 2022 2222 0a20 2020 204d 616b  .    """.    Mak
+0000e940: 6520 616e 203c 7572 692d 7072 6f70 3e20  e an <uri-prop> 
+0000e950: 6672 6f6d 206f 6e65 206f 7220 6d6f 7265  from one or more
+0000e960: 2055 5249 732e 2054 6865 2055 5249 2873   URIs. The URI(s
+0000e970: 2920 6361 6e20 6265 2070 726f 7669 6465  ) can be provide
+0000e980: 6420 6173 2073 7472 696e 6720 6f72 2061  d as string or a
+0000e990: 7320 5072 6f70 6572 7479 456c 656d 656e  s PropertyElemen
+0000e9a0: 7420 7769 7468 2061 2073 7472 696e 670a  t with a string.
+0000e9b0: 2020 2020 696e 7369 6465 2e20 4966 2070      inside. If p
+0000e9c0: 726f 7669 6465 6420 6173 2073 7472 696e  rovided as strin
+0000e9d0: 672c 2074 6865 2070 6572 6d69 7373 696f  g, the permissio
+0000e9e0: 6e73 2064 6566 6175 6c74 2074 6f20 2270  ns default to "p
+0000e9f0: 726f 702d 6465 6661 756c 7422 2e0a 0a20  rop-default"... 
+0000ea00: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0000ea10: 206e 616d 653a 2074 6865 206e 616d 6520   name: the name 
+0000ea20: 6f66 2074 6869 7320 7072 6f70 6572 7479  of this property
+0000ea30: 2061 7320 6465 6669 6e65 6420 696e 2074   as defined in t
+0000ea40: 6865 206f 6e74 6f0a 2020 2020 2020 2020  he onto.        
+0000ea50: 7661 6c75 653a 206f 6e65 206f 7220 6d6f  value: one or mo
+0000ea60: 7265 2055 5249 732c 2061 7320 7374 7269  re URIs, as stri
+0000ea70: 6e67 2f50 726f 7065 7274 7945 6c65 6d65  ng/PropertyEleme
+0000ea80: 6e74 2c20 6f72 2061 7320 6974 6572 6162  nt, or as iterab
+0000ea90: 6c65 206f 6620 7374 7269 6e67 732f 5072  le of strings/Pr
+0000eaa0: 6f70 6572 7479 456c 656d 656e 7473 0a20  opertyElements. 
+0000eab0: 2020 2020 2020 2063 616c 6c69 6e67 5f72         calling_r
+0000eac0: 6573 6f75 7263 653a 2074 6865 206e 616d  esource: the nam
+0000ead0: 6520 6f66 2074 6865 2070 6172 656e 7420  e of the parent 
+0000eae0: 7265 736f 7572 6365 2028 666f 7220 6265  resource (for be
+0000eaf0: 7474 6572 2065 7272 6f72 206d 6573 7361  tter error messa
+0000eb00: 6765 7329 0a0a 2020 2020 5761 726e 733a  ges)..    Warns:
+0000eb10: 0a20 2020 2020 2020 2049 6620 6f6e 6520  .        If one 
+0000eb20: 6f66 2074 6865 2076 616c 7565 7320 6973  of the values is
+0000eb30: 206e 6f74 2061 2076 616c 6964 2055 5249   not a valid URI
+0000eb40: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
+0000eb50: 2020 2020 2020 2061 6e20 6574 7265 652e         an etree.
+0000eb60: 5f45 6c65 6d65 6e74 2074 6861 7420 6361  _Element that ca
+0000eb70: 6e20 6265 2061 7070 656e 6465 6420 746f  n be appended to
+0000eb80: 2074 6865 2070 6172 656e 7420 7265 736f   the parent reso
+0000eb90: 7572 6365 2077 6974 6820 7265 736f 7572  urce with resour
+0000eba0: 6365 2e61 7070 656e 6428 6d61 6b65 5f2a  ce.append(make_*
+0000ebb0: 5f70 726f 7028 2e2e 2e29 290a 0a20 2020  _prop(...))..   
+0000ebc0: 2045 7861 6d70 6c65 733a 0a20 2020 2020   Examples:.     
+0000ebd0: 2020 203e 3e3e 2065 7863 656c 3278 6d6c     >>> excel2xml
+0000ebe0: 2e6d 616b 655f 7572 695f 7072 6f70 2822  .make_uri_prop("
+0000ebf0: 3a74 6573 7470 726f 7065 7274 7922 2c20  :testproperty", 
+0000ec00: 2277 7777 2e74 6573 742e 636f 6d22 290a  "www.test.com").
+0000ec10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec20: 3c75 7269 2d70 726f 7020 6e61 6d65 3d22  <uri-prop name="
+0000ec30: 3a74 6573 7470 726f 7065 7274 7922 3e0a  :testproperty">.
+0000ec40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec50: 2020 2020 3c75 7269 2070 6572 6d69 7373      <uri permiss
+0000ec60: 696f 6e73 3d22 7072 6f70 2d64 6566 6175  ions="prop-defau
+0000ec70: 6c74 223e 7777 772e 7465 7374 2e63 6f6d  lt">www.test.com
+0000ec80: 3c2f 7572 693e 0a20 2020 2020 2020 2020  </uri>.         
+0000ec90: 2020 2020 2020 203c 2f75 7269 2d70 726f         </uri-pro
+0000eca0: 703e 0a20 2020 2020 2020 203e 3e3e 2065  p>.        >>> e
+0000ecb0: 7863 656c 3278 6d6c 2e6d 616b 655f 7572  xcel2xml.make_ur
+0000ecc0: 695f 7072 6f70 2822 3a74 6573 7470 726f  i_prop(":testpro
+0000ecd0: 7065 7274 7922 2c20 6578 6365 6c32 786d  perty", excel2xm
+0000ece0: 6c2e 5072 6f70 6572 7479 456c 656d 656e  l.PropertyElemen
+0000ecf0: 7428 2277 7777 2e74 6573 742e 636f 6d22  t("www.test.com"
+0000ed00: 2c20 7065 726d 6973 7369 6f6e 733d 2270  , permissions="p
+0000ed10: 726f 702d 7265 7374 7269 6374 6564 222c  rop-restricted",
+0000ed20: 2063 6f6d 6d65 6e74 3d22 6578 616d 706c   comment="exampl
+0000ed30: 6522 2929 0a20 2020 2020 2020 2020 2020  e")).           
+0000ed40: 2020 2020 203c 7572 692d 7072 6f70 206e       <uri-prop n
+0000ed50: 616d 653d 223a 7465 7374 7072 6f70 6572  ame=":testproper
+0000ed60: 7479 223e 0a20 2020 2020 2020 2020 2020  ty">.           
+0000ed70: 2020 2020 2020 2020 203c 7572 6920 7065           <uri pe
+0000ed80: 726d 6973 7369 6f6e 733d 2270 726f 702d  rmissions="prop-
+0000ed90: 7265 7374 7269 6374 6564 2220 636f 6d6d  restricted" comm
+0000eda0: 656e 743d 2265 7861 6d70 6c65 223e 7777  ent="example">ww
+0000edb0: 772e 7465 7374 2e63 6f6d 3c2f 7572 693e  w.test.com</uri>
+0000edc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000edd0: 203c 2f75 7269 2d70 726f 703e 0a20 2020   </uri-prop>.   
+0000ede0: 2020 2020 203e 3e3e 2065 7863 656c 3278       >>> excel2x
+0000edf0: 6d6c 2e6d 616b 655f 7572 695f 7072 6f70  ml.make_uri_prop
+0000ee00: 2822 3a74 6573 7470 726f 7065 7274 7922  (":testproperty"
+0000ee10: 2c20 5b22 7777 772e 312e 636f 6d22 2c20  , ["www.1.com", 
+0000ee20: 2277 7777 2e32 2e63 6f6d 225d 290a 2020  "www.2.com"]).  
+0000ee30: 2020 2020 2020 2020 2020 2020 2020 3c75                <u
+0000ee40: 7269 2d70 726f 7020 6e61 6d65 3d22 3a74  ri-prop name=":t
+0000ee50: 6573 7470 726f 7065 7274 7922 3e0a 2020  estproperty">.  
+0000ee60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee70: 2020 3c75 7269 2070 6572 6d69 7373 696f    <uri permissio
+0000ee80: 6e73 3d22 7072 6f70 2d64 6566 6175 6c74  ns="prop-default
+0000ee90: 223e 7777 772e 312e 636f 6d3c 2f75 7269  ">www.1.com</uri
+0000eea0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+0000eeb0: 2020 2020 2020 3c75 7269 2070 6572 6d69        <uri permi
+0000eec0: 7373 696f 6e73 3d22 7072 6f70 2d64 6566  ssions="prop-def
+0000eed0: 6175 6c74 223e 7777 772e 322e 636f 6d3c  ault">www.2.com<
+0000eee0: 2f75 7269 3e0a 2020 2020 2020 2020 2020  /uri>.          
+0000eef0: 2020 2020 2020 3c2f 7572 692d 7072 6f70        </uri-prop
+0000ef00: 3e0a 0a20 2020 2053 6565 2068 7474 7073  >..    See https
+0000ef10: 3a2f 2f64 6f63 732e 6461 7363 682e 7377  ://docs.dasch.sw
+0000ef20: 6973 732f 6c61 7465 7374 2f44 5350 2d54  iss/latest/DSP-T
+0000ef30: 4f4f 4c53 2f66 696c 652d 666f 726d 6174  OOLS/file-format
+0000ef40: 732f 786d 6c2d 6461 7461 2d66 696c 652f  s/xml-data-file/
+0000ef50: 2375 7269 2d70 726f 700a 2020 2020 2222  #uri-prop.    ""
+0000ef60: 220a 0a20 2020 2023 2063 6865 636b 2074  "..    # check t
+0000ef70: 6865 2069 6e70 7574 3a20 7072 6570 6172  he input: prepar
+0000ef80: 6520 6120 6c69 7374 2077 6974 6820 7661  e a list with va
+0000ef90: 6c69 6420 7661 6c75 6573 0a20 2020 2076  lid values.    v
+0000efa0: 616c 7565 7320 3d20 7072 6570 6172 655f  alues = prepare_
+0000efb0: 7661 6c75 6528 7661 6c75 6529 0a0a 2020  value(value)..  
+0000efc0: 2020 2320 6368 6563 6b20 7661 6c75 6520    # check value 
+0000efd0: 7479 7065 0a20 2020 2066 6f72 2076 616c  type.    for val
+0000efe0: 2069 6e20 7661 6c75 6573 3a0a 2020 2020   in values:.    
+0000eff0: 2020 2020 6966 206e 6f74 2069 735f 7572      if not is_ur
+0000f000: 6928 7374 7228 7661 6c2e 7661 6c75 6529  i(str(val.value)
+0000f010: 293a 0a20 2020 2020 2020 2020 2020 206d  ):.            m
+0000f020: 7367 203d 2028 0a20 2020 2020 2020 2020  sg = (.         
+0000f030: 2020 2020 2020 2066 2246 6169 6c65 6420         f"Failed 
+0000f040: 7661 6c69 6461 7469 6f6e 2069 6e20 7265  validation in re
+0000f050: 736f 7572 6365 2027 7b63 616c 6c69 6e67  source '{calling
+0000f060: 5f72 6573 6f75 7263 657d 272c 2070 726f  _resource}', pro
+0000f070: 7065 7274 7920 277b 6e61 6d65 7d27 3a20  perty '{name}': 
+0000f080: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000f090: 2020 6622 277b 7661 6c2e 7661 6c75 657d    f"'{val.value}
+0000f0a0: 2720 6973 206e 6f74 2061 2076 616c 6964  ' is not a valid
+0000f0b0: 2055 5249 2e22 0a20 2020 2020 2020 2020   URI.".         
+0000f0c0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000f0d0: 2077 6172 6e69 6e67 732e 7761 726e 2844   warnings.warn(D
+0000f0e0: 7370 546f 6f6c 7355 7365 7257 6172 6e69  spToolsUserWarni
+0000f0f0: 6e67 286d 7367 2929 0a0a 2020 2020 2320  ng(msg))..    # 
+0000f100: 6d61 6b65 2078 6d6c 2073 7472 7563 7475  make xml structu
+0000f110: 7265 206f 6620 7468 6520 7661 6c69 6420  re of the valid 
+0000f120: 7661 6c75 6573 0a20 2020 2070 726f 705f  values.    prop_
+0000f130: 203d 2065 7472 6565 2e45 6c65 6d65 6e74   = etree.Element
+0000f140: 280a 2020 2020 2020 2020 227b 2573 7d75  (.        "{%s}u
+0000f150: 7269 2d70 726f 7022 2025 2078 6d6c 5f6e  ri-prop" % xml_n
+0000f160: 616d 6573 7061 6365 5f6d 6170 5b4e 6f6e  amespace_map[Non
+0000f170: 655d 2c0a 2020 2020 2020 2020 6e61 6d65  e],.        name
+0000f180: 3d6e 616d 652c 0a20 2020 2020 2020 206e  =name,.        n
+0000f190: 736d 6170 3d78 6d6c 5f6e 616d 6573 7061  smap=xml_namespa
+0000f1a0: 6365 5f6d 6170 2c0a 2020 2020 290a 2020  ce_map,.    ).  
+0000f1b0: 2020 666f 7220 7661 6c20 696e 2076 616c    for val in val
+0000f1c0: 7565 733a 0a20 2020 2020 2020 206b 7761  ues:.        kwa
+0000f1d0: 7267 7320 3d20 7b22 7065 726d 6973 7369  rgs = {"permissi
+0000f1e0: 6f6e 7322 3a20 7661 6c2e 7065 726d 6973  ons": val.permis
+0000f1f0: 7369 6f6e 737d 0a20 2020 2020 2020 2069  sions}.        i
+0000f200: 6620 7661 6c2e 636f 6d6d 656e 7420 616e  f val.comment an
+0000f210: 6420 6368 6563 6b5f 6e6f 746e 6128 7661  d check_notna(va
+0000f220: 6c2e 636f 6d6d 656e 7429 3a0a 2020 2020  l.comment):.    
+0000f230: 2020 2020 2020 2020 6b77 6172 6773 5b22          kwargs["
+0000f240: 636f 6d6d 656e 7422 5d20 3d20 7661 6c2e  comment"] = val.
+0000f250: 636f 6d6d 656e 740a 2020 2020 2020 2020  comment.        
+0000f260: 7661 6c75 655f 203d 2065 7472 6565 2e45  value_ = etree.E
+0000f270: 6c65 6d65 6e74 280a 2020 2020 2020 2020  lement(.        
+0000f280: 2020 2020 227b 2573 7d75 7269 2220 2520      "{%s}uri" % 
+0000f290: 786d 6c5f 6e61 6d65 7370 6163 655f 6d61  xml_namespace_ma
+0000f2a0: 705b 4e6f 6e65 5d2c 0a20 2020 2020 2020  p[None],.       
+0000f2b0: 2020 2020 202a 2a6b 7761 7267 732c 2020       **kwargs,  
+0000f2c0: 2320 7479 7065 3a20 6967 6e6f 7265 5b61  # type: ignore[a
+0000f2d0: 7267 2d74 7970 655d 0a20 2020 2020 2020  rg-type].       
+0000f2e0: 2020 2020 206e 736d 6170 3d78 6d6c 5f6e       nsmap=xml_n
+0000f2f0: 616d 6573 7061 6365 5f6d 6170 2c0a 2020  amespace_map,.  
+0000f300: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000f310: 7661 6c75 655f 2e74 6578 7420 3d20 7374  value_.text = st
+0000f320: 7228 7661 6c2e 7661 6c75 6529 0a20 2020  r(val.value).   
+0000f330: 2020 2020 2070 726f 705f 2e61 7070 656e       prop_.appen
+0000f340: 6428 7661 6c75 655f 290a 0a20 2020 2072  d(value_)..    r
+0000f350: 6574 7572 6e20 7072 6f70 5f0a 0a0a 6465  eturn prop_...de
+0000f360: 6620 6d61 6b65 5f72 6567 696f 6e28 2020  f make_region(  
+0000f370: 2320 6e6f 7161 3a20 4434 3137 2028 756e  # noqa: D417 (un
+0000f380: 646f 6375 6d65 6e74 6564 2d70 6172 616d  documented-param
+0000f390: 290a 2020 2020 6c61 6265 6c3a 2073 7472  ).    label: str
+0000f3a0: 2c0a 2020 2020 6964 3a20 7374 722c 0a20  ,.    id: str,. 
+0000f3b0: 2020 2070 6572 6d69 7373 696f 6e73 3a20     permissions: 
+0000f3c0: 7374 7220 3d20 2272 6573 2d64 6566 6175  str = "res-defau
+0000f3d0: 6c74 222c 0a20 2020 2061 726b 3a20 4f70  lt",.    ark: Op
+0000f3e0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+0000f3f0: 6e65 2c0a 2020 2020 6972 693a 204f 7074  ne,.    iri: Opt
+0000f400: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+0000f410: 652c 0a20 2020 2063 7265 6174 696f 6e5f  e,.    creation_
+0000f420: 6461 7465 3a20 4f70 7469 6f6e 616c 5b73  date: Optional[s
+0000f430: 7472 5d20 3d20 4e6f 6e65 2c0a 2920 2d3e  tr] = None,.) ->
+0000f440: 2065 7472 6565 2e5f 456c 656d 656e 743a   etree._Element:
+0000f450: 0a20 2020 2022 2222 0a20 2020 2043 7265  .    """.    Cre
+0000f460: 6174 6573 2061 6e20 656d 7074 7920 7265  ates an empty re
+0000f470: 6769 6f6e 2065 6c65 6d65 6e74 2c20 7769  gion element, wi
+0000f480: 7468 2074 6865 2061 7474 7269 6275 7465  th the attribute
+0000f490: 7320 6173 2073 7065 6369 6669 6564 2062  s as specified b
+0000f4a0: 7920 7468 6520 6172 6775 6d65 6e74 730a  y the arguments.
+0000f4b0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
+0000f4c0: 2020 2054 6865 2061 7267 756d 656e 7473     The arguments
+0000f4d0: 2063 6f72 7265 7370 6f6e 6420 313a 3120   correspond 1:1 
+0000f4e0: 746f 2074 6865 2061 7474 7269 6275 7465  to the attribute
+0000f4f0: 7320 6f66 2074 6865 203c 7265 6769 6f6e  s of the <region
+0000f500: 3e20 656c 656d 656e 742e 0a0a 2020 2020  > element...    
+0000f510: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
+0000f520: 5761 726e 696e 673a 2069 6620 626f 7468  Warning: if both
+0000f530: 2061 6e20 4152 4b20 616e 6420 616e 2049   an ARK and an I
+0000f540: 5249 2061 7265 2070 726f 7669 6465 640a  RI are provided.
+0000f550: 2020 2020 2020 2020 4261 7365 4572 726f          BaseErro
+0000f560: 723a 2069 6620 7468 6520 6372 6561 7469  r: if the creati
+0000f570: 6f6e 2064 6174 6520 6973 2069 6e76 616c  on date is inval
+0000f580: 6964 0a0a 2020 2020 5265 7475 726e 733a  id..    Returns:
+0000f590: 0a20 2020 2020 2020 2054 6865 2072 6567  .        The reg
+0000f5a0: 696f 6e20 656c 656d 656e 742c 2077 6974  ion element, wit
+0000f5b0: 686f 7574 2061 6e79 2063 6869 6c64 7265  hout any childre
+0000f5c0: 6e2c 2062 7574 2077 6974 6820 7468 6520  n, but with the 
+0000f5d0: 6174 7472 6962 7574 6573 3a0a 2020 2020  attributes:.    
+0000f5e0: 2020 2020 3c72 6567 696f 6e20 6c61 6265      <region labe
+0000f5f0: 6c3d 6c61 6265 6c20 6964 3d69 6420 7065  l=label id=id pe
+0000f600: 726d 6973 7369 6f6e 733d 7065 726d 6973  rmissions=permis
+0000f610: 7369 6f6e 7320 6172 6b3d 6172 6b20 6972  sions ark=ark ir
+0000f620: 693d 6972 693e 3c2f 7265 6769 6f6e 3e0a  i=iri></region>.
+0000f630: 0a20 2020 2045 7861 6d70 6c65 733a 0a20  .    Examples:. 
+0000f640: 2020 2020 2020 203e 3e3e 2072 6567 696f         >>> regio
+0000f650: 6e20 3d20 6578 6365 6c32 786d 6c2e 6d61  n = excel2xml.ma
+0000f660: 6b65 5f72 6567 696f 6e28 226c 6162 656c  ke_region("label
+0000f670: 222c 2022 6964 2229 0a20 2020 2020 2020  ", "id").       
+0000f680: 203e 3e3e 2072 6567 696f 6e2e 6170 7065   >>> region.appe
+0000f690: 6e64 2865 7863 656c 3278 6d6c 2e6d 616b  nd(excel2xml.mak
+0000f6a0: 655f 7465 7874 5f70 726f 7028 2268 6173  e_text_prop("has
+0000f6b0: 436f 6d6d 656e 7422 2c20 2254 6869 7320  Comment", "This 
+0000f6c0: 6973 2061 2063 6f6d 6d65 6e74 2229 290a  is a comment")).
+0000f6d0: 2020 2020 2020 2020 3e3e 3e20 7265 6769          >>> regi
+0000f6e0: 6f6e 2e61 7070 656e 6428 6578 6365 6c32  on.append(excel2
+0000f6f0: 786d 6c2e 6d61 6b65 5f63 6f6c 6f72 5f70  xml.make_color_p
+0000f700: 726f 7028 2268 6173 436f 6c6f 7222 2c20  rop("hasColor", 
+0000f710: 2223 3564 3166 3165 2229 290a 2020 2020  "#5d1f1e")).    
+0000f720: 2020 2020 3e3e 3e20 7265 6769 6f6e 2e61      >>> region.a
+0000f730: 7070 656e 6428 6578 6365 6c32 786d 6c2e  ppend(excel2xml.
+0000f740: 6d61 6b65 5f72 6573 7074 725f 7072 6f70  make_resptr_prop
+0000f750: 2822 6973 5265 6769 6f6e 4f66 222c 2022  ("isRegionOf", "
+0000f760: 696d 6167 655f 3022 2929 0a20 2020 2020  image_0")).     
+0000f770: 2020 203e 3e3e 2072 6567 696f 6e2e 6170     >>> region.ap
+0000f780: 7065 6e64 2865 7863 656c 3278 6d6c 2e6d  pend(excel2xml.m
+0000f790: 616b 655f 6765 6f6d 6574 7279 5f70 726f  ake_geometry_pro
+0000f7a0: 7028 2268 6173 4765 6f6d 6574 7279 222c  p("hasGeometry",
+0000f7b0: 2022 7b2e 2e2e 7d22 2929 0a20 2020 2020   "{...}")).     
+0000f7c0: 2020 203e 3e3e 2072 6f6f 742e 6170 7065     >>> root.appe
+0000f7d0: 6e64 2872 6567 696f 6e29 0a0a 2020 2020  nd(region)..    
+0000f7e0: 5365 6520 6874 7470 733a 2f2f 646f 6373  See https://docs
+0000f7f0: 2e64 6173 6368 2e73 7769 7373 2f6c 6174  .dasch.swiss/lat
+0000f800: 6573 742f 4453 502d 544f 4f4c 532f 6669  est/DSP-TOOLS/fi
+0000f810: 6c65 2d66 6f72 6d61 7473 2f78 6d6c 2d64  le-formats/xml-d
+0000f820: 6174 612d 6669 6c65 2f23 7265 6769 6f6e  ata-file/#region
+0000f830: 0a20 2020 2022 2222 0a0a 2020 2020 6b77  .    """..    kw
+0000f840: 6172 6773 203d 207b 226c 6162 656c 223a  args = {"label":
+0000f850: 206c 6162 656c 2c20 2269 6422 3a20 6964   label, "id": id
+0000f860: 2c20 2270 6572 6d69 7373 696f 6e73 223a  , "permissions":
+0000f870: 2070 6572 6d69 7373 696f 6e73 2c20 226e   permissions, "n
+0000f880: 736d 6170 223a 2078 6d6c 5f6e 616d 6573  smap": xml_names
+0000f890: 7061 6365 5f6d 6170 7d0a 2020 2020 6966  pace_map}.    if
+0000f8a0: 2061 726b 3a0a 2020 2020 2020 2020 6b77   ark:.        kw
+0000f8b0: 6172 6773 5b22 6172 6b22 5d20 3d20 6172  args["ark"] = ar
+0000f8c0: 6b0a 2020 2020 6966 2069 7269 3a0a 2020  k.    if iri:.  
+0000f8d0: 2020 2020 2020 6b77 6172 6773 5b22 6972        kwargs["ir
+0000f8e0: 6922 5d20 3d20 6972 690a 2020 2020 6966  i"] = iri.    if
+0000f8f0: 2061 726b 2061 6e64 2069 7269 3a0a 2020   ark and iri:.  
+0000f900: 2020 2020 2020 6d73 6720 3d20 6622 426f        msg = f"Bo
+0000f910: 7468 2041 524b 2061 6e64 2049 5249 2077  th ARK and IRI w
+0000f920: 6572 6520 7072 6f76 6964 6564 2066 6f72  ere provided for
+0000f930: 2072 6573 6f75 7263 6520 277b 6c61 6265   resource '{labe
+0000f940: 6c7d 2720 287b 6964 7d29 2e20 5468 6520  l}' ({id}). The 
+0000f950: 4152 4b20 7769 6c6c 206f 7665 7272 6964  ARK will overrid
+0000f960: 6520 7468 6520 4952 492e 220a 2020 2020  e the IRI.".    
+0000f970: 2020 2020 7761 726e 696e 6773 2e77 6172      warnings.war
+0000f980: 6e28 4473 7054 6f6f 6c73 5573 6572 5761  n(DspToolsUserWa
+0000f990: 726e 696e 6728 6d73 6729 290a 2020 2020  rning(msg)).    
+0000f9a0: 6966 2063 7265 6174 696f 6e5f 6461 7465  if creation_date
+0000f9b0: 3a0a 2020 2020 2020 2020 7472 793a 0a20  :.        try:. 
+0000f9c0: 2020 2020 2020 2020 2020 2044 6174 6554             DateT
+0000f9d0: 696d 6553 7461 6d70 2863 7265 6174 696f  imeStamp(creatio
+0000f9e0: 6e5f 6461 7465 290a 2020 2020 2020 2020  n_date).        
+0000f9f0: 6578 6365 7074 2042 6173 6545 7272 6f72  except BaseError
+0000fa00: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+0000fa10: 6973 6520 4261 7365 4572 726f 7228 0a20  ise BaseError(. 
+0000fa20: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000fa30: 2254 6865 2072 6567 696f 6e20 277b 6c61  "The region '{la
+0000fa40: 6265 6c7d 2720 2849 443a 207b 6964 7d29  bel}' (ID: {id})
+0000fa50: 2068 6173 2061 6e20 696e 7661 6c69 6420   has an invalid 
+0000fa60: 6372 6561 7469 6f6e 2064 6174 6520 277b  creation date '{
+0000fa70: 6372 6561 7469 6f6e 5f64 6174 657d 272e  creation_date}'.
+0000fa80: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+0000fa90: 2020 2066 2244 6964 2079 6f75 2070 6572     f"Did you per
+0000faa0: 6861 7073 2066 6f72 6765 7420 7468 6520  haps forget the 
+0000fab0: 7469 6d65 7a6f 6e65 3f22 0a20 2020 2020  timezone?".     
+0000fac0: 2020 2020 2020 2029 2066 726f 6d20 4e6f         ) from No
+0000fad0: 6e65 0a20 2020 2020 2020 206b 7761 7267  ne.        kwarg
+0000fae0: 735b 2263 7265 6174 696f 6e5f 6461 7465  s["creation_date
+0000faf0: 225d 203d 2063 7265 6174 696f 6e5f 6461  "] = creation_da
+0000fb00: 7465 0a0a 2020 2020 7265 7475 726e 2065  te..    return e
+0000fb10: 7472 6565 2e45 6c65 6d65 6e74 280a 2020  tree.Element(.  
+0000fb20: 2020 2020 2020 227b 2573 7d72 6567 696f        "{%s}regio
+0000fb30: 6e22 2025 2078 6d6c 5f6e 616d 6573 7061  n" % xml_namespa
+0000fb40: 6365 5f6d 6170 5b4e 6f6e 655d 2c0a 2020  ce_map[None],.  
+0000fb50: 2020 2020 2020 2a2a 6b77 6172 6773 2c20        **kwargs, 
+0000fb60: 2023 2074 7970 653a 2069 676e 6f72 655b   # type: ignore[
+0000fb70: 6172 672d 7479 7065 5d0a 2020 2020 290a  arg-type].    ).
+0000fb80: 0a0a 6465 6620 6d61 6b65 5f61 6e6e 6f74  ..def make_annot
+0000fb90: 6174 696f 6e28 2020 2320 6e6f 7161 3a20  ation(  # noqa: 
+0000fba0: 4434 3137 2028 756e 646f 6375 6d65 6e74  D417 (undocument
+0000fbb0: 6564 2d70 6172 616d 290a 2020 2020 6c61  ed-param).    la
+0000fbc0: 6265 6c3a 2073 7472 2c0a 2020 2020 6964  bel: str,.    id
+0000fbd0: 3a20 7374 722c 0a20 2020 2070 6572 6d69  : str,.    permi
+0000fbe0: 7373 696f 6e73 3a20 7374 7220 3d20 2272  ssions: str = "r
+0000fbf0: 6573 2d64 6566 6175 6c74 222c 0a20 2020  es-default",.   
+0000fc00: 2061 726b 3a20 4f70 7469 6f6e 616c 5b73   ark: Optional[s
+0000fc10: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+0000fc20: 6972 693a 204f 7074 696f 6e61 6c5b 7374  iri: Optional[st
+0000fc30: 725d 203d 204e 6f6e 652c 0a20 2020 2063  r] = None,.    c
+0000fc40: 7265 6174 696f 6e5f 6461 7465 3a20 4f70  reation_date: Op
+0000fc50: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+0000fc60: 6e65 2c0a 2920 2d3e 2065 7472 6565 2e5f  ne,.) -> etree._
+0000fc70: 456c 656d 656e 743a 0a20 2020 2022 2222  Element:.    """
+0000fc80: 0a20 2020 2043 7265 6174 6573 2061 6e20  .    Creates an 
+0000fc90: 656d 7074 7920 616e 6e6f 7461 7469 6f6e  empty annotation
+0000fca0: 2065 6c65 6d65 6e74 2c20 7769 7468 2074   element, with t
+0000fcb0: 6865 2061 7474 7269 6275 7465 7320 6173  he attributes as
+0000fcc0: 2073 7065 6369 6669 6564 2062 7920 7468   specified by th
+0000fcd0: 6520 6172 6775 6d65 6e74 730a 0a20 2020  e arguments..   
+0000fce0: 2041 7267 733a 0a20 2020 2020 2020 2054   Args:.        T
+0000fcf0: 6865 2061 7267 756d 656e 7473 2063 6f72  he arguments cor
+0000fd00: 7265 7370 6f6e 6420 313a 3120 746f 2074  respond 1:1 to t
+0000fd10: 6865 2061 7474 7269 6275 7465 7320 6f66  he attributes of
+0000fd20: 2074 6865 203c 616e 6e6f 7461 7469 6f6e   the <annotation
+0000fd30: 3e20 656c 656d 656e 742e 0a0a 2020 2020  > element...    
+0000fd40: 5261 6973 6573 3a0a 2020 2020 2020 2020  Raises:.        
+0000fd50: 5761 726e 696e 673a 2069 6620 626f 7468  Warning: if both
+0000fd60: 2061 6e20 4152 4b20 616e 6420 616e 2049   an ARK and an I
+0000fd70: 5249 2061 7265 2070 726f 7669 6465 640a  RI are provided.
+0000fd80: 2020 2020 2020 2020 4261 7365 4572 726f          BaseErro
+0000fd90: 723a 2069 6620 7468 6520 6372 6561 7469  r: if the creati
+0000fda0: 6f6e 2064 6174 6520 6973 2069 6e76 616c  on date is inval
+0000fdb0: 6964 0a0a 2020 2020 5265 7475 726e 733a  id..    Returns:
+0000fdc0: 0a20 2020 2020 2020 2054 6865 2061 6e6e  .        The ann
+0000fdd0: 6f74 6174 696f 6e20 656c 656d 656e 742c  otation element,
+0000fde0: 2077 6974 686f 7574 2061 6e79 2063 6869   without any chi
+0000fdf0: 6c64 7265 6e2c 2062 7574 2077 6974 6820  ldren, but with 
+0000fe00: 7468 6520 6174 7472 6962 7574 6573 3a0a  the attributes:.
+0000fe10: 2020 2020 2020 2020 3c61 6e6e 6f74 6174          <annotat
+0000fe20: 696f 6e20 6c61 6265 6c3d 6c61 6265 6c20  ion label=label 
+0000fe30: 6964 3d69 6420 7065 726d 6973 7369 6f6e  id=id permission
+0000fe40: 733d 7065 726d 6973 7369 6f6e 7320 6172  s=permissions ar
+0000fe50: 6b3d 6172 6b20 6972 693d 6972 693e 3c2f  k=ark iri=iri></
+0000fe60: 616e 6e6f 7461 7469 6f6e 3e0a 0a20 2020  annotation>..   
+0000fe70: 2045 7861 6d70 6c65 733a 0a20 2020 2020   Examples:.     
+0000fe80: 2020 203e 3e3e 2061 6e6e 6f74 6174 696f     >>> annotatio
+0000fe90: 6e20 3d20 6578 6365 6c32 786d 6c2e 6d61  n = excel2xml.ma
+0000fea0: 6b65 5f61 6e6e 6f74 6174 696f 6e28 226c  ke_annotation("l
+0000feb0: 6162 656c 222c 2022 6964 2229 0a20 2020  abel", "id").   
+0000fec0: 2020 2020 203e 3e3e 2061 6e6e 6f74 6174       >>> annotat
+0000fed0: 696f 6e2e 6170 7065 6e64 2865 7863 656c  ion.append(excel
+0000fee0: 3278 6d6c 2e6d 616b 655f 7465 7874 5f70  2xml.make_text_p
+0000fef0: 726f 7028 2268 6173 436f 6d6d 656e 7422  rop("hasComment"
+0000ff00: 2c20 2254 6869 7320 6973 2061 2063 6f6d  , "This is a com
+0000ff10: 6d65 6e74 2229 290a 2020 2020 2020 2020  ment")).        
+0000ff20: 3e3e 3e20 616e 6e6f 7461 7469 6f6e 2e61  >>> annotation.a
+0000ff30: 7070 656e 6428 6578 6365 6c32 786d 6c2e  ppend(excel2xml.
+0000ff40: 6d61 6b65 5f72 6573 7074 725f 7072 6f70  make_resptr_prop
+0000ff50: 2822 6973 416e 6e6f 7461 7469 6f6e 4f66  ("isAnnotationOf
+0000ff60: 222c 2022 7265 736f 7572 6365 5f30 2229  ", "resource_0")
+0000ff70: 290a 2020 2020 2020 2020 3e3e 3e20 726f  ).        >>> ro
+0000ff80: 6f74 2e61 7070 656e 6428 616e 6e6f 7461  ot.append(annota
+0000ff90: 7469 6f6e 290a 0a20 2020 2053 6565 2068  tion)..    See h
+0000ffa0: 7474 7073 3a2f 2f64 6f63 732e 6461 7363  ttps://docs.dasc
+0000ffb0: 682e 7377 6973 732f 6c61 7465 7374 2f44  h.swiss/latest/D
+0000ffc0: 5350 2d54 4f4f 4c53 2f66 696c 652d 666f  SP-TOOLS/file-fo
+0000ffd0: 726d 6174 732f 786d 6c2d 6461 7461 2d66  rmats/xml-data-f
+0000ffe0: 696c 652f 2361 6e6e 6f74 6174 696f 6e0a  ile/#annotation.
+0000fff0: 2020 2020 2222 220a 0a20 2020 206b 7761      """..    kwa
+00010000: 7267 7320 3d20 7b22 6c61 6265 6c22 3a20  rgs = {"label": 
+00010010: 6c61 6265 6c2c 2022 6964 223a 2069 642c  label, "id": id,
+00010020: 2022 7065 726d 6973 7369 6f6e 7322 3a20   "permissions": 
+00010030: 7065 726d 6973 7369 6f6e 732c 2022 6e73  permissions, "ns
+00010040: 6d61 7022 3a20 786d 6c5f 6e61 6d65 7370  map": xml_namesp
+00010050: 6163 655f 6d61 707d 0a20 2020 2069 6620  ace_map}.    if 
+00010060: 6172 6b3a 0a20 2020 2020 2020 206b 7761  ark:.        kwa
+00010070: 7267 735b 2261 726b 225d 203d 2061 726b  rgs["ark"] = ark
+00010080: 0a20 2020 2069 6620 6972 693a 0a20 2020  .    if iri:.   
+00010090: 2020 2020 206b 7761 7267 735b 2269 7269       kwargs["iri
+000100a0: 225d 203d 2069 7269 0a20 2020 2069 6620  "] = iri.    if 
+000100b0: 6172 6b20 616e 6420 6972 693a 0a20 2020  ark and iri:.   
+000100c0: 2020 2020 2077 6172 6e69 6e67 203d 2066       warning = f
+000100d0: 2242 6f74 6820 4152 4b20 616e 6420 4952  "Both ARK and IR
+000100e0: 4920 7765 7265 2070 726f 7669 6465 6420  I were provided 
+000100f0: 666f 7220 7265 736f 7572 6365 2027 7b6c  for resource '{l
+00010100: 6162 656c 7d27 2028 7b69 647d 292e 2054  abel}' ({id}). T
+00010110: 6865 2041 524b 2077 696c 6c20 6f76 6572  he ARK will over
+00010120: 7269 6465 2074 6865 2049 5249 2e22 0a20  ride the IRI.". 
+00010130: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
+00010140: 7761 726e 2844 7370 546f 6f6c 7355 7365  warn(DspToolsUse
+00010150: 7257 6172 6e69 6e67 2877 6172 6e69 6e67  rWarning(warning
+00010160: 2929 0a20 2020 2069 6620 6372 6561 7469  )).    if creati
+00010170: 6f6e 5f64 6174 653a 0a20 2020 2020 2020  on_date:.       
+00010180: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00010190: 2020 4461 7465 5469 6d65 5374 616d 7028    DateTimeStamp(
+000101a0: 6372 6561 7469 6f6e 5f64 6174 6529 0a20  creation_date). 
+000101b0: 2020 2020 2020 2065 7863 6570 7420 4261         except Ba
+000101c0: 7365 4572 726f 723a 0a20 2020 2020 2020  seError:.       
+000101d0: 2020 2020 2072 6169 7365 2042 6173 6545       raise BaseE
+000101e0: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+000101f0: 2020 2020 2020 6622 5468 6520 616e 6e6f        f"The anno
+00010200: 7461 7469 6f6e 2027 7b6c 6162 656c 7d27  tation '{label}'
+00010210: 2028 4944 3a20 7b69 647d 2920 6861 7320   (ID: {id}) has 
+00010220: 616e 2069 6e76 616c 6964 2063 7265 6174  an invalid creat
+00010230: 696f 6e20 6461 7465 2027 7b63 7265 6174  ion date '{creat
+00010240: 696f 6e5f 6461 7465 7d27 2e20 220a 2020  ion_date}'. ".  
+00010250: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00010260: 4469 6420 796f 7520 7065 7268 6170 7320  Did you perhaps 
+00010270: 666f 7267 6574 2074 6865 2074 696d 657a  forget the timez
+00010280: 6f6e 653f 220a 2020 2020 2020 2020 2020  one?".          
+00010290: 2020 2920 6672 6f6d 204e 6f6e 650a 2020    ) from None.  
+000102a0: 2020 2020 2020 6b77 6172 6773 5b22 6372        kwargs["cr
+000102b0: 6561 7469 6f6e 5f64 6174 6522 5d20 3d20  eation_date"] = 
+000102c0: 6372 6561 7469 6f6e 5f64 6174 650a 0a20  creation_date.. 
+000102d0: 2020 2072 6574 7572 6e20 6574 7265 652e     return etree.
+000102e0: 456c 656d 656e 7428 0a20 2020 2020 2020  Element(.       
+000102f0: 2022 7b25 737d 616e 6e6f 7461 7469 6f6e   "{%s}annotation
+00010300: 2220 2520 786d 6c5f 6e61 6d65 7370 6163  " % xml_namespac
+00010310: 655f 6d61 705b 4e6f 6e65 5d2c 0a20 2020  e_map[None],.   
+00010320: 2020 2020 202a 2a6b 7761 7267 732c 2020       **kwargs,  
+00010330: 2320 7479 7065 3a20 6967 6e6f 7265 5b61  # type: ignore[a
+00010340: 7267 2d74 7970 655d 0a20 2020 2029 0a0a  rg-type].    )..
+00010350: 0a64 6566 206d 616b 655f 6c69 6e6b 2820  .def make_link( 
+00010360: 2023 206e 6f71 613a 2044 3431 3720 2875   # noqa: D417 (u
+00010370: 6e64 6f63 756d 656e 7465 642d 7061 7261  ndocumented-para
+00010380: 6d29 0a20 2020 206c 6162 656c 3a20 7374  m).    label: st
+00010390: 722c 0a20 2020 2069 643a 2073 7472 2c0a  r,.    id: str,.
+000103a0: 2020 2020 7065 726d 6973 7369 6f6e 733a      permissions:
+000103b0: 2073 7472 203d 2022 7265 732d 6465 6661   str = "res-defa
+000103c0: 756c 7422 2c0a 2020 2020 6172 6b3a 204f  ult",.    ark: O
+000103d0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+000103e0: 6f6e 652c 0a20 2020 2069 7269 3a20 4f70  one,.    iri: Op
+000103f0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00010400: 6e65 2c0a 2020 2020 6372 6561 7469 6f6e  ne,.    creation
+00010410: 5f64 6174 653a 204f 7074 696f 6e61 6c5b  _date: Optional[
+00010420: 7374 725d 203d 204e 6f6e 652c 0a29 202d  str] = None,.) -
+00010430: 3e20 6574 7265 652e 5f45 6c65 6d65 6e74  > etree._Element
+00010440: 3a0a 2020 2020 2222 220a 2020 2020 4372  :.    """.    Cr
+00010450: 6561 7465 7320 616e 2065 6d70 7479 206c  eates an empty l
+00010460: 696e 6b20 656c 656d 656e 742c 2077 6974  ink element, wit
+00010470: 6820 7468 6520 6174 7472 6962 7574 6573  h the attributes
+00010480: 2061 7320 7370 6563 6966 6965 6420 6279   as specified by
+00010490: 2074 6865 2061 7267 756d 656e 7473 0a0a   the arguments..
+000104a0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+000104b0: 2020 5468 6520 6172 6775 6d65 6e74 7320    The arguments 
+000104c0: 636f 7272 6573 706f 6e64 2031 3a31 2074  correspond 1:1 t
+000104d0: 6f20 7468 6520 6174 7472 6962 7574 6573  o the attributes
+000104e0: 206f 6620 7468 6520 3c6c 696e 6b3e 2065   of the <link> e
+000104f0: 6c65 6d65 6e74 2e0a 0a20 2020 2052 6169  lement...    Rai
+00010500: 7365 733a 0a20 2020 2020 2020 2057 6172  ses:.        War
+00010510: 6e69 6e67 3a20 6966 2062 6f74 6820 616e  ning: if both an
+00010520: 2041 524b 2061 6e64 2061 6e20 4952 4920   ARK and an IRI 
+00010530: 6172 6520 7072 6f76 6964 6564 0a20 2020  are provided.   
+00010540: 2020 2020 2042 6173 6545 7272 6f72 3a20       BaseError: 
+00010550: 6966 2074 6865 2063 7265 6174 696f 6e20  if the creation 
+00010560: 6461 7465 2069 7320 696e 7661 6c69 640a  date is invalid.
+00010570: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
+00010580: 2020 2020 2020 5468 6520 6c69 6e6b 2065        The link e
+00010590: 6c65 6d65 6e74 2c20 7769 7468 6f75 7420  lement, without 
+000105a0: 616e 7920 6368 696c 6472 656e 2c20 6275  any children, bu
+000105b0: 7420 7769 7468 2074 6865 2061 7474 7269  t with the attri
+000105c0: 6275 7465 733a 0a20 2020 2020 2020 203c  butes:.        <
+000105d0: 6c69 6e6b 206c 6162 656c 3d6c 6162 656c  link label=label
+000105e0: 2069 643d 6964 2070 6572 6d69 7373 696f   id=id permissio
+000105f0: 6e73 3d70 6572 6d69 7373 696f 6e73 2061  ns=permissions a
+00010600: 726b 3d61 726b 2069 7269 3d69 7269 3e3c  rk=ark iri=iri><
+00010610: 2f6c 696e 6b3e 0a0a 2020 2020 4578 616d  /link>..    Exam
+00010620: 706c 6573 3a0a 2020 2020 2020 2020 3e3e  ples:.        >>
+00010630: 3e20 6c69 6e6b 203d 2065 7863 656c 3278  > link = excel2x
+00010640: 6d6c 2e6d 616b 655f 6c69 6e6b 2822 6c61  ml.make_link("la
+00010650: 6265 6c22 2c20 2269 6422 290a 2020 2020  bel", "id").    
+00010660: 2020 2020 3e3e 3e20 6c69 6e6b 2e61 7070      >>> link.app
+00010670: 656e 6428 6578 6365 6c32 786d 6c2e 6d61  end(excel2xml.ma
+00010680: 6b65 5f74 6578 745f 7072 6f70 2822 6861  ke_text_prop("ha
+00010690: 7343 6f6d 6d65 6e74 222c 2022 5468 6973  sComment", "This
+000106a0: 2069 7320 6120 636f 6d6d 656e 7422 2929   is a comment"))
+000106b0: 0a20 2020 2020 2020 203e 3e3e 206c 696e  .        >>> lin
+000106c0: 6b2e 6170 7065 6e64 2865 7863 656c 3278  k.append(excel2x
+000106d0: 6d6c 2e6d 616b 655f 7265 7370 7472 5f70  ml.make_resptr_p
+000106e0: 726f 7028 2268 6173 4c69 6e6b 546f 222c  rop("hasLinkTo",
+000106f0: 205b 2272 6573 6f75 7263 655f 3022 2c20   ["resource_0", 
+00010700: 2272 6573 6f75 7263 655f 3122 5d29 290a  "resource_1"])).
+00010710: 2020 2020 2020 2020 3e3e 3e20 726f 6f74          >>> root
+00010720: 2e61 7070 656e 6428 6c69 6e6b 290a 0a20  .append(link).. 
+00010730: 2020 2053 6565 2068 7474 7073 3a2f 2f64     See https://d
+00010740: 6f63 732e 6461 7363 682e 7377 6973 732f  ocs.dasch.swiss/
+00010750: 6c61 7465 7374 2f44 5350 2d54 4f4f 4c53  latest/DSP-TOOLS
+00010760: 2f66 696c 652d 666f 726d 6174 732f 786d  /file-formats/xm
+00010770: 6c2d 6461 7461 2d66 696c 652f 236c 696e  l-data-file/#lin
+00010780: 6b0a 2020 2020 2222 220a 0a20 2020 206b  k.    """..    k
+00010790: 7761 7267 7320 3d20 7b22 6c61 6265 6c22  wargs = {"label"
+000107a0: 3a20 6c61 6265 6c2c 2022 6964 223a 2069  : label, "id": i
+000107b0: 642c 2022 7065 726d 6973 7369 6f6e 7322  d, "permissions"
+000107c0: 3a20 7065 726d 6973 7369 6f6e 732c 2022  : permissions, "
+000107d0: 6e73 6d61 7022 3a20 786d 6c5f 6e61 6d65  nsmap": xml_name
+000107e0: 7370 6163 655f 6d61 707d 0a20 2020 2069  space_map}.    i
+000107f0: 6620 6172 6b3a 0a20 2020 2020 2020 206b  f ark:.        k
+00010800: 7761 7267 735b 2261 726b 225d 203d 2061  wargs["ark"] = a
+00010810: 726b 0a20 2020 2069 6620 6972 693a 0a20  rk.    if iri:. 
+00010820: 2020 2020 2020 206b 7761 7267 735b 2269         kwargs["i
+00010830: 7269 225d 203d 2069 7269 0a20 2020 2069  ri"] = iri.    i
+00010840: 6620 6172 6b20 616e 6420 6972 693a 0a20  f ark and iri:. 
+00010850: 2020 2020 2020 206d 7367 203d 2066 2242         msg = f"B
+00010860: 6f74 6820 4152 4b20 616e 6420 4952 4920  oth ARK and IRI 
+00010870: 7765 7265 2070 726f 7669 6465 6420 666f  were provided fo
+00010880: 7220 7265 736f 7572 6365 2027 7b6c 6162  r resource '{lab
+00010890: 656c 7d27 2028 7b69 647d 292e 2054 6865  el}' ({id}). The
+000108a0: 2041 524b 2077 696c 6c20 6f76 6572 7269   ARK will overri
+000108b0: 6465 2074 6865 2049 5249 2e22 0a20 2020  de the IRI.".   
+000108c0: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
+000108d0: 726e 2844 7370 546f 6f6c 7355 7365 7257  rn(DspToolsUserW
+000108e0: 6172 6e69 6e67 286d 7367 2929 0a20 2020  arning(msg)).   
+000108f0: 2069 6620 6372 6561 7469 6f6e 5f64 6174   if creation_dat
+00010900: 653a 0a20 2020 2020 2020 2074 7279 3a0a  e:.        try:.
+00010910: 2020 2020 2020 2020 2020 2020 4461 7465              Date
+00010920: 5469 6d65 5374 616d 7028 6372 6561 7469  TimeStamp(creati
+00010930: 6f6e 5f64 6174 6529 0a20 2020 2020 2020  on_date).       
+00010940: 2065 7863 6570 7420 4261 7365 4572 726f   except BaseErro
+00010950: 723a 0a20 2020 2020 2020 2020 2020 2072  r:.            r
+00010960: 6169 7365 2042 6173 6545 7272 6f72 280a  aise BaseError(.
+00010970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010980: 6622 5468 6520 6c69 6e6b 2027 7b6c 6162  f"The link '{lab
+00010990: 656c 7d27 2028 4944 3a20 7b69 647d 2920  el}' (ID: {id}) 
+000109a0: 6861 7320 616e 2069 6e76 616c 6964 2063  has an invalid c
+000109b0: 7265 6174 696f 6e20 6461 7465 2027 7b63  reation date '{c
+000109c0: 7265 6174 696f 6e5f 6461 7465 7d27 2e20  reation_date}'. 
+000109d0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+000109e0: 2020 6622 4469 6420 796f 7520 7065 7268    f"Did you perh
+000109f0: 6170 7320 666f 7267 6574 2074 6865 2074  aps forget the t
+00010a00: 696d 657a 6f6e 653f 220a 2020 2020 2020  imezone?".      
+00010a10: 2020 2020 2020 2920 6672 6f6d 204e 6f6e        ) from Non
+00010a20: 650a 2020 2020 2020 2020 6b77 6172 6773  e.        kwargs
+00010a30: 5b22 6372 6561 7469 6f6e 5f64 6174 6522  ["creation_date"
+00010a40: 5d20 3d20 6372 6561 7469 6f6e 5f64 6174  ] = creation_dat
+00010a50: 650a 0a20 2020 2072 6574 7572 6e20 6574  e..    return et
+00010a60: 7265 652e 456c 656d 656e 7428 0a20 2020  ree.Element(.   
+00010a70: 2020 2020 2022 7b25 737d 6c69 6e6b 2220       "{%s}link" 
+00010a80: 2520 786d 6c5f 6e61 6d65 7370 6163 655f  % xml_namespace_
+00010a90: 6d61 705b 4e6f 6e65 5d2c 0a20 2020 2020  map[None],.     
+00010aa0: 2020 202a 2a6b 7761 7267 732c 2020 2320     **kwargs,  # 
+00010ab0: 7479 7065 3a20 6967 6e6f 7265 5b61 7267  type: ignore[arg
+00010ac0: 2d74 7970 655d 0a20 2020 2029 0a0a 0a64  -type].    )...d
+00010ad0: 6566 206d 616b 655f 6175 6469 6f5f 7365  ef make_audio_se
+00010ae0: 676d 656e 7428 2020 2320 6e6f 7161 3a20  gment(  # noqa: 
+00010af0: 4434 3137 2028 756e 646f 6375 6d65 6e74  D417 (undocument
+00010b00: 6564 2d70 6172 616d 290a 2020 2020 6c61  ed-param).    la
+00010b10: 6265 6c3a 2073 7472 2c0a 2020 2020 6964  bel: str,.    id
+00010b20: 3a20 7374 722c 0a20 2020 2070 6572 6d69  : str,.    permi
+00010b30: 7373 696f 6e73 3a20 7374 7220 3d20 2272  ssions: str = "r
+00010b40: 6573 2d64 6566 6175 6c74 222c 0a29 202d  es-default",.) -
+00010b50: 3e20 6574 7265 652e 5f45 6c65 6d65 6e74  > etree._Element
+00010b60: 3a0a 2020 2020 2222 220a 2020 2020 4372  :.    """.    Cr
+00010b70: 6561 7465 7320 616e 2065 6d70 7479 203c  eates an empty <
+00010b80: 6175 6469 6f2d 7365 676d 656e 743e 2065  audio-segment> e
+00010b90: 6c65 6d65 6e74 2c20 7769 7468 2074 6865  lement, with the
+00010ba0: 2061 7474 7269 6275 7465 7320 6173 2073   attributes as s
+00010bb0: 7065 6369 6669 6564 2062 7920 7468 6520  pecified by the 
+00010bc0: 6172 6775 6d65 6e74 730a 0a20 2020 2041  arguments..    A
+00010bd0: 7267 733a 0a20 2020 2020 2020 2054 6865  rgs:.        The
+00010be0: 2061 7267 756d 656e 7473 2063 6f72 7265   arguments corre
+00010bf0: 7370 6f6e 6420 313a 3120 746f 2074 6865  spond 1:1 to the
+00010c00: 2061 7474 7269 6275 7465 7320 6f66 2074   attributes of t
+00010c10: 6865 203c 6175 6469 6f2d 7365 676d 656e  he <audio-segmen
+00010c20: 743e 2065 6c65 6d65 6e74 2e0a 0a20 2020  t> element...   
+00010c30: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00010c40: 2020 5468 6520 6175 6469 6f2d 7365 676d    The audio-segm
+00010c50: 656e 7420 656c 656d 656e 742c 2077 6974  ent element, wit
+00010c60: 686f 7574 2061 6e79 2063 6869 6c64 7265  hout any childre
+00010c70: 6e2c 2062 7574 2077 6974 6820 7468 6520  n, but with the 
+00010c80: 6174 7472 6962 7574 6573 3a0a 2020 2020  attributes:.    
+00010c90: 2020 2020 3c61 7564 696f 2d73 6567 6d65      <audio-segme
+00010ca0: 6e74 206c 6162 656c 3d6c 6162 656c 2069  nt label=label i
+00010cb0: 643d 6964 2070 6572 6d69 7373 696f 6e73  d=id permissions
+00010cc0: 3d70 6572 6d69 7373 696f 6e73 3e3c 2f61  =permissions></a
+00010cd0: 7564 696f 2d73 6567 6d65 6e74 3e0a 0a20  udio-segment>.. 
+00010ce0: 2020 2045 7861 6d70 6c65 733a 0a20 2020     Examples:.   
+00010cf0: 2020 2020 203e 3e3e 2061 7564 696f 5f73       >>> audio_s
+00010d00: 6567 6d65 6e74 203d 2065 7863 656c 3278  egment = excel2x
+00010d10: 6d6c 2e6d 616b 655f 6175 6469 6f5f 7365  ml.make_audio_se
+00010d20: 676d 656e 7428 226c 6162 656c 222c 2022  gment("label", "
+00010d30: 6964 2229 0a20 2020 2020 2020 203e 3e3e  id").        >>>
+00010d40: 2061 7564 696f 5f73 6567 6d65 6e74 2e61   audio_segment.a
+00010d50: 7070 656e 6428 6578 6365 6c32 786d 6c2e  ppend(excel2xml.
+00010d60: 6d61 6b65 5f72 6573 7074 725f 7072 6f70  make_resptr_prop
+00010d70: 2822 6973 5365 676d 656e 744f 6622 2c20  ("isSegmentOf", 
+00010d80: 2261 7564 696f 5f72 6573 6f75 7263 655f  "audio_resource_
+00010d90: 6964 2229 290a 2020 2020 2020 2020 3e3e  id")).        >>
+00010da0: 3e20 6175 6469 6f5f 7365 676d 656e 742e  > audio_segment.
+00010db0: 6170 7065 6e64 2865 7863 656c 3278 6d6c  append(excel2xml
+00010dc0: 2e6d 616b 655f 696e 7465 7276 616c 5f70  .make_interval_p
+00010dd0: 726f 7028 2268 6173 5365 676d 656e 7442  rop("hasSegmentB
+00010de0: 6f75 6e64 7322 2c20 2236 303a 3132 3022  ounds", "60:120"
+00010df0: 290a 2020 2020 2020 2020 3e3e 3e20 726f  ).        >>> ro
+00010e00: 6f74 2e61 7070 656e 6428 6175 6469 6f5f  ot.append(audio_
+00010e10: 7365 676d 656e 7429 0a0a 2020 2020 5365  segment)..    Se
+00010e20: 6520 6874 7470 733a 2f2f 646f 6373 2e64  e https://docs.d
+00010e30: 6173 6368 2e73 7769 7373 2f6c 6174 6573  asch.swiss/lates
+00010e40: 742f 4453 502d 544f 4f4c 532f 6669 6c65  t/DSP-TOOLS/file
+00010e50: 2d66 6f72 6d61 7473 2f78 6d6c 2d64 6174  -formats/xml-dat
+00010e60: 612d 6669 6c65 2f23 7669 6465 6f2d 7365  a-file/#video-se
+00010e70: 676d 656e 742d 6175 6469 6f2d 7365 676d  gment-audio-segm
+00010e80: 656e 740a 2020 2020 2222 220a 2020 2020  ent.    """.    
+00010e90: 7265 7475 726e 2065 7472 6565 2e45 6c65  return etree.Ele
+00010ea0: 6d65 6e74 280a 2020 2020 2020 2020 227b  ment(.        "{
+00010eb0: 2573 7d61 7564 696f 2d73 6567 6d65 6e74  %s}audio-segment
+00010ec0: 2220 2520 786d 6c5f 6e61 6d65 7370 6163  " % xml_namespac
+00010ed0: 655f 6d61 705b 4e6f 6e65 5d2c 0a20 2020  e_map[None],.   
+00010ee0: 2020 2020 206c 6162 656c 3d6c 6162 656c       label=label
+00010ef0: 2c0a 2020 2020 2020 2020 6964 3d69 642c  ,.        id=id,
+00010f00: 0a20 2020 2020 2020 2070 6572 6d69 7373  .        permiss
+00010f10: 696f 6e73 3d70 6572 6d69 7373 696f 6e73  ions=permissions
+00010f20: 2c0a 2020 2020 2020 2020 6e73 6d61 703d  ,.        nsmap=
+00010f30: 786d 6c5f 6e61 6d65 7370 6163 655f 6d61  xml_namespace_ma
+00010f40: 702c 0a20 2020 2029 0a0a 0a64 6566 206d  p,.    )...def m
+00010f50: 616b 655f 7669 6465 6f5f 7365 676d 656e  ake_video_segmen
+00010f60: 7428 2020 2320 6e6f 7161 3a20 4434 3137  t(  # noqa: D417
+00010f70: 2028 756e 646f 6375 6d65 6e74 6564 2d70   (undocumented-p
+00010f80: 6172 616d 290a 2020 2020 6c61 6265 6c3a  aram).    label:
+00010f90: 2073 7472 2c0a 2020 2020 6964 3a20 7374   str,.    id: st
+00010fa0: 722c 0a20 2020 2070 6572 6d69 7373 696f  r,.    permissio
+00010fb0: 6e73 3a20 7374 7220 3d20 2272 6573 2d64  ns: str = "res-d
+00010fc0: 6566 6175 6c74 222c 0a29 202d 3e20 6574  efault",.) -> et
+00010fd0: 7265 652e 5f45 6c65 6d65 6e74 3a0a 2020  ree._Element:.  
+00010fe0: 2020 2222 220a 2020 2020 4372 6561 7465    """.    Create
+00010ff0: 7320 616e 2065 6d70 7479 203c 7669 6465  s an empty <vide
+00011000: 6f2d 7365 676d 656e 743e 2065 6c65 6d65  o-segment> eleme
+00011010: 6e74 2c20 7769 7468 2074 6865 2061 7474  nt, with the att
+00011020: 7269 6275 7465 7320 6173 2073 7065 6369  ributes as speci
+00011030: 6669 6564 2062 7920 7468 6520 6172 6775  fied by the argu
+00011040: 6d65 6e74 730a 0a20 2020 2041 7267 733a  ments..    Args:
+00011050: 0a20 2020 2020 2020 2054 6865 2061 7267  .        The arg
+00011060: 756d 656e 7473 2063 6f72 7265 7370 6f6e  uments correspon
+00011070: 6420 313a 3120 746f 2074 6865 2061 7474  d 1:1 to the att
+00011080: 7269 6275 7465 7320 6f66 2074 6865 203c  ributes of the <
+00011090: 7669 6465 6f2d 7365 676d 656e 743e 2065  video-segment> e
+000110a0: 6c65 6d65 6e74 2e0a 0a20 2020 2052 6574  lement...    Ret
+000110b0: 7572 6e73 3a0a 2020 2020 2020 2020 5468  urns:.        Th
+000110c0: 6520 7669 6465 6f2d 7365 676d 656e 7420  e video-segment 
+000110d0: 656c 656d 656e 742c 2077 6974 686f 7574  element, without
+000110e0: 2061 6e79 2063 6869 6c64 7265 6e2c 2062   any children, b
+000110f0: 7574 2077 6974 6820 7468 6520 6174 7472  ut with the attr
+00011100: 6962 7574 6573 3a0a 2020 2020 2020 2020  ibutes:.        
+00011110: 3c76 6964 656f 2d73 6567 6d65 6e74 206c  <video-segment l
+00011120: 6162 656c 3d6c 6162 656c 2069 643d 6964  abel=label id=id
+00011130: 2070 6572 6d69 7373 696f 6e73 3d70 6572   permissions=per
+00011140: 6d69 7373 696f 6e73 3e3c 2f76 6964 656f  missions></video
+00011150: 2d73 6567 6d65 6e74 3e0a 0a20 2020 2045  -segment>..    E
+00011160: 7861 6d70 6c65 733a 0a20 2020 2020 2020  xamples:.       
+00011170: 203e 3e3e 2076 6964 656f 5f73 6567 6d65   >>> video_segme
+00011180: 6e74 203d 2065 7863 656c 3278 6d6c 2e6d  nt = excel2xml.m
+00011190: 616b 655f 7669 6465 6f5f 7365 676d 656e  ake_video_segmen
+000111a0: 7428 226c 6162 656c 222c 2022 6964 2229  t("label", "id")
+000111b0: 0a20 2020 2020 2020 203e 3e3e 2076 6964  .        >>> vid
+000111c0: 656f 5f73 6567 6d65 6e74 2e61 7070 656e  eo_segment.appen
+000111d0: 6428 6578 6365 6c32 786d 6c2e 6d61 6b65  d(excel2xml.make
+000111e0: 5f72 6573 7074 725f 7072 6f70 2822 6973  _resptr_prop("is
+000111f0: 5365 676d 656e 744f 6622 2c20 2276 6964  SegmentOf", "vid
+00011200: 656f 5f72 6573 6f75 7263 655f 6964 2229  eo_resource_id")
+00011210: 290a 2020 2020 2020 2020 3e3e 3e20 7669  ).        >>> vi
+00011220: 6465 6f5f 7365 676d 656e 742e 6170 7065  deo_segment.appe
+00011230: 6e64 2865 7863 656c 3278 6d6c 2e6d 616b  nd(excel2xml.mak
+00011240: 655f 696e 7465 7276 616c 5f70 726f 7028  e_interval_prop(
+00011250: 2268 6173 5365 676d 656e 7442 6f75 6e64  "hasSegmentBound
+00011260: 7322 2c20 2236 303a 3132 3022 290a 2020  s", "60:120").  
+00011270: 2020 2020 2020 3e3e 3e20 726f 6f74 2e61        >>> root.a
+00011280: 7070 656e 6428 7669 6465 6f5f 7365 676d  ppend(video_segm
+00011290: 656e 7429 0a0a 2020 2020 5365 6520 6874  ent)..    See ht
+000112a0: 7470 733a 2f2f 646f 6373 2e64 6173 6368  tps://docs.dasch
+000112b0: 2e73 7769 7373 2f6c 6174 6573 742f 4453  .swiss/latest/DS
+000112c0: 502d 544f 4f4c 532f 6669 6c65 2d66 6f72  P-TOOLS/file-for
+000112d0: 6d61 7473 2f78 6d6c 2d64 6174 612d 6669  mats/xml-data-fi
+000112e0: 6c65 2f23 7669 6465 6f2d 7365 676d 656e  le/#video-segmen
+000112f0: 742d 6175 6469 6f2d 7365 676d 656e 740a  t-audio-segment.
+00011300: 2020 2020 2222 220a 2020 2020 7265 7475      """.    retu
+00011310: 726e 2065 7472 6565 2e45 6c65 6d65 6e74  rn etree.Element
+00011320: 280a 2020 2020 2020 2020 227b 2573 7d76  (.        "{%s}v
+00011330: 6964 656f 2d73 6567 6d65 6e74 2220 2520  ideo-segment" % 
+00011340: 786d 6c5f 6e61 6d65 7370 6163 655f 6d61  xml_namespace_ma
+00011350: 705b 4e6f 6e65 5d2c 0a20 2020 2020 2020  p[None],.       
+00011360: 206c 6162 656c 3d6c 6162 656c 2c0a 2020   label=label,.  
+00011370: 2020 2020 2020 6964 3d69 642c 0a20 2020        id=id,.   
+00011380: 2020 2020 2070 6572 6d69 7373 696f 6e73       permissions
+00011390: 3d70 6572 6d69 7373 696f 6e73 2c0a 2020  =permissions,.  
+000113a0: 2020 2020 2020 6e73 6d61 703d 786d 6c5f        nsmap=xml_
+000113b0: 6e61 6d65 7370 6163 655f 6d61 702c 0a20  namespace_map,. 
+000113c0: 2020 2029 0a0a 0a64 6566 2063 7265 6174     )...def creat
+000113d0: 655f 696e 7465 7276 616c 5f76 616c 7565  e_interval_value
+000113e0: 2873 7461 7274 3a20 7374 722c 2065 6e64  (start: str, end
+000113f0: 3a20 7374 7229 202d 3e20 7374 723a 0a20  : str) -> str:. 
+00011400: 2020 2022 2222 0a20 2020 2054 7261 6e73     """.    Trans
+00011410: 666f 726d 2061 2073 7461 7274 2061 6e64  form a start and
+00011420: 2065 6e64 2074 696d 6520 696e 746f 2061   end time into a
+00011430: 2076 616c 6964 2044 5350 2069 6e74 6572   valid DSP inter
+00011440: 7661 6c20 7661 6c75 652c 0a20 2020 2077  val value,.    w
+00011450: 6869 6368 2074 6865 6e20 6361 6e20 6265  hich then can be
+00011460: 2075 7365 6420 696e 2061 6e20 3c69 6e74   used in an <int
+00011470: 6572 7661 6c20 6e61 6d65 3d22 6861 7353  erval name="hasS
+00011480: 6567 6d65 6e74 426f 756e 6473 223e 2074  egmentBounds"> t
+00011490: 6167 2c0a 2020 2020 7768 6963 6820 6973  ag,.    which is
+000114a0: 2075 7365 6420 696e 203c 6175 6469 6f2d   used in <audio-
+000114b0: 7365 676d 656e 743e 2061 6e64 203c 7669  segment> and <vi
+000114c0: 6465 6f2d 7365 676d 656e 743e 2065 6c65  deo-segment> ele
+000114d0: 6d65 6e74 732e 0a0a 2020 2020 4172 6773  ments...    Args
+000114e0: 3a0a 2020 2020 2020 2020 7374 6172 743a  :.        start:
+000114f0: 2073 7461 7274 2074 696d 6520 6f66 2074   start time of t
+00011500: 6865 2076 6964 656f 2f61 7564 696f 2073  he video/audio s
+00011510: 6567 6d65 6e74 2c20 696e 2074 6865 2066  egment, in the f
+00011520: 6f72 6d61 7420 2748 2848 293a 4d4d 3a53  ormat 'H(H):MM:S
+00011530: 5328 2e73 2927 0a20 2020 2020 2020 2065  S(.s)'.        e
+00011540: 6e64 3a20 656e 6420 7469 6d65 206f 6620  nd: end time of 
+00011550: 7468 6520 7669 6465 6f2f 6175 6469 6f20  the video/audio 
+00011560: 7365 676d 656e 742c 2069 6e20 7468 6520  segment, in the 
+00011570: 666f 726d 6174 2027 4828 4829 3a4d 4d3a  format 'H(H):MM:
+00011580: 5353 282e 7329 270a 0a20 2020 2052 6169  SS(.s)'..    Rai
+00011590: 7365 733a 0a20 2020 2020 2020 2056 616c  ses:.        Val
+000115a0: 7565 4572 726f 723a 2069 6620 7468 6520  ueError: if the 
+000115b0: 7072 6f76 6964 6564 2061 7267 756d 656e  provided argumen
+000115c0: 7473 2061 7265 206e 6f74 2069 6e20 7468  ts are not in th
+000115d0: 6520 636f 7272 6563 7420 666f 726d 6174  e correct format
+000115e0: 2c20 6f72 2069 6620 7468 6520 7374 6172  , or if the star
+000115f0: 7420 7469 6d65 2069 7320 6772 6561 7465  t time is greate
+00011600: 7220 7468 616e 2074 6865 2065 6e64 2074  r than the end t
+00011610: 696d 650a 0a20 2020 2052 6574 7572 6e73  ime..    Returns
+00011620: 3a0a 2020 2020 2020 2020 6120 4453 5020  :.        a DSP 
+00011630: 696e 7465 7276 616c 2076 616c 7565 2069  interval value i
+00011640: 6e20 7468 6520 666f 726d 6174 2027 7374  n the format 'st
+00011650: 6172 745f 7365 636f 6e64 733a 656e 645f  art_seconds:end_
+00011660: 7365 636f 6e64 7327 0a0a 2020 2020 4578  seconds'..    Ex
+00011670: 616d 706c 6573 3a0a 2020 2020 2020 2020  amples:.        
+00011680: 3e3e 3e20 6578 6365 6c32 786d 6c2e 6372  >>> excel2xml.cr
+00011690: 6561 7465 5f69 6e74 6572 7661 6c5f 7661  eate_interval_va
+000116a0: 6c75 6528 2230 3a30 313a 3030 222c 2022  lue("0:01:00", "
+000116b0: 303a 3032 3a30 3022 290a 2020 2020 2020  0:02:00").      
+000116c0: 2020 2236 303a 3132 3022 0a20 2020 2020    "60:120".     
+000116d0: 2020 203e 3e3e 2065 7863 656c 3278 6d6c     >>> excel2xml
+000116e0: 2e63 7265 6174 655f 696e 7465 7276 616c  .create_interval
+000116f0: 5f76 616c 7565 2822 303a 3031 3a30 302e  _value("0:01:00.
+00011700: 3522 2c20 2230 3a30 313a 3030 2e36 2229  5", "0:01:00.6")
+00011710: 0a20 2020 2020 2020 2022 3630 2e35 3a36  .        "60.5:6
+00011720: 302e 3622 0a20 2020 2022 2222 0a20 2020  0.6".    """.   
+00011730: 2073 7461 7274 5f6d 6174 6368 203d 2072   start_match = r
+00011740: 6567 6578 2e73 6561 7263 6828 7222 5e28  egex.search(r"^(
+00011750: 5c64 2b29 3a28 5b30 2d35 5d5b 302d 395d  \d+):([0-5][0-9]
+00011760: 293a 285b 302d 355d 5b30 2d39 5d28 3f3a  ):([0-5][0-9](?:
+00011770: 5c2e 5b30 2d39 5d2b 293f 2924 222c 2073  \.[0-9]+)?)$", s
+00011780: 7461 7274 290a 2020 2020 656e 645f 6d61  tart).    end_ma
+00011790: 7463 6820 3d20 7265 6765 782e 6d61 7463  tch = regex.matc
+000117a0: 6828 7222 5e28 5c64 2b29 3a28 5b30 2d35  h(r"^(\d+):([0-5
+000117b0: 5d5b 302d 395d 293a 285b 302d 355d 5b30  ][0-9]):([0-5][0
+000117c0: 2d39 5d28 3f3a 5c2e 5b30 2d39 5d2b 293f  -9](?:\.[0-9]+)?
+000117d0: 2924 222c 2065 6e64 290a 2020 2020 6966  )$", end).    if
+000117e0: 206e 6f74 2073 7461 7274 5f6d 6174 6368   not start_match
+000117f0: 206f 7220 6e6f 7420 656e 645f 6d61 7463   or not end_matc
+00011800: 683a 0a20 2020 2020 2020 2072 6169 7365  h:.        raise
+00011810: 2056 616c 7565 4572 726f 7228 2254 6865   ValueError("The
+00011820: 2073 7461 7274 2061 6e64 2065 6e64 2076   start and end v
+00011830: 616c 7565 7320 6d75 7374 2062 6520 696e  alues must be in
+00011840: 2074 6865 2066 6f72 6d61 7420 2748 2848   the format 'H(H
+00011850: 293a 4d4d 3a53 5328 2e73 2927 2229 0a20  ):MM:SS(.s)'"). 
+00011860: 2020 2073 7461 7274 5f68 2c20 7374 6172     start_h, star
+00011870: 745f 6d2c 2073 7461 7274 5f73 203d 2073  t_m, start_s = s
+00011880: 7461 7274 5f6d 6174 6368 2e67 726f 7570  tart_match.group
+00011890: 7328 290a 2020 2020 656e 645f 682c 2065  s().    end_h, e
+000118a0: 6e64 5f6d 2c20 656e 645f 7320 3d20 656e  nd_m, end_s = en
+000118b0: 645f 6d61 7463 682e 6772 6f75 7073 2829  d_match.groups()
+000118c0: 0a20 2020 2073 7461 7274 5f73 6563 6f6e  .    start_secon
+000118d0: 6473 203d 2069 6e74 2873 7461 7274 5f68  ds = int(start_h
+000118e0: 2920 2a20 3336 3030 202b 2069 6e74 2873  ) * 3600 + int(s
+000118f0: 7461 7274 5f6d 2920 2a20 3630 202b 2066  tart_m) * 60 + f
+00011900: 6c6f 6174 2873 7461 7274 5f73 290a 2020  loat(start_s).  
+00011910: 2020 656e 645f 7365 636f 6e64 7320 3d20    end_seconds = 
+00011920: 696e 7428 656e 645f 6829 202a 2033 3630  int(end_h) * 360
+00011930: 3020 2b20 696e 7428 656e 645f 6d29 202a  0 + int(end_m) *
+00011940: 2036 3020 2b20 666c 6f61 7428 656e 645f   60 + float(end_
+00011950: 7329 0a20 2020 2073 7461 7274 5f73 6563  s).    start_sec
+00011960: 6f6e 6473 203d 2069 6e74 2873 7461 7274  onds = int(start
+00011970: 5f73 6563 6f6e 6473 2920 6966 2073 7461  _seconds) if sta
+00011980: 7274 5f73 6563 6f6e 6473 2e69 735f 696e  rt_seconds.is_in
+00011990: 7465 6765 7228 2920 656c 7365 2073 7461  teger() else sta
+000119a0: 7274 5f73 6563 6f6e 6473 0a20 2020 2065  rt_seconds.    e
+000119b0: 6e64 5f73 6563 6f6e 6473 203d 2069 6e74  nd_seconds = int
+000119c0: 2865 6e64 5f73 6563 6f6e 6473 2920 6966  (end_seconds) if
+000119d0: 2065 6e64 5f73 6563 6f6e 6473 2e69 735f   end_seconds.is_
+000119e0: 696e 7465 6765 7228 2920 656c 7365 2065  integer() else e
+000119f0: 6e64 5f73 6563 6f6e 6473 0a20 2020 2069  nd_seconds.    i
+00011a00: 6620 7374 6172 745f 7365 636f 6e64 7320  f start_seconds 
+00011a10: 3e20 656e 645f 7365 636f 6e64 733a 0a20  > end_seconds:. 
+00011a20: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00011a30: 7565 4572 726f 7228 2254 6865 2073 7461  ueError("The sta
+00011a40: 7274 2076 616c 7565 206d 7573 7420 6265  rt value must be
+00011a50: 2073 6d61 6c6c 6572 2074 6861 6e20 7468   smaller than th
+00011a60: 6520 656e 6420 7661 6c75 6522 290a 2020  e end value").  
+00011a70: 2020 7265 7475 726e 2066 227b 7374 6172    return f"{star
+00011a80: 745f 7365 636f 6e64 737d 3a7b 656e 645f  t_seconds}:{end_
+00011a90: 7365 636f 6e64 737d 220a 0a0a 6465 6620  seconds}"...def 
+00011aa0: 6372 6561 7465 5f6a 736f 6e5f 6578 6365  create_json_exce
+00011ab0: 6c5f 6c69 7374 5f6d 6170 7069 6e67 280a  l_list_mapping(.
+00011ac0: 2020 2020 7061 7468 5f74 6f5f 6a73 6f6e      path_to_json
+00011ad0: 3a20 7374 722c 0a20 2020 206c 6973 745f  : str,.    list_
+00011ae0: 6e61 6d65 3a20 7374 722c 0a20 2020 2065  name: str,.    e
+00011af0: 7863 656c 5f76 616c 7565 733a 2049 7465  xcel_values: Ite
+00011b00: 7261 626c 655b 7374 725d 2c0a 2020 2020  rable[str],.    
+00011b10: 7365 703a 2073 7472 203d 2027 2b22 2ac3  sep: str = '+"*.
+00011b20: a725 262f 2829 3d27 2c0a 2020 2020 636f  .%&/()=',.    co
+00011b30: 7272 6563 7469 6f6e 733a 204f 7074 696f  rrections: Optio
+00011b40: 6e61 6c5b 6469 6374 5b73 7472 2c20 7374  nal[dict[str, st
+00011b50: 725d 5d20 3d20 4e6f 6e65 2c0a 2920 2d3e  r]] = None,.) ->
+00011b60: 2064 6963 745b 7374 722c 2073 7472 5d3a   dict[str, str]:
+00011b70: 0a20 2020 2022 2222 0a20 2020 204f 6674  .    """.    Oft
+00011b80: 656e 2c20 6461 7461 2073 6f75 7263 6573  en, data sources
+00011b90: 2063 6f6e 7461 696e 206c 6973 7420 7661   contain list va
+00011ba0: 6c75 6573 2074 6861 7420 6172 656e 2774  lues that aren't
+00011bb0: 2069 6465 6e74 6963 616c 2074 6f20 7468   identical to th
+00011bc0: 6520 6e61 6d65 206f 6620 7468 6520 6e6f  e name of the no
+00011bd0: 6465 2069 6e20 7468 6520 6c69 7374 206f  de in the list o
+00011be0: 6620 7468 6520 4a53 4f4e 0a20 2020 2070  f the JSON.    p
+00011bf0: 726f 6a65 6374 2066 696c 6520 2863 6f6c  roject file (col
+00011c00: 6c6f 7175 6961 6c6c 793a 206f 6e74 6f6c  loquially: ontol
+00011c10: 6f67 7929 2e20 496e 206f 7264 6572 2074  ogy). In order t
+00011c20: 6f20 6372 6561 7465 2061 2063 6f72 7265  o create a corre
+00011c30: 6374 2058 4d4c 2066 6f72 2074 6865 2060  ct XML for the `
+00011c40: 6473 702d 746f 6f6c 7320 786d 6c75 706c  dsp-tools xmlupl
+00011c50: 6f61 6460 2c20 6120 6d61 7070 696e 6720  oad`, a mapping 
+00011c60: 6973 0a20 2020 206e 6563 6573 7361 7279  is.    necessary
+00011c70: 2e20 5468 6973 2066 756e 6374 696f 6e20  . This function 
+00011c80: 7461 6b65 7320 6120 4a53 4f4e 206c 6973  takes a JSON lis
+00011c90: 7420 616e 6420 616e 2045 7863 656c 2063  t and an Excel c
+00011ca0: 6f6c 756d 6e20 636f 6e74 6169 6e69 6e67  olumn containing
+00011cb0: 206c 6973 742d 7661 6c75 6573 2c20 616e   list-values, an
+00011cc0: 6420 7472 6965 7320 746f 206d 6174 6368  d tries to match
+00011cd0: 2074 6865 6d0a 2020 2020 6175 746f 6d61   them.    automa
+00011ce0: 7469 6361 6c6c 7920 6261 7365 6420 6f6e  tically based on
+00011cf0: 2073 696d 696c 6172 6974 792e 2054 6865   similarity. The
+00011d00: 2072 6573 756c 7420 6973 2061 2064 6963   result is a dic
+00011d10: 7420 6f66 2074 6865 2066 6f72 6d20 7b65  t of the form {e
+00011d20: 7863 656c 5f76 616c 7565 3a20 6c69 7374  xcel_value: list
+00011d30: 5f6e 6f64 655f 6e61 6d65 7d2e 0a0a 2020  _node_name}...  
+00011d40: 2020 416c 7465 726e 6174 6976 656c 792c    Alternatively,
+00011d50: 2063 6f6e 7369 6465 7220 7573 696e 6720   consider using 
+00011d60: 7468 6520 6675 6e63 7469 6f6e 2063 7265  the function cre
+00011d70: 6174 655f 6a73 6f6e 5f6c 6973 745f 6d61  ate_json_list_ma
+00011d80: 7070 696e 6728 292c 2077 6869 6368 2061  pping(), which a
+00011d90: 6c73 6f20 6275 696c 6473 2061 2064 6963  lso builds a dic
+00011da0: 7469 6f6e 6172 792c 0a20 2020 2062 7574  tionary,.    but
+00011db0: 2066 726f 6d20 7468 6520 6e61 6d65 7320   from the names 
+00011dc0: 616e 6420 6c61 6265 6c73 2069 6e20 7468  and labels in th
+00011dd0: 6520 4a53 4f4e 206c 6973 742c 2077 6869  e JSON list, whi
+00011de0: 6368 2069 7320 6c65 7373 2065 7272 6f72  ch is less error
+00011df0: 2d70 726f 6e65 2074 6861 6e20 7468 6973  -prone than this
+00011e00: 2066 756e 6374 696f 6e27 7320 6170 7072   function's appr
+00011e10: 6f61 6368 2e20 486f 7765 7665 722c 0a20  oach. However,. 
+00011e20: 2020 2074 6869 7320 6675 6e63 7469 6f6e     this function
+00011e30: 2068 6173 2074 6865 2061 6476 616e 7461   has the advanta
+00011e40: 6765 2074 6861 7420 6974 2065 7665 6e20  ge that it even 
+00011e50: 776f 726b 7320 7768 656e 2079 6f75 7220  works when your 
+00011e60: 6461 7461 2073 6f75 7263 6520 646f 6573  data source does
+00011e70: 6e27 7420 7573 6520 7468 6520 6c69 7374  n't use the list
+00011e80: 206c 6162 656c 7320 636f 7272 6563 746c   labels correctl
+00011e90: 792e 0a0a 2020 2020 4172 6773 3a0a 2020  y...    Args:.  
+00011ea0: 2020 2020 2020 7061 7468 5f74 6f5f 6a73        path_to_js
+00011eb0: 6f6e 3a20 7061 7468 2074 6f20 7468 6520  on: path to the 
+00011ec0: 4a53 4f4e 2070 726f 6a65 6374 2066 696c  JSON project fil
+00011ed0: 650a 2020 2020 2020 2020 6c69 7374 5f6e  e.        list_n
+00011ee0: 616d 653a 206e 616d 6520 6f66 2074 6865  ame: name of the
+00011ef0: 206c 6973 7420 696e 2074 6865 204a 534f   list in the JSO
+00011f00: 4e20 7072 6f6a 6563 7420 6669 6c65 2028  N project file (
+00011f10: 6361 6e20 616c 736f 2062 6520 6120 6e65  can also be a ne
+00011f20: 7374 6564 206c 6973 7429 0a20 2020 2020  sted list).     
+00011f30: 2020 2065 7863 656c 5f76 616c 7565 733a     excel_values:
+00011f40: 2074 6865 2045 7863 656c 2063 6f6c 756d   the Excel colum
+00011f50: 6e20 2865 2e67 2e20 6173 206c 6973 7429  n (e.g. as list)
+00011f60: 2077 6974 6820 7468 6520 6c69 7374 2076   with the list v
+00011f70: 616c 7565 7320 696e 2069 740a 2020 2020  alues in it.    
+00011f80: 2020 2020 7365 703a 2073 6570 6172 6174      sep: separat
+00011f90: 6f72 2073 7472 696e 672c 2069 6620 7468  or string, if th
+00011fa0: 6520 6365 6c6c 7320 696e 2074 6865 2045  e cells in the E
+00011fb0: 7863 656c 2063 6f6e 7461 696e 206d 6f72  xcel contain mor
+00011fc0: 6520 7468 616e 206f 6e65 206c 6973 7420  e than one list 
+00011fd0: 656e 7472 790a 2020 2020 2020 2020 636f  entry.        co
+00011fe0: 7272 6563 7469 6f6e 733a 2064 6963 7420  rrections: dict 
+00011ff0: 7769 7468 2077 726f 6e67 2065 6e74 7269  with wrong entri
+00012000: 6573 2c20 6561 6368 2070 6f69 6e74 696e  es, each pointin
+00012010: 6720 746f 2069 7473 2063 6f72 7265 6374  g to its correct
+00012020: 2063 6f75 6e74 6572 7061 7274 0a0a 2020   counterpart..  
+00012030: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
+00012040: 2020 5761 726e 696e 673a 2069 6620 7468    Warning: if th
+00012050: 6572 6520 6973 2061 6e20 4578 6365 6c20  ere is an Excel 
+00012060: 7661 6c75 6520 7468 6174 2063 6f75 6c64  value that could
+00012070: 6e27 7420 6265 206d 6174 6368 6564 0a20  n't be matched. 
+00012080: 2020 2020 2020 2045 7863 6570 7469 6f6e         Exception
+00012090: 3a20 6966 2074 6865 2070 6174 6820 646f  : if the path do
+000120a0: 6573 6e27 7420 706f 696e 7420 746f 2061  esn't point to a
+000120b0: 204a 534f 4e20 7072 6f6a 6563 7420 6669   JSON project fi
+000120c0: 6c65 0a0a 2020 2020 5265 7475 726e 733a  le..    Returns:
+000120d0: 0a20 2020 2020 2020 2064 6963 7420 6f66  .        dict of
+000120e0: 2074 6865 2066 6f72 6d20 6060 7b65 7863   the form ``{exc
+000120f0: 656c 5f76 616c 7565 3a20 6c69 7374 5f6e  el_value: list_n
+00012100: 6f64 655f 6e61 6d65 7d60 602e 0a20 2020  ode_name}``..   
+00012110: 2020 2020 2020 2020 2045 7665 7279 2065           Every e
+00012120: 7863 656c 5f76 616c 7565 2069 7320 7374  xcel_value is st
+00012130: 7269 7070 6564 2c20 616e 6420 616c 736f  ripped, and also
+00012140: 2070 7265 7365 6e74 2069 6e20 6120 6c6f   present in a lo
+00012150: 7765 7263 6173 6520 666f 726d 2e0a 0a20  wercase form... 
+00012160: 2020 2045 7861 6d70 6c65 733a 0a20 2020     Examples:.   
+00012170: 2020 2020 203e 3e3e 206a 736f 6e5f 6c69       >>> json_li
+00012180: 7374 5f6e 6f64 6573 203d 205b 0a20 2020  st_nodes = [.   
+00012190: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
+000121a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121b0: 2020 2022 6e61 6d65 223a 2022 6769 7261     "name": "gira
+000121c0: 6666 6522 2c0a 2020 2020 2020 2020 2020  ffe",.          
+000121d0: 2020 2020 2020 2020 2020 226c 6162 656c            "label
+000121e0: 7322 3a20 7b22 656e 223a 2022 6769 7261  s": {"en": "gira
+000121f0: 6666 6522 7d0a 2020 2020 2020 2020 2020  ffe"}.          
+00012200: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00012210: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+00012220: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00012230: 6e61 6d65 223a 2022 616e 7465 6c6f 7065  name": "antelope
+00012240: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00012250: 2020 2020 2020 2022 6c61 6265 6c73 223a         "labels":
+00012260: 207b 2265 6e22 3a20 2261 6e74 656c 6f70   {"en": "antelop
+00012270: 6522 7d0a 2020 2020 2020 2020 2020 2020  e"}.            
+00012280: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+00012290: 2020 5d0a 2020 2020 2020 2020 3e3e 3e20    ].        >>> 
+000122a0: 6578 6365 6c5f 726f 775f 3120 3d20 5b22  excel_row_1 = ["
+000122b0: 4769 7261 6666 6565 6820 222c 2022 2041  Giraffeeh ", " A
+000122c0: 6e74 696c 6f75 7065 222c 2022 4769 7272  ntiloupe", "Girr
+000122d0: 6166 6665 202c 2041 6e74 696c 6f75 7065  affe , Antiloupe
+000122e0: 2022 5d0a 2020 2020 2020 2020 3e3e 3e20   "].        >>> 
+000122f0: 6a73 6f6e 5f65 7863 656c 5f6c 6973 745f  json_excel_list_
+00012300: 6d61 7070 696e 6720 3d20 7b0a 2020 2020  mapping = {.    
+00012310: 2020 2020 2020 2020 2020 2020 2247 6972              "Gir
+00012320: 6166 6665 6568 223a 2022 6769 7261 6666  affeeh": "giraff
+00012330: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00012340: 2020 2020 2267 6972 6166 6665 6568 223a      "giraffeeh":
+00012350: 2022 6769 7261 6666 6522 2c0a 2020 2020   "giraffe",.    
+00012360: 2020 2020 2020 2020 2020 2020 2247 6972              "Gir
+00012370: 7261 6666 6522 3a20 2267 6972 6166 6665  raffe": "giraffe
+00012380: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00012390: 2020 2022 6769 7272 6166 6665 223a 2022     "girraffe": "
+000123a0: 6769 7261 6666 6522 2c0a 2020 2020 2020  giraffe",.      
+000123b0: 2020 2020 2020 2020 2020 2241 6e74 696c            "Antil
+000123c0: 6f75 7065 223a 2022 616e 7465 6c6f 7065  oupe": "antelope
+000123d0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000123e0: 2020 2022 616e 7469 6c6f 7570 6522 3a20     "antiloupe": 
+000123f0: 2261 6e74 656c 6f70 6522 0a20 2020 2020  "antelope".     
+00012400: 2020 2020 2020 207d 0a20 2020 2022 2222         }.    """
+00012410: 0a0a 2020 2020 2320 6176 6f69 6420 6d75  ..    # avoid mu
+00012420: 7461 626c 6520 6465 6661 756c 7420 6172  table default ar
+00012430: 6775 6d65 6e74 0a20 2020 2063 6f72 7265  gument.    corre
+00012440: 6374 696f 6e73 203d 2063 6f72 7265 6374  ctions = correct
+00012450: 696f 6e73 206f 7220 7b7d 0a0a 2020 2020  ions or {}..    
+00012460: 2320 7370 6c69 7420 7468 6520 7661 6c75  # split the valu
+00012470: 6573 2c20 6966 206e 6563 6573 7361 7279  es, if necessary
+00012480: 0a20 2020 2065 7863 656c 5f76 616c 7565  .    excel_value
+00012490: 735f 6e65 7720 3d20 5b5d 0a20 2020 2066  s_new = [].    f
+000124a0: 6f72 2076 616c 2069 6e20 6578 6365 6c5f  or val in excel_
+000124b0: 7661 6c75 6573 3a0a 2020 2020 2020 2020  values:.        
+000124c0: 6966 2069 7369 6e73 7461 6e63 6528 7661  if isinstance(va
+000124d0: 6c2c 2073 7472 293a 0a20 2020 2020 2020  l, str):.       
+000124e0: 2020 2020 2065 7863 656c 5f76 616c 7565       excel_value
+000124f0: 735f 6e65 772e 6578 7465 6e64 285b 782e  s_new.extend([x.
+00012500: 7374 7269 7028 2920 666f 7220 7820 696e  strip() for x in
+00012510: 2076 616c 2e73 706c 6974 2873 6570 2920   val.split(sep) 
+00012520: 6966 2078 5d29 0a0a 2020 2020 2320 7265  if x])..    # re
+00012530: 6164 2074 6865 206c 6973 7420 6f66 2074  ad the list of t
+00012540: 6865 204a 534f 4e20 7072 6f6a 6563 7420  he JSON project 
+00012550: 2877 6f72 6b73 2061 6c73 6f20 666f 7220  (works also for 
+00012560: 6e65 7374 6564 206c 6973 7473 290a 2020  nested lists).  
+00012570: 2020 7769 7468 206f 7065 6e28 7061 7468    with open(path
+00012580: 5f74 6f5f 6a73 6f6e 2c20 656e 636f 6469  _to_json, encodi
+00012590: 6e67 3d22 7574 662d 3822 2920 6173 2066  ng="utf-8") as f
+000125a0: 3a0a 2020 2020 2020 2020 6a73 6f6e 5f66  :.        json_f
+000125b0: 696c 6520 3d20 6a73 6f6e 2e6c 6f61 6428  ile = json.load(
+000125c0: 6629 0a20 2020 206a 736f 6e5f 7375 6273  f).    json_subs
+000125d0: 6574 203d 205b 5d0a 2020 2020 666f 7220  et = [].    for 
+000125e0: 656c 656d 2069 6e20 6a73 6f6e 5f66 696c  elem in json_fil
+000125f0: 655b 2270 726f 6a65 6374 225d 5b22 6c69  e["project"]["li
+00012600: 7374 7322 5d3a 0a20 2020 2020 2020 2069  sts"]:.        i
+00012610: 6620 656c 656d 5b22 6e61 6d65 225d 203d  f elem["name"] =
+00012620: 3d20 6c69 7374 5f6e 616d 653a 0a20 2020  = list_name:.   
+00012630: 2020 2020 2020 2020 206a 736f 6e5f 7375           json_su
+00012640: 6273 6574 203d 2065 6c65 6d5b 226e 6f64  bset = elem["nod
+00012650: 6573 225d 0a20 2020 206a 736f 6e5f 7661  es"].    json_va
+00012660: 6c75 6573 203d 2073 6574 285f 6e65 7374  lues = set(_nest
+00012670: 6564 5f64 6963 745f 7661 6c75 6573 5f69  ed_dict_values_i
+00012680: 7465 7261 746f 7228 6a73 6f6e 5f73 7562  terator(json_sub
+00012690: 7365 7429 290a 0a20 2020 2023 2062 7569  set))..    # bui
+000126a0: 6c64 2064 6963 7469 6f6e 6172 7920 7769  ld dictionary wi
+000126b0: 7468 2074 6865 206d 6170 7069 6e67 2c20  th the mapping, 
+000126c0: 6261 7365 6420 6f6e 2073 7472 696e 6720  based on string 
+000126d0: 7369 6d69 6c61 7269 7479 0a20 2020 2072  similarity.    r
+000126e0: 6573 203d 207b 7d0a 2020 2020 666f 7220  es = {}.    for 
+000126f0: 6578 6365 6c5f 7661 6c75 6520 696e 2065  excel_value in e
+00012700: 7863 656c 5f76 616c 7565 735f 6e65 773a  xcel_values_new:
+00012710: 0a20 2020 2020 2020 2065 7863 656c 5f76  .        excel_v
+00012720: 616c 7565 5f63 6f72 7265 6374 6564 203d  alue_corrected =
+00012730: 2063 6f72 7265 6374 696f 6e73 2e67 6574   corrections.get
+00012740: 2865 7863 656c 5f76 616c 7565 2c20 6578  (excel_value, ex
+00012750: 6365 6c5f 7661 6c75 6529 0a20 2020 2020  cel_value).     
+00012760: 2020 2065 7863 656c 5f76 616c 7565 5f73     excel_value_s
+00012770: 696d 706c 203d 2073 696d 706c 6966 795f  impl = simplify_
+00012780: 6e61 6d65 2865 7863 656c 5f76 616c 7565  name(excel_value
+00012790: 5f63 6f72 7265 6374 6564 2920 2023 2069  _corrected)  # i
+000127a0: 6e63 7265 6173 6520 6d61 7463 6820 7072  ncrease match pr
+000127b0: 6f62 6162 696c 6974 7920 6279 2072 656d  obability by rem
+000127c0: 6f76 696e 6720 696c 6c65 6761 6c20 6368  oving illegal ch
+000127d0: 6172 730a 2020 2020 2020 2020 6966 206d  ars.        if m
+000127e0: 6174 6368 6573 203a 3d20 6469 6666 6c69  atches := diffli
+000127f0: 622e 6765 745f 636c 6f73 655f 6d61 7463  b.get_close_matc
+00012800: 6865 7328 0a20 2020 2020 2020 2020 2020  hes(.           
+00012810: 2077 6f72 643d 6578 6365 6c5f 7661 6c75   word=excel_valu
+00012820: 655f 7369 6d70 6c2c 0a20 2020 2020 2020  e_simpl,.       
+00012830: 2020 2020 2070 6f73 7369 6269 6c69 7469       possibiliti
+00012840: 6573 3d6a 736f 6e5f 7661 6c75 6573 2c0a  es=json_values,.
+00012850: 2020 2020 2020 2020 2020 2020 6e3d 312c              n=1,
+00012860: 0a20 2020 2020 2020 2020 2020 2063 7574  .            cut
+00012870: 6f66 663d 302e 362c 0a20 2020 2020 2020  off=0.6,.       
+00012880: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+00012890: 7265 735b 6578 6365 6c5f 7661 6c75 655d  res[excel_value]
+000128a0: 203d 206d 6174 6368 6573 5b30 5d0a 2020   = matches[0].  
+000128b0: 2020 2020 2020 2020 2020 7265 735b 6578            res[ex
+000128c0: 6365 6c5f 7661 6c75 652e 6c6f 7765 7228  cel_value.lower(
+000128d0: 295d 203d 206d 6174 6368 6573 5b30 5d0a  )] = matches[0].
+000128e0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000128f0: 2020 2020 2020 2020 2020 6d73 6720 3d20            msg = 
+00012900: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00012910: 2020 6622 4469 6420 6e6f 7420 6669 6e64    f"Did not find
+00012920: 2061 2063 6c6f 7365 206d 6174 6368 2074   a close match t
+00012930: 6f20 7468 6520 6578 6365 6c20 6c69 7374  o the excel list
+00012940: 2065 6e74 7279 2027 7b65 7863 656c 5f76   entry '{excel_v
+00012950: 616c 7565 7d27 2022 0a20 2020 2020 2020  alue}' ".       
+00012960: 2020 2020 2020 2020 2066 2261 6d6f 6e67           f"among
+00012970: 2074 6865 2076 616c 7565 7320 696e 2074   the values in t
+00012980: 6865 204a 534f 4e20 7072 6f6a 6563 7420  he JSON project 
+00012990: 6c69 7374 2027 7b6c 6973 745f 6e61 6d65  list '{list_name
+000129a0: 7d27 220a 2020 2020 2020 2020 2020 2020  }'".            
+000129b0: 290a 2020 2020 2020 2020 2020 2020 7761  ).            wa
+000129c0: 726e 696e 6773 2e77 6172 6e28 4473 7054  rnings.warn(DspT
+000129d0: 6f6f 6c73 5573 6572 5761 726e 696e 6728  oolsUserWarning(
+000129e0: 6d73 6729 290a 0a20 2020 2072 6574 7572  msg))..    retur
+000129f0: 6e20 7265 730a 0a0a 6465 6620 5f6e 6573  n res...def _nes
+00012a00: 7465 645f 6469 6374 5f76 616c 7565 735f  ted_dict_values_
+00012a10: 6974 6572 6174 6f72 2864 6963 7473 3a20  iterator(dicts: 
+00012a20: 6c69 7374 5b64 6963 745b 7374 722c 2041  list[dict[str, A
+00012a30: 6e79 5d5d 2920 2d3e 2049 7465 7261 626c  ny]]) -> Iterabl
+00012a40: 655b 7374 725d 3a0a 2020 2020 2222 220a  e[str]:.    """.
+00012a50: 2020 2020 5969 656c 6420 616c 6c20 7661      Yield all va
+00012a60: 6c75 6573 206f 6620 6120 6e65 7374 6564  lues of a nested
+00012a70: 2064 6963 7469 6f6e 6172 792e 0a0a 2020   dictionary...  
+00012a80: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00012a90: 6469 6374 733a 206c 6973 7420 6f66 206e  dicts: list of n
+00012aa0: 6573 7465 6420 6469 6374 696f 6e61 7269  ested dictionari
+00012ab0: 6573 0a0a 2020 2020 5969 656c 6473 3a0a  es..    Yields:.
+00012ac0: 2020 2020 2020 2020 7661 6c75 6573 206f          values o
+00012ad0: 6620 7468 6520 6e65 7374 6564 2064 6963  f the nested dic
+00012ae0: 7469 6f6e 6172 6965 730a 2020 2020 2222  tionaries.    ""
+00012af0: 220a 2020 2020 2320 4372 6564 6974 733a  ".    # Credits:
+00012b00: 2068 7474 7073 3a2f 2f74 6869 7370 6f69   https://thispoi
+00012b10: 6e74 6572 2e63 6f6d 2f70 7974 686f 6e2d  nter.com/python-
+00012b20: 6974 6572 6174 652d 6c6f 6f70 2d6f 7665  iterate-loop-ove
+00012b30: 722d 616c 6c2d 6e65 7374 6564 2d64 6963  r-all-nested-dic
+00012b40: 7469 6f6e 6172 792d 7661 6c75 6573 2f0a  tionary-values/.
+00012b50: 2020 2020 666f 7220 5f64 6963 7420 696e      for _dict in
+00012b60: 2064 6963 7473 3a0a 2020 2020 2020 2020   dicts:.        
+00012b70: 6966 2022 6e6f 6465 7322 2069 6e20 5f64  if "nodes" in _d
+00012b80: 6963 743a 0a20 2020 2020 2020 2020 2020  ict:.           
+00012b90: 2079 6965 6c64 2066 726f 6d20 5f6e 6573   yield from _nes
+00012ba0: 7465 645f 6469 6374 5f76 616c 7565 735f  ted_dict_values_
+00012bb0: 6974 6572 6174 6f72 285f 6469 6374 5b22  iterator(_dict["
+00012bc0: 6e6f 6465 7322 5d29 0a20 2020 2020 2020  nodes"]).       
+00012bd0: 2069 6620 226e 616d 6522 2069 6e20 5f64   if "name" in _d
+00012be0: 6963 743a 0a20 2020 2020 2020 2020 2020  ict:.           
+00012bf0: 2079 6965 6c64 205f 6469 6374 5b22 6e61   yield _dict["na
+00012c00: 6d65 225d 0a0a 0a64 6566 2063 7265 6174  me"]...def creat
+00012c10: 655f 6a73 6f6e 5f6c 6973 745f 6d61 7070  e_json_list_mapp
+00012c20: 696e 6728 0a20 2020 2070 6174 685f 746f  ing(.    path_to
+00012c30: 5f6a 736f 6e3a 2073 7472 2c0a 2020 2020  _json: str,.    
+00012c40: 6c69 7374 5f6e 616d 653a 2073 7472 2c0a  list_name: str,.
+00012c50: 2020 2020 6c61 6e67 7561 6765 5f6c 6162      language_lab
+00012c60: 656c 3a20 7374 722c 0a29 202d 3e20 6469  el: str,.) -> di
+00012c70: 6374 5b73 7472 2c20 7374 725d 3a0a 2020  ct[str, str]:.  
+00012c80: 2020 2222 220a 2020 2020 4f66 7465 6e2c    """.    Often,
+00012c90: 2064 6174 6120 736f 7572 6365 7320 636f   data sources co
+00012ca0: 6e74 6169 6e20 6c69 7374 2076 616c 7565  ntain list value
+00012cb0: 7320 6e61 6d65 6420 6166 7465 7220 7468  s named after th
+00012cc0: 6520 226c 6162 656c 2220 6f66 2074 6865  e "label" of the
+00012cd0: 204a 534f 4e20 7072 6f6a 6563 7420 6c69   JSON project li
+00012ce0: 7374 206e 6f64 652c 2069 6e73 7465 6164  st node, instead
+00012cf0: 206f 6620 7468 6520 226e 616d 6522 0a20   of the "name". 
+00012d00: 2020 2077 6869 6368 2069 7320 6e65 6564     which is need
+00012d10: 6564 2066 6f72 2074 6865 2060 6473 702d  ed for the `dsp-
+00012d20: 746f 6f6c 7320 786d 6c75 706c 6f61 6460  tools xmlupload`
+00012d30: 2e20 496e 206f 7264 6572 2074 6f20 6372  . In order to cr
+00012d40: 6561 7465 2061 2063 6f72 7265 6374 2058  eate a correct X
+00012d50: 4d4c 2c20 796f 7520 6e65 6564 2061 2064  ML, you need a d
+00012d60: 6963 7469 6f6e 6172 7920 7468 6174 206d  ictionary that m
+00012d70: 6170 7320 7468 650a 2020 2020 226c 6162  aps the.    "lab
+00012d80: 656c 7322 2074 6f20 7468 6569 7220 636f  els" to their co
+00012d90: 7272 6563 7420 226e 616d 6573 222e 0a0a  rrect "names"...
+00012da0: 2020 2020 416c 7465 726e 6174 6976 656c      Alternativel
+00012db0: 792c 2063 6f6e 7369 6465 7220 7573 696e  y, consider usin
+00012dc0: 6720 7468 6520 6d65 7468 6f64 2063 7265  g the method cre
+00012dd0: 6174 655f 6a73 6f6e 5f65 7863 656c 5f6c  ate_json_excel_l
+00012de0: 6973 745f 6d61 7070 696e 6728 292c 2077  ist_mapping(), w
+00012df0: 6869 6368 2061 6c73 6f20 6372 6561 7465  hich also create
+00012e00: 7320 6120 6469 6374 696f 6e61 7279 2c20  s a dictionary, 
+00012e10: 6275 7420 6d61 7073 0a20 2020 2076 616c  but maps.    val
+00012e20: 7565 7320 6672 6f6d 2079 6f75 7220 6461  ues from your da
+00012e30: 7461 2073 6f75 7263 6520 746f 206c 6973  ta source to lis
+00012e40: 7420 6e6f 6465 206e 616d 6573 2066 726f  t node names fro
+00012e50: 6d20 7468 6520 4a53 4f4e 2070 726f 6a65  m the JSON proje
+00012e60: 6374 2066 696c 652c 2062 6173 6564 206f  ct file, based o
+00012e70: 6e20 7369 6d69 6c61 7269 7479 2e0a 0a20  n similarity... 
+00012e80: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00012e90: 2070 6174 685f 746f 5f6a 736f 6e3a 2070   path_to_json: p
+00012ea0: 6174 6820 746f 2061 204a 534f 4e20 7072  ath to a JSON pr
+00012eb0: 6f6a 6563 7420 6669 6c65 2028 612e 6b2e  oject file (a.k.
+00012ec0: 612e 206f 6e74 6f6c 6f67 7929 0a20 2020  a. ontology).   
+00012ed0: 2020 2020 206c 6973 745f 6e61 6d65 3a20       list_name: 
+00012ee0: 6e61 6d65 206f 6620 6120 6c69 7374 2069  name of a list i
+00012ef0: 6e20 7468 6520 4a53 4f4e 2070 726f 6a65  n the JSON proje
+00012f00: 6374 2028 776f 726b 7320 616c 736f 2066  ct (works also f
+00012f10: 6f72 206e 6573 7465 6420 6c69 7374 7329  or nested lists)
+00012f20: 0a20 2020 2020 2020 206c 616e 6775 6167  .        languag
+00012f30: 655f 6c61 6265 6c3a 2077 6869 6368 206c  e_label: which l
+00012f40: 616e 6775 6167 6520 6f66 2074 6865 206c  anguage of the l
+00012f50: 6162 656c 2074 6f20 6368 6f6f 7365 0a0a  abel to choose..
+00012f60: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00012f70: 2020 2020 2061 2064 6963 7469 6f6e 6172       a dictionar
+00012f80: 7920 6f66 2074 6865 2066 6f72 6d20 7b6c  y of the form {l
+00012f90: 6162 656c 3a20 6e61 6d65 7d0a 2020 2020  abel: name}.    
+00012fa0: 2222 220a 2020 2020 7769 7468 206f 7065  """.    with ope
+00012fb0: 6e28 7061 7468 5f74 6f5f 6a73 6f6e 2c20  n(path_to_json, 
+00012fc0: 656e 636f 6469 6e67 3d22 7574 662d 3822  encoding="utf-8"
+00012fd0: 2920 6173 2066 3a0a 2020 2020 2020 2020  ) as f:.        
+00012fe0: 6a73 6f6e 5f66 696c 6520 3d20 6a73 6f6e  json_file = json
+00012ff0: 2e6c 6f61 6428 6629 0a20 2020 206a 736f  .load(f).    jso
+00013000: 6e5f 7375 6273 6574 203d 205b 7820 666f  n_subset = [x fo
+00013010: 7220 7820 696e 206a 736f 6e5f 6669 6c65  r x in json_file
+00013020: 5b22 7072 6f6a 6563 7422 5d5b 226c 6973  ["project"]["lis
+00013030: 7473 225d 2069 6620 785b 226e 616d 6522  ts"] if x["name"
+00013040: 5d20 3d3d 206c 6973 745f 6e61 6d65 5d0a  ] == list_name].
+00013050: 2020 2020 2320 6a73 6f6e 5f73 7562 7365      # json_subse
+00013060: 7420 6973 2061 206c 6973 7420 636f 6e74  t is a list cont
+00013070: 6169 6e69 6e67 206f 6e65 2069 7465 6d2c  aining one item,
+00013080: 206e 616d 656c 7920 7468 6520 6a73 6f6e   namely the json
+00013090: 206f 626a 6563 7420 636f 6e74 6169 6e69   object containi
+000130a0: 6e67 2074 6865 2065 6e74 6972 6520 6a73  ng the entire js
+000130b0: 6f6e 2d6c 6973 740a 0a20 2020 2072 6573  on-list..    res
+000130c0: 203d 207b 7d0a 2020 2020 666f 7220 6c61   = {}.    for la
+000130d0: 6265 6c2c 206e 616d 6520 696e 205f 6e61  bel, name in _na
+000130e0: 6d65 5f6c 6162 656c 5f6d 6170 7065 725f  me_label_mapper_
+000130f0: 6974 6572 6174 6f72 286a 736f 6e5f 7375  iterator(json_su
+00013100: 6273 6574 2c20 6c61 6e67 7561 6765 5f6c  bset, language_l
+00013110: 6162 656c 293a 0a20 2020 2020 2020 2069  abel):.        i
+00013120: 6620 6e61 6d65 2021 3d20 6c69 7374 5f6e  f name != list_n
+00013130: 616d 653a 0a20 2020 2020 2020 2020 2020  ame:.           
+00013140: 2072 6573 5b6c 6162 656c 5d20 3d20 6e61   res[label] = na
+00013150: 6d65 0a20 2020 2020 2020 2020 2020 2072  me.            r
+00013160: 6573 5b6c 6162 656c 2e73 7472 6970 2829  es[label.strip()
+00013170: 2e6c 6f77 6572 2829 5d20 3d20 6e61 6d65  .lower()] = name
+00013180: 0a0a 2020 2020 7265 7475 726e 2072 6573  ..    return res
+00013190: 0a0a 0a64 6566 205f 6e61 6d65 5f6c 6162  ...def _name_lab
+000131a0: 656c 5f6d 6170 7065 725f 6974 6572 6174  el_mapper_iterat
+000131b0: 6f72 280a 2020 2020 6a73 6f6e 5f73 7562  or(.    json_sub
+000131c0: 7365 743a 206c 6973 745b 6469 6374 5b73  set: list[dict[s
+000131d0: 7472 2c20 416e 795d 5d2c 0a20 2020 206c  tr, Any]],.    l
+000131e0: 616e 6775 6167 655f 6c61 6265 6c3a 2073  anguage_label: s
+000131f0: 7472 2c0a 2920 2d3e 2049 7465 7261 626c  tr,.) -> Iterabl
+00013200: 655b 7475 706c 655b 7374 722c 2073 7472  e[tuple[str, str
+00013210: 5d5d 3a0a 2020 2020 2222 220a 2020 2020  ]]:.    """.    
+00013220: 476f 2074 6872 6f75 6768 206c 6973 7420  Go through list 
+00013230: 6e6f 6465 7320 6f66 2061 204a 534f 4e20  nodes of a JSON 
+00013240: 7072 6f6a 6563 7420 616e 6420 7969 656c  project and yiel
+00013250: 6420 286c 6162 656c 2c20 6e61 6d65 2920  d (label, name) 
+00013260: 7061 6972 732e 0a0a 2020 2020 4172 6773  pairs...    Args
+00013270: 3a0a 2020 2020 2020 2020 6a73 6f6e 5f73  :.        json_s
+00013280: 7562 7365 743a 206c 6973 7420 6f66 2044  ubset: list of D
+00013290: 5350 206c 6973 7473 2028 6120 4453 5020  SP lists (a DSP 
+000132a0: 6c69 7374 2062 6569 6e67 2061 2064 6963  list being a dic
+000132b0: 7469 6f6e 6172 7920 7769 7468 2074 6865  tionary with the
+000132c0: 206b 6579 7320 226e 616d 6522 2c20 226c   keys "name", "l
+000132d0: 6162 656c 7322 2061 6e64 2022 6e6f 6465  abels" and "node
+000132e0: 7322 290a 2020 2020 2020 2020 6c61 6e67  s").        lang
+000132f0: 7561 6765 5f6c 6162 656c 3a20 7768 6963  uage_label: whic
+00013300: 6820 6c61 6e67 7561 6765 206f 6620 7468  h language of th
+00013310: 6520 6c61 6265 6c20 746f 2063 686f 6f73  e label to choos
+00013320: 650a 0a20 2020 2059 6965 6c64 733a 0a20  e..    Yields:. 
+00013330: 2020 2020 2020 2028 6c61 6265 6c2c 206e         (label, n
+00013340: 616d 6529 2070 6169 7273 0a20 2020 2022  ame) pairs.    "
+00013350: 2222 0a20 2020 2066 6f72 206e 6f64 6520  "".    for node 
+00013360: 696e 206a 736f 6e5f 7375 6273 6574 3a0a  in json_subset:.
+00013370: 2020 2020 2020 2020 2320 6e6f 6465 2069          # node i
+00013380: 7320 7468 6520 6a73 6f6e 206f 626a 6563  s the json objec
+00013390: 7420 636f 6e74 6169 6e69 6e67 2074 6865  t containing the
+000133a0: 2065 6e74 6972 6520 6a73 6f6e 2d6c 6973   entire json-lis
+000133b0: 740a 2020 2020 2020 2020 6966 2022 6e6f  t.        if "no
+000133c0: 6465 7322 2069 6e20 6e6f 6465 3a0a 2020  des" in node:.  
+000133d0: 2020 2020 2020 2020 2020 2320 226e 6f64            # "nod
+000133e0: 6573 2220 6973 2074 6865 206a 736f 6e20  es" is the json 
+000133f0: 7375 622d 6f62 6a65 6374 2063 6f6e 7461  sub-object conta
+00013400: 696e 696e 6720 7468 6520 656e 7472 6965  ining the entrie
+00013410: 7320 6f66 2074 6865 206a 736f 6e2d 6c69  s of the json-li
+00013420: 7374 0a20 2020 2020 2020 2020 2020 2079  st.            y
+00013430: 6965 6c64 2066 726f 6d20 5f6e 616d 655f  ield from _name_
+00013440: 6c61 6265 6c5f 6d61 7070 6572 5f69 7465  label_mapper_ite
+00013450: 7261 746f 7228 6e6f 6465 5b22 6e6f 6465  rator(node["node
+00013460: 7322 5d2c 206c 616e 6775 6167 655f 6c61  s"], language_la
+00013470: 6265 6c29 0a20 2020 2020 2020 2020 2020  bel).           
+00013480: 2023 2065 6163 6820 7969 656c 6465 6420   # each yielded 
+00013490: 7661 6c75 6520 6973 2061 2028 6c61 6265  value is a (labe
+000134a0: 6c2c 206e 616d 6529 2070 6169 7220 6f66  l, name) pair of
+000134b0: 2061 2073 696e 676c 6520 6c69 7374 2065   a single list e
+000134c0: 6e74 7279 0a20 2020 2020 2020 2069 6620  ntry.        if 
+000134d0: 226e 616d 6522 2069 6e20 6e6f 6465 3a0a  "name" in node:.
+000134e0: 2020 2020 2020 2020 2020 2020 7969 656c              yiel
+000134f0: 6420 286e 6f64 655b 226c 6162 656c 7322  d (node["labels"
+00013500: 5d5b 6c61 6e67 7561 6765 5f6c 6162 656c  ][language_label
+00013510: 5d2c 206e 6f64 655b 226e 616d 6522 5d29  ], node["name"])
+00013520: 0a20 2020 2020 2020 2020 2020 2023 2074  .            # t
+00013530: 6865 2061 6374 7561 6c20 7661 6c75 6573  he actual values
+00013540: 206f 6620 7468 6520 6e61 6d65 2061 6e64   of the name and
+00013550: 2074 6865 206c 6162 656c 0a0a 0a64 6566   the label...def
+00013560: 2077 7269 7465 5f78 6d6c 280a 2020 2020   write_xml(.    
+00013570: 726f 6f74 3a20 6574 7265 652e 5f45 6c65  root: etree._Ele
+00013580: 6d65 6e74 2c0a 2020 2020 6669 6c65 7061  ment,.    filepa
+00013590: 7468 3a20 7374 7220 7c20 5061 7468 2c0a  th: str | Path,.
+000135a0: 2920 2d3e 204e 6f6e 653a 0a20 2020 2022  ) -> None:.    "
+000135b0: 2222 0a20 2020 2057 7269 7465 2074 6865  "".    Write the
+000135c0: 2066 696e 6973 6865 6420 584d 4c20 746f   finished XML to
+000135d0: 2061 2066 696c 652e 0a0a 2020 2020 4172   a file...    Ar
+000135e0: 6773 3a0a 2020 2020 2020 2020 726f 6f74  gs:.        root
+000135f0: 3a20 6574 7265 6520 456c 656d 656e 7420  : etree Element 
+00013600: 7769 7468 2074 6865 2065 6e74 6972 6520  with the entire 
+00013610: 584d 4c20 646f 6375 6d65 6e74 0a20 2020  XML document.   
+00013620: 2020 2020 2066 696c 6570 6174 683a 2077       filepath: w
+00013630: 6865 7265 2074 6f20 7361 7665 2074 6865  here to save the
+00013640: 2066 696c 650a 0a20 2020 2057 6172 6e69   file..    Warni
+00013650: 6e67 3a0a 2020 2020 2020 2020 6966 2074  ng:.        if t
+00013660: 6865 2058 4d4c 2069 7320 6e6f 7420 7661  he XML is not va
+00013670: 6c69 6420 6163 636f 7264 696e 6720 746f  lid according to
+00013680: 2074 6865 2073 6368 656d 610a 2020 2020   the schema.    
+00013690: 2222 220a 2020 2020 6574 7265 652e 696e  """.    etree.in
+000136a0: 6465 6e74 2872 6f6f 742c 2073 7061 6365  dent(root, space
+000136b0: 3d22 2020 2020 2229 0a20 2020 2078 6d6c  ="    ").    xml
+000136c0: 5f73 7472 696e 6720 3d20 6574 7265 652e  _string = etree.
+000136d0: 746f 7374 7269 6e67 280a 2020 2020 2020  tostring(.      
+000136e0: 2020 726f 6f74 2c0a 2020 2020 2020 2020    root,.        
+000136f0: 656e 636f 6469 6e67 3d22 756e 6963 6f64  encoding="unicod
+00013700: 6522 2c0a 2020 2020 2020 2020 7072 6574  e",.        pret
+00013710: 7479 5f70 7269 6e74 3d54 7275 652c 0a20  ty_print=True,. 
+00013720: 2020 2020 2020 2064 6f63 7479 7065 3d27         doctype='
+00013730: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
+00013740: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
+00013750: 462d 3822 3f3e 272c 0a20 2020 2029 0a20  F-8"?>',.    ). 
+00013760: 2020 2078 6d6c 5f73 7472 696e 6720 3d20     xml_string = 
+00013770: 786d 6c5f 7374 7269 6e67 2e72 6570 6c61  xml_string.repla
+00013780: 6365 2872 225c 2722 2c20 2227 2229 0a20  ce(r"\'", "'"). 
+00013790: 2020 2077 6974 6820 6f70 656e 2866 696c     with open(fil
+000137a0: 6570 6174 682c 2022 7722 2c20 656e 636f  epath, "w", enco
+000137b0: 6469 6e67 3d22 7574 662d 3822 2920 6173  ding="utf-8") as
+000137c0: 2066 3a0a 2020 2020 2020 2020 662e 7772   f:.        f.wr
+000137d0: 6974 6528 786d 6c5f 7374 7269 6e67 290a  ite(xml_string).
+000137e0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+000137f0: 2076 616c 6964 6174 655f 786d 6c5f 6669   validate_xml_fi
+00013800: 6c65 2869 6e70 7574 5f66 696c 653d 6669  le(input_file=fi
+00013810: 6c65 7061 7468 290a 2020 2020 2020 2020  lepath).        
+00013820: 7072 696e 7428 6622 5468 6520 584d 4c20  print(f"The XML 
+00013830: 6669 6c65 2077 6173 2073 7563 6365 7373  file was success
+00013840: 6675 6c6c 7920 7361 7665 6420 746f 207b  fully saved to {
+00013850: 6669 6c65 7061 7468 7d22 290a 2020 2020  filepath}").    
+00013860: 6578 6365 7074 2042 6173 6545 7272 6f72  except BaseError
+00013870: 2061 7320 6572 723a 0a20 2020 2020 2020   as err:.       
+00013880: 206d 7367 203d 2028 0a20 2020 2020 2020   msg = (.       
+00013890: 2020 2020 2066 2254 6865 2058 4d4c 2066       f"The XML f
+000138a0: 696c 6520 7761 7320 7375 6363 6573 7366  ile was successf
+000138b0: 756c 6c79 2073 6176 6564 2074 6f20 7b66  ully saved to {f
+000138c0: 696c 6570 6174 687d 2c20 220a 2020 2020  ilepath}, ".    
+000138d0: 2020 2020 2020 2020 6622 6275 7420 7468          f"but th
+000138e0: 6520 666f 6c6c 6f77 696e 6720 5363 6865  e following Sche
+000138f0: 6d61 2076 616c 6964 6174 696f 6e20 6572  ma validation er
+00013900: 726f 7228 7329 206f 6363 7572 7265 643a  ror(s) occurred:
+00013910: 207b 6572 722e 6d65 7373 6167 657d 220a   {err.message}".
+00013920: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00013930: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
+00013940: 4473 7054 6f6f 6c73 5573 6572 5761 726e  DspToolsUserWarn
+00013950: 696e 6728 6d73 6729 290a                 ing(msg)).
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2xml/propertyelement.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/excel2xml/propertyelement.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/id2iri.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/id2iri.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py`

 * *Files 23% similar despite different names*

```diff
@@ -25,50 +25,50 @@
     Raises:
         InputError: if no file was found
     """
     filepath = Path(f"mapping-{shortcode}.csv")
     if not filepath.is_file():
         raise InputError(f"No mapping CSV file was found at {filepath}.")
     df = pd.read_csv(filepath)
-    msg = f"The file '{filepath}' is used to map the internal original filepaths to the internal SIPI image IDs."
+    msg = f"The file '{filepath}' is used to map the internal original filepaths to the internal image IDs."
     print(msg)
     logger.info(msg)
     return dict(zip(df["original"].tolist(), df["derivative"].tolist()))
 
 
-def replace_filepath_with_sipi_id(
-    xml_tree: etree._ElementTree[etree._Element],
-    orig_path_2_id_filename: dict[str, str],
-) -> tuple[etree._ElementTree[etree._Element], IngestInformation]:
+def replace_filepath_with_internal_filename(
+    xml_tree: etree._Element,
+    orig_path_2_asset_id: dict[str, str],
+) -> tuple[etree._Element, IngestInformation]:
     """
     Replace the original filepaths in the <bitstream> tags by the id filenames of the uploaded files.
 
     Args:
         xml_tree: The parsed original XML tree
-        orig_path_2_id_filename: Mapping from original filenames to id filenames from the mapping.csv
+        orig_path_2_asset_id: Mapping from original filenames to asset IDs from the mapping.csv
 
     Returns:
         A copy of the XMl tree, with the replaced filepaths.
         Message informing if all referenced files were uploaded or not.
     """
     no_id_found = []
     used_media_file_paths = []
     new_tree = deepcopy(xml_tree)
     for elem in new_tree.iter():
         if not etree.QName(elem).localname.endswith("bitstream") or not elem.text:
             continue
         img_path = Path(elem.text)
         img_path = img_path.relative_to(Path.cwd()) if img_path.is_absolute() else img_path
         img_path_str = str(img_path)
-        if img_path_str not in orig_path_2_id_filename:
+        if img_path_str not in orig_path_2_asset_id:
             img_path_str = str(img_path.with_suffix(img_path.suffix.lower()))
-        if img_path_str not in orig_path_2_id_filename:
+        if img_path_str not in orig_path_2_asset_id:
             img_path_str = str(img_path.with_suffix(img_path.suffix.upper()))
 
-        if img_path_str in orig_path_2_id_filename:
-            elem.text = orig_path_2_id_filename[img_path_str]
+        if img_path_str in orig_path_2_asset_id:
+            elem.text = orig_path_2_asset_id[img_path_str]
             used_media_file_paths.append(img_path_str)
         else:
             no_id_found.append((cast("etree._Element", elem.getparent()).attrib["id"], str(elem.text)))
 
-    unused_media_paths = [x for x in orig_path_2_id_filename if x not in used_media_file_paths]
+    unused_media_paths = [x for x in orig_path_2_asset_id if x not in used_media_file_paths]
     return new_tree, IngestInformation(unused_mediafiles=unused_media_paths, mediafiles_no_id=no_id_found)
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/ingest_xmlupload/user_information.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/ingest_xmlupload/user_information.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     and the filepaths used in the XML file.
     """
 
     unused_mediafiles: list[str]
     mediafiles_no_id: list[tuple[str, str]]
     maximum_prints: int = 20
     csv_directory_path: Path = field(default=Path.cwd())
-    unused_mediafiles_csv: str = "UnusedMediaUploadedInSipi.csv"
-    mediafiles_no_id_csv: str = "FilesNotUploadedToSipi.csv"
+    unused_mediafiles_csv: str = "UnusedMediaUploaded.csv"
+    mediafiles_no_id_csv: str = "FilesNotUploaded.csv"
 
     def ok_msg(self) -> str | None:
         """
         This function checks if no media was unused or not uploaded.
         If that is the case it returns the message,
         if not, it ends without an effect.
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/create/project_create.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/project/create/project_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """This module handles the ontology creation, update and upload to a DSP server. This includes the creation and update
 of the project, the creation of groups, users, lists, resource classes, properties and cardinalities."""
 
 from pathlib import Path
 from typing import Any
 from typing import Optional
-from typing import Union
 from typing import cast
 
 import regex
 from loguru import logger
 
+from dsp_tools.cli.args import ServerCredentials
 from dsp_tools.commands.excel2json.lists import expand_lists_from_excel
 from dsp_tools.commands.project.create.project_create_lists import create_lists_on_server
 from dsp_tools.commands.project.create.project_validate import validate_project
 from dsp_tools.commands.project.models.context import Context
 from dsp_tools.commands.project.models.group import Group
 from dsp_tools.commands.project.models.helpers import Cardinality
 from dsp_tools.commands.project.models.ontology import Ontology
@@ -924,32 +924,28 @@
             raise UserError(f"ERROR: {msg}")
         prop["gui_attributes"]["hlist"] = deduced_list_name
 
     return properties
 
 
 def create_project(
-    project_file_as_path_or_parsed: Union[str, Path, dict[str, Any]],
-    server: str,
-    user_mail: str,
-    password: str,
+    project_file_as_path_or_parsed: str | Path | dict[str, Any],
+    creds: ServerCredentials,
     verbose: bool = False,
 ) -> bool:
     """
     Creates a project from a JSON project file on a DSP server.
     A project must contain at least one ontology,
     and it may contain lists, users, and groups.
     Severe errors lead to a BaseError,
     while other errors are printed without interrupting the process.
 
     Args:
         project_file_as_path_or_parsed: path to the JSON project definition, or parsed JSON object
-        server: the URL of the DSP server on which the project should be created
-        user_mail: a username (e-mail) who has the permission to create a project
-        password: the user's password
+        creds: credentials to connect to the DSP server
         verbose: prints more information if set to True
 
     Raises:
         UserError:
           - if the project cannot be created
           - if the login fails
           - if an ontology cannot be created
@@ -973,16 +969,16 @@
     project_definition = _prepare_and_validate_project(project_json)
 
     all_lists = _get_all_lists(project_json)
 
     all_ontos = _get_all_ontos(project_json, all_lists)
 
     # establish connection to DSP server
-    con = ConnectionLive(server)
-    con.login(user_mail, password)
+    con = ConnectionLive(creds.server)
+    con.login(creds.user, creds.password)
 
     # create project on DSP server
     info_str = f"Create project '{project_definition.shortname}' ({project_definition.shortcode})..."
     print(info_str)
     logger.info(info_str)
     project_remote, success = _create_project_on_server(
         project_definition=project_definition,
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/create/project_create_lists.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/project/create/project_create_lists.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Any
 from typing import Optional
 from typing import Union
 
 from loguru import logger
 
+from dsp_tools.cli.args import ServerCredentials
 from dsp_tools.commands.excel2json.lists import expand_lists_from_excel
 from dsp_tools.commands.project.create.project_validate import validate_project
 from dsp_tools.commands.project.models.listnode import ListNode
 from dsp_tools.commands.project.models.project import Project
 from dsp_tools.models.exceptions import BaseError
 from dsp_tools.models.exceptions import UserError
 from dsp_tools.utils.connection import Connection
@@ -130,32 +131,28 @@
         print(f"    Created list '{new_lst['name']}'.")
 
     return current_project_lists, overall_success
 
 
 def create_lists(
     project_file_as_path_or_parsed: Union[str, dict[str, Any]],
-    server: str,
-    user: str,
-    password: str,
+    creds: ServerCredentials,
 ) -> tuple[dict[str, Any], bool]:
     """
     This method accepts a JSON project definition,
     expands the Excel sheets referenced in its "lists" section,
     connects to a DSP server,
     and uploads the "lists" section to the server.
 
     The project must already exist on the DSP server.
     If a list with the same name is already existing in this project on the DSP server, this list is skipped.
 
     Args:
         project_file_as_path_or_parsed: path to the JSON project definition, or parsed JSON object
-        server: URL of the DSP server
-        user: Username (e-mail) for the DSP server, must have the permissions to create a project
-        password: Password of the user
+        creds: credentials to connect to the DSP server
 
     Raises:
         UserError:
           - if the project cannot be read from the server
           - if the connection to the DSP server cannot be established
 
         BaseError:
@@ -180,16 +177,16 @@
         return {}, True
     lists_to_create = expand_lists_from_excel(project_definition["project"]["lists"])
     project_definition["project"]["lists"] = lists_to_create
     validate_project(project_definition, expand_lists=False)
     print("JSON project file is syntactically correct and passed validation.")
 
     # connect to the DSP server
-    con = ConnectionLive(server)
-    con.login(user, password)
+    con = ConnectionLive(creds.server)
+    con.login(creds.user, creds.password)
 
     # retrieve the project
     shortcode = project_definition["project"]["shortcode"]
     project_local = Project(con=con, shortcode=shortcode)
     try:
         project_remote = project_local.read()
     except BaseError:
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/create/project_validate.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/project/create/project_validate.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/get.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/project/get.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,50 @@
 import json
 import warnings
 from typing import Any
 
 import regex
 
+from dsp_tools.cli.args import ServerCredentials
 from dsp_tools.commands.project.models.group import Group
 from dsp_tools.commands.project.models.listnode import ListNode
 from dsp_tools.commands.project.models.ontology import Ontology
 from dsp_tools.commands.project.models.project import Project
 from dsp_tools.commands.project.models.user import User
 from dsp_tools.models.exceptions import BaseError
 from dsp_tools.utils.connection import Connection
 from dsp_tools.utils.connection_live import ConnectionLive
 
 
 def get_project(
     project_identifier: str,
     outfile_path: str,
-    server: str,
-    user: str | None = None,
-    password: str | None = None,
+    creds: ServerCredentials,
     verbose: bool = False,
 ) -> bool:
     """
     This function writes a project from a DSP server into a JSON file.
 
     Args:
         project_identifier: the project identifier, either shortcode, shortname or IRI of the project
         outfile_path: the output file the JSON content should be written to
-        server: the DSP server where the data should be read from
-        user: the user (e-mail) who sends the request
-        password: the password of the user who sends the request
+        creds: the credentials to access the DSP server
         verbose: verbose option for the command, if used more output is given to the user
 
     Raises:
         BaseError: if something went wrong
 
     Returns:
         True if the process finishes without errors
     """
-    con = ConnectionLive(server)
-    if user and password:
-        try:
-            con.login(user, password)
-        except BaseError:
-            warnings.warn("WARNING: Missing or wrong credentials. You won't get data about the users of this project.")
+    con = ConnectionLive(creds.server)
+    try:
+        con.login(creds.user, creds.password)
+    except BaseError:
+        warnings.warn("WARNING: Missing or wrong credentials. You won't get data about the users of this project.")
 
     project = _create_project(con, project_identifier)
 
     project = project.read()
     project_obj = project.createDefinitionFileObj()
 
     project_obj["groups"] = _get_groups(con, str(project.iri), verbose)
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/context.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/project/models/context.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/group.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/project/models/group.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/helpers.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/project/models/helpers.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/listnode.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/project/models/listnode.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/ontology.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/project/models/ontology.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/project.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/project/models/project.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/propertyclass.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/project/models/propertyclass.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/resourceclass.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/project/models/resourceclass.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/user.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/project/models/user.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,63 +1,66 @@
 import pickle
 import sys
 
 from loguru import logger
 from termcolor import colored
 
+from dsp_tools.cli.args import ServerCredentials
 from dsp_tools.commands.xmlupload.list_client import ListClient
 from dsp_tools.commands.xmlupload.list_client import ListClientLive
-from dsp_tools.commands.xmlupload.models.sipi import Sipi
+from dsp_tools.commands.xmlupload.models.ingest import AssetClient
+from dsp_tools.commands.xmlupload.models.ingest import BulkIngestedAssetClient
+from dsp_tools.commands.xmlupload.models.ingest import DspIngestClientLive
+from dsp_tools.commands.xmlupload.models.upload_clients import UploadClients
 from dsp_tools.commands.xmlupload.models.upload_state import UploadState
 from dsp_tools.commands.xmlupload.project_client import ProjectClient
 from dsp_tools.commands.xmlupload.project_client import ProjectClientLive
 from dsp_tools.commands.xmlupload.upload_config import UploadConfig
-from dsp_tools.commands.xmlupload.xmlupload import cleanup_upload
-from dsp_tools.commands.xmlupload.xmlupload import upload_resources
+from dsp_tools.commands.xmlupload.xmlupload import execute_upload
 from dsp_tools.utils.connection_live import ConnectionLive
 
 
-def resume_xmlupload(server: str, user: str, password: str, sipi: str, skip_first_resource: bool = False) -> bool:
+def resume_xmlupload(creds: ServerCredentials, skip_first_resource: bool = False) -> bool:
     """
     Resume an interrupted xmlupload.
 
     Args:
-        server: the DSP server where the data should be imported
-        user: the user (e-mail) with which the data should be imported
-        password: the password of the user with which the data should be imported
-        sipi: the sipi instance to be used
+        creds: credentials to access the DSP server
         skip_first_resource: if this flag is set, the first resource of the pending resources is removed
 
     Returns:
         True if all resources could be uploaded without errors; False if one of the resources could not be
         uploaded because there is an error in it
     """
+    server = creds.server
     upload_state = _read_upload_state_from_disk(server)
     if skip_first_resource:
         _skip_first_resource(upload_state)
 
     _print_and_log(upload_state, server)
 
     con = ConnectionLive(server)
-    con.login(user, password)
-    sipi_con = ConnectionLive(sipi, token=con.get_token())
-    sipi_server = Sipi(sipi_con)
+    con.login(creds.user, creds.password)
+
+    ingest_client: AssetClient
+    if upload_state.config.media_previously_uploaded:
+        ingest_client = BulkIngestedAssetClient()
+    else:
+        ingest_client = DspIngestClientLive(
+            dsp_ingest_url=creds.dsp_ingest_url,
+            token=con.get_token(),
+            shortcode=upload_state.config.shortcode,
+            imgdir=".",
+        )
 
     project_client: ProjectClient = ProjectClientLive(con, upload_state.config.shortcode)
     list_client: ListClient = ListClientLive(con, project_client.get_project_iri())
+    clients = UploadClients(ingest_client, project_client, list_client)
 
-    upload_resources(
-        upload_state=upload_state,
-        imgdir=".",
-        sipi_server=sipi_server,
-        project_client=project_client,
-        list_client=list_client,
-    )
-
-    return cleanup_upload(upload_state)
+    return execute_upload(clients, upload_state)
 
 
 def _read_upload_state_from_disk(server: str) -> UploadState:
     save_location = UploadConfig().with_server_info(server, "foo").diagnostics.save_location
     with open(save_location, "rb") as f:
         saved_state: UploadState = pickle.load(f)  # noqa: S301 (deserialization of untrusted data)
     return saved_state
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/rosetta.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/rosetta.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import shutil
 import subprocess
 from pathlib import Path
 
+from dsp_tools.cli.args import ServerCredentials
 from dsp_tools.commands.project.create.project_create import create_project
-from dsp_tools.commands.xmlupload.upload_config import UploadConfig
 from dsp_tools.commands.xmlupload.xmlupload import xmlupload
 from dsp_tools.models.exceptions import UserError
 
 
 def _update_possibly_existing_repo(rosetta_folder: Path) -> bool:
     """
     Makes an attempt to pull the latest version of rosetta from GitHub.
@@ -60,19 +60,18 @@
     Args:
         rosetta_folder: path to the clone
 
     Returns:
         True if the project could be created without problems, False if something went wrong during the creation process
     """
     print("Execute 'dsp-tools create rosetta.json'...")
+    creds = ServerCredentials(server="http://0.0.0.0:3333", user="root@example.com", password="test")
     return create_project(
         project_file_as_path_or_parsed=rosetta_folder / "rosetta.json",
-        server="http://0.0.0.0:3333",
-        user_mail="root@example.com",
-        password="test",
+        creds=creds,
         verbose=False,
     )
 
 
 def _upload_xml(rosetta_folder: Path) -> bool:
     """
     Uplaod the rosetta data on the locally running DSP stack.
@@ -80,22 +79,24 @@
     Args:
         rosetta_folder: path to the clone
 
     Returns:
         True if all data could be uploaded without problems, False if something went wrong during the upload process
     """
     print("Execute 'dsp-tools xmlupload rosetta.xml'...")
-    return xmlupload(
-        input_file=rosetta_folder / "rosetta.xml",
-        server="http://0.0.0.0:3333",
+    creds = ServerCredentials(
         user="root@example.com",
         password="test",
+        server="http://0.0.0.0:3333",
+        dsp_ingest_url="http://0.0.0.0:3340",
+    )
+    return xmlupload(
+        input_file=rosetta_folder / "rosetta.xml",
+        creds=creds,
         imgdir=str(rosetta_folder),
-        sipi="http://0.0.0.0:1024",
-        config=UploadConfig(),
     )
 
 
 def upload_rosetta() -> bool:
     """
     This method clones https://github.com/dasch-swiss/082E-rosetta-scripts
     into ~/.dsp-tools/rosetta.
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/start_stack.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/start_stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 @dataclass(frozen=True)
 class StackConfiguration:
     """
     Groups together configuration information for the StackHandler.
 
     Args:
-        max_file_size: max. multimedia file size allowed by SIPI, in MB (max: 100'000)
+        max_file_size: max. multimedia file size allowed for ingest, in MB (max: 100'000)
         enforce_docker_system_prune: if True, prune Docker without asking the user
         suppress_docker_system_prune: if True, don't prune Docker (and don't ask)
         latest_dev_version: if True, start DSP-API from repo's main branch, instead of the latest deployed version
     """
 
     max_file_size: Optional[int] = None
     enforce_docker_system_prune: bool = False
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/template.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/template.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/ark2iri.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/ark2iri.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/iri_resolver.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/iri_resolver.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/list_client.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/list_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/deserialise/deserialise_value.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/deserialise/deserialise_value.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/deserialise/xmlpermission.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/deserialise/xmlpermission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/namespace_context.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/namespace_context.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,10 @@
-from dataclasses import dataclass
-from dataclasses import field
-
 from rdflib.namespace import Namespace
 
 
-@dataclass
-class NamespaceContext:
-    onto_dict: dict[str, Namespace]
-    knora_api: Namespace = field(default=Namespace("http://api.knora.org/ontology/knora-api/v2#"))
-    salsah_gui: Namespace = field(default=Namespace("http://api.knora.org/ontology/salsah-gui/v2#"))
-
-
 def get_default_json_ld_context() -> dict[str, str]:
     """
     Returns the JSON-LD context as a dictionary.
 
     Returns:
         JSON-LD context as a dictionary.
     """
@@ -24,14 +14,22 @@
         "rdf": "http://www.w3.org/1999/02/22-rdf-syntax-ns#",
         "rdfs": "http://www.w3.org/2000/01/rdf-schema#",
         "owl": "http://www.w3.org/2002/07/owl#",
         "xsd": "http://www.w3.org/2001/XMLSchema#",
     }
 
 
+def make_namespace_dict_from_onto_names(ontos: dict[str, str]) -> dict[str, Namespace]:
+    """Provided a dictionary of ontology names and IRIs, returns a dictionary of Namespace objects."""
+    ontos = correct_project_context_namespaces(ontos)
+    namespaces = {k: Namespace(v) for k, v in ontos.items()}
+    namespaces.update({"knora-api": Namespace("http://api.knora.org/ontology/knora-api/v2#")})
+    return namespaces
+
+
 def correct_project_context_namespaces(ontos: dict[str, str]) -> dict[str, str]:
     """Add the hashtag to make it a valid namespace."""
     return {k: f"{v}#" for k, v in ontos.items()}
 
 
 def get_json_ld_context_for_project(ontos: dict[str, str]) -> dict[str, str]:
     """Provided a dictionary of ontology names and IRIs, returns a JSON-LD context for the project."""
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/permission.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/permission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/serialise/serialise_value.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/serialise/serialise_value.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/upload_state.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/upload_state.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from dataclasses import dataclass
+from dataclasses import field
 
 from dsp_tools.commands.xmlupload.iri_resolver import IriResolver
 from dsp_tools.commands.xmlupload.models.deserialise.xmlresource import XMLResource
 from dsp_tools.commands.xmlupload.models.permission import Permissions
 from dsp_tools.commands.xmlupload.stash.stash_models import Stash
 from dsp_tools.commands.xmlupload.upload_config import UploadConfig
 
@@ -10,12 +11,12 @@
 @dataclass
 class UploadState:
     """
     Save the state of an xmlupload, so that after an interruption, it can be resumed.
     """
 
     pending_resources: list[XMLResource]
-    failed_uploads: list[str]
-    iri_resolver: IriResolver
     pending_stash: Stash | None
     config: UploadConfig
     permissions_lookup: dict[str, Permissions]
+    failed_uploads: list[str] = field(default_factory=list)
+    iri_resolver: IriResolver = field(default_factory=IriResolver)
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/ontology_client.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/ontology_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/project_client.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/project_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,22 +54,23 @@
 def _get_project_info_from_server(con: Connection, shortcode: str) -> ProjectInfo:
     project_iri = _get_project_iri_from_server(con, shortcode)
     ontologies = _get_ontologies_from_server(con, project_iri)
     return ProjectInfo(project_iri=project_iri, ontology_iris=ontologies)
 
 
 def _get_project_iri_from_server(con: Connection, shortcode: str) -> str:
+    url = f"/admin/projects/shortcode/{shortcode}"
     try:
-        url = f"/admin/projects/shortcode/{shortcode}"
         res = con.get(url)
-        iri: str = res["project"]["id"]
     except BaseError as e:
         raise UserError(f"A project with shortcode {shortcode} could not be found on the DSP server") from e
-    except KeyError as e:
-        raise BaseError(f"Unexpected response from server: {res}") from e
+
+    iri: str | None = res.get("project", {}).get("id")
+    if not iri:
+        raise BaseError(f"Unexpected response from server: {res}")
     return iri
 
 
 def _get_ontologies_from_server(con: Connection, project_iri: str) -> list[str]:
     try:
         iri = quote_plus(project_iri)
         url = f"/v2/ontologies/metadata/{iri}"
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,40 @@
 from __future__ import annotations
 
 from pathlib import Path
-from typing import Any
-from typing import Union
 
 import regex
-from loguru import logger
 from lxml import etree
 
 from dsp_tools.models.exceptions import UserError
 from dsp_tools.utils.iri_util import is_resource_iri
-from dsp_tools.utils.xml_utils import parse_and_clean_xml_file
+from dsp_tools.utils.xml_utils import parse_xml_file
+from dsp_tools.utils.xml_utils import remove_comments_from_element_tree
+from dsp_tools.utils.xml_utils import remove_qnames_and_transform_special_tags
 from dsp_tools.utils.xml_validation import validate_xml
 
 
-def validate_and_parse_xml_file(
-    imgdir: str,
-    input_file: Union[str, Path, etree._ElementTree[Any]],
-    preprocessing_done: bool,
-) -> tuple[str, etree._Element, str]:
-    """
-    This function takes an element tree or a path to an XML file.
-    It validates the file against the XML schema.
-    It checks if all the mentioned bitstream files are in the specified location.
-    It retrieves the shortcode and default ontology from the XML file.
+def validate_and_parse(input_file: Path) -> tuple[etree._Element, str, str]:
+    """Parse and validate an XML file.
 
     Args:
-        imgdir: directory to the bitstream files
-        input_file: file or etree that will be processed
-        preprocessing_done: True if the bitstream files have already been processed
+        input_file: Path to the XML file
 
     Returns:
-        The ontology name, the parsed XML file and the shortcode of the project
+        The root element of the parsed XML file, the shortcode, and the default ontology
     """
-    validate_xml(input_file=input_file)
-    root = parse_and_clean_xml_file(input_file=input_file)
+    root = parse_xml_file(input_file)
+    root = remove_comments_from_element_tree(root)
+
+    validate_xml(root)
+    root = remove_qnames_and_transform_special_tags(root)
     _check_if_link_targets_exist(root)
-    if not preprocessing_done:
-        _check_if_bitstreams_exist(root=root, imgdir=imgdir)
     shortcode = root.attrib["shortcode"]
     default_ontology = root.attrib["default-ontology"]
-    logger.info(f"Validated and parsed the XML file. {shortcode=:} and {default_ontology=:}")
-    return default_ontology, root, shortcode
+    return root, shortcode, default_ontology
 
 
 def _check_if_link_targets_exist(root: etree._Element) -> None:
     """
     Make sure that all targets of links (resptr and salsah-links)
     are either IRIs or IDs that exist in the present XML file.
 
@@ -86,18 +75,15 @@
     for inv in invalid_link_values:
         prop_name = next(inv.iterancestors(tag="text-prop")).attrib["name"]
         res_id = next(inv.iterancestors(tag="resource")).attrib["id"]
         errors.append(f"Resource '{res_id}', property '{prop_name}' has an invalid link target '{inv.attrib['href']}'")
     return errors
 
 
-def _check_if_bitstreams_exist(
-    root: etree._Element,
-    imgdir: str,
-) -> None:
+def check_if_bitstreams_exist(root: etree._Element, imgdir: str) -> None:
     """
     Make sure that all bitstreams referenced in the XML file exist in the imgdir.
 
     Args:
         root: parsed XML file
         imgdir: folder where the bitstreams are stored
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/resource_create_client.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/resource_create_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,34 +2,45 @@
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any
 from typing import assert_never
 from typing import cast
 
 from loguru import logger
+from rdflib import RDF
+from rdflib import BNode
+from rdflib import Graph
+from rdflib import Literal
+from rdflib import Namespace
+from rdflib import URIRef
 
 from dsp_tools.commands.xmlupload.ark2iri import convert_ark_v0_to_resource_iri
 from dsp_tools.commands.xmlupload.iri_resolver import IriResolver
 from dsp_tools.commands.xmlupload.models.deserialise.deserialise_value import XMLProperty
 from dsp_tools.commands.xmlupload.models.deserialise.deserialise_value import XMLValue
 from dsp_tools.commands.xmlupload.models.deserialise.xmlresource import BitstreamInfo
 from dsp_tools.commands.xmlupload.models.deserialise.xmlresource import XMLResource
 from dsp_tools.commands.xmlupload.models.formatted_text_value import FormattedTextValue
 from dsp_tools.commands.xmlupload.models.namespace_context import get_json_ld_context_for_project
+from dsp_tools.commands.xmlupload.models.namespace_context import make_namespace_dict_from_onto_names
 from dsp_tools.commands.xmlupload.models.permission import Permissions
+from dsp_tools.commands.xmlupload.models.serialise.jsonld_serialiser import serialise_property_graph
 from dsp_tools.commands.xmlupload.models.serialise.serialise_value import SerialiseProperty
 from dsp_tools.commands.xmlupload.models.serialise.serialise_value import SerialiseURI
 from dsp_tools.commands.xmlupload.models.serialise.serialise_value import SerialiseValue
 from dsp_tools.models.exceptions import BaseError
+from dsp_tools.models.exceptions import InputError
 from dsp_tools.models.exceptions import PermissionNotExistsError
 from dsp_tools.models.exceptions import UserError
 from dsp_tools.utils.connection import Connection
 from dsp_tools.utils.date_util import parse_date_string
 from dsp_tools.utils.iri_util import is_resource_iri
 
+KNORA_API = Namespace("http://api.knora.org/ontology/knora-api/v2#")
+
 
 @dataclass(frozen=True)
 class ResourceCreateClient:
     """client class that creates resources on a DSP server."""
 
     con: Connection
     project_iri: str
@@ -45,28 +56,29 @@
         bitstream_information: BitstreamInfo | None,
     ) -> str:
         """Creates a resource on the DSP server, and returns its IRI"""
         logger.info(
             f"Attempting to create resource {resource.res_id} (label: {resource.label}, iri: {resource.iri})..."
         )
         resource_dict = self._make_resource_with_values(resource, bitstream_information)
-        headers = {"X-Asset-Ingested": "true"} if self.media_previously_ingested else None
-        res = self.con.post(route="/v2/resources", data=resource_dict, headers=headers)
+        res = self.con.post(route="/v2/resources", data=resource_dict, headers={"X-Asset-Ingested": "true"})
         return cast(str, res["@id"])
 
     def _make_resource_with_values(
         self,
         resource: XMLResource,
         bitstream_information: BitstreamInfo | None,
     ) -> dict[str, Any]:
+        res_bnode = BNode()
+        namespaces = make_namespace_dict_from_onto_names(self.project_onto_dict)
         res = self._make_resource(
             resource=resource,
             bitstream_information=bitstream_information,
         )
-        vals = self._make_values(resource)
+        vals = self._make_values(resource, res_bnode, namespaces)
         res.update(vals)
         return res
 
     def _make_resource(
         self,
         resource: XMLResource,
         bitstream_information: BitstreamInfo | None,
@@ -95,55 +107,68 @@
                 "@type": "xsd:dateTimeStamp",
                 "@value": str(resource.creation_date),
             }
         if bitstream_information:
             res.update(_make_bitstream_file_value(bitstream_information))
         return res
 
-    def _make_values(self, resource: XMLResource) -> dict[str, Any]:
+    def _make_values(self, resource: XMLResource, res_bnode: BNode, namespaces: dict[str, Namespace]) -> dict[str, Any]:
         def prop_name(p: XMLProperty) -> str:
             if p.valtype != "resptr":
                 return p.name
             elif p.name == "knora-api:isSegmentOf" and resource.restype == "knora-api:VideoSegment":
                 return "knora-api:isVideoSegmentOfValue"
             elif p.name == "knora-api:isSegmentOf" and resource.restype == "knora-api:AudioSegment":
                 return "knora-api:isAudioSegmentOfValue"
             else:
                 return f"{p.name}Value"
 
         def make_values(p: XMLProperty) -> list[dict[str, Any]]:
             return [self._make_value(v, p.valtype) for v in p.values]
 
         properties_serialised = {}
+        properties_graph = Graph()
+        last_prop_name = None
 
         for prop in resource.properties:
             match prop.valtype:
                 case "uri":
                     properties_serialised.update(_serialise_uri_prop(prop, self.permissions_lookup))
+                case "integer":
+                    int_prop_name = self._get_absolute_prop_iri(prop.name, namespaces)
+                    int_graph = _make_integer_prop(prop, res_bnode, int_prop_name, self.permissions_lookup)
+                    properties_graph += int_graph
+                    last_prop_name = int_prop_name
                 case _:
                     properties_serialised.update({prop_name(prop): make_values(prop)})
-
+        if last_prop_name:
+            serialised_graph_props = serialise_property_graph(properties_graph, last_prop_name)
+            properties_serialised.update(serialised_graph_props)
         return properties_serialised
 
+    def _get_absolute_prop_iri(self, prefixed_prop: str, namespaces: dict[str, Namespace]) -> URIRef:
+        prefix, prop = prefixed_prop.split(":", maxsplit=1)
+        if not (namespace := namespaces.get(prefix)):
+            raise InputError(f"Could not find namespace for prefix: {prefix}")
+        return namespace[prop]
+
     def _make_value(self, value: XMLValue, value_type: str) -> dict[str, Any]:
         match value_type:
             case "boolean":
                 res = _make_boolean_value(value)
             case "color":
                 res = _make_color_value(value)
             case "date":
                 res = _make_date_value(value)
             case "decimal":
                 res = _make_decimal_value(value)
             case "geometry":
                 res = _make_geometry_value(value)
             case "geoname":
                 res = _make_geoname_value(value)
-            case "integer":
-                res = _make_integer_value(value)
             case "interval":
                 res = _make_interval_value(value)
             case "resptr":
                 res = _make_link_value(value, self.iri_resolver)
             case "list":
                 res = _make_list_value(value, self.listnode_lookup)
             case "text":
@@ -272,20 +297,37 @@
 def _make_geoname_value(value: XMLValue) -> dict[str, Any]:
     return {
         "@type": "knora-api:GeonameValue",
         "knora-api:geonameValueAsGeonameCode": value.value,
     }
 
 
-def _make_integer_value(value: XMLValue) -> dict[str, Any]:
+def _make_integer_prop(
+    prop: XMLProperty, res_bn: BNode, prop_name: URIRef, permissions_lookup: dict[str, Permissions]
+) -> Graph:
+    g = Graph()
+    for value in prop.values:
+        single_val_bn = BNode()
+        g.add((res_bn, prop_name, single_val_bn))
+        g += _make_integer_value(value, single_val_bn, permissions_lookup)
+    return g
+
+
+def _make_integer_value(value: XMLValue, val_bn: BNode, permissions_lookup: dict[str, Permissions]) -> Graph:
     s = _assert_is_string(value.value)
-    return {
-        "@type": "knora-api:IntValue",
-        "knora-api:intValueAsInt": int(s),
-    }
+    g = Graph()
+    g.add((val_bn, RDF.type, KNORA_API.IntValue))
+    g.add((val_bn, KNORA_API.intValueAsInt, Literal(int(s))))
+    if value.permissions:
+        if not (per := permissions_lookup.get(value.permissions)):
+            raise PermissionNotExistsError(f"Could not find permissions for value: {value.permissions}")
+        g.add((val_bn, KNORA_API.hasPermissions, Literal(str(per))))
+    if value.comment:
+        g.add((val_bn, KNORA_API.valueHasComment, Literal(value.comment)))
+    return g
 
 
 def _make_interval_value(value: XMLValue) -> dict[str, Any]:
     s = _assert_is_string(value.value)
     match s.split(":", 1):
         case [start, end]:
             return {
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/resource_multimedia.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/models/deserialise/xmlresource.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,126 +1,105 @@
-from __future__ import annotations
+from dataclasses import dataclass
+from typing import Optional
 
-from datetime import datetime
-from pathlib import Path
-
-from loguru import logger
+from lxml import etree
 
 from dsp_tools.commands.xmlupload.models.deserialise.deserialise_value import XMLBitstream
-from dsp_tools.commands.xmlupload.models.deserialise.xmlresource import BitstreamInfo
-from dsp_tools.commands.xmlupload.models.deserialise.xmlresource import XMLResource
+from dsp_tools.commands.xmlupload.models.deserialise.deserialise_value import XMLProperty
 from dsp_tools.commands.xmlupload.models.permission import Permissions
-from dsp_tools.commands.xmlupload.models.sipi import Sipi
-from dsp_tools.models.exceptions import PermanentConnectionError
-
-
-def handle_media_info(
-    resource: XMLResource,
-    media_previously_uploaded: bool,
-    sipi_server: Sipi,
-    imgdir: str,
-    permissions_lookup: dict[str, Permissions],
-) -> tuple[bool, None | BitstreamInfo]:
-    """
-    This function checks if a resource has a bitstream.
-    If not, it reports success and returns None.
-    If the file has been uploaded it returns the internal ID.
-    Else it uploads it and returns the internal ID.
-
-
-    Args:
-        resource: resource holding the bitstream
-        media_previously_uploaded: True if the image is already in SIPI
-        sipi_server: server to upload
-        imgdir: directory of the file
-        permissions_lookup: dictionary that contains the permission name as string and the corresponding Python object
-
-    Returns:
-        If the bitstream could be processed successfully, then the function returns True and the new internal ID.
-        If there was no bitstream, it returns True and None.
-        If the upload was not successful, it returns False and None.
-    """
-    bitstream = resource.bitstream
-    success = True
-    bitstream_information: None | BitstreamInfo = None
-
-    if not bitstream:
-        return success, bitstream_information
-    if not media_previously_uploaded:
-        bitstream_information = _handle_media_upload(
-            resource=resource,
-            bitstream=bitstream,
-            permissions_lookup=permissions_lookup,
-            sipi_server=sipi_server,
-            imgdir=imgdir,
-        )
-        if not bitstream_information:
-            success = False
-    else:
-        bitstream_information = resource.get_bitstream_information(bitstream.value, permissions_lookup)
-    return success, bitstream_information
-
-
-def _handle_media_upload(
-    resource: XMLResource,
-    bitstream: XMLBitstream,
-    permissions_lookup: dict[str, Permissions],
-    sipi_server: Sipi,
-    imgdir: str,
-) -> BitstreamInfo | None:
-    """
-    Upload a bitstream file to SIPI
-
-    Args:
-        resource: resource holding the bitstream
-        bitstream: the bitstream object
-        permissions_lookup: dictionary that contains the permission name as string and the corresponding Python object
-        sipi_server: server to upload
-        imgdir: directory of the file
-
-    Returns:
-        The information from sipi which is needed to establish a link from the resource
-    """
-    try:
-        resource_bitstream = _upload_bitstream(
-            resource=resource,
-            sipi_server=sipi_server,
-            imgdir=imgdir,
-            permissions_lookup=permissions_lookup,
-        )
-        msg = f"Uploaded file '{bitstream.value}'"
-        print(f"{datetime.now()}: {msg}")
-        logger.info(msg)
-        return resource_bitstream
-    except PermanentConnectionError as err:
-        msg = f"Unable to upload file '{bitstream.value}' of resource '{resource.label}' ({resource.res_id})"
-        print(f"{datetime.now()}: WARNING: {msg}: {err.message}")
-        logger.opt(exception=True).warning(msg)
-        return None
-
-
-def _upload_bitstream(
-    resource: XMLResource,
-    sipi_server: Sipi,
-    imgdir: str,
-    permissions_lookup: dict[str, Permissions],
-) -> BitstreamInfo | None:
-    """
-    This function uploads a specified bitstream file to SIPI and then returns the file information from SIPI.
+from dsp_tools.models.datetimestamp import DateTimeStamp
 
-    Args:
-        resource: resource that has a bitstream
-        sipi_server: server to upload
-        imgdir: directory of the file
-        permissions_lookup: dictionary that contains the permission name as string and the corresponding Python object
 
-    Returns:
-        The information from sipi which is needed to establish a link from the resource
+@dataclass(frozen=True)
+class BitstreamInfo:
     """
-    if not resource.bitstream:
-        return None
-    img = sipi_server.upload_bitstream(Path(imgdir) / Path(resource.bitstream.value))
-    internal_file_name_bitstream = img["uploadedFiles"][0]["internalFilename"]
-    return resource.get_bitstream_information(
-        internal_file_name_bitstream=internal_file_name_bitstream,
-        permissions_lookup=permissions_lookup,
-    )
+    Represents a bitstream object,
+    consisting of its file name on the local file system,
+    the internal file name assigned by the ingest service
+    and optionally its permissions.
+    """
+
+    local_file: str
+    internal_file_name: str
+    permissions: Permissions | None = None
+
+
+class XMLResource:
+    """
+    Represents a resource in the XML used for data import.
+
+    Attributes:
+        res_id: The unique id of the resource
+        iri: The custom IRI of the resource
+        ark: The custom ARK of the resource
+        label: The label of the resource
+        restype: The type of the resource
+        permissions: The reference to the permissions set for this resource
+        creation_date: The creation date of the resource
+        bitstream: The bitstream object belonging to the resource
+        properties: The list of properties of the resource
+    """
+
+    res_id: str
+    iri: Optional[str]
+    ark: Optional[str]
+    label: str
+    restype: str
+    permissions: Optional[str]
+    creation_date: Optional[DateTimeStamp]
+    bitstream: Optional[XMLBitstream]
+    properties: list[XMLProperty]
+
+    def __init__(self, node: etree._Element, default_ontology: str) -> None:
+        """
+        Constructor that parses a resource node from the XML DOM
+
+        Args:
+            node: The DOM node to be processed representing a resource (which is a child of the <knora> element)
+            default_ontology: The default ontology (given in the attribute default-ontology of the <knora> element)
+        """
+        self.res_id = node.attrib["id"]
+        self.iri = node.attrib.get("iri")
+        self.ark = node.attrib.get("ark")
+        self.creation_date = None
+        if node.attrib.get("creation_date"):
+            self.creation_date = DateTimeStamp(node.attrib.get("creation_date"))
+        self.label = node.attrib["label"]
+        # get the resource type which is in format namespace:resourcetype, p.ex. rosetta:Image
+        tmp_res_type = node.attrib["restype"].split(":")
+        if len(tmp_res_type) > 1:
+            if tmp_res_type[0]:
+                self.restype = node.attrib["restype"]
+            else:
+                # replace an empty namespace with the default ontology name
+                self.restype = default_ontology + ":" + tmp_res_type[1]
+        else:
+            self.restype = "knora-api:" + tmp_res_type[0]
+        self.permissions = node.attrib.get("permissions")
+        self.bitstream = None
+        self.properties = []
+        for subnode in node:
+            if subnode.tag == "bitstream":
+                self.bitstream = XMLBitstream(subnode)
+            else:
+                # get the property type which is in format type-prop, p.ex. <decimal-prop>
+                prop_type, _ = subnode.tag.split("-")
+                self.properties.append(XMLProperty(subnode, prop_type, default_ontology))
+
+    def get_props_with_links(self) -> list[XMLProperty]:
+        """
+        Get a list of all XMLProperties that have an outgoing link to another resource, be it a resptr-prop link
+        or a standoff link in a text.
+
+        Returns:
+            list of all XMLProperties
+        """
+        link_properties: list[XMLProperty] = []
+        for prop in self.properties:
+            if prop.valtype == "resptr":
+                link_properties.append(prop)
+            elif prop.valtype == "text":
+                for value in prop.values:
+                    if value.resrefs:
+                        link_properties.append(prop)
+                        break
+        return link_properties
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/graph_models.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/stash/graph_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/stash_models.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/stash/stash_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/upload_config.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/upload_config.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/xmlupload.py` & `dsp_tools-8.0.0/src/dsp_tools/commands/xmlupload/xmlupload.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from __future__ import annotations
 
 import pickle
 import sys
 import warnings
 from datetime import datetime
 from pathlib import Path
-from typing import Any
 
 from loguru import logger
 from lxml import etree
 
+from dsp_tools.cli.args import ServerCredentials
 from dsp_tools.commands.xmlupload.check_consistency_with_ontology import do_xml_consistency_check_with_ontology
-from dsp_tools.commands.xmlupload.iri_resolver import IriResolver
 from dsp_tools.commands.xmlupload.list_client import ListClient
 from dsp_tools.commands.xmlupload.list_client import ListClientLive
 from dsp_tools.commands.xmlupload.models.deserialise.xmlpermission import XmlPermission
-from dsp_tools.commands.xmlupload.models.deserialise.xmlresource import BitstreamInfo
 from dsp_tools.commands.xmlupload.models.deserialise.xmlresource import XMLResource
+from dsp_tools.commands.xmlupload.models.ingest import AssetClient
+from dsp_tools.commands.xmlupload.models.ingest import DspIngestClientLive
 from dsp_tools.commands.xmlupload.models.namespace_context import get_json_ld_context_for_project
 from dsp_tools.commands.xmlupload.models.permission import Permissions
-from dsp_tools.commands.xmlupload.models.sipi import Sipi
+from dsp_tools.commands.xmlupload.models.upload_clients import UploadClients
 from dsp_tools.commands.xmlupload.models.upload_state import UploadState
+from dsp_tools.commands.xmlupload.ontology_client import OntologyClient
 from dsp_tools.commands.xmlupload.ontology_client import OntologyClientLive
 from dsp_tools.commands.xmlupload.project_client import ProjectClient
 from dsp_tools.commands.xmlupload.project_client import ProjectClientLive
-from dsp_tools.commands.xmlupload.read_validate_xml_file import validate_and_parse_xml_file
+from dsp_tools.commands.xmlupload.read_validate_xml_file import check_if_bitstreams_exist
+from dsp_tools.commands.xmlupload.read_validate_xml_file import validate_and_parse
 from dsp_tools.commands.xmlupload.resource_create_client import ResourceCreateClient
-from dsp_tools.commands.xmlupload.resource_multimedia import handle_media_info
 from dsp_tools.commands.xmlupload.stash.stash_circular_references import identify_circular_references
 from dsp_tools.commands.xmlupload.stash.stash_circular_references import stash_circular_references
 from dsp_tools.commands.xmlupload.stash.stash_models import Stash
 from dsp_tools.commands.xmlupload.stash.upload_stashed_resptr_props import upload_stashed_resptr_props
 from dsp_tools.commands.xmlupload.stash.upload_stashed_xml_texts import upload_stashed_xml_texts
 from dsp_tools.commands.xmlupload.upload_config import UploadConfig
 from dsp_tools.commands.xmlupload.write_diagnostic_info import write_id2iri_mapping
@@ -42,89 +43,123 @@
 from dsp_tools.models.projectContext import ProjectContext
 from dsp_tools.utils.connection import Connection
 from dsp_tools.utils.connection_live import ConnectionLive
 from dsp_tools.utils.logger_config import logger_savepath
 
 
 def xmlupload(
-    input_file: str | Path | etree._ElementTree[Any],
-    server: str,
-    user: str,
-    password: str,
+    input_file: Path,
+    creds: ServerCredentials,
     imgdir: str,
-    sipi: str,
     config: UploadConfig = UploadConfig(),
 ) -> bool:
     """
     This function reads an XML file and imports the data described in it onto the DSP server.
 
     Args:
-        input_file: path to XML file containing the resources, or the XML tree itself
-        server: the DSP server where the data should be imported
-        user: the user (e-mail) with which the data should be imported
-        password: the password of the user with which the data should be imported
+        input_file: path to XML file containing the resources
+        creds: the credentials to access the DSP server
         imgdir: the image directory
-        sipi: the sipi instance to be used
-        config: the upload configuration
+        config: the configuration for the upload
 
     Raises:
         BaseError: in case of permanent network or software failure
         UserError: in case of permanent network or software failure, or if the XML file is invalid
         InputError: in case of permanent network or software failure, or if the XML file is invalid
 
     Returns:
         True if all resources could be uploaded without errors; False if one of the resources could not be
         uploaded because there is an error in it
     """
 
-    con = ConnectionLive(server)
-    con.login(user, password)
-    sipi_con = ConnectionLive(sipi, token=con.get_token())
-    sipi_server = Sipi(sipi_con)
+    default_ontology, root, shortcode = _pares_xml(input_file=input_file, imgdir=imgdir)
 
-    default_ontology, root, shortcode = validate_and_parse_xml_file(
-        input_file=input_file,
-        imgdir=imgdir,
-        preprocessing_done=config.media_previously_uploaded,
-    )
+    con = ConnectionLive(creds.server)
+    con.login(creds.user, creds.password)
+    config = config.with_server_info(server=creds.server, shortcode=shortcode)
 
-    config = config.with_server_info(
-        server=server,
-        shortcode=shortcode,
-    )
+    ontology_client = OntologyClientLive(con=con, shortcode=shortcode, default_ontology=default_ontology)
+    resources, permissions_lookup, stash = prepare_upload(root, ontology_client)
 
-    ontology_client = OntologyClientLive(
-        con=con,
-        shortcode=shortcode,
-        default_ontology=default_ontology,
-    )
-    do_xml_consistency_check_with_ontology(onto_client=ontology_client, root=root)
+    clients = _get_live_clients(con, creds, shortcode, imgdir)
+    state = UploadState(resources, stash, config, permissions_lookup)
 
-    resources, permissions_lookup, stash = _prepare_upload(
-        root=root,
-        con=con,
-        default_ontology=default_ontology,
-    )
+    return execute_upload(clients, state)
 
-    project_client: ProjectClient = ProjectClientLive(con, config.shortcode)
-    list_client: ListClient = ListClientLive(con, project_client.get_project_iri())
-    upload_state = UploadState(resources, [], IriResolver(), stash, config, permissions_lookup)
 
-    upload_resources(
-        upload_state=upload_state,
+def _pares_xml(imgdir: str, input_file: Path) -> tuple[str, etree._Element, str]:
+    """
+    This function takes a path to an XML file.
+    It validates the file against the XML schema.
+    It checks if all the mentioned bitstream files are in the specified location.
+    It retrieves the shortcode and default ontology from the XML file.
+
+    Args:
+        imgdir: directory to the bitstream files
+        input_file: file that will be pased
+
+    Returns:
+        The ontology name, the parsed XML file and the shortcode of the project
+    """
+    root, shortcode, default_ontology = validate_and_parse(input_file)
+    check_if_bitstreams_exist(root=root, imgdir=imgdir)
+    logger.info(f"Validated and parsed the XML file. {shortcode=:} and {default_ontology=:}")
+    return default_ontology, root, shortcode
+
+
+def _get_live_clients(
+    con: Connection,
+    creds: ServerCredentials,
+    shortcode: str,
+    imgdir: str,
+) -> UploadClients:
+    ingest_client: AssetClient
+    ingest_client = DspIngestClientLive(
+        dsp_ingest_url=creds.dsp_ingest_url,
+        token=con.get_token(),
+        shortcode=shortcode,
         imgdir=imgdir,
-        sipi_server=sipi_server,
+    )
+    project_client: ProjectClient = ProjectClientLive(con, shortcode)
+    list_client: ListClient = ListClientLive(con, project_client.get_project_iri())
+    return UploadClients(
+        asset_client=ingest_client,
         project_client=project_client,
         list_client=list_client,
     )
 
-    return cleanup_upload(upload_state)
 
+def execute_upload(clients: UploadClients, upload_state: UploadState) -> bool:
+    """Execute an upload from an upload state, and clean up afterwards.
+
+    Args:
+        clients: the clients needed for the upload
+        upload_state: the initial state of the upload to execute
 
-def cleanup_upload(upload_state: UploadState) -> bool:
+    Returns:
+        True if all resources could be uploaded without errors; False if any resource could not be uploaded
+    """
+    _upload_resources(clients, upload_state)
+    return _cleanup_upload(upload_state)
+
+
+def prepare_upload(
+    root: etree._Element,
+    ontology_client: OntologyClient,
+) -> tuple[list[XMLResource], dict[str, Permissions], Stash | None]:
+    """Do the consistency check, resolve circular references, and return the resources and permissions."""
+    do_xml_consistency_check_with_ontology(onto_client=ontology_client, root=root)
+    return _resolve_circular_references(
+        root=root,
+        con=ontology_client.con,
+        default_ontology=ontology_client.default_ontology,
+    )
+
+
+def _cleanup_upload(upload_state: UploadState) -> bool:
     """
     Write the id2iri mapping to a file and print a message to the console.
 
     Args:
         upload_state: the current state of the upload
 
     Returns:
@@ -151,15 +186,15 @@
         msg = _save_upload_state(upload_state)
         print(msg)
 
     upload_state.config.diagnostics.save_location.unlink(missing_ok=True)
     return success
 
 
-def _prepare_upload(
+def _resolve_circular_references(
     root: etree._Element,
     con: Connection,
     default_ontology: str,
 ) -> tuple[list[XMLResource], dict[str, Permissions], Stash | None]:
     logger.info("Checking resources for circular references...")
     print(f"{datetime.now()}: Checking resources for circular references...")
     stash_lookup, upload_order = identify_circular_references(root)
@@ -173,41 +208,53 @@
     resources = [sorting_lookup[res_id] for res_id in upload_order]
     logger.info("Stashing circular references...")
     print(f"{datetime.now()}: Stashing circular references...")
     stash = stash_circular_references(resources, stash_lookup, permissions_lookup)
     return resources, permissions_lookup, stash
 
 
-def upload_resources(
-    upload_state: UploadState,
-    imgdir: str,
-    sipi_server: Sipi,
-    project_client: ProjectClient,
-    list_client: ListClient,
-) -> None:
+def _upload_resources(clients: UploadClients, upload_state: UploadState) -> None:
     """
-    Actual upload of all resources to DSP.
+    Iterates through all resources and tries to upload them to DSP.
+    If a temporary exception occurs, the action is repeated until success,
+    and if a permanent exception occurs, the resource is skipped.
 
     Args:
+        clients: the clients needed for the upload
         upload_state: the current state of the upload
-        imgdir: folder containing the multimedia files
-        sipi_server: Sipi instance
-        project_client: a client for HTTP communication with the DSP-API
-        list_client: a client for HTTP communication with the DSP-API
+
+    Raises:
+        BaseException: in case of an unhandled exception during resource creation
+        XmlUploadInterruptedError: if the number of resources created is equal to the interrupt_after value
     """
+    project_iri = clients.project_client.get_project_iri()
+    project_onto_dict = clients.project_client.get_ontology_name_dict()
+    listnode_lookup = clients.list_client.get_list_node_id_to_iri_lookup()
+
+    resource_create_client = ResourceCreateClient(
+        con=clients.project_client.con,
+        project_iri=project_iri,
+        iri_resolver=upload_state.iri_resolver,
+        project_onto_dict=project_onto_dict,
+        permissions_lookup=upload_state.permissions_lookup,
+        listnode_lookup=listnode_lookup,
+        media_previously_ingested=upload_state.config.media_previously_uploaded,
+    )
+
     try:
-        _upload_resources(
-            upload_state=upload_state,
-            imgdir=imgdir,
-            sipi_server=sipi_server,
-            project_client=project_client,
-            list_client=list_client,
-        )
+        for creation_attempts_of_this_round, resource in enumerate(upload_state.pending_resources.copy()):
+            _upload_one_resource(
+                upload_state=upload_state,
+                resource=resource,
+                ingest_client=clients.asset_client,
+                resource_create_client=resource_create_client,
+                creation_attempts_of_this_round=creation_attempts_of_this_round,
+            )
         if upload_state.pending_stash:
-            _upload_stash(upload_state, project_client)
+            _upload_stash(upload_state, clients.project_client)
     except XmlUploadInterruptedError as err:
         _handle_upload_error(err, upload_state)
 
 
 def _get_data_from_xml(
     con: Connection,
     root: etree._Element,
@@ -259,98 +306,53 @@
 
 
 def _extract_resources_from_xml(root: etree._Element, default_ontology: str) -> list[XMLResource]:
     resources = list(root.iter(tag="resource"))
     return [XMLResource(res, default_ontology) for res in resources]
 
 
-def _upload_resources(
-    upload_state: UploadState,
-    imgdir: str,
-    sipi_server: Sipi,
-    project_client: ProjectClient,
-    list_client: ListClient,
-) -> None:
-    """
-    Iterates through all resources and tries to upload them to DSP.
-    If a temporary exception occurs, the action is repeated until success,
-    and if a permanent exception occurs, the resource is skipped.
-
-    Args:
-        upload_state: the current state of the upload
-        imgdir: folder containing the multimedia files
-        sipi_server: Sipi instance
-        project_client: a client for HTTP communication with the DSP-API
-        list_client: a client for HTTP communication with the DSP-API
-
-    Raises:
-        BaseException: in case of an unhandled exception during resource creation
-        XmlUploadInterruptedError: if the number of resources created is equal to the interrupt_after value
-    """
-    project_iri = project_client.get_project_iri()
-    project_onto_dict = project_client.get_ontology_name_dict()
-    listnode_lookup = list_client.get_list_node_id_to_iri_lookup()
-
-    resource_create_client = ResourceCreateClient(
-        con=project_client.con,
-        project_iri=project_iri,
-        iri_resolver=upload_state.iri_resolver,
-        project_onto_dict=project_onto_dict,
-        permissions_lookup=upload_state.permissions_lookup,
-        listnode_lookup=listnode_lookup,
-        media_previously_ingested=upload_state.config.media_previously_uploaded,
-    )
-
-    for creation_attempts_of_this_round, resource in enumerate(upload_state.pending_resources.copy()):
-        _upload_one_resource(
-            upload_state=upload_state,
-            resource=resource,
-            imgdir=imgdir,
-            sipi_server=sipi_server,
-            resource_create_client=resource_create_client,
-            creation_attempts_of_this_round=creation_attempts_of_this_round,
-        )
-
-
 def _upload_one_resource(
     upload_state: UploadState,
     resource: XMLResource,
-    imgdir: str,
-    sipi_server: Sipi,
+    ingest_client: AssetClient,
     resource_create_client: ResourceCreateClient,
     creation_attempts_of_this_round: int,
 ) -> None:
     try:
-        success, media_info = handle_media_info(
-            resource,
-            upload_state.config.media_previously_uploaded,
-            sipi_server,
-            imgdir,
-            upload_state.permissions_lookup,
-        )
+        if resource.bitstream:
+            success, media_info = ingest_client.get_bitstream_info(
+                resource.bitstream, upload_state.permissions_lookup, resource.label, resource.res_id
+            )
+        else:
+            success, media_info = True, None
+
         if not success:
             upload_state.failed_uploads.append(resource.res_id)
             return
     except KeyboardInterrupt:
         raise XmlUploadInterruptedError("KeyboardInterrupt during media file upload") from None
 
+    iri = None
     try:
-        iri = _create_resource(resource, media_info, resource_create_client)
+        iri = resource_create_client.create_resource(resource, media_info)
     except (PermanentTimeOutError, KeyboardInterrupt) as err:
         warnings.warn(DspToolsUserWarning(f"{type(err).__name__}: Tidying up, then exit..."))
         msg = (
             f"There was a {type(err).__name__} while trying to create resource '{resource.res_id}'.\n"
             f"It is unclear if the resource '{resource.res_id}' was created successfully or not.\n"
             f"Please check manually in the DSP-APP or DB.\n"
             f"In case of successful creation, call 'resume-xmlupload' with the flag "
             f"'--skip-first-resource' to prevent duplication.\n"
             f"If not, a normal 'resume-xmlupload' can be started."
         )
         logger.error(msg)
         raise XmlUploadInterruptedError(msg) from None
+    except Exception as err:  # noqa: BLE001 (blind-except)
+        err_msg = err.message if isinstance(err, BaseError) else None
+        _handle_resource_creation_failure(resource, err_msg)
 
     try:
         _tidy_up_resource_creation_idempotent(upload_state, iri, resource)
         _interrupt_if_indicated(upload_state, creation_attempts_of_this_round)
     except KeyboardInterrupt:
         warnings.warn(DspToolsUserWarning("KeyboardInterrupt: Tidying up, then exit..."))
         _tidy_up_resource_creation_idempotent(upload_state, iri, resource)
@@ -386,38 +388,25 @@
         if resource.res_id not in upload_state.failed_uploads:
             upload_state.failed_uploads.append(resource.res_id)
 
     if resource in upload_state.pending_resources:
         upload_state.pending_resources.remove(resource)
 
 
-def _create_resource(
-    resource: XMLResource,
-    bitstream_information: BitstreamInfo | None,
-    resource_create_client: ResourceCreateClient,
-) -> str | None:
-    try:
-        return resource_create_client.create_resource(resource, bitstream_information)
-    except PermanentTimeOutError as err:
-        # The following block catches all exceptions and handles them in a generic way.
-        # Because the calling function needs to know that this was a PermanentTimeOutError, we need to catch and
-        # raise it here.
-        raise err
-    except Exception as err:  # noqa: BLE001 (blind-except)
-        msg = f"{datetime.now()}: WARNING: Unable to create resource '{resource.label}' (ID: '{resource.res_id}')"
-        if isinstance(err, BaseError):
-            msg = f"{msg}: {err.message}"
-        print(msg)
-        log_msg = (
-            f"Unable to create resource '{resource.label}' ({resource.res_id})\n"
-            f"Resource details:\n{vars(resource)}\n"
-            f"Property details:\n" + "\n".join([str(vars(prop)) for prop in resource.properties])
-        )
-        logger.exception(log_msg)
-        return None
+def _handle_resource_creation_failure(resource: XMLResource, err_msg: str | None) -> None:
+    msg = f"{datetime.now()}: WARNING: Unable to create resource '{resource.label}' (ID: '{resource.res_id}')"
+    if err_msg:
+        msg = f"{msg}: {err_msg}"
+    print(msg)
+    log_msg = (
+        f"Unable to create resource '{resource.label}' ({resource.res_id})\n"
+        f"Resource details:\n{vars(resource)}\n"
+        f"Property details:\n" + "\n".join([str(vars(prop)) for prop in resource.properties])
+    )
+    logger.exception(log_msg)
 
 
 def _handle_upload_error(err: BaseException, upload_state: UploadState) -> None:
     """
     In case the xmlupload must be interrupted,
     e.g. because of an error that could not be handled,
     or due to keyboard interrupt,
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/models/custom_warnings.py` & `dsp_tools-8.0.0/src/dsp_tools/models/custom_warnings.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/models/datetimestamp.py` & `dsp_tools-8.0.0/src/dsp_tools/models/datetimestamp.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/models/exceptions.py` & `dsp_tools-8.0.0/src/dsp_tools/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/models/langstring.py` & `dsp_tools-8.0.0/src/dsp_tools/models/langstring.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/models/projectContext.py` & `dsp_tools-8.0.0/src/dsp_tools/models/projectContext.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/resources/0100-template-repo/template.json` & `dsp_tools-8.0.0/src/dsp_tools/resources/0100-template-repo/template.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/resources/0100-template-repo/template.xml` & `dsp_tools-8.0.0/src/dsp_tools/resources/0100-template-repo/template.xml`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/data.xsd` & `dsp_tools-8.0.0/src/dsp_tools/resources/schema/data.xsd`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/lists-only.json` & `dsp_tools-8.0.0/src/dsp_tools/resources/schema/lists-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/project.json` & `dsp_tools-8.0.0/src/dsp_tools/resources/schema/project.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/properties-only.json` & `dsp_tools-8.0.0/src/dsp_tools/resources/schema/properties-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/resources-only.json` & `dsp_tools-8.0.0/src/dsp_tools/resources/schema/resources-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/resources/start-stack/docker-compose.yml` & `dsp_tools-8.0.0/src/dsp_tools/resources/start-stack/docker-compose.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 ---
-
 services:
-
   api:
     # on the verge of every deployment (fortnightly), update the "image" value from the "api" value of
     # https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json
-    image: daschswiss/knora-api:v30.13.0
+    image: daschswiss/knora-api:v30.14.0
     depends_on:
       - sipi
       - db
     ports:
       - "3333:3333"
     networks:
       - knora-net
     environment:
       - TZ=Europe/Zurich
       - KNORA_AKKA_LOGLEVEL=DEBUG
       - KNORA_AKKA_STDOUT_LOGLEVEL=DEBUG
+      - KNORA_WEBAPI_DSP_INGEST_BASE_URL=http://ingest:3340
       - KNORA_WEBAPI_TRIPLESTORE_HOST=db
       - KNORA_WEBAPI_TRIPLESTORE_DBTYPE=fuseki
       - KNORA_WEBAPI_SIPI_INTERNAL_HOST=sipi
       - KNORA_WEBAPI_TRIPLESTORE_FUSEKI_REPOSITORY_NAME=knora-test
       - KNORA_WEBAPI_TRIPLESTORE_FUSEKI_USERNAME=admin
       - KNORA_WEBAPI_TRIPLESTORE_FUSEKI_PASSWORD=test
       - KNORA_WEBAPI_CACHE_SERVICE_ENABLED=true
@@ -29,15 +28,15 @@
       - KNORA_WEBAPI_ALLOW_RELOAD_OVER_HTTP=true
       - KNORA_WEBAPI_KNORA_API_EXTERNAL_HOST=0.0.0.0
       - KNORA_WEBAPI_KNORA_API_EXTERNAL_PORT=3333
       - DSP_API_LOG_LEVEL=INFO
 
   sipi:
     # on the verge of every deployment (fortnightly), take the same tag as DSP-API
-    image: daschswiss/knora-sipi:v30.13.0
+    image: daschswiss/knora-sipi:v30.14.0
     ports:
       - "1024:1024"
     volumes:
       - ./tmp:/tmp
       - .:/sipi/config
       - ./sipi/images:/sipi/images
     networks:
@@ -61,28 +60,28 @@
       - "4200:4200"
     networks:
       - knora-net
 
   db:
     # on the verge of every deployment (fortnightly), update the "image" value from the "db" value of
     # https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json
-    image: daschswiss/apache-jena-fuseki:5.0.0-1
+    image: daschswiss/apache-jena-fuseki:5.0.0-2
     ports:
       - "3030:3030"
     networks:
       - knora-net
     environment:
       - TZ=Europe/Zurich
       - ADMIN_PASSWORD=test
       - JVM_ARGS=-Xmx3G
 
   ingest:
     # on the verge of every deployment (fortnightly), update the "image" value from the "ingest" value of
     # https://github.com/dasch-swiss/ops-deploy/blob/main/roles/dsp-deploy/files/RELEASE.json
-    image: daschswiss/dsp-ingest:v0.9.0
+    image: daschswiss/dsp-ingest:v0.9.1
     ports:
       - "3340:3340"
     volumes:
       - ./sipi/images:/opt/images
       - ./sipi/tmp-dsp-ingest:/opt/temp
     networks:
       - knora-net
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/utils/connection.py` & `dsp_tools-8.0.0/src/dsp_tools/utils/connection.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/utils/connection_live.py` & `dsp_tools-8.0.0/src/dsp_tools/utils/connection_live.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from dataclasses import dataclass
 from dataclasses import field
 from datetime import datetime
 from functools import partial
 from importlib.metadata import version
 from typing import Any
 from typing import Literal
+from typing import Never
 from typing import Optional
 from typing import cast
 
 import regex
 from loguru import logger
 from requests import ReadTimeout
 from requests import RequestException
@@ -19,14 +20,15 @@
 from requests import Session
 
 from dsp_tools.models.exceptions import BadCredentialsError
 from dsp_tools.models.exceptions import BaseError
 from dsp_tools.models.exceptions import PermanentConnectionError
 from dsp_tools.models.exceptions import PermanentTimeOutError
 from dsp_tools.models.exceptions import UserError
+from dsp_tools.utils.connection import Connection
 from dsp_tools.utils.logger_config import logger_savepath
 from dsp_tools.utils.set_encoder import SetEncoder
 
 HTTP_OK = 200
 HTTP_UNAUTHORIZED = 401
 
 
@@ -56,15 +58,15 @@
             "data": self.data_serialized,
             "headers": self.headers,
             "files": self.files,
         }
 
 
 @dataclass
-class ConnectionLive:
+class ConnectionLive(Connection):
     """
     A Connection instance represents a connection to a DSP server.
 
     Attributes:
         server: address of the server, e.g https://api.dasch.swiss
         token: session token received by the server after login
     """
@@ -310,15 +312,15 @@
         print(f"{datetime.now()}: {msg}")
         if exc_info:
             logger.opt(exception=True).error(f"{msg} ({retry_counter=:})")
         else:
             logger.error(f"{msg} ({retry_counter=:})")
         time.sleep(2**retry_counter)
 
-    def _log_and_raise_timeouts(self, error: TimeoutError | ReadTimeout) -> None:
+    def _log_and_raise_timeouts(self, error: TimeoutError | ReadTimeout) -> Never:
         msg = f"A '{error.__class__.__name__}' occurred during the connection to the DSP server."
         print(f"{datetime.now()}: {msg}")
         logger.exception(msg)
         raise PermanentTimeOutError(msg) from None
 
     def _log_response(self, response: Response) -> None:
         dumpobj: dict[str, Any] = {
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/utils/date_util.py` & `dsp_tools-8.0.0/src/dsp_tools/utils/date_util.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/utils/logger_config.py` & `dsp_tools-8.0.0/src/dsp_tools/utils/logger_config.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/utils/set_encoder.py` & `dsp_tools-8.0.0/src/dsp_tools/utils/set_encoder.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/utils/shared.py` & `dsp_tools-8.0.0/src/dsp_tools/utils/shared.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/utils/uri_util.py` & `dsp_tools-8.0.0/src/dsp_tools/utils/uri_util.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/utils/warnings_config.py` & `dsp_tools-8.0.0/src/dsp_tools/utils/warnings_config.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/utils/xml_utils.py` & `dsp_tools-8.0.0/src/dsp_tools/utils/xml_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,42 @@
 from __future__ import annotations
 
 import copy
 from pathlib import Path
-from typing import Any
-from typing import Union
 
 from loguru import logger
 from lxml import etree
 
 from dsp_tools.models.exceptions import InputError
 
 
-def parse_and_clean_xml_file(input_file: Union[str, Path, etree._ElementTree[Any]]) -> etree._Element:
+def parse_and_clean_xml_file(input_file: Path) -> etree._Element:
     """
     Parse an XML file with DSP-conform data,
     remove namespace URI from the elements' names,
     and transform the special tags <annotation>, <region>, <link>, <video-segment>, <audio-segment>
     to their technically correct form
     <resource restype="Annotation">, <resource restype="Region">, <resource restype="LinkObj">,
     <resource restype="VideoSegment">, <resource restype="AudioSegment">.
 
     Args:
-        input_file: path to the XML file, or parsed ElementTree
+        input_file: path to the XML file
 
     Returns:
         the root element of the parsed XML file
 
     Raises:
         InputError: if the input is not of either the expected types
     """
+    root = parse_xml_file(input_file)
+    root = remove_comments_from_element_tree(root)
+    return remove_qnames_and_transform_special_tags(root)
 
-    tree = parse_and_remove_comments_from_xml_file(input_file)
-    return _remove_qnames_and_transform_special_tags(tree)
 
-
-def parse_and_remove_comments_from_xml_file(
-    input_file: Union[str, Path, etree._ElementTree[Any]],
-) -> etree._Element:
-    """
-    Parse an XML file with DSP-conform data,
-    and remove the comments and processing instructions
-    (commented out properties break the XMLProperty constructor)
-
-    Args:
-        input_file: path to the XML file, or parsed ElementTree
-
-    Returns:
-        the root element of the parsed XML file
-
-    Raises:
-        InputError: if the input is not of either the expected types
-    """
-
-    if isinstance(input_file, (str, Path)):
-        tree = _parse_xml_file(input_file)
-    else:
-        tree = input_file
-    tree = remove_comments_from_element_tree(tree)
-
-    return tree.getroot()
-
-
-def _remove_qnames_and_transform_special_tags(
-    input_tree: etree._Element,
-) -> etree._Element:
+def remove_qnames_and_transform_special_tags(input_tree: etree._Element) -> etree._Element:
     """
     This function removes the namespace URIs from the elements' names
     and transforms the special tags <annotation>, <region>, <link>, <video-segment>, <audio-segment>
     to their technically correct form
     <resource restype="Annotation">, <resource restype="Region">, <resource restype="LinkObj">,
     <resource restype="VideoSegment">, <resource restype="AudioSegment">.
 
@@ -93,66 +62,62 @@
             elem.tag = "resource"
         elif elem.tag == "audio-segment":
             elem.attrib["restype"] = "AudioSegment"
             elem.tag = "resource"
     return input_tree
 
 
-def remove_comments_from_element_tree(
-    input_tree: etree._ElementTree[etree._Element],
-) -> etree._ElementTree[etree._Element]:
+def remove_comments_from_element_tree(input_tree: etree._Element) -> etree._Element:
     """
     This function removes comments and processing instructions.
     Commented out properties break the XMLProperty constructor.
 
     Args:
-        input_tree: etree that will be cleaned
+        input_tree: etree root that will be cleaned
 
     Returns:
-        clean etree
+        clean xml
     """
-    tree = copy.deepcopy(input_tree)
-    for c in tree.xpath("//comment()"):
+    root = copy.deepcopy(input_tree)
+    for c in root.xpath("//comment()"):
         c.getparent().remove(c)
-    for c in tree.xpath("//processing-instruction()"):
+    for c in root.xpath("//processing-instruction()"):
         c.getparent().remove(c)
-    return tree
+    return root
 
 
-def _parse_xml_file(input_file: Union[str, Path]) -> etree._ElementTree[etree._Element]:
+def parse_xml_file(input_file: str | Path) -> etree._Element:
     """
     This function parses an XML file and returns an Element Tree
 
     Args:
         input_file: path to the input file
 
     Returns:
         element tree
 
     Raises:
         InputError: if the file contains a syntax error
     """
     parser = etree.XMLParser(remove_comments=True, remove_pis=True)
     try:
-        return etree.parse(source=input_file, parser=parser)
+        return etree.parse(source=input_file, parser=parser).getroot()
     except etree.XMLSyntaxError as err:
         logger.opt(exception=True).error(f"The XML file contains the following syntax error: {err.msg}")
         raise InputError(f"The XML file contains the following syntax error: {err.msg}") from None
 
 
-def remove_namespaces_from_xml(
-    data_xml: etree._Element,
-) -> etree._Element:
+def remove_namespaces_from_xml(data_xml: etree._Element) -> etree._Element:
     """
-    This function removes all the namespaces from an XML file.
+    This function removes all the namespaces from an XML element tree.
 
     Args:
-        data_xml: file with namespaces
+        data_xml: xml with namespaces
 
     Returns:
-        the XMl file without the namespaces
+        the XMl without the namespaces
     """
     xml_no_namespace = copy.deepcopy(data_xml)
     for elem in xml_no_namespace.iter():
         if not isinstance(elem, (etree._Comment, etree._ProcessingInstruction)):
             elem.tag = etree.QName(elem).localname
     return xml_no_namespace
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/utils/xml_validation.py` & `dsp_tools-8.0.0/src/dsp_tools/utils/xml_validation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,100 +1,101 @@
 from __future__ import annotations
 
 import importlib.resources
 from datetime import datetime
 from pathlib import Path
-from typing import Any
-from typing import Union
 
 import regex
 from loguru import logger
 from lxml import etree
 
 from dsp_tools.models.exceptions import InputError
-from dsp_tools.utils.xml_utils import parse_and_remove_comments_from_xml_file
+from dsp_tools.utils.xml_utils import parse_xml_file
+from dsp_tools.utils.xml_utils import remove_comments_from_element_tree
 from dsp_tools.utils.xml_utils import remove_namespaces_from_xml
 from dsp_tools.utils.xml_validation_models import InconsistentTextValueEncodings
 from dsp_tools.utils.xml_validation_models import TextValueData
 
 separator = "\n    "
 list_separator = "\n    - "
 medium_separator = "\n----------------------------\n"
 grand_separator = "\n\n---------------------------------------\n\n"
 
 
-def validate_xml(input_file: Union[str, Path, etree._ElementTree[Any]]) -> bool:
+def validate_xml_file(input_file: Path | str) -> bool:
     """
     Validates an XML file against the DSP XSD schema.
 
     Args:
         input_file: path to the XML file to be validated, or parsed ElementTree
 
     Raises:
         InputError: if the XML file is invalid
 
     Returns:
         True if the XML file is valid
     """
-    data_xml, xmlschema = _parse_schema_and_data_files(input_file)
+    root = parse_xml_file(input_file)
+    data_xml = remove_comments_from_element_tree(root)
+    return validate_xml(data_xml)
 
-    problems = []
 
-    all_good, msg = _validate_xml_against_schema(xmlschema, data_xml)
-    if not all_good:
-        problems.append(msg)
-
-    xml_no_namespace = remove_namespaces_from_xml(data_xml)
-
-    all_good, msg = _find_xml_tags_in_simple_text_elements(xml_no_namespace)
-    if not all_good:
-        problems.append(msg)
-
-    all_good, msg = _find_mixed_encodings_in_one_text_prop(xml_no_namespace)
-    if not all_good:
-        problems.append(msg)
+def validate_xml(xml: etree._Element) -> bool:
+    """
+    Validates an XML element tree against the DSP XSD schema.
 
-    _check_for_deprecated_syntax(xml_no_namespace)
+    Args:
+        xml: the XML element tree to be validated
+
+    Raises:
+        InputError: if the XML file is invalid
+
+    Returns:
+        True if the XML file is valid
+    """
+    xml_no_namespace = remove_namespaces_from_xml(xml)
+
+    problems = []
+
+    problems.extend(_validate_xml_against_schema(xml))
+    problems.extend(_validate_xml_contents(xml_no_namespace))
 
     if len(problems) > 0:
         err_msg = grand_separator.join(problems)
         logger.opt(exception=True).error(err_msg)
         raise InputError(err_msg)
 
     logger.info("The XML file is syntactically correct and passed validation.")
     print(f"{datetime.now()}: The XML file is syntactically correct and passed validation.")
+
     return True
 
 
-def _parse_schema_and_data_files(
-    input_file: Union[str, Path, etree._ElementTree[Any]],
-) -> tuple[etree._Element, etree.XMLSchema]:
-    with (
-        importlib.resources.files("dsp_tools")
-        .joinpath("resources/schema/data.xsd")
-        .open(encoding="utf-8") as schema_file
-    ):
+def _validate_xml_against_schema(data_xml: etree._Element) -> list[str]:
+    schema_res = importlib.resources.files("dsp_tools").joinpath("resources/schema/data.xsd")
+    with schema_res.open(encoding="utf-8") as schema_file:
         xmlschema = etree.XMLSchema(etree.parse(schema_file))
-    data_xml = parse_and_remove_comments_from_xml_file(input_file)
-    return data_xml, xmlschema
-
-
-def _validate_xml_against_schema(xmlschema: etree.XMLSchema, data_xml: etree._Element) -> tuple[bool, str]:
     if not xmlschema.validate(data_xml):
         error_msg = "The XML file cannot be uploaded due to the following validation error(s):"
         for error in xmlschema.error_log:
             error_msg = error_msg + f"{separator}Line {error.line}: {error.message}"
         error_msg = error_msg.replace("{https://dasch.swiss/schema}", "")
-        return False, error_msg
-    return True, ""
+        return [error_msg]
+    return []
+
+
+def _validate_xml_contents(xml_no_namespace: etree._Element) -> list[str]:
+    problems = []
+    problems.extend(_find_xml_tags_in_simple_text_elements(xml_no_namespace))
+    problems.extend(_find_mixed_encodings_in_one_text_prop(xml_no_namespace))
+    _check_for_deprecated_syntax(xml_no_namespace)
+    return problems
 
 
-def _find_xml_tags_in_simple_text_elements(
-    xml_no_namespace: etree._Element,
-) -> tuple[bool, str]:
+def _find_xml_tags_in_simple_text_elements(xml_no_namespace: etree._Element) -> list[str]:
     """
     Makes sure that there are no XML tags in simple texts.
     This can only be done with a regex,
     because even if the simple text contains some XML tags,
     the simple text itself is not valid XML that could be parsed.
     The extra challenge is that lxml transforms
     "pebble (&lt;2cm) and boulder (&gt;20cm)" into
@@ -121,30 +122,28 @@
             resources_with_illegal_xml_tags.append(f"{sourceline}resource '{resname}', property '{propname}'")
     if resources_with_illegal_xml_tags:
         err_msg = (
             "XML-tags are not allowed in text properties with encoding=utf8.\n"
             "The following resources of your XML file violate this rule:"
         )
         err_msg += list_separator + list_separator.join(resources_with_illegal_xml_tags)
-        return False, err_msg
-    return True, ""
+        return [err_msg]
+    return []
 
 
-def _find_mixed_encodings_in_one_text_prop(
-    xml_no_namespace: etree._Element,
-) -> tuple[bool, str]:
+def _find_mixed_encodings_in_one_text_prop(xml_no_namespace: etree._Element) -> list[str]:
     problems = check_if_only_one_encoding_is_used_per_prop_in_root(xml_no_namespace)
     if not problems:
-        return True, ""
+        return []
     msg, df = InconsistentTextValueEncodings(problems).execute_problem_protocol()
     if df is not None:
         csv_path = Path(f"XML_syntax_errors_{datetime.now().strftime('%Y-%m-%d_%H%M%S')}.csv")
         msg = f"\nAll the problems are listed in the file: '{csv_path.absolute()}'" + msg
         df.to_csv(csv_path)
-    return False, msg
+    return [msg]
 
 
 def _check_for_deprecated_syntax(data_xml: etree._Element) -> None:  # noqa: ARG001 (unused argument)
     pass
 
 
 def check_if_only_one_encoding_is_used_per_prop_in_root(
```

### Comparing `dsp_tools-7.2.0.post7/src/dsp_tools/utils/xml_validation_models.py` & `dsp_tools-8.0.0/src/dsp_tools/utils/xml_validation_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post7/PKG-INFO` & `dsp_tools-8.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsp-tools
-Version: 7.2.0.post7
+Version: 8.0.0
 Summary: DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server.
 Home-page: https://www.dasch.swiss/
 License: GPL-3.0-only
 Author: DaSCH - Swiss National Data and Service Center for the Humanities
 Author-email: info@dasch.swiss
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

