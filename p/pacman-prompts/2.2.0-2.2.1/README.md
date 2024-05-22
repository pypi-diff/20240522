# Comparing `tmp/pacman-prompts-2.2.0.tar.gz` & `tmp/pacman_prompts-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pacman-prompts-2.2.0.tar", last modified: Mon Mar 25 18:13:34 2024, max compression
+gzip compressed data, was "pacman_prompts-2.2.1.tar", last modified: Wed May 22 01:38:00 2024, max compression
```

## Comparing `pacman-prompts-2.2.0.tar` & `pacman_prompts-2.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 anishthite   (501) staff       (20)        0 2024-03-25 18:13:34.535856 pacman-prompts-2.2.0/
--rw-r--r--   0 anishthite   (501) staff       (20)      642 2024-03-25 18:13:34.535508 pacman-prompts-2.2.0/PKG-INFO
--rw-r--r--   0 anishthite   (501) staff       (20)     2044 2023-03-27 18:03:15.000000 pacman-prompts-2.2.0/README.md
-drwxr-xr-x   0 anishthite   (501) staff       (20)        0 2024-03-25 18:13:34.533767 pacman-prompts-2.2.0/pacman/
--rw-r--r--   0 anishthite   (501) staff       (20)       56 2023-03-15 16:30:00.000000 pacman-prompts-2.2.0/pacman/__init__.py
--rw-r--r--   0 anishthite   (501) staff       (20)      121 2023-12-14 04:04:03.000000 pacman-prompts-2.2.0/pacman/file_utils.py
--rw-r--r--   0 anishthite   (501) staff       (20)     1592 2024-03-25 18:06:16.000000 pacman-prompts-2.2.0/pacman/pacman.py
--rw-r--r--   0 anishthite   (501) staff       (20)     6921 2024-03-25 18:08:37.000000 pacman-prompts-2.2.0/pacman/prompt.py
-drwxr-xr-x   0 anishthite   (501) staff       (20)        0 2024-03-25 18:13:34.534983 pacman-prompts-2.2.0/pacman_prompts.egg-info/
--rw-r--r--   0 anishthite   (501) staff       (20)      642 2024-03-25 18:13:34.000000 pacman-prompts-2.2.0/pacman_prompts.egg-info/PKG-INFO
--rw-r--r--   0 anishthite   (501) staff       (20)      281 2024-03-25 18:13:34.000000 pacman-prompts-2.2.0/pacman_prompts.egg-info/SOURCES.txt
--rw-r--r--   0 anishthite   (501) staff       (20)        1 2024-03-25 18:13:34.000000 pacman-prompts-2.2.0/pacman_prompts.egg-info/dependency_links.txt
--rw-r--r--   0 anishthite   (501) staff       (20)       22 2024-03-25 18:13:34.000000 pacman-prompts-2.2.0/pacman_prompts.egg-info/requires.txt
--rw-r--r--   0 anishthite   (501) staff       (20)        7 2024-03-25 18:13:34.000000 pacman-prompts-2.2.0/pacman_prompts.egg-info/top_level.txt
--rw-r--r--   0 anishthite   (501) staff       (20)       38 2024-03-25 18:13:34.535930 pacman-prompts-2.2.0/setup.cfg
--rw-r--r--   0 anishthite   (501) staff       (20)      853 2024-03-25 18:12:47.000000 pacman-prompts-2.2.0/setup.py
+drwxr-xr-x   0 anishthite   (501) staff       (20)        0 2024-05-22 01:38:00.557195 pacman_prompts-2.2.1/
+-rw-r--r--   0 anishthite   (501) staff       (20)      662 2024-05-22 01:38:00.556916 pacman_prompts-2.2.1/PKG-INFO
+-rw-r--r--   0 anishthite   (501) staff       (20)     2044 2023-03-27 18:03:15.000000 pacman_prompts-2.2.1/README.md
+drwxr-xr-x   0 anishthite   (501) staff       (20)        0 2024-05-22 01:38:00.554909 pacman_prompts-2.2.1/pacman/
+-rw-r--r--   0 anishthite   (501) staff       (20)       56 2023-03-15 16:30:00.000000 pacman_prompts-2.2.1/pacman/__init__.py
+-rw-r--r--   0 anishthite   (501) staff       (20)      121 2024-04-29 20:40:31.000000 pacman_prompts-2.2.1/pacman/file_utils.py
+-rw-r--r--   0 anishthite   (501) staff       (20)     1777 2024-04-29 20:40:31.000000 pacman_prompts-2.2.1/pacman/pacman.py
+-rw-r--r--   0 anishthite   (501) staff       (20)     7949 2024-05-22 01:14:20.000000 pacman_prompts-2.2.1/pacman/prompt.py
+drwxr-xr-x   0 anishthite   (501) staff       (20)        0 2024-05-22 01:38:00.556603 pacman_prompts-2.2.1/pacman_prompts.egg-info/
+-rw-r--r--   0 anishthite   (501) staff       (20)      662 2024-05-22 01:38:00.000000 pacman_prompts-2.2.1/pacman_prompts.egg-info/PKG-INFO
+-rw-r--r--   0 anishthite   (501) staff       (20)      281 2024-05-22 01:38:00.000000 pacman_prompts-2.2.1/pacman_prompts.egg-info/SOURCES.txt
+-rw-r--r--   0 anishthite   (501) staff       (20)        1 2024-05-22 01:38:00.000000 pacman_prompts-2.2.1/pacman_prompts.egg-info/dependency_links.txt
+-rw-r--r--   0 anishthite   (501) staff       (20)       27 2024-05-22 01:38:00.000000 pacman_prompts-2.2.1/pacman_prompts.egg-info/requires.txt
+-rw-r--r--   0 anishthite   (501) staff       (20)        7 2024-05-22 01:38:00.000000 pacman_prompts-2.2.1/pacman_prompts.egg-info/top_level.txt
+-rw-r--r--   0 anishthite   (501) staff       (20)       38 2024-05-22 01:38:00.557252 pacman_prompts-2.2.1/setup.cfg
+-rw-r--r--   0 anishthite   (501) staff       (20)      867 2024-05-22 00:58:40.000000 pacman_prompts-2.2.1/setup.py
```

### Comparing `pacman-prompts-2.2.0/PKG-INFO` & `pacman_prompts-2.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pacman-prompts
-Version: 2.2.0
+Version: 2.2.1
 Summary: Prompts As Code, man
 Home-page: https://github.com/anishthite/pacman
 Author: Anish Thite
 Author-email: anishthite@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,image recognition
 Classifier: Development Status :: 4 - Beta
@@ -12,7 +12,8 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pyyaml
 Requires-Dist: openai
 Requires-Dist: posthog
+Requires-Dist: groq
```

### Comparing `pacman-prompts-2.2.0/README.md` & `pacman_prompts-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pacman-prompts-2.2.0/pacman/pacman.py` & `pacman_prompts-2.2.1/pacman/pacman.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,47 @@
 # load yml and initialize the prompts
 from .file_utils import load_yml
 from .prompt import Prompt, ChatPrompt, InstuctorPrompt
 import os
 
+
 def load(yaml_path):
     """Load a yaml file and return the prompts"""
     parsed_file = load_yml(yaml_path)
     prompt_collection = {}
-    if 'Prompts' in parsed_file:
-        for name, config in parsed_file['Prompts'].items():
-            prompt_collection[name] = Prompt(config['prompts'], config['provider'], config['config'])
-    if 'ChatPrompts' in parsed_file:
-        for name, config in parsed_file['ChatPrompts'].items():
-            if 'prompts' in config:
-                prompt_collection[name] = ChatPrompt(config['prompts'], config['provider'], config['config'])
+    if "Prompts" in parsed_file:
+        for name, config in parsed_file["Prompts"].items():
+            prompt_collection[name] = Prompt(
+                config["prompts"], config["provider"], config["config"]
+            )
+    if "ChatPrompts" in parsed_file:
+        for name, config in parsed_file["ChatPrompts"].items():
+            if "prompts" in config:
+                prompt_collection[name] = ChatPrompt(
+                    config["prompts"], config["provider"], config["config"]
+                )
             else:
-                prompt_collection[name] = ChatPrompt(config['prompt'], config['provider'], config['config'])
-    if 'InstructorPrompts' in parsed_file:
-        for name, config in parsed_file['InstructorPrompts'].items():
-            if 'prompts' in config:
-                prompt_collection[name] = InstuctorPrompt(config['prompts'], config['provider'], config['config'])
+                prompt_collection[name] = ChatPrompt(
+                    config["prompt"], config["provider"], config["config"]
+                )
+    if "InstructorPrompts" in parsed_file:
+        for name, config in parsed_file["InstructorPrompts"].items():
+            if "prompts" in config:
+                prompt_collection[name] = InstuctorPrompt(
+                    config["prompts"], config["provider"], config["config"]
+                )
             else:
-                prompt_collection[name] = ChatPrompt(config['prompt'], config['provider'], config['config'])
+                prompt_collection[name] = ChatPrompt(
+                    config["prompt"], config["provider"], config["config"]
+                )
 
     return prompt_collection
 
+
 def load_folder(folder_path):
     """Load a folder of yaml files and return the prompts"""
     prompt_collection = {}
     for file in os.listdir(folder_path):
         if file.endswith(".yml"):
             prompts = load(os.path.join(folder_path, file))
             prompt_collection.update(prompts)
-    return prompt_collection
+    return prompt_collection
```

### Comparing `pacman-prompts-2.2.0/pacman/prompt.py` & `pacman_prompts-2.2.1/pacman/prompt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,124 +1,150 @@
 # defines an llm prompt class
 import os
+
 # from dotenv import load_dotenv
 # # Load environment variables from .env file
 # load_dotenv()
 import openai
 import anthropic
 import instructor
+from groq import Groq
+from enum import Enum
 
 
 openai_client = openai.OpenAI(api_key=os.environ["OPENAI_API_KEY"])
 
-anyscale_client =  openai.OpenAI(
-                base_url="https://api.endpoints.anyscale.com/v1",
-                api_key=os.environ["MISTRAL_API_KEY"]
-            )
+anyscale_client = openai.OpenAI(
+    base_url="https://api.endpoints.anyscale.com/v1",
+    api_key=os.environ["MISTRAL_API_KEY"],
+)
 
 anthropic_client = anthropic.Anthropic(
     api_key=os.environ["ANTHROPIC_API_KEY"],
 )
-instructor_client = instructor.patch(openai.OpenAI(api_key=os.environ["OPENAI_API_KEY"]))
 
-# openai.ChatCompletion.create = reliableGPT(openai.ChatCompletion.create,
-#     user_email='claros@claros.so',
-#     #model_limits_dir = {"gpt-3.5-turbo-0613": {"max_token_capacity": 90000, "max_request_capacity": 3500}},
-#     fallback_strategy=['gpt-3.5-turbo-0613', 'gpt-3.5-turbo-0613', 'gpt-3.5-turbo', 'gpt-3.5-turbo-16k'],
-#     caching=False)
+instructor_openai_client = instructor.patch(
+    openai.OpenAI(api_key=os.environ["OPENAI_API_KEY"])
+)
+
+instructor_anthropic_client = instructor.from_anthropic(anthropic_client)
+
+instructor_anyscale_client = instructor.patch(openai.OpenAI(
+        base_url="https://api.endpoints.anyscale.com/v1",
+        api_key=os.environ["MISTRAL_API_KEY"],
+    ), mode=instructor.Mode.JSON_SCHEMA,
+)
+
+groq_client = Groq(
+    api_key=os.environ.get("GROQ_API_KEY"),
+)
+
+
+class Provider(Enum):
+    OPENAI = "openai"
+    ANYSCALE = "anyscale"
+    ANTHROPIC = "anthropic"
+    GROQ = "groq"
+
 
 class PromptConfig:
     def __init__(self, config):
-        #set attributes from config
+        # set attributes from config
         for name, value in config.items():
             setattr(self, name, value)
 
+
 class Prompt:
     def __init__(self, prompts, provider, config):
-
         self.config = PromptConfig(config)
 
         self.provider = provider
 
         if type(prompts) == str:
             self.user_prompt = prompts
             return
 
-        if 'system' not in prompts and 'user' not in prompts:
+        if "system" not in prompts and "user" not in prompts:
             raise Exception("Prompt must have either system prompt or user prompt")
-        if 'system' in prompts:
-            self.system_prompt = prompts['system']
-        if 'user' in prompts:
-            self.user_prompt = prompts['user']
-
+        if "system" in prompts:
+            self.system_prompt = prompts["system"]
+        if "user" in prompts:
+            self.user_prompt = prompts["user"]
 
     def compile(self, inputs):
         print(**inputs)
         return self.prompt.format(**inputs)
 
     def run(self, system_inputs=None, user_inputs=None, **kwargs):
-        #format string
+        # format string
         complete_prompt = self.compile(user_inputs)
-        if  kwargs.get('debug', True):
+        if kwargs.get("debug", True):
             print(complete_prompt)
-        #run in language model
+        # run in language model
         res = openai_client.completions.create(
             prompt=complete_prompt,
-            **self.config.__dict__
-            #stop='\n'
+            **self.config.__dict__,
+            # stop='\n'
         )
         return res
-        #return output
+        # return output
 
     def __call__(self, *args, system_inputs=None, user_inputs=None, **kwargs):
-
         if len(args) == 0:
-            return self.run(system_inputs=system_inputs, user_inputs=user_inputs, **kwargs)
+            return self.run(
+                system_inputs=system_inputs, user_inputs=user_inputs, **kwargs
+            )
 
         if len(args) == 1:
             return self.run(user_inputs=args[0], **kwargs)
 
         raise ValueError("Invalid number of arguments for __call__ method.")
 
+
 def load_prompt(loaded_file):
     prompt = Prompt(**loaded_file)
 
-#make copy of Prompt class but use ChatCompletion in run method
-class ChatPrompt(Prompt):
 
+# make copy of Prompt class but use ChatCompletion in run method
+class ChatPrompt(Prompt):
     def format_messages(self, system_inputs=None, user_inputs=None, **kwargs):
-        if hasattr(self, 'system_prompt'):
+        if hasattr(self, "system_prompt"):
             system_prompt = self.system_prompt.format(**system_inputs)
-        if hasattr(self, 'user_prompt'):
+        if hasattr(self, "user_prompt"):
             user_prompt = self.user_prompt.format(**user_inputs)
 
         initial_message_list = []
-        
-        if hasattr(self, 'system_prompt'):
+
+        if hasattr(self, "system_prompt"):
             initial_message_list.append({"role": "system", "content": system_prompt})
-        if kwargs.get('few_shot', False) and hasattr(self, 'system_prompt') and hasattr(self, 'user_prompt'):
-            initial_message_list.extend(kwargs.get('messages', []))
-        if hasattr(self, 'user_prompt'):
+        if (
+            kwargs.get("few_shot", False)
+            and hasattr(self, "system_prompt")
+            and hasattr(self, "user_prompt")
+        ):
+            initial_message_list.extend(kwargs.get("messages", []))
+        if hasattr(self, "user_prompt"):
             initial_message_list.append({"role": "user", "content": user_prompt})
 
-        if kwargs.get('messages', None) and not kwargs.get('few_shot', False):
-            messages = initial_message_list + kwargs['messages']
+        if kwargs.get("messages", None) and not kwargs.get("few_shot", False):
+            messages = initial_message_list + kwargs["messages"]
         else:
             messages = initial_message_list
-        
+
         return messages
 
     def run(self, system_inputs=None, user_inputs=None, **kwargs):
-        
-        messages = self.format_messages(system_inputs=system_inputs, user_inputs=user_inputs, **kwargs)
+        messages = self.format_messages(
+            system_inputs=system_inputs, user_inputs=user_inputs, **kwargs
+        )
 
-        #TODO: fix the inut s . its flat
-        #TODO: make this all creatable inside the yaml config
-        #TODO: messages is a reserved kwarg, so dont put it in a prompt
-        #run in language model
+        # TODO: fix the inut s . its flat
+        # TODO: make this all creatable inside the yaml config
+        # TODO: messages is a reserved kwarg, so dont put it in a prompt
+        # run in language model
 
         # if self.config['stream'] == True:
         #     try:
         #         resp = ''
         #         for chunk in openai.ChatCompletion.create(
         #             model="gpt-3.5-turbo",
         #             messages=messages,
@@ -130,64 +156,85 @@
         #                 resp += content
         #                 yield f'{content}'
         #     except Exception as e:
         #         print(e)
         #         return str(e)
         # else:
 
-        if kwargs.get('debug', True):
+        if kwargs.get("debug", True):
             print("complete prompt:")
             print(messages)
 
-        if self.provider == "openai":
+        if self.provider == Provider.OPENAI.value:
             res = openai_client.chat.completions.create(
                 messages=messages,
-                **self.config.__dict__
-                #stop='\n'
+                **self.config.__dict__,
+                # stop='\n'
             )
-        elif self.provider == "anyscale":
+        elif self.provider == Provider.ANYSCALE.value:
             res = anyscale_client.chat.completions.create(
-                messages=messages,
-                **self.config.__dict__
+                messages=messages, **self.config.__dict__
             )
-        elif self.provider == "anthropic":
-            if messages and messages[0]['role'] == 'system':
+        elif self.provider == Provider.ANTHROPIC.value:
+            if messages and messages[0]["role"] == "system":
                 msgs = []
                 if len(messages) > 1:
                     msgs = messages[1:]
-                system_content = messages[0]['content']
+                system_content = messages[0]["content"]
                 res = anthropic_client.messages.create(
-                    system=system_content,
-                    messages=msgs
-                    **self.config.__dict__
+                    system=system_content, messages=msgs, **self.config.__dict__
                 )
             else:
                 res = anthropic_client.messages.create(
-                    messages=messages,
-                    **self.config.__dict__
+                    messages=messages, **self.config.__dict__
                 )
+        elif self.provider == Provider.GROQ.value:
+            res = groq_client.chat.completions.create(
+                messages=messages,
+                **self.config.__dict__,
+                # stop='\n'
+            )
         return res
 
+
 class InstuctorPrompt(ChatPrompt):
     def run(self, system_inputs=None, user_inputs=None, response_model=None, **kwargs):
-        messages = self.format_messages(system_inputs=system_inputs, user_inputs=user_inputs, **kwargs)
+        messages = self.format_messages(
+            system_inputs=system_inputs, user_inputs=user_inputs, **kwargs
+        )
 
-        if kwargs.get('debug', True):
+        if kwargs.get("debug", True):
             print("complete prompt:")
             print(messages)
 
-        res = instructor_client.chat.completions.create(
-            messages=messages,
-            response_model=response_model,
-            **self.config.__dict__
-        )
+        if self.provider == Provider.OPENAI.value:
+            res = instructor_openai_client.chat.completions.create(
+                messages=messages, response_model=response_model, **self.config.__dict__
+            )
+
+        if self.provider == Provider.ANTHROPIC.value:
+            res = instructor_anthropic_client.messages.create(
+                messages=messages, response_model=response_model, **self.config.__dict__
+            )
+        
+        if self.provider == Provider.ANYSCALE.value:
+            res = instructor_anyscale_client.chat.completions.create(
+                messages=messages, response_model=response_model, **self.config.__dict__
+            )
+
         return res
-    
-    def __call__(self, *args, system_inputs=None, user_inputs=None, response_model=None, **kwargs):
 
+    def __call__(
+        self, *args, system_inputs=None, user_inputs=None, response_model=None, **kwargs
+    ):
         if len(args) == 0:
-            return self.run(system_inputs=system_inputs, user_inputs=user_inputs, response_model=response_model, **kwargs)
+            return self.run(
+                system_inputs=system_inputs,
+                user_inputs=user_inputs,
+                response_model=response_model,
+                **kwargs,
+            )
 
         if len(args) == 1:
             return self.run(user_inputs=args[0], **kwargs)
 
         raise ValueError("Invalid number of arguments for __call__ method.")
```

### Comparing `pacman-prompts-2.2.0/pacman_prompts.egg-info/PKG-INFO` & `pacman_prompts-2.2.1/pacman_prompts.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pacman-prompts
-Version: 2.2.0
+Version: 2.2.1
 Summary: Prompts As Code, man
 Home-page: https://github.com/anishthite/pacman
 Author: Anish Thite
 Author-email: anishthite@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,image recognition
 Classifier: Development Status :: 4 - Beta
@@ -12,7 +12,8 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pyyaml
 Requires-Dist: openai
 Requires-Dist: posthog
+Requires-Dist: groq
```

### Comparing `pacman-prompts-2.2.0/setup.py` & `pacman_prompts-2.2.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'pacman-prompts',
   packages = find_packages(exclude=['examples']),
-  version = '2.2.0',
+  version = '2.2.1',
   license='MIT',
   description = 'Prompts As Code, man',
   long_description_content_type = 'text/markdown',
   author = 'Anish Thite',
   author_email = 'anishthite@gmail.com',
   url = 'https://github.com/anishthite/pacman',
   keywords = [
     'artificial intelligence',
     'attention mechanism',
     'image recognition'
   ],
   install_requires=[
       'pyyaml',
       'openai',
-      'posthog'
+      'posthog',
+      'groq'
   ],
   setup_requires=[
   ],
   tests_require=[
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
```

