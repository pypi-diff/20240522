# Comparing `tmp/FitTransit-0.1.1-py3-none-any.whl.zip` & `tmp/FitTransit-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 23748 bytes, number of entries: 8
--rwxrwxrwx  2.0 unx    77237 b- defN 23-Mar-13 09:39 FitTransit/Transit_class.py
+Zip file size: 24329 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx    79072 b- defN 24-May-22 07:20 FitTransit/Transit_class.py
+-rw-rw-r--  2.0 unx      132 b- defN 24-May-22 07:20 FitTransit/__init__.py
 -rwxrwxrwx  2.0 unx     3052 b- defN 19-Nov-11 16:59 FitTransit/ga.py
 -rwxrwxrwx  2.0 unx     8552 b- defN 22-Jun-22 10:22 FitTransit/info_ga.py
--rwxrwxrwx  2.0 unx    12637 b- defN 22-Jun-22 09:47 FitTransit/info_mc.py
--rwxrwxrwx  2.0 unx      602 b- defN 23-Mar-13 09:52 FitTransit-0.1.1.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Mar-13 09:52 FitTransit-0.1.1.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       97 b- defN 23-Mar-13 09:52 FitTransit-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      624 b- defN 23-Mar-13 09:52 FitTransit-0.1.1.dist-info/RECORD
-8 files, 102893 bytes uncompressed, 22668 bytes compressed:  78.0%
+-rw-rw-r--  2.0 unx    12641 b- defN 24-Apr-08 11:42 FitTransit/info_mc.py
+-rw-rw-r--  2.0 unx      592 b- defN 24-May-22 07:24 FitTransit-0.1.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-22 07:24 FitTransit-0.1.2.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx       97 b- defN 24-May-22 07:24 FitTransit-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      702 b- defN 24-May-22 07:24 FitTransit-0.1.2.dist-info/RECORD
+9 files, 104932 bytes uncompressed, 23129 bytes compressed:  78.0%
```

## zipnote {}

```diff
@@ -1,25 +1,28 @@
 Filename: FitTransit/Transit_class.py
 Comment: 
 
+Filename: FitTransit/__init__.py
+Comment: 
+
 Filename: FitTransit/ga.py
 Comment: 
 
 Filename: FitTransit/info_ga.py
 Comment: 
 
 Filename: FitTransit/info_mc.py
 Comment: 
 
-Filename: FitTransit-0.1.1.dist-info/METADATA
+Filename: FitTransit-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: FitTransit-0.1.1.dist-info/WHEEL
+Filename: FitTransit-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: FitTransit-0.1.1.dist-info/top_level.txt
+Filename: FitTransit-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: FitTransit-0.1.1.dist-info/RECORD
+Filename: FitTransit-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## FitTransit/Transit_class.py

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 #main classes of FitTransit package
-#version 0.1.1
-#update: 9.2.2023
-# (c) Pavol Gajdos, 2022-2023
+#version 0.1.2
+#update: 22.5.2024
+# (c) Pavol Gajdos, 2022-2024
 
 from time import time
 import sys
 import os
 import threading
 import warnings
 
@@ -131,15 +131,15 @@
 
 
 
 class FitTransit():
     '''class for fitting transits'''
     availableModels=['TransitUniform','TransitLinear','TransitQuadratic','TransitSquareRoot',
                      'TransitLogarithmic','TransitExponential','TransitPower2','TransitNonlinear',
-                     'Gauss','Lorentz','Voigt','Quad','Poly4','Mikulasek']   #list of available models
+                     'Gauss','GaussModif','Lorentz','Voigt','Quad','Poly4','Mikulasek','Binomial']   #list of available models
 
     def __init__(self,t,flux,err=None):
         '''loading times, fluxes, (errors)'''
         self.t=np.array(t)
         self.flux=np.array(flux)
         if err is None:
             #if unknown (not given) errors of data
@@ -189,17 +189,19 @@
                 s+='t0, P, Rp, a, i, e, w, '
                 if 'Uniform' not in model:
                     s+='c1, '
                     if ('Linear' not in model) and ('Power2' not in model):
                         s+='c2, '
                         if 'Nonlinear' in model: s+='c3, c4, '
             if 'Gauss' in model or 'Lorentz' in model or 'Quad' in model: s+='A, tC, w, '
+            if 'Modif' in model: s+='k, '
             if 'Poly4' in model: s+='A, w2, w4, '
             if 'Voigt' in model: s+='A, tC, wG, wL, '
             if 'Mikulasek' in model: s+='A, C, K, tC, w, g, '
+            if 'Binomial' in model: s+='A, tC, T, k1, k2, '
             s+='p0, p1, p2'
             print(s)
 
         if model is None: model=self.model
         if allModels:
             for m in sorted(self.availableModels): Display(m)
         else: Display(model)
@@ -409,14 +411,34 @@
 
         g=1+A*np.exp(-(t-tC)**2/(2*w**2))
 
         flux=g*np.polyval(p,t-tC)         #calculates light curve
 
         return flux
 
+    def GaussModif(self,t,A,tC,w,k,p):
+        '''model of minimum/maximum/eclipse using modificated gaussian function
+        t - times of observations (np.array alebo float) [days]
+        tC - time of center of minimum [days]
+        A - amplitude of gaussian
+        w - width of gaussian [days]
+        k - exponent
+        p - 2nd order polynom coefficients (in list / np.array)
+        output in fluxes
+        '''
+
+        if k<=0:
+            raise ValueError('Exponent "k" should be possitive!')
+
+        g=1+A*np.exp(-np.abs(t-tC)**k/(k*w**k))
+
+        flux=g*np.polyval(p,t-tC)         #calculates light curve
+
+        return flux
+
     def Lorentz(self,t,A,tC,w,p):
         '''model of minimum/maximum/eclipse using lorentzian function / Cauchy curve
         t - times of observations (np.array alebo float) [days]
         tC - time of center of minimum [days]
         A - amplitude of lorentzian
         w - width of lorentzian [days]
         p - 2nd order polynom coefficients (in list / np.array)
@@ -491,25 +513,45 @@
         return flux
 
     def Mikulasek(self,t,A,C,K,tC,w,g,p):
         '''model of minimum/maximum/eclipse based on phenomenological model of Mikulasek (2015)
         t - times of observations (np.array alebo float) [days]
         tC - time of center of minimum [days]
         A - amplitude
+        C,K - correcting parameters
         w - width
+        g - kurtosis
         p - 2nd order polynom coefficients (in list / np.array)
         output in fluxes
         '''
 
         mik=1+A*(1+C*((t-tC)/w)**2+K*((t-tC)/w)**4)*(1-(1-np.exp(1-np.cosh((t-tC)/w)))**g)
 
         flux=mik*np.polyval(p,t-tC)         #calculates light curve
 
         return flux
 
+    def Binomial(self,t,A,tC,T,k1,k2,p):
+        '''model of minimum/maximum/eclipse based on quasi binomial model
+        t - times of observations (np.array alebo float) [days]
+        tC - time of center of minimum [days]
+        A - amplitude
+        T - duration [days]
+        k1, k2 - exponents (standard values: k1=2, k2=1.5)
+        p - 2nd order polynom coefficients (in list / np.array)
+        output in fluxes
+        '''
+
+        model=1+A*(1-(2*np.abs(t-tC)/T)**k1)**k2
+        model[np.isnan(model)]=1
+
+        flux=model*np.polyval(p,t-tC)         #calculates light curve
+
+        return flux
+
 
     def PhaseCurve(self,P,t0,plot=False):
         '''create phase curve'''
         f=np.mod(self.t-t0,P)/float(P)    #phase
         order=np.argsort(f)
         f=f[order]
         flux=self.flux[order]
@@ -846,24 +888,24 @@
                 if x in self.params_err: err.append(str(self.params_err[x]))
                 elif x in self.fit_params: err.append('---')   #errors not calculated
                 else: err.append('fixed')  #fixed params
             elif x in self.fit_params: err.append('---')  #errors not calculated
             else: err.append('fixed')   #fixed params
             #add units
             if x[0]=='a' or x[0]=='R': unit.append('Rstar')
-            elif x[0]=='P':
+            elif x[0]=='P' or x[0]=='T':
                 unit.append('d')
                 #also in years
                 params.append(x)
                 vals.append(str(self.params[x]/year))
                 if err[-1]=='---' or err[-1]=='fixed': err.append(err[-1])  #error not calculated
                 else: err.append(str(float(err[-1])/year)) #error calculated
                 unit.append('yr')
             elif x[0]=='t': unit.append('JD')
-            elif x[0] in 'ecpACKg': unit.append('')
+            elif x[0] in 'ecpACKgk': unit.append('')
             elif x[0]=='w':
                 if 'Transit' in self.model: unit.append('deg')
                 else: unit.append('d')
             elif x[0]=='i': unit.append('deg')
             else: unit.append('NA!')
 
         if 'Transit' in self.model:
@@ -1255,26 +1297,32 @@
                 if ('Linear' not in self.model) or ('Power2' not in self.model):
                     u.append(param['c2'])
                     if 'Nonlinear' in self.model:
                         u.append(param['c3'])
                         u.append(param['c4'])
 
             model=self.Transit(t,param['t0'],param['P'],param['Rp'],param['a'],param['i'],param['e'],param['w'],u,p)
-        elif 'Gauss' in self.model:
+        elif self.model=='Gauss':
             model=self.Gauss(t,param['A'],param['tC'],param['w'],p)
-        elif 'Lorentz' in self.model:
+        elif self.model=='GaussModif':
+            model=self.GaussModif(t,param['A'],param['tC'],param['w'],param['k'],p)
+        elif self.model=='Lorentz':
             model=self.Lorentz(t,param['A'],param['tC'],param['w'],p)
-        elif 'Voigt' in self.model:
+        elif self.model=='Voigt':
             model=self.Voigt(t,param['A'],param['tC'],param['wG'],param['wL'],p)
-        elif 'Quad' in self.model:
+        elif self.model=='Quad':
             model=self.Quad(t,param['A'],param['tC'],param['w'],p)
-        elif 'Poly4' in self.model:
+        elif self.model=='Poly4':
             model=self.Poly4(t,param['A'],param['tC'],param['w2'],param['w4'],p)
-        elif 'Mikulasek' in self.model:
+        elif self.model=='Mikulasek':
             model=self.Mikulasek(t,param['A'],param['C'],param['K'],param['tC'],param['w'],param['g'],p)
+        elif self.model=='Binomial':
+            model=self.Binomial(t,param['A'],param['tC'],param['T'],param['k1'],param['k2'],p)
+        else:
+            raise KeyError('Unknown model "'+self.model+'"! Available models are: '+', '.join(sorted(self.availableModels)))
 
         return model
 
 
     def CalcErr(self):
         '''estimate errors of input data based on current model (useful before using FitMCMC)'''
         model=self.Model(self.t,self.params)  #calculate model values
```

## FitTransit/info_mc.py

```diff
@@ -154,15 +154,15 @@
         values=[]
         tr=[]
         if params is None: params=self.pars
         for p in params:
             i=self.pars.index(p)
             values.append(np.median(self.flat[:,i]))
             tr.append(self.flat[:,i])
-        fig=corner.corner(np.array(tr).transpose(),labels=params,truths=values,quantiles=[1-0.6827,0.6827],show_titles=True)
+        fig=corner.corner(np.array(tr).transpose(),labels=params,truths=values,quantiles=[1-0.6827,0.5,0.6827],show_titles=True)
         return fig
 
     def Hist(self,param,new_fig=True,label=True):
         '''plot histogram for one parameter'''
         i=self.pars.index(param)
         if new_fig: fig=mpl.figure()
         mpl.hist(self.flat[:,i],bins=20,color='k')
```

## Comparing `FitTransit-0.1.1.dist-info/METADATA` & `FitTransit-0.1.2.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: FitTransit
-Version: 0.1.1
+Version: 0.1.2
 Summary: Fitting transits of exoplanets
 Home-page: https://github.com/pavolgaj/FitTransit
 Author: Pavol Gajdos
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
-Requires-Dist: numpy (>=1.10.2)
-Requires-Dist: matplotlib (>=1.5.0)
-Requires-Dist: scipy (>=1.5.0)
-Requires-Dist: batman-package (>=2.4.0)
+Requires-Dist: numpy >=1.10.2
+Requires-Dist: matplotlib >=1.5.0
+Requires-Dist: scipy >=1.5.0
+Requires-Dist: batman-package >=2.4.0
 Provides-Extra: mcmc
-Requires-Dist: emcee (>=3.0.0) ; extra == 'mcmc'
+Requires-Dist: emcee >=3.0.0 ; extra == 'mcmc'
 Requires-Dist: corner ; extra == 'mcmc'
 Requires-Dist: tqdm ; extra == 'mcmc'
```

## Comparing `FitTransit-0.1.1.dist-info/RECORD` & `FitTransit-0.1.2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-FitTransit/Transit_class.py,sha256=LZAk7UDQjG6Zjr4jpuYYMinhfooNqZEWU0B6CZ4WWBc,77237
+FitTransit/Transit_class.py,sha256=mTGs9VIUA1npTGOHcet4LmjFuN1YxC9QSX1er2KWBpw,79072
+FitTransit/__init__.py,sha256=Np2M2NReo19qAdDfC6nCzFjJb7SShsr-vtLukdj-W88,132
 FitTransit/ga.py,sha256=PNJrXh-vEafx_4jqniKC5i3Xq08HLJmrLKBSgAOuMCs,3052
 FitTransit/info_ga.py,sha256=BKNtlI4x3QkNMY1wY89n6oFFhpy6s-gUCmp_r4FurRk,8552
-FitTransit/info_mc.py,sha256=59Sn38GAhX40L7CyngvIEHPYqhtxq5byOylLtqvwOy8,12637
-FitTransit-0.1.1.dist-info/METADATA,sha256=8WVQkpZP_2MtfJSPWiV5xJKtrT6RlZY_MViEysGIZEU,602
-FitTransit-0.1.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-FitTransit-0.1.1.dist-info/top_level.txt,sha256=mLgrlR8bs78cOG8f37cpgnUW7YqBhllbGEDg-JAtTXc,97
-FitTransit-0.1.1.dist-info/RECORD,,
+FitTransit/info_mc.py,sha256=WuPyU9jYzfsLDok-e5R4f15mmiGtcWTycLtIFTkGups,12641
+FitTransit-0.1.2.dist-info/METADATA,sha256=DUzXsMDWFaYA7Vx1bOded6dxh7KjJprC8ep-yuch0HE,592
+FitTransit-0.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+FitTransit-0.1.2.dist-info/top_level.txt,sha256=V2TC_mABGpoxBn6ugAm-Mshk2LvDKjohNN_amwKoEhI,97
+FitTransit-0.1.2.dist-info/RECORD,,
```

