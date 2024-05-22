# Comparing `tmp/StraitFlux-1.0.4.tar.gz` & `tmp/straitflux-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StraitFlux-1.0.4.tar", last modified: Tue Mar 19 12:44:06 2024, max compression
+gzip compressed data, was "straitflux-1.0.5.tar", last modified: Wed May 22 18:36:50 2024, max compression
```

## Comparing `StraitFlux-1.0.4.tar` & `straitflux-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 swinkelbauer (1912200010) users      (100)        0 2024-03-19 12:44:06.587604 StraitFlux-1.0.4/
--rw-r--r--   0 swinkelbauer (1912200010) users      (100)    35149 2024-03-19 12:39:37.000000 StraitFlux-1.0.4/LICENSE
--rw-r--r--   0 swinkelbauer (1912200010) users      (100)      742 2024-03-19 12:44:06.587604 StraitFlux-1.0.4/PKG-INFO
--rw-r--r--   0 swinkelbauer (1912200010) users      (100)     2328 2024-03-19 12:39:37.000000 StraitFlux-1.0.4/README.md
-drwxr-xr-x   0 swinkelbauer (1912200010) users      (100)        0 2024-03-19 12:44:06.584604 StraitFlux-1.0.4/StraitFlux/
--rw-r--r--   0 swinkelbauer (1912200010) users      (100)        1 2024-03-19 12:39:37.000000 StraitFlux-1.0.4/StraitFlux/__init__.py
--rw-r--r--   0 swinkelbauer (1912200010) users      (100)    14233 2024-03-19 12:39:37.000000 StraitFlux-1.0.4/StraitFlux/functions.py
--rw-r--r--   0 swinkelbauer (1912200010) users      (100)    22166 2024-03-19 12:39:37.000000 StraitFlux-1.0.4/StraitFlux/functions_VP.py
--rw-r--r--   0 swinkelbauer (1912200010) users      (100)    13944 2024-03-19 12:39:37.000000 StraitFlux-1.0.4/StraitFlux/indices.py
--rw-r--r--   0 swinkelbauer (1912200010) users      (100)    18563 2024-03-19 12:39:37.000000 StraitFlux-1.0.4/StraitFlux/masterscript_cross.py
--rw-r--r--   0 swinkelbauer (1912200010) users      (100)    13181 2024-03-19 12:39:37.000000 StraitFlux-1.0.4/StraitFlux/masterscript_line.py
--rw-r--r--   0 swinkelbauer (1912200010) users      (100)     7402 2024-03-19 12:39:37.000000 StraitFlux-1.0.4/StraitFlux/preprocessing.py
-drwxr-xr-x   0 swinkelbauer (1912200010) users      (100)        0 2024-03-19 12:44:06.586604 StraitFlux-1.0.4/StraitFlux.egg-info/
--rw-r--r--   0 swinkelbauer (1912200010) users      (100)      742 2024-03-19 12:44:06.000000 StraitFlux-1.0.4/StraitFlux.egg-info/PKG-INFO
--rw-r--r--   0 swinkelbauer (1912200010) users      (100)      394 2024-03-19 12:44:06.000000 StraitFlux-1.0.4/StraitFlux.egg-info/SOURCES.txt
--rw-r--r--   0 swinkelbauer (1912200010) users      (100)        1 2024-03-19 12:44:06.000000 StraitFlux-1.0.4/StraitFlux.egg-info/dependency_links.txt
--rw-r--r--   0 swinkelbauer (1912200010) users      (100)       47 2024-03-19 12:44:06.000000 StraitFlux-1.0.4/StraitFlux.egg-info/requires.txt
--rw-r--r--   0 swinkelbauer (1912200010) users      (100)       11 2024-03-19 12:44:06.000000 StraitFlux-1.0.4/StraitFlux.egg-info/top_level.txt
--rw-r--r--   0 swinkelbauer (1912200010) users      (100)       79 2024-03-19 12:44:06.588605 StraitFlux-1.0.4/setup.cfg
--rw-r--r--   0 swinkelbauer (1912200010) users      (100)      845 2024-03-19 12:39:37.000000 StraitFlux-1.0.4/setup.py
+drwxr-xr-x   0 swinkelbauer (1912200010) users      (100)        0 2024-05-22 18:36:50.163086 straitflux-1.0.5/
+-rw-r--r--   0 swinkelbauer (1912200010) users      (100)    35149 2024-05-22 18:33:25.000000 straitflux-1.0.5/LICENSE
+-rw-r--r--   0 swinkelbauer (1912200010) users      (100)      742 2024-05-22 18:36:50.163086 straitflux-1.0.5/PKG-INFO
+-rw-r--r--   0 swinkelbauer (1912200010) users      (100)     2328 2024-05-22 18:33:25.000000 straitflux-1.0.5/README.md
+drwxr-xr-x   0 swinkelbauer (1912200010) users      (100)        0 2024-05-22 18:36:50.113083 straitflux-1.0.5/StraitFlux/
+-rw-r--r--   0 swinkelbauer (1912200010) users      (100)        1 2024-05-22 18:33:25.000000 straitflux-1.0.5/StraitFlux/__init__.py
+-rw-r--r--   0 swinkelbauer (1912200010) users      (100)    14264 2024-05-22 18:33:25.000000 straitflux-1.0.5/StraitFlux/functions.py
+-rw-r--r--   0 swinkelbauer (1912200010) users      (100)    22170 2024-05-22 18:33:25.000000 straitflux-1.0.5/StraitFlux/functions_VP.py
+-rw-r--r--   0 swinkelbauer (1912200010) users      (100)    13942 2024-05-22 18:33:25.000000 straitflux-1.0.5/StraitFlux/indices.py
+-rw-r--r--   0 swinkelbauer (1912200010) users      (100)    19029 2024-05-22 18:33:25.000000 straitflux-1.0.5/StraitFlux/masterscript_cross.py
+-rw-r--r--   0 swinkelbauer (1912200010) users      (100)    13843 2024-05-22 18:33:25.000000 straitflux-1.0.5/StraitFlux/masterscript_line.py
+-rw-r--r--   0 swinkelbauer (1912200010) users      (100)     7404 2024-05-22 18:33:25.000000 straitflux-1.0.5/StraitFlux/preprocessing.py
+drwxr-xr-x   0 swinkelbauer (1912200010) users      (100)        0 2024-05-22 18:36:50.163086 straitflux-1.0.5/StraitFlux.egg-info/
+-rw-r--r--   0 swinkelbauer (1912200010) users      (100)      742 2024-05-22 18:36:49.000000 straitflux-1.0.5/StraitFlux.egg-info/PKG-INFO
+-rw-r--r--   0 swinkelbauer (1912200010) users      (100)      394 2024-05-22 18:36:49.000000 straitflux-1.0.5/StraitFlux.egg-info/SOURCES.txt
+-rw-r--r--   0 swinkelbauer (1912200010) users      (100)        1 2024-05-22 18:36:49.000000 straitflux-1.0.5/StraitFlux.egg-info/dependency_links.txt
+-rw-r--r--   0 swinkelbauer (1912200010) users      (100)       47 2024-05-22 18:36:49.000000 straitflux-1.0.5/StraitFlux.egg-info/requires.txt
+-rw-r--r--   0 swinkelbauer (1912200010) users      (100)       11 2024-05-22 18:36:49.000000 straitflux-1.0.5/StraitFlux.egg-info/top_level.txt
+-rw-r--r--   0 swinkelbauer (1912200010) users      (100)       79 2024-05-22 18:36:50.168086 straitflux-1.0.5/setup.cfg
+-rw-r--r--   0 swinkelbauer (1912200010) users      (100)      845 2024-05-22 18:33:25.000000 straitflux-1.0.5/setup.py
```

### Comparing `StraitFlux-1.0.4/LICENSE` & `straitflux-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `StraitFlux-1.0.4/PKG-INFO` & `straitflux-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StraitFlux
-Version: 1.0.4
+Version: 1.0.5
 Summary: StraitFlux
 Home-page: https://github.com/susannawinkelbauer/StraitFlux
 Download-URL: https://github.com/susannawinkelbauer/StraitFlux/archive/refs/tags/v1.0.4.tar.gz
 Author: Susanna Winkelbauer
 Author-email: susanna.winkelbauer@univie.ac.at
 Keywords: python,oceanic transports,curvilinear grids
 Classifier: Intended Audience :: Science/Research
```

### Comparing `StraitFlux-1.0.4/README.md` & `straitflux-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `StraitFlux-1.0.4/StraitFlux/functions.py` & `straitflux-1.0.5/StraitFlux/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,18 +137,17 @@
     if min_x == -1:
         min_x = 0
         max_x = max_x + 1
         
     t=t.sel(x=slice(int(min_x)-2,int(max_x)+2),y=slice(int(min_y)-2,int(max_y)+2)).load()
     u=u.sel(x=slice(int(min_x)-1,int(max_x)+1),y=slice(int(min_y)-1,int(max_y)+1)).load()
     v=v.sel(x=slice(int(min_x)-1,int(max_x)+1),y=slice(int(min_y)-1,int(max_y)+1)).load()
-    #print(t)
     try:
         plt.title(model+'_'+strait,fontsize=14)
-        u.uo.plot()
+        plt.pcolormesh(t.x,t.y,(t.thetao/t.thetao),cmap='tab20c')
         plt.scatter(out_v[:,0],out_v[:,1]+0.5,marker='_',c='r',s=200)
         plt.scatter(out_u[:,0]+0.5,out_u[:,1],marker='|',c='r',s=200)
         plt.ylabel('y',fontsize=14)
         plt.xlabel('x',fontsize=14)
         plt.savefig(path_save+strait+'_'+model+'_indices_check.png')
         plt.close()
     except NameError:
```

### Comparing `StraitFlux-1.0.4/StraitFlux/functions_VP.py` & `straitflux-1.0.5/StraitFlux/functions_VP.py`

 * *Files 0% similar despite different names*

```diff
@@ -495,7 +495,9 @@
         dist_listT_kurz2 = np.append(dist_listT_kurz2,distsT_kurz2)
     dist_lastT_kurz2 = prepro.distance(T_proj_lat[-2],T_proj_lon[-2],T_proj_lat[-1],T_proj_lon[-1])
     dist_listT_kurz2 = np.append(dist_listT_kurz2,dist_lastT_kurz2)
 
     return T_proj,dist_listT*1000,dist_listT_kurz2*1000
 
 
+
+
```

### Comparing `StraitFlux-1.0.4/StraitFlux/indices.py` & `straitflux-1.0.5/StraitFlux/indices.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,8 +342,7 @@
     out_v = out_v[~maskv]
     out_u_vz = np.delete(selection,2,1)
     out_u_vz = np.delete(out_u_vz,2,1)
     out_u_vz = out_u_vz[~masku]
 
     return out_u,out_v,out_u_vz
 
-
```

### Comparing `StraitFlux-1.0.4/StraitFlux/masterscript_cross.py` & `straitflux-1.0.5/StraitFlux/masterscript_cross.py`

 * *Files 3% similar despite different names*

```diff
@@ -373,7 +373,13 @@
         T_tot = xa.Dataset({'T':(('time','depth','x'),T_beitrag*(M_beitrag/M_beitrag))},coords=dict(time=t.time,depth=t.lev.data,x=np.cumsum(dist_listT_kurz2)))
         T_tot.to_netcdf(path_save+strait+'_crosssection_T_'+model+'_'+str(time_start)+'-'+str(time_end)+'.nc')
     elif product == 'S':            
         T_tot = xa.Dataset({'S':(('time','depth','x'),T_beitrag*(M_beitrag/M_beitrag))},coords=dict(time=t.time,depth=t.lev.data,x=np.cumsum(dist_listT_kurz2)))
         T_tot.to_netcdf(path_save+strait+'_crosssection_S_'+model+'_'+str(time_start)+'-'+str(time_end)+'.nc')
     return T_tot
 
+
+
+def calc_MOC(strait,model,time_start,time_end,file_u,file_v,file_t,file_z,coords=0,set_latlon=False,lat_p=0,lon_p=0,path_save='',path_indices='',path_mesh='',Arakawa='',saving=True):
+    uv=vel_projection(strait,model,time_start,time_end,file_u,file_v,file_t,file_z,coords=0,set_latlon=False,lat_p=0,lon_p=0,path_save='',path_indices='',path_mesh='',Arakawa='',saving=True)
+    MOC=(uv.uv*uv.dx_int*uv.dz_int).sum(axis=2)[:,::-1].cumsum('depth')/-1
+    return MOC
```

### Comparing `StraitFlux-1.0.4/StraitFlux/masterscript_line.py` & `straitflux-1.0.5/StraitFlux/masterscript_line.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,30 +18,31 @@
 import StraitFlux.preprocessing as prepro
 import StraitFlux.functions as func
 from StraitFlux.indices import check_availability_indices, prepare_indices
 
 
 
 
-def transports(product,strait,model,time_start,time_end,file_u,file_v,file_t,file_z,coords=0,set_latlon=False,lon_p=0,lat_p=0,file_s='',file_sic='',file_sit='',Arakawa='',rho=1026,cp=3996, Tref=0,path_save='',path_indices='',path_mesh='',saving=True):
+def transports(product,strait,model,time_start,time_end,file_u,file_v,file_t,file_z,mesh_dxv=0, mesh_dyu=0,coords=0,set_latlon=False,lon_p=0,lat_p=0,file_s='',file_sic='',file_sit='',Arakawa='',rho=1026,cp=3996, Tref=0,path_save='',path_indices='',path_mesh='',saving=True):
 
     '''Calculation of Transports using line integration
 
     INPUT Parameters:
     product (str): volume, heat, salt or ice
     strait (str): desired oceanic strait, either pre-defined from indices file or new
     model (str): desired CMIP6 model or reanalysis
     time_start (str or int): starting year
     time_end (str or int): ending year
-    file_u (str): path + filename(s) of u field(s); use ice velocities (ui) for ice transports; (multiple files possible, use *; must be possible to combine files over time coordinate)
+    file_u (str OR ): path + filename(s) of u field(s); use ice velocities (ui) for ice transports; (multiple files possible, use *; must be possible to combine files over time coordinate)
     file_v (str): path + filename(s) of v field(s); use ice velocities (vi) for ice transports; (multiple files possible, use *)
     file_t (str): path + filename(s) of temperature field(s); (multiple files possible, use *)
     file_z (str): path + filename(s) of cell thickness field(s); (multiple files possible, use *)
 
     OPTIONAL:
+    mesh_dxu/mesh_dyv (array): arrays containing the exact grid cell dimensions at northern and eastern grid cell faces of u and v cells (dxv and dyu); if not supplied will be calculated
     coords (tuple): coordinates for strait, if not pre-defined: (latitude_start,longitude_start,latitude_end,longitude_end)
     set_latlon: set True if you wish to pass arrays of latitudes and longitudes
     lon (array): longitude coordinates for strait, if not pre-defined. (range -180 to 180; same length as lat needed!)
     lat (array): latitude coordinates for strait, if not pre-defined. (range -90 to 90; same length as lon needed!)
     file_s (str): only needed for salinity transports; path + filename(s) of salinity field(s); (multiple files possible, use *)
     file_sic (str): only needed for ice transports; path + filename(s) of sea ice concentration field(s); (multiple files possible, use *)
     file_sit (str): only needed for ice transports; path + filename(s) of sea ice thickness field(s); (multiple files possible, use *)
@@ -79,15 +80,15 @@
         except NameError:
             ti=ti.load()
             ui=ui.load()
             vi=vi.load()
         indices,line = check_availability_indices(ti,strait,model,coords,lon_p,lat_p,set_latlon)
         i2=indices.indices.where(indices.indices!=0)
         try:
-            plt.pcolormesh((ui.uo))
+            plt.pcolormesh((ti.thetao/ti.thetao),cmap='tab20c')
             plt.scatter(i2[:,2],i2[:,3],color='tab:red',s=0.1,marker='x')
             plt.scatter(i2[:,0],i2[:,1],color='tab:red',s=0.1,marker='x')
             plt.title(model+'_'+strait,fontsize=14)
             plt.ylabel('y',fontsize=14)
             plt.xlabel('x',fontsize=14)
             plt.savefig(path_save+strait+'_'+model+'_indices.png')
             plt.close()
@@ -146,29 +147,35 @@
         min_x = 0
         max_x = max_x + 1
 
     try:
         mu=xa.open_dataset(path_mesh+'mesh_dyu_'+model+'.nc')
         mv=xa.open_dataset(path_mesh+'mesh_dxv_'+model+'.nc')
     except FileNotFoundError:
-        print('calc horizontal meshes')
-        try:
-            mu,mv = prepro.calc_dxdy(model,ui,vi,path_mesh)
-        except NameError:
-            print('read and load files for mesh')
-            ui = xa.open_mfdataset(file_u, preprocess=partial_func).isel(time=0)
-            vi = xa.open_mfdataset(file_v, preprocess=partial_func).isel(time=0)
+        if mesh_dxv!=0:
+            mesh_dxv.to_dataset(name='dxv').to_netcdf(path_mesh+'mesh_dxv_'+model+'.nc')
+            mesh_dyu.to_dataset(name='dyu').to_netcdf(path_mesh+'mesh_dyu_'+model+'.nc')
+            mu=xa.open_dataset(path_mesh+'mesh_dyu_'+model+'.nc')
+            mv=xa.open_dataset(path_mesh+'mesh_dxv_'+model+'.nc')
+        else:       
+            print('calc horizontal meshes')
             try:
-                with ProgressBar():
+                mu,mv = prepro.calc_dxdy(model,ui,vi,path_mesh)
+            except NameError:
+                print('read and load files for mesh')
+                ui = xa.open_mfdataset(file_u, preprocess=partial_func).isel(time=0)
+                vi = xa.open_mfdataset(file_v, preprocess=partial_func).isel(time=0)
+                try:
+                    with ProgressBar():
+                        ui=ui.load()
+                        vi=vi.load()
+                except NameError:
                     ui=ui.load()
                     vi=vi.load()
-            except NameError:
-                ui=ui.load()
-                vi=vi.load()
-            mu,mv = prepro.calc_dxdy(model,ui,vi,path_mesh)
+                mu,mv = prepro.calc_dxdy(model,ui,vi,path_mesh)
 
 
     print('read t, u and v fields')
     partial_func = partial(prepro._preprocess2,lon_bnds=(int(min_x)-1,int(max_x)+1),lat_bnds=(int(min_y)-1,int(max_y)+1))
     t = xa.open_mfdataset(file_t, preprocess=partial_func,chunks={'time':1})
     u = xa.open_mfdataset(file_u, preprocess=partial_func,chunks={'time':1})
     v = xa.open_mfdataset(file_v, preprocess=partial_func,chunks={'time':1})
@@ -308,8 +315,7 @@
     trans = trans.drop_vars('tot_'+product+'_flux')
     trans.to_netcdf(path_save+strait+'_'+product+'_'+model+'_'+str(time_start)+'-'+str(time_end)+'.nc')
 
     return trans
 
 
 
-
```

### Comparing `StraitFlux-1.0.4/StraitFlux/preprocessing.py` & `straitflux-1.0.5/StraitFlux/preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,16 +161,16 @@
     dz=np.sin(lat22)-np.sin(lat11)
     c=np.sqrt(dx*dx+dy*dy+dz*dz)
     distance=a*2*np.arcsin(c/2) 
     return distance
 
 def calc_dxdy(model,u,v,path_mesh):
 
-    dx=xa.DataArray(data=np.zeros(u.lat.shape),coords=u.lat.coords,dims=u.lat.dims)
-    dy=xa.DataArray(data=np.zeros(v.lat.shape),coords=v.lat.coords,dims=v.lat.dims)
+    dy=xa.DataArray(data=np.zeros(u.lat.shape),coords=u.lat.coords,dims=u.lat.dims)
+    dx=xa.DataArray(data=np.zeros(v.lat.shape),coords=v.lat.coords,dims=v.lat.dims)
     for i in tqdm(range(0,len(u.y)-1)):
         #print(i)
         dy[i+1,:]=distance(u.lat[i,:],u.lon[i,:],u.lat[i+1,:],u.lon[i+1,:])
     for i in tqdm(range(0,len(v.x)-1)):
         #print(i)
         dx[:,i+1]=distance(v.lat[:,i],v.lon[:,i],v.lat[:,i+1],v.lon[:,i+1])
             
@@ -231,7 +231,8 @@
             lon = np.degrees(np.arctan(y[i]/x[i])) + 180
         else:
             lon = np.degrees(np.arctan(y[i]/x[i])) - 180
         lon2=np.append(lon2,lon)
     return lat,lon2
 
 
+
```

### Comparing `StraitFlux-1.0.4/StraitFlux.egg-info/PKG-INFO` & `straitflux-1.0.5/StraitFlux.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StraitFlux
-Version: 1.0.4
+Version: 1.0.5
 Summary: StraitFlux
 Home-page: https://github.com/susannawinkelbauer/StraitFlux
 Download-URL: https://github.com/susannawinkelbauer/StraitFlux/archive/refs/tags/v1.0.4.tar.gz
 Author: Susanna Winkelbauer
 Author-email: susanna.winkelbauer@univie.ac.at
 Keywords: python,oceanic transports,curvilinear grids
 Classifier: Intended Audience :: Science/Research
```

### Comparing `StraitFlux-1.0.4/setup.py` & `straitflux-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name = 'StraitFlux',
     packages = ['StraitFlux'],
-    version = '1.0.4',
+    version = '1.0.5',
     install_requires=['xarray', 'netcdf4', 'xesmf', 'xmip', 'tqdm', 'matplotlib', 'dask'], #external packages as dependencies
     python_requires=">=3.10",
     description = 'StraitFlux',
     long_description = 'StraitFlux - calculates oceanic transports and crosssections on different model grids.',
     author = 'Susanna Winkelbauer',
     author_email = 'susanna.winkelbauer@univie.ac.at',
     url = 'https://github.com/susannawinkelbauer/StraitFlux',
```

