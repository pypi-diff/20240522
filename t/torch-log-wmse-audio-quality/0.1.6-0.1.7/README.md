# Comparing `tmp/torch_log_wmse_audio_quality-0.1.6.tar.gz` & `tmp/torch_log_wmse_audio_quality-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_log_wmse_audio_quality-0.1.6.tar", last modified: Mon May 20 21:50:52 2024, max compression
+gzip compressed data, was "torch_log_wmse_audio_quality-0.1.7.tar", last modified: Wed May 22 21:26:09 2024, max compression
```

## Comparing `torch_log_wmse_audio_quality-0.1.6.tar` & `torch_log_wmse_audio_quality-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:50:52.173886 torch_log_wmse_audio_quality-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-05-20 21:50:48.000000 torch_log_wmse_audio_quality-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-05-20 21:50:52.173886 torch_log_wmse_audio_quality-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6743 2024-05-20 21:50:48.000000 torch_log_wmse_audio_quality-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-20 21:50:48.000000 torch_log_wmse_audio_quality-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-20 21:50:52.173886 torch_log_wmse_audio_quality-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:50:52.169886 torch_log_wmse_audio_quality-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-20 21:50:48.000000 torch_log_wmse_audio_quality-0.1.6/tests/test_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:50:52.173886 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-20 21:50:48.000000 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-20 21:50:48.000000 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    32151 2024-05-20 21:50:48.000000 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality/filter_ir.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-20 21:50:48.000000 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality/freq_weighting_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-20 21:50:48.000000 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-20 21:50:48.000000 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:50:52.173886 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-05-20 21:50:52.000000 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-20 21:50:52.000000 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:50:52.000000 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-20 21:50:52.000000 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-20 21:50:52.000000 torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:26:09.932657 torch_log_wmse_audio_quality-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-05-22 21:26:05.000000 torch_log_wmse_audio_quality-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-05-22 21:26:09.932657 torch_log_wmse_audio_quality-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6743 2024-05-22 21:26:05.000000 torch_log_wmse_audio_quality-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-22 21:26:05.000000 torch_log_wmse_audio_quality-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-22 21:26:09.932657 torch_log_wmse_audio_quality-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:26:09.928657 torch_log_wmse_audio_quality-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7999 2024-05-22 21:26:05.000000 torch_log_wmse_audio_quality-0.1.7/tests/test_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:26:09.928657 torch_log_wmse_audio_quality-0.1.7/torch_log_wmse_audio_quality/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-22 21:26:05.000000 torch_log_wmse_audio_quality-0.1.7/torch_log_wmse_audio_quality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-22 21:26:05.000000 torch_log_wmse_audio_quality-0.1.7/torch_log_wmse_audio_quality/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32151 2024-05-22 21:26:05.000000 torch_log_wmse_audio_quality-0.1.7/torch_log_wmse_audio_quality/filter_ir.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-05-22 21:26:05.000000 torch_log_wmse_audio_quality-0.1.7/torch_log_wmse_audio_quality/freq_weighting_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-22 21:26:05.000000 torch_log_wmse_audio_quality-0.1.7/torch_log_wmse_audio_quality/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-22 21:26:05.000000 torch_log_wmse_audio_quality-0.1.7/torch_log_wmse_audio_quality/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:26:09.932657 torch_log_wmse_audio_quality-0.1.7/torch_log_wmse_audio_quality.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-05-22 21:26:09.000000 torch_log_wmse_audio_quality-0.1.7/torch_log_wmse_audio_quality.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-22 21:26:09.000000 torch_log_wmse_audio_quality-0.1.7/torch_log_wmse_audio_quality.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 21:26:09.000000 torch_log_wmse_audio_quality-0.1.7/torch_log_wmse_audio_quality.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-22 21:26:09.000000 torch_log_wmse_audio_quality-0.1.7/torch_log_wmse_audio_quality.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 21:26:09.000000 torch_log_wmse_audio_quality-0.1.7/torch_log_wmse_audio_quality.egg-info/top_level.txt
```

### Comparing `torch_log_wmse_audio_quality-0.1.6/LICENSE` & `torch_log_wmse_audio_quality-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.6/PKG-INFO` & `torch_log_wmse_audio_quality-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-log-wmse-audio-quality
-Version: 0.1.6
+Version: 0.1.7
 Summary: logWMSE is an audio quality metric & loss function with support for digital silence target. Useful for training and evaluating audio source separation systems.
 Home-page: https://github.com/crlandsc/torch-log-wmse-audio-quality
 Author: Christopher Landschoot
 Author-email: crlandschoot@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/crlandsc/torch-log-wmse-audio-quality/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_log_wmse_audio_quality-0.1.6/README.md` & `torch_log_wmse_audio_quality-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.6/setup.cfg` & `torch_log_wmse_audio_quality-0.1.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = torch-log-wmse-audio-quality
-version = 0.1.6
+version = 0.1.7
 author = Christopher Landschoot
 author_email = crlandschoot@gmail.com
 license = Apache License 2.0
 description = logWMSE is an audio quality metric & loss function with support for digital silence target. Useful for training and evaluating audio source separation systems.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/crlandsc/torch-log-wmse-audio-quality
```

### Comparing `torch_log_wmse_audio_quality-0.1.6/tests/test_metric.py` & `torch_log_wmse_audio_quality-0.1.7/tests/test_metric.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,32 +3,35 @@
 sys.path.append("/Users/chris/Desktop/Whitebalance/torch-log-wmse-audio-quality")
 import torch
 import numpy as np
 import matplotlib.pyplot as plt
 from torch_log_wmse_audio_quality import LogWMSE
 from torch_log_wmse_audio_quality.utils import calculate_rms
 from torch_log_wmse_audio_quality.freq_weighting_filter import prepare_impulse_response_fft, HumanHearingSensitivityFilter
+from torch_log_wmse_audio_quality.utils import convert_decibels_to_amplitude_ratio
 
 class TestLogWMSELoss(unittest.TestCase):
     def setUp(self):
         pass # Anything shared between tests
 
     def test_calculate_rms(self):
+        print("Test calculate_rms")
         for i in range(10):
             with self.subTest(i=i):
                 torch.manual_seed(i)
                 samples = torch.rand(2, 2, 44100)
                 rms = calculate_rms(samples)
 
                 self.assertIsInstance(rms, torch.Tensor)
                 self.assertEqual(rms.shape, (2, 2))
 
                 print(f"Test {i}, RMS Value: {rms.mean()}")
 
     def test_calculate_log_wmse(self):
+        print("Test calculate_log_wmse")
         log_wmse_loss = LogWMSE(audio_length=1.0, sample_rate=44100)
         input_rms = torch.ones(2, 2)
         processed_audio = torch.ones(2, 3, 2, 44100)
         target_audio = torch.ones(2, 3, 2, 44100)
 
         values = log_wmse_loss._calculate_log_wmse(
             input_rms,
@@ -39,41 +42,71 @@
 
         self.assertIsInstance(values, torch.Tensor)
         self.assertEqual(values.shape, (2, 3, 2))
 
         print(f"Values: {values}")
 
     def test_forward(self):
+        print("Test forward")
         audio_lengths = [0.1, 0.5, 1.0]  # Different audio lengths
         sample_rate = 44100
         audio_channels = 2 # stereo
         audio_stems = 3 # 3 audio stems
         batch = 4 # batch size
 
         for i, audio_length in enumerate(audio_lengths):
             log_wmse_loss = LogWMSE(audio_length=audio_length, sample_rate=sample_rate)
             for j in range(3):
                 with self.subTest(i=i, j=j):
-                    torch.manual_seed((i+1)*(j+1))  # Ensure reproducibility
+                    torch.manual_seed((i+1)*(j+1)) # Ensure reproducibility
 
                     # Generate random inputs (scale between -1 and 1)
                     audio_lengths_samples = int(audio_length * sample_rate)
                     unprocessed_audio = 2 * torch.rand(batch, audio_channels, audio_lengths_samples) - 1
                     processed_audio = unprocessed_audio.unsqueeze(1).expand(-1, audio_stems, -1, -1) * 0.1
                     target_audio = torch.zeros(batch, audio_stems, audio_channels, audio_lengths_samples)
 
                     loss = log_wmse_loss(unprocessed_audio, processed_audio, target_audio)
 
                     self.assertIsInstance(loss, torch.Tensor)
                     self.assertEqual(loss.ndim, 0)
 
                     print(f"Test {i}, Subtest {j}, Audio Length: {audio_length}, Loss: {loss}, Seed: {(i+1)*(j+1)}")
 
+    # Test forward with silence
+    def test_forward_silence(self):
+        print("Test forward with silence")
+        audio_lengths = [0.1, 0.5, 1.0]
+        sample_rate = 44100
+        audio_channels = 2 # stereo
+        audio_stems = 3 # 3 audio stems
+        batch = 4 # batch size
+
+        for i, audio_length in enumerate(audio_lengths):
+            log_wmse_loss = LogWMSE(audio_length=audio_length, sample_rate=sample_rate)
+            for j in range(3):
+                with self.subTest(i=i, j=j):
+                    torch.manual_seed((i+1)*(j+1)) # Ensure reproducibility
+
+                    # Generate random inputs (scale between -1 and 1)
+                    audio_lengths_samples = int(audio_length * sample_rate)
+                    unprocessed_audio = torch.zeros(batch, audio_channels, audio_lengths_samples)
+                    processed_audio = torch.rand(batch, audio_stems, audio_channels, audio_lengths_samples) * convert_decibels_to_amplitude_ratio(-60)
+                    target_audio = torch.zeros(batch, audio_stems, audio_channels, audio_lengths_samples)
+
+                    loss = log_wmse_loss(unprocessed_audio, processed_audio, target_audio)
+
+                    self.assertIsInstance(loss, torch.Tensor)
+                    self.assertEqual(loss.ndim, 0)
+
+                    print(f"Test {i}, Subtest {j}, Audio Length: {audio_length}, Loss: {loss}, Seed: {(i+1)*(j+1)}")
+
     def test_logWMSE_metric_comparison(self):
         """For comparison with the original logWMSE metric implementation in numpy."""
+        print("Test logWMSE metric comparison")
         audio_lengths = [0.01, 0.1, 0.5, 1.0, 2.0, 10.0]  # Different audio lengths
         for i, audio_length in enumerate(audio_lengths):
             log_wmse_loss = LogWMSE(audio_length=audio_length, sample_rate=44100)
             for j in range(3):
                 with self.subTest(i=i, j=j):
                     torch.manual_seed((i+1)*(j+1))  # Ensure reproducibility
                     np.random.seed((i+1)*(j+1))  # to make the test reproducible
@@ -92,45 +125,51 @@
                     print(f"Test {i}, Subtest {j}, Audio Length: {audio_length}, Loss: {loss}, Seed: {(i+1)*(j+1)}")
 
 class TestFreqWeightingFilter(unittest.TestCase):
     def setUp(self):
         # Example audio data, replace with actual audio loading if needed
         self.plot_output = False
         self.sample_rate = 44100
-        self.audio_length = 1.7516936
+        self.audio_length = 3.7516936
+        tone = 440 # sine wave in Hz
         t = np.arange(0, int(self.audio_length*self.sample_rate)) / self.sample_rate
-        self.audio = torch.tensor(0.5 * np.sin(2 * np.pi * 440 * t))  # A simple 440 Hz sine wave
+        self.audio = torch.tensor(0.5 * np.sin(2 * np.pi * tone * t)) # create sine wave
         self.audio = self.audio[None, None, None, :]
 
     def test_prepare_impulse_response_fft(self):
+        print("Test prepare_impulse_response_fft")
         ir = torch.rand(512)  # Example impulse response
         fft_size = 1024
         ir_fft = prepare_impulse_response_fft(ir, fft_size)
         self.assertEqual(ir_fft.shape[-1], fft_size//2+1)
 
     def test_HumanHearingSensitivityFilter(self):
+        print("Test HumanHearingSensitivityFilter")
         plot_upper_bound = 500
         hhs_filter = HumanHearingSensitivityFilter(audio_length=self.audio_length, sample_rate=self.sample_rate)
         # Add zeros at index 50-100 to demonstrate time alignment
         self.audio[:, :, :, 50:100] = 0
         self.audio[:, :, :, 101:125] = 0.5
         self.audio[:, :, :, 126:150] = -0.5
+        self.audio[:, :, :, 151:200] = 0
 
         filtered_audio = hhs_filter(self.audio)
 
         # Plot the first 1000 samples before and after filtering
         if self.plot_output:
             fig, axs = plt.subplots(2, 1, figsize=(12, 8))
             axs[0].plot(self.audio.squeeze()[:plot_upper_bound])
             axs[0].set_title(f'Original Audio (First {plot_upper_bound} Samples)')
             axs[0].set_ylim(-1, 1)
             axs[1].plot(filtered_audio.squeeze()[:plot_upper_bound])
             axs[1].set_title(f'Filtered Audio (First {plot_upper_bound} Samples)')
             axs[1].set_ylim(-1, 1)
             plt.tight_layout()
             plt.show()
+        else:
+            print("Plotting disabled.")
 
         self.assertEqual(filtered_audio.shape, self.audio.shape)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality/constants.py` & `torch_log_wmse_audio_quality-0.1.7/torch_log_wmse_audio_quality/constants.py`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality/filter_ir.pkl` & `torch_log_wmse_audio_quality-0.1.7/torch_log_wmse_audio_quality/filter_ir.pkl`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality/freq_weighting_filter.py` & `torch_log_wmse_audio_quality-0.1.7/torch_log_wmse_audio_quality/freq_weighting_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,11 +146,11 @@
         audio = torch.nn.functional.pad(audio, (0, padding))
 
         # Apply FFT convolution
         filtered_audio = fft_convolve(audio, self.impulse_response_fft, self.fft_size)
 
         # Circularly shift signal to account for symmetric IR time delay
         if self.symmetric_ir:
-            shift = self.fft_size // 2
+            shift = (self.fft_size - (self.impulse_response.shape[-1] % 2)) // 2 - 1 # added case for odd length IR
             filtered_audio = torch.roll(filtered_audio, -shift, dims=-1)
 
         return filtered_audio[..., :self.audio_length_samples]
```

### Comparing `torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality/metric.py` & `torch_log_wmse_audio_quality-0.1.7/torch_log_wmse_audio_quality/metric.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,18 +58,14 @@
         assert processed_audio.ndim == 4 # processed_audio audio shape: [batch, channel, stem, time]
         assert target_audio.ndim == 4 # target_audio audio shape: [batch, channel, stem, time]
         assert processed_audio.shape == target_audio.shape # processed_audio and target_audio should have the same shape
         assert processed_audio.shape[-1] == target_audio.shape[-1] == unprocessed_audio.shape[-1] # all should have the same length
 
         input_rms = calculate_rms(self.filters(unprocessed_audio.unsqueeze(1))) # unsqueeze to add "stem" dimension
 
-        # Avoid log(0)
-        if input_rms.sum() == 0:
-            return torch.log(torch.tensor(EPS)) * SCALER
-
         # Calculate the logWMSE
         values = self._calculate_log_wmse(
             input_rms,
             self.filters,
             processed_audio,
             target_audio,
         )
@@ -94,14 +90,19 @@
             filters (Callable): A function that applies a filter to the audio (i.e. HumanHearingSensitivityFilter).
             processed_audio (Tensor): The processed audio tensor.
             target_audio (Tensor): The target audio tensor.
 
         Returns:
             Tensor: The logWMSE between the processed audio and target audio.
         """
+
+        # Add EPS if input_rms is 0 (silence) to avoid NaNs
+        if input_rms.sum() == 0:
+            input_rms = torch.ones_like(input_rms) * ERROR_TOLERANCE_THRESHOLD
+
         # Calculate the scaling factor based on the input RMS
         scaling_factor = 1 / input_rms
 
         # Add extra dimensions to scaling_factor to match the shape of processed_audio and target_audio
         if scaling_factor.dim() == 2:
             scaling_factor = scaling_factor.unsqueeze(1)
         while scaling_factor.dim() < processed_audio.dim():
```

### Comparing `torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality/utils.py` & `torch_log_wmse_audio_quality-0.1.7/torch_log_wmse_audio_quality/utils.py`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality.egg-info/PKG-INFO` & `torch_log_wmse_audio_quality-0.1.7/torch_log_wmse_audio_quality.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-log-wmse-audio-quality
-Version: 0.1.6
+Version: 0.1.7
 Summary: logWMSE is an audio quality metric & loss function with support for digital silence target. Useful for training and evaluating audio source separation systems.
 Home-page: https://github.com/crlandsc/torch-log-wmse-audio-quality
 Author: Christopher Landschoot
 Author-email: crlandschoot@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/crlandsc/torch-log-wmse-audio-quality/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_log_wmse_audio_quality-0.1.6/torch_log_wmse_audio_quality.egg-info/SOURCES.txt` & `torch_log_wmse_audio_quality-0.1.7/torch_log_wmse_audio_quality.egg-info/SOURCES.txt`

 * *Files identical despite different names*

