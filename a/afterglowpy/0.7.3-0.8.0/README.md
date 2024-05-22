# Comparing `tmp/afterglowpy-0.7.3.tar.gz` & `tmp/afterglowpy-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afterglowpy-0.7.3.tar", last modified: Thu Apr 29 22:23:17 2021, max compression
+gzip compressed data, was "afterglowpy-0.8.0.tar", last modified: Wed May 22 18:58:01 2024, max compression
```

## Comparing `afterglowpy-0.7.3.tar` & `afterglowpy-0.8.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 22:23:17.149365 afterglowpy-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2021-04-29 22:22:50.000000 afterglowpy-0.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6481 2021-04-29 22:23:17.145365 afterglowpy-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4923 2021-04-29 22:22:50.000000 afterglowpy-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 22:23:17.145365 afterglowpy-0.7.3/afterglowpy/
--rw-r--r--   0 runner    (1001) docker     (121)     2372 2021-04-29 22:22:50.000000 afterglowpy-0.7.3/afterglowpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3074 2021-04-29 22:22:50.000000 afterglowpy-0.7.3/afterglowpy/cocoon.py
--rw-r--r--   0 runner    (1001) docker     (121)    23423 2021-04-29 22:22:50.000000 afterglowpy-0.7.3/afterglowpy/flux.py
--rw-r--r--   0 runner    (1001) docker     (121)    45162 2021-04-29 22:22:50.000000 afterglowpy-0.7.3/afterglowpy/integrate.c
--rw-r--r--   0 runner    (1001) docker     (121)     9276 2021-04-29 22:22:50.000000 afterglowpy-0.7.3/afterglowpy/integrate.h
--rw-r--r--   0 runner    (1001) docker     (121)    12908 2021-04-29 22:22:50.000000 afterglowpy-0.7.3/afterglowpy/interval.c
--rw-r--r--   0 runner    (1001) docker     (121)     3654 2021-04-29 22:22:50.000000 afterglowpy-0.7.3/afterglowpy/interval.h
--rw-r--r--   0 runner    (1001) docker     (121)    38495 2021-04-29 22:22:50.000000 afterglowpy-0.7.3/afterglowpy/jetmodule.c
--rw-r--r--   0 runner    (1001) docker     (121)    11703 2021-04-29 22:22:50.000000 afterglowpy-0.7.3/afterglowpy/offaxis_struct.h
--rw-r--r--   0 runner    (1001) docker     (121)    79229 2021-04-29 22:22:50.000000 afterglowpy-0.7.3/afterglowpy/offaxis_struct_funcs.c
--rw-r--r--   0 runner    (1001) docker     (121)    16115 2021-04-29 22:22:50.000000 afterglowpy-0.7.3/afterglowpy/shockEvolution.c
--rw-r--r--   0 runner    (1001) docker     (121)      834 2021-04-29 22:22:50.000000 afterglowpy-0.7.3/afterglowpy/shockEvolution.h
--rw-r--r--   0 runner    (1001) docker     (121)     6487 2021-04-29 22:22:50.000000 afterglowpy-0.7.3/afterglowpy/shockmodule.c
--rw-r--r--   0 runner    (1001) docker     (121)       91 2021-04-29 22:22:50.000000 afterglowpy-0.7.3/afterglowpy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 22:23:17.145365 afterglowpy-0.7.3/afterglowpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6481 2021-04-29 22:23:17.000000 afterglowpy-0.7.3/afterglowpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      592 2021-04-29 22:23:17.000000 afterglowpy-0.7.3/afterglowpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-29 22:23:17.000000 afterglowpy-0.7.3/afterglowpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-04-29 22:23:17.000000 afterglowpy-0.7.3/afterglowpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-04-29 22:23:17.000000 afterglowpy-0.7.3/afterglowpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-04-29 22:22:50.000000 afterglowpy-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-29 22:23:17.149365 afterglowpy-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2322 2021-04-29 22:22:50.000000 afterglowpy-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 22:23:17.145365 afterglowpy-0.7.3/test/
--rw-r--r--   0 runner    (1001) docker     (121)    20114 2021-04-29 22:22:50.000000 afterglowpy-0.7.3/test/test_flux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:58:01.160007 afterglowpy-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-22 18:57:57.000000 afterglowpy-0.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-22 18:57:57.000000 afterglowpy-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-22 18:58:01.156007 afterglowpy-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-05-22 18:57:57.000000 afterglowpy-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:58:01.156007 afterglowpy-0.8.0/afterglowpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-22 18:57:57.000000 afterglowpy-0.8.0/afterglowpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-22 18:57:57.000000 afterglowpy-0.8.0/afterglowpy/cocoon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24270 2024-05-22 18:57:57.000000 afterglowpy-0.8.0/afterglowpy/flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45788 2024-05-22 18:57:57.000000 afterglowpy-0.8.0/afterglowpy/integrate.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9289 2024-05-22 18:57:57.000000 afterglowpy-0.8.0/afterglowpy/integrate.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12952 2024-05-22 18:57:57.000000 afterglowpy-0.8.0/afterglowpy/interval.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-22 18:57:57.000000 afterglowpy-0.8.0/afterglowpy/interval.h
+-rw-r--r--   0 runner    (1001) docker     (127)    43852 2024-05-22 18:57:57.000000 afterglowpy-0.8.0/afterglowpy/jetmodule.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13016 2024-05-22 18:57:57.000000 afterglowpy-0.8.0/afterglowpy/offaxis_struct.h
+-rw-r--r--   0 runner    (1001) docker     (127)   103635 2024-05-22 18:57:57.000000 afterglowpy-0.8.0/afterglowpy/offaxis_struct_funcs.c
+-rw-r--r--   0 runner    (1001) docker     (127)    25015 2024-05-22 18:57:57.000000 afterglowpy-0.8.0/afterglowpy/shockEvolution.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-22 18:57:57.000000 afterglowpy-0.8.0/afterglowpy/shockEvolution.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-22 18:57:57.000000 afterglowpy-0.8.0/afterglowpy/shockmodule.c
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-22 18:57:57.000000 afterglowpy-0.8.0/afterglowpy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:58:01.156007 afterglowpy-0.8.0/afterglowpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-22 18:58:01.000000 afterglowpy-0.8.0/afterglowpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-22 18:58:01.000000 afterglowpy-0.8.0/afterglowpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 18:58:01.000000 afterglowpy-0.8.0/afterglowpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-22 18:58:01.000000 afterglowpy-0.8.0/afterglowpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 18:58:01.000000 afterglowpy-0.8.0/afterglowpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-22 18:57:57.000000 afterglowpy-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 18:58:01.160007 afterglowpy-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-22 18:57:57.000000 afterglowpy-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:58:01.156007 afterglowpy-0.8.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    20114 2024-05-22 18:57:57.000000 afterglowpy-0.8.0/test/test_flux.py
```

### Comparing `afterglowpy-0.7.3/README.md` & `afterglowpy-0.8.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 # Numeric GRB Afterglow models
 
-A Python 3 module to calculate GRB afterglow light curves and spectra. Details of the methods can be found in [Ryan et al 2019](https://arxiv.org/abs/1909.11691). Builds on [van Eerten & MacFadyen 2010](https://arxiv.org/abs/1006.5125) and [van Eerten 2018](https://arxiv.org/abs/1801.01848).  This code is under active development.
+A Python 3 module to calculate GRB afterglow light curves and spectra. Details of the methods can be found in [Ryan et al 2020](https://ui.adsabs.harvard.edu/abs/2020ApJ...896..166R/abstract). Builds on [van Eerten & MacFadyen 2010](https://arxiv.org/abs/1006.5125) and [van Eerten 2018](https://arxiv.org/abs/1801.01848).  This code is under active development.
 
 Documentation available at <https://afterglowpy.readthedocs.io/>
 
 ## Attribution
 
-If you use this code in a publication, please refer to the package by name and cite "Ryan, G., van Eerten, H., Piro, L. and Troja, E., 2019, arXiv:1910.11691" [arXiv link](https://arxiv.org/abs/1909.11691).
+If you use this code in a publication, please refer to the package by name and cite "Ryan, G., van Eerten, H., Piro, L. and Troja, E., 2020, Astrophysical Journal *896*, 166 (2020)" [arXiv link](https://arxiv.org/abs/1909.11691).
+
+## Acknowledgements
+
+This work is funded in part by the European Union’s Horizon 2020 Programme under the AHEAD2020 project (grant agreement n. 871158).
 
 ## Features
 
 _afterglowpy_ computes synchrotron emission from the forward shock of a relativistic blast wave.  It includes:
 - Fully trans-relativistic shock evolution through a constant density medium.
 - On-the-fly integration over the equal-observer-time slices of the shock surface.
 - Approximate prescription for jet spreading.
 - Arbitrary viewing angles.
 - Angularly structured jets, ie. E(&theta;)
 - Spherical velocity-stratified outflows, ie. E(u)
 - Counter-jet emission.
+- Deep Newtonian emission.
+- Image moments suitable for astrometry: centroid position and image size.
 
 It has limited support (these should be considered experimental) for:
 - Initial energy injection
 - Inverse comption spectra
-- Spatially-resolved intensity maps
 - Early coasting phase
 
 It does not include (yet):
 - External wind medium, ie. n &prop; r<sup>-2</sup>
 - Synchrotron self-absorbtion
 - Reverse shock emission
 
@@ -43,58 +48,41 @@
 If you are working on a local copy of this repo and would like to install from source, you can the run the following from the top level directory of the project.
 ```bash
 $ pip install -e .
 ```
 
 ## Using
 
-**This interface will be updated to be more sensible in the VERY near future**
-
 In your python code, import the library with `import afterglowpy as grb`.  
 
-The main function of interest is`grb.fluxDensity(t, nu, jetType, specType, *pars, **kwargs)`.  See `tests/plotLC.py` for a simple example.
+The main function of interest is`grb.fluxDensity(t, nu, **kwargs)`.  See `examples/plotLightCurve.py` for a simple example.
 
-`jetType` can be -1 (top hat), 0 (Gaussian), 1 (Power Law w/ core), 2 (Gaussian w/ core), 3 (Cocoon), or 4 (Smooth Power Law).  
+For jet-like afterglows there are up to 13 required keyword arguments:
 
-`specType` can be 0 (global cooling time, no inverse compton) or 1 (global cooling time, inverse compton).
+- `jetType` an integer code setting the jet structure. It can be `grb.jet.TopHat`, `grb.jet.Gaussian`, `grb.jet.PowerLawCore`, `grb.jet.GaussianCore`, `grb.jet.Spherical`, or `grb.jet.PowerLaw`.  
+- `specType` an integer code specifying flags for the emissivity function and spectrum. Can be `grb.jet.SimpleSpec` (basic spectrum with &nu;<sub>m</sub> and &nu;<sub>c</sub>), `grb.jet.DeepNewtonian`, `grb.jet.ICCooling` (simple inverse Compton effects on the cooling frequency, experimental).
+- `thetaObs` viewing angle in radians
+- `E0` on-axis isotropic equivalent energy in erg
+- `thetaCore` half-width of the jet core in radians (jetType specific)
+- `thetaWing` "wing" truncation angle of the jet, in radians
+- `b` power for power-law structure, &theta;<sup>-b</sup>
+- `n0` Number density of ISM, in cm<sup>-3</sup>
+- `p` Electron distribution power-law index (p>2)
+- `epsilon_e` Thermal energy fraction in electrons
+- `epsilon_B` Thermal energy fraction in magnetic field
+- `xi_N` Fraction of electrons that get accelerated
+- `d_L` Luminosity distance in cm
 
-For jet-like afterglows (`jetTypes` -2, -1, 0, 1, 2, and 4) `pars` has 14 positional arguments:
-- `0 thetaV` viewing angle in radians
-- `1 E0` on-axis isotropic equivalent energy in erg
-- `2 thetaC` half-width of the jet core in radians (jetType specific)
-- `3 thetaW` "wing" truncation angle of the jet, in radians
-- `4 b` power for power-law structure, &theta;<sup>-b</sup>
-- `5 L0` Fiducial luminosity for energy injection, in erg/s, typically 0.
-- `6 q` Temporal power-law index for energy injection, typically 0.
-- `7 ts` Fiducial time-scale for energy injection, in seconds, typically 0.
-- `8 n0` Number density of ISM, in cm<sup>-3</sup>
-- `9 p` Electron distribution power-law index (p>2)
-- `10 epsilon_e` Thermal energy fraction in electrons
-- `11 epsilon_B` Thermal energy fraction in magnetic field
-- `12 xi_N` Fraction of electrons that get accelerated
-- `13 d_L` Luminosity distance in cm
-
-For cocoon-like afterglows (`jetType` 3) `pars` has 14 positional arguments:
-- `0 umax` Initial maximum outflow 4-velocity
-- `1 umin` Minium outflow 4-velocity
-- `2 Ei` Fiducial energy in velocity distribution, E(>u) = E<sub>i</sub>  u<sup>-k</sup>.
-- `3 k` Power-law index of energy velocity distribution  
-- `4 Mej` Mass of material at `umax' in solar masses
-- `5 L0` Fiducial luminosity for energy injection, in erg/s, typically 0.
-- `6 q` Temporal power-law index for energy injection, typically 0.
-- `7 ts` Fiducial time-scale for energy injection, in seconds, typically 0.
-- `8 n0` Number density of ISM, in cm<sup>-3</sup>
-- `9 p` Electron distribution power-law index (p>2)
-- `10 epsilon_e` Thermal energy fraction in electrons
-- `11 epsilon_B` Thermal energy fraction in magnetic field
-- `12 xi_N` Fraction of electrons that get accelerated
-- `13 d_L` Luminosity distance in cm
-
-Keyword arguments are:
+Optional keyword arguments for all models are:
 - `z` redshift (defaults to 0)
+- `spread` boolean (defaults to True), whether to allow the jet to spread.
+- `counterjet` boolean (defaults to False), whether to include the counterjet
+- `moment` array (integer dtype, same shape as t and nu) which sky moment to compute.
+- `L0` Fiducial luminosity for energy injection, in erg/s, default 0.0.
+- `q` Temporal power-law index for energy injection, default 0.0.
+- `ts` Fiducial time-scale for energy injection, in seconds, default 0.
 - `tRes` time resolution of shock-evolution scheme, number of sample points per decade in time
 - `latRes` latitudinal resolution for structured jets, number of shells per `thetaC`
 - `rtol` target relative tolerance of flux integration
-- `spread` boolean (defaults to True), whether to allow the jet to spread.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `afterglowpy-0.7.3/afterglowpy/__init__.py` & `afterglowpy-0.8.0/afterglowpy/__init__.py`

 * *Files identical despite different names*

### Comparing `afterglowpy-0.7.3/afterglowpy/cocoon.py` & `afterglowpy-0.8.0/afterglowpy/cocoon.py`

 * *Files 15% similar despite different names*

```diff
@@ -41,15 +41,18 @@
     r = ar[ia]*math.pow(te/ate[ia], math.log(ar[ib]/ar[ia])
                         / math.log(ate[ib]/ate[ia]))
 
     g = math.sqrt(u*u+1)
 
     us = 4*u*g / math.sqrt(8*u*u+9)
 
-    em = jet.emissivity(nu, r, mu, te, u, us, n0, p, epsE,
+    rho0 = n0 * mp
+    Msw = rho0 * 4.0/3.0 * np.pi * r**3
+
+    em = jet.emissivity(nu, r, mu, te, u, us, rho0, Msw, p, epsE,
                         epsB, ksiN, specType)
 
     return 2*np.pi * em
 
 
 def fluxDensity(t, nu, **kwargs):
 
@@ -74,14 +77,20 @@
     ts = kwargs['ts'] if 'ts' in kwargs else 0.0
    
     # Numerical integration variables
     rtol = kwargs['rtol'] if 'rtol' in kwargs else 1.0e-3
     tRes = kwargs['tRes'] if 'tRes' in kwargs else 1000
     latRes = kwargs['latRes'] if 'latRes' in kwargs else 0
 
+    # Environment Variables
+    envType = kwargs['envType'] if 'envType' in kwargs else jet.EnvISM
+    R0Env = kwargs['R0Env'] if 'R0Env' in kwargs else 1.0e18
+    kEnv = kwargs['kEnv'] if 'kEnv' in kwargs else 0.0
+    rho1Env = kwargs['rho1Env'] if 'rho1Env' in kwargs else 1.0
+
     rho0 = mp * n0
     Mej = MFast_solar * Msun
     u0 = uMax
     g0 = math.sqrt(1+u0*u0)
     bes0 = 4*u0*g0 / (4*u0*u0+3)
     Rd = math.pow(9*g0*g0*Mej / (4*np.pi*(g0+1)*(4*u0*u0+3)*rho0), 1./3.)
     td = Rd / (bes0 * c)
@@ -95,15 +104,17 @@
     r0 = bes0*c*t0
 
     # Vej0 = 4.0/3.0*np.pi*r0*r0*r0
 
     ate = np.logspace(math.log10(t0), math.log10(t1), num=NT, base=10.0)
 
     ar, au = shock.shockEvolRK4(ate, r0, uMax,
-                                MFast_solar*Msun, rho0, Er, k, uMin, L0, q, ts)
+                                MFast_solar*Msun,
+                                envType, rho0, R0Env, kEnv, rho1Env,
+                                Er, k, uMin, L0, q, ts)
 
     P = np.zeros(t.shape)
 
     wopts = None
 
     for i in range(len(t)):
         amu = c * (ate - t[i]) / ar
```

### Comparing `afterglowpy-0.7.3/afterglowpy/flux.py` & `afterglowpy-0.8.0/afterglowpy/flux.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,16 +42,20 @@
         Frequency of flux in observer frame, measured in Hz, same size as t.
     jetType : int
         Code for type of jet. Model codes are available in ``afterglowpy.jet``
         and include: ``jet.TopHat``, ``jet.Cone``, ``jet.Gaussian``,
         ``jet.PowerLaw``, ``jet.GaussianCore``, ``jet.PowerLawCore``, and
         ``jet.Spherical``.
     specType : int
-        Code for type of spectrum.  Options are: 0 broken power law
-        (Ryan+ 2020), 1 broken power law w/ inverse Compton cooling. Default: 0
+        Flags for type of spectrum/emissivity function. Spectrum flags are
+        available in ``afterglowpy.jet`` and include: ``jet.SimpleSpec``
+        broken power law with nu_m and nu_c (Ryan+ 2020, default),
+        ``jet.ICCooling`` simple inverse-compton contribution to cooling,
+        ``jet.DeepNewtonian`` better handling of late-time emission when 
+        some electrons become non-relativistic (e.g. Sironi+ 2013).
     thetaObs : float
         Viewing angle in radians. Jet models only.
     E0: float
         Isotropic-equivalent energy along the jet axis in ergs. Jet models
         only.
     thetaCore: float
         Half opening angle of jet core in radians. Jet models only.
@@ -106,14 +110,22 @@
     Other Parameters
     ----------------
 
     spread : {True, False}, optional
         Whether to include jet spreading. Defaults to True.
     counterjet : {'True', 'False'}, optional
         Whether to include counterjet emission. Defaults to False.
+    moment : array_like, optional
+        An integer array the same shape as the larger of `t` or `nu`. Selects
+        which image moment to compute. Observer's sky is on the x-y plane, 
+        with the jet propagating in the x-direction.  Moments are in terms of
+        proper length (in cm) Options are: `jet.MOM_0` Flux, default,
+        `jet.MOM_X` x^1 moment, `jet.MOM_Y` y^1 moment, `jet.MOM_Z` z^1 moment,
+        `jet.MOM_XX` x^2 moment, `jet.MOM_YY` y^2 moment, `jet.MOM_ZZ`, z^2
+        moment, `jet.MOM_XY` x^1 y^1, `jet.MOM_YZ`, `jet.MOM_XZ`.
     tRes : int, optional
         Time resolution, number of points per decade in t, for shock evolution.
         Defaults to 1000.
     latRes : int, optional
         Lateral resolution of structured jet, number of conical sections per
         thetaCore-sized interval. Defaults to 5.
     intType : int, optional
@@ -146,50 +158,53 @@
 
     ValueError
         If t, nu are the wrong shape or arguments take illegal values.
     """
 
     argsDict = parseArgs(args, kwargs)
 
+    # Check Arguments, will raise ValueError if args are bad
     t, nu = checkTNu(t, nu)
+    
 
     jetType = argsDict['jetType']
 
     if jetType == jet.Spherical:
         checkCocoonArgs(**argsDict)
     else:
         checkJetArgs(**argsDict)
 
+
     # arguments are good, full steam ahead!
     z = argsDict.pop('z') if 'z' in argsDict else 0.0
 
     tz = t / (1+z)
     nuz = nu * (1+z)
 
+
     # Default spreading method
     if 'spread' in argsDict:
         if argsDict['spread'] == True:
             if jetType == -2 and 'thetaCoreGlobal' in argsDict:
                 argsDict['spread'] = 8
             else:
                 argsDict['spread'] = 7
 
-    # Intercept background luminosities
     # This was a bad idea to add to this function, but is kept for 
     # backwards compatibility. Please don't use these.
     LR = argsDict.pop('LR') if 'LR' in argsDict else 0.0
     LO = argsDict.pop('LO') if 'LO' in argsDict else 0.0
     LX = argsDict.pop('LX') if 'LX' in argsDict else 0.0
     tAdd = argsDict.pop('tAdd') if 'tAdd' in argsDict else 0.0
 
     # timeA = time.time()
 
     Fnu = np.empty(tz.shape)
 
-    if argsDict['jetType'] == jet.Spherical:
+    if jetType == jet.Spherical:
         Fnu.flat[:] = cocoon.fluxDensity(tz.flat, nuz.flat, **argsDict)
     else:
         Fnu.flat[:] = jet.fluxDensity(tz.flat, nuz.flat, **argsDict)
     # timeB = time.time()
     # print("Eval took: {0:f} s".format(timeB - timeA))
 
     
@@ -209,15 +224,15 @@
     if LX > 0.0:
         xry = (nuz >= 100*cocoon.eV2Hz) & (tz > tAdd)  # xray > 100eV
         Lnu = LX / (9.7e3 * cocoon.eV2Hz)  # 9.7 keV bandwidth
         Fnu[xry] += Lnu*L_to_flux
 
     # K-correct the flux
     Fnu *= 1+z
-
+    
     return Fnu
 
 
 def intensity(theta, phi, t, nu, *args, **kwargs):
     """
     Compute the intensity I_nu of a GRB afterglow.
 
@@ -474,18 +489,15 @@
             raise ValueError(msg)
 
     return theta, phi, t, nu
 
 
 def checkJetArgs(**argsDict):
 
-    for _, x in argsDict.items():
-        if not np.isfinite(x):
-            raise ValueError("All parameters must be finite")
-
+    return
 
     jetType = argsDict['jetType']
     specType = argsDict['specType']
 
     theta_obs = argsDict['thetaObs']
     E0 = argsDict['E0']
     theta_c = argsDict['thetaCore']
@@ -665,25 +677,22 @@
                   + " arguments instead, see documentation for details.",
                   FutureWarning)
 
     # Now for the fun part
 
     jetKeys = ['jetType', 'specType', 'thetaObs', 'E0', 'thetaCore',
                'thetaWing', 'b', 'L0', 'q', 'ts', 'n0', 'p', 'epsilon_e',
-               'epsilon_B', 'xi_N', 'd_L', 'g0', 'LR', 'LO', 'LX', 'tAdd', 'z']
+               'epsilon_B', 'xi_N', 'd_L', 'g0', 'LR', 'LO', 'LX', 'tAdd', 'z',
+               'envType', 'R0Env', 'kEnv', 'rho1Env']
     sphKeys = ['jetType', 'specType', 'uMax', 'uMin', 'Er',
                'k', 'MFast_solar', 'L0', 'q', 'ts', 'n0', 'p', 'epsilon_e',
-               'epsilon_B', 'xi_N', 'd_L', 'g0', 'LR', 'LO', 'LX', 'tAdd', 'z']
+               'epsilon_B', 'xi_N', 'd_L', 'g0', 'LR', 'LO', 'LX', 'tAdd', 'z',
+               'envType', 'R0Env', 'kEnv', 'rho1Env']
 
     jetType = args[0]
 
     if jetType == jet.Spherical:
         argsDict.update(zip(sphKeys, args))
     else:
         argsDict.update(zip(jetKeys, args))
 
     return argsDict
-
-
-
-
-
```

### Comparing `afterglowpy-0.7.3/afterglowpy/integrate.c` & `afterglowpy-0.8.0/afterglowpy/integrate.c`

 * *Files 2% similar despite different names*

```diff
@@ -343,20 +343,23 @@
 
     return I;
 }
 
 double cadre_adapt(double (*f)(double, void *), double xa, double xb, int Nmax,
                   double atol, double rtol, void *args, int *Neval,
                   double *eps, int verbose, int (*errf)(void *),
-                  double *pfa, double *pfb)
+                  double *pfa, double *pfb, Mesh9 *mout)
 {
     double I = m9_adapt(f, xa, xb, Nmax, cadreInitInterval,
                         cadreProcessInterval, cadreSplitInterval,
-                        atol, rtol, args, Neval, eps, NULL, verbose, errf,
+                        atol, rtol, args, Neval, eps, mout, verbose, errf,
                         pfa, pfb);
+
+    
+
     return I;
 }
 
 double gk49_adapt(double (*f)(double, void *), double xa, double xb, int Nmax,
                   double atol, double rtol, void *args, int *Neval,
                   double *eps, int verbose, int (*errf)(void *))
 {
@@ -1460,22 +1463,28 @@
 
     Interval9 i = {.a=xa, .b=xb, .I=0, .err=0,
                    .fa=0, .fll=0, .fl=0, .flr=0, .fm=0,
                    .frl=0, .fr=0, .frr=0, .fb=0, .refinement=0};
     int n = initInterval(f, args, &i, errf, pfa, pfb);
     if(errf(args))
     {
-        mesh9Free(&m);
+        if(mout == NULL)
+            mesh9Free(&m);
+        else
+            mout = &m;
         return 0.0;
     }
 
     n += processInterval(f, args, &i, errf);
     if(errf(args))
     {
-        mesh9Free(&m);
+        if(mout == NULL)
+            mesh9Free(&m);
+        else
+            mout = &m;
         return 0.0;
     }
 
     mesh9Insert(&m, &i);
 
     double I = i.I;
     double err = i.err;
@@ -1504,15 +1513,18 @@
         {
             double oldI = i.I;
             double olderr = i.err;
 
             n += processInterval(f, args, &i, errf);
             if(errf(args))
             {
-                mesh9Free(&m);
+                if(mout == NULL)
+                    mesh9Free(&m);
+                else
+                    mout = &m;
                 return 0.0;
             }
             mesh9Insert(&m, &i);
 
             err += i.err - olderr;
             I += i.I - oldI;
 
@@ -1522,15 +1534,18 @@
         else
         {
             Interval9 i1;
             Interval9 i2;
             n += splitInterval(f, args, &i, &i1, &i2, errf);
             if(errf(args))
             {
-                mesh9Free(&m);
+                if(mout == NULL)
+                    mesh9Free(&m);
+                else
+                    mout = &m;
                 return 0.0;
             }
             mesh9Insert(&m, &i1);
             mesh9Insert(&m, &i2);
             num_intervals++;
             
             err += i1.err + i2.err - i.err;
@@ -1564,14 +1579,27 @@
 
     if(eps != NULL)
     {
         err = mesh9TotalError(&m);
         *eps = err;
     }
 
+    // DEBUG DELETE LATER
+    /*
+    char *meshStr;
+    mesh9Write(&m, &meshStr);
+    FILE *fp = fopen("afterglowpy_int_dump.txt", "w");
+    fprintf(fp, "%s\n", meshStr);
+    int idx;
+    for(idx=0; idx<m.N; idx++)
+        interval9Write(m.heap+idx, fp);
+    fclose(fp);
+    free(meshStr);
+    */
+
     if(mout == NULL)
         mesh9Free(&m);
     else
         *mout = m;
 
     return I;
 }
```

### Comparing `afterglowpy-0.7.3/afterglowpy/integrate.h` & `afterglowpy-0.8.0/afterglowpy/integrate.h`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 double hybrid_adapt(double (*f)(double, void *), double xa, double xb, int Nmax,
                   double atol, double rtol, void *args, int *Neval,
                   double *eps, int verbose, int (*errf)(void *),
                   double *pfa, double *pfb);
 double cadre_adapt(double (*f)(double, void *), double xa, double xb, int Nmax,
                   double atol, double rtol, void *args, int *Neval,
                   double *eps, int verbose, int (*errf)(void *),
-                  double *pfa, double *pfb);
+                  double *pfa, double *pfb, Mesh9 *mout);
 double gk49_adapt(double (*f)(double, void *), double xa, double xb, int Nmax,
                   double atol, double rtol, void *args, int *Neval,
                   double *eps, int verbose, int (*errf)(void *));
 double gk715_adapt(double (*f)(double, void *), double xa, double xb, int Nmax,
                   double atol, double rtol, void *args, int *Neval,
                   double *eps, int verbose, int (*errf)(void *));
 double gk1021_adapt(double (*f)(double, void *), double xa, double xb, int Nmax,
```

### Comparing `afterglowpy-0.7.3/afterglowpy/interval.c` & `afterglowpy-0.8.0/afterglowpy/interval.c`

 * *Files 0% similar despite different names*

```diff
@@ -476,16 +476,19 @@
     m->heap = (struct Interval9 *)malloc(size * sizeof(struct Interval9));
 }
 
 void mesh9Free(struct Mesh9 *m)
 {
     m->totalSize = 0;
     m->N = 0;
-    free(m->heap);
-    m->heap = NULL;
+    if(m->heap != NULL)
+    {
+        free(m->heap);
+        m->heap = NULL;
+    }
 }
 
 void mesh9Insert(struct Mesh9 *m, struct Interval9 *i)
 {
     // Resize if necessary
     while(m->N >= m->totalSize)
     {
@@ -618,11 +621,11 @@
     *buf = (char *) realloc(*buf, (c+1) * sizeof(char));
 }
 
 void interval9Write(struct Interval9 *i, FILE *stream)
 {
     fprintf(stream, "(%.3le, %.3le)  %.12le +/- %.3le   %d\n",
             i->a, i->b, i->I, i->err, i->refinement);
-    fprintf(stream, "   [%.3le %.3le %.3le %.3le %.3le %.3le"
-                    " %.3le %.3le %.3le]\n", i->fa, i->fll, i->fl, i->flr,
+    fprintf(stream, "   [%.6le %.6le %.6le %.6le %.6le %.6le"
+                    " %.6le %.6le %.6le]\n", i->fa, i->fll, i->fl, i->flr,
                     i->fm, i->frl, i->fr, i->frr, i->fb);
 }
```

### Comparing `afterglowpy-0.7.3/afterglowpy/interval.h` & `afterglowpy-0.8.0/afterglowpy/interval.h`

 * *Files identical despite different names*

### Comparing `afterglowpy-0.7.3/afterglowpy/jetmodule.c` & `afterglowpy-0.8.0/afterglowpy/jetmodule.c`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 #include <Python.h>
-#define NPY_NO_DEPRECATED_API NPY_1_11_API_VERSION
+#define NPY_NO_DEPRECATED_API NPY_1_13_API_VERSION
 #include <numpy/arrayobject.h>
 #include <time.h>
 #include "offaxis_struct.h"
+#include "shockEvolution.h"
 
 #define PROFILE
 #define PROFILE1
 #define PROFILE2
 #define PROFILEOUTA
 
 static const int jet_type_default = -1;
 static const int spec_type_default = 0;
 static const double theta_obs_default = 0.0;
 static const double E_iso_core_default = 1.0e53;
 static const double theta_h_core_default = 0.1;
 static const double theta_h_wing_default = 0.4;
 static const double b_default = 0.0;
-static const double L0_default = 0.0;
-static const double q_default = 0.0;
-static const double ts_default = 0.0; 
+static const double L0_inj_default = 0.0;
+static const double q_inj_default = 0.0;
+static const double ts_inj_default = 0.0; 
+static const double t0_inj_default = 1.0e3; 
 static const double n_0_default = 1.0;
 static const double p_default = 2.2;
 static const double epsilon_E_default = 0.1;
 static const double epsilon_B_default = 0.01;
 static const double ksi_N_default = 1.0; 
 static const double d_L_default = 1.0e27;
 
 static const int latRes_default = 5;
 static const int tRes_default = 1000;
 static const int spread_default = 7;
 static const int counterjet_default = 0;
 static const int gamma_type_default = GAMMA_INF;
 static const double g0_default = -1.0;
+
+static const int envType_default = ENV_ISM;
+static const double R0_env_default = 1e18;
+static const double k_env_default = 0.0;
+static const double rho1_env_default = 1.0;
+
 static const double E_core_global_default = 0.0;
 static const double theta_h_core_global_default = 0.0;
 
 static const double rtol_struct_default = 1.0e-2;
 static const double rtol_theta_default = 1.0e-2;
 static const double rtol_phi_default = 1.0e-2;
 static const int int_type_default = INT_CADRE;
@@ -154,33 +162,54 @@
     PyModule_AddIntConstant(module, "Gaussian", _Gaussian);
     PyModule_AddIntConstant(module, "PowerLaw", _powerlaw);
     PyModule_AddIntConstant(module, "PowerLawCore", _powerlaw_core);
     PyModule_AddIntConstant(module, "GaussianCore", _Gaussian_core);
     PyModule_AddIntConstant(module, "Exponential", _exponential);
     PyModule_AddIntConstant(module, "TwoComponent", _twocomponent);
     PyModule_AddIntConstant(module, "Spherical", _spherical);
+    
     PyModule_AddIntConstant(module, "TrapFixed", INT_TRAP_FIXED);
     PyModule_AddIntConstant(module, "TrapAdapt", INT_TRAP_ADAPT);
     PyModule_AddIntConstant(module, "SimpFixed", INT_SIMP_FIXED);
     PyModule_AddIntConstant(module, "SimpAdapt", INT_SIMP_ADAPT);
     PyModule_AddIntConstant(module, "RombAdapt", INT_ROMB_ADAPT);
     PyModule_AddIntConstant(module, "TrapNL", INT_TRAP_NL);
     PyModule_AddIntConstant(module, "Hybrid", INT_HYBRID);
     PyModule_AddIntConstant(module, "Cadre", INT_CADRE);
     PyModule_AddIntConstant(module, "GK49Adapt", INT_GK49_ADAPT);
     PyModule_AddIntConstant(module, "GK715Adapt", INT_GK715_ADAPT);
     PyModule_AddIntConstant(module, "GK1021Adapt", INT_GK1021_ADAPT);
+    
     PyModule_AddIntConstant(module, "GammaInf", GAMMA_INF);
     PyModule_AddIntConstant(module, "GammaFlat", GAMMA_FLAT);
     PyModule_AddIntConstant(module, "GammaEvenMass", GAMMA_EVENMASS);
     PyModule_AddIntConstant(module, "GammaStruct", GAMMA_STRUCT);
+
+    PyModule_AddIntConstant(module, "SimpleSpec", SIMPLE_SPEC);
     PyModule_AddIntConstant(module, "ICCooling", IC_COOLING_FLAG);
     PyModule_AddIntConstant(module, "EpsEBar", EPS_E_BAR_FLAG);
     PyModule_AddIntConstant(module, "SSASmooth", SSA_SMOOTH_FLAG);
     PyModule_AddIntConstant(module, "SSASharp", SSA_SHARP_FLAG);
+    PyModule_AddIntConstant(module, "NoCooling", NO_COOLING_FLAG);
+    PyModule_AddIntConstant(module, "DeepNewtonian", DEEP_NEWTONIAN_FLAG);
+    PyModule_AddIntConstant(module, "BulkBM", BULK_BM_FLAG);
+    PyModule_AddIntConstant(module, "EnvISM", ENV_ISM);
+    PyModule_AddIntConstant(module, "EnvWind", ENV_WIND);
+    PyModule_AddIntConstant(module, "EnvPL", ENV_PL);
+    PyModule_AddIntConstant(module, "EnvStep", ENV_STEP);
+    PyModule_AddIntConstant(module, "MOM_0", MOM_0);
+    PyModule_AddIntConstant(module, "MOM_X", MOM_X);
+    PyModule_AddIntConstant(module, "MOM_Y", MOM_Y);
+    PyModule_AddIntConstant(module, "MOM_Z", MOM_Z);
+    PyModule_AddIntConstant(module, "MOM_XX", MOM_XX);
+    PyModule_AddIntConstant(module, "MOM_YY", MOM_YY);
+    PyModule_AddIntConstant(module, "MOM_ZZ", MOM_ZZ);
+    PyModule_AddIntConstant(module, "MOM_XY", MOM_XY);
+    PyModule_AddIntConstant(module, "MOM_YZ", MOM_YZ);
+    PyModule_AddIntConstant(module, "MOM_XZ", MOM_XZ);
 
 #if PY_MAJOR_VERSION >= 3
     return module;
 #endif
 }
 
 static PyObject *error_out(PyObject *m)
@@ -192,14 +221,15 @@
 
 static PyObject *jet_fluxDensity(PyObject *self, PyObject *args, 
                                     PyObject *kwargs)
 {
     PyObject *t_obj = NULL;
     PyObject *nu_obj = NULL;
     PyObject *mask_obj = NULL;
+    PyObject *moment_obj = NULL;
 
 #ifdef PROFILE
     clock_t profClock1A, profClock1B, profClock2A, profClock2B;
 #endif
 
 #ifdef PROFILE1
     //Profile 1
@@ -209,27 +239,34 @@
     int jet_type = jet_type_default;
     int spec_type = spec_type_default;
     double theta_obs = theta_obs_default;
     double E_iso_core = E_iso_core_default;
     double theta_h_core = theta_h_core_default;
     double theta_h_wing = theta_h_wing_default;
     double b = b_default;
-    double L0 = L0_default;
-    double q = q_default;
-    double ts = ts_default; 
+    double L0_inj = L0_inj_default;
+    double q_inj = q_inj_default;
+    double t0_inj = t0_inj_default; 
+    double ts_inj = ts_inj_default; 
     double n_0 = n_0_default;
     double p = p_default;
     double epsilon_E = epsilon_E_default;
     double epsilon_B = epsilon_B_default;
     double ksi_N = ksi_N_default; 
     double d_L = d_L_default;
 
     int latRes = latRes_default;
     int tRes = tRes_default;
     double g0 = g0_default;
+    
+    int envType = envType_default;
+    double R0_env = R0_env_default;
+    double k_env = k_env_default;
+    double rho1_env = rho1_env_default;
+    
     double E_core_global = E_core_global_default;
     double theta_h_core_global = theta_h_core_global_default;
 
     double rtol_struct = rtol_struct_default;
     double rtol_theta = rtol_theta_default;
     double rtol_phi = rtol_phi_default;
     int int_type = int_type_default;
@@ -238,131 +275,180 @@
 
     int spread = spread_default;
     int counterjet = counterjet_default;
     int gamma_type = gamma_type_default;
 
     static char *kwlist[] = {"t", "nu", "jetType", "specType",
                                 "thetaObs", "E0", "thetaCore", "thetaWing",
-                                    "b", "L0", "q", "ts", "n0", "p",
+                                    "b",
+                                    "L0", "q", "ts",
+                                    "n0", "p",
                                     "epsilon_e", "epsilon_B", "xi_N", "d_L",
                                     "g0",
+                                "envType", "R0Env", "kEnv", "rho1Env",
+                                "t0_inj",
                                 "E0Global", "thetaCoreGlobal",
                                 "tRes", "latRes", "intType", "rtolStruct",
                                     "rtolPhi", "rtolTheta", "NPhi", "NTheta",
                                 "mask",
-                                "spread", "counterjet", "gammaType",
+                                "spread", "counterjet", "gammaType", "moment",
                                 NULL};
 
+    //printf("About to parse args\n");
     //Parse Arguments
     if(!PyArg_ParseTupleAndKeywords(args, kwargs,
-                "OO|ii""ddddddddddddddd""dd""iiidddii""O""iii",
-                //"OO|ii ddddddddddddddd dd iiidddii O iii",
+                "OO|ii""ddddddddddddddd""iddd""d""dd""iiidddii""O""iii""O",
                 kwlist,
-                &t_obj, &nu_obj, &jet_type, &spec_type,
-                &theta_obs, &E_iso_core, &theta_h_core, &theta_h_wing, &b, &L0,
-                    &q, &ts, &n_0, &p, &epsilon_E, &epsilon_B, &ksi_N, &d_L,
+                &t_obj, &nu_obj,
+                &jet_type, &spec_type,
+                &theta_obs, &E_iso_core, &theta_h_core, &theta_h_wing, &b,
+                    &L0_inj, &q_inj, &ts_inj,
+                    &n_0, &p, &epsilon_E, &epsilon_B, &ksi_N, &d_L,
                     &g0,
+                &envType, &R0_env, &k_env, &rho1_env,
+                &t0_inj,
                 &E_core_global, &theta_h_core_global,
                 &tRes, &latRes, &int_type, &rtol_struct, &rtol_phi,
                     &rtol_theta, &nmax_phi, &nmax_theta,
                 &mask_obj,
-                &spread, &counterjet, &gamma_type))
+                &spread, &counterjet, &gamma_type, &moment_obj))
     {
-        //PyErr_SetString(PyExc_RuntimeError, "Could not parse arguments.");
+        PyErr_SetString(PyExc_RuntimeError, "Could not parse arguments.");
         return NULL;
     }
 
+    //printf("Args loaded\n");
+
     if(int_type < 0 || int_type >= INT_UNDEFINED)
     {
         PyErr_SetString(PyExc_RuntimeError,
                         "intType out of range, unknown integrator");
         return NULL;
     }
 
+    //printf("Args parsed\n");
+
     //Grab NUMPY arrays
     PyArrayObject *t_arr;
     PyArrayObject *nu_arr;
     PyArrayObject *mask_arr = NULL;
+    PyArrayObject *moment_arr = NULL;
+
+    int givenMask = mask_obj != NULL && mask_obj != Py_None;
+    int givenMoment = moment_obj != NULL && moment_obj != Py_None;
 
     t_arr = (PyArrayObject *) PyArray_FROM_OTF(t_obj, NPY_DOUBLE,
                                                 NPY_ARRAY_IN_ARRAY);
     nu_arr = (PyArrayObject *) PyArray_FROM_OTF(nu_obj, NPY_DOUBLE,
                                                 NPY_ARRAY_IN_ARRAY);
-    if(mask_obj != NULL)
+    if(givenMask)
         mask_arr = (PyArrayObject *) PyArray_FROM_OTF(mask_obj, NPY_DOUBLE,
                                                 NPY_ARRAY_IN_ARRAY);
+    if(givenMoment)
+        moment_arr = (PyArrayObject *) PyArray_FROM_OTF(moment_obj, NPY_INT64,
+                                                NPY_ARRAY_IN_ARRAY);
 
-    if(t_arr == NULL || nu_arr == NULL || (mask_obj != NULL
-                                            && mask_arr == NULL))
+    if(t_arr == NULL || nu_arr == NULL || (givenMask && mask_arr == NULL)
+            || (givenMoment && moment_arr == NULL))
     {
         PyErr_SetString(PyExc_RuntimeError, "Could not read input arrays.");
         Py_XDECREF(t_arr);
         Py_XDECREF(nu_arr);
         Py_XDECREF(mask_arr);
+        Py_XDECREF(moment_arr);
         return NULL;
     }
+    
+    //printf("Arrays grabbed\n");
 
     int t_ndim = (int) PyArray_NDIM(t_arr);
     int nu_ndim = (int) PyArray_NDIM(nu_arr);
     int mask_ndim = 0;
+    int moment_ndim = 0;
     if(mask_obj != NULL)
         mask_ndim = (int) PyArray_NDIM(mask_arr);
+    if(givenMoment)
+        moment_ndim = (int) PyArray_NDIM(moment_arr);
 
-    if(t_ndim != 1 || nu_ndim != 1 || (mask_obj != NULL && mask_ndim != 1))
+    if(t_ndim != 1 || nu_ndim != 1 || (givenMask && mask_ndim != 1)
+            || (givenMoment && moment_ndim != 1))
     {
         PyErr_SetString(PyExc_RuntimeError, "Arrays must be 1-D.");
         Py_DECREF(t_arr);
         Py_DECREF(nu_arr);
-        if(mask_obj != NULL)
+        if(mask_arr != NULL)
             Py_DECREF(mask_arr);
+        if(moment_arr != NULL)
+            Py_DECREF(moment_arr);
         return NULL;
     }
+    
+    //printf("NDims checked\n");
 
     int N = (int)PyArray_DIM(t_arr, 0);
     int Nnu = (int)PyArray_DIM(nu_arr, 0);
     int Nmask = 0;
-    if(mask_obj != NULL)
+    if(givenMask)
         Nmask = (int)PyArray_DIM(mask_arr, 0);
+    int Nmoment = 0;
+    if(givenMoment)
+        Nmoment = (int)PyArray_DIM(moment_arr, 0);
 
-    if(N != Nnu)
+    if(N != Nnu || (givenMoment && (Nmoment != N)))
     {
         PyErr_SetString(PyExc_RuntimeError, "Arrays must be same size.");
         Py_DECREF(t_arr);
         Py_DECREF(nu_arr);
-        if(mask_obj != NULL)
+        if(mask_arr != NULL)
             Py_DECREF(mask_arr);
+        if(moment_arr != NULL)
+            Py_DECREF(moment_arr);
         return NULL;
     }
     if(mask_obj != NULL && Nmask%9 != 0)
     {
         PyErr_SetString(PyExc_RuntimeError, 
                             "Mask length must be multiple of 9.");
         Py_DECREF(t_arr);
         Py_DECREF(nu_arr);
         Py_DECREF(mask_arr);
+        if(moment_arr != NULL)
+            Py_DECREF(moment_arr);
         return NULL;
     }
+    
+    //printf("Dims checked\n");
 
     double *t = (double *)PyArray_DATA(t_arr);
     double *nu = (double *)PyArray_DATA(nu_arr);
     double *mask = NULL;
-    if(mask_obj != NULL)
+    if(mask_arr != NULL)
         mask = (double *)PyArray_DATA(mask_arr);
     int masklen = Nmask/9;
+    
+    long *moment = NULL;
+    if(moment_arr != NULL)
+        moment = (long *)PyArray_DATA(moment_arr);
+
+    //printf("Data got\n");
 
     //Allocate output array
 
     npy_intp dims[1] = {N};
     PyObject *Fnu_obj = PyArray_SimpleNew(1, dims, NPY_DOUBLE);
 
     if(Fnu_obj == NULL)
     {
         PyErr_SetString(PyExc_RuntimeError, "Could not make flux array.");
         Py_DECREF(t_arr);
         Py_DECREF(nu_arr);
+        if(mask_arr != NULL)
+            Py_DECREF(mask_arr);
+        if(moment_arr != NULL)
+            Py_DECREF(moment_arr);
         return NULL;
     }
     double *Fnu = PyArray_DATA((PyArrayObject *) Fnu_obj);
 
 #ifdef PROFILE2
     //Profile 2
     profClock2A = clock();
@@ -380,51 +466,64 @@
         else if(t[i] > tb)
             tb = t[i];
     }
     
     struct fluxParams fp;
     setup_fluxParams(&fp, d_L, theta_obs, E_iso_core, theta_h_core,
                         theta_h_wing, b,
-                        L0, q, ts,
+                        L0_inj, q_inj, t0_inj, ts_inj,
                         n_0, p, epsilon_E, epsilon_B, ksi_N, g0, 
+                        envType, R0_env, k_env, rho1_env,
                         E_core_global, theta_h_core_global, ta, tb,
                         tRes, latRes, int_type,
                         rtol_struct, rtol_phi, rtol_theta,
                         nmax_phi, nmax_theta,
                         spec_type, mask, masklen,
                         spread, counterjet, gamma_type);
 
+    //printf("Ready to go!\n");
+
     // Calculate the flux!
-    calc_flux_density(jet_type, spec_type, t, nu, Fnu, N, &fp);
+    calc_flux_density(jet_type, spec_type, t, nu, Fnu, moment, N, &fp);
+    
+    //printf("Gone!\n");
    
     if(fp.error)
     {
         PyErr_SetString(PyExc_RuntimeError, fp.error_msg);
         free_fluxParams(&fp);
         return NULL;
     }
 
+
     //Free the parameters!
     free_fluxParams(&fp);
+    //printf("Freed params!\n");
 
 #ifdef PROFILE2
     //Profile 2
     profClock2B = clock();
 #endif
 
 
     // Clean up!
     Py_DECREF(t_arr);
     Py_DECREF(nu_arr);
     if(mask_obj != NULL)
         Py_DECREF(mask_arr);
+    if(moment_obj != NULL)
+        Py_DECREF(moment_arr);
+    
+    //printf("Decref'ed inputs!\n");
 
     //Build output
     PyObject *ret = Py_BuildValue("N", Fnu_obj);
     
+    //printf("Built outputs!\n");
+    
 #ifdef PROFILE1
     //Profile 1 and output
     profClock1B = clock();
 #endif
 
 #ifdef PROFILEOUT
 #ifdef PROFILE2
@@ -439,28 +538,29 @@
     
     return ret;
 }
 
 static PyObject *jet_emissivity(PyObject *self, PyObject *args)
 {
     int spec_type = 0;
-    double nu, R, mu, te, u, us, n0, p, epse, epsB, xi_N;
+    double nu, R, mu, te, u, us, rho0, Msw, p, epse, epsB, xi_N;
 
 
     //Parse Arguments
-    if(!PyArg_ParseTuple(args, "ddddddddddd|i", &nu, &R, &mu, &te,
-                            &u, &us, &n0, &p, &epse, &epsB, &xi_N, &spec_type))
+    if(!PyArg_ParseTuple(args, "dddddddddddd|i", &nu, &R, &mu, &te,
+                            &u, &us, &rho0, &Msw, &p, &epse, &epsB, &xi_N,
+                            &spec_type))
     {
         //PyErr_SetString(PyExc_RuntimeError, "Could not parse arguments.");
         return NULL;
     }
 
     // Calculate it!
-    double em = emissivity(nu, R, mu, te, u, us, n0, p, epse, epsB, 
-                            xi_N, spec_type);
+    double em = emissivity(nu, R, mu, te, u, us, rho0, Msw, p, epse, epsB, 
+                           xi_N, spec_type);
 
     //Build output
     PyObject *ret = Py_BuildValue("d", em);
     
     return ret;
 }
 
@@ -475,27 +575,34 @@
     int jet_type = jet_type_default;
     int spec_type = spec_type_default;
     double theta_obs = theta_obs_default;
     double E_iso_core = E_iso_core_default;
     double theta_h_core = theta_h_core_default;
     double theta_h_wing = theta_h_wing_default;
     double b = b_default;
-    double L0 = L0_default;
-    double q = q_default;
-    double ts = ts_default; 
+    double L0_inj = L0_inj_default;
+    double q_inj = q_inj_default;
+    double t0_inj = t0_inj_default; 
+    double ts_inj = ts_inj_default; 
     double n_0 = n_0_default;
     double p = p_default;
     double epsilon_E = epsilon_E_default;
     double epsilon_B = epsilon_B_default;
     double ksi_N = ksi_N_default; 
     double d_L = d_L_default;
 
     int latRes = latRes_default;
     int tRes = tRes_default;
     double g0 = g0_default;
+    
+    int envType = envType_default;
+    double R0_env = R0_env_default;
+    double k_env = k_env_default;
+    double rho1_env = rho1_env_default;
+    
     double E_core_global = E_core_global_default;
     double theta_h_core_global = theta_h_core_global_default;
 
     double rtol_struct = rtol_struct_default;
     double rtol_theta = rtol_theta_default;
     double rtol_phi = rtol_phi_default;
     int int_type = int_type_default;
@@ -507,29 +614,34 @@
     int gamma_type = gamma_type_default;
 
     static char *kwlist[] = {"theta", "phi", "t", "nu", "jetType", "specType",
                                 "thetaObs", "E0", "thetaCore", "thetaWing",
                                     "b", "L0", "q", "ts", "n0", "p",
                                     "epsilon_e", "epsilon_B", "xi_N", "d_L",
                                     "g0",
+                                "envType", "R0Env", "kEnv", "rho1Env",
+                                "t0_inj",
                                 "E0Global", "thetaCoreGlobal",
                                 "tRes", "latRes", "intType", "rtolStruct",
                                     "rtolPhi", "rtolTheta", "NPhi", "NTheta",
                                 "mask",
                                 "spread", "counterjet", "gammaType",
                                 NULL};
 
     //Parse Arguments
     if(!PyArg_ParseTupleAndKeywords(args, kwargs,
-                "OOOO|ii""ddddddddddddddd""dd""iiidddii""O""iii",
+                "OOOO|ii""ddddddddddddddd""iddd""d""dd""iiidddii""O""iii",
                 kwlist,
                 &theta_obj, &phi_obj, &t_obj, &nu_obj, &jet_type, &spec_type,
-                &theta_obs, &E_iso_core, &theta_h_core, &theta_h_wing, &b, &L0,
-                    &q, &ts, &n_0, &p, &epsilon_E, &epsilon_B, &ksi_N, &d_L,
+                &theta_obs, &E_iso_core, &theta_h_core, &theta_h_wing, &b,
+                    &L0_inj, &q_inj, &ts_inj,
+                    &n_0, &p, &epsilon_E, &epsilon_B, &ksi_N, &d_L,
                     &g0,
+                &envType, &R0_env, &k_env, &rho1_env,
+                    &t0_inj,
                 &E_core_global, &theta_h_core_global,
                 &tRes, &latRes, &int_type, &rtol_struct, &rtol_phi,
                     &rtol_theta, &nmax_phi, &nmax_theta,
                 &mask_obj,
                 &spread, &counterjet, &gamma_type))
     {
         //PyErr_SetString(PyExc_RuntimeError, "Could not parse arguments.");
@@ -663,16 +775,17 @@
         else if(t[i] > tb)
             tb = t[i];
     }
     
     struct fluxParams fp;
     setup_fluxParams(&fp, d_L, theta_obs, E_iso_core, theta_h_core,
                         theta_h_wing, b,
-                        L0, q, ts,
+                        L0_inj, q_inj, t0_inj, ts_inj,
                         n_0, p, epsilon_E, epsilon_B, ksi_N, g0, 
+                        envType, R0_env, k_env, rho1_env,
                         E_core_global, theta_h_core_global, ta, tb,
                         tRes, latRes, int_type,
                         rtol_struct, rtol_phi, rtol_theta,
                         nmax_phi, nmax_theta,
                         spec_type, mask, masklen,
                         spread, counterjet, gamma_type);
 
@@ -712,31 +825,38 @@
 
     int jet_type = jet_type_default;
     double theta_obs = theta_obs_default;
     double E_iso_core = E_iso_core_default;
     double theta_h_core = theta_h_core_default;
     double theta_h_wing = theta_h_wing_default;
     double b = b_default;
-    double L0 = L0_default;
-    double q = q_default;
-    double ts = ts_default; 
+    double L0_inj = L0_inj_default;
+    double q_inj = q_inj_default;
+    double t0_inj = t0_inj_default; 
+    double ts_inj = ts_inj_default; 
     double n_0 = n_0_default;
     double p = p_default;
     double epsilon_E = epsilon_E_default;
     double epsilon_B = epsilon_B_default;
     double ksi_N = ksi_N_default; 
     double d_L = d_L_default;
 
     int latRes = latRes_default;
     int tRes = tRes_default;
     int spread = spread_default;
     int counterjet = counterjet_default;
     int gamma_type = gamma_type_default;
     int spec_type = spec_type_default;
     double g0 = g0_default;
+
+    int envType = envType_default;
+    double R0_env = R0_env_default;
+    double k_env = k_env_default;
+    double rho1_env = rho1_env_default;
+    
     double E_core_global = E_core_global_default;
     double theta_h_core_global = theta_h_core_global_default;
 
     double rtol_struct = rtol_struct_default;
     double rtol_theta = rtol_theta_default;
     double rtol_phi = rtol_phi_default;
     int int_type = int_type_default;
@@ -744,29 +864,34 @@
     int nmax_theta = nmax_theta_default;
 
     static char *kwlist[] = {"theta", "phi", "t", "jetType", "specType",
                                 "thetaObs", "E0", "thetaCore", "thetaWing",
                                     "b", "L0", "q", "ts", "n0", "p",
                                     "epsilon_e", "epsilon_B", "xi_N", "d_L",
                                     "g0",
+                                "envType", "R0Env", "kEnv", "rho1Env",
+                                "t0_inj",
                                 "E0Global", "thetaCoreGlobal",
                                 "tRes", "latRes", "intType", "rtolStruct",
                                     "rtolPhi", "rtolTheta", "NPhi", "NTheta",
                                 "mask",
                                 "spread", "counterjet", "gammaType",
                                 NULL};
 
     //Parse Arguments
     if(!PyArg_ParseTupleAndKeywords(args, kwargs,
-                "OOO|ii""ddddddddddddddd""dd""iiidddii""O""iii",
+                "OOO|ii""ddddddddddddddd""iddd""d""dd""iiidddii""O""iii",
                 kwlist,
                 &theta_obj, &phi_obj, &t_obj, &jet_type, &spec_type,
-                &theta_obs, &E_iso_core, &theta_h_core, &theta_h_wing, &b, &L0,
-                    &q, &ts, &n_0, &p, &epsilon_E, &epsilon_B, &ksi_N, &d_L,
+                &theta_obs, &E_iso_core, &theta_h_core, &theta_h_wing, &b,
+                    &L0_inj, &q_inj, &ts_inj, &n_0, &p, &epsilon_E, &epsilon_B,
+                    &ksi_N, &d_L,
                     &g0,
+                &envType, &R0_env, &k_env, &rho1_env,
+                &t0_inj,
                 &E_core_global, &theta_h_core_global,
                 &tRes, &latRes, &int_type, &rtol_struct, &rtol_phi,
                     &rtol_theta, &nmax_phi, &nmax_theta,
                 &mask_obj,
                 &spread, &counterjet, &gamma_type))
     {
         //PyErr_SetString(PyExc_RuntimeError, "Could not parse arguments.");
@@ -897,16 +1022,17 @@
         else if(t[i] > tb)
             tb = t[i];
     }
 
     struct fluxParams fp;
     setup_fluxParams(&fp, d_L, theta_obs, E_iso_core, theta_h_core,
                         theta_h_wing, b,
-                        L0, q, ts,
+                        L0_inj, q_inj, t0_inj, ts_inj,
                         n_0, p, epsilon_E, epsilon_B, ksi_N, g0, 
+                        envType, R0_env, k_env, rho1_env,
                         E_core_global, theta_h_core_global, ta, tb,
                         tRes, latRes, int_type,
                         rtol_struct, rtol_phi, rtol_theta,
                         nmax_phi, nmax_theta,
                         spec_type, mask, masklen,
                         spread, counterjet, gamma_type);
 
@@ -953,17 +1079,18 @@
     double ta = Rt0;
     double tb = Rt1;
 
     struct fluxParams pars;
     pars.ta = ta;
     pars.tb = tb;
     pars.n_0 = n0;
-    pars.L0 = L0;
-    pars.q = q;
-    pars.ts = ts;
+    pars.L0_inj = L0;
+    pars.q_inj = q;
+    pars.t0_inj = t0_inj_default;
+    pars.ts_inj = ts;
     pars.tRes = tRes;
     pars.E_tot = -1.0;
     pars.t_table = NULL;
     pars.R_table = NULL;
     pars.u_table = NULL;
     pars.th_table = NULL;
     pars.mu_table = NULL;
@@ -1040,17 +1167,18 @@
         return NULL;
     }
 
     struct fluxParams pars;
     pars.ta = ta;
     pars.tb = tb;
     pars.n_0 = n0;
-    pars.L0 = L0;
-    pars.q = q;
-    pars.ts = ts;
+    pars.L0_inj = L0;
+    pars.q_inj = q;
+    pars.t0_inj = t0_inj_default;
+    pars.ts_inj = ts;
     pars.tRes = tRes;
     pars.E_tot = -1.0;
     pars.t_table = NULL;
     pars.R_table = NULL;
     pars.u_table = NULL;
     pars.th_table = NULL;
     pars.mu_table = NULL;
@@ -1059,23 +1187,23 @@
     pars.R_table_inner = NULL;
     pars.u_table_inner = NULL;
     pars.th_table_inner = NULL;
     pars.mu_table_inner = NULL;
     pars.table_entries_inner = 0;
     pars.spread = spread;
 
-    printf("set_jet_params\n");
+    //printf("set_jet_params\n");
     set_jet_params(&pars, E0, thetah);
     if(pars.error)
     {
         PyErr_SetString(PyExc_RuntimeError, pars.error_msg);
         free_fluxParams(&pars);
         return NULL;
     }
-    printf("done\n");
+    //printf("done\n");
 
     //Allocate output arrays
     int N = pars.table_entries;
     npy_intp dims[1] = {N};
     PyObject *t_obj = PyArray_SimpleNew(1, dims, NPY_DOUBLE);
     PyObject *R_obj = PyArray_SimpleNew(1, dims, NPY_DOUBLE);
     PyObject *u_obj = PyArray_SimpleNew(1, dims, NPY_DOUBLE);
@@ -1111,22 +1239,23 @@
     
     return ret;
 }
 
 static PyObject *jet_find_jet_edge(PyObject *self, PyObject *args)
 {
     double tobs, phi, theta_obs, theta_0;
+    int funcVer;
     PyObject *t_obj = NULL;
     PyObject *R_obj = NULL;
     PyObject *thj_obj = NULL;
     
 
     //Parse Arguments
-    if(!PyArg_ParseTuple(args, "OOOdddd", &t_obj, &R_obj, &thj_obj, &tobs,
-                         &phi, &theta_obs, &theta_0))
+    if(!PyArg_ParseTuple(args, "OOOddddi", &t_obj, &R_obj, &thj_obj, &tobs,
+                         &phi, &theta_obs, &theta_0, &funcVer))
     {
         //PyErr_SetString(PyExc_RuntimeError, "Could not parse arguments.");
         return NULL;
     }
     
     PyArrayObject *t_arr;
     PyArrayObject *R_arr;
@@ -1178,16 +1307,39 @@
     double *thj = (double *)PyArray_DATA(thj_arr);
 
     double *mu = (double *)malloc(N * sizeof(double));
     int i;
     for(i=0; i<N; i++)
         mu[i] = (t[i] - tobs) * v_light / R[i];
 
-    double th = find_jet_edge(phi, cos(theta_obs), sin(theta_obs), theta_0,
-                              mu, thj, N);
+    double *cth = (double *)malloc(N * sizeof(double));
+    double *sth = (double *)malloc(N * sizeof(double));
+    for(i=0; i<N; i++)
+    {
+        cth[i] = cos(thj[i]);
+        sth[i] = sin(thj[i]);
+    }
+
+    int idx_mu_neg1 = searchSorted(-1.0, mu, N);
+    if(idx_mu_neg1 > 0)
+        idx_mu_neg1--;
+    
+    int idx_mu_pos1 = searchSorted(1.0, mu, N);
+    if(idx_mu_pos1 + 1 < N)
+        idx_mu_pos1++;
+
+    double th;
+    if(funcVer)
+        th = find_jet_edge(phi, cos(theta_obs), sin(theta_obs), theta_0,
+                              mu, thj, N, idx_mu_neg1, idx_mu_pos1, cth, sth);
+    else
+        th = find_jet_edge_old(phi, cos(theta_obs), sin(theta_obs), theta_0,
+                              mu, thj, N, idx_mu_neg1, idx_mu_pos1, cth, sth);
 
     free(mu);
+    free(cth);
+    free(sth);
 
     PyObject *ret = Py_BuildValue("d", th);
     
     return ret;
 }
```

### Comparing `afterglowpy-0.7.3/afterglowpy/offaxis_struct.h` & `afterglowpy-0.8.0/afterglowpy/offaxis_struct.h`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 // offaxis.h
 
 #include <stdlib.h>
 #include <stdio.h>
 #include <math.h>
 #include "integrate.h"
+#include "interval.h"
 
 #define ERR_CHK_VOID(pars) if(pars->error){ return;}
 #define ERR_CHK_INT(pars) if(pars->error){ return 0;}
 #define ERR_CHK_DBL(pars) if(pars->error){ return 0.0;}
 #define MSG_LEN 4096
 #define DUMP_MSG_LEN_MAX 16384  //overkill: 200 lines * 80c per line = 16000
 
@@ -48,40 +49,50 @@
 #define _Gaussian_core 2 // has a core as well
 #define _spherical 3
 #define _powerlaw 4
 #define _exponential 5
 #define _twocomponent 6
 #define _exponential2 7
 
+#define SIMPLE_SPEC 0
 #define IC_COOLING_FLAG 1
 #define EPS_E_BAR_FLAG  2
 #define SSA_SMOOTH_FLAG 4
 #define SSA_SHARP_FLAG  8
+#define NO_COOLING_FLAG  16
+#define DEEP_NEWTONIAN_FLAG  32
+#define BULK_BM_FLAG  64
+#define FIXED_PL_FLAG  128
 
 enum{INT_TRAP_FIXED, INT_TRAP_ADAPT, INT_SIMP_FIXED, INT_SIMP_ADAPT,
      INT_ROMB_ADAPT, INT_TRAP_NL, INT_HYBRID, INT_CADRE,
      INT_GK49_ADAPT, INT_GK715_ADAPT, INT_GK1021_ADAPT,
      INT_UNDEFINED};
 
 enum{GAMMA_INF, GAMMA_FLAT, GAMMA_EVENMASS, GAMMA_STRUCT};
 
+enum{MOM_0, MOM_X, MOM_Y, MOM_Z, MOM_XX, MOM_YY, MOM_ZZ,
+     MOM_XY, MOM_YZ, MOM_XZ};
+
 struct fluxParams
 {
     double theta;
     double phi;
     double cp;
+    double sp;
     double ct;
     double st;
     double cto;
     double sto;
     
     double theta_obs;
     double t_obs;
     double nu_obs;
     double d_L;
+    long moment;
 
     double E_iso;
     double n_0;
     double g_init;
 
     double p;
     double epsilon_E;
@@ -95,23 +106,27 @@
     double b;
     double E_tot;
     double g_core;
     double E_core_global;
     double theta_core_global;
 
     int envType;
-    double As;
-    double Rwind;
-
-    double L0;
-    double q;
-    double ts;
+    double R0_env;
+    double k_env;
+    double rho1_env;
+
+    double L0_inj;
+    double q_inj;
+    double t0_inj;
+    double ts_inj;
     
     double current_theta_cone_hi;
     double current_theta_cone_low;
+    double current_theta_b;
+    double current_theta_a;
     double theta_obs_cur;
     int tRes;
     int latRes;
     int spread;
     int counterjet;
 
     int int_type;
@@ -128,29 +143,42 @@
     double ta;
     double tb;
 
     double C_BMsqrd;
     double C_STsqrd;
 
     double t_NR;
+    int cur_entry;
 
     double *t_table;
     double *R_table;
     double *u_table;
     double *th_table;
     double *mu_table;
+    double *cth_table;
+    double *sth_table;
     int table_entries;
 
     double *t_table_inner;
     double *R_table_inner;
     double *u_table_inner;
     double *th_table_inner;
     double *mu_table_inner;
+    double *cth_table_inner;
+    double *sth_table_inner;
     int table_entries_inner;
 
+    int idx_mu_neg1;
+    int idx_mu_pos1;
+    int idx_mu_neg1_inner;
+    int idx_mu_pos1_inner;
+
+    Mesh9 phi_mesh;
+    Mesh9 theta_mesh;
+
     int spec_type;
     int gamma_type;
 
     double (*f_E)(double, void *);
 
     double *mask;
     int nmask;
@@ -173,28 +201,44 @@
 double f_Etot_tophat(void *params);
 double f_Etot_Gaussian(void *params);
 double f_Etot_powerlaw(void *params);
 
 void make_R_table(struct fluxParams *pars);
 void make_mu_table(struct fluxParams *pars);
 double check_t_e(double t_e, double mu, double t_obs, double *mu_table, int N);
-int searchSorted(double x, double *arr, int N);
+int searchSorted(double x, const double *arr, int N);
 double interpolateLin(int a, int b, double x, double *X, double *Y, int N);
 double interpolateLog(int a, int b, double x, double *X, double *Y, int N);
+double find_jet_edge_old(double phi, double cto, double sto, double theta0,
+                     const double *a_mu, const double *a_thj, int N,
+                     int idx_mu_neg1, int idx_mu_pos1,
+                     const double *a_cthj, const double *a_sthj);
 double find_jet_edge(double phi, double cto, double sto, double theta0,
-                     double *a_mu, double *a_thj, int N);
+                      const double *a_mu, const double *a_thj, int N,
+                      int idx_mu_neg1, int idx_mu_pos1,
+                      const double *a_cthj, const double *a_sthj);
 double costheta_integrand(double a_theta, void* params); // inner integral
 double phi_integrand(double a_phi, void* params); // outer integral
 double emissivity(double nu, double R, double mu, double te,
-                    double u, double us, double n0, double p, double epse,
-                    double epsB, double ksiN, int specType); //emissivity of
+                    double u, double us, double rho0, double Msw, double p,
+                    double epse, double epsB, double ksiN,
+                    int specType); //emissivity of
                                                              // a zone.
+
+void calc_absorption_length(double R, double mu, double delta,
+                              double betaS, double uS,
+                              double *length_back, double *length_front);
+double absorption_integral(double Rb, double dR, double taua, double taub,
+                           int order);
+double absorption_integral_core(double a, double b, int order);
+
 double flux(struct fluxParams *pars, double atol); // determine flux for a given t_obs
 
-double flux_cone(double t_obs, double nu_obs, double E_iso, double theta_h,
+double flux_cone(double t_obs, double nu_obs, long moment,
+                    double E_iso, double theta_h,
                     double theta_cone_low, double theta_cone_hi,
                     double atol, struct fluxParams *pars);
 double intensity(double theta, double phi, double tobs, double nuobs,
                 double theta_obs, double theta_cone_hi, double theta_cone_low,
                 struct fluxParams *pars);
 void shockVals(double theta, double phi, double tobs,
                  double *t, double *R, double *u, double *thj,
@@ -228,71 +272,68 @@
                         struct fluxParams *pars);
 void shockVals_structCore(double *theta, double *phi, double *tobs,
                         double *t, double *R, double *u, double *thj, int N,
                         double E_iso_core, 
                         double theta_h_core, double theta_h_wing,
                         int res_cones, double (*f_E)(double,void *),
                         struct fluxParams *pars);
-void lc_tophat(double *t, double *nu, double *F, int Nt,
+void lc_tophat(double *t, double *nu, double *F, long *moment, int Nt,
                 double E_iso, double theta_h, struct fluxParams *pars);
-void lc_cone(double *t, double *nu, double *F, int Nt, double E_iso,
-                double theta_h, double theta_wing, struct fluxParams *pars);
-void lc_powerlawCore(double *t, double *nu, double *F, int Nt,
-                    double E_iso_core, double theta_h_core, 
-                    double theta_h_wing, double beta,
-                    double *theta_c_arr, double *E_iso_arr,
-                    int res_cones, struct fluxParams *pars);
-void lc_powerlaw(double *t, double *nu, double *F, int Nt,
-                    double E_iso_core, double theta_h_core, 
-                    double theta_h_wing,
-                    double *theta_c_arr, double *E_iso_arr,
-                    int res_cones, struct fluxParams *pars);
-void lc_Gaussian(double *t, double *nu, double *F, int Nt,
+void lc_cone(double *t, double *nu, double *F, long *moment, int Nt,
+                double E_iso, double theta_h, double theta_wing,
+                struct fluxParams *pars);
+void lc_struct(double *t, double *nu, double *F, long *moment, int Nt,
                         double E_iso_core, 
                         double theta_h_core, double theta_h_wing,
                         double *theta_c_arr, double *E_iso_arr,
-                        int res_cones, struct fluxParams *pars);
-void lc_GaussianCore(double *t, double *nu, double *F, int Nt,
-                        double E_iso_core,
+                        int res_cones, double (*f_E)(double,void *),
+                        struct fluxParams *pars);
+void lc_structCore(double *t, double *nu, double *F, long *moment, int Nt,
+                        double E_iso_core, 
                         double theta_h_core, double theta_h_wing,
                         double *theta_c_arr, double *E_iso_arr,
-                        int res_cones, struct fluxParams *pars);
+                        int res_cones, double (*f_E)(double,void *),
+                        struct fluxParams *pars);
 
 void calc_flux_density(int jet_type, int spec_type, 
-                            double *t, double *nu, double *Fnu, int N,
-                            struct fluxParams *fp);
+                            double *t, double *nu, double *Fnu, long *moment,
+                            int N, struct fluxParams *fp);
 void calc_intensity(int jet_type, int spec_type, double *theta, double *phi,
                             double *t, double *nu, double *Inu, int N,
                             struct fluxParams *fp);
 void calc_shockVals(int jet_type, double *theta, double *phi, double *tobs,
                             double *t, double *R, double *u, double *thj, int N,
                             struct fluxParams *fp);
 
 void setup_fluxParams(struct fluxParams *pars,
                     double d_L,
                     double theta_obs,
                     double E_iso_core, double theta_core, double theta_wing,
-                    double b, double L0, double q, double ts, 
+                    double b,
+                    double L0_inj, double q_inj, double t0_inj, double ts_inj, 
                     double n_0,
                     double p,
                     double epsilon_E,
                     double epsilon_B, 
                     double ksi_N,
                     double g0,
+                    int envType, double R0_env, double k_env, double rho1_env, 
                     double E_core_global,
                     double theta_core_global,
                     double ta, double tb,
                     int tRes, int latRes, int int_type,
                     double rtol_struct, double rtol_phi, double rtol_theta,
                     int nmax_phi, int nmax_theta,
                     int spec_type,
                     double *mask, int nmask,
                     int spread, int counterjet, int gamma_type);
+
 void set_jet_params(struct fluxParams *pars, double E_iso, double theta_h);
-void set_obs_params(struct fluxParams *pars, double t_obs, double nu_obs,
+void set_obs_params(struct fluxParams *pars,
+                        double t_obs, double nu_obs, long moment,
                         double theta_obs_cur, double current_theta_cone_hi, 
                         double current_theta_cone_low);
 int check_error(void *params);
 void set_error(struct fluxParams *pars, char msg[]);
 void free_fluxParams(struct fluxParams *pars);
 
 #endif
```

### Comparing `afterglowpy-0.7.3/afterglowpy/offaxis_struct_funcs.c` & `afterglowpy-0.8.0/afterglowpy/offaxis_struct_funcs.c`

 * *Files 12% similar despite different names*

```diff
@@ -176,15 +176,15 @@
         //return t_obs / (1.0 - mu); // so return small t_e limit
         return -1;
     }
 
     return t_e;
 }
 
-int searchSorted(double x, double *arr, int N)
+int searchSorted(double x, const double *arr, int N)
 {
     if(x <= arr[0])
         return 0;
     else if(x >= arr[N-1])
         return N-2;
 
   unsigned int i = ((unsigned int) N) >> 1;
@@ -244,14 +244,35 @@
         mu_table[i] = (t_table[i] - t_obs) / R_table[i] * v_light;
     }
     for (i = 0; i< table_entries_inner; i++)
     {
         mu_table_inner[i] = (t_table_inner[i] - t_obs)
                             / R_table_inner[i] * v_light;
     }
+
+    pars->idx_mu_neg1 = searchSorted(-1.0, mu_table, table_entries);
+    if(pars->idx_mu_neg1 > 0)
+        pars->idx_mu_neg1--;
+    
+    pars->idx_mu_pos1 = searchSorted(1.0, mu_table, table_entries);
+    if(pars->idx_mu_pos1 + 1 < table_entries)
+        pars->idx_mu_pos1++;
+
+    if(table_entries_inner > 0)
+    {
+        pars->idx_mu_neg1_inner = searchSorted(-1.0, mu_table_inner,
+                                               table_entries_inner);
+        if(pars->idx_mu_neg1_inner > 0)
+            pars->idx_mu_neg1_inner--;
+        
+        pars->idx_mu_pos1_inner = searchSorted(1.0, mu_table_inner,
+                                               table_entries_inner);
+        if(pars->idx_mu_pos1_inner + 1 < table_entries_inner)
+            pars->idx_mu_pos1_inner++;
+    }
 }
 
 void make_R_table(struct fluxParams *pars)
 {
     int tRes = pars->tRes;
     double Rt0 = pars->Rt0;
     double Rt1 = pars->Rt1;
@@ -272,19 +293,29 @@
     pars->u_table = (double *)realloc(temp, sizeof(double) * table_entries);
     temp = pars->th_table_inner;
     pars->th_table_inner = pars->th_table;
     pars->th_table = (double *)realloc(temp, sizeof(double) * table_entries);
     temp = pars->mu_table_inner;
     pars->mu_table_inner = pars->mu_table;
     pars->mu_table = (double *)realloc(temp, sizeof(double) * table_entries);
+    
+    temp = pars->cth_table_inner;
+    pars->cth_table_inner = pars->cth_table;
+    pars->cth_table = (double *)realloc(temp, sizeof(double) * table_entries);
+    temp = pars->sth_table_inner;
+    pars->sth_table_inner = pars->sth_table;
+    pars->sth_table = (double *)realloc(temp, sizeof(double) * table_entries);
+
 
     double *t_table = pars->t_table;
     double *R_table = pars->R_table;
     double *u_table = pars->u_table;
     double *th_table = pars->th_table;
+    double *cth_table = pars->cth_table;
+    double *sth_table = pars->sth_table;
 
     double fac = pow(Rt1/Rt0, 1.0/(table_entries-1.0));
     t_table[0] = Rt0;
 
     int i;
     for(i=1; i<table_entries; i++)
         t_table[i] = t_table[i-1] * fac;
@@ -303,26 +334,40 @@
     if(thC <= 0.0)
         thC = pars->theta_wing;
     //thC = 0.08; //th0;
     double thCg = pars->theta_core_global;
     if(thCg <= 0.0)
         thCg = thC;
 
-    double args[12] = {pars->E_iso, Mej_sph, m_p*pars->n_0, 0.0, 0.0, 0.0, 
-                        pars->L0, pars->q, pars->ts, thC, th0, thCg};
+    //double args[12] = {pars->E_iso, Mej_sph, m_p*pars->n_0, 0.0, 0.0, 0.0, 
+    //                    pars->L0_inj, pars->q_inj, pars->ts_inj,
+    //                    thC, th0, thCg};
     int spread = pars->spread;
+
+    struct shockParams shock_pars;
+    setup_shockParams(&shock_pars, spread, pars->E_iso, Mej_sph,
+                      pars->envType, m_p*pars->n_0, pars->R0_env, pars->k_env,
+                      pars->rho1_env,
+                      pars->L0_inj, pars->q_inj, pars->t0_inj, pars->ts_inj,
+                      0.0, 0.0, 0.0,
+                      thC, th0, thCg);
+
     double R0, u0;
     //shockInitDecel(Rt0, &R0, &u0, args);
-    shockInitFind(Rt0, &R0, &u0, pars->tRes/10, args);
+    shockInitFind(Rt0, &R0, &u0, pars->tRes/10, &shock_pars);
     //printf("t0=%.6le R0=%.6le u0=%.6le\n", Rt0, R0, u0);
 
-    args[0] = pars->E_iso * fom;
-    args[1] = Mej_sph * fom;
+    //args[0] = pars->E_iso * fom;
+    //args[1] = Mej_sph * fom;
+
+    shock_pars.E0 = pars->E_iso * fom;
+    shock_pars.Mej = Mej_sph * fom;
+
     shockEvolveSpreadRK4(t_table, R_table, u_table, th_table, table_entries,
-                            R0, u0, th0, args, spread);
+                            R0, u0, th0, &shock_pars);
 
     if(R_table[0] != R_table[0])
     {
         char msg[MSG_LEN];
         int c = 0;
         c += snprintf(msg, MSG_LEN,
                       "Shock integration Error: R[0]=%.3e  (fac=%.3e)\n",
@@ -345,56 +390,187 @@
 
         c += snprintf(msg+c, MSG_LEN-c,
                       "    t0=%.3e R0=%.3e u0=%.3e th0=%.3e\n",
                       Rt0, R0, u0, th0);
         set_error(pars, msg);
         return;
     }
+
+    for(i=0; i<table_entries; i++)
+    {
+        cth_table[i] = cos(th_table[i]);
+        sth_table[i] = sin(th_table[i]);
+    }
+}
+double absorption_integral_core(double a, double b, int order)
+{
+    /*
+     * Evaluates \int_0^1  (1-a*x)^2 * \exp(-b*x) dx
+     *
+     * with an approximation encoded by "order"
+     */
+
+    double dV = 3 - 3*a + a*a;
+    double I = dV / (3 + dV*b);
+    
+    if(order  >= 1)
+    {
+        double A = dV/3.0;
+        double B = -(0.5 - 2*a/3.0 + 0.25*a*a);
+        double D = 1.0;
+        double E = -2*a;
+
+        I = (A*(D*D+A*E) + (A*A+B*D)*D*b) / (
+                D*D+A*E + (A*D-B*E)*b + (A*A+B*D)*b*b);
+    }
+
+    return I;
+}
+
+double absorption_integral(double Rb, double dR, double taua, double taub,
+                           int order)
+{
+    /*
+     * Evaluates the integral \int_Ra^Rb R^2 \exp(-tau(R)) dR
+     *
+     * where tau(R) = (Rb-R)/dR * taua  +  (R-Ra)/dR * taub
+     * and Ra = Rb-dR
+     *
+     * this function is mainly to swap arguments depending on whether
+     * tau(Ra) < tau(Rb), as the approximation used to evaluate the integral
+     * requires the argument to the exponential to be negative.
+     */
+
+    if(taub < taua)
+    {
+        return Rb*Rb*dR * exp(-taub)
+                * absorption_integral_core(dR/Rb, taua - taub, order);
+    }
+    else
+    {
+        double Ra = Rb - dR;
+        return Ra*Ra*dR * exp(-taua)
+                * absorption_integral_core(dR/Ra, taub - taua, order);
+    }
+}
+
+void calc_absorption_length(double R, double mu, double delta,
+                              double betaS, double uS,
+                              double *length_back, double *length_front)
+{
+    // betaI = (1-delta) * betaS
+    //
+    // ==> uI = (1-delta) * uS / sqrt(1 + (2-delta)*delta * uS^2)
+
+    double gS = sqrt(1 + uS*uS);
+    
+    double uI = (1-delta) * uS / sqrt(1 + (2-delta)*delta * uS*uS);
+    double gI = sqrt(1 + uI*uI);
+    double betaI = uI / gI;
+
+    double dl_delta = sqrt((2-delta)*delta);
+
+    double dcos1 = gS*((1-delta)*mu - betaS);
+
+    double dl_sphere_front = mu > betaS ? 0.0 : 2*R*gS*gS*(betaS-mu);
+    double dl_sphere_back = 0.0;
+
+    if(dcos1 >= -dl_delta)
+        dl_sphere_back = R*gS*gS * (1-betaS*mu)/(1-betaI*mu)
+                    * (2-delta)*delta
+                    / (gS*(dcos1 + sqrt(dcos1*dcos1 + (2-delta)*delta)));
+    else
+        dl_sphere_back = R*gS * (1-betaS*mu)/(1-betaI*mu)
+                    * (sqrt(dcos1*dcos1 + (2-delta)*delta) - dcos1);
+
+    double dl_cavity_front = 0.0;
+    double dl_cavity_back = mu  > betaI ? 0.0 : 
+            2*R*gI*gI*(1-betaS*mu)/(1-betaI*mu) * (1-delta) * (betaI-mu);
+
+    
+    if(mu < (1-delta)*betaI - dl_delta/gI)
+    {
+        double dcos2 = gI * (mu - (1-delta)*betaI);
+        dl_cavity_front = 2*R*gI * sqrt((dcos2-dl_delta) * (dcos2+dl_delta));
+    }
+
+    /* 
+    if(mu >= betaS)
+        printf("AAA\n");
+    else if(mu >= betaI)
+        printf("BBB\n");
+    else if(mu >= (1-delta)*betaI - dl_delta/gI)
+        printf("CCC\n");
+    else
+        printf("DDD\n");
+
+    printf("betaS=%.3le uS=%.3le gS=%.3le, 1-bS=%.3le, 1-mu*bS=%.3le\n",
+            betaS, uS, gS, 1-betaS, 1-mu*betaS);
+    printf("betaI=%.3le uI=%.3le gI=%.3le, 1-bI=%.3le, 1-mu*bI=%.3le\n",
+            betaI, betaI*gI, gI, 1-betaI, 1-mu*betaI);
+    printf("mu=%.3le d=%.3le\n", mu, gS, delta);
+    printf("dcos1=%.6le\n", dcos1);
+    printf("%.6le  %.6le  %.6le  %.6le\n", dl_sphere_back, dl_sphere_front,
+            dl_cavity_back, dl_cavity_front);
+    */
+
+    *length_back = dl_sphere_back - dl_cavity_back;
+    *length_front = dl_sphere_front - dl_cavity_front;
+
+    //printf("%.6le    %.6le\n", *length_back, *length_front);
 }
 
 ///////////////////////////////////////////////////////////////////////////////
 
 double emissivity(double nu, double R, double mu, double te,
-                    double u, double us, double n0, double p, double epse,
+                    double u, double us, double rho0, double Msw,
+                    double p, double epse,
                     double epsB, double ksiN, int specType)
 {
     if(us < 1.0e-5)
     {
         //shock is ~ at sound speed of warm ISM. Won't shock, approach invalid.
         return 0.0;
     }
     if(R == 0.0)
         return 0.0;
 
     // set remaining fluid quantities
+    double n0 = rho0 / m_p;
     double g = sqrt(1+u*u);
     double beta = u/g;
     double betaS = us / sqrt(1+us*us);
     double nprime = 4.0 * n0 * g; // comoving number density
     double e_th = u*u/(g+1) * nprime * m_p * v_light * v_light;
     double B = sqrt(epsB * 8.0 * PI * e_th);
     double a = (1.0 - mu * beta); // beaming factor
     double ashock = (1.0 - mu * betaS); // shock velocity beaming factor
-    double DR = R / (12.0 * g*g * ashock);
+    double DR0 = Msw / (16*M_PI * R*R * g*g * rho0);  //shock width in labframe
+    double DR = DR0 / ashock; //shock width for constant-tobs slice
+    //double DR = R / (12.0 * g*g * ashock);
     if (DR < 0.0) DR *= -1.0; // DR is function of the absolute value of mu
 
-
     double epsebar;
     if(specType & EPS_E_BAR_FLAG)
+    {
         epsebar = epse;
+        epse = (p-1) / (p-2) * epsebar;
+    }
     else
         epsebar = (2.0-p) / (1.0-p) * epse;
 
 
     // set local emissivity 
     double nuprime = nu * g * a; // comoving observer frequency
     double g_m = epsebar * e_th / (ksiN * nprime * m_e * v_light * v_light);
     double g_c = 6 * PI * m_e * g * v_light / (sigma_T * B * B * te);
+    if((specType & DEEP_NEWTONIAN_FLAG) && g_m < 1.0)
+        g_m = 1.0;
 
-    //Inverse Compton adjustment of lfac_c
+    //Inverse Compton adjustment of g_c
     if(specType & IC_COOLING_FLAG)
     {
         double gr = g_c / g_m;
         double y = beta * epse/epsB;
         double X = 1.0;
 
         if(gr <= 1.0 || gr*gr-gr-y <= 0.0)
@@ -426,40 +602,65 @@
         g_c /= X;
     }
 
     double nu_m = 3.0 * g_m * g_m * e_e * B / (4.0 * PI * m_e * v_light);
     double nu_c = 3.0 * g_c * g_c * e_e * B / (4.0 * PI * m_e * v_light);
     double em = 0.5*(p - 1.0)*sqrt(3.0) * e_e*e_e*e_e * ksiN * nprime * B
                     / (m_e*v_light*v_light);
+
+    if(specType & DEEP_NEWTONIAN_FLAG)
+        em *= epsebar * e_th 
+                / (ksiN*nprime * g_m * m_e * v_light*v_light);
   
     double freq = 0.0; // frequency dependent part of emissivity
+    double back_pow = 10.0;
+    double eff_k = 3 - Msw / (4*M_PI*R*R*R*rho0);
 
+    if(specType & NO_COOLING_FLAG)
+        nu_c = 1.0e200;
 
     // set frequency dependence
     if (nu_c > nu_m)
     {
-        if (nuprime < nu_m) 
+        if (nuprime < nu_m)
+        {
             freq = pow(nuprime / nu_m, 1.0 / 3.0 );
+            back_pow = (28-11*eff_k)/(9*(4-eff_k));
+        }
         else if (nuprime < nu_c)
+        {
             freq = pow(nuprime / nu_m, 0.5 * (1.0 - p));
+            back_pow = (33+13*p - (15-p)*eff_k)/(12*(4-eff_k));
+        }
         else
+        {
             freq = pow(nu_c / nu_m, 0.5 * (1.0 - p))
                     * pow(nuprime / nu_c, -0.5*p);
+            back_pow = (-6+13*p - (6-p)*eff_k)/(12*(4-eff_k));
+        }
     }
     else
     {
         if (nuprime < nu_c)
+        {
             freq = pow(nuprime / nu_c, 1.0/3.0);
+            back_pow = (18-5*eff_k)/(3*(4-eff_k));
+        }
         else if (nuprime < nu_m)
+        {
             freq = sqrt(nu_c / nuprime);
+            back_pow = (7-5*eff_k)/(12*(4-eff_k));
+        }
         else
+        {
             freq = sqrt(nu_c/nu_m) * pow(nuprime / nu_m, -0.5 * p);
+            back_pow = (-6+13*p - (6-p)*eff_k)/(12*(4-eff_k));
+        }
     }
 
-
     if(em != em || em < 0.0)
     {
         fprintf(stderr, "bad em:%.3le te=%.3le mu=%.3lf\n",
                 em, te, mu);
         return -1;
     }
     if(freq != freq || freq < 0.0)
@@ -483,81 +684,161 @@
             abs_com_freq = pow(nuprime / nu_m, 1.0/3.0);
         else
             abs_com_freq = pow(nuprime / nu_m, -0.5*p);
 
         // Lab frame absorption coefficient
         double abs = abs_com_P * abs_com_freq * a*g;
 
+        double la = 0.0;
+        double lb = 0.0;
+
+        calc_absorption_length(R, mu, DR0/R, betaS, us, &la, &lb);
+
+        if(la < 0.0 || lb < 0.0)
+            return -1.0;
+
+        double taua = la * abs;
+        double taub = lb * abs;
+
+        /*
         // (Signed) Optical depth through this shell.
         // if negative, face is oriented away from observer.
         double dtau;
         if(mu == betaS)
             dtau = 1.0e100; // HUGE VAL, just in case
         else
             dtau = abs * DR * (1 - mu*betaS) / (mu - betaS);
+        */
 
 
         // Now that we know the optical depth, we apply it in a way
         // according to the given specType
 
         if((specType & SSA_SMOOTH_FLAG) && (specType & SSA_SHARP_FLAG))
         {
             //Special case: use the optically thick limit *everywhere*
+
+            double tau1 = taub;
+            double dtau = taua - taub;
+            double R_correction = 1.0;
+
+            if(taua < taub)
+            {
+                tau1 = taua;
+                dtau = taub - taua;
+                R_correction = (R-DR)/R;
+            }
+
+            em_lab *= R_correction*R_correction*exp(-tau1)/dtau;
+
+            /*
             if(dtau <= 0.0)
                 em_lab = 0.0;
             else
                 em_lab /= dtau;
+            */
         }
         else if(specType & SSA_SMOOTH_FLAG)
         {
             // Apply self-absorption "properly"
             //
             // correction factor to emissivity from absorption
             // ( 1 - e^(-tau) ) / tau  (on front face)
             //
             // back face has extra factor ~ e^-betaS/(mu-betaS)
             //
             // for now ignoring shadowing by the front face.
+            /*
             double abs_fac;
             if(dtau == 0.0)
                 abs_fac = 1.0;
             else if(dtau > 0.0)
                 abs_fac = -expm1(-dtau) / dtau;
             else
             {
-                abs_fac = expm1(dtau) / dtau; //* exp(
+                abs_fac = expm1(dtau) / dtau; // * exp(
                             //abs * DR * betaS*mu / (mu - betaS));
             }
+            */
+
+            double abs_fac = absorption_integral(R, DR, taua, taub, 0) 
+                                / (R*R*DR);
 
+            //printf("F %.6le %.6le %.6le %.6le %.6le %.6le\n", abs,
+            //        la, lb, taua, taub, abs_fac);
+                    
             em_lab *= abs_fac;
         }
         else if(specType & SSA_SHARP_FLAG)
         {
             // Apply self-absorption "simply".  
             //
             // Compute flux in optically thick limit,
             // use in final result if less than optically thin calculation.
             //
             // e.g. use tau->infty limit if tau > 1.0
 
+            double tau1 = taub;
+            double dtau = taua - taub;
+            double R_correction = 1.0;
+
+            if(taua < taub)
+            {
+                tau1 = taua;
+                dtau = taub - taua;
+                R_correction = (R-DR)/R;
+            }
+
+            double abs_fac = R_correction*R_correction*exp(-tau1)/dtau;
+
+            if(abs_fac < 1.0)
+                em_lab *= abs_fac;
+
+            /*
             // "Forward" face
             if(dtau > 1.0)
                 em_lab /= dtau;
             
             // "Back" face --> assume shadowed by front
             else if(dtau < -1.0)
                 em_lab = 0.0;
+            */
         }
     }
     if(specType < 0)
         em_lab = 1.0;
 
+    if(specType & BULK_BM_FLAG)
+    {
+        double d0 = DR / R;
+        double chi_peak = g*g*(1-mu*mu);
+        if(chi_peak > 1.0)
+        {
+            double d = d0 * (pow(chi_peak, 1-back_pow)-back_pow) / (1-back_pow);
+            DR = R * d;
+        }
+    }
+
+    if(specType & FIXED_PL_FLAG)
+        em_lab = epse/(g*g*a*a) * pow(nuprime, p-4);
+
     return R * R * DR * em_lab;
 }
 
+double get_u(double mu, struct fluxParams *pars)
+{
+    int ia = searchSorted(mu, pars->mu_table, pars->table_entries);
+    int ib = ia+1;
+    double t_e = interpolateLin(ia, ib, mu, pars->mu_table, pars->t_table, 
+                            pars->table_entries);
+    double u = interpolateLog(ia, ib, t_e, pars->t_table, pars->u_table,
+                                    pars->table_entries);
+    return u;
+}
+
 double costheta_integrand(double aomct, void* params) // inner integral
 {
     /*
      * This is the integrand for the inner integral, over theta.
      * The integral is actually performed over 1-cos(theta), 
      * which eliminates the geometrical sin(theta) factor the standard volume
      * element and retains numerical accuracy near theta=0.
@@ -582,14 +863,15 @@
 
     //double a_theta = acos(act);
     //double ast = sqrt((1.0 - act)*(1 + act));
     double mu = ast * (pars->cp) * (pars->sto) + act * (pars->cto);
 
     int ia = searchSorted(mu, pars->mu_table, pars->table_entries);
     int ib = ia+1;
+    pars->cur_entry = ia;
     double t_e = interpolateLin(ia, ib, mu, pars->mu_table, pars->t_table, 
                             pars->table_entries);
     t_e = check_t_e(t_e, mu, pars->t_obs, pars->mu_table, pars->table_entries);
 
     if(t_e < 0.0)
     {
         char msg[MSG_LEN];
@@ -597,16 +879,16 @@
         c += snprintf(msg, MSG_LEN-c,
                      "BAD t_e: %.6lf Eiso=%.3le n0=%.3le thetah=%.3le\n",
                      t_e, pars->E_iso, pars->n_0, pars->theta_h);
         c += snprintf(msg+c, MSG_LEN-c,
                       "    theta_obs=%.3lf phi=%.3lf theta=%.3lf mu=%.3lf\n",
                       pars->theta_obs, pars->phi, pars->theta, mu);
         c += snprintf(msg+c, MSG_LEN-c,
-                      "    L0=%.3le q=%.3lf ts=%.3le\n",
-                      pars->L0, pars->q, pars->ts);
+                    "    L0_inj=%.3le q_inj=%.3lf t0_inj=%.3le ts_inj=%.3le\n",
+                      pars->L0_inj, pars->q_inj, pars->t0_inj, pars->ts_inj);
         c += snprintf(msg+c, MSG_LEN-c,
                       "    t[0]=%.3le t[-1]=%.3le R[0]=%.3le R[-1]=%.3le\n",
                       pars->t_table[0], pars->t_table[pars->table_entries-1],
                       pars->R_table[0], pars->R_table[pars->table_entries-1]);
         c += snprintf(msg+c, MSG_LEN-c,
                       "    u[0]=%.3le u[-1]=%.3le th[0]=%.3le th[-1]=%.3le\n",
                       pars->u_table[0], pars->u_table[pars->table_entries-1],
@@ -618,17 +900,22 @@
     double R = interpolateLog(ia, ib, t_e, pars->t_table, pars->R_table, 
                             pars->table_entries);
 
     double us, u;
     u = interpolateLog(ia, ib, t_e, pars->t_table, pars->u_table,
                                     pars->table_entries);
     us = shockVel(u);
+
+    double rho0 = envDensity(R, pars->envType, m_p*pars->n_0, pars->R0_env,
+                             pars->k_env, pars->rho1_env);
+    double Msw = envMass(R, pars->envType, m_p*pars->n_0, pars->R0_env,
+                         pars->k_env, pars->rho1_env);
     
     double dFnu =  emissivity(pars->nu_obs, R, mu, t_e, u, us,
-                                pars->n_0, pars->p, pars->epsilon_E,
+                                rho0, Msw, pars->p, pars->epsilon_E,
                                 pars->epsilon_B, pars->ksi_N, pars->spec_type);
 
     if(dFnu != dFnu || dFnu < 0.0)
     {
         char msg[MSG_LEN];
         int c = 0;
         c += snprintf(msg, MSG_LEN,
@@ -638,20 +925,52 @@
                      "      t=%.3le u=%.3le us=%.3le n0=%.3le p=%.3lf\n",
                      t_e, u, us, pars->n_0, pars->p);
         c += snprintf(msg+c, MSG_LEN-c,
                      "      epse=%.3le epsB=%.3le ksiN=%.3le specType=%d\n",
                      pars->epsilon_E, pars->epsilon_B, pars->ksi_N,
                      pars->spec_type);
         c += snprintf(msg+c, MSG_LEN-c,
-                     "      Rt0=%.3le Rt1=%.3le E_iso=%.3le L0=%.3le ts=%.3le\n",
-                     pars->Rt0, pars->Rt1, pars->E_iso, pars->L0, pars->ts);
+                     "      Rt0=%.3le Rt1=%.3le E_iso=%.3le L0_inj=%.3le ts_inj=%.3le\n",
+                     pars->Rt0, pars->Rt1, pars->E_iso,
+                     pars->L0_inj, pars->ts_inj);
         set_error(pars, msg);
         return 0.0;
     }
 
+    double momentFactor = 1.0;
+    if(pars->moment > 0)
+    {
+        double xlab = R * ast * pars->cp;
+        double ylab = R * ast * pars->sp;
+        double zlab = R * act;
+
+        double xobs = -(pars->cto * xlab - pars->sto * zlab);
+        double yobs = -ylab;
+        double zobs = (pars->sto * xlab + pars->cto * zlab);
+
+        if(pars->moment == MOM_X)
+            momentFactor = xobs;
+        else if(pars->moment == MOM_Y)
+            momentFactor = yobs;
+        else if(pars->moment == MOM_Z)
+            momentFactor = zobs;
+        else if(pars->moment == MOM_XX)
+            momentFactor = xobs*xobs;
+        else if(pars->moment == MOM_YY)
+            momentFactor = yobs*yobs;
+        else if(pars->moment == MOM_ZZ)
+            momentFactor = zobs*zobs;
+        else if(pars->moment == MOM_XY)
+            momentFactor = xobs*yobs;
+        else if(pars->moment == MOM_YZ)
+            momentFactor = yobs*zobs;
+        else if(pars->moment == MOM_XZ)
+            momentFactor = xobs*zobs;
+    }
+
     int i;
     double fac = 1.0;
     for(i=0; i<pars->nmask; i++)
     {
         double *m = &((pars->mask)[9*i]);
         if(m[0]<t_e && t_e<m[1] && m[2]<R && R<m[3] && m[4]<a_theta
                 && a_theta<m[5] && m[6]<pars->phi && pars->phi<m[7])
@@ -662,80 +981,90 @@
     {
         char msg[MSG_LEN];
         snprintf(msg, MSG_LEN, "bad mask fac: %.3le\n", fac);
         set_error(pars, msg);
         return 0.0;
     }
 
-    return fac * dFnu;
+    return momentFactor * fac * dFnu;
 }
 
 ///////////////////////////////////////////////////////////////////////////////
 
 double phi_integrand(double a_phi, void* params) // outer integral
 {
     /*
      * This is the integrand for the (outer) phi integral. This is the
      * inner integral over ~theta.  For stability and smoothness, the
      * integral is performed over 1-cos(theta) instead of over theta 
      * itself.  It is good to know that 1 - cos(theta) = 2 * sin(theta/2)^2
      */
 
+    //printf("In phi_integrand. phi=%.16lf\n", a_phi);
+
     double result;
 
     struct fluxParams *pars = (struct fluxParams *) params;
   
     // set up integration routine
 
     pars->phi = a_phi;
     pars->cp = cos(a_phi);
+    pars->sp = sin(a_phi);
   
   // implement sideways spreading approximation until spherical symmetry reached
     double theta_1 = pars->current_theta_cone_hi;
     double theta_0 = pars->current_theta_cone_low;
     double Dtheta = theta_1 - theta_0;
     int spreadVersion = 1;
     if(pars->th_table != NULL && spreadVersion==1)
     {
         double th_0, th_1;
         th_1 = find_jet_edge(a_phi, pars->cto, pars->sto, theta_1,
                              pars->mu_table, pars->th_table,
-                             pars->table_entries);
+                             pars->table_entries,
+                             pars->idx_mu_neg1, pars->idx_mu_pos1,
+                             pars->cth_table, pars->sth_table);
 
         if(pars->table_entries_inner == 0)
         {
             double frac = theta_0 / theta_1;
             th_0 = frac * th_1;
         }
         else
         {
             th_0 = find_jet_edge(a_phi, pars->cto, pars->sto, theta_0,
                                  pars->mu_table_inner, pars->th_table_inner,
-                                 pars->table_entries_inner);
+                                 pars->table_entries_inner,
+                                 pars->idx_mu_neg1_inner,
+                                 pars->idx_mu_pos1_inner,
+                                 pars->cth_table_inner,
+                                 pars->sth_table_inner);
         }
         /*
         double frac = theta_0 / theta_1;
         double th_0 = frac * th_1;
         */
         theta_0 = th_0;
         theta_1 = th_1;
         if(theta_0 > 0.5*M_PI)
             theta_0 = 0.5*M_PI;
         if(theta_1 > 0.5*M_PI)
             theta_1 = 0.5*M_PI;
     }
-    if(pars->th_table != NULL && spreadVersion==2)
+    else if(pars->th_table != NULL && spreadVersion==2)
     {
         // approx mu
         double ct = cos(0.5*(theta_0+theta_1));
         double st = sin(0.5*(theta_0+theta_1));
         double mu = pars->cp * st * (pars->sto) + ct * (pars->cto);
 
         int ia = searchSorted(mu, pars->mu_table, pars->table_entries);
         int ib = ia+1;
+        pars->cur_entry = ia;
         double th = interpolateLin(ia, ib, mu, pars->mu_table, pars->th_table, 
                                     pars->table_entries);
 
         theta_0 *= th/pars->theta_h;
         theta_1 *= th/pars->theta_h;
         if(theta_0 > 0.5*M_PI)
             theta_0 = 0.5*M_PI;
@@ -746,26 +1075,32 @@
     {
         theta_1 = dmin(0.5 * PI, 
                         pars->theta_h + 0.1 * log( pars->t_obs / pars->t_NR));
         if(theta_0 != 0.0)
             theta_0 = theta_1-Dtheta;
     }
 
+    //printf("    In phi_integrand theta_0=%.16lf, theta_1=%.16lf\n",
+    //       theta_0, theta_1);
+
     if(theta_0 >= theta_1)
         return 0.0;
  
     //printf("# theta integration domain: %e - %e\n", theta_1 - Dtheta, theta_1); fflush(stdout);
  
     // For a given phi, integrate over 1 - cos(theta)
 
     double sht0 = sin(0.5*theta_0);
     double sht1 = sin(0.5*theta_1);
     double omct0 = 2 * sht0*sht0;
     double omct1 = 2 * sht1*sht1;
 
+    pars->current_theta_a = theta_0;
+    pars->current_theta_b = theta_1;
+
     if(pars->int_type == INT_TRAP_FIXED)
     {
         result = trap(&costheta_integrand, omct0, omct1, pars->nmax_theta,
                       params, check_error);
     }
     else if(pars->int_type == INT_TRAP_ADAPT)
     {
@@ -810,18 +1145,76 @@
         result = hybrid_adapt(&costheta_integrand, omct0, omct1,
                               pars->nmax_theta, pars->atol_theta,
                               pars->rtol_theta, params, NULL, NULL, 0,
                               check_error, NULL, NULL);
     }
     else if(pars->int_type == INT_CADRE)
     {
-        result = cadre_adapt(&costheta_integrand, omct0, omct1,
-                              pars->nmax_theta, pars->atol_theta,
-                              pars->rtol_theta, params, NULL, NULL, 0,
-                              check_error, NULL, NULL);
+        mesh9Free(&(pars->theta_mesh));
+        //printf("Start.  phi = %.16lf  (%.16lg, %.16lg)\n", a_phi,
+        //       theta_0, theta_1);
+       
+        double theta_obs = pars->theta_obs;
+
+        if(theta_obs > theta_0 && theta_obs < theta_1)
+        {
+            //double acto = 1 - omcto;
+            //double asto = sqrt(omcto * (1+acto));
+            //double mu = asto * (pars->cp) * (pars->sto) + acto * (pars->cto);
+
+            double u = get_u(1.0, pars);
+            double g = sqrt(1 + u*u);
+
+            if(a_phi * g < 4.0)
+            {
+                double shto = sin(0.5*theta_obs);
+                double omcto = 2 * shto*shto;
+
+                //printf("In middle  %le %le %le\n", theta_0, theta_obs, theta_1);
+                //printf("           %le %le %le\n", omct0, omcto, omct1);
+                
+                double result1 = cadre_adapt(&costheta_integrand, omct0, omcto,
+                                      pars->nmax_theta, pars->atol_theta,
+                                      pars->rtol_theta, params, NULL, NULL, 0,
+                                      check_error, NULL, NULL, &(pars->theta_mesh));
+                mesh9Free(&(pars->theta_mesh));
+                ERR_CHK_DBL(pars)
+                double result2 = cadre_adapt(&costheta_integrand, omcto, omct1,
+                                      pars->nmax_theta, pars->atol_theta,
+                                      pars->rtol_theta, params, NULL, NULL, 0,
+                                      check_error, NULL, NULL, &(pars->theta_mesh));
+                /*
+                mesh9Free(&(pars->theta_mesh));
+                ERR_CHK_DBL(pars)
+                double result0 = cadre_adapt(&costheta_integrand, omct0, omct1,
+                                      pars->nmax_theta, pars->atol_theta,
+                                      pars->rtol_theta, params, NULL, NULL, 0,
+                                      check_error, NULL, NULL, &(pars->theta_mesh));
+                printf("           %le %le %le\n", result0, result1, result2);
+                */
+
+                result = result1 + result2;
+            }
+            else
+            {
+                result = cadre_adapt(&costheta_integrand, omct0, omct1,
+                                      pars->nmax_theta, pars->atol_theta,
+                                      pars->rtol_theta, params, NULL, NULL, 0,
+                                      check_error, NULL, NULL, &(pars->theta_mesh));
+            }
+        }
+        else
+        {
+            result = cadre_adapt(&costheta_integrand, omct0, omct1,
+                                  pars->nmax_theta, pars->atol_theta,
+                                  pars->rtol_theta, params, NULL, NULL, 0,
+                                  check_error, NULL, NULL, &(pars->theta_mesh));
+        }
+        //printf("           %le  %le\n", pars->nu_obs, result);
+        //printf("End.\n");
     }
     else if(pars->int_type == INT_GK49_ADAPT)
     {
         result = gk49_adapt(&costheta_integrand, omct0, omct1,
                               pars->nmax_theta, pars->atol_theta,
                               pars->rtol_theta, params, NULL, NULL, 0,
                               check_error);
@@ -846,35 +1239,37 @@
         snprintf(msg, MSG_LEN,
                  "Unknown integrator %d!  Aborting.\n", pars->int_type);
         set_error(pars, msg);
         return 0.0;
     }
     ERR_CHK_DBL(pars)
 
-    if(result != result || result < 0.0)
+    if(result != result || (result < 0.0 && pars->moment == MOM_0))
     {
         char msg[MSG_LEN];
         int c = 0;
         c += snprintf(msg, MSG_LEN,
                      "bad result in phi_integrand :%.3le\n", result);
 
         c += snprintf(msg+c, MSG_LEN-c,
                      "   t_obs=%.3le theta_lo=%.3lf theta_hi=%.3lf phi=%.3lf\n",
                      pars->t_obs, theta_0, theta_1, pars->phi);
         set_error(pars, msg);
         return 0.0;
     }
   
-    //printf("   a_phi: %.6lf (%.6le)\n", a_phi, result);
+    //printf("Leaving phi_integrand: %.6lf (%.6le)\n", a_phi, result);
 
     return result;
 }
 
-double find_jet_edge(double phi, double cto, double sto, double theta0,
-                     double *a_mu, double *a_thj, int N)
+double find_jet_edge_old(double phi, double cto, double sto, double theta0,
+                     const double *a_mu, const double *a_thj, int N,
+                     int idx_mu_neg1, int idx_mu_pos1,
+                     const double *a_cthj, const double *a_sthj)
 {
     /*
      *
      * Return the (outer) edge of the jet section for a particular obs.
      *
      * phi: double
      *      phi-coordinate of jet along which to search
@@ -887,55 +1282,130 @@
      * a_mu: double array
      *      time-ordered array of mu values for this observation.
      *      mu = c * (t_em - t_obs) / R(t_em)
      *         = cos(th_obs)*cos(theta) + sin(theta_obs)*sin(theta)*cos(phi)
      * a_thj: double array
      *      time ordered array of jet-edge values.
      */
-    
+
     double cp = cos(phi);
     double mu = cos(theta0)*cto + sin(theta0)*sto*cp;
 
-    int ia = searchSorted(mu, a_mu, N);
+    int ia0 = searchSorted(mu, a_mu, N);
     
-    if(a_thj[ia] <= theta0 && theta0 <= a_thj[ia+1])
+    if(a_thj[ia0] <= theta0 && theta0 <= a_thj[ia0+1])
+    {
         return theta0;
+    }
 
     double tha, thb;
-    if(theta0 < a_thj[ia])
+    if(theta0 < a_thj[ia0])
     {
         //The jet is spreading
         tha = theta0;
         thb = 0.5*M_PI;
     }
     else
     {
         //Guessed too far out!
         tha = 0.0;
         thb = theta0;
     }
 
-    int i = 0;
-    while(thb-tha > 1.0e-5 && i < 100)
+    int iter_count = 0;
+    int ia;
+    while(thb-tha > 1.0e-5 && iter_count < 100)
     {
         double th = 0.5*(tha+thb);
         mu = cos(th)*cto + sin(th)*sto*cp;
         ia = searchSorted(mu, a_mu, N);
         if(th < a_thj[ia])
             tha = th;
         else
             thb = th;
-        i++;
+        iter_count++;
     }
 
-    //printf("iter: %d, th0=%.6lf, th=%.6lf\n", i, theta0, tha);
-
     return tha;
 }
 
+double find_jet_edge(double phi, double cto, double sto, double theta0,
+                      const double *a_mu, const double *a_thj, int N,
+                      int idx_mu_neg1, int idx_mu_pos1,
+                      const double *a_cthj, const double *a_sthj)
+{
+    /*
+     *
+     * Return the (outer) edge of the jet section for a particular obs.
+     *
+     * phi: double
+     *      phi-coordinate of jet along which to search
+     * cto: double
+     *      cos(theta_obs) cosine of observer angle
+     * sto: double
+     *      sin(theta_obs) sine of observer angle
+     * theta0: double
+     *      
+     * a_mu: double array
+     *      time-ordered array of mu values for this observation.
+     *      mu = c * (t_em - t_obs) / R(t_em)
+     *         = cos(th_obs)*cos(theta) + sin(theta_obs)*sin(theta)*cos(phi)
+     * a_thj: double array
+     *      time ordered array of jet-edge values.
+     */
+    
+    double sto_cp = sto * cos(phi);
+    // Find the (lab) time indices that bracket mu(t) == mu(th)
+    // Assuming that mu(t) is increasing, a solution exists,
+    // and mu(t=0) < mu(th(t=0))
+    
+
+    unsigned int ita = idx_mu_neg1;
+    unsigned int itb = idx_mu_pos1;
+
+    double th_a, th_b, mu_th_a, mu_th_b, mu_t_a, mu_t_b;
+
+    while(itb - ita > 1u)
+    {
+        unsigned int i = (ita + itb) >> 1;
+        //double th = a_thj[i];
+        //double mu_th = cos(th)*cto + sin(th)*sto_cp;
+        double mu_th = a_cthj[i]*cto + a_sthj[i]*sto_cp;
+
+        if(a_mu[i] < mu_th)
+            ita = i;
+        else
+            itb = i;
+    }
+
+    // Now ita and itb = ita + 1 should bracket the solution.
+    // Do a quick interpolation to refine the solution inside the bracket.
+    
+    th_a = a_thj[ita];
+    th_b = a_thj[itb];
+    //mu_th_a = cos(th_a)*cto + sin(th_a)*sto_cp;
+    //mu_th_b = cos(th_b)*cto + sin(th_b)*sto_cp;
+    mu_th_a = a_cthj[ita]*cto + a_sthj[ita]*sto_cp;
+    mu_th_b = a_cthj[itb]*cto + a_sthj[itb]*sto_cp;
+    mu_t_a = a_mu[ita];
+    mu_t_b = a_mu[itb];
+    
+    // find the mu where mu(t) crosses mu(th)
+    double mu_th = (mu_t_b * mu_th_a - mu_t_a * mu_th_b)
+                    / ((mu_t_b - mu_t_a) - (mu_th_b - mu_th_a));
+
+    //Could do a non-linear inversion here, but let's settle for a linear one:
+    double th1 = 0.5*(th_a + th_b);
+    if(th_a != th_b)
+        th1 = ((mu_th_b - mu_th) * th_a + (mu_th - mu_th_a) * th_b)
+                / (mu_th_b - mu_th_a);
+
+    return th1;
+}
+
 
 ///////////////////////////////////////////////////////////////////////////////
 
 double flux(struct fluxParams *pars, double atol) // determine flux for a given t_obs
 {
     double result;
     double phi_0 = 0.0;
@@ -1007,18 +1477,22 @@
         result = 2 * Fcoeff * hybrid_adapt(&phi_integrand, phi_0, phi_1,
                                            pars->nmax_phi, atol/(2*Fcoeff),
                                            pars->rtol_phi, pars, NULL, NULL,
                                            0, check_error, NULL, NULL);
     }
     else if(pars->int_type == INT_CADRE)
     {
+        mesh9Free(&(pars->phi_mesh));
+        //printf("Start.\n");
         result = 2 * Fcoeff * cadre_adapt(&phi_integrand, phi_0, phi_1,
                                            pars->nmax_phi, atol/(2*Fcoeff),
                                            pars->rtol_phi, pars, NULL, NULL,
-                                           0, check_error, NULL, NULL);
+                                           0, check_error, NULL, NULL,
+                                           &(pars->phi_mesh));
+        //printf("End.\n");
     }
     else if(pars->int_type == INT_GK49_ADAPT)
     {
         result = 2 * Fcoeff * gk49_adapt(&phi_integrand, phi_0, phi_1,
                                            pars->nmax_phi, atol/(2*Fcoeff),
                                            pars->rtol_phi, pars, NULL, NULL,
                                            0, check_error);
@@ -1044,15 +1518,15 @@
                  "Unknown integrator %d!  Aborting.\n", pars->int_type);
         set_error(pars, msg);
         return 0.0;
     }
 
     ERR_CHK_DBL(pars)
     
-    if(result != result || result < 0.0)
+    if(result != result || (result < 0.0 && pars->moment == MOM_0))
     {
         char msg[MSG_LEN];
         int c = 0;
         c += snprintf(msg, MSG_LEN,
                      "bad result in flux() :%.3le\n", result);
 
         c += snprintf(msg+c, MSG_LEN-c,
@@ -1061,49 +1535,61 @@
                      pars->current_theta_cone_hi);
         c += snprintf(msg+c, MSG_LEN-c,
                 "   Fcoeff=%.6le\n", Fcoeff);
         set_error(pars, msg);
         return 0.0;
     }
 
+    if(pars->moment == MOM_Y || pars->moment == MOM_XY
+        || pars->moment == MOM_YZ)
+    {
+        result = 0.0;
+    }
+
+    mesh9Free(&(pars->theta_mesh));
+    mesh9Free(&(pars->phi_mesh));
+
     return result;
 }
 
-void lc_cone(double *t, double *nu, double *F, int Nt, double E_iso,
-                double theta_core, double theta_wing, struct fluxParams *pars)
+void lc_cone(double *t, double *nu, double *F, long *moment, int Nt,
+             double E_iso, double theta_core, double theta_wing,
+             struct fluxParams *pars)
 {
     int i;
 
     set_jet_params(pars, E_iso, theta_wing);
     ERR_CHK_VOID(pars)
 
     for(i=0; i<Nt; i++)
     {
-        F[i] = flux_cone(t[i], nu[i], -1, -1, theta_core, theta_wing, 0.0,
+        long mom = moment == NULL ? 0 : moment[i];
+        F[i] = flux_cone(t[i], nu[i], mom, -1, -1, theta_core, theta_wing, 0.0,
                             pars);
         ERR_CHK_VOID(pars)
     }
 }
 
-void lc_tophat(double *t, double *nu, double *F, int Nt,
+void lc_tophat(double *t, double *nu, double *F, long *moment, int Nt,
                 double E_iso, double theta_h, struct fluxParams *pars)
 {
     int i;
 
     set_jet_params(pars, E_iso, theta_h);
     ERR_CHK_VOID(pars)
 
     for(i=0; i<Nt; i++)
     {
-        F[i] = flux_cone(t[i], nu[i], -1, -1, 0.0, theta_h, 0.0, pars);
+        long mom = moment == NULL ? 0 : moment[i];
+        F[i] = flux_cone(t[i], nu[i], mom, -1, -1, 0.0, theta_h, 0.0, pars);
         ERR_CHK_VOID(pars)
     }
 }
 
-void lc_struct(double *t, double *nu, double *F, int Nt,
+void lc_struct(double *t, double *nu, double *F, long *moment, int Nt,
                         double E_iso_core, 
                         double theta_h_core, double theta_h_wing,
                         double *theta_c_arr, double *E_iso_arr,
                         int res_cones, double (*f_E)(double,void *),
                         struct fluxParams *pars)
 {
     //Flux from a structured jet.
@@ -1139,33 +1625,34 @@
 
         set_jet_params(pars, E_iso, theta_h);
         ERR_CHK_VOID(pars)
 
         for(j=0; j<Nt; j++)
         {
             //printf("tobs = %.6le\n", t[j]);
-            F[j] += flux_cone(t[j], nu[j], -1, -1, theta_cone_low,
+            long mom = moment == NULL ? 0 : moment[j];
+            F[j] += flux_cone(t[j], nu[j], mom, -1, -1, theta_cone_low,
                                 theta_cone_hi,
-                                F[j]*pars->rtol_struct/res_cones,
+                                fabs(F[j])*pars->rtol_struct/res_cones,
                                 pars);
             ERR_CHK_VOID(pars)
         }
     }
 }
 
-void lc_structCore(double *t, double *nu, double *F, int Nt,
+void lc_structCore(double *t, double *nu, double *F, long *moment, int Nt,
                         double E_iso_core, 
                         double theta_h_core, double theta_h_wing,
-                        double *theta_c_arr, double *E_iso_arr,
+                                double *theta_c_arr, double *E_iso_arr,
                         int res_cones, double (*f_E)(double,void *),
                         struct fluxParams *pars)
 {
     //Flux from a structured jet with core.
     
-    lc_tophat(t, nu, F, Nt, E_iso_core, theta_h_core, pars);
+    lc_tophat(t, nu, F, moment, Nt, E_iso_core, theta_h_core, pars);
     ERR_CHK_VOID(pars)
 
     double Dtheta, theta_cone_hi, theta_cone_low, theta_h, theta_c, E_iso;
 
     Dtheta = (theta_h_wing - theta_h_core) / res_cones;
 
     int i,j;
@@ -1187,24 +1674,26 @@
             continue;
 
         set_jet_params(pars, E_iso, theta_h);
         ERR_CHK_VOID(pars)
 
         for(j=0; j<Nt; j++)
         {
-            F[j] += flux_cone(t[j], nu[j], -1, -1, theta_cone_low,
+            long mom = moment == NULL ? 0 : moment[j];
+            F[j] += flux_cone(t[j], nu[j], mom, -1, -1, theta_cone_low,
                                 theta_cone_hi,
-                                F[j]*pars->rtol_struct/res_cones,
+                                fabs(F[j])*pars->rtol_struct/res_cones,
                                 pars);
             ERR_CHK_VOID(pars)
         }
     }
 }
 
-double flux_cone(double t_obs, double nu_obs, double E_iso, double theta_h,
+double flux_cone(double t_obs, double nu_obs, long moment,
+                    double E_iso, double theta_h,
                     double theta_cone_low, double theta_cone_hi, double atol,
                     struct fluxParams *pars)
 {
     //printf("      t: %.3le th1: %.3f th2 %.3f\n", t_obs, theta_cone_low,
     //        theta_cone_hi);
 
     double theta_obs, theta_obs_cur;
@@ -1216,45 +1705,45 @@
     {
         set_jet_params(pars, E_iso, theta_h);
         ERR_CHK_DBL(pars)
     }
 
     //Jet 
     theta_obs_cur = theta_obs;
-    set_obs_params(pars, t_obs, nu_obs, theta_obs_cur, 
+    set_obs_params(pars, t_obs, nu_obs, moment, theta_obs_cur, 
                     theta_cone_hi, theta_cone_low);
     F1 = flux(pars, atol);
     ERR_CHK_DBL(pars)
     
     //Counter-jet
     if(pars->counterjet)
     {
-        theta_obs_cur = 180*deg2rad - theta_obs;
-        set_obs_params(pars, t_obs, nu_obs, theta_obs_cur, 
+        theta_obs_cur = 180*deg2rad + theta_obs;
+        set_obs_params(pars, t_obs, nu_obs, moment, theta_obs_cur, 
                         theta_cone_hi, theta_cone_low);
         F2 = flux(pars, atol);
         ERR_CHK_DBL(pars)
     }
     else
         F2 = 0.0;
     
     Fboth = F1 + F2;
 
 
-    if(F1 != F1 || F1 < 0.0)
+    if(F1 != F1 || (F1 < 0.0 && pars->moment == MOM_0))
     {
         char msg[MSG_LEN];
         int c = snprintf(msg, MSG_LEN, "bad F1 in flux_cone:%.3lg\n", F1);
         c += snprintf(msg+c, MSG_LEN-c,
                       "      t_obs=%.3le theta_lo=%.3lf theta_hi=%.3lf\n",
                       t_obs, theta_cone_low, theta_cone_hi);
         set_error(pars, msg);
         return 0.0;
     }
-    if(F2 != F2 || F2 < 0.0)
+    if(F2 != F2 || (F2 < 0.0 && pars->moment == MOM_0))
     {
         char msg[MSG_LEN];
         int c = snprintf(msg, MSG_LEN, "bad F2 in flux_cone:%.3lg\n", F2);
         c += snprintf(msg+c, MSG_LEN-c,
                       "      t_obs=%.3le theta_lo=%.3lf theta_hi=%.3lf\n",
                       t_obs, theta_cone_low, theta_cone_hi);
         set_error(pars, msg);
@@ -1271,25 +1760,29 @@
                 struct fluxParams *pars)
 {
     double I = 0;
 
     int remakeMu = 0;
     if(tobs != pars->t_obs)
         remakeMu = 1;
-    set_obs_params(pars, tobs, nuobs, theta_obs, theta_cone_hi, 
+    set_obs_params(pars, tobs, nuobs, 0, theta_obs, theta_cone_hi, 
                     theta_cone_low);
 
     if(remakeMu)
+    {
+        //printf("Remaking mu\n");
         make_mu_table(pars);
+    }
 
     double mu = cos(theta)*cos(theta_obs)
                     + sin(theta)*sin(theta_obs)*cos(phi);
 
     int ia = searchSorted(mu, pars->mu_table, pars->table_entries);
     int ib = ia + 1;
+    pars->cur_entry = ia;
     double t_e = interpolateLin(ia, ib, mu, pars->mu_table,
                                 pars->t_table, pars->table_entries);
     t_e = check_t_e(t_e, mu, pars->t_obs, pars->mu_table, 
                                 pars->table_entries);
     if(t_e < 0.0)
     {
         char msg[MSG_LEN];
@@ -1297,16 +1790,16 @@
         c += snprintf(msg, MSG_LEN-c,
                      "BAD t_e: %.6lf Eiso=%.3le n0=%.3le thetah=%.3le\n",
                      t_e, pars->E_iso, pars->n_0, pars->theta_h);
         c += snprintf(msg+c, MSG_LEN-c,
                       "    theta_obs=%.3lf phi=%.3lf theta=%.3lf mu=%.3lf\n",
                       pars->theta_obs, pars->phi, pars->theta, mu);
         c += snprintf(msg+c, MSG_LEN-c,
-                      "    L0=%.3le q=%.3lf ts=%.3le\n",
-                      pars->L0, pars->q, pars->ts);
+                    "    L0_inj=%.3le q_inj=%.3lf t0_inj=%.3le ts_inj=%.3le\n",
+                      pars->L0_inj, pars->q_inj, pars->t0_inj, pars->ts_inj);
         c += snprintf(msg+c, MSG_LEN-c,
                       "    t[0]=%.3le t[-1]=%.3le R[0]=%.3le R[-1]=%.3le\n",
                       pars->t_table[0], pars->t_table[pars->table_entries-1],
                       pars->R_table[0], pars->R_table[pars->table_entries-1]);
         c += snprintf(msg+c, MSG_LEN-c,
                       "    u[0]=%.3le u[-1]=%.3le th[0]=%.3le th[-1]=%.3le\n",
                       pars->u_table[0], pars->u_table[pars->table_entries-1],
@@ -1316,41 +1809,47 @@
     }
 
     double R = interpolateLog(ia, ib, t_e, pars->t_table,
                                 pars->R_table, pars->table_entries);
     double u = interpolateLog(ia, ib, t_e, pars->t_table,
                                 pars->u_table, pars->table_entries);
     double us = shockVel(u);
+    
+    double rho0 = envDensity(R, pars->envType, m_p*pars->n_0, pars->R0_env,
+                             pars->k_env, pars->rho1_env);
+    double Msw = envMass(R, pars->envType, m_p*pars->n_0, pars->R0_env,
+                         pars->k_env, pars->rho1_env);
 
-    I = emissivity(pars->nu_obs, R, mu, t_e, u, us, pars->n_0,
+    I = emissivity(pars->nu_obs, R, mu, t_e, u, us, rho0, Msw,
                         pars->p, pars->epsilon_E, pars->epsilon_B, 
                         pars->ksi_N, pars->spec_type);
 
     return I;
 }
 
 void shockVals(double theta, double phi, double tobs,
                  double *t, double *R, double *u, double *thj,
                  double theta_obs, double theta_cone_hi, double theta_cone_low,
                  struct fluxParams *pars)
 {
     int remakeMu = 0;
     if(tobs != pars->t_obs)
         remakeMu = 1;
-    set_obs_params(pars, tobs, 1.0, theta_obs, theta_cone_hi, 
+    set_obs_params(pars, tobs, 1.0, 0, theta_obs, theta_cone_hi, 
                     theta_cone_low);
 
     if(remakeMu)
         make_mu_table(pars);
 
     double mu = cos(theta)*cos(theta_obs)
                     + sin(theta)*sin(theta_obs)*cos(phi);
 
     int ia = searchSorted(mu, pars->mu_table, pars->table_entries);
     int ib = ia + 1;
+    pars->cur_entry = ia;
     double t_e = interpolateLin(ia, ib, mu, pars->mu_table,
                                 pars->t_table, pars->table_entries);
     t_e = check_t_e(t_e, mu, pars->t_obs, pars->mu_table, 
                                 pars->table_entries);
     if(t_e < 0.0)
     {
         char msg[MSG_LEN];
@@ -1358,16 +1857,16 @@
         c += snprintf(msg, MSG_LEN-c,
                      "BAD t_e: %.6lf Eiso=%.3le n0=%.3le thetah=%.3le\n",
                      t_e, pars->E_iso, pars->n_0, pars->theta_h);
         c += snprintf(msg+c, MSG_LEN-c,
                       "    theta_obs=%.3lf phi=%.3lf theta=%.3lf mu=%.3lf\n",
                       pars->theta_obs, pars->phi, pars->theta, mu);
         c += snprintf(msg+c, MSG_LEN-c,
-                      "    L0=%.3le q=%.3lf ts=%.3le\n",
-                      pars->L0, pars->q, pars->ts);
+                    "    L0_inj=%.3le q_inj=%.3lf t0_inj=%.3le ts_inj=%.3le\n",
+                      pars->L0_inj, pars->q_inj, pars->t0_inj, pars->ts_inj);
         c += snprintf(msg+c, MSG_LEN-c,
                       "    t[0]=%.3le t[-1]=%.3le R[0]=%.3le R[-1]=%.3le\n",
                       pars->t_table[0], pars->t_table[pars->table_entries-1],
                       pars->R_table[0], pars->R_table[pars->table_entries-1]);
         c += snprintf(msg+c, MSG_LEN-c,
                       "    u[0]=%.3le u[-1]=%.3le th[0]=%.3le th[-1]=%.3le\n",
                       pars->u_table[0], pars->u_table[pars->table_entries-1],
@@ -1402,46 +1901,52 @@
     double Fcoeff = cgs2mJy / (4*M_PI*dL*dL);
 
     double theta_cone_hi = theta_h_wing;
     double theta_cone_low = theta_h_core;
 
     set_jet_params(pars, E_iso_core, theta_h_wing);
     ERR_CHK_VOID(pars)
-    set_obs_params(pars, t[0], nu[0], theta_obs,
+    set_obs_params(pars, t[0], nu[0], 0, theta_obs,
                    theta_cone_hi, theta_cone_low);
     make_mu_table(pars);
     double tobs = t[0];
 
     for(j=0; j<N; j++)
     {
         double th = theta[j];
         double ph = phi[j];
 
         if(I[j] > 0.0 || th < theta_cone_low)
             continue;
 
-        set_obs_params(pars, t[j], nu[j], theta_obs,
+        set_obs_params(pars, t[j], nu[j], 0, theta_obs,
                        theta_cone_hi, theta_cone_low);
         if(tobs != t[j])
         {
             make_mu_table(pars);
             tobs = t[j];
         }
 
         double th_a, th_b;
         th_b = find_jet_edge(ph, pars->cto, pars->sto, theta_cone_hi,
                              pars->mu_table, pars->th_table,
-                             pars->table_entries);
+                             pars->table_entries,
+                             pars->idx_mu_neg1, pars->idx_mu_pos1,
+                             pars->cth_table, pars->sth_table);
         if(pars->table_entries_inner == 0)
             th_a = (theta_cone_low / theta_cone_hi) * th_b;
         else
             th_a = find_jet_edge(ph, pars->cto, pars->sto, theta_cone_low,
                                  pars->mu_table_inner, 
                                  pars->th_table_inner,
-                                 pars->table_entries_inner);
+                                 pars->table_entries_inner,
+                                 pars->idx_mu_neg1_inner,
+                                 pars->idx_mu_pos1_inner,
+                                 pars->cth_table_inner,
+                                 pars->sth_table_inner);
 
         if(th < th_a || th > th_b)
             continue;
 
         I[j] = Fcoeff * intensity(th, ph, t[j], nu[j], theta_obs,        
                                     theta_cone_hi, theta_cone_low, pars);
     }
@@ -1478,15 +1983,15 @@
         theta_cone_hi = (i+1) * Dtheta;
         theta_cone_low = i * Dtheta;
         theta_h = theta_cone_hi;
 
         set_jet_params(pars, E_iso, theta_h);
         ERR_CHK_VOID(pars)
 
-        set_obs_params(pars, t[0], nu[0], theta_obs, theta_cone_hi, 
+        set_obs_params(pars, t[0], nu[0], 0, theta_obs, theta_cone_hi, 
                        theta_cone_low);
         make_mu_table(pars);
         double tobs = t[0];
 
         //printf("Cone: %d of %d\n", i, res_cones);
 
         for(j=0; j<N; j++)
@@ -1494,35 +1999,41 @@
             double th = theta[j];
             double ph = phi[j];
 
             if(I[j] > 0.0 || th < theta_cone_low)
                 continue;
 
 
-            set_obs_params(pars, t[j], nu[j], theta_obs, theta_cone_hi, 
+            set_obs_params(pars, t[j], nu[j], 0, theta_obs, theta_cone_hi, 
                             theta_cone_low);
             if(tobs != t[j])
             {
                 make_mu_table(pars);
                 tobs = t[j];
             }
 
             double th_a, th_b;
             th_b = find_jet_edge(ph, pars->cto, pars->sto, theta_cone_hi,
                                  pars->mu_table, pars->th_table,
-                                 pars->table_entries);
+                                 pars->table_entries,
+                                 pars->idx_mu_neg1, pars->idx_mu_pos1,
+                             pars->cth_table, pars->sth_table);
             ERR_CHK_VOID(pars)
             if(pars->table_entries_inner == 0)
                 th_a = (theta_cone_low / theta_cone_hi) * th_b;
             else
             {
                 th_a = find_jet_edge(ph, pars->cto, pars->sto, theta_cone_low,
                                      pars->mu_table_inner, 
                                      pars->th_table_inner,
-                                     pars->table_entries_inner);
+                                     pars->table_entries_inner,
+                                     pars->idx_mu_neg1_inner,
+                                     pars->idx_mu_pos1_inner,
+                                 pars->cth_table_inner,
+                                 pars->sth_table_inner);
                 ERR_CHK_VOID(pars)
             }
 
             if(th < th_a || th > th_b)
                 continue;
 
             I[j] += Fcoeff * intensity(th, ph, t[j], nu[j], theta_obs,        
@@ -1563,48 +2074,55 @@
 
         theta_cone_hi = (i+1) * Dtheta;
         theta_cone_low = i * Dtheta;
         theta_h = theta_cone_hi;
 
         set_jet_params(pars, E_iso, theta_h);
         ERR_CHK_VOID(pars)
-        set_obs_params(pars, t[0], nu[0], theta_obs, theta_cone_hi, 
+        set_obs_params(pars, t[0], nu[0], 0, theta_obs, theta_cone_hi, 
                         theta_cone_low);
         make_mu_table(pars);
         double tobs = t[0];
         
         for(j=0; j<N; j++)
         {
             double th = theta[j];
             double ph = phi[j];
             
             if(I[j] > 0.0 || th < theta_cone_low)
                 continue;
 
-            set_obs_params(pars, t[j], nu[j], theta_obs, theta_cone_hi, 
+            set_obs_params(pars, t[j], nu[j], 0, theta_obs, theta_cone_hi, 
                             theta_cone_low);
             if(tobs != t[j])
             {
                 make_mu_table(pars);
                 tobs = t[j];
             }
 
             double th_a, th_b;
             th_b = find_jet_edge(ph, pars->cto, pars->sto, theta_cone_hi,
                                  pars->mu_table, pars->th_table,
-                                 pars->table_entries);
+                                 pars->table_entries,
+                                 pars->idx_mu_neg1, pars->idx_mu_pos1,
+                             pars->cth_table, pars->sth_table);
             ERR_CHK_VOID(pars)
             if(pars->table_entries_inner == 0)
                 th_a = (theta_cone_low / theta_cone_hi) * th_b;
             else
             {
                 th_a = find_jet_edge(ph, pars->cto, pars->sto, theta_cone_low,
                                      pars->mu_table_inner, 
                                      pars->th_table_inner,
-                                     pars->table_entries_inner);
+                                     pars->table_entries_inner,
+                                     pars->idx_mu_neg1_inner,
+                                     pars->idx_mu_pos1_inner,
+                                 pars->cth_table_inner,
+                                 pars->sth_table_inner);
+
                 ERR_CHK_VOID(pars)
             }
 
             if(th < th_a || th > th_b)
                 continue;
 
             I[j] += Fcoeff * intensity(th, ph, t[j], nu[j], theta_obs,        
@@ -1616,15 +2134,15 @@
 
 void shockVals_cone(double *theta, double *phi, double *tobs,
                     double *t, double *R, double *u, double *thj, 
                     int N, double E_iso_core, 
                     double theta_h_core, double theta_h_wing, 
                     struct fluxParams *pars)
 {
-    //Intensity of a cone segment.
+    //shockVals of a cone segment.
     
     int j;
     for(j=0; j<N; j++)
     {
         t[j] = 0.0;
         R[j] = 0.0;
         u[j] = 0.0;
@@ -1634,48 +2152,54 @@
     double theta_obs = pars->theta_obs;
 
     double theta_cone_hi = theta_h_wing;
     double theta_cone_low = theta_h_core;
 
     set_jet_params(pars, E_iso_core, theta_h_wing);
     ERR_CHK_VOID(pars)
-    set_obs_params(pars, tobs[0], 1.0, theta_obs, theta_cone_hi, 
+    set_obs_params(pars, tobs[0], 1.0, 0, theta_obs, theta_cone_hi, 
                     theta_cone_low);
     make_mu_table(pars);
     double tobs_cur = t[0];
 
     for(j=0; j<N; j++)
     {
         double th = theta[j];
         double ph = phi[j];
 
         if(t[j] > 0.0 || th < theta_cone_low)
             continue;
 
-        set_obs_params(pars, tobs[j], 1.0, theta_obs,
+        set_obs_params(pars, tobs[j], 1.0, 0, theta_obs,
                        theta_cone_hi, theta_cone_low);
         if(tobs_cur != tobs[j])
         {
             make_mu_table(pars);
             tobs_cur = tobs[j];
         }
 
         double th_a, th_b;
         th_b = find_jet_edge(ph, pars->cto, pars->sto, theta_cone_hi,
                              pars->mu_table, pars->th_table,
-                             pars->table_entries);
+                             pars->table_entries,
+                             pars->idx_mu_neg1, pars->idx_mu_pos1,
+                             pars->cth_table, pars->sth_table);
         ERR_CHK_VOID(pars)
         if(pars->table_entries_inner == 0)
             th_a = (theta_cone_low / theta_cone_hi) * th_b;
         else
         {
             th_a = find_jet_edge(ph, pars->cto, pars->sto, theta_cone_low,
                                  pars->mu_table_inner, 
                                  pars->th_table_inner,
-                                 pars->table_entries_inner);
+                                 pars->table_entries_inner,
+                                 pars->idx_mu_neg1_inner,
+                                 pars->idx_mu_pos1_inner,
+                                 pars->cth_table_inner,
+                                 pars->sth_table_inner);
             ERR_CHK_VOID(pars)
         }
 
         if(th < th_a || th > th_b)
             continue;
 
         shockVals(th, ph, tobs[j], t+j, R+j, u+j, thj+j,
@@ -1716,48 +2240,54 @@
 
         theta_cone_hi = (i+1) * Dtheta;
         theta_cone_low = i * Dtheta;
         theta_h = theta_cone_hi;
 
         set_jet_params(pars, E_iso, theta_h);
         ERR_CHK_VOID(pars)
-        set_obs_params(pars, tobs[0], 1.0, theta_obs, theta_cone_hi, 
+        set_obs_params(pars, tobs[0], 1.0, 0, theta_obs, theta_cone_hi, 
                         theta_cone_low);
         make_mu_table(pars);
         double tobs_cur = t[0];
 
         for(j=0; j<N; j++)
         {
             double th = theta[j];
             double ph = phi[j];
 
             if(t[j] > 0.0 || th < theta_cone_low)
                 continue;
 
-            set_obs_params(pars, tobs[j], 1.0, theta_obs, theta_cone_hi, 
+            set_obs_params(pars, tobs[j], 1.0, 0, theta_obs, theta_cone_hi, 
                             theta_cone_low);
             if(tobs_cur != tobs[j])
             {
                 make_mu_table(pars);
                 tobs_cur = tobs[j];
             }
 
             double th_a, th_b;
             th_b = find_jet_edge(ph, pars->cto, pars->sto, theta_cone_hi,
                                  pars->mu_table, pars->th_table,
-                                 pars->table_entries);
+                                 pars->table_entries,
+                                 pars->idx_mu_neg1, pars->idx_mu_pos1,
+                             pars->cth_table, pars->sth_table);
             ERR_CHK_VOID(pars)
             if(pars->table_entries_inner == 0)
                 th_a = (theta_cone_low / theta_cone_hi) * th_b;
             else
             {
                 th_a = find_jet_edge(ph, pars->cto, pars->sto, theta_cone_low,
                                      pars->mu_table_inner, 
                                      pars->th_table_inner,
-                                     pars->table_entries_inner);
+                                     pars->table_entries_inner,
+                                     pars->idx_mu_neg1_inner,
+                                     pars->idx_mu_pos1_inner,
+                                 pars->cth_table_inner,
+                                 pars->sth_table_inner);
                 ERR_CHK_VOID(pars)
             }
 
             if(th < th_a || th > th_b)
                 continue;
 
             shockVals(th, ph, tobs[j], t+j, R+j, u+j, thj+j,
@@ -1796,113 +2326,121 @@
 
         theta_cone_hi = (i+1) * Dtheta;
         theta_cone_low = i * Dtheta;
         theta_h = theta_cone_hi;
 
         set_jet_params(pars, E_iso, theta_h);
         ERR_CHK_VOID(pars)
-        set_obs_params(pars, tobs[0], 1.0, theta_obs, theta_cone_hi, 
+        set_obs_params(pars, tobs[0], 1.0, 0, theta_obs, theta_cone_hi, 
                         theta_cone_low);
         make_mu_table(pars);
         double tobs_cur = tobs[0];
         
         for(j=0; j<N; j++)
         {
             double th = theta[j];
             double ph = phi[j];
             
             if(t[j] > 0.0 || th < theta_cone_low)
                 continue;
 
-            set_obs_params(pars, tobs[j], 1.0, theta_obs, theta_cone_hi, 
+            set_obs_params(pars, tobs[j], 1.0, 0, theta_obs, theta_cone_hi, 
                             theta_cone_low);
             if(tobs_cur != tobs[j])
             {
                 make_mu_table(pars);
                 tobs_cur = tobs[j];
             }
 
             double th_a, th_b;
             th_b = find_jet_edge(ph, pars->cto, pars->sto, theta_cone_hi,
                                  pars->mu_table, pars->th_table,
-                                 pars->table_entries);
+                                 pars->table_entries,
+                                 pars->idx_mu_neg1, pars->idx_mu_pos1,
+                             pars->cth_table, pars->sth_table);
             ERR_CHK_VOID(pars)
             if(pars->table_entries_inner == 0)
                 th_a = (theta_cone_low / theta_cone_hi) * th_b;
             else
             {
                 th_a = find_jet_edge(ph, pars->cto, pars->sto, theta_cone_low,
                                      pars->mu_table_inner, 
                                      pars->th_table_inner,
-                                     pars->table_entries_inner);
+                                     pars->table_entries_inner,
+                                     pars->idx_mu_neg1_inner,
+                                     pars->idx_mu_pos1_inner,
+                                 pars->cth_table_inner,
+                                 pars->sth_table_inner);
                 ERR_CHK_VOID(pars)
             }
 
             if(th < th_a || th > th_b)
                 continue;
 
             shockVals(th, ph, tobs[j], t+j, R+j, u+j, thj+j,
                       theta_obs, theta_cone_hi, theta_cone_low, pars);
             ERR_CHK_VOID(pars)
         }
     }
 }
 
 void calc_flux_density(int jet_type, int spec_type, double *t, double *nu,
-                            double *Fnu, int N, struct fluxParams *fp)
+                            double *Fnu, long *moment, int N,
+                            struct fluxParams *fp)
 {
     int latRes = fp->latRes;
     double E_iso_core = fp->E_iso_core;
     double theta_h_core = fp->theta_core;
     double theta_h_wing = fp->theta_wing;
 
     int res_cones = (int) (latRes*theta_h_wing / theta_h_core);
 
 
     if(jet_type == _tophat)
     {
-        lc_tophat(t, nu, Fnu, N, E_iso_core, theta_h_core, fp);
+        lc_tophat(t, nu, Fnu, moment, N, E_iso_core, theta_h_core, fp);
     }
     else if(jet_type == _cone)
     {
-        lc_cone(t, nu, Fnu, N, E_iso_core, theta_h_core, theta_h_wing, fp);
+        lc_cone(t, nu, Fnu, moment, N, E_iso_core, theta_h_core, theta_h_wing,
+                fp);
     }
     else if(jet_type == _Gaussian)
     {
-        lc_struct(t, nu, Fnu, N, E_iso_core, theta_h_core, 
-                theta_h_wing, NULL, NULL, res_cones, &f_E_Gaussian, fp);
+        lc_struct(t, nu, Fnu, moment, N, E_iso_core, theta_h_core, 
+                  theta_h_wing, NULL, NULL, res_cones, &f_E_Gaussian, fp);
     }
     else if(jet_type == _powerlaw)
     {
-        lc_struct(t, nu, Fnu, N, E_iso_core, theta_h_core, 
-                theta_h_wing, NULL, NULL, res_cones, &f_E_powerlaw, fp);
+        lc_struct(t, nu, Fnu, moment, N, E_iso_core, theta_h_core, 
+                  theta_h_wing, NULL, NULL, res_cones, &f_E_powerlaw, fp);
     }
     else if(jet_type == _twocomponent)
     {
-        lc_struct(t, nu, Fnu, N, E_iso_core, theta_h_core, 
+        lc_struct(t, nu, Fnu, moment, N, E_iso_core, theta_h_core, 
                 theta_h_wing, NULL, NULL, res_cones, &f_E_twocomponent, fp);
     }
     else if(jet_type == _Gaussian_core)
     {
-        lc_structCore(t, nu, Fnu, N, E_iso_core, theta_h_core, 
+        lc_structCore(t, nu, Fnu, moment, N, E_iso_core, theta_h_core, 
                 theta_h_wing, NULL, NULL, res_cones, &f_E_GaussianCore, fp);
     }
     else if(jet_type == _powerlaw_core)
     {
-        lc_structCore(t, nu, Fnu, N, E_iso_core, theta_h_core, 
+        lc_structCore(t, nu, Fnu, moment, N, E_iso_core, theta_h_core, 
                 theta_h_wing, NULL, NULL, res_cones, &f_E_powerlawCore, fp);
     }
     else if(jet_type == _exponential)
     {
-        lc_structCore(t, nu, Fnu, N, E_iso_core, theta_h_core, 
+        lc_structCore(t, nu, Fnu, moment, N, E_iso_core, theta_h_core, 
                 theta_h_wing, NULL, NULL, res_cones, &f_E_exponential, fp);
     }
     else if(jet_type == _exponential2)
     {
-        lc_structCore(t, nu, Fnu, N, E_iso_core, theta_h_core, 
+        lc_structCore(t, nu, Fnu, moment, N, E_iso_core, theta_h_core, 
                 theta_h_wing, NULL, NULL, res_cones, &f_E_exponential2, fp);
     }
 
     //printf("  Calc took %ld evalutions\n", fp->nevals);
 }    
 
 void calc_intensity(int jet_type, int spec_type, double *theta, double *phi,
@@ -2002,21 +2540,23 @@
 }
 ///////////////////////////////////////////////////////////////////////////////
 
 void setup_fluxParams(struct fluxParams *pars,
                     double d_L,
                     double theta_obs,
                     double E_iso_core, double theta_core, double theta_wing,
-                    double b, double L0, double q, double ts, 
+                    double b,
+                    double L0_inj, double q_inj, double t0_inj, double ts_inj, 
                     double n_0,
                     double p,
                     double epsilon_E,
                     double epsilon_B, 
                     double ksi_N,
                     double g0,
+                    int envType, double R0_env, double k_env, double rho1_env, 
                     double E_core_global,
                     double theta_core_global,
                     double ta, double tb,
                     int tRes, int latRes, int int_type,
                     double rtol_struct, double rtol_phi, double rtol_theta,
                     int nmax_phi, int nmax_theta,
                     int spec_type,
@@ -2024,21 +2564,30 @@
                     int spread, int counterjet, int gamma_type)
 {
     pars->t_table = NULL;
     pars->R_table = NULL;
     pars->u_table = NULL;
     pars->th_table = NULL;
     pars->mu_table = NULL;
+    pars->cth_table = NULL;
+    pars->sth_table = NULL;
     pars->table_entries = 0;
     pars->t_table_inner = NULL;
     pars->R_table_inner = NULL;
     pars->u_table_inner = NULL;
     pars->th_table_inner = NULL;
     pars->mu_table_inner = NULL;
+    pars->cth_table_inner = NULL;
+    pars->sth_table_inner = NULL;
     pars->table_entries_inner = 0;
+    pars->cur_entry = -1;
+    pars->idx_mu_neg1 = 0;
+    pars->idx_mu_pos1 = 0;
+    pars->idx_mu_neg1_inner = 0;
+    pars->idx_mu_pos1_inner = 0;
 
     pars->spec_type = spec_type;
     pars->gamma_type = gamma_type;
 
     pars->d_L = d_L;
     pars->theta_obs = theta_obs;
     pars->E_iso_core = E_iso_core;
@@ -2046,46 +2595,57 @@
     pars->theta_wing = theta_wing;
     pars->b = b;
     pars->E_tot = -1;
     pars->g_core = g0;
     pars->E_core_global = E_core_global;
     pars->theta_core_global = theta_core_global;
    
-    pars->L0 = L0;
-    pars->q = q;
-    pars->ts = ts;
+    pars->L0_inj = L0_inj;
+    pars->q_inj = q_inj;
+    pars->t0_inj = t0_inj;
+    pars->ts_inj = ts_inj;
 
     pars->n_0 = n_0;
     pars->p = p;
     pars->epsilon_E = epsilon_E;
     pars->epsilon_B = epsilon_B;
     pars->ksi_N = ksi_N;
 
+    pars->envType = envType;
+    pars->R0_env = R0_env;
+    pars->k_env = k_env;
+    pars->rho1_env = rho1_env;
+
     pars->ta = ta;
     pars->tb = tb;
     pars->tRes = tRes;
     pars->latRes = latRes;
     pars->int_type = int_type;
     pars->rtol_struct = rtol_struct;
     pars->rtol_phi = rtol_phi;
     pars->rtol_theta = rtol_theta;
     pars->nmax_phi = nmax_phi;
     pars->nmax_theta = nmax_theta;
-    
+
     pars->atol_theta = 0.0;
 
     pars->mask = mask;
     pars->nmask = nmask;
     pars->spread = spread;
     pars->counterjet = counterjet;
 
     pars->nevals = 0;
 
     pars->error = 0;
     pars->error_msg = NULL;
+
+    Mesh9 empty_mesh = {.totalSize=0, .N=0, .heap=NULL};
+
+    pars->theta_mesh = empty_mesh;
+    pars->phi_mesh = empty_mesh;
 }
 
 ///////////////////////////////////////////////////////////////////////////////
 
 void set_jet_params(struct fluxParams *pars, double E_iso, double theta_h)
 {
     // min/max observer times
@@ -2101,19 +2661,19 @@
     if(pars->E_tot > 0.0)
         E_jet = pars->E_tot;
     else
         E_jet = (1.0 - cos(theta_h)) * E_iso;
 
     double Einj = 0.0;
     double ti = 0.0;
-    if(pars->L0 > 0.0 && pars->ts > 0.0)
+    if(pars->L0_inj > 0.0 && pars->ts_inj > 0.0)
     {
         // Energy injection uses 1e3s as reference time. 
-        Einj = E_inj(pars->ts, pars->L0, pars->q, pars->ts);
-        ti = pars->ts;
+        Einj = E_inj(pars->ts_inj, pars->L0_inj, pars->q_inj, pars->ts_inj);
+        ti = pars->ts_inj;
     }
     E_jet += Einj;
 
     double c5 = v_light*v_light*v_light*v_light*v_light;
     double n_0 = pars->n_0;
     double C_BM = sqrt(17.0 * E_iso / (8.0 * PI * m_p * n_0 * c5));
     double C_ST = 2.0 / 5.0 * 1.15 * pow(E_jet / (m_p * n_0), 1.0 / 5.0 )
@@ -2182,42 +2742,48 @@
     /*
     if(tb > 0.1*t_NR)  // at late times R ~ c t_NR << c t so t_obs ~ t_e
         Rt1 = 100*(tb+t_NR);
     else // at early times t_obs ~ t*(gamma_sh^-2)/8 ~ CBM^-2 * t^4 / 8
         Rt1 = 100*pow(8*tb*C_BM*C_BM, 0.25);
     */
 
+    //TODO: FIX THIS
+
     Rt1 = 100*(tb + t_NR2 + ti);
 
     pars->Rt0 = Rt0;
     pars->Rt1 = Rt1;
     
     make_R_table(pars);
 }
 
 ///////////////////////////////////////////////////////////////////////////////
 
-void set_obs_params(struct fluxParams *pars, double t_obs, double nu_obs,
+void set_obs_params(struct fluxParams *pars,
+                        double t_obs, double nu_obs, long moment,
                         double theta_obs_cur, double current_theta_cone_hi, 
                         double current_theta_cone_low)
 {
     pars->t_obs = t_obs;
     pars->nu_obs = nu_obs;
+    pars->moment = moment;
     pars->theta_obs_cur = theta_obs_cur;
     pars->cto = cos(theta_obs_cur);
     pars->sto = sin(theta_obs_cur);
     pars->current_theta_cone_hi = current_theta_cone_hi;
     pars->current_theta_cone_low = current_theta_cone_low;
 }
 
 ///////////////////////////////////////////////////////////////////////////////
 
 int check_error(void *params)
 {
     struct fluxParams *fp = (struct fluxParams *) params;
+    if(fp->error)
+        fprintf(stderr, "Oh no there's an error\n");
     return fp->error;
 }
 
 ///////////////////////////////////////////////////////////////////////////////
 
 void set_error(struct fluxParams *pars, char msg[])
 {
@@ -2231,65 +2797,79 @@
             pars->theta);
     c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    phi: %.12lg\n", pars->phi);
     c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    cp: %.12lg\n", pars->cp);
     c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    ct: %.12lg\n", pars->ct);
     c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    st: %.12lg\n", pars->st);
     c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    cto: %.12lg\n", pars->cto);
     c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    sto: %.12lg\n", pars->sto);
-    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    theta_obs: %.12lg\n",
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    theta_obs: %.20lg\n",
             pars->theta_obs);
-    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    t_obs: %.12lg\n",
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    t_obs: %.20lg\n",
             pars->t_obs);
-    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    nu_obs: %.12lg\n",
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    nu_obs: %.20lg\n",
             pars->nu_obs);
-    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    d_L: %.12lg\n", pars->d_L);
-    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    E_iso: %.12lg\n",
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    d_L: %.20lg\n", pars->d_L);
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    E_iso: %.20lg\n",
             pars->E_iso);
-    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    n_0: %.12lg\n", pars->n_0);
-    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    g_init: %.12lg\n",
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    n_0: %.20lg\n", pars->n_0);
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    g_init: %.20lg\n",
             pars->g_init);
-    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    p: %.12lg\n", pars->p);
-    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    epsilon_E: %.12lg\n",
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    p: %.20lg\n", pars->p);
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    epsilon_E: %.20lg\n",
                 pars->epsilon_E);
-    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    epsilon_B: %.12lg\n",
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    epsilon_B: %.20lg\n",
             pars->epsilon_B);
-    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    ksi_N: %.12lg\n",
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    ksi_N: %.20lg\n",
             pars->ksi_N);
-    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    theta_h: %.12lg\n",
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    theta_h: %.20lg\n",
             pars->theta_h);
-    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    E_iso_core: %.12lg\n",
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    E_iso_core: %.20lg\n",
             pars->E_iso_core);
-    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    theta_core: %.12lg\n",
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    theta_core: %.20lg\n",
             pars->theta_core);
-    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    theta_wing: %.12lg\n",
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    theta_wing: %.20lg\n",
             pars->theta_wing);
-    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    b: %.12lg\n", pars->b);
-    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    E_tot: %.12lg\n",
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    b: %.20lg\n", pars->b);
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    E_tot: %.20lg\n",
             pars->E_tot);
-    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    g_core: %.12lg\n",
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    g_core: %.20lg\n",
             pars->g_core);
-    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    E_core_global: %.12lg\n",
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    E_core_global: %.20lg\n",
             pars->E_core_global);
     c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c,
             "    theta_core_global: %.12lg\n", pars->theta_core_global);
     c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    envType: %d\n",
             pars->envType);
-    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    As: %.12lg\n", pars->As);
-    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    Rwind: %.12lg\n",
-            pars->Rwind);
-    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    L0: %.12lg\n", pars->L0);
-    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    q: %.12lg\n", pars->q);
-    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    ts: %.12lg\n", pars->ts);
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    R0_env: %.20lg\n",
+            pars->R0_env);
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    k_env: %.20lg\n",
+            pars->k_env);
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    rho1_env: %.20lg\n",
+            pars->rho1_env);
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    L0_inj: %.20lg\n",
+            pars->L0_inj);
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    q_inj: %.20lg\n",
+            pars->q_inj);
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    t0_inj: %.20lg\n",
+            pars->t0_inj);
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    ts_inj: %.20lg\n",
+            pars->ts_inj);
     c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c,
-            "    current_theta_cone_hi: %.12lg\n",
+            "    current_theta_cone_hi: %.20lg\n",
             pars->current_theta_cone_hi);
     c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c,
-            "    current_theta_cone_low: %.12lg\n", 
+            "    current_theta_cone_low: %.20lg\n", 
             pars->current_theta_cone_low);
-    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    theta_obs_cur: %.12lg\n",
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c,
+            "    current_theta_a: %.20lg\n",
+            pars->current_theta_a);
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c,
+            "    current_theta_b: %.20lg\n", 
+            pars->current_theta_b);
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    theta_obs_cur: %.20lg\n",
             pars->theta_obs_cur);
     c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    tRes: %d\n", pars->tRes);
     c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    latRes: %d\n",
             pars->latRes);
     c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    spread: %d\n",
             pars->spread);
     c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    counterjet: %d\n",
@@ -2318,32 +2898,108 @@
             pars->C_STsqrd);
     c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    t_NR: %.12lg\n",
             pars->t_NR);
     c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    table_entries: %d\n",
             pars->table_entries);
     c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    table_entries_inner: %d\n",
             pars->table_entries_inner);
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    idx_mu_neg1: %d\n",
+            pars->idx_mu_neg1);
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    idx_mu_pos1: %d\n",
+            pars->idx_mu_pos1);
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    idx_mu_neg1_inner: %d\n",
+            pars->idx_mu_neg1_inner);
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    idx_mu_pos1_inner: %d\n",
+            pars->idx_mu_pos1_inner);
     c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    spec_type: %d\n",
             pars->spec_type);
     c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    gamma_type: %d\n",
             pars->gamma_type);
     c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    nmask: %d\n",
             pars->nmask);
     c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    nevals: %ld\n",
             pars->nevals);
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    moment: %ld\n",
+            pars->moment);
+    c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    current_entry: %d\n",
+            pars->cur_entry);
+    if(pars->cur_entry >= 0 && pars->t_table != NULL)
+    {
+        c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "        t[c]: %lg\n",
+                      pars->t_table[pars->cur_entry]);
+    }
+    if(pars->cur_entry >= 0 && pars->R_table != NULL)
+    {
+        c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "        R[c]: %lg\n",
+                      pars->R_table[pars->cur_entry]);
+    }
+    if(pars->cur_entry >= 0 && pars->u_table != NULL)
+    {
+        c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "        u[c]: %lg\n",
+                      pars->u_table[pars->cur_entry]);
+    }
+    if(pars->cur_entry >= 0 && pars->th_table != NULL)
+    {
+        c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "        th[c]: %lg\n",
+                      pars->th_table[pars->cur_entry]);
+    }
+    if(pars->cur_entry >= 0 && pars->mu_table != NULL)
+    {
+        c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "        mu[c]: %lg\n",
+                      pars->mu_table[pars->cur_entry]);
+    }
     c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "    error: %d\n", pars->error);
     c += snprintf(dump+c, DUMP_MSG_LEN_MAX-c, "}\n");
 
     int dumplen = strlen(dump);
     int len = msglen + dumplen + 1;
 
     pars->error_msg = (char *)malloc(len * sizeof(char));
     
     strcpy(pars->error_msg, msg);
     strcpy(pars->error_msg+msglen, dump);
+
+    if(1)
+    {
+        char *meshStr;
+        mesh9Write(&(pars->theta_mesh), &meshStr);
+        FILE *f = fopen("afterglowpy_mesh_theta.txt", "w");
+        fprintf(f, "%s\n", meshStr);
+        int i;
+        for(i=0; i<pars->theta_mesh.N; i++)
+            interval9Write(&(pars->theta_mesh.heap[i]), f);
+            
+        fclose(f);
+        free(meshStr);
+
+        mesh9Write(&(pars->phi_mesh), &meshStr);
+        f = fopen("afterglowpy_mesh_phi.txt", "w");
+        fprintf(f, "%s\n", meshStr);
+        for(i=0; i<pars->phi_mesh.N; i++)
+            interval9Write(&(pars->phi_mesh.heap[i]), f);
+        fclose(f);
+        free(meshStr);
+
+        f = fopen("afterglowpy_shock_table.txt", "w");
+        for(i=0; i<pars->table_entries; i++)
+            fprintf(f, "%.16lg %.16lg %.16lg %.16lg %.16lg\n",
+                    pars->t_table[i], pars->R_table[i], pars->u_table[i],
+                    pars->th_table[i], pars->mu_table[i]);
+        fclose(f);
+
+        f = fopen("afterglowpy_shock_table_inner.txt", "w");
+        for(i=0; i<pars->table_entries_inner; i++)
+            fprintf(f, "%.16lg %.16lg %.16lg %.16lg %.16lg\n",
+                    pars->t_table_inner[i], pars->R_table_inner[i],
+                    pars->u_table_inner[i], pars->th_table_inner[i],
+                    pars->mu_table_inner[i]);
+        fclose(f);
+    }
+    mesh9Free(&(pars->theta_mesh));
+    mesh9Free(&(pars->phi_mesh));
 }
 
 
 ///////////////////////////////////////////////////////////////////////////////
 
 
 void free_fluxParams(struct fluxParams *pars)
@@ -2369,14 +3025,24 @@
         pars->th_table = NULL;
     }
     if(pars->mu_table != NULL)
     {
         free(pars->mu_table);
         pars->mu_table = NULL;
     }
+    if(pars->cth_table != NULL)
+    {
+        free(pars->cth_table);
+        pars->cth_table = NULL;
+    }
+    if(pars->sth_table != NULL)
+    {
+        free(pars->sth_table);
+        pars->sth_table = NULL;
+    }
 
     if(pars->t_table_inner != NULL)
     {
         free(pars->t_table_inner);
         pars->t_table_inner = NULL;
     }
     if(pars->R_table_inner != NULL)
@@ -2395,14 +3061,24 @@
         pars->th_table_inner = NULL;
     }
     if(pars->mu_table_inner != NULL)
     {
         free(pars->mu_table_inner);
         pars->mu_table_inner = NULL;
     }
+    if(pars->cth_table_inner != NULL)
+    {
+        free(pars->cth_table_inner);
+        pars->cth_table_inner = NULL;
+    }
+    if(pars->sth_table_inner != NULL)
+    {
+        free(pars->sth_table_inner);
+        pars->sth_table_inner = NULL;
+    }
 
     if(pars->error_msg != NULL)
     {
         free(pars->error_msg);
         pars->error_msg = NULL;
     }
 }
```

### Comparing `afterglowpy-0.7.3/afterglowpy/shockmodule.c` & `afterglowpy-0.8.0/afterglowpy/shockmodule.c`

 * *Files 21% similar despite different names*

```diff
@@ -96,19 +96,24 @@
 }
 
 static PyObject *shock_shockEvolRK4(PyObject *self, PyObject *args)
 {
     PyObject *t_obj = NULL;
 
     double R0, u0;
-    double Mej, rho0, Einj, k, umin, L0, q, ts;
+    double Mej, rho0_env, R0_env, k_env, rho1_env, Einj, k, umin, L0, q, ts;
+    int envType;
 
     //Parse Arguments
-    if(!PyArg_ParseTuple(args, "Odddddddddd", &t_obj, &R0, &u0, &Mej, &rho0,
-                                            &Einj, &k, &umin, &L0, &q, &ts))
+    if(!PyArg_ParseTuple(args, "Odd""d""idddd""ddd""ddd",
+                         &t_obj, &R0, &u0,
+                         &Mej,
+                         &envType, &rho0_env, &R0_env, &k_env, &rho1_env,
+                         &Einj, &k, &umin,
+                         &L0, &q, &ts))
     {
         PyErr_SetString(PyExc_RuntimeError, "Could not parse arguments.");
         return NULL;
     }
 
     //Grab NUMPY arrays
     PyArrayObject *t_arr;
@@ -147,16 +152,22 @@
         Py_XDECREF(u_obj);
         return NULL;
     }
     double *R = PyArray_DATA((PyArrayObject *) R_obj);
     double *u = PyArray_DATA((PyArrayObject *) u_obj);
 
     // Evolve the shock!
-    double shockArgs[9] = {u0, Mej, rho0, Einj, k, umin, L0, q, ts};
-    shockEvolveRK4(t, R, u, N, R0, u0, shockArgs);
+    struct shockParams shock_pars;
+    setup_shockParams(&shock_pars, 0, 0.0, Mej,
+                      envType, rho0_env, R0_env, k_env, rho1_env,
+                      L0, q, 1.0e3, ts,
+                      Einj, k, umin,
+                      0.0, 0.0, 0.0);
+    //double shockArgs[9] = {0.0, Mej, rho0, Einj, k, umin, L0, q, ts};
+    shockEvolveRK4(t, R, u, N, R0, u0, &shock_pars);
 
     // Clean up!
     Py_DECREF(t_arr);
 
     //Build output
     PyObject *ret = Py_BuildValue("NN", R_obj, u_obj);
     
@@ -164,20 +175,27 @@
 }
 
 static PyObject *shock_shockEvolSpreadRK4(PyObject *self, PyObject *args)
 {
     PyObject *t_obj = NULL;
 
     double R0, u0, th0;
-    double Mej, rho0, Einj, k, umin, L0, q, ts, thC;
+    double Mej, rho0_env, R0_env, k_env, rho1_env;
+    double Einj, k, umin, L0, q, ts, thC;
+    int envType;
     int spread;
 
     //Parse Arguments
-    if(!PyArg_ParseTuple(args, "Oddddddddddddi", &t_obj, &R0, &u0, &th0, 
-                                &Mej, &rho0, &Einj, &k, &umin, &L0, &q, &ts,
+    if(!PyArg_ParseTuple(args, "Oddd""d""idddd""ddd""ddd""di",
+                                &t_obj, &R0, &u0, &th0, 
+                                &Mej, 
+                                &envType, &rho0_env, &R0_env, &k_env,
+                                    &rho1_env,
+                                &Einj, &k, &umin, 
+                                &L0, &q, &ts,
                                 &thC, &spread))
     {
         PyErr_SetString(PyExc_RuntimeError, "Could not parse arguments.");
         return NULL;
     }
 
     //Grab NUMPY arrays
@@ -220,17 +238,25 @@
         return NULL;
     }
     double *R = PyArray_DATA((PyArrayObject *) R_obj);
     double *u = PyArray_DATA((PyArrayObject *) u_obj);
     double *th = PyArray_DATA((PyArrayObject *) th_obj);
 
     // Evolve the shock!
-    double shockArgs[12] = {u0, Mej, rho0, Einj, k, umin, L0, q, ts, thC, th0,
-                            thC};
-    shockEvolveSpreadRK4(t, R, u, th, N, R0, u0, th0, shockArgs, spread);
+    //double shockArgs[12] = {0.0, Mej, rho0, Einj, k, umin, L0, q, ts, thC, th0,
+    //                        thC};
+    
+    struct shockParams shock_pars;
+    setup_shockParams(&shock_pars, spread, 0.0, Mej,
+                        envType, rho0_env, R0_env, k_env, rho1_env,
+                        L0, q, 1.0e3, ts,
+                        Einj, k, umin,
+                        thC, th0, thC);
+
+    shockEvolveSpreadRK4(t, R, u, th, N, R0, u0, th0, &shock_pars);
 
     // Clean up!
     Py_DECREF(t_arr);
 
     //Build output
     PyObject *ret = Py_BuildValue("NNN", R_obj, u_obj, th_obj);
```

### Comparing `afterglowpy-0.7.3/afterglowpy.egg-info/SOURCES.txt` & `afterglowpy-0.8.0/afterglowpy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 afterglowpy/__init__.py
 afterglowpy/cocoon.py
 afterglowpy/flux.py
```

### Comparing `afterglowpy-0.7.3/setup.py` & `afterglowpy-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                         include_dirs=inc, depends=shockdepends,
                         extra_compile_args=['-Wall'])
 
 setup(
     name='afterglowpy',
     version=version['__version__'],
     author="Geoffrey Ryan",
-    author_email="gsryan@umd.edu",
+    author_email="gryan@perimeterinstitute.ca",
     description='GRB Afterglow Models',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/geoffryan/afterglowpy',
     packages=['afterglowpy'],
     ext_modules=[jetmodule, shockmodule],
@@ -52,15 +52,15 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: C",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Astronomy"],
-    install_requires=['numpy>=1.10', 'scipy>=0.14'],
+    install_requires=['numpy>=1.13', 'scipy>=0.14'],
     extras_require={
         'docs': ['numpydoc']
         },
     project_urls={
         "Source Code": "https://github.com/geoffryan/afterglowpy",
         "Documentation": "https://afterglowpy.readthedocs.io"}
     )
```

### Comparing `afterglowpy-0.7.3/test/test_flux.py` & `afterglowpy-0.8.0/test/test_flux.py`

 * *Files identical despite different names*

