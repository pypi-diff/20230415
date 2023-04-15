# Comparing `tmp/gerabaldi-0.1.0.tar.gz` & `tmp/gerabaldi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gerabaldi-0.1.0.tar", last modified: Thu Apr  6 20:37:00 2023, max compression
+gzip compressed data, was "gerabaldi-0.1.2.tar", last modified: Sat Apr 15 02:52:36 2023, max compression
```

## Comparing `gerabaldi-0.1.0.tar` & `gerabaldi-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 20:37:00.895627 gerabaldi-0.1.0/
--rw-rw-rw-   0        0        0    11543 2023-01-29 20:03:58.000000 gerabaldi-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     5683 2023-04-06 20:37:00.895111 gerabaldi-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4986 2023-04-06 19:55:40.000000 gerabaldi-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 20:37:00.877243 gerabaldi-0.1.0/gerabaldi/
--rw-rw-rw-   0        0        0     3188 2023-04-06 20:36:27.000000 gerabaldi-0.1.0/gerabaldi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 20:37:00.886331 gerabaldi-0.1.0/gerabaldi/cookbook/
--rw-rw-rw-   0        0        0      497 2023-04-06 19:55:40.000000 gerabaldi-0.1.0/gerabaldi/cookbook/__init__.py
--rw-rw-rw-   0        0        0     1383 2023-04-06 19:55:40.000000 gerabaldi-0.1.0/gerabaldi/cookbook/mech_mdls.py
--rw-rw-rw-   0        0        0     2273 2023-04-06 19:55:40.000000 gerabaldi-0.1.0/gerabaldi/cookbook/test_envs.py
--rw-rw-rw-   0        0        0     2843 2023-04-06 19:55:40.000000 gerabaldi-0.1.0/gerabaldi/cookbook/test_specs.py
--rw-rw-rw-   0        0        0     1375 2023-04-06 19:55:40.000000 gerabaldi-0.1.0/gerabaldi/exceptions.py
--rw-rw-rw-   0        0        0     3148 2023-04-06 19:55:40.000000 gerabaldi-0.1.0/gerabaldi/helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-06 20:37:00.893590 gerabaldi-0.1.0/gerabaldi/models/
--rw-rw-rw-   0        0        0      576 2023-04-06 19:55:40.000000 gerabaldi-0.1.0/gerabaldi/models/__init__.py
--rw-rw-rw-   0        0        0    58182 2023-04-06 19:55:40.000000 gerabaldi-0.1.0/gerabaldi/models/devices.py
--rw-rw-rw-   0        0        0    21521 2023-04-06 19:55:40.000000 gerabaldi-0.1.0/gerabaldi/models/phys_envs.py
--rw-rw-rw-   0        0        0    10795 2023-04-06 19:55:40.000000 gerabaldi-0.1.0/gerabaldi/models/random_vars.py
--rw-rw-rw-   0        0        0     9767 2023-04-06 19:55:40.000000 gerabaldi-0.1.0/gerabaldi/models/reports.py
--rw-rw-rw-   0        0        0     2348 2023-04-06 19:55:40.000000 gerabaldi-0.1.0/gerabaldi/models/states.py
--rw-rw-rw-   0        0        0     9993 2023-04-06 19:55:40.000000 gerabaldi-0.1.0/gerabaldi/models/test_specs.py
--rw-rw-rw-   0        0        0    10292 2023-04-06 19:55:40.000000 gerabaldi-0.1.0/gerabaldi/sim.py
-drwxrwxrwx   0        0        0        0 2023-04-06 20:37:00.882957 gerabaldi-0.1.0/gerabaldi.egg-info/
--rw-rw-rw-   0        0        0     5683 2023-04-06 20:37:00.000000 gerabaldi-0.1.0/gerabaldi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      630 2023-04-06 20:37:00.000000 gerabaldi-0.1.0/gerabaldi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 20:37:00.000000 gerabaldi-0.1.0/gerabaldi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-06 20:37:00.000000 gerabaldi-0.1.0/gerabaldi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-06 20:37:00.000000 gerabaldi-0.1.0/gerabaldi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      998 2023-04-06 20:25:07.000000 gerabaldi-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       50 2023-01-29 20:03:58.000000 gerabaldi-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 20:37:00.895627 gerabaldi-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-15 02:52:36.158421 gerabaldi-0.1.2/
+-rw-rw-rw-   0        0        0    11543 2023-01-29 20:03:58.000000 gerabaldi-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     5800 2023-04-15 02:52:36.158421 gerabaldi-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5104 2023-04-14 01:33:06.000000 gerabaldi-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 02:52:36.120621 gerabaldi-0.1.2/gerabaldi/
+-rw-rw-rw-   0        0        0     3188 2023-04-12 21:48:17.000000 gerabaldi-0.1.2/gerabaldi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 02:52:36.147183 gerabaldi-0.1.2/gerabaldi/cookbook/
+-rw-rw-rw-   0        0        0      497 2023-04-06 19:55:40.000000 gerabaldi-0.1.2/gerabaldi/cookbook/__init__.py
+-rw-rw-rw-   0        0        0     1383 2023-04-06 19:55:40.000000 gerabaldi-0.1.2/gerabaldi/cookbook/mech_mdls.py
+-rw-rw-rw-   0        0        0     2268 2023-04-12 21:49:48.000000 gerabaldi-0.1.2/gerabaldi/cookbook/test_envs.py
+-rw-rw-rw-   0        0        0     3614 2023-04-15 01:38:14.000000 gerabaldi-0.1.2/gerabaldi/cookbook/test_specs.py
+-rw-rw-rw-   0        0        0     1375 2023-04-06 19:55:40.000000 gerabaldi-0.1.2/gerabaldi/exceptions.py
+-rw-rw-rw-   0        0        0     3148 2023-04-06 19:55:40.000000 gerabaldi-0.1.2/gerabaldi/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-15 02:52:36.157391 gerabaldi-0.1.2/gerabaldi/models/
+-rw-rw-rw-   0        0        0      576 2023-04-06 19:55:40.000000 gerabaldi-0.1.2/gerabaldi/models/__init__.py
+-rw-rw-rw-   0        0        0    58316 2023-04-13 01:06:48.000000 gerabaldi-0.1.2/gerabaldi/models/devices.py
+-rw-rw-rw-   0        0        0    21559 2023-04-12 21:46:15.000000 gerabaldi-0.1.2/gerabaldi/models/phys_envs.py
+-rw-rw-rw-   0        0        0    10804 2023-04-12 21:47:29.000000 gerabaldi-0.1.2/gerabaldi/models/random_vars.py
+-rw-rw-rw-   0        0        0     9989 2023-04-14 01:53:22.000000 gerabaldi-0.1.2/gerabaldi/models/reports.py
+-rw-rw-rw-   0        0        0     2386 2023-04-12 21:48:55.000000 gerabaldi-0.1.2/gerabaldi/models/states.py
+-rw-rw-rw-   0        0        0    10031 2023-04-12 21:49:05.000000 gerabaldi-0.1.2/gerabaldi/models/test_specs.py
+-rw-rw-rw-   0        0        0    11427 2023-04-14 01:43:14.000000 gerabaldi-0.1.2/gerabaldi/sim.py
+drwxrwxrwx   0        0        0        0 2023-04-15 02:52:36.133396 gerabaldi-0.1.2/gerabaldi.egg-info/
+-rw-rw-rw-   0        0        0     5800 2023-04-15 02:52:36.000000 gerabaldi-0.1.2/gerabaldi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      630 2023-04-15 02:52:36.000000 gerabaldi-0.1.2/gerabaldi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 02:52:36.000000 gerabaldi-0.1.2/gerabaldi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-15 02:52:36.000000 gerabaldi-0.1.2/gerabaldi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-15 02:52:36.000000 gerabaldi-0.1.2/gerabaldi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      997 2023-04-12 21:47:46.000000 gerabaldi-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       50 2023-01-29 20:03:58.000000 gerabaldi-0.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 02:52:36.158933 gerabaldi-0.1.2/setup.cfg
```

### Comparing `gerabaldi-0.1.0/LICENSE` & `gerabaldi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gerabaldi-0.1.0/PKG-INFO` & `gerabaldi-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: gerabaldi
-Version: 0.1.0
-Summary: A temporal simulator for probabilistic degradation and failure processes with a focus on integrated circuit wear-out 
-Author-email: Ian Hill <ianrmhill@gmail.com>
-Project-URL: Homepage, https://github.com/ianrmhill/gerabaldi
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Intended Audience :: Science/Research
-Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Gerabaldi Wear-Out Reliability Simulator / Generative Aging Model
 
 The Gerabaldi module allows for generic simulation of arbitrary integrated circuit reliability tests, enabling data
 generation for tests or use cases where obtaining the corresponding real-world data could require hundreds of hours or
 even years to obtain. Results realism is of course governed by the quality of the physical model used to simulate some
 real-world hardware device, as with any generative model.
 
@@ -43,26 +27,27 @@
 ## Demos
 
 The 'demos' folder of this repository contains some useful references for full working simulations with command-line
 interfaces and visualization of results. These can be run directly if you have cloned the source code, or if you
 installed the packaged version it is easiest to copy-paste the source code from Github (you will want to remove the
 automated path add code at the very top of the demo file as the 'gerabaldi' import should already work without it).
 
-Note that the VTS paper demos will take a significant amount of time to run due to the size of the simulations, these
-can be reduced by changing the three globals near the tops of the files as follows:
-
-For demo 1:
-`NUM_SAMPLES = 5`
-`NUM_DEVICES = 5`
-`NUM_LOTS = 5`
-
-For demo 2:
-`TEST_LEN = 24 * 7 * 52 * 2`
-`NUM_SAMPLES = 100`
-`C_LATENT = 4e-5`
+Note that the VTS paper demos will require modification and take a significant amount of time to obtain the exact
+results shown due to the size of the simulations, to run the full simulations change the three globals near the tops of
+the files as follows:
+
+For demo 1 (pre-silicon variability analysis):
+`NUM_DEVICES = 10`
+`NUM_CHIPS = 10`
+`NUM_LOTS = 10`
+
+For demo 2 (TDDB model sensitivity):
+`TEST_LEN = 24 * 7 * 52 * 20`
+`NUM_SAMPLES = 1000`
+`C_LATENT = 4e-6`
 
 Running the simulations with these values will provide similar-looking results but with far less computation and is
 useful for quickly seeing these more complex simulations in action.
 
 
 ## Basic Use
```

### Comparing `gerabaldi-0.1.0/README.md` & `gerabaldi-0.1.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: gerabaldi
+Version: 0.1.2
+Summary: A temporal simulator for probabilistic degradation and failure processes with a focus on integrated circuit wear-out 
+Author-email: Ian Hill <ianrmhill@gmail.com>
+Project-URL: Homepage, https://github.com/ianrmhill/gerabaldi
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Intended Audience :: Science/Research
+Classifier: Development Status :: 3 - Alpha
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Gerabaldi Wear-Out Reliability Simulator / Generative Aging Model
 
 The Gerabaldi module allows for generic simulation of arbitrary integrated circuit reliability tests, enabling data
 generation for tests or use cases where obtaining the corresponding real-world data could require hundreds of hours or
 even years to obtain. Results realism is of course governed by the quality of the physical model used to simulate some
 real-world hardware device, as with any generative model.
 
@@ -27,26 +43,27 @@
 ## Demos
 
 The 'demos' folder of this repository contains some useful references for full working simulations with command-line
 interfaces and visualization of results. These can be run directly if you have cloned the source code, or if you
 installed the packaged version it is easiest to copy-paste the source code from Github (you will want to remove the
 automated path add code at the very top of the demo file as the 'gerabaldi' import should already work without it).
 
-Note that the VTS paper demos will take a significant amount of time to run due to the size of the simulations, these
-can be reduced by changing the three globals near the tops of the files as follows:
-
-For demo 1:
-`NUM_SAMPLES = 5`
-`NUM_DEVICES = 5`
-`NUM_LOTS = 5`
-
-For demo 2:
-`TEST_LEN = 24 * 7 * 52 * 2`
-`NUM_SAMPLES = 100`
-`C_LATENT = 4e-5`
+Note that the VTS paper demos will require modification and take a significant amount of time to obtain the exact
+results shown due to the size of the simulations, to run the full simulations change the three globals near the tops of
+the files as follows:
+
+For demo 1 (pre-silicon variability analysis):
+`NUM_DEVICES = 10`
+`NUM_CHIPS = 10`
+`NUM_LOTS = 10`
+
+For demo 2 (TDDB model sensitivity):
+`TEST_LEN = 24 * 7 * 52 * 20`
+`NUM_SAMPLES = 1000`
+`C_LATENT = 4e-6`
 
 Running the simulations with these values will provide similar-looking results but with far less computation and is
 useful for quickly seeing these more complex simulations in action.
 
 
 ## Basic Use
```

### Comparing `gerabaldi-0.1.0/gerabaldi/__init__.py` & `gerabaldi-0.1.2/gerabaldi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 TestSpec - Class that is instantiated to define the test specification model
 PhysTestEnv - Class that is instantiated to define the physical test environment model
 DeviceMdl - Class that is instantiated to define a physical device/hardware model
 simulate - The main procedure for the module, uses the above three models to run a wear-out simulation and return data
 """
 
 # This value determines the project version for PyPi as well
-__version__ = '0.1.0'
+__version__ = '0.1.2'
 
 from . import models
 from . import cookbook
 from .sim import simulate, gen_init_state
 
 __all__ = ['simulate', 'gen_init_state', 'models', 'cookbook']
 __all__.extend(models.__all__)
```

### Comparing `gerabaldi-0.1.0/gerabaldi/cookbook/mech_mdls.py` & `gerabaldi-0.1.2/gerabaldi/cookbook/mech_mdls.py`

 * *Files identical despite different names*

### Comparing `gerabaldi-0.1.0/gerabaldi/cookbook/test_envs.py` & `gerabaldi-0.1.2/gerabaldi/cookbook/test_envs.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,13 +35,13 @@
                             vrtn_type='offset', name='Voltage Variation Model')
     # Temperature varies little between devices, 0.2 degree shifts between chips and overall 0.5 test chamber error
     temp_vrtns = EnvVrtnMdl(dev_vrtn_mdl=Normal(0, 0.05), chp_vrtn_mdl=Normal(0, 0.2), batch_vrtn_mdl=Normal(0, 0.5),
                             vrtn_type='offset', name='Temperature Variation Model')
 
     # Voltmeter shows to nearest mV, noise error offsets of 0.2mV, range of 0V to 12V
     volt_meas = MeasInstrument(precision=3, error=Normal(0, 0.0002), meas_lims=(0, 12), name='Basic Voltmeter')
-    # Temperature shows to nearest hundreths of a degree, error offset of 0.2K and converts to Celsius, range -40 to 180
+    # Temperature to nearest hundredths of a degree, error offset of 0.2K and converts to Celsius, range -40 to 180
     temp_meas = MeasInstrument(precision=2, error=Normal(-273.15, 0.2), meas_lims=(-40, 180), name='Basic Temp Sensor')
 
     return PhysTestEnv(env_vrtns={'temp': temp_vrtns, 'vdd': volt_vrtns},
                        meas_instms={'temp': temp_meas, 'vdd': volt_meas},
                        env_name='Stochastic Voltage and Temperature Affected Test Environment')
```

### Comparing `gerabaldi-0.1.0/gerabaldi/exceptions.py` & `gerabaldi-0.1.2/gerabaldi/exceptions.py`

 * *Files identical despite different names*

### Comparing `gerabaldi-0.1.0/gerabaldi/helpers.py` & `gerabaldi-0.1.2/gerabaldi/helpers.py`

 * *Files identical despite different names*

### Comparing `gerabaldi-0.1.0/gerabaldi/models/__init__.py` & `gerabaldi-0.1.2/gerabaldi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gerabaldi-0.1.0/gerabaldi/models/devices.py` & `gerabaldi-0.1.2/gerabaldi/models/devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Copyright (c) 2023 Ian Hill
 # SPDX-License-Identifier: Apache-2.0
 
 """Classes for defining degradation models for tuning or use in simulating wear-out tests"""
 
+from __future__ import annotations
+
 import inspect
 import numpy as np
 from scipy.optimize import minimize_scalar
 from typing import Callable
 
 from gerabaldi.models.random_vars import RandomVar, Deterministic
 from gerabaldi.models.states import TestSimState
@@ -88,25 +90,26 @@
         if not dev_vrtn_mdl and deter_val is None:
             raise UserConfigError(f"Latent {self.name} definition must include either a device distribution or"
                                   "deterministic value argument.")
 
     def __setattr__(self, name, value):
         if name == 'name':
             # Need to also update the naming of the probabilistic distributions to have CBI export work correctly
-            if self._dev_vrtns and not self.dev_vrtn_mdl.name:
-                # Set the distribution name to be the variable name + '_dev' suffix, unless the device variation model
-                # fully specifies the variable value, in which case don't add the suffix
-                if not self._chp_vrtns and not self._lot_vrtns and not self._dev_vrtns:
-                    self.dev_vrtn_mdl.name = name
-                else:
-                    self.dev_vrtn_mdl.name = name + '_dev'
-            if self._chp_vrtns:
-                self.chp_vrtn_mdl.name = name + '_chp'
-            if self._chp_vrtns:
-                self.lot_vrtn_mdl.name = name + '_lot'
+            if value is not None:
+                if self._dev_vrtns:
+                    # Set the distribution name to be the variable name + '_dev' suffix, unless the device variation
+                    # model fully specifies the variable value, in which case don't add the suffix
+                    if not self._chp_vrtns and not self._lot_vrtns:
+                        self.dev_vrtn_mdl.name = value
+                    else:
+                        self.dev_vrtn_mdl.name = value + '_dev'
+                if self._chp_vrtns:
+                    self.chp_vrtn_mdl.name = value + '_chp'
+                if self._lot_vrtns:
+                    self.lot_vrtn_mdl.name = value + '_lot'
         if name == 'vrtn_type':
             # If changing the variation type we need to also update all the attributes that are used to compute values
             if value not in ['scaling', 'offset']:
                 raise InvalidTypeError(f"Latent {self.name} variation type can only be one of 'scaling', 'offset'.")
             # Only need to update all the attributes if the variation type is actually changing
             if not hasattr(self, 'vrtn_type') or self.vrtn_type != value:
                 self._op = np.multiply if value == 'scaling' else np.add
@@ -242,15 +245,15 @@
         self.compute = mdl_eqn
         self.compute_args = inspect.signature(self.compute).parameters.keys()
         # Define 'true'/underlying values for equation inputs used to simulate degradation
         # No latent variable values should be specified when performing model inference
         self.latent_vars = []
         for var in latent_vars:
             # If no name was specified for the latent variable, nice to set it to the same name as used in the model
-            if not latent_vars[var].name:
+            if latent_vars[var].name == '' or not latent_vars[var].name:
                 latent_vars[var].name = var
             # Indicate the latent variable attributes as private since they're supposed to be uncertain
             setattr(self, f"_latent_{var}", latent_vars[var])
             self.latent_vars.append(var)
 
     def latent_var(self, var: str):
         """
@@ -320,15 +323,15 @@
         # Now define the model's compute function
         computed = self.compute(**vals)
 
         # Finally, define the output as a variable as well
         if target_framework == 'pymc':
             return pymc.Normal(name=self.name, mu=computed, sigma=1, observed=observed[self.name])
         elif target_framework == 'pyro':
-            return pyro.sample(self.name, dist.Normal(computed, 1), obs=observed[self.name])
+            return pyro.sample(self.name, dist.Normal(computed, 0.1), obs=observed[self.name]).to_event(1)
 
 
 class MechMdl(LatentMdl):
     """
     Class for modelling the effect of a wear-out reliability mechanism on some physical parameter.
 
     This class should not be instantiated directly, use an inheriting class.
@@ -804,15 +807,16 @@
         """
         # Overload the gen_latent_vals method to add generation of latents for sub-models
         # Note that initial value variations are not generated because they don't need to be persisted, only used once
         latents = {'cond': self.cond_mdl.gen_latent_vals(num_devs, num_chps, num_lots)}
         for mech in self.mech_mdl_list:
             latents[mech] = self.mech_mdl(mech).gen_latent_vals(num_devs, num_chps, num_lots)
         # The degraded parameter compute equation can have its own latent variables if desired, merge those if so
-        return latents | super().gen_latent_vals(num_devs, num_chps, num_lots)
+        latents.update(super().gen_latent_vals(num_devs, num_chps, num_lots))
+        return latents
 
     def gen_init_mech_vals(self, num_devs: int = 1, num_chps: int = 1, num_lots: int = 1) -> dict:
         """
         Generates initial values for the mechanisms that affect this parameter's value, typically unitary values
 
         Parameters
         ----------
```

### Comparing `gerabaldi-0.1.0/gerabaldi/models/phys_envs.py` & `gerabaldi-0.1.2/gerabaldi/models/phys_envs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Copyright (c) 2023 Ian Hill
 # SPDX-License-Identifier: Apache-2.0
 
 """Classes for defining physical noise sources and measurement capabilities in a test environment."""
 
+from __future__ import annotations
+
 from math import floor, log10
 import numpy as np
 import pandas as pd
 # For some reason using pd.Series doesn't play well with type annotations
 from pandas import Series
 
 from gerabaldi.models.devices import DeviceMdl
```

### Comparing `gerabaldi-0.1.0/gerabaldi/models/random_vars.py` & `gerabaldi-0.1.2/gerabaldi/models/random_vars.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Copyright (c) 2023 Ian Hill
 # SPDX-License-Identifier: Apache-2.0
 
 """Custom generators for random variables used for experiment simulation and model specification. Necessary as the Numpy
 and PyMC RVs either cannot be persisted or futz about with tensor types."""
 
+from __future__ import annotations
+
 import numpy as np
 
 from gerabaldi.helpers import _on_demand_import
 
 # Optional imports are loaded using a helper function that suppresses import errors until attempted use
 pymc = _on_demand_import('pymc')
 pyro = _on_demand_import('pyro', 'pyro-ppl')
@@ -29,23 +31,22 @@
         # Test seed is used to make the random variable sampling reproducible for testing purposes only
         if test_seed:
             self._generator = getattr(np.random.default_rng(seed=test_seed), self._dist_type)
         else:
             self._generator = getattr(np.random.default_rng(), self._dist_type)
 
     def _get_dist_params(self, target: str = 'pymc'):
-        match target:
-            case 'pymc':
-                return self._params_for_pymc()
-            case 'numpy':
-                return self._params_for_numpy()
-            case 'pyro':
-                return self._params_for_pyro()
-            case _:
-                raise NotImplementedError(f"Invalid target library {target} requested.")
+        if target == 'pymc':
+            return self._params_for_pymc()
+        elif target == 'numpy':
+            return self._params_for_numpy()
+        elif target == 'pyro':
+            return self._params_for_pyro()
+        else:
+            raise NotImplementedError(f"Invalid target library {target} requested.")
 
     def sample(self, quantity: int = 1) -> np.ndarray:
         """
         Return a quantity of random generated samples from the random variable distribution
 
         Parameters
         ----------
```

### Comparing `gerabaldi-0.1.0/gerabaldi/models/reports.py` & `gerabaldi-0.1.2/gerabaldi/models/reports.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Copyright (c) 2023 Ian Hill
 # SPDX-License-Identifier: Apache-2.0
 
 """Custom classes for reporting results of Gerabaldi simulations"""
 
+from __future__ import annotations
+
 import json
 import pandas as pd
 import numpy as np
 from datetime import timedelta
 from pathlib import Path
 
 from gerabaldi.models.test_specs import TestSpec
@@ -32,16 +34,16 @@
         A mapping from names of device parameters being measured to the quantities of each measured per chip
     num_chps: int
         The quantity of chips in the simulation per production lot
     num_lots: int
         The quantity of lots in the simulation
     measurements: pandas.DataFrame
         A tabular data structure with all the simulated measurements of device parameters conducted during the test
-    stress_summary: pandas.DataFrame
-        A tabular data structure that explains the stress conditions used during the test
+    test_summary: pandas.DataFrame
+        A tabular data structure that explains the stress and measure conditions used during the test
     """
 
     def __init__(self, test_spec: TestSpec = None, name: str = None, description: str = None, file: str = None):
         """
         Parameters
         ----------
         test_spec: TestSpec, optional
@@ -56,56 +58,58 @@
         # Standard construction is using a test specification to determine all the basic test information
         if test_spec:
             self.test_name = name if name else test_spec.name
             self.test_description = description if description else test_spec.description
             self.num_chps, self.num_lots = test_spec.num_chps, test_spec.num_lots
             self.dev_counts = test_spec.calc_samples_needed()
             self.measurements = pd.DataFrame()
-            self.stress_summary = pd.DataFrame()
+            self.test_summary = pd.DataFrame()
         # Can also load existing test data from a file
         elif file:
             if file:
                 try:
                     with open(file, 'r') as f:
                         report_json = json.load(f)
                 except FileNotFoundError:
                     msg = f"Could not find the requested data file {file}, the file does not appear to exist."
                     raise FileNotFoundError(msg)
             self.test_name = report_json['Test Name']
             self.test_description = report_json['Description']
             self.measurements = pd.read_json(report_json['Measurements'])
-            self.stress_summary = pd.read_json(report_json['Stress Summary'])
+            self.test_summary = pd.read_json(report_json['Test Summary'])
             # Convert the times back to time deltas
             units = report_json['Time Units'].lower()
             self.measurements['time'] = self.measurements['time'].apply(_convert_time, units=units, axis=1)
-            self.stress_summary['start time'] = self.stress_summary['start time'].apply(_convert_time, units=units,
-                                                                                        axis=1)
-            self.stress_summary['end time'] = self.stress_summary['end time'].apply(_convert_time, units=units, axis=1)
-            self.stress_summary['duration'] = self.stress_summary['duration'].apply(_convert_time, units=units, axis=1)
+            self.test_summary['start time'] = self.test_summary['start time'].apply(_convert_time, units=units,
+                                                                                    axis=1)
+            self.test_summary['end time'] = self.test_summary['end time'].apply(_convert_time, units=units, axis=1)
+            self.test_summary['duration'] = self.test_summary['duration'].apply(_convert_time, units=units, axis=1)
         # Allow for empty report initializations, though is not an expected use case
         else:
             self.test_name, self.test_description = name, description
-            self.measurements, self.stress_summary = None, None
+            self.measurements, self.test_summary = None, None
             self.num_chps, self.num_lots, self.dev_counts = None, None, None
 
     @staticmethod
-    def format_measurements(measured_vals: list | pd.Series | np.ndarray, prm_name: str, meas_time: timedelta,
-                            prm_type: str = 'parameter') -> pd.DataFrame:
+    def format_measurements(measured_vals: list | pd.Series | np.ndarray, prm_name: str,
+                            meas_time: timedelta, meas_step: int, prm_type: str = 'parameter') -> pd.DataFrame:
         """
         Take a set of measured values of a parameter and condition and create a formatted dataframe to report the
         measured values in.
 
         Parameters
         ----------
         measured_vals: list or pandas.Series or numpy.ndarray
             The unformatted (i.e. simulator internal) set of measurement data to send to a tabular format
         prm_name: str
             The name of the parameter that the measured_vals measurements correspond to
         meas_time: timedelta
             The relative time at which the measurements were taken within the test duration
+        meas_step: int
+            The unique number of the test step that this measurement data is associated with
         prm_type: str, optional
             Whether the measurements are for a device 'parameter' or a stress 'condition' (default 'parameter')
 
         Returns
         -------
         pandas.DataFrame
             A formatted tabular structure that can be concatenated/appended to other sets of formatted measurements
@@ -118,14 +122,15 @@
             circ_num = np.tile(np.linspace(0, num_meas - 1, num_meas, dtype=int), num_devs * num_lots)
             dev_num = np.tile(np.repeat(np.linspace(0, num_devs - 1, num_devs, dtype=int), num_meas), num_lots)
             lot_num = np.repeat(np.linspace(0, num_lots - 1, num_lots, dtype=int), num_meas * num_devs)
         elif prm_type == 'condition':
             num_lots, num_devs, num_meas = measured_vals.shape
             measured_vals = measured_vals.reshape(num_meas * num_devs * num_lots)
         formatted = pd.DataFrame({'param': prm_name,
+                                  'step #': meas_step,
                                   'device #': circ_num,
                                   'chip #': dev_num,
                                   'lot #': lot_num,
                                   'time': meas_time,
                                   'measured': measured_vals})
         return formatted
 
@@ -136,24 +141,24 @@
         Parameters
         ----------
         measured: pandas.DataFrame
             The formatted measurements to concatenate/append to the existing full set of measurements
         """
         self.measurements = pd.concat([self.measurements, measured], ignore_index=True)
 
-    def add_stress_report(self, strs_conds: pd.DataFrame):
+    def add_summary_report(self, summary_info: pd.DataFrame):
         """
-        Add stress reporting rows to the dataframe of all reported stress phases
+        Add summary reporting rows to the dataframe of all existing test step summaries
 
         Parameters
         ----------
-        strs_conds: pandas.DataFrame
-            The formatted report of stress conditions to add to the full stress summary
+        summary_info: pandas.DataFrame
+            The formatted report of test step information to add to the full test summary
         """
-        self.stress_summary = pd.concat([self.stress_summary, strs_conds], ignore_index=True)
+        self.test_summary = pd.concat([self.test_summary, summary_info], ignore_index=True)
 
     def export_to_json(self, file: str = None, time_units: str = 'seconds') -> None | dict:
         """
         Formats a test report as a json string so that it can be saved as a file for storage or sharing
 
         Parameters
         ----------
@@ -178,19 +183,19 @@
                                           "defaulting to seconds.")
             div_time = 1
             report_json['Time Units'] = 'Seconds'
 
         meas_cpy = self.measurements.copy()
         meas_cpy['time'] = meas_cpy['time'].apply(_convert_time, units=div_time, axis=1)
         report_json['Measurements'] = meas_cpy.to_json()
-        strs_cpy = self.stress_summary.copy()
+        strs_cpy = self.test_summary.copy()
         strs_cpy['duration'] = strs_cpy['duration'].apply(_convert_time, units=div_time, axis=1)
         strs_cpy['start time'] = strs_cpy['start time'].apply(_convert_time, units=div_time, axis=1)
         strs_cpy['end time'] = strs_cpy['end time'].apply(_convert_time, units=div_time, axis=1)
-        report_json['Stress Summary'] = strs_cpy.to_json()
+        report_json['Test Summary'] = strs_cpy.to_json()
 
         if file:
             # Make the directory if it doesn't yet exist, otherwise the file open will fail
             data_dir = file.rpartition('/')[0]
             Path(data_dir).mkdir(exist_ok=True)
             with open(file, 'w') as f:
                 json.dump(report_json, f)
```

### Comparing `gerabaldi-0.1.0/gerabaldi/models/states.py` & `gerabaldi-0.1.2/gerabaldi/models/states.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Copyright (c) 2023 Ian Hill
 # SPDX-License-Identifier: Apache-2.0
 
 """Custom classes for simulation state persistence"""
 
+from __future__ import annotations
+
 from datetime import timedelta
 from copy import deepcopy
 
 __all__ = ['TestSimState']
 
 
 class TestSimState:
```

### Comparing `gerabaldi-0.1.0/gerabaldi/models/test_specs.py` & `gerabaldi-0.1.2/gerabaldi/models/test_specs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Copyright (c) 2023 Ian Hill
 # SPDX-License-Identifier: Apache-2.0
 
 """Classes for defining wear-out tests in terms of conditions, durations, execution steps, and collected data"""
 
+from __future__ import annotations
+
 from datetime import timedelta
 
 from gerabaldi.exceptions import UserConfigError
 
 __all__ = ['MeasSpec', 'StrsSpec', 'TestSpec']
```

### Comparing `gerabaldi-0.1.0/gerabaldi/sim.py` & `gerabaldi-0.1.2/gerabaldi/sim.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Copyright (c) 2023 Ian Hill
 # SPDX-License-Identifier: Apache-2.0
 
 """Gerabaldi top-level simulation execution functions"""
 
+from __future__ import annotations
+
 import pandas as pd
 from datetime import timedelta
 from copy import deepcopy
 
 from gerabaldi.models import *
 from gerabaldi.exceptions import MissingParamError, UserConfigError
 
@@ -47,32 +49,41 @@
     elif dev_counts:
         devs, chps, lots = dev_counts, num_chps, num_lots
     else:
         raise UserConfigError('The number of devices for each parameter must be specified either manually or by report.'
                               'Cannot provide neither or both.')
 
     # Check the parameter dependencies for each circuit parameter that could depend on one or more degraded parameters
-    for circ_prm in [prm for prm in devs if type(dev_mdl.prm_mdl(prm)) == CircPrmMdl]:
-        for required_prm in dev_mdl.prm_mdl(circ_prm).get_required_prms(dev_mdl.prm_mdl_list):
-            # Ensure that enough of the required degraded parameters are specified to support the circuit parameters
-            if required_prm not in devs.keys() or devs[required_prm] < devs[circ_prm]:
-                devs[required_prm] = devs[circ_prm]
-                # If a report was used to specify device counts, update the report to include the changes
-                if quantity_info:
-                    quantity_info.dev_counts[required_prm] = devs[circ_prm]
+    # Have to copy the dict of measured parameters as we will modify the original copy within the below loop
+    measured_devs = devs.copy()
+    for prm in measured_devs:
+        # First check if the parameter is a device parameter or a stress condition, skip if a stress condition
+        try:
+            prm_type = type(dev_mdl.prm_mdl(prm))
+        except AttributeError:
+            continue
+        # Now get dependencies of the circuit parameter, i.e. which other device parameters are needed to compute
+        if prm_type == CircPrmMdl:
+            for required_prm in dev_mdl.prm_mdl(prm).get_required_prms(dev_mdl.prm_mdl_list):
+                # Ensure that enough of the required degraded parameters are specified to support the circuit parameters
+                if required_prm not in devs.keys() or devs[required_prm] < devs[prm]:
+                    devs[required_prm] = devs[prm]
+                    # If a report was used to specify device counts, update the report to include the changes
+                    if quantity_info:
+                        quantity_info.dev_counts[required_prm] = devs[prm]
 
     # Now initialize the physical state and override the elapsed time if specified
     init_state = dev_mdl.gen_init_state(devs, chps, lots)
     if elapsed_time != 0:
         init_state.elapsed = elapsed_time
     return init_state
 
 
 def _sim_stress_step(step: StrsSpec, sim_state: TestSimState, dev_mdl: DeviceMdl,
-                     test_env: PhysTestEnv, report: TestSimReport):
+                     test_env: PhysTestEnv, report: TestSimReport, step_id: int):
     # 1. Build the stochastically-adjusted set of stress conditions
     # Only need to generate stress conditions for device parameters that degrade, get the list of those parameters
     deg_prm_list = [prm for prm in dev_mdl.prm_mdl_list if type(dev_mdl.prm_mdl(prm)) == DegPrmMdl]
     strs_conds = test_env.gen_env_cond_vals(step.conditions, deg_prm_list, report, dev_mdl, 'stress')
 
     for prm in deg_prm_list:
         # 2. Calculate the equivalent stress times that would have been needed under the generated stress conditions to
@@ -92,64 +103,73 @@
             sim_state.latent_var_vals[prm], sim_state.curr_deg_mech_vals[prm]
         )
 
     # Update the elapsed real-world test time
     sim_state.elapsed += step.duration
 
     # 4. Report the stress conditions used during this step
-    merged = {'stress step': step.name, 'duration': step.duration,
-              'start time': sim_state.elapsed - step.duration, 'end time': sim_state.elapsed} | step.conditions
+    merged = {'step name': step.name, 'step type': 'stress', 'step number': step_id, 'duration': step.duration,
+              'start time': sim_state.elapsed - step.duration, 'end time': sim_state.elapsed}
+    merged.update(step.conditions)
     # Use a DataFrame instead of a Series to simplify the process of merging the reports of different stress steps
     stress_report = pd.DataFrame(merged, index=[0])
-    report.add_stress_report(stress_report)
+    report.add_summary_report(stress_report)
 
 
 def _sim_meas_step(step: MeasSpec, sim_state: TestSimState, dev_mdl: DeviceMdl,
-                   test_env: PhysTestEnv, report: TestSimReport):
+                   test_env: PhysTestEnv, report: TestSimReport, step_id: int):
     """
     Given a test measurement specification, generate the set of observed values. The baseline/true parameter values
     are provided within the step and deg_data arguments, the measurement process adjusts these values according to test
     conditions, stochastic variations, and imperfect measurement instruments.
     """
     # Loop through the parameters to measure and determine if they are degraded parameters or independent conditions
     meas_results = pd.DataFrame()
     # Generate 'true' values for environmental conditions specified by the step (using their variability models)
-    env_conds = test_env.gen_env_cond_vals(step.conditions, step.measurements, report, dev_mdl, 'measure')
+    conds = test_env.gen_env_cond_vals(step.conditions, step.measurements, report, dev_mdl, 'measure')
 
     for prm in step.measurements:
         # There are three types of parameters: environmental conditions, degraded parameters and derived parameters
         if prm in sim_state.curr_prm_vals:
             # Adjust the param values based on environmental conditions during measurement and the instrument used
             measured = dev_mdl.prm_mdl(prm).calc_cond_shifted_vals(
                 (report.num_lots, report.num_chps, step.measurements[prm]),
-                env_conds[prm], sim_state.curr_prm_vals[prm], sim_state.latent_var_vals[prm])
-            measured = TestSimReport.format_measurements(measured, prm, sim_state.elapsed, 'parameter')
+                conds[prm], sim_state.curr_prm_vals[prm], sim_state.latent_var_vals[prm])
+            measured = TestSimReport.format_measurements(measured, prm, sim_state.elapsed, step_id, 'parameter')
 
         elif prm in dev_mdl.prm_mdl_list:
             # Derived parameter values that can depend on multiple degraded parameters, i.e. circuit models
             measured = dev_mdl.prm_mdl(prm).calc_circ_vals(
-                step.measurements[prm], env_conds[prm], sim_state.curr_prm_vals, sim_state.latent_var_vals[prm])
-            measured = TestSimReport.format_measurements(measured, prm, sim_state.elapsed, 'parameter')
+                step.measurements[prm], conds[prm], sim_state.curr_prm_vals, sim_state.latent_var_vals[prm])
+            measured = TestSimReport.format_measurements(measured, prm, sim_state.elapsed, step_id, 'parameter')
 
         elif prm in step.conditions:
             # These parameters are not degraded parameters of the device but instead environmental parameters
-            measured = TestSimReport.format_measurements(env_conds[prm][prm], prm, sim_state.elapsed, 'condition')
+            measured = TestSimReport.format_measurements(conds[prm][prm], prm, sim_state.elapsed, step_id, 'condition')
 
         else:
             raise MissingParamError(f"Requested measurement of param '{prm}' failed, param is not defined within the \
             simulated test.")
 
         # With the measurements completed, configure the dataframe for reporting and add to the merged dataframe
         measured['measured'] = test_env.meas_instm(prm).measure(measured['measured'])
         meas_results = pd.concat((meas_results, measured), ignore_index=True)
 
     if step.verbose:
         print(f"Conducted measurement {step.name} at simulation time {sim_state.elapsed}.")
     report.add_measurements(meas_results)
 
+    # Report the stress conditions used during this step
+    merged = {'step name': step.name, 'step type': 'measure', 'step number': step_id, 'duration': timedelta(),
+              'start time': sim_state.elapsed, 'end time': sim_state.elapsed}
+    merged.update(step.conditions)
+    # Use a DataFrame instead of a Series to simplify the process of merging the reports of different stress steps
+    meas_report = pd.DataFrame(merged, index=[0])
+    report.add_summary_report(meas_report)
+
 
 def simulate(test_def: TestSpec, dev_mdl: DeviceMdl, test_env: PhysTestEnv,
              init_state: TestSimState = None) -> TestSimReport:
     """
     Simulate a given wear-out test using a given underlying model
 
     Parameters
@@ -174,14 +194,14 @@
     if not init_state:
         sim_state = gen_init_state(dev_mdl, quantity_info=test_report)
     else:
         sim_state = deepcopy(init_state)
 
     # We now execute the test step by step, sequentially performing measurements and stress intervals in order
     # Note that sim_state and test_report are mutated as the test progresses, the other data structures are untouched
-    for step in test_def:
+    for i, step in enumerate(test_def):
         # Check whether the next step is a measurement or period of stress
         if type(step) is StrsSpec:
-            _sim_stress_step(step, sim_state, dev_mdl, test_env, test_report)
+            _sim_stress_step(step, sim_state, dev_mdl, test_env, test_report, i)
         elif type(step) is MeasSpec:
-            _sim_meas_step(step, sim_state, dev_mdl, test_env, test_report)
+            _sim_meas_step(step, sim_state, dev_mdl, test_env, test_report, i)
     return test_report
```

### Comparing `gerabaldi-0.1.0/gerabaldi.egg-info/PKG-INFO` & `gerabaldi-0.1.2/gerabaldi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: gerabaldi
-Version: 0.1.0
+Version: 0.1.2
 Summary: A temporal simulator for probabilistic degradation and failure processes with a focus on integrated circuit wear-out 
 Author-email: Ian Hill <ianrmhill@gmail.com>
 Project-URL: Homepage, https://github.com/ianrmhill/gerabaldi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.10
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Gerabaldi Wear-Out Reliability Simulator / Generative Aging Model
 
 The Gerabaldi module allows for generic simulation of arbitrary integrated circuit reliability tests, enabling data
 generation for tests or use cases where obtaining the corresponding real-world data could require hundreds of hours or
@@ -43,26 +43,27 @@
 ## Demos
 
 The 'demos' folder of this repository contains some useful references for full working simulations with command-line
 interfaces and visualization of results. These can be run directly if you have cloned the source code, or if you
 installed the packaged version it is easiest to copy-paste the source code from Github (you will want to remove the
 automated path add code at the very top of the demo file as the 'gerabaldi' import should already work without it).
 
-Note that the VTS paper demos will take a significant amount of time to run due to the size of the simulations, these
-can be reduced by changing the three globals near the tops of the files as follows:
-
-For demo 1:
-`NUM_SAMPLES = 5`
-`NUM_DEVICES = 5`
-`NUM_LOTS = 5`
-
-For demo 2:
-`TEST_LEN = 24 * 7 * 52 * 2`
-`NUM_SAMPLES = 100`
-`C_LATENT = 4e-5`
+Note that the VTS paper demos will require modification and take a significant amount of time to obtain the exact
+results shown due to the size of the simulations, to run the full simulations change the three globals near the tops of
+the files as follows:
+
+For demo 1 (pre-silicon variability analysis):
+`NUM_DEVICES = 10`
+`NUM_CHIPS = 10`
+`NUM_LOTS = 10`
+
+For demo 2 (TDDB model sensitivity):
+`TEST_LEN = 24 * 7 * 52 * 20`
+`NUM_SAMPLES = 1000`
+`C_LATENT = 4e-6`
 
 Running the simulations with these values will provide similar-looking results but with far less computation and is
 useful for quickly seeing these more complex simulations in action.
 
 
 ## Basic Use
```

### Comparing `gerabaldi-0.1.0/gerabaldi.egg-info/SOURCES.txt` & `gerabaldi-0.1.2/gerabaldi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gerabaldi-0.1.0/pyproject.toml` & `gerabaldi-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 name = "gerabaldi"
 dynamic = ["version", "dependencies"]
 authors = [
   { name="Ian Hill", email="ianrmhill@gmail.com" },
 ]
 description = "A temporal simulator for probabilistic degradation and failure processes with a focus on integrated circuit wear-out "
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Physics",
     "Intended Audience :: Science/Research",
     "Development Status :: 3 - Alpha",
```

