# Comparing `tmp/airbyte_source_clockify-0.3.3.tar.gz` & `tmp/airbyte_source_clockify-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_clockify-0.3.3.tar", max compression
+gzip compressed data, was "airbyte_source_clockify-0.3.4.tar", max compression
```

## Comparing `airbyte_source_clockify-0.3.3.tar` & `airbyte_source_clockify-0.3.4.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     4532 2024-05-01 18:33:42.797930 airbyte_source_clockify-0.3.3/README.md
--rw-r--r--   0        0        0      755 2024-05-01 18:37:32.174572 airbyte_source_clockify-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      128 2024-05-01 18:33:42.797930 airbyte_source_clockify-0.3.3/source_clockify/__init__.py
--rw-r--r--   0        0        0    26215 2024-05-01 18:33:42.797930 airbyte_source_clockify-0.3.3/source_clockify/manifest.yaml
--rw-r--r--   0        0        0      236 2024-05-01 18:33:42.797930 airbyte_source_clockify-0.3.3/source_clockify/run.py
--rw-r--r--   0        0        0      477 2024-05-01 18:33:42.797930 airbyte_source_clockify-0.3.3/source_clockify/source.py
--rw-r--r--   0        0        0      848 2024-05-01 18:33:42.797930 airbyte_source_clockify-0.3.3/source_clockify/spec.yaml
--rw-r--r--   0        0        0     5242 1970-01-01 00:00:00.000000 airbyte_source_clockify-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     4542 2024-05-21 23:44:21.259656 airbyte_source_clockify-0.3.4/README.md
+-rw-r--r--   0        0        0      755 2024-05-21 23:48:50.450609 airbyte_source_clockify-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      128 2024-05-21 23:44:21.259656 airbyte_source_clockify-0.3.4/source_clockify/__init__.py
+-rw-r--r--   0        0        0    28813 2024-05-21 23:44:21.259656 airbyte_source_clockify-0.3.4/source_clockify/manifest.yaml
+-rw-r--r--   0        0        0      236 2024-05-21 23:44:21.259656 airbyte_source_clockify-0.3.4/source_clockify/run.py
+-rw-r--r--   0        0        0      477 2024-05-21 23:44:21.259656 airbyte_source_clockify-0.3.4/source_clockify/source.py
+-rw-r--r--   0        0        0     5252 1970-01-01 00:00:00.000000 airbyte_source_clockify-0.3.4/PKG-INFO
```

### Comparing `airbyte_source_clockify-0.3.3/README.md` & `airbyte_source_clockify-0.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Clockify source connector
 
-
 This is the repository for the Clockify source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/clockify).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
-
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/clockify)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_clockify/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-clockify spec
 poetry run source-clockify check --config secrets/config.json
 poetry run source-clockify discover --config secrets/config.json
 poetry run source-clockify read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
+
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
+
 ```bash
 airbyte-ci connectors --name=source-clockify build
 ```
 
 An image will be available on your host with the tag `airbyte/source-clockify:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-clockify:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-clockify:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-clockify:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-clockify:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-clockify test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
-All of your dependencies should be managed via Poetry. 
+
+All of your dependencies should be managed via Poetry.
 To add a new dependency, run:
+
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-clockify test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/clockify.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_clockify-0.3.3/pyproject.toml` & `airbyte_source_clockify-0.3.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.3.3"
+version = "0.3.4"
 name = "airbyte-source-clockify"
 description = "Source implementation for Clockify."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_clockify-0.3.3/source_clockify/manifest.yaml` & `airbyte_source_clockify-0.3.4/source_clockify/manifest.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,868 +1,1043 @@
-version: "0.29.0"
+version: 0.78.5
 
-definitions:
-  selector:
-    type: RecordSelector
-    extractor:
-      type: DpathExtractor
-      field_path: []
+type: DeclarativeSource
+
+check:
+  type: CheckStream
+  stream_names:
+    - users
 
-  requester:
+definitions:
+  streams:
+    users:
+      type: DeclarativeStream
+      name: users
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: workspaces/{{ config['workspace_id'] }}/users
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+        paginator:
+          type: DefaultPaginator
+          page_token_option:
+            type: RequestOption
+            inject_into: request_parameter
+            field_name: page
+          page_size_option:
+            type: RequestOption
+            inject_into: request_parameter
+            field_name: page-size
+          pagination_strategy:
+            type: PageIncrement
+            page_size: 50
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/users"
+    projects:
+      type: DeclarativeStream
+      name: projects
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: workspaces/{{ config['workspace_id'] }}/projects
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+        paginator:
+          type: DefaultPaginator
+          page_token_option:
+            type: RequestOption
+            inject_into: request_parameter
+            field_name: page
+          page_size_option:
+            type: RequestOption
+            inject_into: request_parameter
+            field_name: page-size
+          pagination_strategy:
+            type: PageIncrement
+            page_size: 50
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/projects"
+    clients:
+      type: DeclarativeStream
+      name: clients
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: workspaces/{{ config['workspace_id'] }}/clients
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+        paginator:
+          type: DefaultPaginator
+          page_token_option:
+            type: RequestOption
+            inject_into: request_parameter
+            field_name: page
+          page_size_option:
+            type: RequestOption
+            inject_into: request_parameter
+            field_name: page-size
+          pagination_strategy:
+            type: PageIncrement
+            page_size: 50
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/clients"
+    tags:
+      type: DeclarativeStream
+      name: tags
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: workspaces/{{ config['workspace_id'] }}/tags
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+        paginator:
+          type: DefaultPaginator
+          page_token_option:
+            type: RequestOption
+            inject_into: request_parameter
+            field_name: page
+          page_size_option:
+            type: RequestOption
+            inject_into: request_parameter
+            field_name: page-size
+          pagination_strategy:
+            type: PageIncrement
+            page_size: 50
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/tags"
+    user_groups:
+      type: DeclarativeStream
+      name: user_groups
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: workspaces/{{ config['workspace_id'] }}/user-groups
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+        paginator:
+          type: DefaultPaginator
+          page_token_option:
+            type: RequestOption
+            inject_into: request_parameter
+            field_name: page
+          page_size_option:
+            type: RequestOption
+            inject_into: request_parameter
+            field_name: page-size
+          pagination_strategy:
+            type: PageIncrement
+            page_size: 50
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/user_groups"
+    time_entries:
+      type: DeclarativeStream
+      name: time_entries
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: >-
+            workspaces/{{ config['workspace_id'] }}/user/{{
+            stream_partition.user_id}}/time-entries
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+        paginator:
+          type: DefaultPaginator
+          page_token_option:
+            type: RequestOption
+            inject_into: request_parameter
+            field_name: page
+          page_size_option:
+            type: RequestOption
+            inject_into: request_parameter
+            field_name: page-size
+          pagination_strategy:
+            type: PageIncrement
+            page_size: 50
+        partition_router:
+          - type: SubstreamPartitionRouter
+            parent_stream_configs:
+              - type: ParentStreamConfig
+                parent_key: id
+                partition_field: user_id
+                stream:
+                  $ref: "#/definitions/streams/users"
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/time_entries"
+    tasks:
+      type: DeclarativeStream
+      name: tasks
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: >-
+            workspaces/{{ config['workspace_id'] }}/projects/{{
+            stream_partition.project_id}}/tasks
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+        paginator:
+          type: DefaultPaginator
+          page_token_option:
+            type: RequestOption
+            inject_into: request_parameter
+            field_name: page
+          page_size_option:
+            type: RequestOption
+            inject_into: request_parameter
+            field_name: page-size
+          pagination_strategy:
+            type: PageIncrement
+            page_size: 50
+        partition_router:
+          - type: SubstreamPartitionRouter
+            parent_stream_configs:
+              - type: ParentStreamConfig
+                parent_key: id
+                partition_field: project_id
+                stream:
+                  $ref: "#/definitions/streams/projects"
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/tasks"
+  base_requester:
     type: HttpRequester
-    url_base: "https://api.clockify.me/api/v1/"
-    http_method: "GET"
+    url_base: https://api.clockify.me/api/v1/
     authenticator:
-      type: "ApiKeyAuthenticator"
-      header: "X-Api-Key"
+      type: ApiKeyAuthenticator
       api_token: "{{ config['api_key'] }}"
+      path: workspaces/{{ config['workspace_id'] }}/users
+      inject_into:
+        type: RequestOption
+        field_name: X-Api-Key
+        inject_into: header
 
-  retriever:
-    type: SimpleRetriever
-    record_selector:
-      $ref: "#/definitions/selector"
-    paginator:
-      type: "DefaultPaginator"
-      page_size_option:
-        type: "RequestOption"
-        inject_into: "request_parameter"
-        field_name: "page-size"
-      pagination_strategy:
-        type: "PageIncrement"
-        page_size: 50
-      page_token_option:
-        type: "RequestOption"
-        inject_into: "request_parameter"
-        field_name: "page"
-    requester:
-      $ref: "#/definitions/requester"
+streams:
+  - $ref: "#/definitions/streams/users"
+  - $ref: "#/definitions/streams/projects"
+  - $ref: "#/definitions/streams/clients"
+  - $ref: "#/definitions/streams/tags"
+  - $ref: "#/definitions/streams/user_groups"
+  - $ref: "#/definitions/streams/time_entries"
+  - $ref: "#/definitions/streams/tasks"
 
-  base_stream:
-    type: DeclarativeStream
-    retriever:
-      $ref: "#/definitions/retriever"
+spec:
+  type: Spec
+  connection_specification:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    required:
+      - api_key
+      - workspace_id
+    properties:
+      api_key:
+        type: string
+        title: API Key
+        airbyte_secret: true
+        description: >-
+          You can get your api access_key <a
+          href="https://app.clockify.me/user/settings">here</a> This API is Case
+          Sensitive.
+        order: 0
+      api_url:
+        type: string
+        title: API Url
+        description: >-
+          The URL for the Clockify API. This should only need to be modified if
+          connecting to an enterprise version of Clockify.
+        default: https://api.clockify.me
+        order: 1
+      workspace_id:
+        type: string
+        title: Workspace Id
+        description: WorkSpace Id
+        order: 2
+    additionalProperties: true
 
-  users_stream:
-    $ref: "#/definitions/base_stream"
-    name: "users"
-    primary_key: "id"
-    $parameters:
-      path: "workspaces/{{ config['workspace_id'] }}/users"
+metadata:
+  autoImportSchema:
+    users: false
+    projects: false
+    clients: false
+    tags: false
+    user_groups: false
+    time_entries: false
+    tasks: false
 
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/draft-07/schema#
-        additionalProperties: true
+schemas:
+  users:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    additionalProperties: true
+    properties:
+      activeWorkspace:
+        type:
+          - "null"
+          - string
+        description: The ID of the active workspace for the user.
+      customFields:
+        type:
+          - "null"
+          - array
+        description: Any custom fields associated with the user's profile.
+      defaultWorkspace:
+        type:
+          - "null"
+          - string
+        description: The default workspace ID for the user.
+      email:
+        type:
+          - "null"
+          - string
+        description: The email address of the user.
+      id:
+        type:
+          - "null"
+          - string
+        description: The unique identifier of the user.
+      memberships:
+        type:
+          - "null"
+          - array
+        description: List of memberships the user belongs to.
+      name:
+        type:
+          - "null"
+          - string
+        description: The name of the user.
+      profilePicture:
+        type:
+          - "null"
+          - string
+        description: URL to the user's profile picture.
+      settings:
+        type:
+          - "null"
+          - object
+        description: User-specific settings for the user account.
         properties:
-          activeWorkspace:
-            description: The ID of the active workspace for the user.
+          alerts:
             type:
               - "null"
-              - string
-          customFields:
-            description: Any custom fields associated with the user's profile.
+              - boolean
+            description: User's alerts settings.
+          approval:
             type:
               - "null"
-              - array
-          defaultWorkspace:
-            description: The default workspace ID for the user.
+              - boolean
+            description: User's approval settings.
+          collapseAllProjectLists:
+            type:
+              - "null"
+              - boolean
+            description: User's preference for collapsing all project lists.
+          dashboardPinToTop:
+            type:
+              - "null"
+              - boolean
+            description: User's preference for pinning dashboard to the top.
+          dashboardSelection:
             type:
               - "null"
               - string
-          email:
-            description: The email address of the user.
+            description: User's dashboard selection.
+          dashboardViewType:
             type:
               - "null"
               - string
-          id:
-            description: The unique identifier of the user.
+            description: User's preferred dashboard view type.
+          dateFormat:
             type:
               - "null"
               - string
-          memberships:
-            description: List of memberships the user belongs to.
+            description: User's preferred date format.
+          groupSimilarEntriesDisabled:
             type:
               - "null"
-              - array
-          name:
-            description: The name of the user.
+              - boolean
+            description: User's preference for grouping similar entries.
+          isCompactViewOn:
             type:
               - "null"
-              - string
-          profilePicture:
-            description: URL to the user's profile picture.
+              - boolean
+            description: User's preference for compact view.
+          lang:
             type:
               - "null"
               - string
-          settings:
-            description: User-specific settings for the user account.
-            properties:
-              alerts:
-                description: User's alerts settings.
-                type:
-                  - "null"
-                  - boolean
-              approval:
-                description: User's approval settings.
-                type:
-                  - "null"
-                  - boolean
-              collapseAllProjectLists:
-                description: User's preference for collapsing all project lists.
-                type:
-                  - "null"
-                  - boolean
-              dashboardPinToTop:
-                description: User's preference for pinning dashboard to the top.
-                type:
-                  - "null"
-                  - boolean
-              dashboardSelection:
-                description: User's dashboard selection.
-                type:
-                  - "null"
-                  - string
-              dashboardViewType:
-                description: User's preferred dashboard view type.
-                type:
-                  - "null"
-                  - string
-              dateFormat:
-                description: User's preferred date format.
-                type:
-                  - "null"
-                  - string
-              groupSimilarEntriesDisabled:
-                description: User's preference for grouping similar entries.
-                type:
-                  - "null"
-                  - boolean
-              isCompactViewOn:
-                description: User's preference for compact view.
-                type:
-                  - "null"
-                  - boolean
-              lang:
-                description: User's preferred language.
-                type:
-                  - "null"
-                  - string
-              longRunning:
-                description: User's long running settings.
-                type:
-                  - "null"
-                  - boolean
-              multiFactorEnabled:
-                description: Whether multi-factor authentication is enabled.
-                type:
-                  - "null"
-                  - boolean
-              myStartOfDay:
-                description: User's start of day setting.
-                type:
-                  - "null"
-                  - string
-              onboarding:
-                description: User's onboarding settings.
-                type:
-                  - "null"
-                  - boolean
-              projectListCollapse:
-                description: User's project list collapse setting.
-                type:
-                  - "null"
-                  - integer
-              projectPickerTaskFilter:
-                description: User's task filter for project picker.
-                type:
-                  - "null"
-                  - boolean
-              pto:
-                description: User's PTO settings.
-                type:
-                  - "null"
-                  - boolean
-              reminders:
-                description: User's reminder settings.
-                type:
-                  - "null"
-                  - boolean
-              scheduledReports:
-                description: User's scheduled reports settings.
-                type:
-                  - "null"
-                  - boolean
-              scheduling:
-                description: User's scheduling settings.
-                type:
-                  - "null"
-                  - boolean
-              sendNewsletter:
-                description: User's preference for receiving newsletters.
-                type:
-                  - "null"
-                  - boolean
-              showOnlyWorkingDays:
-                description: User's preference for showing only working days.
-                type:
-                  - "null"
-                  - boolean
-              summaryReportSettings:
-                description: Settings for summary report.
-                properties:
-                  group:
-                    description: Group setting for summary report.
-                    type:
-                      - "null"
-                      - string
-                  subgroup:
-                    description: Subgroup setting for summary report.
-                    type:
-                      - "null"
-                      - string
-                type:
-                  - "null"
-                  - object
-              theme:
-                description: User's preferred theme.
-                type:
-                  - "null"
-                  - string
-              timeFormat:
-                description: User's preferred time format.
-                type:
-                  - "null"
-                  - string
-              timeTrackingManual:
-                description: User's manual time tracking settings.
-                type:
-                  - "null"
-                  - boolean
-              timeZone:
-                description: User's preferred time zone.
-                type:
-                  - "null"
-                  - string
-              weekStart:
-                description: User's preferred start of the week.
-                type:
-                  - "null"
-                  - string
-              weeklyUpdates:
-                description: User's settings for receiving weekly updates.
-                type:
-                  - "null"
-                  - boolean
+            description: User's preferred language.
+          longRunning:
             type:
               - "null"
-              - object
-          status:
-            description: User's status.
+              - boolean
+            description: User's long running settings.
+          multiFactorEnabled:
+            type:
+              - "null"
+              - boolean
+            description: Whether multi-factor authentication is enabled.
+          myStartOfDay:
             type:
               - "null"
               - string
-        type: object
-  projects_stream:
-    $ref: "#/definitions/base_stream"
-    name: "projects"
-    primary_key: "id"
-    $parameters:
-      path: "workspaces/{{ config['workspace_id'] }}/projects"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/draft-07/schema#
-        additionalProperties: true
-        properties:
-          archived:
-            description: Indicates if the project is archived or not.
+            description: User's start of day setting.
+          onboarding:
             type:
               - "null"
               - boolean
-          billable:
-            description: Indicates if the project is billable or not.
+            description: User's onboarding settings.
+          projectListCollapse:
+            type:
+              - "null"
+              - integer
+            description: User's project list collapse setting.
+          projectPickerTaskFilter:
             type:
               - "null"
               - boolean
-          budgetEstimate:
-            description: The estimated budget for the project.
-            anyOf:
-              - type: "null"
-              - type: integer
-              - properties:
-                  estimate:
-                    type:
-                      - "null"
-                      - string
-                  type:
-                    type:
-                      - "null"
-                      - string
-                  resetOption:
-                    type:
-                      - "null"
-                      - string
-                  active:
-                    type:
-                      - "null"
-                      - boolean
-                type:
-                  - "null"
-                  - object
-          clientId:
-            description: The ID of the client associated with the project.
+            description: User's task filter for project picker.
+          pto:
             type:
               - "null"
-              - string
-          clientName:
-            description: The name of the client associated with the project.
+              - boolean
+            description: User's PTO settings.
+          reminders:
             type:
               - "null"
-              - string
-          color:
-            description: Color code used to visually identify the project.
+              - boolean
+            description: User's reminder settings.
+          scheduledReports:
             type:
               - "null"
-              - string
-          costRate:
-            description: Cost rate for the project.
-            anyOf:
-              - type: "null"
-              - type: string
-              - properties:
-                  amount:
-                    type:
-                      - "null"
-                      - string
-                      - integer
-                  currency:
-                    type:
-                      - "null"
-                      - string
-                type:
-                  - "null"
-                  - object
-          duration:
-            description: Total duration tracked for the project.
+              - boolean
+            description: User's scheduled reports settings.
+          scheduling:
             type:
               - "null"
-              - string
-          estimate:
-            description: Project estimation details.
-            properties:
-              estimate:
-                description: Estimated time for the project.
-                type: string
-              type:
-                description: Type of estimation (e.g., hours, days).
-                type: string
+              - boolean
+            description: User's scheduling settings.
+          sendNewsletter:
+            type:
+              - "null"
+              - boolean
+            description: User's preference for receiving newsletters.
+          showOnlyWorkingDays:
+            type:
+              - "null"
+              - boolean
+            description: User's preference for showing only working days.
+          summaryReportSettings:
             type:
               - "null"
               - object
-          hourlyRate:
-            description: Hourly rate for the project.
+            description: Settings for summary report.
             properties:
-              amount:
-                description: Hourly rate amount.
+              group:
                 type:
                   - "null"
-                  - integer
-              currency:
-                description: Currency of the hourly rate.
+                  - string
+                description: Group setting for summary report.
+              subgroup:
                 type:
                   - "null"
                   - string
+                description: Subgroup setting for summary report.
+          theme:
             type:
               - "null"
-              - object
-          id:
-            description: Unique identifier for the project.
+              - string
+            description: User's preferred theme.
+          timeFormat:
             type:
               - "null"
               - string
-          memberships:
-            description: List of project memberships.
-            items:
-              properties:
-                costRate:
-                  description: Cost rate for the membership.
-                  type:
-                    - "null"
-                hourlyRate:
-                  description: Hourly rate for the membership.
-                  anyOf:
-                    - type: "null"
-                    - properties:
-                        amount:
-                          type:
-                            - "null"
-                            - integer
-                        currency:
-                          type:
-                            - "null"
-                            - string
-                      type:
-                        - "null"
-                        - object
-                membershipStatus:
-                  description: Status of the membership.
-                  type:
-                    - "null"
-                    - string
-                membershipType:
-                  description: Type of membership.
-                  type:
-                    - "null"
-                    - string
-                targetId:
-                  description: ID of the target associated with the membership.
-                  type:
-                    - "null"
-                    - string
-                userId:
-                  description: ID of the user associated with the membership.
-                  type:
-                    - "null"
-                    - string
-              type:
-                - "null"
-                - object
+            description: User's preferred time format.
+          timeTrackingManual:
             type:
               - "null"
-              - array
-          name:
-            description: Name of the project.
+              - boolean
+            description: User's manual time tracking settings.
+          timeZone:
             type:
               - "null"
               - string
-          note:
-            description: Additional notes or comments related to the project.
+            description: User's preferred time zone.
+          weekStart:
             type:
               - "null"
               - string
-          public:
-            description: Indicates if the project is public or private.
+            description: User's preferred start of the week.
+          weeklyUpdates:
             type:
               - "null"
               - boolean
-          template:
-            description: Indicates if the project is a template or not.
-            type:
+            description: User's settings for receiving weekly updates.
+      status:
+        type:
+          - "null"
+          - string
+        description: User's status.
+  projects:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    additionalProperties: true
+    properties:
+      archived:
+        type:
+          - "null"
+          - boolean
+        description: Indicates if the project is archived or not.
+      billable:
+        type:
+          - "null"
+          - boolean
+        description: Indicates if the project is billable or not.
+      budgetEstimate:
+        anyOf:
+          - type: "null"
+          - type: integer
+          - type:
               - "null"
-              - boolean
-          timeEstimate:
-            description: Time estimation details for the project.
+              - object
             properties:
+              type:
+                type:
+                  - "null"
+                  - string
               active:
-                description: Indicates if the time estimate is active or not.
                 type:
                   - "null"
                   - boolean
               estimate:
-                description: Estimated time for the project.
                 type:
                   - "null"
                   - string
-              includeNonBillable:
-                description: Indicates if non-billable time is included in the estimate.
+              resetOption:
                 type:
                   - "null"
-                  - boolean
-              resetOption:
-                description: Option to reset the time estimate.
+                  - string
+        description: The estimated budget for the project.
+      clientId:
+        type:
+          - "null"
+          - string
+        description: The ID of the client associated with the project.
+      clientName:
+        type:
+          - "null"
+          - string
+        description: The name of the client associated with the project.
+      color:
+        type:
+          - "null"
+          - string
+        description: Color code used to visually identify the project.
+      costRate:
+        anyOf:
+          - type: "null"
+          - type: string
+          - type:
+              - "null"
+              - object
+            properties:
+              amount:
                 type:
                   - "null"
                   - string
-              type:
-                description: Type of time estimation (e.g., hours, days).
+                  - integer
+              currency:
                 type:
                   - "null"
                   - string
+        description: Cost rate for the project.
+      duration:
+        type:
+          - "null"
+          - string
+        description: Total duration tracked for the project.
+      estimate:
+        type:
+          - "null"
+          - object
+        description: Project estimation details.
+        properties:
+          type:
+            type: string
+            description: Type of estimation (e.g., hours, days).
+          estimate:
+            type: string
+            description: Estimated time for the project.
+      hourlyRate:
+        type:
+          - "null"
+          - object
+        description: Hourly rate for the project.
+        properties:
+          amount:
             type:
               - "null"
-              - object
-          workspaceId:
-            description: ID of the workspace to which the project belongs.
+              - integer
+            description: Hourly rate amount.
+          currency:
             type:
               - "null"
               - string
-        type: object
-  clients_stream:
-    $ref: "#/definitions/base_stream"
-    name: "clients"
-    primary_key: "id"
-    $parameters:
-      path: "workspaces/{{ config['workspace_id'] }}/clients"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/draft-07/schema#
-        additionalProperties: true
+            description: Currency of the hourly rate.
+      id:
+        type:
+          - "null"
+          - string
+        description: Unique identifier for the project.
+      memberships:
+        type:
+          - "null"
+          - array
+        description: List of project memberships.
+        items:
+          type:
+            - "null"
+            - object
+          properties:
+            costRate:
+              type:
+                - "null"
+              description: Cost rate for the membership.
+            hourlyRate:
+              anyOf:
+                - type: "null"
+                - type:
+                    - "null"
+                    - object
+                  properties:
+                    amount:
+                      type:
+                        - "null"
+                        - integer
+                    currency:
+                      type:
+                        - "null"
+                        - string
+              description: Hourly rate for the membership.
+            membershipStatus:
+              type:
+                - "null"
+                - string
+              description: Status of the membership.
+            membershipType:
+              type:
+                - "null"
+                - string
+              description: Type of membership.
+            targetId:
+              type:
+                - "null"
+                - string
+              description: ID of the target associated with the membership.
+            userId:
+              type:
+                - "null"
+                - string
+              description: ID of the user associated with the membership.
+      name:
+        type:
+          - "null"
+          - string
+        description: Name of the project.
+      note:
+        type:
+          - "null"
+          - string
+        description: Additional notes or comments related to the project.
+      public:
+        type:
+          - "null"
+          - boolean
+        description: Indicates if the project is public or private.
+      template:
+        type:
+          - "null"
+          - boolean
+        description: Indicates if the project is a template or not.
+      timeEstimate:
+        type:
+          - "null"
+          - object
+        description: Time estimation details for the project.
         properties:
-          address:
-            description: Client's physical address.
+          type:
             type:
               - "null"
               - string
-          archived:
-            description: Indicates if the client is archived (true) or active (false).
+            description: Type of time estimation (e.g., hours, days).
+          active:
             type:
               - "null"
               - boolean
-          id:
-            description: Unique identifier for the client.
-            type:
-              - "null"
-              - string
-          email:
-            description: Client's contact email address.
-            type:
-              - "null"
-              - string
-          name:
-            description: Name of the client.
-            type:
-              - "null"
-              - string
-          note:
-            description: Additional notes related to the client.
-            type:
-              - "null"
-              - string
-          workspaceId:
-            description: Identifier for the workspace to which the client belongs.
+            description: Indicates if the time estimate is active or not.
+          estimate:
             type:
               - "null"
               - string
-        type: object
-  tags_stream:
-    $ref: "#/definitions/base_stream"
-    name: "tags"
-    primary_key: "id"
-    $parameters:
-      path: "workspaces/{{ config['workspace_id'] }}/tags"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/draft-07/schema#
-        additionalProperties: true
-        properties:
-          archived:
-            description: Indicates if the tag is archived or active.
+            description: Estimated time for the project.
+          includeNonBillable:
             type:
               - "null"
               - boolean
-          id:
-            description: Unique identifier for the tag.
-            type:
-              - "null"
-              - string
-          name:
-            description: Name of the tag.
-            type:
-              - "null"
-              - string
-          workspaceId:
-            description: Identifier of the workspace to which the tag belongs.
-            type:
-              - "null"
-              - string
-        type: object
-  user_groups_stream:
-    $ref: "#/definitions/base_stream"
-    name: "user_groups"
-    primary_key: "id"
-    $parameters:
-      path: "workspaces/{{ config['workspace_id'] }}/user-groups"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/draft-07/schema#
-        additionalProperties: true
-        properties:
-          id:
-            description: Unique identifier for the user group.
+            description: Indicates if non-billable time is included in the estimate.
+          resetOption:
             type:
               - "null"
               - string
-          name:
-            description: Name of the user group.
-            type:
-              - "null"
-              - string
-          userIds:
-            description: List of user IDs belonging to the user group.
-            items:
-              description: User ID of a member in the group.
+            description: Option to reset the time estimate.
+      workspaceId:
+        type:
+          - "null"
+          - string
+        description: ID of the workspace to which the project belongs.
+  clients:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    additionalProperties: true
+    properties:
+      address:
+        type:
+          - "null"
+          - string
+        description: Client's physical address.
+      archived:
+        type:
+          - "null"
+          - boolean
+        description: Indicates if the client is archived (true) or active (false).
+      email:
+        type:
+          - "null"
+          - string
+        description: Client's contact email address.
+      id:
+        type:
+          - "null"
+          - string
+        description: Unique identifier for the client.
+      name:
+        type:
+          - "null"
+          - string
+        description: Name of the client.
+      note:
+        type:
+          - "null"
+          - string
+        description: Additional notes related to the client.
+      workspaceId:
+        type:
+          - "null"
+          - string
+        description: Identifier for the workspace to which the client belongs.
+  tags:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    additionalProperties: true
+    properties:
+      archived:
+        type:
+          - "null"
+          - boolean
+        description: Indicates if the tag is archived or active.
+      id:
+        type:
+          - "null"
+          - string
+        description: Unique identifier for the tag.
+      name:
+        type:
+          - "null"
+          - string
+        description: Name of the tag.
+      workspaceId:
+        type:
+          - "null"
+          - string
+        description: Identifier of the workspace to which the tag belongs.
+  user_groups:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    additionalProperties: true
+    properties:
+      id:
+        type:
+          - "null"
+          - string
+        description: Unique identifier for the user group.
+      name:
+        type:
+          - "null"
+          - string
+        description: Name of the user group.
+      userIds:
+        type:
+          - "null"
+          - array
+        description: List of user IDs belonging to the user group.
+        items:
+          type:
+            - "null"
+            - string
+          description: User ID of a member in the group.
+      workspaceId:
+        type:
+          - "null"
+          - string
+        description: Identifier for the workspace to which the user group belongs.
+  time_entries:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    additionalProperties: true
+    properties:
+      billable:
+        description: Indicates if the time entry is billable or not
+        type:
+          - "null"
+          - boolean
+      customFieldValues:
+        description: Values for custom fields related to the time entry
+        type:
+          - "null"
+          - array
+      description:
+        description: Description or notes about the time entry
+        type:
+          - "null"
+          - string
+      id:
+        description: Unique identifier for the time entry
+        type:
+          - "null"
+          - string
+      isLocked:
+        description: Indicates if the time entry is locked or not
+        type:
+          - "null"
+          - boolean
+      kioskId:
+        description: Identifier for the kiosk associated with the time entry
+        type:
+          - "null"
+          - string
+      projectId:
+        description: Unique identifier for the project related to the time entry
+        type:
+          - "null"
+          - string
+      tagIds:
+        description: Identifiers of tags associated with the time entry
+        anyOf:
+          - type: "null"
+          - items:
               type:
                 - "null"
                 - string
             type:
               - "null"
               - array
-          workspaceId:
-            description: Identifier for the workspace to which the user group belongs.
-            type:
-              - "null"
-              - string
-        type: object
-  users_partition_router:
-    type: SubstreamPartitionRouter
-    parent_stream_configs:
-      - stream: "#/definitions/users_stream"
-        parent_key: "id"
-        partition_field: "user_id"
-
-  time_entries_stream:
-    $ref: "#/definitions/base_stream"
-    $parameters:
-      name: "time_entries"
-      primary_key: "id"
-      path:
-        "workspaces/{{ config['workspace_id'] }}/user/{{ stream_partition.user_id
-        }}/time-entries"
-    retriever:
-      $ref: "#/definitions/retriever"
-      partition_router:
-        $ref: "#/definitions/users_partition_router"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/draft-07/schema#
-        additionalProperties: true
+      taskId:
+        description: Unique identifier for the task related to the time entry
+        type:
+          - "null"
+          - string
+      timeInterval:
+        description: Represents the time interval for the time entry
         properties:
-          billable:
-            description: Indicates if the time entry is billable or not
-            type:
-              - "null"
-              - boolean
-          customFieldValues:
-            description: Values for custom fields related to the time entry
-            type:
-              - "null"
-              - array
-          description:
-            description: Description or notes about the time entry
-            type:
-              - "null"
-              - string
-          id:
-            description: Unique identifier for the time entry
-            type:
-              - "null"
-              - string
-          isLocked:
-            description: Indicates if the time entry is locked or not
-            type:
-              - "null"
-              - boolean
-          kioskId:
-            description: Identifier for the kiosk associated with the time entry
+          duration:
+            description: Duration of the time entry
             type:
               - "null"
               - string
-          projectId:
-            description: Unique identifier for the project related to the time entry
+          end:
+            description: End timestamp of the time entry
             type:
               - "null"
               - string
-          tagIds:
-            description: Identifiers of tags associated with the time entry
-            anyOf:
-              - type: "null"
-              - items:
-                  type:
-                    - "null"
-                    - string
-                type:
-                  - "null"
-                  - array
-          taskId:
-            description: Unique identifier for the task related to the time entry
+          start:
+            description: Start timestamp of the time entry
             type:
               - "null"
               - string
-          timeInterval:
-            description: Represents the time interval for the time entry
-            properties:
-              duration:
-                description: Duration of the time entry
-                type:
-                  - "null"
-                  - string
-              end:
-                description: End timestamp of the time entry
+        type:
+          - "null"
+          - object
+      type:
+        description: Type of the time entry (e.g., time, leave, holiday)
+        type:
+          - "null"
+          - string
+      userId:
+        description: Unique identifier for the user associated with the time entry
+        type:
+          - "null"
+          - string
+      workspaceId:
+        description: Unique identifier for the workspace of the time entry
+        type:
+          - "null"
+          - string
+  tasks:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    additionalProperties: true
+    properties:
+      budgetEstimate:
+        description: Estimated budget for the task.
+        type:
+          - "null"
+          - number
+      assigneeId:
+        description: The unique identifier of the user assigned to the task.
+        type:
+          - "null"
+          - string
+      assigneeIds:
+        description: The list of unique identifiers of users assigned to the task.
+        items:
+          description: Unique identifier of a user.
+          type:
+            - "null"
+            - string
+        type:
+          - "null"
+          - array
+      billable:
+        description: Indicates whether the task is billable or not.
+        type:
+          - "null"
+          - boolean
+      costRate:
+        description: Cost rate associated with the task.
+        anyOf:
+          - type: "null"
+          - type: string
+          - properties:
+              amount:
                 type:
                   - "null"
                   - string
-              start:
-                description: Start timestamp of the time entry
+                  - integer
+              currency:
                 type:
                   - "null"
                   - string
             type:
               - "null"
               - object
-          type:
-            description: Type of the time entry (e.g., time, leave, holiday)
-            type:
-              - "null"
-              - string
-          userId:
-            description: Unique identifier for the user associated with the time entry
-            type:
-              - "null"
-              - string
-          workspaceId:
-            description: Unique identifier for the workspace of the time entry
-            type:
-              - "null"
-              - string
-        type: object
-  projects_partition_router:
-    type: SubstreamPartitionRouter
-    parent_stream_configs:
-      - stream: "#/definitions/projects_stream"
-        parent_key: "id"
-        partition_field: "project_id"
-
-  tasks_stream:
-    $ref: "#/definitions/base_stream"
-    $parameters:
-      name: "tasks"
-      primary_key: "id"
-      path:
-        "workspaces/{{ config['workspace_id'] }}/projects/{{ stream_partition.project_id
-        }}/tasks"
-    retriever:
-      $ref: "#/definitions/retriever"
-      partition_router:
-        $ref: "#/definitions/projects_partition_router"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/draft-07/schema#
-        additionalProperties: true
-        properties:
-          budgetEstimate:
-            description: Estimated budget for the task.
-            type:
-              - "null"
-              - number
-          assigneeId:
-            description: The unique identifier of the user assigned to the task.
-            type:
-              - "null"
-              - string
-          assigneeIds:
-            description: The list of unique identifiers of users assigned to the task.
-            items:
-              description: Unique identifier of a user.
-              type:
-                - "null"
-                - string
-            type:
-              - "null"
-              - array
-          billable:
-            description: Indicates whether the task is billable or not.
-            type:
-              - "null"
-              - boolean
-          costRate:
-            description: Cost rate associated with the task.
-            anyOf:
-              - type: "null"
-              - type: string
-              - properties:
-                  amount:
-                    type:
-                      - "null"
-                      - string
-                      - integer
-                  currency:
-                    type:
-                      - "null"
-                      - string
+      duration:
+        description: Total duration of the task.
+        type:
+          - "null"
+          - string
+      estimate:
+        description: Estimated time required to complete the task.
+        type:
+          - "null"
+          - string
+      hourlyRate:
+        description: Hourly rate for billing purposes.
+        anyOf:
+          - type: "null"
+          - properties:
+              amount:
                 type:
                   - "null"
-                  - object
-          duration:
-            description: Total duration of the task.
-            type:
-              - "null"
-              - string
-          estimate:
-            description: Estimated time required to complete the task.
-            type:
-              - "null"
-              - string
-          hourlyRate:
-            description: Hourly rate for billing purposes.
-            anyOf:
-              - type: "null"
-              - properties:
-                  amount:
-                    type:
-                      - "null"
-                      - integer
-                  currency:
-                    type:
-                      - "null"
-                      - string
+                  - integer
+              currency:
                 type:
                   - "null"
-                  - object
-          id:
-            description: Unique identifier of the task.
-            type:
-              - "null"
-              - string
-          name:
-            description: Name or title of the task.
-            type:
-              - "null"
-              - string
-          projectId:
-            description: Unique identifier of the project the task belongs to.
-            type:
-              - "null"
-              - string
-          status:
-            description: Current status of the task.
-            type:
-              - "null"
-              - string
-          userGroupIds:
-            description:
-              List of unique identifiers of user groups associated with
-              the task.
+                  - string
             type:
               - "null"
-              - array
-        type: object
-streams:
-  - "#/definitions/users_stream"
-  - "#/definitions/projects_stream"
-  - "#/definitions/clients_stream"
-  - "#/definitions/tags_stream"
-  - "#/definitions/user_groups_stream"
-  - "#/definitions/time_entries_stream"
-  - "#/definitions/tasks_stream"
-
-check:
-  type: CheckStream
-  stream_names:
-    - "users"
-    - "projects"
-    - "clients"
-    - "tags"
-    - "user_groups"
-    - "time_entries"
-    - "tasks"
+              - object
+      id:
+        description: Unique identifier of the task.
+        type:
+          - "null"
+          - string
+      name:
+        description: Name or title of the task.
+        type:
+          - "null"
+          - string
+      projectId:
+        description: Unique identifier of the project the task belongs to.
+        type:
+          - "null"
+          - string
+      status:
+        description: Current status of the task.
+        type:
+          - "null"
+          - string
+      userGroupIds:
+        description: List of unique identifiers of user groups associated with
+          the task.
+        type:
+          - "null"
+          - array
```

### Comparing `airbyte_source_clockify-0.3.3/PKG-INFO` & `airbyte_source_clockify-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-clockify
-Version: 0.3.3
+Version: 0.3.4
 Summary: Source implementation for Clockify.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -15,96 +15,110 @@
 Requires-Dist: airbyte-cdk (==0.80.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/clockify
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Clockify source connector
 
-
 This is the repository for the Clockify source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/clockify).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
-
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/clockify)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_clockify/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-clockify spec
 poetry run source-clockify check --config secrets/config.json
 poetry run source-clockify discover --config secrets/config.json
 poetry run source-clockify read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
+
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
+
 ```bash
 airbyte-ci connectors --name=source-clockify build
 ```
 
 An image will be available on your host with the tag `airbyte/source-clockify:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-clockify:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-clockify:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-clockify:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-clockify:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-clockify test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
-All of your dependencies should be managed via Poetry. 
+
+All of your dependencies should be managed via Poetry.
 To add a new dependency, run:
+
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-clockify test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/clockify.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```

