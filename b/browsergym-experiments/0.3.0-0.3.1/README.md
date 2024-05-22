# Comparing `tmp/browsergym_experiments-0.3.0.tar.gz` & `tmp/browsergym_experiments-0.3.1.tar.gz`

## Comparing `browsergym_experiments-0.3.0.tar` & `browsergym_experiments-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.0/requirements.txt
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.0/src/browsergym/experiments/__init__.py
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.0/src/browsergym/experiments/agent.py
--rw-r--r--   0        0        0    21090 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.0/src/browsergym/experiments/loop.py
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.0/src/browsergym/experiments/utils.py
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.0/tests/test_exp_loop.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.0/.gitignore
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.0/README.md
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.1/requirements.txt
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.1/src/browsergym/experiments/__init__.py
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.1/src/browsergym/experiments/agent.py
+-rw-r--r--   0        0        0    21097 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.1/src/browsergym/experiments/loop.py
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.1/src/browsergym/experiments/utils.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.1/tests/test_exp_loop.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.1/.gitignore
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.1/README.md
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 browsergym_experiments-0.3.1/PKG-INFO
```

### Comparing `browsergym_experiments-0.3.0/src/browsergym/experiments/agent.py` & `browsergym_experiments-0.3.1/src/browsergym/experiments/agent.py`

 * *Files identical despite different names*

### Comparing `browsergym_experiments-0.3.0/src/browsergym/experiments/loop.py` & `browsergym_experiments-0.3.1/src/browsergym/experiments/loop.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,15 @@
             self.stack_trace = stack_trace
 
             logging.warning(err_msg + "\n" + stack_trace)
             if _is_debugging() and self.enable_debug:
                 raise
 
         finally:
-            # TODO should save at each step
+            step_info.save_step_info(self.exp_dir)
             _save_summary_info(episode_info, self.exp_dir, err_msg, stack_trace)
             try:
                 env.close()
             except Exception as e:
                 logging.error(f"Error while closing the environment: {e}")
```

### Comparing `browsergym_experiments-0.3.0/src/browsergym/experiments/utils.py` & `browsergym_experiments-0.3.1/src/browsergym/experiments/utils.py`

 * *Files identical despite different names*

### Comparing `browsergym_experiments-0.3.0/tests/test_exp_loop.py` & `browsergym_experiments-0.3.1/tests/test_exp_loop.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,16 @@
             "env_args.record_video": False,
             "n_steps": 1,
             "cum_reward": 1.0,
             "terminated": True,
             "truncated": False,
         }
 
+        assert len(exp_result.steps_info) == 2
+
         for key, target_val in target.items():
             assert key in exp_record
             assert exp_record[key] == target_val
 
         # TODO investigate why it's taking almost 5 seconds to solve
         assert exp_record["stats.cum_step_elapsed"] < 5
         if exp_record["stats.cum_step_elapsed"] > 3:
```

### Comparing `browsergym_experiments-0.3.0/pyproject.toml` & `browsergym_experiments-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `browsergym_experiments-0.3.0/PKG-INFO` & `browsergym_experiments-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.3
 Name: browsergym-experiments
-Version: 0.3.0
+Version: 0.3.1
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
-Requires-Dist: browsergym-core==0.3.0
+Requires-Dist: browsergym-core==0.3.1
 Requires-Dist: tiktoken>=0.4
 Description-Content-Type: text/markdown
 
 # BrowserGym experiments
 
 This package provides `browsergym.experiments`, a suite of experimentation tools for [BrowserGym](https://github.com/ServiceNow/BrowserGym).
```

