# Comparing `tmp/glview-1.9.1.tar.gz` & `tmp/glview-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glview-1.9.1.tar", last modified: Fri Oct 27 11:55:15 2023, max compression
+gzip compressed data, was "glview-1.9.2.tar", last modified: Mon Nov 27 16:31:52 2023, max compression
```

## Comparing `glview-1.9.1.tar` & `glview-1.9.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-10-27 11:55:15.256990 glview-1.9.1/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1068 2023-03-13 15:45:56.000000 glview-1.9.1/LICENSE
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       99 2023-03-13 15:45:56.000000 glview-1.9.1/MANIFEST.in
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      829 2023-10-27 11:55:15.256990 glview-1.9.1/PKG-INFO
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      380 2023-09-14 11:42:57.000000 glview-1.9.1/README.md
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-10-27 11:55:15.256990 glview-1.9.1/glview/
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      332 2023-07-26 12:23:21.000000 glview-1.9.1/glview/__init__.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    15417 2023-03-13 15:45:56.000000 glview-1.9.1/glview/argv.py
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    12685 2023-10-13 13:47:38.000000 glview-1.9.1/glview/glrenderer.py
--rwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)    10688 2023-10-24 12:57:48.000000 glview-1.9.1/glview/glview.py
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    10468 2023-10-24 13:50:19.000000 glview-1.9.1/glview/imageprovider.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      297 2023-05-09 09:52:42.000000 glview-1.9.1/glview/panzoom.vs
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    21812 2023-10-27 11:47:24.000000 glview-1.9.1/glview/pygletui.py
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    14856 2023-09-29 14:12:12.000000 glview-1.9.1/glview/texture.fs
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       22 2023-10-27 11:47:24.000000 glview-1.9.1/glview/version.py
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-10-27 11:55:15.256990 glview-1.9.1/glview.egg-info/
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      829 2023-10-27 11:55:15.000000 glview-1.9.1/glview.egg-info/PKG-INFO
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      431 2023-10-27 11:55:15.000000 glview-1.9.1/glview.egg-info/SOURCES.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-10-27 11:55:15.000000 glview-1.9.1/glview.egg-info/dependency_links.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       39 2023-10-27 11:55:15.000000 glview-1.9.1/glview.egg-info/entry_points.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      126 2023-10-27 11:55:15.000000 glview-1.9.1/glview.egg-info/requires.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        7 2023-10-27 11:55:15.000000 glview-1.9.1/glview.egg-info/top_level.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-10-27 11:55:15.000000 glview-1.9.1/glview.egg-info/zip-safe
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      161 2023-08-28 12:14:07.000000 glview-1.9.1/requirements.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       38 2023-10-27 11:55:15.256990 glview-1.9.1/setup.cfg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1200 2023-03-13 15:45:56.000000 glview-1.9.1/setup.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-11-27 16:31:52.464191 glview-1.9.2/
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1068 2023-03-13 15:45:56.000000 glview-1.9.2/LICENSE
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       99 2023-11-07 09:19:48.000000 glview-1.9.2/MANIFEST.in
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      829 2023-11-27 16:31:52.464191 glview-1.9.2/PKG-INFO
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      380 2023-11-07 09:19:48.000000 glview-1.9.2/README.md
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-11-27 16:31:52.460190 glview-1.9.2/glview/
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      332 2023-11-07 09:19:48.000000 glview-1.9.2/glview/__init__.py
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    15417 2023-11-07 09:19:48.000000 glview-1.9.2/glview/argv.py
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    16538 2023-11-27 16:26:39.000000 glview-1.9.2/glview/glrenderer.py
+-rwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)    10687 2023-11-27 16:27:07.000000 glview-1.9.2/glview/glview.py
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    11597 2023-11-27 16:26:51.000000 glview-1.9.2/glview/imageprovider.py
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      297 2023-11-07 09:19:48.000000 glview-1.9.2/glview/panzoom.vs
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    22167 2023-11-27 16:26:39.000000 glview-1.9.2/glview/pygletui.py
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)    14856 2023-11-07 09:19:48.000000 glview-1.9.2/glview/texture.fs
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       22 2023-11-27 16:28:34.000000 glview-1.9.2/glview/version.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-11-27 16:31:52.464191 glview-1.9.2/glview.egg-info/
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      829 2023-11-27 16:31:52.000000 glview-1.9.2/glview.egg-info/PKG-INFO
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      431 2023-11-27 16:31:52.000000 glview-1.9.2/glview.egg-info/SOURCES.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-11-27 16:31:52.000000 glview-1.9.2/glview.egg-info/dependency_links.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       39 2023-11-27 16:31:52.000000 glview-1.9.2/glview.egg-info/entry_points.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      126 2023-11-27 16:31:52.000000 glview-1.9.2/glview.egg-info/requires.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        7 2023-11-27 16:31:52.000000 glview-1.9.2/glview.egg-info/top_level.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-11-27 16:31:52.000000 glview-1.9.2/glview.egg-info/zip-safe
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      161 2023-11-07 09:19:48.000000 glview-1.9.2/requirements.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       38 2023-11-27 16:31:52.464191 glview-1.9.2/setup.cfg
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     1200 2023-11-07 09:19:48.000000 glview-1.9.2/setup.py
```

### Comparing `glview-1.9.1/LICENSE` & `glview-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `glview-1.9.1/PKG-INFO` & `glview-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glview
-Version: 1.9.1
+Version: 1.9.2
 Summary: Lightning-fast image viewer with smooth zooming & panning.
 Home-page: http://github.com/toaarnio/glview
 Author: Tomi Aarnio
 Author-email: tomi.p.aarnio@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `glview-1.9.1/glview/argv.py` & `glview-1.9.2/glview/argv.py`

 * *Files identical despite different names*

### Comparing `glview-1.9.1/glview/glview.py` & `glview-1.9.2/glview/glview.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         print("    l                       toggle current image linearization on/off")
         print("    s                       split window into 1/2/3/4 tiles")
         print("    1 / 2 / 3 / 4           select active tile for PageUp/PageDown/r/l")
         print("    h                       reset zoom/pan/exposure to initial state")
         print("    f                       toggle fullscreen <-> windowed")
         print("    t                       toggle nearest <-> linear filtering")
         print("    g                       toggle output gamma: sRGB/HDR10/HLG")
-        print("    n                       toggle exposure normalization on/off")
+        print("    n                       toggle exposure normalization modes")
         print("    e                       slide exposure from -2EV to +2EV & back")
         print("    b                       toggle between HDR/LDR exposure control")
         print("    i                       toggle input color space: sRGB/P3/Rec2020")
         print("    o                       toggle output color space: sRGB/P3/Rec2020")
         print("    k                       toggle gamut compression strength")
         print("    x                       print image information (EXIF)")
         print("    w                       write a screenshot as both JPG & PFM")
```

### Comparing `glview-1.9.1/glview/imageprovider.py` & `glview-1.9.2/glview/imageprovider.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,14 +83,32 @@
 
     def release_image(self, index):
         """
         Release the image at the given index to (eventually) free up the memory.
         """
         self.files.images[index] = "RELEASED"
 
+    def _degamma(self, frame: np.ndarray) -> np.ndarray:
+        """
+        Apply standard sRGB inverse gamma on the given uint8/16 frame, returning
+        the result in normalized float16 format.
+        """
+        assert frame.dtype in [np.uint8, np.uint16], frame.dtype
+        t0 = time.time()
+        bpp = 8 if frame.dtype == np.uint8 else 16
+        lut = np.linspace(0, 1, 2 ** bpp).astype(np.float16)
+        srgb_lo = lut / 12.92
+        srgb_hi = np.power((lut + 0.055) / 1.055, 2.4)
+        threshold_mask = (lut > 0.04045)
+        lut = srgb_hi * threshold_mask + srgb_lo * (~threshold_mask)
+        frame = lut[frame]
+        elapsed = (time.time() - t0) * 1000
+        self._vprint(f"Applying inverse sRGB gamma took {elapsed:.1f} ms")
+        return frame
+
     def _parallel_loader(self, downsample):
         ram_total = psutil.virtual_memory().total / 1024**2
         ram_before = psutil.virtual_memory().available / 1024**2
         verbose = self.verbose or self.files.numfiles < 200
         def split():
             nfiles = self.files.numfiles
             splits = [2, 8, 16] + list(range(32, nfiles, 32))
@@ -175,14 +193,20 @@
                     basename = os.path.basename(filespec)
                     with tempfile.NamedTemporaryFile(suffix=f"_{basename}") as tmpfile:
                         tmpfile.write(data)
                         img, maxval = imgio.imread(tmpfile.name, verbose=verbose)
                 img = img[::downsample, ::downsample]
                 img = np.atleast_3d(img)  # {2D, 3D} => 3D
                 img = img[:, :, :3]  # scrap alpha channel, if any
+                if self.files.linearize[idx]:
+                    # invert sRGB gamma, as OpenGL texture filtering assumes
+                    # linear colors; float16 precision is the minimum to avoid
+                    # clipping dark colors to black
+                    self.files.linearize[idx] = False
+                    img = self._degamma(img)
                 if img.dtype == np.uint16:
                     # uint16 still doesn't work in ModernGL as of 5.7.4;
                     # scale to [0, 1] and use float32 instead
                     norm = max(maxval, np.max(img))
                     img = img.astype(np.float32) / norm
                 if img.dtype == np.float64:
                     # float64 is not universally supported yet
```

### Comparing `glview-1.9.1/glview/pygletui.py` & `glview-1.9.2/glview/pygletui.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         self.renderer = None
         self.texture_filter = "NEAREST"
         self.img_per_tile = [0, 1, 2, 3]
         self.images_pending = True
         self.cs_in = 0
         self.cs_out = 0
         self.gamma = 1
-        self.normalize = False
+        self.normalize = 0  # 0|1|2|...
         self.ev_range = 2
         self.ev_linear = 0.0
         self.ev = 0.0
         self.gamut_fit = 0  # 0|1|2...
         self.gamut_lim = np.ones(3) * 1.1
         self.gamut_pow = np.ones(3) * 1.5
         self.gamut_thr = np.ones(3) * 0.8
@@ -87,15 +87,15 @@
         parent = self
 
         class _EventLoop(pyglet.app.EventLoop):
             def idle(self):
                 parent._keyboard_zoom_pan()
                 parent._smooth_exposure()
                 parent._poll_loading()
-                self.clock.update_time()
+                parent._upload_textures()
                 window = list(pyglet.app.windows)[0]
                 window.dispatch_event("on_draw")
                 return 1/60  # pan/zoom at max 60 fps
 
         return _EventLoop()
 
     def _init_pyglet(self):
@@ -122,20 +122,27 @@
                 self.images_pending = True
                 break
         else:
             if self.images_pending:
                 self.images_pending = False
                 self.need_redraw = True
 
+    def _upload_textures(self):
+        if not self.images_pending and not self.need_redraw:
+            for imgidx in range(self.files.numfiles):
+                texture = self.renderer.upload_texture(imgidx, piecewise=True)
+                if not texture.extra.done:
+                    break
+
     def _caption(self):
         ver = self.version
-        fps = pyglet.clock.get_frequency()
+        fps = np.median(self.renderer.fps)
         cspaces = ["sRGB", "DCI-P3", "Rec2020"]
         csc = f"{cspaces[self.cs_in]} => {cspaces[self.cs_out]}"
-        norm = "off" if not self.normalize else "on"
+        norm = ["off", "max", "99.5%", "98%", "95%", "90%", "mean"][self.normalize]
         gamma = ["off", "sRGB", "HLG", "HDR10"][self.gamma]
         gamut = "clip" if not self.gamut_fit else f"fit p = {self.gamut_pow[0]:.1f}"
         caption = f"glview {ver} | {self.ev:+1.2f}EV | norm {norm} | {csc} | gamut {gamut} | gamma {gamma} | {fps:.0f} fps"
         for tileidx in range(self.numtiles):
             imgidx = self.img_per_tile[tileidx]
             basename = self.files.filespecs[imgidx]
             caption = f"{caption} | {basename} [{imgidx+1}/{self.files.numfiles}]"
@@ -355,16 +362,16 @@
                     self.need_redraw = True
                 if symbol == keys.B:  # toggle between narrow/wide (LDR/HDR) exposure control
                     self.ev_range = (self.ev_range + 6) % 12
                     self.need_redraw = True
                 if symbol == keys.K: # cycle through gamut compression modes (off/hi/lo)
                     self._switch_gamut_curve()
                     self.need_redraw = True
-                if symbol == keys.N:  # normalize
-                    self.normalize = not self.normalize
+                if symbol == keys.N:  # normalize off/max/...
+                    self.normalize = (self.normalize + 1) % 7
                     self.need_redraw = True
                 if symbol == keys.T:  # texture filtering
                     self.texture_filter = "LINEAR" if self.texture_filter == "NEAREST" else "NEAREST"
                     self.need_redraw = True
                 if symbol == keys.S:  # split
                     if self.numtiles == 4 and self.layout == "N x 1":
                         self.layout = "2 x 2"
```

### Comparing `glview-1.9.1/glview/texture.fs` & `glview-1.9.2/glview/texture.fs`

 * *Files identical despite different names*

### Comparing `glview-1.9.1/glview.egg-info/PKG-INFO` & `glview-1.9.2/glview.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glview
-Version: 1.9.1
+Version: 1.9.2
 Summary: Lightning-fast image viewer with smooth zooming & panning.
 Home-page: http://github.com/toaarnio/glview
 Author: Tomi Aarnio
 Author-email: tomi.p.aarnio@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `glview-1.9.1/setup.py` & `glview-1.9.2/setup.py`

 * *Files identical despite different names*

