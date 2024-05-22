# Comparing `tmp/fugent_model-0.0.1.tar.gz` & `tmp/fugent_model-0.0.2.tar.gz`

## Comparing `fugent_model-0.0.1.tar` & `fugent_model-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fugent_model-0.0.1/src/fugent_model/__init__.py
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 fugent_model-0.0.1/src/fugent_model/__main__.py
--rw-r--r--   0        0        0    18790 2020-02-02 00:00:00.000000 fugent_model-0.0.1/src/fugent_model/environment.py
--rw-r--r--   0        0        0    12122 2020-02-02 00:00:00.000000 fugent_model-0.0.1/src/fugent_model/model.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 fugent_model-0.0.1/src/fugent_model/requirements.txt
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 fugent_model-0.0.1/src/fugent_model/run.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 fugent_model-0.0.1/src/fugent_model/train.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 fugent_model-0.0.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 fugent_model-0.0.1/LICENSE
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 fugent_model-0.0.1/README.md
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 fugent_model-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 fugent_model-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fugent_model-0.0.2/src/fugent_model/__init__.py
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 fugent_model-0.0.2/src/fugent_model/__main__.py
+-rw-r--r--   0        0        0    18790 2020-02-02 00:00:00.000000 fugent_model-0.0.2/src/fugent_model/environment.py
+-rw-r--r--   0        0        0    11547 2020-02-02 00:00:00.000000 fugent_model-0.0.2/src/fugent_model/model.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 fugent_model-0.0.2/src/fugent_model/requirements.txt
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 fugent_model-0.0.2/src/fugent_model/run.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 fugent_model-0.0.2/src/fugent_model/train.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fugent_model-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 fugent_model-0.0.2/LICENSE
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 fugent_model-0.0.2/README.md
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 fugent_model-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 fugent_model-0.0.2/PKG-INFO
```

### Comparing `fugent_model-0.0.1/src/fugent_model/__main__.py` & `fugent_model-0.0.2/src/fugent_model/__main__.py`

 * *Files identical despite different names*

### Comparing `fugent_model-0.0.1/src/fugent_model/environment.py` & `fugent_model-0.0.2/src/fugent_model/environment.py`

 * *Files identical despite different names*

### Comparing `fugent_model-0.0.1/src/fugent_model/model.py` & `fugent_model-0.0.2/src/fugent_model/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     
     Critic = Model(inputs = inputs, outputs = value, name='critic')
     Critic.compile(loss='mse', optimizer=RMSprop(learning_rate=learning_rate))
     
     return Actor, Critic
     
 class A3CAgent:
-    def __init__(self, model_path, envClass, learning_rate=0.00025, episodes=100, name=None, load_only=False):
+    def __init__(self, model_path, envClass, learning_rate=0.00025, episodes=100, name=None, load_only=False, load_path=None):
         self.environment = envClass
         self.env = self.environment()
         self.lock = Lock()
         self.action_size = self.env.action_size
         self.max_average = -1000000
         
         self.name = name if name is not None else type(self.env).__name__
@@ -144,15 +144,15 @@
         self.inputSize = self.env.inputSize
         
         #HYPERPARAMETERS
         self.history_length = self.env.history_length
         self.episodes = episodes
         self.learning_rate = learning_rate
         
-        self.save_path = model_path or os.path.join(os.path.dirname(__file__), "Models")
+        self.save_path = load_path if load_path is not None else os.path.join(os.path.dirname(__file__), "Models")
         self.save_name = self.name
         self.model_name = os.path.join(self.save_path, self.save_name)
         
         if load_only:
             if self.exists():
                 self.load(self.model_name)
             else: 
@@ -315,25 +315,8 @@
         reward = np.reshape(reward, expected_reward.shape)
         
         # Compute advantages
         advantages = reward - expected_reward
         
         # training Actor and Critic networks
         self.actor.fit(states, actions, sample_weight=advantages, epochs=1, verbose=0)
-        self.critic.fit(states, reward, epochs=1, verbose=0)
-
-
-
-class Fugent_A3CAgent(A3CAgent):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        
-    def onehot_actionMap(self, state):
-        state = np.reshape(state, (1, self.history_length, self.stateSize+self.imgSize))
-        prediction = self.actor.predict(state)[0]
-        prediction = np.reshape(prediction, self.env.gridSize)
-        return prediction    
-        
-    def critic_act(self, state):
-        state = np.reshape(state, (1, self.history_length, self.stateSize+self.imgSize))
-        prediction = float(self.critic.predict(state)[0][0])
-        return prediction
+        self.critic.fit(states, reward, epochs=1, verbose=0)
```

### Comparing `fugent_model-0.0.1/src/fugent_model/run.py` & `fugent_model-0.0.2/src/fugent_model/run.py`

 * *Files identical despite different names*

### Comparing `fugent_model-0.0.1/src/fugent_model/train.py` & `fugent_model-0.0.2/src/fugent_model/train.py`

 * *Files identical despite different names*

### Comparing `fugent_model-0.0.1/LICENSE` & `fugent_model-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fugent_model-0.0.1/pyproject.toml` & `fugent_model-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "Fugent_Model"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="James Hammer", email="jhammer3@vols.utk.edu" },
 ]
 description = "code required for training and running Fugent Agents"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -22,9 +22,9 @@
   "scipy==1.11.4",
   "tensorflow==2.15.0.post1",
   "tf-slim==1.1.0",
   "pillow==10.3.0"
 ]
 
 [project.urls]
-Homepage = "https://github.com/seelabutk/xgc_poincare"
-Issues = "https://github.com/seelabutk/XGC_Poincare/issues"
+Homepage = "https://github.com/seelabutk/Fugent_Model"
+Issues = "https://github.com/seelabutk/Fugent_Model/issues"
```

