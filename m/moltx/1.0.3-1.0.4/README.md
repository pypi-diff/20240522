# Comparing `tmp/moltx-1.0.3.tar.gz` & `tmp/moltx-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moltx-1.0.3.tar", last modified: Tue May 21 01:34:08 2024, max compression
+gzip compressed data, was "moltx-1.0.4.tar", last modified: Wed May 22 10:55:40 2024, max compression
```

## Comparing `moltx-1.0.3.tar` & `moltx-1.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:34:08.637158 moltx-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-21 01:34:04.000000 moltx-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-05-21 01:34:08.637158 moltx-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-21 01:34:04.000000 moltx-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:34:08.637158 moltx-1.0.3/moltx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 01:34:04.000000 moltx-1.0.3/moltx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 01:34:04.000000 moltx-1.0.3/moltx/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:34:08.637158 moltx-1.0.3/moltx/data/
--rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-05-21 01:34:04.000000 moltx-1.0.3/moltx/data/spe_safe.txt
--rw-r--r--   0 runner    (1001) docker     (127)    27879 2024-05-21 01:34:04.000000 moltx-1.0.3/moltx/data/spe_smiles.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-05-21 01:34:04.000000 moltx-1.0.3/moltx/data/tks_safe.json
--rw-r--r--   0 runner    (1001) docker     (127)    36304 2024-05-21 01:34:04.000000 moltx-1.0.3/moltx/data/tks_smiles.json
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-21 01:34:04.000000 moltx-1.0.3/moltx/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-05-21 01:34:04.000000 moltx-1.0.3/moltx/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-21 01:34:04.000000 moltx-1.0.3/moltx/nets.py
--rw-r--r--   0 runner    (1001) docker     (127)    10328 2024-05-21 01:34:04.000000 moltx-1.0.3/moltx/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-21 01:34:04.000000 moltx-1.0.3/moltx/tokenizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:34:08.637158 moltx-1.0.3/moltx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-05-21 01:34:08.000000 moltx-1.0.3/moltx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-21 01:34:08.000000 moltx-1.0.3/moltx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 01:34:08.000000 moltx-1.0.3/moltx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 01:34:08.000000 moltx-1.0.3/moltx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 01:34:08.000000 moltx-1.0.3/moltx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 01:34:04.000000 moltx-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-21 01:34:08.637158 moltx-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 01:34:04.000000 moltx-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 01:34:08.637158 moltx-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-21 01:34:04.000000 moltx-1.0.3/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-21 01:34:04.000000 moltx-1.0.3/tests/test_nets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-05-21 01:34:04.000000 moltx-1.0.3/tests/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-21 01:34:04.000000 moltx-1.0.3/tests/test_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:55:40.166641 moltx-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-22 10:55:35.000000 moltx-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-05-22 10:55:40.166641 moltx-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-22 10:55:35.000000 moltx-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:55:40.162641 moltx-1.0.4/moltx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:55:35.000000 moltx-1.0.4/moltx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 10:55:35.000000 moltx-1.0.4/moltx/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:55:40.166641 moltx-1.0.4/moltx/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-05-22 10:55:35.000000 moltx-1.0.4/moltx/data/spe_safe.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    27879 2024-05-22 10:55:35.000000 moltx-1.0.4/moltx/data/spe_smiles.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-05-22 10:55:35.000000 moltx-1.0.4/moltx/data/tks_safe.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36304 2024-05-22 10:55:35.000000 moltx-1.0.4/moltx/data/tks_smiles.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-22 10:55:35.000000 moltx-1.0.4/moltx/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-05-22 10:55:35.000000 moltx-1.0.4/moltx/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-22 10:55:35.000000 moltx-1.0.4/moltx/nets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10328 2024-05-22 10:55:35.000000 moltx-1.0.4/moltx/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-22 10:55:35.000000 moltx-1.0.4/moltx/tokenizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:55:40.166641 moltx-1.0.4/moltx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-05-22 10:55:40.000000 moltx-1.0.4/moltx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-22 10:55:40.000000 moltx-1.0.4/moltx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:55:40.000000 moltx-1.0.4/moltx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 10:55:40.000000 moltx-1.0.4/moltx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 10:55:40.000000 moltx-1.0.4/moltx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 10:55:35.000000 moltx-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-22 10:55:40.166641 moltx-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 10:55:35.000000 moltx-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:55:40.166641 moltx-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-22 10:55:35.000000 moltx-1.0.4/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-22 10:55:35.000000 moltx-1.0.4/tests/test_nets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-05-22 10:55:35.000000 moltx-1.0.4/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-22 10:55:35.000000 moltx-1.0.4/tests/test_tokenizer.py
```

### Comparing `moltx-1.0.3/LICENSE` & `moltx-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `moltx-1.0.3/PKG-INFO` & `moltx-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moltx
-Version: 1.0.3
+Version: 1.0.4
 Summary: Molcule Transformer X Model
 Author: Michael Ding
 Author-email: yandy.ding@gmail.com
 Keywords: molcule,AI,deep learning,transformer
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX
```

### Comparing `moltx-1.0.3/README.md` & `moltx-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `moltx-1.0.3/moltx/data/spe_safe.txt` & `moltx-1.0.4/moltx/data/spe_safe.txt`

 * *Files identical despite different names*

### Comparing `moltx-1.0.3/moltx/data/spe_smiles.txt` & `moltx-1.0.4/moltx/data/spe_smiles.txt`

 * *Files identical despite different names*

### Comparing `moltx-1.0.3/moltx/data/tks_safe.json` & `moltx-1.0.4/moltx/data/tks_safe.json`

 * *Files identical despite different names*

### Comparing `moltx-1.0.3/moltx/data/tks_smiles.json` & `moltx-1.0.4/moltx/data/tks_smiles.json`

 * *Files identical despite different names*

### Comparing `moltx-1.0.3/moltx/datasets.py` & `moltx-1.0.4/moltx/datasets.py`

 * *Files identical despite different names*

### Comparing `moltx-1.0.3/moltx/models.py` & `moltx-1.0.4/moltx/models.py`

 * *Files identical despite different names*

### Comparing `moltx-1.0.3/moltx/nets.py` & `moltx-1.0.4/moltx/nets.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         return self.transformer(src, tgt, tgt_mask=mask, tgt_is_causal=True)
 
     def forward_feature(self, src: torch.Tensor, tgt: torch.Tensor) -> torch.Tensor:
         out = self.forward_(src, tgt)
         indices = (tgt > 0).sum(dim=-1, keepdim=True) - 1
         indices = indices.unsqueeze(-1).repeat(*
                                                [1 for _ in range(tgt.dim())], out.shape[-1])
-        return torch.gather(input=out, dim=-2, index=indices).squeeze()
+        return torch.gather(input=out, dim=-2, index=indices).squeeze(-2)
 
     def forward_generation(self, src: torch.Tensor, tgt: torch.Tensor) -> torch.Tensor:
         out = self.forward_(src, tgt)
         return self.token_output(out)
 
 
 @dataclass
@@ -101,12 +101,12 @@
         return self.transformer(tgt, mask=mask, is_causal=True)
 
     def forward_feature(self, tgt: torch.Tensor) -> torch.Tensor:
         out = self.forward_(tgt)
         indices = (tgt > 0).sum(dim=-1, keepdim=True) - 1
         indices = indices.unsqueeze(-1).repeat(*
                                                [1 for _ in range(tgt.dim())], out.shape[-1])
-        return torch.gather(input=out, dim=-2, index=indices).squeeze()
+        return torch.gather(input=out, dim=-2, index=indices).squeeze(-2)
 
     def forward_generation(self, tgt: torch.Tensor) -> torch.Tensor:
         out = self.forward_(tgt)
         return self.token_output(out)
```

### Comparing `moltx-1.0.3/moltx/pipelines.py` & `moltx-1.0.4/moltx/pipelines.py`

 * *Files identical despite different names*

### Comparing `moltx-1.0.3/moltx/tokenizers.py` & `moltx-1.0.4/moltx/tokenizers.py`

 * *Files identical despite different names*

### Comparing `moltx-1.0.3/moltx.egg-info/PKG-INFO` & `moltx-1.0.4/moltx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moltx
-Version: 1.0.3
+Version: 1.0.4
 Summary: Molcule Transformer X Model
 Author: Michael Ding
 Author-email: yandy.ding@gmail.com
 Keywords: molcule,AI,deep learning,transformer
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX
```

### Comparing `moltx-1.0.3/moltx.egg-info/SOURCES.txt` & `moltx-1.0.4/moltx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moltx-1.0.3/setup.cfg` & `moltx-1.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `moltx-1.0.3/tests/test_datasets.py` & `moltx-1.0.4/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `moltx-1.0.3/tests/test_nets.py` & `moltx-1.0.4/tests/test_nets.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,18 @@
     out = model.forward_(tokens, tokens)
     assert out.shape == (32, 8)
     feat = model.forward_feature(tokens, tokens)
     assert feat.shape == (8,)
     assert feat.eq(out[-1]).all()
     gen = model.forward_generation(tokens, tokens)
     assert gen.shape == (32, 16)
+    
+    tokens = torch.randint(1, 16, (1, 32))
+    feat = model.forward_feature(tokens, tokens)
+    assert feat.shape == (1, 8)
 
     conf = nets.AbsPosEncoderDecoderConfig(
         token_size=16, max_len=32, d_model=8, nhead=2,
         num_encoder_layers=2, num_decoder_layers=2, dtype=torch.bfloat16)
     model = nets.AbsPosEncoderDecoder(conf=conf)
     model.eval()
     model.requires_grad_(False)
@@ -81,14 +85,18 @@
     out = model.forward_(tokens)
     assert out.shape == (32, 8)
     feat = model.forward_feature(tokens)
     assert feat.shape == (8,)
     assert feat.eq(out[-1]).all()
     gen = model.forward_generation(tokens)
     assert gen.shape == (32, 16)
+    
+    tokens = torch.randint(1, 16, (1, 32))
+    feat = model.forward_feature(tokens)
+    assert feat.shape == (1, 8)  
 
     conf = nets.AbsPosEncoderCausalConfig(
         token_size=16, max_len=32, d_model=8, nhead=2, num_layers=2, dtype=torch.bfloat16)
     model = nets.AbsPosEncoderCausal(conf=conf)
     model.eval()
     model.requires_grad_(False)
```

### Comparing `moltx-1.0.3/tests/test_pipelines.py` & `moltx-1.0.4/tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `moltx-1.0.3/tests/test_tokenizer.py` & `moltx-1.0.4/tests/test_tokenizer.py`

 * *Files identical despite different names*

