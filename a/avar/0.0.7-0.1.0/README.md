# Comparing `tmp/avar-0.0.7.tar.gz` & `tmp/avar-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avar-0.0.7.tar", last modified: Mon May 13 22:04:43 2024, max compression
+gzip compressed data, was "avar-0.1.0.tar", last modified: Wed May 22 21:53:09 2024, max compression
```

## Comparing `avar-0.0.7.tar` & `avar-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-13 22:04:43.000876 avar-0.0.7/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-18 11:26:07.000000 avar-0.0.7/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     3779 2024-05-13 22:04:43.000819 avar-0.0.7/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     3311 2024-05-13 22:03:51.000000 avar-0.0.7/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2024-04-18 11:26:07.000000 avar-0.0.7/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      576 2024-05-13 22:04:43.001109 avar-0.0.7/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-13 22:04:42.998910 avar-0.0.7/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-13 22:04:42.999743 avar-0.0.7/src/avar/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-04-18 11:28:55.000000 avar-0.0.7/src/avar/__init__.py
--rwxr-xr-x   0 davidwoodburn   (501) staff       (20)    16465 2024-05-13 22:02:40.000000 avar-0.0.7/src/avar/avar.py
--rwxr-xr-x   0 davidwoodburn   (501) staff       (20)     1130 2024-05-13 21:07:17.000000 avar-0.0.7/src/avar/test_avar.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-13 22:04:43.000623 avar-0.0.7/src/avar.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     3779 2024-05-13 22:04:42.000000 avar-0.0.7/src/avar.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      265 2024-05-13 22:04:42.000000 avar-0.0.7/src/avar.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-13 22:04:42.000000 avar-0.0.7/src/avar.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       12 2024-05-13 22:04:42.000000 avar-0.0.7/src/avar.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        5 2024-05-13 22:04:42.000000 avar-0.0.7/src/avar.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-22 21:53:09.667864 avar-0.1.0/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-18 11:26:07.000000 avar-0.1.0/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     3853 2024-05-22 21:53:09.667814 avar-0.1.0/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     3385 2024-05-22 21:52:23.000000 avar-0.1.0/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2024-04-18 11:26:07.000000 avar-0.1.0/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      576 2024-05-22 21:53:09.668099 avar-0.1.0/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-22 21:53:09.665867 avar-0.1.0/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-22 21:53:09.666907 avar-0.1.0/src/avar/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       54 2024-04-18 11:28:55.000000 avar-0.1.0/src/avar/__init__.py
+-rwxr-xr-x   0 davidwoodburn   (501) staff       (20)    17403 2024-05-22 21:43:21.000000 avar-0.1.0/src/avar/avar.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-22 21:53:09.667639 avar-0.1.0/src/avar.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     3853 2024-05-22 21:53:09.000000 avar-0.1.0/src/avar.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      243 2024-05-22 21:53:09.000000 avar-0.1.0/src/avar.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-22 21:53:09.000000 avar-0.1.0/src/avar.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       12 2024-05-22 21:53:09.000000 avar-0.1.0/src/avar.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        5 2024-05-22 21:53:09.000000 avar-0.1.0/src/avar.egg-info/top_level.txt
```

### Comparing `avar-0.0.7/LICENSE.txt` & `avar-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `avar-0.0.7/PKG-INFO` & `avar-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avar
-Version: 0.0.7
+Version: 0.1.0
 Summary: Allan variance tools
 Home-page: https://gitlab.com/davidwoodburn/avar
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -96,7 +96,9 @@
 avar.noise(K, T, p)
 ```
 
 Generate a noise signal of length `K`, sampling period `T`, and parameters `p`.
 Parameter `p` is a `params` object (see the section on Ideal Allan Variance).
 
 This function returns the noise signal `y`.
+
+For flicker (bias-instability) noise, multiple, balanced FOGMs are used.
```

### Comparing `avar-0.0.7/README.md` & `avar-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -80,7 +80,9 @@
 avar.noise(K, T, p)
 ```
 
 Generate a noise signal of length `K`, sampling period `T`, and parameters `p`.
 Parameter `p` is a `params` object (see the section on Ideal Allan Variance).
 
 This function returns the noise signal `y`.
+
+For flicker (bias-instability) noise, multiple, balanced FOGMs are used.
```

### Comparing `avar-0.0.7/setup.cfg` & `avar-0.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = avar
-version = 0.0.7
+version = 0.1.0
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = Allan variance tools
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/avar
 classifiers =
```

### Comparing `avar-0.0.7/src/avar/avar.py` & `avar-0.1.0/src/avar/avar.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 __author__ = "David Woodburn"
 __license__ = "MIT"
-__date__ = "2024-05-13"
+__date__ = "2024-05-22"
 __maintainer__ = "David Woodburn"
 __email__ = "david.woodburn@icloud.com"
 __status__ = "Development"
 
 import numpy as np
 import scipy.optimize as opt
 
@@ -98,31 +98,33 @@
             delta = (Yc - 2*Yb + Yj - yj)/m
             v[:, n_tau] = np.mean(delta**2, axis=1)/2
 
     return v
 
 
 class params:
-    def __init__(self, vc, vfogm=None, tfogm=None):
+    def __init__(self, vc=None, vfogm=None, tfogm=None):
         """
         Parameters
         ----------
-        vc : (5,) np.ndarray
+        vc : (5,) np.ndarray, default None
             Variances of the five basic component noises: quantization, white,
             flicker, walk, and ramp. If `fogms` is not 0, the third element of `vc`
             will be zero. For any elements of `mask` which are `False`, the
             corresponding elements of `vc` will be zero.
         vfogm : (F,) np.ndarray, default None
             Array of FOGM variances.
         tfogm : (F,) np.ndarray, default None
             Array of FOGM time constants (s).
         """
 
         # Convert lists and tuples to arrays.
-        if isinstance(vc, (list, tuple)):
+        if vc is None:
+            vc = np.zeros(5)
+        elif isinstance(vc, (list, tuple)):
             vc = np.array(vc)
         if len(vc) != 5:
             raise ValueError("vc should be a 5-element array.")
         if isinstance(vfogm, (list, tuple)):
             vfogm = np.array(vfogm, dtype=float)
         elif isinstance(vfogm, (int, float)):
             vfogm = np.array([vfogm], dtype=float)
@@ -215,24 +217,23 @@
     ----------
     tau : (I,) np.ndarray
         Array of averaging periods (s).
     va : (I,) np.ndarray
         Array of Allan variances.
     mask : (5,) bool array_like, default None
         Array to mask which component variances to use. Left as `None`, no basic
-        component variances will be excluded. However, a positive value for
-        `fogms` will override the third element of the mask, regardless of
-        whether it is `True` or `False`.
+        component variances will be excluded. For any element equal to `False`,
+        the corresponding component noise will be excluded.
     fogms : int, default 0
         The maximum number of first-order, Gauss-Markov (FOGM) noise components
         to try to fit to the data. This is the maximum number, not the required
         number. The best fit might not use any.
     tol : float, default 0.007
-        Normalized mean absolute error tolerance to meet as various combinations
-        of the component noises are applied to the fitting.
+        Early-exit, minimum normalized mean absolute error (NMAE). If the NMAE
+        falls below this tolerance the search will end early.
     vtol : float, default 0.0
         Minimum allowed variance for fitted component noise variances.
 
     Returns
     -------
     vf : (I,) np.ndarray
         Fitted Allan variance curve.
@@ -242,15 +243,15 @@
     Notes
     -----
     This function will iterate through the various permutations of component
     noises, starting with 0 FOGMs. If a fit satisfies the specified `tol`, the
     search will end. Otherwise, the best fit will be used.
     """
 
-    def fopt(k, H, M, T, va):
+    def fopt(k, H, M, T, va, vtol):
         """
         Parameters
         ----------
         k : (B + 2*F,) np.ndarray
             Array of variables to tune for, starting with some `B` basic noise
             component variances followed by `F` pairs of FOGM variances and time
             constants.
@@ -264,34 +265,42 @@
             Array of Allan variances to fit.
         """
 
         # Get the number of basic components and FOGM components.
         B = H.shape[1]
         F = (len(k) - B)//2
 
+        # Zero components below tolerance.
+        k[:Bp] = np.where(k[:Bp] > vtol, k[:Bp], 0)
+        k[Bp::2] = np.where(k[Bp::2] > vtol, k[Bp::2], 0)
+        if np.sum(k[:Bp]) + np.sum(k[Bp::2]) == 0:
+            return va*0 + np.inf
+
         # Initialize the normalized fit with the basic components.
         vfn = H/va[:, None] @ np.abs(k[:B])
 
-        # Add to the fit each of the FOGM components.
+        # Add to the fit each of the FOGM components (normalized by the real
+        # Allan variance curve, `va`).
         for f in range(F):
-            v = abs(k[B + 2*f])
-            t = abs(k[B + 2*f + 1])
+            v = abs(k[B + 2*f]) # FOGM variances
+            t = abs(k[B + 2*f + 1]) # FOGM time constants
             q = np.exp(-T/t)
-            vfn += (1/va)*(v/M**2)*(M*(1 - q)**2 + 2*q*M*(1 - q)
-                    - 2*q*(1 - q**M) - q*(1 - q**M)**2)/(1 - q)**2
+            a = 1 - q
+            a2 = a**2
+            b = 1 - q**M
+            vfn += (v/va)*(1/M**2)*(M*a2 + 2*q*M*(1 - q) - 2*q*b - q*b**2)/a2
 
+        # The normalized variance should be compared to 1.
         return vfn - 1
 
     # Adjust the mask.
     if mask is None:
         mask = np.ones(5, dtype=bool)
     if isinstance(mask, (list, tuple)):
         mask = np.array(mask, dtype=bool)
-    if fogms > 0:
-        mask[2] = False
 
     # Build the basic component Allan variances.
     qnt = 3/(tau**2)
     wht = 1/tau
     flk = 2*np.log(2)/np.pi + 0*tau
     bwn = tau/3
     rmp = (tau**2)/2
@@ -299,29 +308,31 @@
     H = H5[:, mask]
 
     # Get the dimensions.
     B = H.shape[1] # number of basic components to consider
 
     # Get the range of averaging periods.
     T = tau[0] # sampling period
-    talg = np.log10(T)
-    tblg = np.log10(tau[-1])
+    ta_lg = np.log10(T)
+    tb_lg = np.log10(tau[-1])
 
     # Define the reused arrays.
     I = len(va)
     OI = np.ones(I)
     M = tau/T # averaging window sizes
 
     # Initialize the outputs.
     vf = np.zeros(I)
     p = params(np.zeros(5), np.zeros(fogms), np.zeros(fogms))
 
     # Define the NMAE components.
     va_lg = np.log10(va)
     range_lg = np.max(va_lg) - np.min(va_lg)
+    if range_lg == 0:
+        range_lg = 1.0
     nmae_min = np.inf
 
     # Initialize the metrics
     fit_metrics.init((2**B - 1)*(fogms + 1))
 
     # Estimate the component variances.
     for F in range(fogms + 1): # the number of possible FOGMs
@@ -338,32 +349,32 @@
 
             # Optimize for this permutation.
             if F == 0: # no FOGMs
                 try: # This can fail.
                     k = opt.nnls(Hp/va[:, None], OI)[0]
                 except ValueError or RuntimeError:
                     continue
-                # Remove components below tolerance.
+                # Zero components below tolerance.
                 k = np.where(k > vtol, k, 0)
                 if np.sum(k) == 0:
                     continue
                 # Get the fitted Allan variance.
                 vfp = Hp @ k
             else: # some FOGMs
                 try: # This can fail.
                     # Initialize the parameters, spacing out the FOGM time
-                    # constants.
+                    # constants and neglecting the ends.
                     k = np.ones(Bp + 2*F)
-                    k[Bp + 1::2] = np.logspace(talg, tblg, F + 2)[1:-1]
+                    k[Bp + 1::2] = np.logspace(ta_lg, tb_lg, F + 2)[1:-1]
                     # Optimize.
                     k = np.abs(opt.leastsq(fopt, k,
-                            args=(Hp, M, T, va), maxfev=1000)[0])
+                            args=(Hp, M, T, va, vtol), maxfev=1000)[0])
                 except ValueError or RuntimeError:
                     continue
-                # Remove components below tolerance.
+                # Zero components below tolerance.
                 k[:Bp] = np.where(k[:Bp] > vtol, k[:Bp], 0)
                 k[Bp::2] = np.where(k[Bp::2] > vtol, k[Bp::2], 0)
                 if np.sum(k[:Bp]) + np.sum(k[Bp::2]) == 0:
                     continue
                 # Get the fitted Allan variance.
                 vfp = Hp @ np.abs(k[:Bp])
                 for f in range(F):
@@ -412,15 +423,15 @@
     variance analysis and any first-order, Gauss-Markov (FOGM) noises specified.
     The basic component noises are generated as the following:
 
         Type            Implementation
         ------------    ---------------------------------------
         quantization    differentiated white, Gaussian noise
         white           white, Gaussian noise
-        flicker         first-order, Gauss-Markov (FOGM) noise
+        flicker         multiple, balanced FOGM noises
         walk            integrated white, Gaussian noise
         ramp            doubly integrated white, Gaussian noise
 
     Parameters
     ----------
     K : int
         Number of samples.
@@ -444,16 +455,18 @@
     in order to get the Allan variance of this generated noise to match the
     expected ideal Allan variance magnitude, the amplitude of the noise signal
     is scaled according to the number of samples.
 
     The scaling factors for the quantization and ramp noises have been empiric-
     ally, not analytically, derived. However, given their simplicity (`1` and
     `sqrt(2)`, respectively) and the very small errors between the average Allan
-    variance curves of 10 thousand Monte-Carlo samples of noise and the ideal
-    Allan variance curve, it seems they are correct.
+    variance curves of 10 000 Monte-Carlo samples of noise and the ideal Allan
+    variance curve, it seems they are correct.
+
+    The flicker noise is approximated by multiple FOGM noises in parallel.
     """
 
     # Initialize the noise array.
     y = np.zeros(K)
 
     # Quantization noise
     if p.vc[0] != 0:
@@ -461,23 +474,34 @@
         y += np.sqrt(p.vc[0])*np.diff(w)/T
 
     # White noise
     if p.vc[1] != 0:
         w = np.random.randn(K)
         y += np.sqrt(p.vc[1]/T)*w
 
-    # Bias instability (flicker)
-    #if p.vc[2] != 0:
-    #    ka = np.exp(-T/taub)
-    #    kb = np.sqrt(p.vc[2]*(1 - np.exp(-2*T/taub)))
-    #    eta = kb*np.random.randn(K)
-    #    x = np.sqrt(p.vc[2])*np.random.randn() # state
-    #    for k in range(K):
-    #        y[k] += x
-    #        x = ka*x + eta[k]
+    # Bias instability (flicker) using multiple FOGMs
+    if p.vc[2] != 0:
+        # Get the tau values.
+        a = np.log10(T)     # exponent of minimum x
+        b = np.log10(K*T/2) # exponent of maximum x
+        N = int((b - a - 0.28)/0.784) + 1 # number of FOGMs
+        ee = a + 0.28 + 0.784*np.arange(N)
+        tt = (5/(3*np.pi)) * 10**ee
+
+        # Get the adjusted variance.
+        v = np.pi/(2*np.exp(1)) * p.vc[2]
+
+        # Build the noise.
+        ka = np.exp(-T/tt)
+        kb = np.sqrt(v*(1 - np.exp(-2*T/tt)))
+        eta = kb[:, None]*np.random.randn(N, K)
+        x = np.sqrt(v)*np.random.randn(N) # state
+        for k in range(K):
+            y[k] += np.sum(x)
+            x = ka*x + eta[:, k]
 
     # Random walk noise
     if p.vc[3] != 0:
         w = np.random.randn(K)
         y += np.cumsum(np.sqrt(p.vc[3]*T)*w)
 
     # Ramp noise
```

### Comparing `avar-0.0.7/src/avar.egg-info/PKG-INFO` & `avar-0.1.0/src/avar.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avar
-Version: 0.0.7
+Version: 0.1.0
 Summary: Allan variance tools
 Home-page: https://gitlab.com/davidwoodburn/avar
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -96,7 +96,9 @@
 avar.noise(K, T, p)
 ```
 
 Generate a noise signal of length `K`, sampling period `T`, and parameters `p`.
 Parameter `p` is a `params` object (see the section on Ideal Allan Variance).
 
 This function returns the noise signal `y`.
+
+For flicker (bias-instability) noise, multiple, balanced FOGMs are used.
```

