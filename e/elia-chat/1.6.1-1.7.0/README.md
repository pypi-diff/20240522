# Comparing `tmp/elia_chat-1.6.1.tar.gz` & `tmp/elia_chat-1.7.0.tar.gz`

## Comparing `elia_chat-1.6.1.tar` & `elia_chat-1.7.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 elia_chat-1.6.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 elia_chat-1.6.1/.python-version
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 elia_chat-1.6.1/requirements-dev.lock
--rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 elia_chat-1.6.1/requirements.lock
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 elia_chat-1.6.1/.idea/.gitignore
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 elia_chat-1.6.1/.idea/elia.iml
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 elia_chat-1.6.1/.idea/misc.xml
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 elia_chat-1.6.1/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 elia_chat-1.6.1/.idea/vcs.xml
--rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 elia_chat-1.6.1/.idea/workspace.xml
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 elia_chat-1.6.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 elia_chat-1.6.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 elia_chat-1.6.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/__init__.py
--rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/__main__.py
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/app.py
--rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/chats_manager.py
--rw-r--r--   0        0        0     6340 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/config.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/constants.py
--rw-r--r--   0        0        0     9138 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/elia.scss
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/launch_args.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/locations.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/models.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/runtime_config.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/time_display.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/database/__init__.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/database/converters.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/database/database.py
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/database/import_chatgpt.py
--rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/database/models.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/screens/chat_details.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/screens/chat_screen.py
--rw-r--r--   0        0        0     5936 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/screens/help_screen.py
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/screens/home_screen.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/widgets/agent_is_typing.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/widgets/app_header.py
--rw-r--r--   0        0        0    11022 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/widgets/chat.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/widgets/chat_header.py
--rw-r--r--   0        0        0     5677 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/widgets/chat_list.py
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/widgets/chat_options.py
--rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/widgets/chatbox.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/widgets/prompt_input.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 elia_chat-1.6.1/elia_chat/widgets/token_analysis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.6.1/tests/__init__.py
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 elia_chat-1.6.1/.gitignore
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 elia_chat-1.6.1/README.md
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 elia_chat-1.6.1/pyproject.toml
--rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 elia_chat-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 elia_chat-1.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 elia_chat-1.7.0/.python-version
+-rw-r--r--   0        0        0     4983 2020-02-02 00:00:00.000000 elia_chat-1.7.0/requirements-dev.lock
+-rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 elia_chat-1.7.0/requirements.lock
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 elia_chat-1.7.0/.idea/.gitignore
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 elia_chat-1.7.0/.idea/elia.iml
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 elia_chat-1.7.0/.idea/misc.xml
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 elia_chat-1.7.0/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 elia_chat-1.7.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 elia_chat-1.7.0/.idea/workspace.xml
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 elia_chat-1.7.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 elia_chat-1.7.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 elia_chat-1.7.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/__init__.py
+-rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/__main__.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/app.py
+-rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/chats_manager.py
+-rw-r--r--   0        0        0     6340 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/config.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/constants.py
+-rw-r--r--   0        0        0     9510 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/elia.scss
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/launch_args.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/locations.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/models.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/runtime_config.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/time_display.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/database/__init__.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/database/converters.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/database/database.py
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/database/import_chatgpt.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/database/models.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/screens/chat_details.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/screens/chat_screen.py
+-rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/screens/help_screen.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/screens/home_screen.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/screens/rename_chat_screen.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/widgets/agent_is_typing.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/widgets/app_header.py
+-rw-r--r--   0        0        0    11659 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/widgets/chat.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/widgets/chat_header.py
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/widgets/chat_list.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/widgets/chat_options.py
+-rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/widgets/chatbox.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/widgets/prompt_input.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 elia_chat-1.7.0/elia_chat/widgets/token_analysis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.7.0/tests/__init__.py
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 elia_chat-1.7.0/.gitignore
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 elia_chat-1.7.0/README.md
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 elia_chat-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 elia_chat-1.7.0/PKG-INFO
```

### Comparing `elia_chat-1.6.1/.pre-commit-config.yaml` & `elia_chat-1.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `elia_chat-1.6.1/requirements-dev.lock` & `elia_chat-1.7.0/requirements-dev.lock`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     # via textual-dev
 aiosignal==1.3.1
     # via aiohttp
 aiosqlite==0.20.0
     # via elia-chat
 annotated-types==0.6.0
     # via pydantic
-anyio==4.2.0
+anyio==4.3.0
     # via httpx
     # via openai
 attrs==23.2.0
     # via aiohttp
 black==24.1.1
 cachetools==5.3.3
     # via google-auth
@@ -47,15 +47,15 @@
     # via openai
 filelock==3.13.1
     # via huggingface-hub
     # via virtualenv
 frozenlist==1.4.1
     # via aiohttp
     # via aiosignal
-fsspec==2024.3.1
+fsspec==2024.5.0
     # via huggingface-hub
 google-ai-generativelanguage==0.6.3
     # via google-generativeai
 google-api-core==2.19.0
     # via google-ai-generativelanguage
     # via google-api-python-client
     # via google-generativeai
@@ -72,46 +72,47 @@
 google-generativeai==0.5.3
     # via elia-chat
 googleapis-common-protos==1.63.0
     # via google-api-core
     # via grpcio-status
 greenlet==3.0.3
     # via elia-chat
+    # via sqlalchemy
 grpcio==1.63.0
     # via google-api-core
     # via grpcio-status
 grpcio-status==1.62.2
     # via google-api-core
 h11==0.14.0
     # via httpcore
-httpcore==1.0.2
+httpcore==1.0.5
     # via httpx
 httplib2==0.22.0
     # via google-api-python-client
     # via google-auth-httplib2
-httpx==0.26.0
+httpx==0.27.0
     # via openai
-huggingface-hub==0.22.2
+huggingface-hub==0.23.1
     # via tokenizers
 humanize==4.9.0
     # via elia-chat
 identify==2.5.34
     # via pre-commit
 idna==3.6
     # via anyio
     # via httpx
     # via requests
     # via yarl
 importlib-metadata==7.1.0
     # via litellm
-jinja2==3.1.3
+jinja2==3.1.4
     # via litellm
 linkify-it-py==2.0.3
     # via markdown-it-py
-litellm==1.35.38
+litellm==1.37.19
     # via elia-chat
 markdown-it-py==3.0.0
     # via mdit-py-plugins
     # via rich
     # via textual
 markupsafe==2.1.5
     # via jinja2
@@ -126,15 +127,15 @@
     # via yarl
 mypy==1.8.0
 mypy-extensions==1.0.0
     # via black
     # via mypy
 nodeenv==1.8.0
     # via pre-commit
-openai==1.12.0
+openai==1.30.1
     # via litellm
 packaging==23.2
     # via black
     # via huggingface-hub
 pathspec==0.12.1
     # via black
 platformdirs==4.2.0
@@ -170,40 +171,40 @@
 pyperclip==1.8.2
     # via elia-chat
 python-dotenv==1.0.1
     # via litellm
 pyyaml==6.0.1
     # via huggingface-hub
     # via pre-commit
-regex==2023.12.25
+regex==2024.5.15
     # via tiktoken
 requests==2.31.0
     # via google-api-core
     # via huggingface-hub
     # via litellm
     # via tiktoken
 rich==13.7.0
     # via textual
 rsa==4.9
     # via google-auth
 setuptools==69.0.3
     # via nodeenv
-sniffio==1.3.0
+sniffio==1.3.1
     # via anyio
     # via httpx
     # via openai
 sqlalchemy==2.0.25
     # via sqlmodel
 sqlmodel==0.0.14
     # via elia-chat
-textual==0.62.0
+textual==0.60.0
     # via elia-chat
     # via textual-dev
 textual-dev==1.4.0
-tiktoken==0.5.2
+tiktoken==0.7.0
     # via litellm
 tokenizers==0.19.1
     # via litellm
 tqdm==4.66.2
     # via google-generativeai
     # via huggingface-hub
     # via openai
@@ -232,9 +233,9 @@
     # via requests
 virtualenv==20.25.0
     # via pre-commit
 xdg-base-dirs==6.0.1
     # via elia-chat
 yarl==1.9.4
     # via aiohttp
-zipp==3.18.1
+zipp==3.18.2
     # via importlib-metadata
```

### Comparing `elia_chat-1.6.1/requirements.lock` & `elia_chat-1.7.0/requirements.lock`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     # via litellm
 aiosignal==1.3.1
     # via aiohttp
 aiosqlite==0.20.0
     # via elia-chat
 annotated-types==0.6.0
     # via pydantic
-anyio==4.2.0
+anyio==4.3.0
     # via httpx
     # via openai
 attrs==23.2.0
     # via aiohttp
 cachetools==5.3.3
     # via google-auth
 certifi==2024.2.2
@@ -33,20 +33,20 @@
     # via click-default-group
     # via elia-chat
     # via litellm
 click-default-group==1.2.4
     # via elia-chat
 distro==1.9.0
     # via openai
-filelock==3.13.4
+filelock==3.14.0
     # via huggingface-hub
 frozenlist==1.4.1
     # via aiohttp
     # via aiosignal
-fsspec==2024.3.1
+fsspec==2024.5.0
     # via huggingface-hub
 google-ai-generativelanguage==0.6.3
     # via google-generativeai
 google-api-core==2.19.0
     # via google-ai-generativelanguage
     # via google-api-python-client
     # via google-generativeai
@@ -63,61 +63,62 @@
 google-generativeai==0.5.3
     # via elia-chat
 googleapis-common-protos==1.63.0
     # via google-api-core
     # via grpcio-status
 greenlet==3.0.3
     # via elia-chat
+    # via sqlalchemy
 grpcio==1.63.0
     # via google-api-core
     # via grpcio-status
 grpcio-status==1.62.2
     # via google-api-core
 h11==0.14.0
     # via httpcore
-httpcore==1.0.2
+httpcore==1.0.5
     # via httpx
 httplib2==0.22.0
     # via google-api-python-client
     # via google-auth-httplib2
-httpx==0.26.0
+httpx==0.27.0
     # via openai
-huggingface-hub==0.22.2
+huggingface-hub==0.23.1
     # via tokenizers
 humanize==4.9.0
     # via elia-chat
 idna==3.6
     # via anyio
     # via httpx
     # via requests
     # via yarl
 importlib-metadata==7.1.0
     # via litellm
-jinja2==3.1.3
+jinja2==3.1.4
     # via litellm
 linkify-it-py==2.0.3
     # via markdown-it-py
-litellm==1.35.38
+litellm==1.37.19
     # via elia-chat
 markdown-it-py==3.0.0
     # via mdit-py-plugins
     # via rich
     # via textual
 markupsafe==2.1.5
     # via jinja2
 mdit-py-plugins==0.4.0
     # via markdown-it-py
 mdurl==0.1.2
     # via markdown-it-py
 multidict==6.0.5
     # via aiohttp
     # via yarl
-openai==1.12.0
+openai==1.30.1
     # via litellm
-packaging==23.2
+packaging==24.0
     # via huggingface-hub
 proto-plus==1.23.0
     # via google-ai-generativelanguage
     # via google-api-core
 protobuf==4.25.3
     # via google-ai-generativelanguage
     # via google-api-core
@@ -142,36 +143,36 @@
     # via httplib2
 pyperclip==1.8.2
     # via elia-chat
 python-dotenv==1.0.1
     # via litellm
 pyyaml==6.0.1
     # via huggingface-hub
-regex==2023.12.25
+regex==2024.5.15
     # via tiktoken
 requests==2.31.0
     # via google-api-core
     # via huggingface-hub
     # via litellm
     # via tiktoken
 rich==13.7.0
     # via textual
 rsa==4.9
     # via google-auth
-sniffio==1.3.0
+sniffio==1.3.1
     # via anyio
     # via httpx
     # via openai
 sqlalchemy==2.0.25
     # via sqlmodel
 sqlmodel==0.0.14
     # via elia-chat
-textual==0.62.0
+textual==0.60.0
     # via elia-chat
-tiktoken==0.5.2
+tiktoken==0.7.0
     # via litellm
 tokenizers==0.19.1
     # via litellm
 tqdm==4.66.2
     # via google-generativeai
     # via huggingface-hub
     # via openai
@@ -195,9 +196,9 @@
     # via google-api-python-client
 urllib3==2.2.0
     # via requests
 xdg-base-dirs==6.0.1
     # via elia-chat
 yarl==1.9.4
     # via aiohttp
-zipp==3.18.1
+zipp==3.18.2
     # via importlib-metadata
```

### Comparing `elia_chat-1.6.1/.idea/elia.iml` & `elia_chat-1.7.0/.idea/elia.iml`

 * *Files identical despite different names*

### Comparing `elia_chat-1.6.1/.idea/workspace.xml` & `elia_chat-1.7.0/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `elia_chat-1.6.1/.idea/inspectionProfiles/Project_Default.xml` & `elia_chat-1.7.0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `elia_chat-1.6.1/elia_chat/__main__.py` & `elia_chat-1.7.0/elia_chat/__main__.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.6.1/elia_chat/app.py` & `elia_chat-1.7.0/elia_chat/app.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.6.1/elia_chat/chats_manager.py` & `elia_chat-1.7.0/elia_chat/chats_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 
     @staticmethod
     async def get_chat(chat_id: int) -> ChatData:
         chat_dao = await ChatDao.from_id(chat_id)
         return chat_dao_to_chat_data(chat_dao)
 
     @staticmethod
+    async def rename_chat(chat_id: int, new_title: str) -> None:
+        await ChatDao.rename_chat(chat_id, new_title)
+
+    @staticmethod
     async def get_messages(
         chat_id: int,
     ) -> list[ChatMessage]:
         async with get_session() as session:
             try:
                 chat: ChatDao | None = await session.get(ChatDao, chat_id)
             except ValueError:
@@ -62,15 +66,15 @@
 
         model = chat_data.model
         lookup_key = model.lookup_key
         async with get_session() as session:
             chat = ChatDao(
                 model=lookup_key,
                 title="",
-                started_at=datetime.datetime.now(datetime.UTC),
+                started_at=datetime.datetime.now(datetime.timezone.utc),
             )
             session.add(chat)
             await session.commit()
 
             chat_id = chat.id
             for message in chat_data.messages:
                 litellm_message = message.message
```

### Comparing `elia_chat-1.6.1/elia_chat/config.py` & `elia_chat-1.7.0/elia_chat/config.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.6.1/elia_chat/elia.scss` & `elia_chat-1.7.0/elia_chat/elia.scss`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 $main-lighten-2: #9061F9;
 $main-lighten-1: #7E3AF2;
 $main: #6C2BD9;
 $main-darken-1: #5521B5;
 $main-darken-2: #4A1D96;
 $main-border-text-color: greenyellow 70%;
-$main-border-color: $main-lighten-1 50%;
-$main-border-color-focus: $main-lighten-1 100%;
+$main-border-color: $main-lighten-1 90%;
+$main-border-color-focus: $main-lighten-2 100%;
 
 $left-border-trim: vkey $main-lighten-2 15%;
 
 * {
   scrollbar-color: $panel;
   scrollbar-color-hover: $main-lighten-1 40%;
   scrollbar-color-active: $main-darken-1;
@@ -323,45 +323,61 @@
 }
 
 OptionList > .option-list--option-hover-highlighted-disabled {
   color: $text-disabled;
   background: $main 60%;
 }
 
-ChatDetails {
-  align: center middle;
+RenameChat {
+  & > Vertical {
+    background: $background 0%;
+    height: auto;
+    & Input {
+      padding: 0 4;
+      border: none;
+      border-bottom: hkey $main-border-color;
+      border-top: hkey $main-border-color;
+      border-subtitle-color: $main-border-text-color;
+      border-subtitle-background: $background;
+    }
+  }
+
 }
 
-ChatDetails > #container {
-  width: 90%;
-  height: 85%;
-  background: $background;
-  padding: 1 2;
-  border: wide $main-border-color-focus;
-  border-title-color: $main-border-text-color;
-  border-title-background: $background;
-  border-title-style: b;
-  border-subtitle-color: $text-muted;
-  border-subtitle-background: $background;
+ChatDetails {
+  align: center middle;
+  & > #container {
+    width: 90%;
+    height: 85%;
+    background: $background;
+    padding: 1 2;
+    border: wide $main-border-color-focus;
+    border-title-color: $main-border-text-color;
+    border-title-background: $background;
+    border-title-style: b;
+    border-subtitle-color: $text-muted;
+    border-subtitle-background: $background;
+
+    & Markdown {
+      padding: 0;
+      margin: 0;
+    }
 
-  & Markdown {
-    padding: 0;
-    margin: 0;
-  }
+    & .heading {
+      color: $text-muted;
+    }
 
-  & .heading {
-    color: $text-muted;
-  }
+    & .datum {
+      text-style: i;
+    }
 
-  & .datum {
-    text-style: i;
   }
-
 }
 
+
 MessageInfo #message-info-header {
   dock: top;
   width: 1fr;
   height: auto;
   background: $main-darken-2 70%;
   color: $text;
 }
```

### Comparing `elia_chat-1.6.1/elia_chat/locations.py` & `elia_chat-1.7.0/elia_chat/locations.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.6.1/elia_chat/models.py` & `elia_chat-1.7.0/elia_chat/models.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.6.1/elia_chat/time_display.py` & `elia_chat-1.7.0/elia_chat/time_display.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.6.1/elia_chat/database/converters.py` & `elia_chat-1.7.0/elia_chat/database/converters.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.6.1/elia_chat/database/database.py` & `elia_chat-1.7.0/elia_chat/database/database.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.6.1/elia_chat/database/import_chatgpt.py` & `elia_chat-1.7.0/elia_chat/database/import_chatgpt.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.6.1/elia_chat/database/models.py` & `elia_chat-1.7.0/elia_chat/database/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                 .group_by(MessageDao.chat_id)
                 .alias("subquery")
             )
 
             statement = (
                 select(ChatDao)
                 .join(subquery, subquery.c.chat_id == ChatDao.id)
-                .where(ChatDao.archived == False)
+                .where(ChatDao.archived == False)  # noqa: E712
                 .order_by(desc(subquery.c.max_timestamp))
                 .options(selectinload(ChatDao.messages))
             )
             results = await session.exec(statement)
             return list(results)
 
     @staticmethod
@@ -88,7 +88,15 @@
             statement = (
                 select(ChatDao)
                 .where(ChatDao.id == int(chat_id))
                 .options(selectinload(ChatDao.messages))
             )
             result = await session.exec(statement)
             return result.one()
+
+    @staticmethod
+    async def rename_chat(chat_id: int, new_title: str) -> None:
+        async with get_session() as session:
+            chat = await ChatDao.from_id(chat_id)
+            chat.title = new_title
+            session.add(chat)
+            await session.commit()
```

### Comparing `elia_chat-1.6.1/elia_chat/screens/chat_details.py` & `elia_chat-1.7.0/elia_chat/screens/chat_details.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import timezone
 from typing import TYPE_CHECKING, cast
 import humanize
 from textual.app import ComposeResult
 from textual.binding import Binding
 from textual.containers import Horizontal, Vertical, VerticalScroll
 from textual.screen import ModalScreen
 from textual.widgets import Label, Markdown, Rule
@@ -61,29 +62,31 @@
                     if provider := model.provider:
                         yield Label(provider, classes="datum")
 
                     yield Rule()
 
                     yield Label("First message", classes="heading")
                     if chat.create_timestamp:
-                        create_timestamp = chat.create_timestamp.replace(tzinfo=None)
+                        create_timestamp = chat.create_timestamp.replace(
+                            tzinfo=timezone.utc
+                        )
                         yield Label(
                             f"{humanize.naturaltime(create_timestamp)}",
                             classes="datum",
                         )
                     else:
                         yield Label("N/A")
 
                     yield Rule()
 
-                    update_time = chat.update_time
+                    update_time = chat.update_time.replace(tzinfo=timezone.utc)
                     yield Label("Updated at", classes="heading")
                     if update_time:
                         yield Label(
-                            f"{humanize.naturaltime(chat.update_time.replace(tzinfo=None))}",
+                            f"{humanize.naturaltime(chat.update_time)}",
                             classes="datum",
                         )
                     else:
                         yield Label("N/A")
 
                     yield Rule()
```

### Comparing `elia_chat-1.6.1/elia_chat/screens/chat_screen.py` & `elia_chat-1.7.0/elia_chat/screens/chat_screen.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.6.1/elia_chat/screens/help_screen.py` & `elia_chat-1.7.0/elia_chat/screens/help_screen.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,17 +47,18 @@
 
 If you can see a scrollbar, `pageup`, `pagedown`, `home`, and `end` can also
 be used to navigate.
 
 On the chat screen, pressing `up` and `down` will navigate through messages,
 but if you just wish to scroll a little, you can use `shift+up` and `shift+down`.
 
-### The chat history
+### The chat list
 
 - `up,down,k,j`: Navigate through chats.
+- `a`: Archive the highlighted chat.
 - `pageup,pagedown`: Up/down a page.
 - `home,end`: Go to first/last chat.
 - `g,G`: Go to first/last chat.
 - `enter,l`: Open chat.
 
 ### The options window
 
@@ -116,18 +117,19 @@
 
 The arrow keys can also be used to move focus _out_ of the prompt box.
 For example, pressing `up` while the prompt is focussed on the chat screen
 and the cursor is at (0, 0) will move focus to the latest message.
 
 ### The chat screen
 
-Press `shift+tab` to focus the latest message (or move the cursor `up` from (0, 0)).
-
 You can use the arrow keys to move up and down through messages.
 
+- `ctrl+r`: Rename the chat (or click the chat title).
+- `f2`: View more information about the chat.
+
 _With a message focused_:
 
 - `y,c`: Copy the raw Markdown of the message to the clipboard.
     - This requires terminal support. The default MacOS terminal is not supported.
 - `enter`: Enter _select mode_.
     - In this mode, you can move a cursor through the text, optionally holding
         `shift` to select text as you move.
@@ -138,15 +140,14 @@
 - `enter`: View more details about a message.
     - The amount of details available may vary depending on the model
         or provider being used.
 - `g`: Focus the first message.
 - `G`: Focus the latest message.
 - `m`: Move focus to the prompt box.
 - `up,down,k,j`: Navigate through messages.
-- `f2`: View more information about the chat.
 
 """
 
     def compose(self) -> ComposeResult:
         with Vertical(id="help-container") as vertical:
             vertical.border_title = "Elia Help"
             with VerticalScroll():
```

### Comparing `elia_chat-1.6.1/elia_chat/screens/home_screen.py` & `elia_chat-1.7.0/elia_chat/screens/home_screen.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.6.1/elia_chat/widgets/app_header.py` & `elia_chat-1.7.0/elia_chat/widgets/app_header.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.6.1/elia_chat/widgets/chat.py` & `elia_chat-1.7.0/elia_chat/widgets/chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from textual.reactive import reactive
 from textual.widget import Widget
 
 from elia_chat.chats_manager import ChatsManager
 from elia_chat.models import ChatData, ChatMessage
 from elia_chat.screens.chat_details import ChatDetails
 from elia_chat.widgets.agent_is_typing import AgentIsTyping
-from elia_chat.widgets.chat_header import ChatHeader
+from elia_chat.widgets.chat_header import ChatHeader, TitleStatic
 from elia_chat.widgets.prompt_input import PromptInput
 from elia_chat.widgets.chatbox import Chatbox
 
 
 if TYPE_CHECKING:
     from elia_chat.app import Elia
     from litellm.types.completion import (
@@ -33,14 +33,15 @@
 
 class ChatPromptInput(PromptInput):
     BINDINGS = [Binding("escape", "app.pop_screen", "Close chat", key_display="esc")]
 
 
 class Chat(Widget):
     BINDINGS = [
+        Binding("ctrl+r", "rename", "Rename", key_display="^r"),
         Binding("shift+down", "scroll_container_down", show=False),
         Binding("shift+up", "scroll_container_up", show=False),
         Binding(
             key="g",
             action="focus_first_message",
             description="First message",
             key_display="g",
@@ -126,15 +127,15 @@
         original_prompt = event.last_message.message.get("content", "")
         if isinstance(original_prompt, str):
             self.query_one(ChatPromptInput).text = original_prompt
 
     async def new_user_message(self, content: str) -> None:
         log.debug(f"User message submitted in chat {self.chat_data.id!r}: {content!r}")
 
-        now_utc = datetime.datetime.now(datetime.UTC)
+        now_utc = datetime.datetime.now(datetime.timezone.utc)
         user_message: ChatCompletionUserMessageParam = {
             "content": content,
             "role": "user",
         }
 
         user_chat_message = ChatMessage(user_message, now_utc, self.chat_data.model)
         self.chat_data.messages.append(user_chat_message)
@@ -189,15 +190,15 @@
             self.post_message(self.AgentResponseFailed(self.chat_data.messages[-1]))
             return
 
         ai_message: ChatCompletionAssistantMessageParam = {
             "content": "",
             "role": "assistant",
         }
-        now = datetime.datetime.now(datetime.UTC)
+        now = datetime.datetime.now(datetime.timezone.utc)
         message = ChatMessage(message=ai_message, model=model, timestamp=now)
 
         response_chatbox = Chatbox(
             message=message,
             model=self.chat_data.model,
             classes="response-in-progress",
         )
@@ -264,23 +265,35 @@
     async def on_cursor_up_from_prompt(self) -> None:
         self.focus_latest_message()
 
     @on(Chatbox.CursorEscapingBottom)
     def move_focus_to_prompt(self) -> None:
         self.query_one(ChatPromptInput).focus()
 
+    @on(TitleStatic.ChatRenamed)
+    async def handle_chat_rename(self, event: TitleStatic.ChatRenamed) -> None:
+        if event.chat_id == self.chat_data.id and event.new_title:
+            self.chat_data.title = event.new_title
+            header = self.query_one(ChatHeader)
+            header.update_header(self.chat_data, self.model)
+            await ChatsManager.rename_chat(event.chat_id, event.new_title)
+
     def get_latest_chatbox(self) -> Chatbox:
         return self.query(Chatbox).last()
 
     def focus_latest_message(self) -> None:
         try:
             self.get_latest_chatbox().focus()
         except NoMatches:
             pass
 
+    def action_rename(self) -> None:
+        title_static = self.query_one(TitleStatic)
+        title_static.begin_rename()
+
     def action_focus_latest_message(self) -> None:
         self.focus_latest_message()
 
     def action_focus_first_message(self) -> None:
         try:
             self.query(Chatbox).first().focus()
         except NoMatches:
```

### Comparing `elia_chat-1.6.1/elia_chat/widgets/chat_list.py` & `elia_chat-1.7.0/elia_chat/widgets/chat_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 class ChatListItemRenderable:
     chat: ChatData
     config: LaunchConfig
 
     def __rich_console__(
         self, console: Console, options: ConsoleOptions
     ) -> RenderResult:
-        now = datetime.datetime.now(datetime.UTC)
+        now = datetime.datetime.now(datetime.timezone.utc)
         delta = now - self.chat.update_time
         time_ago = humanize.naturaltime(delta)
         time_ago_text = Text(time_ago, style="dim i")
         model = self.chat.model
         subtitle = f"[dim]{escape(model.display_name or model.name)}"
         if model.provider:
             subtitle += f" [i]by[/] {escape(model.provider)}"
@@ -135,15 +135,18 @@
         self.remove_option_at_index(self.highlighted)
 
         chat_id = item.chat.id
         await ChatsManager.archive_chat(chat_id)
 
         self.border_title = self.get_border_title()
         self.refresh()
-        self.app.notify(f"Chat [b]{chat_id!r}[/] archived")
+        self.app.notify(
+            item.chat.title or f"Chat [b]{chat_id!r}[/] archived.",
+            title="Chat archived",
+        )
 
     def get_border_title(self) -> str:
         return f"History ({len(self.options)})"
 
     def create_chat(self, chat_data: ChatData) -> None:
         new_chat_list_item = ChatListItem(chat_data, self.app.launch_config)
         log.debug(f"Creating new chat {new_chat_list_item!r}")
```

### Comparing `elia_chat-1.6.1/elia_chat/widgets/chat_options.py` & `elia_chat-1.7.0/elia_chat/widgets/chat_options.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.6.1/elia_chat/widgets/chatbox.py` & `elia_chat-1.7.0/elia_chat/widgets/chatbox.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.6.1/elia_chat/widgets/prompt_input.py` & `elia_chat-1.7.0/elia_chat/widgets/prompt_input.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.6.1/elia_chat/widgets/token_analysis.py` & `elia_chat-1.7.0/elia_chat/widgets/token_analysis.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.6.1/.gitignore` & `elia_chat-1.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `elia_chat-1.6.1/README.md` & `elia_chat-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `elia_chat-1.6.1/pyproject.toml` & `elia_chat-1.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [project]
 name = "elia_chat"
-version = "1.6.1"
+version = "1.7.0"
 description = "A powerful terminal user interface for interacting with large language models."
 authors = [
     { name = "Darren Burns", email = "darrenb900@gmail.com" }
 ]
 dependencies = [
-    "textual[syntax]==0.62.0",
+    "textual[syntax]==0.60.0",
     "sqlmodel>=0.0.9",
     "humanize>=4.6.0",
     "click>=8.1.6",
     "xdg-base-dirs>=6.0.1",
     "aiosqlite>=0.20.0",
     "click-default-group>=1.2.4",
-    "litellm==1.35.38",
     "greenlet>=3.0.3",
     "google-generativeai>=0.5.3",
     "pyperclip>=1.8.2",
+    "litellm>=1.37.19",
 ]
 readme = "README.md"
 requires-python = ">= 3.11"
 
 [project.scripts]
 elia = "elia_chat.__main__:cli"
```

### Comparing `elia_chat-1.6.1/PKG-INFO` & `elia_chat-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.3
 Name: elia_chat
-Version: 1.6.1
+Version: 1.7.0
 Summary: A powerful terminal user interface for interacting with large language models.
 Author-email: Darren Burns <darrenb900@gmail.com>
 Requires-Python: >=3.11
 Requires-Dist: aiosqlite>=0.20.0
 Requires-Dist: click-default-group>=1.2.4
 Requires-Dist: click>=8.1.6
 Requires-Dist: google-generativeai>=0.5.3
 Requires-Dist: greenlet>=3.0.3
 Requires-Dist: humanize>=4.6.0
-Requires-Dist: litellm==1.35.38
+Requires-Dist: litellm>=1.37.19
 Requires-Dist: pyperclip>=1.8.2
 Requires-Dist: sqlmodel>=0.0.9
-Requires-Dist: textual[syntax]==0.62.0
+Requires-Dist: textual[syntax]==0.60.0
 Requires-Dist: xdg-base-dirs>=6.0.1
 Description-Content-Type: text/markdown
 
 <h1 align="center">
     <img src="https://github.com/darrenburns/elia/assets/5740731/4037b91a-1ad8-4d5b-884d-b3f1b495acf4" width="126px">
 </h1>
 <p align="center">
```

