# Comparing `tmp/turbx-0.2.1.tar.gz` & `tmp/turbx-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbx-0.2.1.tar", last modified: Thu Apr 13 18:11:17 2023, max compression
+gzip compressed data, was "turbx-0.2.2.tar", last modified: Sat Apr 15 18:53:07 2023, max compression
```

## Comparing `turbx-0.2.1.tar` & `turbx-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 iagappel  (1000) iagappel  (1000)        0 2023-04-13 18:11:17.748169 turbx-0.2.1/
--rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     1065 2022-06-30 12:13:09.000000 turbx-0.2.1/LICENSE
--rw-rw-r--   0 iagappel  (1000) iagappel  (1000)     2342 2023-04-13 18:11:17.748169 turbx-0.2.1/PKG-INFO
--rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     1061 2022-07-01 07:43:09.000000 turbx-0.2.1/README.md
--rw-rw-r--   0 iagappel  (1000) iagappel  (1000)       38 2023-04-13 18:11:17.748169 turbx-0.2.1/setup.cfg
--rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     2295 2023-04-13 18:04:16.000000 turbx-0.2.1/setup.py
-drwxrwxr-x   0 iagappel  (1000) iagappel  (1000)        0 2023-04-13 18:11:17.748169 turbx-0.2.1/turbx/
--rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     2937 2023-04-13 18:06:57.000000 turbx-0.2.1/turbx/__init__.py
--rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)  1088399 2023-04-13 18:00:07.000000 turbx-0.2.1/turbx/turbx.py
-drwxrwxr-x   0 iagappel  (1000) iagappel  (1000)        0 2023-04-13 18:11:17.748169 turbx-0.2.1/turbx.egg-info/
--rw-rw-r--   0 iagappel  (1000) iagappel  (1000)     2342 2023-04-13 18:11:17.000000 turbx-0.2.1/turbx.egg-info/PKG-INFO
--rw-rw-r--   0 iagappel  (1000) iagappel  (1000)      203 2023-04-13 18:11:17.000000 turbx-0.2.1/turbx.egg-info/SOURCES.txt
--rw-rw-r--   0 iagappel  (1000) iagappel  (1000)        1 2023-04-13 18:11:17.000000 turbx-0.2.1/turbx.egg-info/dependency_links.txt
--rw-rw-r--   0 iagappel  (1000) iagappel  (1000)      143 2023-04-13 18:11:17.000000 turbx-0.2.1/turbx.egg-info/requires.txt
--rw-rw-r--   0 iagappel  (1000) iagappel  (1000)        6 2023-04-13 18:11:17.000000 turbx-0.2.1/turbx.egg-info/top_level.txt
+drwxrwxr-x   0 iagappel  (1000) iagappel  (1000)        0 2023-04-15 18:53:07.196434 turbx-0.2.2/
+-rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     1065 2022-06-30 12:13:09.000000 turbx-0.2.2/LICENSE
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)     2353 2023-04-15 18:53:07.196434 turbx-0.2.2/PKG-INFO
+-rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     1072 2023-04-15 18:45:25.000000 turbx-0.2.2/README.md
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)       38 2023-04-15 18:53:07.196434 turbx-0.2.2/setup.cfg
+-rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     2295 2023-04-15 18:44:51.000000 turbx-0.2.2/setup.py
+drwxrwxr-x   0 iagappel  (1000) iagappel  (1000)        0 2023-04-15 18:53:07.192434 turbx-0.2.2/turbx/
+-rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)     3154 2023-04-15 18:44:32.000000 turbx-0.2.2/turbx/__init__.py
+-rwxrwxr-x   0 iagappel  (1000) iagappel  (1000)  1143769 2023-04-15 18:41:25.000000 turbx-0.2.2/turbx/turbx.py
+drwxrwxr-x   0 iagappel  (1000) iagappel  (1000)        0 2023-04-15 18:53:07.196434 turbx-0.2.2/turbx.egg-info/
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)     2353 2023-04-15 18:53:07.000000 turbx-0.2.2/turbx.egg-info/PKG-INFO
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)      203 2023-04-15 18:53:07.000000 turbx-0.2.2/turbx.egg-info/SOURCES.txt
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)        1 2023-04-15 18:53:07.000000 turbx-0.2.2/turbx.egg-info/dependency_links.txt
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)      143 2023-04-15 18:53:07.000000 turbx-0.2.2/turbx.egg-info/requires.txt
+-rw-rw-r--   0 iagappel  (1000) iagappel  (1000)        6 2023-04-15 18:53:07.000000 turbx-0.2.2/turbx.egg-info/top_level.txt
```

### Comparing `turbx-0.2.1/LICENSE` & `turbx-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `turbx-0.2.1/PKG-INFO` & `turbx-0.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbx
-Version: 0.2.1
+Version: 0.2.2
 Summary: Extensible toolkit for analyzing turbulent flow datasets
 Home-page: https://github.com/iagappel/turbx
 Author: Jason A
 Maintainer: Jason A
 License: MIT
 Keywords: scientific computing,statistics,simulation,turbulence,turbulent flows,direct numerical simulation,DNS,parallel,visualization
 Platform: any
@@ -29,15 +29,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # turbx
 [![PyPI version](https://badge.fury.io/py/turbx.svg)](https://badge.fury.io/py/turbx)
 [![Downloads](https://pepy.tech/badge/turbx)](https://pepy.tech/project/turbx)
 
-Tools for analysis of turbulent flow datasets.
+Extensible toolkit for analyzing turbulent flow datasets.
 
 Install with `pip`:
 
 ```
 pip install --upgrade --user turbx
 ```
```

### Comparing `turbx-0.2.1/README.md` & `turbx-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # turbx
 [![PyPI version](https://badge.fury.io/py/turbx.svg)](https://badge.fury.io/py/turbx)
 [![Downloads](https://pepy.tech/badge/turbx)](https://pepy.tech/project/turbx)
 
-Tools for analysis of turbulent flow datasets.
+Extensible toolkit for analyzing turbulent flow datasets.
 
 Install with `pip`:
 
 ```
 pip install --upgrade --user turbx
 ```
```

### Comparing `turbx-0.2.1/setup.py` & `turbx-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='turbx',
-    version='0.2.1',
+    version='0.2.2',
     description='Extensible toolkit for analyzing turbulent flow datasets',
     
     long_description=long_description,
     long_description_content_type='text/markdown',
     
     url='https://github.com/iagappel/turbx',
     author='Jason A',
```

### Comparing `turbx-0.2.1/turbx/__init__.py` & `turbx-0.2.2/turbx/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''
 turbx
 
 Extensible toolkit for analyzing turbulent flow datasets
 '''
 
-__version__ = '0.2.1'
+__version__ = '0.2.2'
 __author__ = 'Jason A'
 
 from .turbx import cgd
 from .turbx import rgd
 from .turbx import eas4
 from .turbx import ztmd
 from .turbx import lpd
@@ -19,14 +19,17 @@
 
 from .turbx import eas3
 
 from .turbx import curve_fitter
 
 from .turbx import Blasius_solution
 from .turbx import freestream_parameters
+from .turbx import calc_bl_edge_1d
+from .turbx import calc_d99_1d
+from .turbx import calc_bl_integral_quantities_1d
 
 from .turbx import interp_2d_structured
 from .turbx import interp_1d
 from .turbx import fd_coeff_calculator
 from .turbx import gradient
 from .turbx import get_metric_tensor_3d
 from .turbx import get_metric_tensor_2d
@@ -72,14 +75,17 @@
            'spd',
            'h5_visititems_print_attrs',
            'h5_visit_container',
            'eas3',
            'curve_fitter',
            'Blasius_solution',
            'freestream_parameters',
+           'calc_bl_edge_1d',
+           'calc_d99_1d',
+           'calc_bl_integral_quantities_1d',
            'interp_2d_structured',
            'interp_1d',
            'fd_coeff_calculator',
            'gradient',
            'get_metric_tensor_3d',
            'get_metric_tensor_2d',
            'get_grid_quality_metrics_2d',
```

### Comparing `turbx-0.2.1/turbx/turbx.py` & `turbx-0.2.2/turbx/turbx.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,14 +261,20 @@
         if ('duration_avg' in self.attrs.keys()):
             self.duration_avg = self.attrs['duration_avg']
         if ('rectilinear' in self.attrs.keys()):
             self.rectilinear = self.attrs['rectilinear']
         if ('curvilinear' in self.attrs.keys()):
             self.curvilinear = self.attrs['curvilinear']
         
+        ## these should be set in the (init_from_() funcs)
+        if ('fclass' in self.attrs.keys()):
+            self.fclass = self.attrs['fclass'] ## 'cgd'
+        if ('fsubtype' in self.attrs.keys()):
+            self.fsubtype = self.attrs['fsubtype'] ## 'unsteady','mean','prime'
+        
         # === udef
         
         if ('header' in self):
             
             udef_real = np.copy(self['header/udef_real'][:])
             udef_char = np.copy(self['header/udef_char'][:]) ## the unpacked numpy array of |S128 encoded fixed-length character objects
             udef_char = [s.decode('utf-8') for s in udef_char] ## convert it to a python list of utf-8 strings
@@ -311,26 +317,30 @@
             cp      = self.cp      = self.R*self.kappa/(self.kappa-1.)
             cv      = self.cv      = self.cp/self.kappa
             r       = self.r       = self.Pr**(1/3)
             Tw      = self.Tw      = self.T_inf
             Taw     = self.Taw     = self.T_inf + self.r*self.U_inf**2/(2*self.cp)
             lchar   = self.lchar   = self.Re*self.nu_inf/self.U_inf
             
+            tchar   = self.tchar = self.lchar / self.U_inf
+            uchar   = self.uchar = self.U_inf
+            
             if verbose: print(72*'-')
             if verbose: even_print('rho_inf' , '%0.3f [kg/m³]'    % self.rho_inf )
             if verbose: even_print('mu_inf'  , '%0.6E [kg/(m·s)]' % self.mu_inf  )
             if verbose: even_print('nu_inf'  , '%0.6E [m²/s]'     % self.nu_inf  )
             if verbose: even_print('a_inf'   , '%0.6f [m/s]'      % self.a_inf   )
             if verbose: even_print('U_inf'   , '%0.6f [m/s]'      % self.U_inf   )
             if verbose: even_print('cp'      , '%0.3f [J/(kg·K)]' % self.cp      )
             if verbose: even_print('cv'      , '%0.3f [J/(kg·K)]' % self.cv      )
             if verbose: even_print('r'       , '%0.6f [-]'        % self.r       )
             if verbose: even_print('Tw'      , '%0.3f [K]'        % self.Tw      )
             if verbose: even_print('Taw'     , '%0.3f [K]'        % self.Taw     )
             if verbose: even_print('lchar'   , '%0.6E [m]'        % self.lchar   )
+            if verbose: even_print('tchar'   , '%0.6E [s]'        % self.tchar   )
             if verbose: print(72*'-')
             #if verbose: print(72*'-'+'\n')
             
             # === write the 'derived' udef variables to a dict attribute of the CGD instance
             udef_char_deriv = ['rho_inf', 'mu_inf', 'nu_inf', 'a_inf', 'U_inf', 'cp', 'cv', 'r', 'Tw', 'Taw', 'lchar']
             udef_real_deriv = [ rho_inf,   mu_inf,   nu_inf,   a_inf,   U_inf,   cp,   cv,   r,   Tw,   Taw,   lchar ]
             self.udef_deriv = dict(zip(udef_char_deriv, udef_real_deriv))
@@ -571,14 +581,18 @@
         # xi_max = kwargs.get('xi_max',None)
         # yi_max = kwargs.get('yi_max',None)
         # zi_max = kwargs.get('zi_max',None)
         
         ## grid filters are currently not supported for CGD
         self.hasGridFilter=False
         
+        ## set default attributes
+        self.attrs['fsubtype'] = 'unsteady'
+        self.attrs['fclass']   = 'cgd'
+        
         if verbose: print('\n'+'cgd.init_from_eas4()'+'\n'+72*'-')
         t_start_func = timeit.default_timer()
         
         if verbose: even_print('infile', os.path.basename(fn_eas4))
         if verbose: even_print('infile size', '%0.2f [GB]'%(os.path.getsize(fn_eas4)/1024**3))
         if verbose: even_print('outfile', self.fname)
         
@@ -867,14 +881,18 @@
         copy_grid = kwargs.get('copy_grid',True)
         chunk_kb = kwargs.get('chunk_kb',4*1024) ## 4 [MB]
         
         verbose = kwargs.get('verbose',True)
         if (self.rank!=0):
             verbose=False
         
+        ## set default attributes
+        self.attrs['fsubtype'] = 'unsteady'
+        self.attrs['fclass']   = 'cgd'
+        
         rx = kwargs.get('rx',1)
         ry = kwargs.get('ry',1)
         rz = kwargs.get('rz',1)
         
         if (rx*ry*rz != self.n_ranks):
             raise AssertionError('rx*ry*rz != self.n_ranks')
         
@@ -1065,15 +1083,47 @@
                 self.nt = self.t.size
                 self.create_dataset('dims/t', data=hf_ref.t)
             else:
                 t = np.array([0.], dtype=np.float64)
                 if ('dims/t' in self):
                     del self['dims/t']
                 self.create_dataset('dims/t', data=t)
-        
+            
+            # === 
+            
+            ## add additional [dims/<>] dsets
+            for dsn in [ 'dims/stang', 'dims/snorm', 'dims/crv_R' ]:
+                if (dsn in hf_ref):
+                    if (dsn in self):
+                        del self[dsn]
+                    data = np.copy(hf_ref[dsn][()])
+                    
+                    if (dsn=='dims/stang') and (data.shape!=(self.nx,)):
+                        raise ValueError
+                    if (dsn=='dims/snorm') and (data.shape!=(self.ny,)):
+                        raise ValueError
+                    
+                    ds = self.create_dataset(dsn, data=data, chunks=None)
+                    #if verbose: even_print(dsn,'%s'%str(ds.shape))
+            
+            ## add additional [csys/<>] dsets
+            for dsn in [ 'csys/vtang', 'csys/vnorm' ]:
+                if (dsn in hf_ref):
+                    if (dsn in self):
+                        del self[dsn]
+                    data = np.copy(hf_ref[dsn][()])
+                    
+                    if (data.ndim!=3):
+                        raise ValueError
+                    if (data.shape!=(self.nx,self.ny,2)):
+                        raise ValueError
+                    
+                    ds = self.create_dataset(dsn, data=data, chunks=None)
+                    #if verbose: even_print(dsn,'%s'%str(ds.shape))
+            
         self.get_header(verbose=False)
         return
     
     def import_eas4(self, fn_eas4_list, **kwargs):
         '''
         import data from a series of EAS4 files to a CGD
         '''
@@ -2467,24 +2517,18 @@
         if verbose: print('\n'+72*'-')
         if verbose: print('total time : cgd.make_test_file() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
         if verbose: print(72*'-')
         return
     
     # === post-processing
     
-    def calc_grid_metrics(self,):
-        '''
-        calculate the metric tensor M and save it to the file
-        '''
-        pass
-        return
-    
     def get_mean(self, **kwargs):
         '''
         get mean in [t] --> leaves [x,y,z,1]
+        --> save to new CGD file
         '''
         
         if (self.rank==0):
             verbose = True
         else:
             verbose = False
         
@@ -2572,65 +2616,83 @@
             ti_for_avg = np.copy( self.ti )
         
         nt_avg       = ti_for_avg.shape[0]
         t_avg_start  = self.t[ti_for_avg[0]]
         t_avg_end    = self.t[ti_for_avg[-1]]
         duration_avg = t_avg_end - t_avg_start
         
+        ## assert constant Δt, later attach dt as attribute to mean file
+        dt0 = np.diff(self.t)[0]
+        if not np.all(np.isclose(np.diff(self.t), dt0, rtol=1e-7)):
+            raise ValueError
+        
         if verbose: even_print('n timesteps avg','%i/%i'%(nt_avg,self.nt))
         if verbose: even_print('t index avg start','%i'%(ti_for_avg[0],))
         if verbose: even_print('t index avg end','%i'%(ti_for_avg[-1],))
         if verbose: even_print('t avg start','%0.2f [-]'%(t_avg_start,))
         if verbose: even_print('t avg end','%0.2f [-]'%(t_avg_end,))
         if verbose: even_print('duration avg','%0.2f [-]'%(duration_avg,))
+        if verbose: even_print('Δt','%0.2f [-]'%(dt0,))
         if verbose: print(72*'-')
         
         ## performance
         t_read = 0.
         t_write = 0.
         data_gb_read = 0.
         data_gb_write = 0.
         
         #data_gb      = 4*self.nx*self.ny*self.nz*self.nt / 1024**3
         data_gb      = 4*self.nx*self.ny*self.nz*nt_avg / 1024**3
         data_gb_mean = 4*self.nx*self.ny*self.nz*1      / 1024**3
         
-        scalars_re = ['u','v','w','p','T','rho']
-        scalars_fv = ['u','v','w','p','T','rho']
+        scalars_re = [ 'u','v','w','p','T','rho' ] #, 'utang','unorm', 'vort_x','vort_y','vort_z','vort_tang' ]
+        scalars_fv = [ 'u','v','w','p','T','rho' ]
         
         #with cgd(fn_cgd_mean, 'w', force=force, driver='mpio', comm=MPI.COMM_WORLD) as hf_mean:
         with cgd(fn_cgd_mean, 'w', force=force, driver=self.driver, comm=self.comm) as hf_mean:
             
+            ## initialize the mean file from the opened unsteady cgd file
+            hf_mean.init_from_cgd(self.fname, rx=rx,ry=ry,rz=rz, chunk_kb=chunk_kb)
+            
+            ## set some top-level attributes
             hf_mean.attrs['duration_avg'] = duration_avg ## duration of mean
             #hf_mean.attrs['duration_avg'] = self.duration
+            hf_mean.attrs['dt'] = dt0
+            #hf_mean.attrs['fclass'] = 'cgd'
+            hf_mean.attrs['fsubtype'] = 'mean'
             
-            hf_mean.init_from_cgd(self.fname, rx=rx,ry=ry,rz=rz) ## initialize the mean file from the cgd file
+            if verbose: print(72*'-')
             
             # === initialize mean datasets
             for scalar in self.scalars:
                 
                 shape  = (1,self.nz,self.ny,self.nx)
                 chunks = rgd.chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=2)
                 
                 if reynolds:
-                    if ('data/%s'%scalar in hf_mean):
-                        del hf_mean['data/%s'%scalar]
-                    if (self.rank==0):
-                        even_print('initializing data/%s'%(scalar,),'%0.3f [GB]'%(data_gb_mean,))
-                    dset = hf_mean.create_dataset('data/%s'%scalar,
-                                                  shape=shape,
-                                                  dtype=np.float32,
-                                                  chunks=chunks,
-                                                  )
-                    hf_mean.scalars.append('data/%s'%scalar)
                     
-                    chunk_kb_ = np.prod(dset.chunks)*4 / 1024. ## actual
-                    if verbose:
-                        even_print('chunk shape (t,z,y,x)','%s'%str(dset.chunks))
-                        even_print('chunk size','%i [KB]'%int(round(chunk_kb_)))
+                    ## do the Re mean of all scalars in file, regardless whether explicitly in scalars_re or not
+                    #if scalar in scalars_re:
+                    if True:
+                        
+                        if ('data/%s'%scalar in hf_mean):
+                            del hf_mean['data/%s'%scalar]
+                        if (self.rank==0):
+                            even_print('initializing data/%s'%(scalar,),'%0.3f [GB]'%(data_gb_mean,))
+                        dset = hf_mean.create_dataset('data/%s'%scalar,
+                                                    shape=shape,
+                                                    dtype=np.float32,
+                                                    chunks=chunks,
+                                                    )
+                        hf_mean.scalars.append('data/%s'%scalar)
+                        
+                        chunk_kb_ = np.prod(dset.chunks)*4 / 1024. ## actual
+                        if verbose:
+                            even_print('chunk shape (t,z,y,x)','%s'%str(dset.chunks))
+                            even_print('chunk size','%i [KB]'%int(round(chunk_kb_)))
                 
                 if favre:
                     if (scalar in scalars_fv):
                         if ('data/%s_fv'%scalar in hf_mean):
                             del hf_mean['data/%s_fv'%scalar]
                         if (self.rank==0):
                             even_print('initializing data/%s_fv'%(scalar,),'%0.3f [GB]'%(data_gb_mean,))
@@ -2702,15 +2764,18 @@
                 if reynolds:
                     data_mean    = np.mean(data,     axis=-1, keepdims=True, dtype=np.float64).astype(np.float32)
                 if favre:
                     data_mean_fv = np.mean(data*rho, axis=-1, keepdims=True, dtype=np.float64).astype(np.float32) / rho_mean
                 
                 # === write
                 if reynolds:
-                    if scalar in scalars_re:
+                    
+                    ## do the Re mean of all scalars in file, regardless whether explicitly in scalars_re or not
+                    #if scalar in scalars_re:
+                    if True:
                         
                         dset = hf_mean['data/%s'%scalar]
                         if self.usingmpi: self.comm.Barrier()
                         t_start = timeit.default_timer()
                         if self.usingmpi:
                             with dset.collective:
                                 dset[:,rz1:rz2,ry1:ry2,rx1:rx2] = data_mean.T
@@ -2767,30 +2832,429 @@
         if verbose: even_print('write total avg', '%0.2f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb_write,t_write,(data_gb_write/t_write)))
         if verbose: print(72*'-')
         #if verbose: print('\n'+72*'-')
         if verbose: print('total time : cgd.get_mean() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
         if verbose: print(72*'-')
         return
     
-    def get_mean_dimensional(self, **kwargs):
+    def add_mean_dimensional_data_xpln(self, **kwargs):
+        '''
+        get dimensionalized mean data for [x]/[s1] plane
+        --> save to existing CGD file with fsubtype=mean
+        - assumes volume which is thin in [x]/[s1] direction
+        - a CGD which is the output of cgd.get_mean() should be opened here
+        - not parallel
+        '''
+        
+        verbose = kwargs.get('verbose',True)
+        epsilon = kwargs.get('epsilon',5e-4)
+        
+        if (self.rank==0):
+            verbose = True
+        else:
+            verbose = False
+        
+        if verbose: print('\n'+'cgd.add_mean_dimensional_data_xpln()'+'\n'+72*'-')
+        t_start_func = timeit.default_timer()
+        
+        ## this func is not parallel
+        if self.usingmpi:
+            raise NotImplementedError
+        
+        ## 'r' and 'w' open modes are not allowed
+        if not (self.open_mode=='a') or (self.open_mode=='r+'):
+            raise ValueError(f'open mode is {self.open_mode}')
+        
+        ## assert that this is a mean flow file ( i.e. output from cgd.get_mean() )
+        if (self.fsubtype!='mean'):
+            print(self.fsubtype)
+            raise ValueError
+        
+        ## assert that 'data/utang' and 'data/unorm' are present
+        if not ('data/utang' in self):
+            raise ValueError
+        if not ('data/unorm' in self):
+            raise ValueError
+        
+        ## assert that 'dims/stang' and 'data/snorm' are present
+        if not ('dims/stang' in self):
+            raise ValueError
+        if not ('dims/snorm' in self):
+            raise ValueError
+        
+        ## get size of infile
+        fsize = os.path.getsize(self.fname)/1024**3
+        if verbose: even_print(os.path.basename(self.fname),'%0.1f [GB]'%fsize)
+        if verbose: even_print('nx','%i'%self.nx)
+        if verbose: even_print('ny','%i'%self.ny)
+        if verbose: even_print('nz','%i'%self.nz)
+        if verbose: even_print('nt','%i'%self.nt)
+        if verbose: even_print('ngp','%0.1f [M]'%(self.ngp/1e6,))
+        if verbose: print(72*'-')
+        
+        ## read in 3D coordinate arrays, then dimensinoalize [m]
+        x = np.copy( self['dims/x'][()].T * self.lchar )
+        y = np.copy( self['dims/y'][()].T * self.lchar )
+        z = np.copy( self['dims/z'][()].T * self.lchar )
+        nx = self.nx
+        ny = self.ny
+        nz = self.nz
+        
+        ## read in 1D coordinate arrays, then dimensinoalize [m]
+        stang_ = np.copy(self['dims/stang'])
+        stang  = np.copy( stang_ * self.lchar ) ## dimensional [m]
+        
+        snorm_ = np.copy(self['dims/snorm'])
+        snorm  = np.copy( snorm_ * self.lchar ) ## dimensional [m]
+        
+        ## assert [z] is same over all [x,y]
+        if (z.ndim!=3):
+            raise ValueError
+        z1d = np.copy(z[0,0,:])
+        for i in range(nx):
+            for j in range(ny):
+                np.testing.assert_allclose(z1d, z[i,j,:], rtol=1e-14, atol=1e-14)
+        
+        ## assert [x,y] is same over all [z]
+        x2d  = np.copy(x[:,:,0])
+        y2d  = np.copy(y[:,:,0])
+        xy2d = np.stack((x2d,y2d), axis=-1)
+        for k in range(nz):
+            x2d_  = np.copy(x[:,:,k])
+            y2d_  = np.copy(y[:,:,k])
+            xy2d_ = np.stack((x2d_,y2d_), axis=-1)
+            np.testing.assert_allclose(xy2d, xy2d_, rtol=1e-14, atol=1e-14)
+        
+        ## check if constant Δz (calculate Δz+ later)
+        dz0 = np.diff(z1d)[0]
+        if not np.all(np.isclose(np.diff(z1d), dz0, rtol=1e-7)):
+            raise NotImplementedError
+        
+        ## check if mean cgd has attr 'dt'
+        if ('dt' in self.attrs.keys()):
+            dt = self.attrs['dt']
+            if (dt is not None):
+                dt *= self.tchar
+        else:
+            raise ValueError
+        
+        if verbose: even_print('Δt/tchar','%0.8f'%(dt/self.tchar))
+        if verbose: even_print('Δt','%0.3e [s]'%(dt,))
+        if verbose: even_print('duration/tchar','%0.1f'%(self.duration_avg,))
+        if verbose: even_print('duration','%0.3e [s]'%(self.duration_avg*self.tchar,))
+        if verbose: print(72*'-')
+        
+        u   =  self.U_inf                     * np.copy( self['data/u'][()].T   )
+        v   =  self.U_inf                     * np.copy( self['data/v'][()].T   )
+        w   =  self.U_inf                     * np.copy( self['data/w'][()].T   )
+        rho =  self.rho_inf                   * np.copy( self['data/rho'][()].T )
+        p   =  (self.rho_inf * self.U_inf**2) * np.copy( self['data/p'][()].T   )
+        T   =  self.T_inf                     * np.copy( self['data/T'][()].T   )
+        
+        utang = self.U_inf * np.copy( self['data/utang'][()].T )
+        unorm = self.U_inf * np.copy( self['data/unorm'][()].T )
+        
+        # mu1 = (14.58e-7 * T**1.5) / ( T + 110.4 )
+        # mu2 = self.mu_Suth_ref * ( T / self.T_Suth_ref )**(3/2) * (self.T_Suth_ref+self.S_Suth)/(T+self.S_Suth)
+        # mu3 = self.C_Suth * T**(3/2) / (T + self.S_Suth)
+        # np.testing.assert_allclose(mu1, mu2, rtol=1e-14, atol=1e-14)
+        # np.testing.assert_allclose(mu2, mu3, rtol=1e-14, atol=1e-14)
+        # mu = np.copy(mu3)
+        
+        mu = self.C_Suth * T**(3/2) / (T + self.S_Suth)
+        nu = mu / rho
+        
+        # === average in [z]/[s3] --> leave 2D [x,y]/[s1,s2]
+        
+        u     = np.squeeze( np.mean( u     , axis=2, dtype=np.float64).astype(np.float32) )
+        v     = np.squeeze( np.mean( v     , axis=2, dtype=np.float64).astype(np.float32) )
+        w     = np.squeeze( np.mean( w     , axis=2, dtype=np.float64).astype(np.float32) )
+        rho   = np.squeeze( np.mean( rho   , axis=2, dtype=np.float64).astype(np.float32) )
+        p     = np.squeeze( np.mean( p     , axis=2, dtype=np.float64).astype(np.float32) )
+        T     = np.squeeze( np.mean( T     , axis=2, dtype=np.float64).astype(np.float32) )
+        utang = np.squeeze( np.mean( utang , axis=2, dtype=np.float64).astype(np.float32) )
+        unorm = np.squeeze( np.mean( unorm , axis=2, dtype=np.float64).astype(np.float32) )
+        mu    = np.squeeze( np.mean( mu    , axis=2, dtype=np.float64).astype(np.float32) )
+        nu    = np.squeeze( np.mean( nu    , axis=2, dtype=np.float64).astype(np.float32) )
+        
+        # === get 2D metric tensor
+        
+        if (nx<3):
+            raise ValueError('dds1[] not possible because nx<3')
+        elif (nx>=3) and (nx<5):
+            acc = 2
+        elif (nx>=5) and (nx<7):
+            acc = 4
+        elif (nx>=7):
+            acc = 6
+        else:
+            raise ValueError('this should never happen')
+        
+        edge_stencil = 'half'
+        if verbose: even_print('acc','%i'%acc)
+        if verbose: even_print('edge_stencil',edge_stencil)
+        
+        M = get_metric_tensor_2d(x2d, y2d, acc=acc, edge_stencil=edge_stencil, no_warn=True, verbose=verbose)
+        
+        ddx_q1 = np.copy( M[:,:,0,0] ) ## ξ_x
+        ddx_q2 = np.copy( M[:,:,1,0] ) ## η_x
+        ddy_q1 = np.copy( M[:,:,0,1] ) ## ξ_y
+        ddy_q2 = np.copy( M[:,:,1,1] ) ## η_y
+        
+        if verbose: even_print('ξ_x','%s'%str(ddx_q1.shape))
+        if verbose: even_print('η_x','%s'%str(ddx_q2.shape))
+        if verbose: even_print('ξ_y','%s'%str(ddy_q1.shape))
+        if verbose: even_print('η_y','%s'%str(ddy_q2.shape))
+        
+        M = None; del M
+        
+        ## the 'computational' grid (unit Cartesian)
+        #x_comp = np.arange(nx, dtype=np.float64)
+        #y_comp = np.arange(ny, dtype=np.float64)
+        x_comp = 1.
+        y_comp = 1.
+        
+        # === get gradients & vort_z
+        
+        ddx_u_comp = gradient(u, x_comp, axis=0, acc=acc, edge_stencil=edge_stencil, d=1, no_warn=True)
+        ddy_u_comp = gradient(u, y_comp, axis=1, acc=acc, edge_stencil=edge_stencil, d=1, no_warn=True)
+        ddx_u      = ddx_u_comp*ddx_q1 + ddy_u_comp*ddx_q2
+        ddy_u      = ddx_u_comp*ddy_q1 + ddy_u_comp*ddy_q2
+        
+        ddx_v_comp = gradient(v, x_comp, axis=0, acc=acc, edge_stencil=edge_stencil, d=1, no_warn=True)
+        ddy_v_comp = gradient(v, y_comp, axis=1, acc=acc, edge_stencil=edge_stencil, d=1, no_warn=True)
+        ddx_v      = ddx_v_comp*ddx_q1 + ddy_v_comp*ddx_q2
+        ddy_v      = ddx_v_comp*ddy_q1 + ddy_v_comp*ddy_q2
+        
+        ## dimensional [1/s]
+        vort_z = ddx_v - ddy_u
+        
+        # ===
+        
+        s1 = np.copy( stang )
+        s2 = np.copy( snorm )
+        
+        ## [s2] gradients --> yields 1D in [y]/[s2]
+        dds2_u     = gradient(u     , s2, axis=1, acc=acc, edge_stencil=edge_stencil)
+        dds2_v     = gradient(v     , s2, axis=1, acc=acc, edge_stencil=edge_stencil)
+        dds2_T     = gradient(T     , s2, axis=1, acc=acc, edge_stencil=edge_stencil)
+        dds2_p     = gradient(p     , s2, axis=1, acc=acc, edge_stencil=edge_stencil)
+        dds2_rho   = gradient(rho   , s2, axis=1, acc=acc, edge_stencil=edge_stencil)
+        dds2_utang = gradient(utang , s2, axis=1, acc=acc, edge_stencil=edge_stencil)
+        dds2_unorm = gradient(unorm , s2, axis=1, acc=acc, edge_stencil=edge_stencil)
+        
+        ## wall quantities --> mean over [x]/[s1] --> leave 0D float
+        dds2_u1_wall = float( np.mean( dds2_utang[:,0] ) )
+        dds2_T       = float( np.mean( dds2_T[:,0]     ) )
+        rho_wall     = float( np.mean( rho[:,0]        ) )
+        nu_wall      = float( np.mean( nu[:,0]         ) )
+        mu_wall      = float( np.mean( mu[:,0]         ) )
+        T_wall       = float( np.mean( T[:,0]          ) )
+        tau_wall     = mu_wall * dds2_u1_wall
+        q_wall       = self.cp * mu_wall / self.Pr * dds2_T ### wall heat flux
+        
+        ## friction velocity
+        u_tau  = np.sqrt(tau_wall/rho_wall)
+        #y_plus = np.copy( s2 * u_tau / nu_wall )
+        
+        # === populate 1D & 2D arrays using calc_bl_edge_1d(), calc_d99_1d()
+        
+        psvel = np.zeros((nx,ny), dtype=np.float64)
+        
+        psvel_edge = np.zeros((nx,), dtype=np.float64)
+        u1_edge    = np.zeros((nx,), dtype=np.float64)
+        rho_edge   = np.zeros((nx,), dtype=np.float64)
+        mu_edge    = np.zeros((nx,), dtype=np.float64)
+        nu_edge    = np.zeros((nx,), dtype=np.float64)
+        T_edge     = np.zeros((nx,), dtype=np.float64)
+        
+        s2_edge = np.zeros((nx,), dtype=np.float64)
+        d99     = np.zeros((nx,), dtype=np.float64)
+        
+        u1_99  = np.zeros((nx,), dtype=np.float64)
+        
+        for i in range(nx):
+            
+            vort_z_ = np.copy( vort_z[i,:] )
+            psvel_  = sp.integrate.cumulative_trapezoid(-1*vort_z_, s2, initial=0.)
+            psvel[i,:] = psvel_
+            
+            ## get edge
+            s2_edge_ = calc_bl_edge_1d( y=s2, psvel=psvel_, ynorm=self.lchar, acc=acc, edge_stencil=edge_stencil, epsilon=epsilon )
+            #aa = ( s2_edge_ - s2.min() ) / ( s2.max() - s2.min() )
+            #tqdm.write(f'{aa:0.9f}')
+            s2_edge[i] = s2_edge_
+            
+            ## interpolate at edge
+            psvel_edge_ = sp.interpolate.interp1d(s2, psvel_ , kind='cubic', bounds_error=True)(s2_edge_)
+            psvel_edge_ = float(psvel_edge_)
+            psvel_edge[i] = psvel_edge_
+            
+            u1_edge[i]  = sp.interpolate.interp1d(s2, utang[i,:] , kind='cubic', bounds_error=True)(s2_edge_)
+            rho_edge[i] = sp.interpolate.interp1d(s2, rho[i,:]   , kind='cubic', bounds_error=True)(s2_edge_)
+            mu_edge[i]  = sp.interpolate.interp1d(s2, mu[i,:]    , kind='cubic', bounds_error=True)(s2_edge_)
+            nu_edge[i]  = sp.interpolate.interp1d(s2, nu[i,:]    , kind='cubic', bounds_error=True)(s2_edge_)
+            T_edge[i]   = sp.interpolate.interp1d(s2, T[i,:]     , kind='cubic', bounds_error=True)(s2_edge_)
+            
+            ## get d99
+            d99_ = calc_d99_1d( y=s2, y_edge=s2_edge_, psvel=psvel_, psvel_edge=psvel_edge_ )
+            d99_ = float(d99_)
+            d99[i] = d99_
+            
+            u1_99[i] = sp.interpolate.interp1d(s2, utang[i,:] , kind='cubic', bounds_error=True)(d99_)
+        
+        # === avg in [x]/[s1] --> leave [y]/[s2]
+        
+        psvel = np.mean( psvel , axis=0 )
+        utang = np.mean( utang , axis=0 )
+        rho   = np.mean( rho   , axis=0 )
+        
+        psvel_edge  = np.mean( psvel_edge )
+        u1_edge     = np.mean( u1_edge    )
+        rho_edge    = np.mean( rho_edge   )
+        mu_edge     = np.mean( mu_edge    )
+        nu_edge     = np.mean( nu_edge    )
+        T_edge      = np.mean( T_edge     )
+        
+        s2_edge     = np.mean( s2_edge     )
+        d99         = np.mean( d99        )
+        
+        u1_99       = np.mean( u1_99      )
+        
+        sc_l_out = d99
+        sc_u_out = u1_99
+        sc_t_out = d99/u1_99
+        np.testing.assert_allclose(sc_t_out, sc_l_out/sc_u_out, rtol=1e-14, atol=1e-14)
+        
+        sc_u_in = u_tau
+        sc_l_in = nu_wall / u_tau
+        sc_t_in = nu_wall / u_tau**2
+        np.testing.assert_allclose(sc_t_in, sc_l_in/sc_u_in, rtol=1e-14, atol=1e-14)
+        
+        t_meas = self.duration_avg * (self.lchar / self.U_inf)
+        t_eddy = t_meas / (d99/u_tau)
+        
+        # === get 0D BL integral quantities
+        
+        dd = calc_bl_integral_quantities_1d( y=s2,
+                                             u=utang,
+                                             rho=rho,
+                                             u_tau=u_tau,
+                                             d99=d99,
+                                             y_edge=s2_edge,
+                                             rho_edge=rho_edge,
+                                             nu_edge=nu_edge,
+                                             u_edge=u1_edge,
+                                             nu_wall=nu_wall,
+                                            )
+        
+        # === add to file
+        
+        gn = 'data_dim'
+        if (gn in self):
+            del self[gn]
+        
+        ## 1D
+        self.create_dataset(f'{gn}/psvel' , data=psvel, chunks=None)
+        self.create_dataset(f'{gn}/utang' , data=utang, chunks=None)
+        self.create_dataset(f'{gn}/rho'   , data=rho,   chunks=None)
+        
+        self.create_dataset(f'{gn}/z1d'   , data=z1d,   chunks=None)
+        
+        ## 0D
+        self.create_dataset(f'{gn}/dz0'        , data=dz0, chunks=None)
+        self.create_dataset(f'{gn}/dt'         , data=dt, chunks=None)
+        
+        self.create_dataset(f'{gn}/s2_edge'    , data=s2_edge    , chunks=None)
+        self.create_dataset(f'{gn}/d99'        , data=d99        , chunks=None)
+        self.create_dataset(f'{gn}/u1_99'      , data=u1_99      , chunks=None)
+        
+        self.create_dataset(f'{gn}/psvel_edge' , data=psvel_edge , chunks=None)
+        self.create_dataset(f'{gn}/u1_edge'    , data=u1_edge    , chunks=None)
+        self.create_dataset(f'{gn}/rho_edge'   , data=rho_edge   , chunks=None)
+        self.create_dataset(f'{gn}/mu_edge'    , data=mu_edge    , chunks=None)
+        self.create_dataset(f'{gn}/nu_edge'    , data=nu_edge    , chunks=None)
+        self.create_dataset(f'{gn}/T_edge'     , data=T_edge     , chunks=None)
+        
+        self.create_dataset(f'{gn}/u_tau'      , data=u_tau      , chunks=None)
+        
+        self.create_dataset(f'{gn}/dds2_u1_wall' , data=dds2_u1_wall , chunks=None )
+        self.create_dataset(f'{gn}/dds2_T'       , data=dds2_T       , chunks=None )
+        self.create_dataset(f'{gn}/rho_wall'     , data=rho_wall     , chunks=None )
+        self.create_dataset(f'{gn}/nu_wall'      , data=nu_wall      , chunks=None )
+        self.create_dataset(f'{gn}/mu_wall'      , data=mu_wall      , chunks=None )
+        self.create_dataset(f'{gn}/T_wall'       , data=T_wall       , chunks=None )
+        self.create_dataset(f'{gn}/tau_wall'     , data=tau_wall     , chunks=None )
+        self.create_dataset(f'{gn}/q_wall'       , data=q_wall       , chunks=None )
+        
+        self.create_dataset(f'{gn}/sc_u_in'    , data=sc_u_in    , chunks=None)
+        self.create_dataset(f'{gn}/sc_l_in'    , data=sc_l_in    , chunks=None)
+        self.create_dataset(f'{gn}/sc_t_in'    , data=sc_t_in    , chunks=None)
+        self.create_dataset(f'{gn}/sc_u_out'   , data=sc_u_out   , chunks=None)
+        self.create_dataset(f'{gn}/sc_l_out'   , data=sc_l_out   , chunks=None)
+        self.create_dataset(f'{gn}/sc_t_out'   , data=sc_t_out   , chunks=None)
+        
+        ## add integrated quantities (all 0D)
+        for key,val in dd.items():
+            self.create_dataset(f'{gn}/{key}', data=val, chunks=None)
+        
+        # === report
+        
+        if verbose:
+            print(72*'-')
+            even_print('Re_τ'                      , '%0.1f'%dd['Re_tau']            )
+            even_print('Re_θ'                      , '%0.1f'%dd['Re_theta']          )
+            even_print('θ'                         , '%0.5e [m]'%dd['theta_cmp']     )
+            even_print('δ*'                        , '%0.5e [m]'%dd['dstar_cmp']     )
+            even_print('H12'                       , '%0.5f'%dd['H12']               )
+            ##
+            even_print('δ99'                       , '%0.5e [m]'%d99                 )
+            even_print('u_τ'                       , '%0.3f [m/s]'%u_tau             )
+            even_print('ν_wall'                    , '%0.5e [m²/s]'%nu_wall          )
+            even_print('t_meas'                    , '%0.5e [s]'%t_meas              )
+            even_print('t_meas/tchar'              , '%0.1f'%(t_meas/self.tchar)     )
+            even_print('t_eddy = t_meas/(δ99/u_τ)' , '%0.2f'%t_eddy                  )
+            even_print('t_meas/(δ99/u1_99)'        , '%0.2f'%(t_meas/(d99/u1_99))    )
+            even_print('t_meas/(20·δ99/u1_99)'     , '%0.2f'%(t_meas/(20*d99/u1_99)) )
+            print(72*'-')
+            even_print('sc_u_in = u_τ'               , '%0.5e [m/s]'%(sc_u_in,)  )
+            even_print('sc_l_in = δ_ν = ν_wall/u_τ'  , '%0.5e [m]'%(sc_l_in,)    )
+            even_print('sc_t_in = t_ν = ν_wall/u_τ²' , '%0.5e [s]'%(sc_t_in,)    )
+            even_print('sc_u_out = u1_99'            , '%0.5e [m/s]'%(sc_u_out,) )
+            even_print('sc_l_out = δ99'              , '%0.5e [m]'%(sc_l_out,)   )
+            even_print('sc_t_out = δ99/u1_99'        , '%0.5e [s]'%(sc_t_out,)   )
+        
+        # ===
+        
+        if verbose: print(72*'-')
+        if verbose: print('total time : cgd.add_mean_dimensional_data_xpln() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
+        if verbose: print(72*'-')
+        
         return
     
+    # === post-processing (unsteady)
+    
     def get_prime(self, **kwargs):
         '''
         get mean-removed (prime) variables in [t]
+        --> save to new CGD file
         -----
         XI  : Reynolds primes : mean(XI)=0
         XII : Favre primes    : mean(ρ·XII)=0 --> mean(XII)≠0 !!
         '''
         
         if (self.rank==0):
             verbose = True
         else:
             verbose = False
         
+        ## assert that the opened CGD has fsubtype 'unsteady'
+        if (self.fsubtype!='unsteady'):
+            raise ValueError
+        
         if verbose: print('\n'+'cgd.get_prime()'+'\n'+72*'-')
         t_start_func = timeit.default_timer()
         
         rx = kwargs.get('rx',1)
         ry = kwargs.get('ry',1)
         rz = kwargs.get('rz',1)
         #rt = kwargs.get('rt',1)
@@ -2920,16 +3384,16 @@
         data_gb_read = 0.
         data_gb_write = 0.
         
         #data_gb      = 4*self.nx*self.ny*self.nz*self.nt / 1024**3
         data_gb      = 4*self.nx*self.ny*self.nz*nt_prime / 1024**3
         data_gb_mean = 4*self.nx*self.ny*self.nz*1       / 1024**3
         
-        scalars_re = ['u','v','w','T','p','rho']
-        scalars_fv = ['u','v','w','T'] ## p'' and ρ'' are never really needed
+        scalars_re = ['u','v','w','T','p','rho', 'utang', 'unorm']
+        scalars_fv = ['u','v','w','T', 'utang', 'unorm'] ## p'' and ρ'' are never really needed
         
         scalars_re_ = []
         for scalar in scalars_re:
             if (scalar in self.scalars) and (scalar in sfp):
                 scalars_re_.append(scalar)
         scalars_re = scalars_re_
         
@@ -2941,15 +3405,20 @@
         
         # ===
         
         comm_cgd_prime = MPI.COMM_WORLD
         
         with cgd(fn_cgd_prime, 'w', force=force, driver=self.driver, comm=self.comm) as hf_prime:
             
-            hf_prime.init_from_cgd(self.fname, rx=rx,ry=ry,rz=rz)
+            ## initialize CGD file
+            hf_prime.init_from_cgd(self.fname, rx=rx,ry=ry,rz=rz, chunk_kb=chunk_kb)
+            
+            ## add top-level attributes
+            #hf_prime.attrs['fclass'] = 'cgd'
+            hf_prime.attrs['fsubtype'] = 'prime'
             
             #shape  = (self.nt,self.nz,self.ny,self.nx)
             shape  = (nt_prime,self.nz,self.ny,self.nx)
             chunks = rgd.chunk_sizer(nxi=shape, constraint=(1,None,None,None), size_kb=chunk_kb, base=2)
             
             # === initialize prime datasets + rho
             
@@ -3017,14 +3486,31 @@
                 if (scalar in scalars_fv) and favre:
                     n_pbar += 1
             
             comm_cgd_mean = MPI.COMM_WORLD
             
             with cgd(fn_cgd_mean, 'r', driver=self.driver, comm=self.comm) as hf_mean:
                 
+                ## copy over 'data_dim' from mean file
+                if ('data_dim' in hf_mean):
+                    grp = hf_mean['data_dim']
+                    for dsn in grp.keys():
+                        ds = hf_mean[f'data_dim/{dsn}']
+                        data = np.copy(ds[()])
+                        #if (f'data_dim/{dsn}' in hf_prime):
+                        #    del hf_prime[f'data_dim/{dsn}']
+                        
+                        #if self.usingmpi:
+                        #    with dset.collective:
+                        #        hf_prime.create_dataset(f'data_dim/{dsn}', data=data, chunks=None)
+                        #else:
+                        #    hf_prime.create_dataset(f'data_dim/{dsn}', data=data, chunks=None)
+                        
+                        hf_prime.create_dataset(f'data_dim/{dsn}', data=data, chunks=None)
+                
                 if verbose:
                     progress_bar = tqdm(total=ct*n_pbar, ncols=100, desc='prime', leave=False, file=sys.stdout)
                 
                 for ctl_ in ctl:
                     ct1, ct2 = ctl_
                     ntc = ct2 - ct1
                     
@@ -5132,14 +5618,528 @@
         
         if verbose: print(72*'-')
         if verbose: print('total time : cgd.calc_vorticity_tangnorm() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
         if verbose: print(72*'-')
         
         return
     
+    # ===
+    
+    def calc_turb_spectrum_span_xpln(self, **kwargs):
+        '''
+        calculate FFT in [z] (wavenumber) at every [x,y,t], avg in [x,t]
+        - designed for analyzing unsteady, thin planes in [x]
+        '''
+        
+        if (self.rank==0):
+            verbose = True
+        else:
+            verbose = False
+        
+        if verbose: print('\n'+'cgd.calc_turb_spectrum_span_xpln()'+'\n'+72*'-')
+        t_start_func = timeit.default_timer()
+        
+        rx = kwargs.get('rx',1)
+        ry = kwargs.get('ry',1)
+        rz = kwargs.get('rz',1)
+        rt = kwargs.get('rt',1)
+        
+        fn_dat_fft  = kwargs.get('fn_dat_fft',None)
+        fn_cgd_mean = kwargs.get('fn_cgd_mean',None)
+        
+        ## assert that a CGD with (fsubtype=='prime') was opened
+        if (self.fsubtype!='prime'):
+            raise ValueError("fsubtype!='prime'")
+        
+        ## for now only distribute data in [y] --> allows [x,t] mean before Send/Recv
+        if (rx!=1):
+            raise AssertionError('rx!=1')
+        if (rz!=1):
+            raise AssertionError('rz!=1')
+        if (rt!=1):
+            raise AssertionError('rt!=1')
+        
+        ## check the choice of ranks per dimension
+        if (rx*ry*rz*rt != self.n_ranks):
+            raise AssertionError('rx*ry*rz*rt != self.n_ranks')
+        if (rx>self.nx):
+            raise AssertionError('rx>self.nx')
+        if (ry>self.ny):
+            raise AssertionError('ry>self.ny')
+        if (rz>self.nz):
+            raise AssertionError('rz>self.nz')
+        if (rt>self.nt):
+            raise AssertionError('rt>self.nt')
+        
+        # === distribute 4D data over ranks
+        
+        #comm4d = self.comm.Create_cart(dims=[rx,ry,ry,rt], periods=[False,False,False,False], reorder=False)
+        #t4d = comm4d.Get_coords(self.rank)
+        
+        #rxl_ = np.array_split(np.arange(self.nx,dtype=np.int64),min(rx,self.nx))
+        ryl_ = np.array_split(np.arange(self.ny,dtype=np.int64),min(ry,self.ny))
+        #rzl_ = np.array_split(np.arange(self.nz,dtype=np.int64),min(rz,self.nz))
+        #rtl_ = np.array_split(np.arange(self.nt,dtype=np.int64),min(rt,self.nt))
+        
+        #rxl = [[b[0],b[-1]+1] for b in rxl_ ]
+        ryl = [[b[0],b[-1]+1] for b in ryl_ ]
+        #rzl = [[b[0],b[-1]+1] for b in rzl_ ]
+        #rtl = [[b[0],b[-1]+1] for b in rtl_ ]
+        
+        #rx1, rx2 = rxl[t4d[0]]; nxr = rx2 - rx1
+        #ry1, ry2 = ryl[t4d[1]]; nyr = ry2 - ry1
+        #rz1, rz2 = rzl[t4d[2]]; nzr = rz2 - rz1
+        #rt1, rt2 = rtl[t4d[3]]; ntr = rt2 - rt1
+        
+        ry1,ry2 = ryl[self.rank]; nyr = ry2 - ry1
+        
+        # # === mean file name (for reading)
+        # if (fn_cgd_mean is None):
+        #     fname_path = os.path.dirname(self.fname)
+        #     fname_base = os.path.basename(self.fname)
+        #     fname_root, fname_ext = os.path.splitext(fname_base)
+        #     if ('_prime' in fname_root):
+        #         fname_root = fname_root.replace('_prime','')
+        #     fname_mean_h5_base = fname_root+'_mean.h5'
+        #     #fn_cgd_mean = os.path.join(fname_path, fname_mean_h5_base)
+        #     fn_cgd_mean = str(PurePosixPath(fname_path, fname_mean_h5_base))
+        #     #fn_cgd_mean = Path(fname_path, fname_mean_h5_base)
+        
+        # === fft file name (for writing) : dat
+        if (fn_dat_fft is None):
+            fname_path = os.path.dirname(self.fname)
+            fname_base = os.path.basename(self.fname)
+            fname_root, fname_ext = os.path.splitext(fname_base)
+            fname_root = re.findall('io\S+_mpi_[0-9]+', fname_root)[0]
+            fname_fft_dat_base = fname_root+'_turb_spec_span.dat'
+            fn_dat_fft = str(PurePosixPath(fname_path, fname_fft_dat_base))
+        
+        if verbose: even_print('fn_cgd_prime'    , self.fname   )
+        #if verbose: even_print('fn_cgd_mean'     , fn_cgd_mean  )
+        if verbose: even_print('fn_dat_fft'      , fn_dat_fft   )
+        if verbose: print(72*'-')
+        
+        #if not os.path.isfile(fn_cgd_mean):
+        #    raise FileNotFoundError('%s not found'%fn_cgd_mean)
+        
+        #with cgd(fn_cgd_mean, 'r', driver=self.driver, comm=self.comm) as hf_mean:
+        #    if (self.fsubtype!='mean'):
+        #        raise ValueError("fsubtype!='mean'")
+        
+        # ===
+        
+        ## the data dictionary to be pickled later
+        data = {}
+        
+        if ('data_dim' not in self):
+            raise ValueError('data_dim not present')
+        
+        ## put all data from 'data_dim' into the dictionary data which will be pickled at the end
+        for dsn in self['data_dim'].keys():
+            d_ = np.copy( self[f'data_dim/{dsn}'][()] )
+            if (d_.ndim == 0):
+                d_ = float(d_)
+            data[dsn] = d_
+        
+        ## 1D
+        rho   = np.copy( self['data_dim/rho'][()]   )
+        utang = np.copy( self['data_dim/utang'][()] )
+        
+        ## 0D
+        u_tau    = float( self['data_dim/u_tau'][()]    )
+        nu_wall  = float( self['data_dim/nu_wall'][()]  )
+        rho_wall = float( self['data_dim/rho_wall'][()] )
+        d99      = float( self['data_dim/d99'][()]      )
+        u1_99    = float( self['data_dim/u1_99'][()]    )
+        Re_tau   = float( self['data_dim/Re_tau'][()]   )
+        Re_theta = float( self['data_dim/Re_theta'][()] )
+        sc_u_in  = float( self['data_dim/sc_u_in'][()]  )
+        sc_l_in  = float( self['data_dim/sc_l_in'][()]  )
+        sc_t_in  = float( self['data_dim/sc_t_in'][()]  )
+        sc_u_out = float( self['data_dim/sc_u_out'][()] )
+        sc_l_out = float( self['data_dim/sc_l_out'][()] )
+        sc_t_out = float( self['data_dim/sc_t_out'][()] )
+        
+        ## these are recalculated and checked in next step
+        z1d_ = np.copy( self['data_dim/z1d'][()] )
+        dz0_ = np.copy( self['data_dim/dz0'][()] )
+        dt_  = np.copy( self['data_dim/dt'][()]  )
+        
+        # ===
+        
+        ## get size of infile
+        fsize = os.path.getsize(self.fname)/1024**3
+        if verbose: even_print(os.path.basename(self.fname),'%0.1f [GB]'%fsize)
+        if verbose: even_print('nx','%i'%self.nx)
+        if verbose: even_print('ny','%i'%self.ny)
+        if verbose: even_print('nz','%i'%self.nz)
+        if verbose: even_print('nt','%i'%self.nt)
+        if verbose: even_print('ngp','%0.1f [M]'%(self.ngp/1e6,))
+        if verbose: print(72*'-')
+        
+        lchar   = self.lchar   ; data['lchar']   = lchar
+        U_inf   = self.U_inf   ; data['U_inf']   = U_inf
+        rho_inf = self.rho_inf ; data['rho_inf'] = rho_inf
+        T_inf   = self.T_inf   ; data['T_inf']   = T_inf
+        
+        ## read in 3D coordinate arrays, then dimensinoalize [m]
+        ## every ranks gets full grid
+        x = np.copy( self['dims/x'][()].T * self.lchar )
+        y = np.copy( self['dims/y'][()].T * self.lchar )
+        z = np.copy( self['dims/z'][()].T * self.lchar )
+        nx = self.nx
+        ny = self.ny
+        nz = self.nz
+        
+        ## read in 1D coordinate arrays, then dimensinoalize [m]
+        stang_ = np.copy(self['dims/stang'])
+        stang  = np.copy( stang_ * self.lchar ) ## dimensional [m]
+        data['stang'] = stang
+        
+        snorm_ = np.copy(self['dims/snorm'])
+        snorm  = np.copy( snorm_ * self.lchar ) ## dimensional [m]
+        data['snorm'] = snorm
+        
+        ## assert [z] is same over all [x,y]
+        if (z.ndim!=3):
+            raise ValueError
+        z1d = np.copy(z[0,0,:])
+        for i in range(nx):
+            for j in range(ny):
+                np.testing.assert_allclose(z1d, z[i,j,:], rtol=1e-14, atol=1e-14)
+        data['z1d'] = z1d
+        
+        ## assert [x,y] is same over all [z]
+        x2d  = np.copy(x[:,:,0])
+        y2d  = np.copy(y[:,:,0])
+        xy2d = np.stack((x2d,y2d), axis=-1)
+        for k in range(nz):
+            x2d_  = np.copy(x[:,:,k])
+            y2d_  = np.copy(y[:,:,k])
+            xy2d_ = np.stack((x2d_,y2d_), axis=-1)
+            np.testing.assert_allclose(xy2d, xy2d_, rtol=1e-14, atol=1e-14)
+        
+        ## check if constant Δz (calculate Δz+ later)
+        dz0 = np.diff(z1d)[0]
+        if not np.all(np.isclose(np.diff(z1d), dz0, rtol=1e-7)):
+            raise NotImplementedError
+        data['dz0'] = dz0
+        
+        ## dimensional [s]
+        dt = self.dt * self.tchar
+        data['dt'] = dt
+        
+        t_meas = self.duration * self.tchar
+        data['t_meas'] = t_meas
+        
+        ## check against values in 'data_dim' (imported above)
+        np.testing.assert_allclose(dt  , dt_  , rtol=1e-14, atol=1e-14)
+        np.testing.assert_allclose(dz0 , dz0_ , rtol=1e-14, atol=1e-14)
+        np.testing.assert_allclose(z1d , z1d_ , rtol=1e-14, atol=1e-14)
+        
+        zrange = z1d.max() - z1d.min()
+        data['zrange'] = zrange
+        
+        if verbose: even_print('Δt/tchar','%0.8f'%(dt/self.tchar))
+        if verbose: even_print('Δt','%0.3e [s]'%(dt,))
+        if verbose: even_print('duration/tchar','%0.1f'%(self.duration,))
+        if verbose: even_print('duration','%0.3e [s]'%(self.duration*self.tchar,))
+        if verbose: print(72*'-')
+        
+        # === report
+        if verbose:
+            #even_print('nx'     , '%i'        %nx     )
+            #even_print('ny'     , '%i'        %ny     )
+            #even_print('nz'     , '%i'        %nz     )
+            #even_print('nt'     , '%i'        %nt     )
+            #even_print('dt'     , '%0.5e [s]' %dt     )
+            #even_print('t_meas' , '%0.5e [s]' %t_meas )
+            even_print('dz0'    , '%0.5e [m]' %dz0     )
+            even_print('zrange' , '%0.5e [m]' %zrange  )
+            print(72*'-')
+        
+        if verbose:
+            even_print('Re_τ'    , '%0.1f'        % Re_tau    )
+            even_print('Re_θ'    , '%0.1f'        % Re_theta  )
+            even_print('δ99'     , '%0.5e [m]'    % d99       )
+            even_print('δ_ν=(ν_wall/u_τ)' , '%0.5e [m]' % sc_l_in )
+            even_print('U_inf'  , '%0.3f [m/s]'   % self.U_inf )
+            even_print('u_τ'    , '%0.3f [m/s]'   % u_tau     )
+            even_print('ν_wall' , '%0.5e [m²/s]'  % nu_wall   )
+            even_print('ρ_wall' , '%0.6f [kg/m³]' % rho_wall  )
+            ##
+            even_print( 'Δz+' , '%0.3f'%(dz0/sc_l_in) )
+            even_print( 'Δt+' , '%0.3f'%(dt/sc_t_in) )
+            print(72*'-')
+        
+        ## get spanwise wavenumber [kz] vector
+        kz_full = sp.fft.fftfreq(n=nz, d=dz0) * ( 2 * np.pi )
+        kzp     = np.where(kz_full>0)
+        kz      = np.copy(kz_full[kzp])
+        dkz     = kz[1]-kz[0]
+        nkz     = kz.size
+        
+        if verbose:
+            even_print('kz min','%0.1f [1/m]'%kz.min())
+            even_print('kz max','%0.1f [1/m]'%kz.max())
+            even_print('dkz','%0.1f [1/m]'%dkz)
+            even_print('nkz','%i'%nkz)
+            
+            kz_inner = np.copy( kz * sc_l_in  )
+            kz_outer = np.copy( kz * sc_l_out )
+            
+            even_print('(kz·δ_ν) min' , '%0.5e [-]'%kz_inner.min())
+            even_print('(kz·δ_ν) max' , '%0.5f [-]'%kz_inner.max())
+            even_print('(kz·δ99) min' , '%0.5f [-]'%kz_outer.min())
+            even_print('(kz·δ99) max' , '%0.5f [-]'%kz_outer.max())
+            
+            print(72*'-')
+        
+        # === read in data (prime) --> still dimless (char)
+        
+        #scalars = [ 'uI','vI','wI' , 'rho','uII','vII','wII' ]
+        scalars = [ 'uI','vI','wI', 'utangI', 'unormI' ]
+        scalars_dtypes = [self.scalars_dtypes_dict[s] for s in scalars]
+        
+        ## [var1, var2, density_scaling]
+        fft_combis = [
+                     # [ 'uI'  , 'uI'  , False ],
+                     # [ 'vI'  , 'vI'  , False ],
+                     # [ 'wI'  , 'wI'  , False ],
+                     # [ 'uI'  , 'vI'  , False ],
+                     # [ 'uII' , 'uII' , True  ],
+                     # [ 'vII' , 'vII' , True  ],
+                     # [ 'wII' , 'wII' , True  ],
+                     # [ 'uII' , 'vII' , True  ],
+                     ##
+                     [ 'utangI'  , 'utangI'  , False ],
+                     [ 'unormI'  , 'unormI'  , False ],
+                     [ 'wI'      , 'wI'      , False ],
+                     [ 'utangI'  , 'unormI'  , False ],
+                     [ 'utangI'  , 'wI'      , False ],
+                     ]
+        
+        scalars_dtypes = [ self.scalars_dtypes_dict[s] for s in scalars ]
+        
+        ## dtype of prime data (currently must be all same dtype)
+        if np.all( [ (dtp==np.float32) for dtp in scalars_dtypes ] ):
+            dtype_primes = np.float32
+        elif np.all( [ (dtp==np.float64) for dtp in scalars_dtypes ] ):
+            dtype_primes = np.float64
+        else:
+            raise NotImplementedError
+        
+        ## 5D [scalar][x,y,z,t] structured array
+        data_prime = np.zeros(shape=(self.nx, nyr, self.nz, self.nt), dtype={'names':scalars, 'formats':scalars_dtypes})
+        
+        for scalar in scalars:
+            
+            dset = self[f'data/{scalar}']
+            dtype = dset.dtype
+            float_bytes = dtype.itemsize
+            
+            self.comm.Barrier()
+            t_start = timeit.default_timer()
+            with dset.collective:
+                data_prime[scalar] = np.copy( dset[:,:,ry1:ry2,:].T )
+            self.comm.Barrier()
+            t_delta = timeit.default_timer() - t_start
+            
+            data_gb = float_bytes * self.nx * self.ny * self.nz * self.nt / 1024**3
+            
+            if verbose:
+                even_print('read: %s'%scalar, '%0.3f [GB]  %0.3f [s]  %0.3f [GB/s]'%(data_gb,t_delta,(data_gb/t_delta)))
+        
+        # === redimensionalize prime data
+        
+        for var in data_prime.dtype.names:
+            if var in ['u','v','w', 'uI','vI','wI', 'uII','vII','wII', 'utangI','unormI', 'utangII','unormII']:
+                data_prime[var] *= U_inf
+            elif var in ['r_uII','r_vII','r_wII']:
+                data_prime[var] *= (U_inf*rho_inf)
+            elif var in ['T','TI','TII']:
+                data_prime[var] *= T_inf
+            elif var in ['r_TII']:
+                data_prime[var] *= (T_inf*rho_inf)
+            elif var in ['rho','rhoI']:
+                data_prime[var] *= rho_inf
+            elif var in ['p','pI','pII']:
+                data_prime[var] *= (rho_inf * U_inf**2)
+            else:
+                raise ValueError('condition needed for redimensionalizing \'%s\''%var)
+        
+        ## force the ∫PSD == (co)variance
+        ## this usually represents about a 1-2% power correction which comes about due to 
+        ##   non-stationarity of windowed data
+        normalize_psd_by_cov = False
+        
+        ## initialize buffers
+        Euu_scalars         = [ '%s%s'%(cc[0],cc[1]) for cc in fft_combis ]
+        Euu_scalars_dtypes  = [ dtype_primes for s in Euu_scalars ]
+        Euu                 = np.zeros(shape=(self.nx, nyr, self.nt, nkz) , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes})
+        uIuI_avg            = np.zeros(shape=(self.nx, nyr, self.nt)      , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes})
+        if normalize_psd_by_cov:
+            energy_norm_fac_arr = np.zeros(shape=(self.nx, nyr, self.nt) , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes}) ## just for monitoring
+        
+        ## check memory
+        mem_total_gb = psutil.virtual_memory().total/1024**3
+        mem_avail_gb = psutil.virtual_memory().available/1024**3
+        mem_free_gb  = psutil.virtual_memory().free/1024**3
+        if verbose:
+            even_print('mem total',     '%0.1f [GB]'%(mem_total_gb,))
+            even_print('mem available', '%0.1f [GB] / %0.1f[%%]'%(mem_avail_gb,(100*mem_avail_gb/mem_total_gb)))
+            even_print('mem free',      '%0.1f [GB] / %0.1f[%%]'%(mem_free_gb,(100*mem_free_gb/mem_total_gb)))
+        
+        ## for spanwise mean, no overlapping windows are applied, so win_len = [z] vec length
+        win_len = nz
+        
+        ## the window function
+        window_type = 'tukey'
+        if (window_type=='tukey'):
+            window = sp.signal.windows.tukey(win_len, alpha=0.1)
+        elif (window_type is None):
+            window = np.ones(win_len, dtype=np.float64)
+        if verbose:
+            even_print('window type', '\'%s\''%str(window_type))
+        
+        ## sum of sqrt of window: needed for power normalization
+        sum_sqrt_win = np.sum(np.sqrt(window))
+        
+        # === main loop
+        
+        self.comm.Barrier()
+        if verbose: progress_bar = tqdm(total=self.nx*nyr*self.nt, ncols=100, desc='fft', leave=False)
+        for xi in range(self.nx):
+            for yi in range(nyr):
+                for ti in range(self.nt):
+                    for cci,cc in enumerate(fft_combis):
+                        
+                        tag = Euu_scalars[cci]
+                        ccL,ccR,density_scaling = cc
+                        
+                        uL = np.copy( data_prime[ccL][xi,yi,:,ti] )
+                        uR = np.copy( data_prime[ccR][xi,yi,:,ti] )
+                        
+                        if ('rho' in data_prime.dtype.names):
+                            rho     = np.copy( data_prime['rho'][xi,yi,:,ti] )
+                            rho_avg = np.mean( rho, dtype=np.float64 )
+                        else:
+                            rho     = None
+                            rho_avg = None
+                        
+                        # ===
+                        
+                        if density_scaling:
+                            uIuI_avg_ijk = np.mean(uL*uR*rho, dtype=np.float64) / rho_avg
+                        else:
+                            uIuI_avg_ijk = np.mean(uL*uR,     dtype=np.float64)
+                        
+                        uIuI_avg[tag][xi,yi,ti] = uIuI_avg_ijk
+                        
+                        if density_scaling:
+                            ui = np.copy( uL * rho )
+                            uj = np.copy( uR * rho )
+                        else:
+                            ui = np.copy( uL )
+                            uj = np.copy( uR )
+                        
+                        n     = ui.size
+                        #A_ui = sp.fft.fft(ui)[fp] / n
+                        #A_uj = sp.fft.fft(uj)[fp] / n
+                        ui   *= window
+                        uj   *= window
+                        #ui  -= np.mean(ui) ## de-trend
+                        #uj  -= np.mean(uj)
+                        A_ui    = sp.fft.fft(ui)[kzp] / sum_sqrt_win
+                        A_uj    = sp.fft.fft(uj)[kzp] / sum_sqrt_win
+                        Euu_ijk = 2 * np.real(A_ui*np.conj(A_uj)) / dkz
+                        
+                        ## divide off mean mass density
+                        if density_scaling:
+                            Euu_ijk /= rho_avg**2
+                        
+                        ## normalize such that ∫PSD=(co)variance
+                        if normalize_psd_by_cov:
+                            if (uIuI_avg_ijk!=0.):
+                                energy_norm_fac = np.sum(dkz*Euu_ijk) / uIuI_avg_ijk
+                            else:
+                                energy_norm_fac = 1.
+                            Euu_ijk /= energy_norm_fac
+                            energy_norm_fac_arr[tag][xi,yi,ti] = energy_norm_fac
+                        
+                        ## write
+                        Euu[tag][xi,yi,ti,:] = Euu_ijk
+                    
+                    if verbose: progress_bar.update()
+        if verbose: progress_bar.close()
+        
+        ## report energy normalization factors --> tmp,only rank 0 currently!
+        if normalize_psd_by_cov:
+            if verbose: print(72*'-')
+            for tag in Euu_scalars:
+                energy_norm_fac_min = energy_norm_fac_arr[tag].min()
+                energy_norm_fac_max = energy_norm_fac_arr[tag].max()
+                energy_norm_fac_avg = np.mean(energy_norm_fac_arr[tag], axis=(0,1,2), dtype=np.float64)
+                if verbose:
+                    even_print('energy norm min/max/avg : %s'%tag, '%0.4f / %0.4f / %0.4f'%(energy_norm_fac_min,energy_norm_fac_max,energy_norm_fac_avg))
+            energy_norm_fac_arr = None ; del energy_norm_fac_arr
+        
+        # === average in [x,t] --> leave [y,kz]
+        
+        Euu_      = np.zeros(shape=(nyr,nkz) , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes})
+        uIuI_avg_ = np.zeros(shape=(nyr,)    , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes})
+        self.comm.Barrier()
+        
+        for tag in Euu_scalars:
+            Euu_[tag]      = np.mean( Euu[tag]      , axis=(0,2) , dtype=np.float64) #.astype(np.float32) ## avg in [x,t] --> leave [y,kz]
+            uIuI_avg_[tag] = np.mean( uIuI_avg[tag] , axis=(0,2) , dtype=np.float64) #.astype(np.float32) ## avg in [x,t] --> leave [y]
+        Euu      = np.copy( Euu_ )
+        uIuI_avg = np.copy( uIuI_avg_ )
+        self.comm.Barrier()
+        
+        # === gather all results
+        # --> arrays are very small at this point, just do 'lazy' gather/bcast, dont worry about buffers etc
+        
+        G = self.comm.gather([self.rank, 
+                              Euu, uIuI_avg ], root=0)
+        G = self.comm.bcast(G, root=0)
+        
+        Euu      = np.zeros( (ny,nkz) , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes})
+        uIuI_avg = np.zeros( (ny,)    , dtype={'names':Euu_scalars, 'formats':Euu_scalars_dtypes})
+        
+        for ri in range(self.n_ranks):
+            j = ri
+            for GG in G:
+                if (GG[0]==ri):
+                    for tag in Euu_scalars:
+                        Euu[tag][ryl[j][0]:ryl[j][1],:]    = GG[1][tag]
+                        uIuI_avg[tag][ryl[j][0]:ryl[j][1]] = GG[2][tag]
+                else:
+                    pass
+        if verbose: print(72*'-')
+        
+        # === save results
+        if (self.rank==0):
+            
+            data['Euu']      = Euu
+            data['uIuI_avg'] = uIuI_avg
+            
+            with open(fn_dat_fft,'wb') as f:
+                pickle.dump(data, f, protocol=4)
+            print('--w-> %s : %0.2f [MB]'%(fn_dat_fft,os.path.getsize(fn_dat_fft)/1024**2))
+        
+        # ===
+        
+        self.comm.Barrier()
+        if verbose: print(72*'-')
+        if verbose: print('total time : cgd.calc_turb_spectrum_span_xpln() : %s'%format_time_string((timeit.default_timer() - t_start_func)))
+        if verbose: print(72*'-')
+        
+        return
+    
     # === polydata
     
     def export_polydata_wall(self, fn_spd=None, **kwargs):
         '''
         get 2D [x,z] wall quantities, export structured polydata (SPD) file
         '''
         
@@ -17691,16 +18691,14 @@
     
     # === post-processing
     
     def calc_bl_edge(self, **kwargs):
         '''
         determine the boundary layer edge location
         psvel : pseudo-velocity, i.e. [-ω_z] cumulatively integrated in wall-normal direction
-        j_max : the index of max pseudo-velocity (discrete)
-        y_max : the wall-normal coordinate corresponding to the index of discrete max pseudo-velocity
         y_edge : the wall-normal coordinate corresponding to the peak of the (interpolated) pseudo-velocity
         j_edge : the nearest index to y_edge
         '''
         
         verbose      = kwargs.get('verbose',True)
         #method       = kwargs.get('method','psvel')
         epsilon      = kwargs.get('epsilon',5e-4)
@@ -19766,18 +20764,14 @@
         if ('libver' not in kwargs):
             kwargs['libver'] = 'latest'
         
         ## catch possible user error --> could prevent accidental EAS overwrites
         if (self.fname_ext=='.eas'):
             raise ValueError('EAS4 files should not be opened with turbx.spd()')
         
-        # ## mpio driver for SPD currently not supported
-        # if ('driver' in kwargs) and (kwargs['driver']=='mpio'):
-        #     raise ValueError('SPD class is currently not set up to be used with MPI')
-        
         ## determine if using mpi
         if ('driver' in kwargs) and (kwargs['driver']=='mpio'):
             self.usingmpi = True
         else:
             self.usingmpi = False
         
         ## determine communicator & rank info
@@ -20169,35 +21163,70 @@
             self.scalars_dtypes = []
             self.scalars_dtypes_dict = dict(zip(self.scalars, self.scalars_dtypes))
         
         return
     
     def make_unstruct(self,**kwargs):
         '''
-        make unstructured datasets from structured data
+        convert structured datasets (data/<scalar>) to unstructured (data_unstruct/<scalar>)
         /dims_unstruct/quads
         /dims_unstruct/pts
         /data_unstruct/<scalar>
-        --> currently not parallel!
+        --> currently only parallelized over [t]
+        --> parallelization over [i] and [j] is probably a bit more tricky due to reshaping
         '''
+        
         verbose  = kwargs.get( 'verbose'  , True )
         indexing = kwargs.get( 'xy'       , 'xy' ) ## 'xy', 'ij'
-        chunk_kb = kwargs.get('chunk_kb'  , 16*1024 ) ## 16 [MB]
+        chunk_kb = kwargs.get( 'chunk_kb' , 16*1024 ) ## 16 [MB]
+        
+        ri = kwargs.get('ri',1) ## should be =1
+        rj = kwargs.get('rj',1) ## should be =1
+        rt = kwargs.get('rt',1)
         
         if (self.rank!=0):
             verbose=False
         else:
             verbose=True
         
         if 'dims/xyz' not in self:
             raise ValueError('dims/xyz not in file')
         
         if verbose: print('\n'+'spd.make_unstruct()'+'\n'+72*'-')
         t_start_func = timeit.default_timer()
         
+        if (ri*rj*rt != self.n_ranks):
+            raise AssertionError('ri*rj*rt != n_ranks')
+        if (ri!=1):
+            raise AssertionError('ri!=1')
+        if (rj!=1):
+            raise AssertionError('rj!=1')
+        #if (rt>self.nt):
+        #    raise AssertionError('rt>self.nt')
+        
+        #if verbose: even_print('ri','%i'%ri)
+        #if verbose: even_print('rj','%i'%rj)
+        if verbose: even_print('rt','%i'%rt)
+        #if verbose: print(72*'-')
+        
+        # ===
+        
+        rtl_ = np.array_split(np.arange(self.nt,dtype=np.int64),min(rt,self.nt))
+        rtl = [[b[0],b[-1]+1] for b in rtl_ ]
+        
+        ## if rt>nt, assign null range
+        try:
+            rt1,rt2 = rtl[self.rank]
+        except IndexError:
+            rt1,rt2 = 0,0
+        ntr = rt2 - rt1
+        
+        # ===
+        
+        ## every rank gets grid
         xyz = np.copy( self['dims/xyz'][()] )
         if verbose:
             even_print('dims/xyz',str(xyz.shape))
         
         if (xyz.ndim!=3):
             raise ValueError('xyz.ndim!=3')
         
@@ -20250,52 +21279,118 @@
         if (indexing=='xy'):
             order='C'
         elif (indexing=='ij'):
             order = 'F'
         else:
             raise ValueError
         
+        # ===
+        
         ## flatten quad index vector
         quads = np.reshape(quads, ((ni-1)*(nj-1),4), order=order)
         
         dsn = 'dims_unstruct/quads'
         if (dsn in self):
             del self[dsn]
-        ds = self.create_dataset(dsn, data=quads, chunks=True)
+        
+        shape = quads.shape
+        dtype = quads.dtype
+        itemsize = quads.dtype.itemsize
+        chunks = rgd.chunk_sizer(nxi=shape, constraint=(None,None), size_kb=chunk_kb, base=2, data_byte=itemsize)
+        ds = self.create_dataset(dsn,
+                                 shape=shape,
+                                 chunks=chunks,
+                                 dtype=dtype )
+        
+        chunk_kb_ = np.prod(ds.chunks)*itemsize / 1024. ## actual
+        if verbose:
+            even_print('chunk shape (n_quads,4)','%s'%str(ds.chunks))
+            even_print('chunk size','%i [KB]'%int(round(chunk_kb_)))
+        
         if verbose: even_print(dsn,'%s'%str(ds.shape))
         
+        if self.usingmpi:
+            with ds.collective:
+                ds[:,:] = quads
+        else:
+            ds[:,:] = quads
+        
+        # ===
+        
         ## flatten point coordinate vector
         pts = np.reshape(xyz, (ni*nj,3), order=order)
         
         dsn = 'dims_unstruct/pts'
         if (dsn in self):
             del self[dsn]
-        ds = self.create_dataset(dsn, data=pts, chunks=True)
+        
+        shape = pts.shape
+        dtype = pts.dtype
+        itemsize = pts.dtype.itemsize
+        chunks = rgd.chunk_sizer(nxi=shape, constraint=(None,None), size_kb=chunk_kb, base=2, data_byte=itemsize)
+        ds = self.create_dataset(dsn,
+                                 shape=shape,
+                                 chunks=chunks,
+                                 dtype=dtype )
+        
+        chunk_kb_ = np.prod(ds.chunks)*itemsize / 1024. ## actual
+        if verbose:
+            even_print('chunk shape (n_pts,3)','%s'%str(ds.chunks))
+            even_print('chunk size','%i [KB]'%int(round(chunk_kb_)))
+        
         if verbose: even_print(dsn,'%s'%str(ds.shape))
         
-        ## initialize data_unstruct/<scalar> datasets
-        shape = (ni*nj,nt)
-        chunks = rgd.chunk_sizer(nxi=shape, constraint=(None,1), size_kb=chunk_kb, base=2, data_byte=4)
+        if self.usingmpi:
+            with ds.collective:
+                ds[:,:] = pts
+        else:
+            ds[:,:] = pts
+        
+        # ===
         
+        ## initialize all data_unstruct/<scalar> datasets
         for scalar in self.scalars:
+            
+            dsn = f'data/{scalar}'
+            dtype = self[dsn].dtype
+            itemsize = pts.dtype.itemsize
+            
+            ## initialize data_unstruct/<scalar> datasets
+            shape = (ni*nj,nt)
+            chunks = rgd.chunk_sizer(nxi=shape, constraint=(None,1), size_kb=chunk_kb, base=2, data_byte=itemsize)
+            
             dsn = f'data_unstruct/{scalar}'
             if (dsn in self):
                 del self[dsn]
-            ds = self.create_dataset(dsn, shape=shape, chunks=chunks)
+            
+            ds = self.create_dataset(dsn,
+                                     shape=shape,
+                                     chunks=chunks,
+                                     dtype=dtype,
+                                     )
+            
+            # chunk_kb_ = np.prod(ds.chunks)*itemsize / 1024. ## actual
+            # if verbose:
+            #     even_print('chunk shape (n_pts,3)','%s'%str(ds.chunks))
+            #     even_print('chunk size','%i [KB]'%int(round(chunk_kb_)))
+            
             if verbose: even_print(dsn,'%s'%str(ds.shape))
         
+        # ===
+        
         ## copy scalar data, reshape, write
-        if verbose: progress_bar = tqdm(total=self.n_scalars*self.nt, ncols=100, desc='reshape', leave=False, file=sys.stdout)
+        if verbose: progress_bar = tqdm(total=self.n_scalars*ntr, ncols=100, desc='reshape', leave=False, file=sys.stdout)
         for scalar in self.scalars:
             
             dsn = f'data_unstruct/{scalar}'
             ds = self[dsn]
             #if verbose: even_print(dsn,str(ds.shape))
             
-            for ti in range(nt):
+            #for ti in range(nt):
+            for ti in range(rt1,rt2):
                 
                 ## get structured scalar data
                 data = np.copy( self[f'data/{scalar}'][:,:,ti] )
                 #_,_,one = data.shape
                 
                 ## reshape / flatten scalar data
                 #data = np.reshape(data, (ni*nj,nt), order=order)
@@ -20642,20 +21737,14 @@
         dsn = 'dims_unstruct/quads'
         n_quads,four = self[dsn].shape
         dsn = 'dims_unstruct/pts'
         n_pts,three = self[dsn].shape
         self.n_quads = n_quads
         self.n_pts   = n_pts
         
-        # ## TMP TMP TMP TMP TMP TMP
-        # if not hasattr(self,'t'):
-        #     dsn = 'data/tau'
-        #     _,_,nt = self[dsn].shape
-        #     self.t = np.arange(nt,dtype=np.float64)
-        
         if verbose: print('\n'+'spd.make_xdmf()'+'\n'+72*'-')
         
         dataset_precision_dict = {} ## holds dtype.itemsize ints i.e. 4,8
         dataset_numbertype_dict = {} ## holds string description of dtypes i.e. 'Float','Integer'
         
         # === 1D coordinate dimension vectors --> get dtype.name
         for dsn_unstruct in ['pts','quads']:
@@ -21583,14 +22672,224 @@
         even_print('uchar'          , '%0.5f [m/s]'         % self.uchar      )
         even_print('lchar'          , '%0.5e [m]'           % self.lchar      )
         even_print('tchar'          , '%0.5e [s]'           % self.tchar      )
         print(72*'-')
         
         return
 
+def calc_bl_edge_1d(y, psvel, **kwargs):
+    '''
+    determine the boundary layer edge location of 1D profile
+    '''
+    verbose      = kwargs.get('verbose',True)
+    #method       = kwargs.get('method','psvel')
+    epsilon      = kwargs.get('epsilon',5e-4)
+    acc          = kwargs.get('acc',8)
+    edge_stencil = kwargs.get('edge_stencil','half')
+    
+    ynorm = kwargs.get('ynorm',1.) ## normalization factor... usually lchar
+    
+    if (y.ndim!=1):
+        raise ValueError
+    if (psvel.ndim!=1):
+        raise ValueError
+    if (psvel.shape[0]!=y.shape[0]):
+        raise ValueError
+    
+    ny = y.shape[0]
+    psvel_max = psvel.max()
+    
+    ddy_psvel_normed = gradient( psvel/psvel_max, y/ynorm, axis=0, d=1, acc=acc, edge_stencil=edge_stencil )
+    #ddy_psvel_normed = gradient( psvel, y/ynorm, axis=0, d=1, acc=acc, edge_stencil=edge_stencil )
+    
+    ## debug plot
+    # plt.close('all')
+    # fig1 = plt.figure(figsize=(3,3), dpi=300)
+    # ax1 = plt.gca()
+    # ax1.plot(  ddy_psvel_normed, y/ynorm, lw=0.5 )
+    # ax1.axvline(x=epsilon, linestyle='dashed', c='lightgray', zorder=1, lw=0.3)
+    # fig1.tight_layout(pad=0.25)
+    # fig1.tight_layout(pad=0.25)
+    # plt.show()
+    
+    ## get [y] of first intersection
+    jtop = ny-1
+    for j in range(ny):
+        if ( ddy_psvel_normed[j] < epsilon):
+            jtop = j
+            break
+    
+    intrp_func = sp.interpolate.interp1d(y/ynorm, ddy_psvel_normed, kind='linear', bounds_error=True)
+    
+    def __f_opt1(y_test, intrp_func, epsilon, ynorm):
+        ddy_psvel_test = intrp_func(y_test/ynorm)
+        root = np.abs( ddy_psvel_test - epsilon )
+        return root
+    
+    sol = sp.optimize.least_squares(fun=__f_opt1,
+                                    args=(intrp_func, epsilon, ynorm),
+                                    x0=0.5*(y[jtop-2]+y[jtop]),
+                                    xtol=1e-14,
+                                    #ftol=1e-15,
+                                    method='dogbox',
+                                    bounds=(y[jtop-2], y[jtop]))
+    if not sol.success:
+        raise ValueError
+    
+    y_edge = sol.x[0]
+    
+    return y_edge
+
+def calc_d99_1d(y, psvel, y_edge, psvel_edge, **kwargs):
+    '''
+    calculate [δ99] of 1D profile
+    '''
+    
+    if (y.ndim!=1):
+        raise ValueError
+    if (psvel.ndim!=1):
+        raise ValueError
+    if (psvel.shape[0]!=y.shape[0]):
+        raise ValueError
+    if not isinstance(y_edge, (float,)):
+        raise ValueError
+    if not isinstance(psvel_edge, (float,)):
+        raise ValueError
+    
+    if (y_edge>y.max()):
+        raise ValueError
+    if (y_edge<y.min()):
+        raise ValueError
+    
+    ny = y.shape[0]
+    
+    j_edge = np.abs(y-y_edge).argmin()
+    y_edge_g = y[j_edge]
+    
+    je = j_edge + 2
+    #je = min( j_edge + 2, ny+1 )
+    
+    intrp_func = sp.interpolate.interp1d(y[:je], psvel[:je], kind='cubic', bounds_error=True)
+    
+    ## check that [psvel_edge] is correct
+    psvel_edge_ = intrp_func(y_edge)
+    np.testing.assert_allclose(psvel_edge, psvel_edge_, rtol=1e-7)
+    
+    def __f_opt(y_test, intrp_func, psvel_edge):
+        root = np.abs( 0.99*psvel_edge - intrp_func(y_test) )
+        return root
+    
+    sol = sp.optimize.least_squares(fun=__f_opt,
+                                    args=(intrp_func,psvel_edge),
+                                    #args=(intrp_func,u_edge_),
+                                    x0=0.99*y_edge,
+                                    xtol=1e-14,
+                                    #ftol=1e-14,
+                                    method='dogbox',
+                                    bounds=(y.min(), y_edge))
+    if not sol.success:
+        raise ValueError
+    
+    d99 = sol.x[0]
+    
+    return d99
+
+def calc_bl_integral_quantities_1d( y, u, rho, u_tau, d99, y_edge, rho_edge, nu_edge, u_edge, nu_wall, **kwargs):
+    '''
+    for 1D profile get [θ, δ*, Re_θ, Re_τ]
+    '''
+    
+    if (y.ndim!=1):
+        raise ValueError
+    
+    if (u.ndim!=1):
+        raise ValueError
+    if (u.shape[0]!=y.shape[0]):
+        raise ValueError
+    if (rho.ndim!=1):
+        raise ValueError
+    if (rho.shape[0]!=y.shape[0]):
+        raise ValueError
+    
+    if not isinstance(u_tau, (float,)):
+        raise ValueError
+    if not isinstance(d99, (float,)):
+        raise ValueError
+    if not isinstance(y_edge, (float,)):
+        raise ValueError
+    if not isinstance(rho_edge, (float,)):
+        raise ValueError
+    if not isinstance(nu_edge, (float,)):
+        raise ValueError
+    if not isinstance(u_edge, (float,)):
+        raise ValueError
+    if not isinstance(nu_wall, (float,)):
+        raise ValueError
+    
+    if (y_edge>y.max()):
+        raise ValueError
+    if (y_edge<y.min()):
+        raise ValueError
+    
+    ny = y.shape[0]
+    
+    rho_edge_ = sp.interpolate.interp1d(y, rho, kind='cubic', bounds_error=True)(y_edge)
+    np.testing.assert_allclose(rho_edge, rho_edge_, rtol=1e-7)
+    
+    u_edge_ = sp.interpolate.interp1d(y, u, kind='cubic', bounds_error=True)(y_edge)
+    np.testing.assert_allclose(u_edge, u_edge_, rtol=1e-7)
+    
+    # ===
+    
+    integrand_theta_cmp = (u*rho)/(u_edge*rho_edge)*(1-(u/u_edge))
+    integrand_dstar_cmp = (1-((u*rho)/(u_edge*rho_edge)))
+    
+    theta_cmp_     = sp.integrate.cumulative_trapezoid(y=integrand_theta_cmp, x=y, initial=0.)
+    theta_cmp_func = sp.interpolate.interp1d(y, theta_cmp_, kind='cubic')
+    theta_cmp      = theta_cmp_func(y_edge)
+    
+    dstar_cmp_     = sp.integrate.cumulative_trapezoid(y=integrand_dstar_cmp, x=y, initial=0.)
+    dstar_cmp_func = sp.interpolate.interp1d(y, dstar_cmp_, kind='cubic')
+    dstar_cmp      = dstar_cmp_func(y_edge)
+    
+    integrand_theta_inc = (u/u_edge)*(1-(u/u_edge))
+    integrand_dstar_inc = 1-(u/u_edge)
+    
+    theta_inc_     = sp.integrate.cumulative_trapezoid(y=integrand_theta_inc, x=y, initial=0.)
+    theta_inc_func = sp.interpolate.interp1d(y, theta_inc_, kind='cubic')
+    theta_inc      = theta_inc_func(y_edge)
+    
+    dstar_inc_     = sp.integrate.cumulative_trapezoid(y=integrand_dstar_inc, x=y, initial=0.)
+    dstar_inc_func = sp.interpolate.interp1d(y, dstar_inc_, kind='cubic')
+    dstar_inc      = dstar_inc_func(y_edge)
+    
+    # ===
+    
+    H12     = dstar_cmp/theta_cmp
+    H12_inc = dstar_inc/theta_inc
+    
+    Re_tau       = d99*u_tau/nu_wall
+    Re_theta     = theta_cmp*u_edge/nu_edge
+    Re_theta_inc = theta_inc*u_edge/nu_edge
+    Re_d99       = d99*u_edge/nu_edge
+    
+    dd = { 'theta_cmp':theta_cmp,
+           'dstar_cmp':dstar_cmp,
+           'theta_inc':theta_inc,
+           'dstar_inc':dstar_inc,
+           'H12':H12,
+           'H12_inc':H12_inc,
+           'Re_tau':Re_tau,
+           'Re_theta':Re_theta,
+           'Re_theta_inc':Re_theta_inc,
+           'Re_d99':Re_d99,
+         }
+    
+    return dd
+
 # numerical & grid
 # ======================================================================
 
 def interp_2d_structured(x2d_A, y2d_A, x2d_B, y2d_B, data_A, **kwargs):
     '''
     interpolate 2D array 'data_A' from grid A onto grid B, yielding 'data_B'
     --> based on sp.interpolate.griddata()
@@ -22242,14 +23541,15 @@
     compute the grid metric tensor (inverse of grid Jacobian) for a 2D grid
     -----
     Computational Fluid Mechanics and Heat Transfer (2012) Pletcher, Tannehill, Anderson
     p.266-270, 335-337, 652
     '''
     
     verbose = kwargs.get('verbose',False)
+    no_warn = kwargs.get('no_warn',False)
     
     if not isinstance(x2d, np.ndarray):
         raise ValueError('x2d should be of type np.ndarray')
     if not isinstance(y2d, np.ndarray):
         raise ValueError('y2d should be of type np.ndarray')
     
     if (x2d.ndim!=2):
@@ -22269,18 +23569,18 @@
     x_comp = 1.
     y_comp = 1.
     
     # === get Jacobian :: ∂(x,y)/∂(q1,q2)
     
     t_start = timeit.default_timer()
     
-    dxdx = gradient(x2d, x_comp, axis=0, d=1, acc=acc, edge_stencil=edge_stencil)
-    dydx = gradient(y2d, x_comp, axis=0, d=1, acc=acc, edge_stencil=edge_stencil)
-    dxdy = gradient(x2d, y_comp, axis=1, d=1, acc=acc, edge_stencil=edge_stencil)
-    dydy = gradient(y2d, y_comp, axis=1, d=1, acc=acc, edge_stencil=edge_stencil)
+    dxdx = gradient(x2d, x_comp, axis=0, d=1, acc=acc, edge_stencil=edge_stencil, no_warn=no_warn)
+    dydx = gradient(y2d, x_comp, axis=0, d=1, acc=acc, edge_stencil=edge_stencil, no_warn=no_warn)
+    dxdy = gradient(x2d, y_comp, axis=1, d=1, acc=acc, edge_stencil=edge_stencil, no_warn=no_warn)
+    dydy = gradient(y2d, y_comp, axis=1, d=1, acc=acc, edge_stencil=edge_stencil, no_warn=no_warn)
     
     J = np.stack((np.stack((dxdx, dydx), axis=2),
                   np.stack((dxdy, dydy), axis=2)), axis=3)
     
     t_delta = timeit.default_timer() - t_start
     if verbose: tqdm.write( even_print('get J','%0.3f [s]'%(t_delta,), s=True) )
     
@@ -24053,8 +25353,8 @@
     print('--w-> %s'%fname)
     return
 
 # main()
 # ======================================================================
 
 if __name__ == '__main__':
-    pass
+    pass
```

### Comparing `turbx-0.2.1/turbx.egg-info/PKG-INFO` & `turbx-0.2.2/turbx.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbx
-Version: 0.2.1
+Version: 0.2.2
 Summary: Extensible toolkit for analyzing turbulent flow datasets
 Home-page: https://github.com/iagappel/turbx
 Author: Jason A
 Maintainer: Jason A
 License: MIT
 Keywords: scientific computing,statistics,simulation,turbulence,turbulent flows,direct numerical simulation,DNS,parallel,visualization
 Platform: any
@@ -29,15 +29,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # turbx
 [![PyPI version](https://badge.fury.io/py/turbx.svg)](https://badge.fury.io/py/turbx)
 [![Downloads](https://pepy.tech/badge/turbx)](https://pepy.tech/project/turbx)
 
-Tools for analysis of turbulent flow datasets.
+Extensible toolkit for analyzing turbulent flow datasets.
 
 Install with `pip`:
 
 ```
 pip install --upgrade --user turbx
 ```
```

