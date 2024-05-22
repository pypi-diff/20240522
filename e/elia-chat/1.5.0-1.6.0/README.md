# Comparing `tmp/elia_chat-1.5.0.tar.gz` & `tmp/elia_chat-1.6.0.tar.gz`

## Comparing `elia_chat-1.5.0.tar` & `elia_chat-1.6.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 elia_chat-1.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 elia_chat-1.5.0/.python-version
--rw-r--r--   0        0        0     5048 2020-02-02 00:00:00.000000 elia_chat-1.5.0/requirements-dev.lock
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 elia_chat-1.5.0/requirements.lock
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 elia_chat-1.5.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/__init__.py
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/__main__.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/app.py
--rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/chats_manager.py
--rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/config.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/constants.py
--rw-r--r--   0        0        0     8984 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/elia.scss
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/launch_args.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/locations.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/models.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/runtime_config.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/time_display.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/database/__init__.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/database/converters.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/database/database.py
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/database/import_chatgpt.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/database/models.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/screens/chat_details.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/screens/chat_screen.py
--rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/screens/help_screen.py
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/screens/home_screen.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/widgets/agent_is_typing.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/widgets/app_header.py
--rw-r--r--   0        0        0    11022 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/widgets/chat.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/widgets/chat_header.py
--rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/widgets/chat_list.py
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/widgets/chat_options.py
--rw-r--r--   0        0        0    10814 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/widgets/chatbox.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/widgets/prompt_input.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 elia_chat-1.5.0/elia_chat/widgets/token_analysis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.5.0/tests/__init__.py
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 elia_chat-1.5.0/.gitignore
--rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 elia_chat-1.5.0/README.md
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 elia_chat-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 elia_chat-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 elia_chat-1.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 elia_chat-1.6.0/.python-version
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 elia_chat-1.6.0/requirements-dev.lock
+-rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 elia_chat-1.6.0/requirements.lock
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 elia_chat-1.6.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/__init__.py
+-rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/__main__.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/app.py
+-rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/chats_manager.py
+-rw-r--r--   0        0        0     6338 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/config.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/constants.py
+-rw-r--r--   0        0        0     9138 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/elia.scss
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/launch_args.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/locations.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/models.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/runtime_config.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/time_display.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/database/__init__.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/database/converters.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/database/database.py
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/database/import_chatgpt.py
+-rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/database/models.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/screens/chat_details.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/screens/chat_screen.py
+-rw-r--r--   0        0        0     5936 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/screens/help_screen.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/screens/home_screen.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/widgets/agent_is_typing.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/widgets/app_header.py
+-rw-r--r--   0        0        0    11022 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/widgets/chat.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/widgets/chat_header.py
+-rw-r--r--   0        0        0     5677 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/widgets/chat_list.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/widgets/chat_options.py
+-rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/widgets/chatbox.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/widgets/prompt_input.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 elia_chat-1.6.0/elia_chat/widgets/token_analysis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 elia_chat-1.6.0/.gitignore
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 elia_chat-1.6.0/README.md
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 elia_chat-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 elia_chat-1.6.0/PKG-INFO
```

### Comparing `elia_chat-1.5.0/.pre-commit-config.yaml` & `elia_chat-1.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `elia_chat-1.5.0/requirements-dev.lock` & `elia_chat-1.6.0/requirements-dev.lock`

 * *Files 3% similar despite different names*

```diff
@@ -72,15 +72,14 @@
 google-generativeai==0.5.3
     # via elia-chat
 googleapis-common-protos==1.63.0
     # via google-api-core
     # via grpcio-status
 greenlet==3.0.3
     # via elia-chat
-    # via sqlalchemy
 grpcio==1.63.0
     # via google-api-core
     # via grpcio-status
 grpcio-status==1.62.2
     # via google-api-core
 h11==0.14.0
     # via httpcore
@@ -156,28 +155,26 @@
     # via pyasn1-modules
     # via rsa
 pyasn1-modules==0.4.0
     # via google-auth
 pydantic==2.6.1
     # via google-generativeai
     # via openai
-    # via pydantic-settings
     # via sqlmodel
 pydantic-core==2.16.2
     # via pydantic
-pydantic-settings==2.2.1
-    # via elia-chat
 pygments==2.17.2
     # via rich
 pyinstrument==4.6.2
 pyparsing==3.1.2
     # via httplib2
+pyperclip==1.8.2
+    # via elia-chat
 python-dotenv==1.0.1
     # via litellm
-    # via pydantic-settings
 pyyaml==6.0.1
     # via huggingface-hub
     # via pre-commit
 regex==2023.12.25
     # via tiktoken
 requests==2.31.0
     # via google-api-core
@@ -194,15 +191,15 @@
     # via anyio
     # via httpx
     # via openai
 sqlalchemy==2.0.25
     # via sqlmodel
 sqlmodel==0.0.14
     # via elia-chat
-textual==0.58.1
+textual==0.62.0
     # via elia-chat
     # via textual-dev
 textual-dev==1.4.0
 tiktoken==0.5.2
     # via litellm
 tokenizers==0.19.1
     # via litellm
```

### Comparing `elia_chat-1.5.0/requirements.lock` & `elia_chat-1.6.0/requirements.lock`

 * *Files 6% similar despite different names*

```diff
@@ -63,15 +63,14 @@
 google-generativeai==0.5.3
     # via elia-chat
 googleapis-common-protos==1.63.0
     # via google-api-core
     # via grpcio-status
 greenlet==3.0.3
     # via elia-chat
-    # via sqlalchemy
 grpcio==1.63.0
     # via google-api-core
     # via grpcio-status
 grpcio-status==1.62.2
     # via google-api-core
 h11==0.14.0
     # via httpcore
@@ -130,27 +129,25 @@
     # via pyasn1-modules
     # via rsa
 pyasn1-modules==0.4.0
     # via google-auth
 pydantic==2.6.1
     # via google-generativeai
     # via openai
-    # via pydantic-settings
     # via sqlmodel
 pydantic-core==2.16.2
     # via pydantic
-pydantic-settings==2.2.1
-    # via elia-chat
 pygments==2.17.2
     # via rich
 pyparsing==3.1.2
     # via httplib2
+pyperclip==1.8.2
+    # via elia-chat
 python-dotenv==1.0.1
     # via litellm
-    # via pydantic-settings
 pyyaml==6.0.1
     # via huggingface-hub
 regex==2023.12.25
     # via tiktoken
 requests==2.31.0
     # via google-api-core
     # via huggingface-hub
@@ -164,15 +161,15 @@
     # via anyio
     # via httpx
     # via openai
 sqlalchemy==2.0.25
     # via sqlmodel
 sqlmodel==0.0.14
     # via elia-chat
-textual==0.58.1
+textual==0.62.0
     # via elia-chat
 tiktoken==0.5.2
     # via litellm
 tokenizers==0.19.1
     # via litellm
 tqdm==4.66.2
     # via google-generativeai
```

### Comparing `elia_chat-1.5.0/elia_chat/__main__.py` & `elia_chat-1.6.0/elia_chat/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,26 +2,25 @@
 Elia CLI
 """
 
 import asyncio
 import pathlib
 from textwrap import dedent
 import tomllib
-from typing import Any, Tuple
+from typing import Any
 
 import click
 from click_default_group import DefaultGroup
 
 from rich.console import Console
 
 from elia_chat.app import Elia
 from elia_chat.config import LaunchConfig
 from elia_chat.database.import_chatgpt import import_chatgpt_data
 from elia_chat.database.database import create_database, sqlite_file_name
-from elia_chat.launch_args import QuickLaunchArgs
 from elia_chat.locations import config_file
 
 console = Console()
 
 
 def create_db_if_not_exists() -> None:
     if not sqlite_file_name.exists():
@@ -47,21 +46,40 @@
 @click.group(cls=DefaultGroup, default="default", default_if_no_args=True)
 def cli() -> None:
     """Interact with large language models using your terminal."""
 
 
 @cli.command()
 @click.argument("prompt", nargs=-1, type=str, required=False)
-def default(prompt: tuple[str, ...]):
+@click.option(
+    "-m",
+    "--model",
+    type=str,
+    default="",
+    help="The model to use for the chat",
+)
+@click.option(
+    "-i",
+    "--inline",
+    is_flag=True,
+    help="Run in inline mode, without launching full TUI.",
+    default=False,
+)
+def default(prompt: tuple[str, ...], model: str, inline: bool):
     prompt = prompt or ("",)
     joined_prompt = " ".join(prompt)
     create_db_if_not_exists()
     file_config = load_or_create_config_file()
-    app = Elia(LaunchConfig(**file_config), startup_prompt=joined_prompt)
-    app.run()
+    cli_config = {}
+    if model:
+        cli_config["default_model"] = model
+
+    launch_config: dict[str, Any] = {**file_config, **cli_config}
+    app = Elia(LaunchConfig(**launch_config), startup_prompt=joined_prompt)
+    app.run(inline=inline)
 
 
 @cli.command()
 def reset() -> None:
     """
     Reset the database
 
@@ -106,33 +124,9 @@
     This command will import the ChatGPT conversations from a local
     JSON file into the database.
     """
     asyncio.run(import_chatgpt_data(file=file))
     console.print(f"[green]ChatGPT data imported from {str(file)!r}")
 
 
-@cli.command()
-@click.argument("message", nargs=-1, type=str, required=True)
-@click.option(
-    "-m",
-    "--model",
-    type=str,
-    default="gpt-3.5-turbo",
-    help="The model to use for the chat",
-)
-def chat(message: Tuple[str, ...], model: str) -> None:
-    """
-    Start Elia with a chat message
-    """
-    quick_launch_args = QuickLaunchArgs(
-        launch_prompt=" ".join(message),
-        launch_prompt_model_name=model,
-    )
-    launch_config = LaunchConfig(
-        default_model=quick_launch_args.launch_prompt_model_name,
-    )
-    app = Elia(launch_config, quick_launch_args.launch_prompt)
-    app.run()
-
-
 if __name__ == "__main__":
     cli()
```

### Comparing `elia_chat-1.5.0/elia_chat/app.py` & `elia_chat-1.6.0/elia_chat/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 class Elia(App[None]):
     ENABLE_COMMAND_PALETTE = False
     CSS_PATH = Path(__file__).parent / "elia.scss"
     BINDINGS = [
         Binding("q", "app.quit", "Quit", show=False),
-        Binding("?", "help", "Help"),
+        Binding("f1,?", "help", "Help"),
     ]
 
     def __init__(self, config: LaunchConfig, startup_prompt: str = ""):
         super().__init__()
         self.launch_config = config
         launch_config.set(config)
         self._runtime_config = RuntimeConfig(
```

### Comparing `elia_chat-1.5.0/elia_chat/chats_manager.py` & `elia_chat-1.6.0/elia_chat/chats_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 import datetime
 
+from sqlmodel import select
 from textual import log
 
 from elia_chat.database.converters import (
     chat_dao_to_chat_data,
     chat_message_to_message_dao,
     message_dao_to_chat_message,
 )
@@ -84,14 +85,23 @@
                 (await chat.awaitable_attrs.messages).append(new_message)
 
             await session.commit()
 
         return chat.id
 
     @staticmethod
+    async def archive_chat(chat_id: int) -> None:
+        async with get_session() as session:
+            statement = select(ChatDao).where(ChatDao.id == chat_id)
+            result = await session.exec(statement)
+            chat_dao = result.one()
+            chat_dao.archived = True
+            await session.commit()
+
+    @staticmethod
     async def add_message_to_chat(chat_id: int, message: ChatMessage) -> None:
         async with get_session() as session:
             chat: ChatDao | None = await session.get(ChatDao, chat_id)
             if not chat:
                 raise Exception(f"Chat with ID {chat_id} not found.")
             message_dao = chat_message_to_message_dao(message, chat_id)
             (await chat.awaitable_attrs.messages).append(message_dao)
```

### Comparing `elia_chat-1.5.0/elia_chat/config.py` & `elia_chat-1.6.0/elia_chat/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             display_name="GPT-3.5 Turbo",
             provider="OpenAI",
             product="ChatGPT",
             description="Fast & inexpensive model for simple tasks.",
         ),
         EliaChatModel(
             id="elia-gpt-4o",
-            name="openai/gpt-4o",
+            name="gpt-4o",
             display_name="GPT-4o",
             provider="OpenAI",
             product="ChatGPT",
             description="Fastest and most affordable flagship model.",
         ),
         EliaChatModel(
             id="elia-gpt-4-turbo",
@@ -142,21 +142,23 @@
     """The config of the application at launch.
 
     Values may be sourced via command line options, env vars, config files.
     """
 
     model_config = ConfigDict(frozen=True)
 
-    default_model: str = Field(default="elia-gpt-3.5-turbo")
+    default_model: str = Field(default="elia-gpt-4o")
     """The ID or name of the default model."""
     system_prompt: str = Field(
         default=os.getenv(
             "ELIA_SYSTEM_PROMPT", "You are a helpful assistant named Elia."
         )
     )
+    message_code_theme: str = Field(default="monokai")
+    """The default Pygments syntax highlighting theme to be used in chatboxes."""
     models: list[EliaChatModel] = Field(default_factory=list)
     builtin_models: list[EliaChatModel] = Field(
         default_factory=get_builtin_models, init=False
     )
 
     @property
     def all_models(self) -> list[EliaChatModel]:
```

### Comparing `elia_chat-1.5.0/elia_chat/elia.scss` & `elia_chat-1.6.0/elia_chat/elia.scss`

 * *Files 6% similar despite different names*

```diff
@@ -26,20 +26,27 @@
   color: $main-lighten-2 50%;
   background: $main 75%;
 }
 
 Screen {
   background: $background;
   padding: 0 2 1 2;
+  &:inline {
+    height: 80vh;
+    padding: 0 2;
+  }
 }
 
 ModalScreen {
   background: black 50%;
   padding: 0;
-
+  &:inline {
+    padding: 0;
+    border: none;
+  }
   & Footer {
     margin: 0 2 1 2;
   }
 }
 
 Rule {
   color: white 20%;
@@ -71,14 +78,17 @@
 
 Chat {
   ChatHeader {
     width: 100%;
     height: auto;
     padding: 1 2;
     background: $background;
+    &:inline {
+      padding: 0 2 1 2;
+    }
 
     & #model-static {
       color: $text-muted;
     }
   }
   PromptInput {
     height: auto;
@@ -159,14 +169,19 @@
 }
 
 AppHeader {
   dock: top;
   width: 1fr;
   padding: 1 2;
   height: auto;
+
+  &:inline {
+    padding: 0 2 1 2;
+  }
+
   & .app-title {
     color: $text-muted;
   }
 
   & .app-subtitle {
     color: greenyellow 50%;
     text-style: bold;
@@ -376,18 +391,14 @@
   width: auto;
 }
 
 Tabs:focus .underline--bar {
   color: $text 35%;
 }
 
-TokenAnalysis {
-  height: auto;
-}
-
 MessageInfo #inner-container ContentSwitcher {
   height: auto;
   padding: 1 2;
 }
 
 MessageInfo #inner-container #markdown-content {
   height: 1fr;
```

### Comparing `elia_chat-1.5.0/elia_chat/locations.py` & `elia_chat-1.6.0/elia_chat/locations.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.5.0/elia_chat/models.py` & `elia_chat-1.6.0/elia_chat/models.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.5.0/elia_chat/time_display.py` & `elia_chat-1.6.0/elia_chat/time_display.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.5.0/elia_chat/database/converters.py` & `elia_chat-1.6.0/elia_chat/database/converters.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.5.0/elia_chat/database/database.py` & `elia_chat-1.6.0/elia_chat/database/database.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.5.0/elia_chat/database/import_chatgpt.py` & `elia_chat-1.6.0/elia_chat/database/import_chatgpt.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.5.0/elia_chat/database/models.py` & `elia_chat-1.6.0/elia_chat/database/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,14 +71,15 @@
                 .group_by(MessageDao.chat_id)
                 .alias("subquery")
             )
 
             statement = (
                 select(ChatDao)
                 .join(subquery, subquery.c.chat_id == ChatDao.id)
+                .where(ChatDao.archived == False)
                 .order_by(desc(subquery.c.max_timestamp))
                 .options(selectinload(ChatDao.messages))
             )
             results = await session.exec(statement)
             return list(results)
 
     @staticmethod
```

### Comparing `elia_chat-1.5.0/elia_chat/screens/chat_details.py` & `elia_chat-1.6.0/elia_chat/screens/chat_details.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.5.0/elia_chat/screens/chat_screen.py` & `elia_chat-1.6.0/elia_chat/screens/chat_screen.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 class ChatScreen(Screen[None]):
     AUTO_FOCUS = "ChatPromptInput"
     BINDINGS = [
         Binding(
             key="escape",
-            action="focus('prompt')",
+            action="app.focus('prompt')",
             description="Focus prompt",
             key_display="esc",
         ),
     ]
 
     def __init__(
         self,
```

### Comparing `elia_chat-1.5.0/elia_chat/screens/help_screen.py` & `elia_chat-1.6.0/elia_chat/screens/help_screen.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from textual.screen import ModalScreen
 from textual.widgets import Footer, Markdown
 
 
 class HelpScreen(ModalScreen[None]):
     BINDINGS = [
         Binding("q", "app.quit", "Quit", show=False),
-        Binding("escape,?", "app.pop_screen()", "Close help", key_display="esc"),
+        Binding("escape,f1,?", "app.pop_screen()", "Close help", key_display="esc"),
     ]
 
     HELP_MARKDOWN = """\
 ### How do I quit Elia?
 
 Press `Ctrl+C` on your keyboard.
 `q` also works if an input isn't currently focused.
```

### Comparing `elia_chat-1.5.0/elia_chat/screens/home_screen.py` & `elia_chat-1.6.0/elia_chat/screens/home_screen.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.5.0/elia_chat/widgets/app_header.py` & `elia_chat-1.6.0/elia_chat/widgets/app_header.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.5.0/elia_chat/widgets/chat.py` & `elia_chat-1.6.0/elia_chat/widgets/chat.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -82,21 +82,21 @@
         last_message: ChatMessage
 
     @dataclass
     class FirstMessageSent(Message):
         chat_data: ChatData
 
     def compose(self) -> ComposeResult:
+        yield AgentIsTyping()
         yield ChatHeader(chat=self.chat_data, model=self.model)
 
         with VerticalScroll(id="chat-container") as vertical_scroll:
             vertical_scroll.can_focus = False
 
         yield ChatPromptInput(id="prompt")
-        yield AgentIsTyping()
 
     async def on_mount(self, _: events.Mount) -> None:
         """
         When the component is mounted, we need to check if there is a new chat to start
         """
         await self.load_chat(self.chat_data)
```

### Comparing `elia_chat-1.5.0/elia_chat/widgets/chat_header.py` & `elia_chat-1.6.0/elia_chat/widgets/chat_header.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.5.0/elia_chat/widgets/chat_list.py` & `elia_chat-1.6.0/elia_chat/widgets/chat_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import datetime
 from dataclasses import dataclass
+from typing import cast
 
 import humanize
 from rich.console import RenderResult, Console, ConsoleOptions
 from rich.markup import escape
 from rich.padding import Padding
 from rich.text import Text
 from textual import events, log, on
@@ -53,16 +54,17 @@
         self.chat = chat
         self.config = config
 
 
 class ChatList(OptionList):
     BINDINGS = [
         Binding(
-            "escape", "screen.focus('home-prompt')", "Focus prompt", key_display="esc"
+            "escape", "app.focus('home-prompt')", "Focus prompt", key_display="esc"
         ),
+        Binding("a", "archive_chat", "Archive chat", key_display="a"),
         Binding("j,down", "cursor_down", "Down", show=False),
         Binding("k,up", "cursor_up", "Up", show=False),
         Binding("l,right,enter", "select", "Select", show=False),
         Binding("g,home", "first", "First", show=False),
         Binding("G,end", "last", "Last", show=False),
         Binding("pagedown", "page_down", "Page Down", show=False),
         Binding("pageup", "page_up", "Page Up", show=False),
@@ -106,28 +108,46 @@
         Args:
             new_highlighted: The index to highlight after refresh.
         """
         self.options = await self.load_chat_list_items()
         old_highlighted = self.highlighted
         self.clear_options()
         self.add_options(self.options)
-        self.border_title = f"History ({len(self.options)})"
+        self.border_title = self.get_border_title()
         if new_highlighted > -1:
             self.highlighted = new_highlighted
         else:
             self.highlighted = old_highlighted
 
     async def load_chat_list_items(self) -> list[ChatListItem]:
         chats = await self.load_chats()
         return [ChatListItem(chat, self.app.launch_config) for chat in chats]
 
     async def load_chats(self) -> list[ChatData]:
         all_chats = await ChatsManager.all_chats()
         return all_chats
 
+    async def action_archive_chat(self) -> None:
+        if self.highlighted is None:
+            return
+
+        item = cast(ChatListItem, self.get_option_at_index(self.highlighted))
+        self.options.pop(self.highlighted)
+        self.remove_option_at_index(self.highlighted)
+
+        chat_id = item.chat.id
+        await ChatsManager.archive_chat(chat_id)
+
+        self.border_title = self.get_border_title()
+        self.refresh()
+        self.app.notify(f"Chat [b]{chat_id!r}[/] archived")
+
+    def get_border_title(self) -> str:
+        return f"History ({len(self.options)})"
+
     def create_chat(self, chat_data: ChatData) -> None:
         new_chat_list_item = ChatListItem(chat_data, self.app.launch_config)
         log.debug(f"Creating new chat {new_chat_list_item!r}")
 
         option_list = self.query_one(OptionList)
         self.options = [
             new_chat_list_item,
```

### Comparing `elia_chat-1.5.0/elia_chat/widgets/chat_options.py` & `elia_chat-1.6.0/elia_chat/widgets/chat_options.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.5.0/elia_chat/widgets/chatbox.py` & `elia_chat-1.6.0/elia_chat/widgets/chatbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from textual.widget import Widget
 from textual.widgets import TextArea
 from textual.widgets.text_area import Selection
 from textual.document._syntax_aware_document import SyntaxAwareDocumentError
 
 from elia_chat.config import EliaChatModel
 from elia_chat.models import ChatMessage
+from elia_chat.config import launch_config
 
 
 class SelectionTextArea(TextArea):
     class LeaveSelectionMode(Message):
         """Broadcast that the user wants to leave selection mode."""
 
     @dataclass
@@ -93,15 +94,17 @@
             message = f"Copied {len(text_to_copy)} selected characters to clipboard."
             self.notify(message, title="Selection copied")
         else:
             text_to_copy = self.text
             message = f"Copied message ({len(text_to_copy)} characters)."
             self.notify(message, title="Message copied")
 
-        self.app.copy_to_clipboard(text_to_copy)
+        import pyperclip
+
+        pyperclip.copy(text_to_copy)
         self.visual_mode = False
 
     def action_next_code_block(self) -> None:
         try:
             query = self.document.prepare_query(
                 "(fenced_code_block (code_fence_content) @code_block)"
             )
@@ -199,15 +202,17 @@
         self.selection_mode = not self.selection_mode
         self.set_class(self.selection_mode, "selecting")
 
     def action_copy_to_clipboard(self) -> None:
         if not self.selection_mode:
             text_to_copy = self.message.message.get("content")
             if isinstance(text_to_copy, str):
-                self.app.copy_to_clipboard(text_to_copy)
+                import pyperclip
+
+                pyperclip.copy(text_to_copy)
                 message = f"Copied message ({len(text_to_copy)} characters)."
                 self.notify(message, title="Message copied")
             else:
                 message = "Unable to copy message"
                 self.notify(message, title="Clipboard error", severity="error")
 
     async def watch_selection_mode(self, value: bool) -> None:
@@ -256,15 +261,17 @@
 
     @property
     def markdown(self) -> Markdown:
         """Return the content as a Rich Markdown object."""
         content = self.message.message.get("content")
         if not isinstance(content, str):
             content = ""
-        return Markdown(content)
+
+        config = launch_config.get()
+        return Markdown(content, code_theme=config.message_code_theme)
 
     def render(self) -> RenderableType:
         if self.selection_mode:
             # When in selection mode, this widget has a SelectionTextArea child,
             # so we do not need to render anything.
             return ""
```

### Comparing `elia_chat-1.5.0/elia_chat/widgets/prompt_input.py` & `elia_chat-1.6.0/elia_chat/widgets/prompt_input.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.5.0/elia_chat/widgets/token_analysis.py` & `elia_chat-1.6.0/elia_chat/widgets/token_analysis.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.5.0/.gitignore` & `elia_chat-1.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `elia_chat-1.5.0/README.md` & `elia_chat-1.6.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -28,18 +28,30 @@
 
 Launch Elia from the command line:
 
 ```bash
 elia
 ```
 
-Launch directly a new chat from the command line:
+Launch a new chat inline (under your prompt) with `-i`/`--inline`:
 
 ```bash
-elia "What is the Zen of Python?"
+elia -i "What is the Zen of Python?"
+```
+
+Launch a new chat in full-screen mode:
+
+```bash
+elia "Tell me a cool fact about lizards!"
+```
+
+Specify a model via the command line using `-m`/`--model`:
+
+```bash
+elia -m gpt-4o
 ```
 
 ## Running local models
 
 1. Install [`ollama`](https://github.com/ollama/ollama).
 2. Pull the model you require, e.g. `ollama pull llama3`.
 3. Run the local ollama server: `ollama serve`.
@@ -49,20 +61,22 @@
 
 The location of the configuration file is noted at the bottom of
 the options window (`ctrl+o`).
 
 The example file below shows the available options, as well as examples of how to add new models.
 
 ```toml
-# the *ID* for the model that is selected by default on launch
-# to use one of the default builtin OpenAI/anthropic models, prefix
-# the model name with `elia-`.
-default_model = "elia-gpt-3.5-turbo"
+# the ID or name of the model that is selected by default on launch
+default_model = "gpt-4o"
 # the system prompt on launch
 system_prompt = "You are a helpful assistant who talks like a pirate."
+# change the syntax highlighting theme of code in messages
+# choose from https://pygments.org/styles/
+# defaults to "monokai"
+message_code_theme = "dracula"
 
 # example of adding local llama3 support
 # only the `name` field is required here.
 [[models]]
 name = "ollama/llama3"
 
 # example of a model running on a local server, e.g. LocalAI
```

### Comparing `elia_chat-1.5.0/pyproject.toml` & `elia_chat-1.6.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [project]
 name = "elia_chat"
-version = "1.5.0"
+version = "1.6.0"
 description = "A powerful terminal user interface for interacting with large language models."
 authors = [
     { name = "Darren Burns", email = "darrenb900@gmail.com" }
 ]
 dependencies = [
-    "textual[syntax]==0.58.1",
+    "textual[syntax]==0.62.0",
     "sqlmodel>=0.0.9",
     "humanize>=4.6.0",
     "click>=8.1.6",
     "xdg-base-dirs>=6.0.1",
-    "pydantic-settings>=2.2.1",
     "aiosqlite>=0.20.0",
     "click-default-group>=1.2.4",
-    "litellm>=1.35.38",
+    "litellm==1.35.38",
     "greenlet>=3.0.3",
     "google-generativeai>=0.5.3",
+    "pyperclip>=1.8.2",
 ]
 readme = "README.md"
 requires-python = ">= 3.11"
 
 [project.scripts]
 elia = "elia_chat.__main__:cli"
```

### Comparing `elia_chat-1.5.0/PKG-INFO` & `elia_chat-1.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.3
 Name: elia_chat
-Version: 1.5.0
+Version: 1.6.0
 Summary: A powerful terminal user interface for interacting with large language models.
 Author-email: Darren Burns <darrenb900@gmail.com>
 Requires-Python: >=3.11
 Requires-Dist: aiosqlite>=0.20.0
 Requires-Dist: click-default-group>=1.2.4
 Requires-Dist: click>=8.1.6
 Requires-Dist: google-generativeai>=0.5.3
 Requires-Dist: greenlet>=3.0.3
 Requires-Dist: humanize>=4.6.0
-Requires-Dist: litellm>=1.35.38
-Requires-Dist: pydantic-settings>=2.2.1
+Requires-Dist: litellm==1.35.38
+Requires-Dist: pyperclip>=1.8.2
 Requires-Dist: sqlmodel>=0.0.9
-Requires-Dist: textual[syntax]==0.58.1
+Requires-Dist: textual[syntax]==0.62.0
 Requires-Dist: xdg-base-dirs>=6.0.1
 Description-Content-Type: text/markdown
 
 <h1 align="center">
     <img src="https://github.com/darrenburns/elia/assets/5740731/4037b91a-1ad8-4d5b-884d-b3f1b495acf4" width="126px">
 </h1>
 <p align="center">
@@ -47,18 +47,30 @@
 
 Launch Elia from the command line:
 
 ```bash
 elia
 ```
 
-Launch directly a new chat from the command line:
+Launch a new chat inline (under your prompt) with `-i`/`--inline`:
 
 ```bash
-elia "What is the Zen of Python?"
+elia -i "What is the Zen of Python?"
+```
+
+Launch a new chat in full-screen mode:
+
+```bash
+elia "Tell me a cool fact about lizards!"
+```
+
+Specify a model via the command line using `-m`/`--model`:
+
+```bash
+elia -m gpt-4o
 ```
 
 ## Running local models
 
 1. Install [`ollama`](https://github.com/ollama/ollama).
 2. Pull the model you require, e.g. `ollama pull llama3`.
 3. Run the local ollama server: `ollama serve`.
@@ -68,20 +80,22 @@
 
 The location of the configuration file is noted at the bottom of
 the options window (`ctrl+o`).
 
 The example file below shows the available options, as well as examples of how to add new models.
 
 ```toml
-# the *ID* for the model that is selected by default on launch
-# to use one of the default builtin OpenAI/anthropic models, prefix
-# the model name with `elia-`.
-default_model = "elia-gpt-3.5-turbo"
+# the ID or name of the model that is selected by default on launch
+default_model = "gpt-4o"
 # the system prompt on launch
 system_prompt = "You are a helpful assistant who talks like a pirate."
+# change the syntax highlighting theme of code in messages
+# choose from https://pygments.org/styles/
+# defaults to "monokai"
+message_code_theme = "dracula"
 
 # example of adding local llama3 support
 # only the `name` field is required here.
 [[models]]
 name = "ollama/llama3"
 
 # example of a model running on a local server, e.g. LocalAI
```

