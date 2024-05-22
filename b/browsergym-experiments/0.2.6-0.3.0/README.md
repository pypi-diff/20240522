# Comparing `tmp/browsergym_experiments-0.2.6.tar.gz` & `tmp/browsergym_experiments-0.3.0.tar.gz`

## Comparing `browsergym_experiments-0.2.6.tar` & `browsergym_experiments-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 browsergym_experiments-0.2.6/requirements.txt
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 browsergym_experiments-0.2.6/src/browsergym/experiments/__init__.py
--rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 browsergym_experiments-0.2.6/src/browsergym/experiments/agent.py
--rw-r--r--   0        0        0    21085 2020-02-02 00:00:00.000000 browsergym_experiments-0.2.6/src/browsergym/experiments/loop.py
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 browsergym_experiments-0.2.6/src/browsergym/experiments/utils.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 browsergym_experiments-0.2.6/tests/test_exp_loop.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 browsergym_experiments-0.2.6/.gitignore
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 browsergym_experiments-0.2.6/README.md
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 browsergym_experiments-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 browsergym_experiments-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.0/requirements.txt
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.0/src/browsergym/experiments/__init__.py
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.0/src/browsergym/experiments/agent.py
+-rw-r--r--   0        0        0    21090 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.0/src/browsergym/experiments/loop.py
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.0/src/browsergym/experiments/utils.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.0/tests/test_exp_loop.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.0/.gitignore
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.0/README.md
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.0/PKG-INFO
```

### Comparing `browsergym_experiments-0.2.6/src/browsergym/experiments/loop.py` & `browsergym_experiments-0.3.0/src/browsergym/experiments/loop.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     def run(self):
         """Run the experiment and save the results"""
 
         episode_info = []
         try:
             logging.info(f"Running experiment {self.exp_name} in:\n  {self.exp_dir}")
             agent = self.agent_args.make_agent()
-            env = self.env_args.make_env(action_mapping=agent.action_mapping)
+            env = self.env_args.make_env(action_mapping=agent.action_set.to_python_code)
 
             err_msg, stack_trace = None, None
             step_info = StepInfo(step=0)
             episode_info = [step_info]
             step_info.from_reset(env, seed=self.env_args.task_seed)
 
             while not step_info.is_done:  # set a limit
@@ -253,16 +253,16 @@
 
         t.action_exec_start = env_info["action_exec_start"]  # start
         t.action_exect_after_timeout = env_info["action_exec_stop"]
         t.action_exec_stop = env_info["action_exec_stop"] - env_info["action_exec_timeout"]
 
     def from_action(self, agent: Agent):
         self.profiling.agent_start = time.time()
-        if agent.observation_mapping:
-            self.obs = agent.observation_mapping(self.obs)
+        if agent.obs_preprocessor:
+            self.obs = agent.obs_preprocessor(self.obs)
         self.action, self.agent_info = agent.get_action(self.obs)
         self.profiling.agent_stop = time.time()
 
         self.make_stats()
 
         return self.action
```

### Comparing `browsergym_experiments-0.2.6/src/browsergym/experiments/utils.py` & `browsergym_experiments-0.3.0/src/browsergym/experiments/utils.py`

 * *Files identical despite different names*

### Comparing `browsergym_experiments-0.2.6/tests/test_exp_loop.py` & `browsergym_experiments-0.3.0/tests/test_exp_loop.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,18 @@
 from browsergym.experiments.agent import Agent
 from browsergym.experiments.loop import AbstractAgentArgs, EnvArgs, ExpArgs, get_exp_result
 from browsergym.utils.obs import flatten_axtree_to_str
 
 
 class MiniwobTestAgent(Agent):
 
-    def observation_mapping(self, obs: dict):
-        return {"axtree_txt": flatten_axtree_to_str(obs["axtree_object"])}
-
-    def action_mapping(self, action: str):
-        return self.action_space.to_python_code(action)
+    action_set = HighLevelActionSet(subsets="bid")
 
-    def __init__(self):
-        self.action_space = HighLevelActionSet(subsets="bid")
+    def obs_preprocessor(self, obs: dict):
+        return {"axtree_txt": flatten_axtree_to_str(obs["axtree_object"])}
 
     def get_action(self, obs: dict) -> tuple[str, dict]:
         match = re.search(r"^\s*\[(\d+)\].*button", obs["axtree_txt"], re.MULTILINE | re.IGNORECASE)
 
         if match:
             bid = match.group(1)
             action = f'click("{bid}")'
```

### Comparing `browsergym_experiments-0.2.6/pyproject.toml` & `browsergym_experiments-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `browsergym_experiments-0.2.6/PKG-INFO` & `browsergym_experiments-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.3
 Name: browsergym-experiments
-Version: 0.2.6
+Version: 0.3.0
 Summary: Experimentation tools for BrowserGym
 Project-URL: homepage, https://github.com/ServiceNow/BrowserGym
 Author: Alex Lacoste, Massimo Caccia, Maxime Gasse, Thibault Le Sellier De Chezelles
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >3.7
-Requires-Dist: browsergym-core==0.2.6
+Requires-Dist: browsergym-core==0.3.0
 Requires-Dist: tiktoken>=0.4
 Description-Content-Type: text/markdown
 
 # BrowserGym experiments
 
 This package provides `browsergym.experiments`, a suite of experimentation tools for [BrowserGym](https://github.com/ServiceNow/BrowserGym).
```

