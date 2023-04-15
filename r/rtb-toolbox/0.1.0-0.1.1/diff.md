# Comparing `tmp/rtb_toolbox-0.1.0.tar.gz` & `tmp/rtb_toolbox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtb_toolbox-0.1.0.tar", max compression
+gzip compressed data, was "rtb_toolbox-0.1.1.tar", max compression
```

## Comparing `rtb_toolbox-0.1.0.tar` & `rtb_toolbox-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0        0 2023-04-14 21:56:06.455291 rtb_toolbox-0.1.0/README.md
--rw-r--r--   0        0        0      322 2023-04-14 22:04:11.923360 rtb_toolbox-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4034 2023-04-14 21:53:58.999300 rtb_toolbox-0.1.0/src/rtb_toolbox/README.md
--rw-r--r--   0        0        0      180 2023-04-14 21:57:08.635282 rtb_toolbox-0.1.0/src/rtb_toolbox/__init__.py
--rw-r--r--   0        0        0     2290 2023-04-14 21:52:22.187974 rtb_toolbox-0.1.0/src/rtb_toolbox/forward_dynamics/__init__.py
--rw-r--r--   0        0        0     3517 2023-04-14 21:52:22.191974 rtb_toolbox-0.1.0/src/rtb_toolbox/forward_kinematics/__init__.py
--rw-r--r--   0        0        0     3097 2023-04-14 21:52:22.203974 rtb_toolbox-0.1.0/src/rtb_toolbox/frame/__init__.py
--rw-r--r--   0        0        0    33140 2023-04-14 21:54:20.903286 rtb_toolbox-0.1.0/src/rtb_toolbox/images/full_ik.png
--rw-r--r--   0        0        0    33229 2023-04-14 21:54:20.907286 rtb_toolbox-0.1.0/src/rtb_toolbox/images/partial_ik.png
--rw-r--r--   0        0        0     6569 2023-04-14 21:54:20.915286 rtb_toolbox-0.1.0/src/rtb_toolbox/images/tau1.png
--rw-r--r--   0        0        0     5005 2023-04-14 21:54:20.915286 rtb_toolbox-0.1.0/src/rtb_toolbox/images/tau2.png
--rw-r--r--   0        0        0   479230 2023-04-14 21:54:20.923286 rtb_toolbox-0.1.0/src/rtb_toolbox/images/trajectories.png
--rw-r--r--   0        0        0     7386 2023-04-14 21:52:22.211974 rtb_toolbox-0.1.0/src/rtb_toolbox/inverse_kinematics/__init__.py
--rw-r--r--   0        0        0     1665 2023-04-14 21:52:22.219974 rtb_toolbox-0.1.0/src/rtb_toolbox/link/__init__.py
--rw-r--r--   0        0        0       55 2023-04-14 21:52:22.347973 rtb_toolbox-0.1.0/src/rtb_toolbox/symbols.py
--rw-r--r--   0        0        0     1150 2023-04-14 21:52:22.231974 rtb_toolbox-0.1.0/src/rtb_toolbox/trajectory/__init__.py
--rw-r--r--   0        0        0     4724 2023-04-14 21:52:22.283974 rtb_toolbox-0.1.0/src/rtb_toolbox/utils/__init__.py
--rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 rtb_toolbox-0.1.0/setup.py
--rw-r--r--   0        0        0      339 1970-01-01 00:00:00.000000 rtb_toolbox-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-14 21:56:06.455291 rtb_toolbox-0.1.1/README.md
+-rw-r--r--   0        0        0      322 2023-04-14 22:14:05.543963 rtb_toolbox-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4034 2023-04-14 21:53:58.999300 rtb_toolbox-0.1.1/src/rtb_toolbox/README.md
+-rw-r--r--   0        0        0      264 2023-04-14 22:12:13.127853 rtb_toolbox-0.1.1/src/rtb_toolbox/__init__.py
+-rw-r--r--   0        0        0     2298 2023-04-14 22:12:18.847856 rtb_toolbox-0.1.1/src/rtb_toolbox/forward_dynamics/__init__.py
+-rw-r--r--   0        0        0     3533 2023-04-14 22:12:26.419864 rtb_toolbox-0.1.1/src/rtb_toolbox/forward_kinematics/__init__.py
+-rw-r--r--   0        0        0     3097 2023-04-14 21:52:22.203974 rtb_toolbox-0.1.1/src/rtb_toolbox/frame/__init__.py
+-rw-r--r--   0        0        0    33140 2023-04-14 21:54:20.903286 rtb_toolbox-0.1.1/src/rtb_toolbox/images/full_ik.png
+-rw-r--r--   0        0        0    33229 2023-04-14 21:54:20.907286 rtb_toolbox-0.1.1/src/rtb_toolbox/images/partial_ik.png
+-rw-r--r--   0        0        0     6569 2023-04-14 21:54:20.915286 rtb_toolbox-0.1.1/src/rtb_toolbox/images/tau1.png
+-rw-r--r--   0        0        0     5005 2023-04-14 21:54:20.915286 rtb_toolbox-0.1.1/src/rtb_toolbox/images/tau2.png
+-rw-r--r--   0        0        0   479230 2023-04-14 21:54:20.923286 rtb_toolbox-0.1.1/src/rtb_toolbox/images/trajectories.png
+-rw-r--r--   0        0        0     7410 2023-04-14 22:12:36.779874 rtb_toolbox-0.1.1/src/rtb_toolbox/inverse_kinematics/__init__.py
+-rw-r--r--   0        0        0     1673 2023-04-14 22:12:40.815878 rtb_toolbox-0.1.1/src/rtb_toolbox/link/__init__.py
+-rw-r--r--   0        0        0       55 2023-04-14 21:52:22.347973 rtb_toolbox-0.1.1/src/rtb_toolbox/symbols.py
+-rw-r--r--   0        0        0     1150 2023-04-14 21:52:22.231974 rtb_toolbox-0.1.1/src/rtb_toolbox/trajectory/__init__.py
+-rw-r--r--   0        0        0     4732 2023-04-14 22:12:47.927885 rtb_toolbox-0.1.1/src/rtb_toolbox/utils/__init__.py
+-rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 rtb_toolbox-0.1.1/setup.py
+-rw-r--r--   0        0        0      339 1970-01-01 00:00:00.000000 rtb_toolbox-0.1.1/PKG-INFO
```

### Comparing `rtb_toolbox-0.1.0/src/rtb_toolbox/README.md` & `rtb_toolbox-0.1.1/src/rtb_toolbox/README.md`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.0/src/rtb_toolbox/forward_dynamics/__init__.py` & `rtb_toolbox-0.1.1/src/rtb_toolbox/forward_dynamics/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sympy as sp
 
-from lib.symbols import g, t
+from rtb_toolbox.symbols import g, t
 
 
 class ForwardDynamics:
     def __init__(self, forward_kinematics):
         self.jacobian = forward_kinematics.jacobian
         self.links = forward_kinematics.links_zero_i
```

### Comparing `rtb_toolbox-0.1.0/src/rtb_toolbox/forward_kinematics/__init__.py` & `rtb_toolbox-0.1.1/src/rtb_toolbox/forward_kinematics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import sympy as sp
 
-from lib.link import Link
-from lib.utils import compute_homogeneous_transformation
+from rtb_toolbox.link import Link
+from rtb_toolbox.utils import compute_homogeneous_transformation
 
 
 class ForwardKinematic:
     def __init__(self,
                  links,
         ):
```

### Comparing `rtb_toolbox-0.1.0/src/rtb_toolbox/frame/__init__.py` & `rtb_toolbox-0.1.1/src/rtb_toolbox/frame/__init__.py`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.0/src/rtb_toolbox/images/full_ik.png` & `rtb_toolbox-0.1.1/src/rtb_toolbox/images/full_ik.png`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.0/src/rtb_toolbox/images/partial_ik.png` & `rtb_toolbox-0.1.1/src/rtb_toolbox/images/partial_ik.png`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.0/src/rtb_toolbox/images/tau1.png` & `rtb_toolbox-0.1.1/src/rtb_toolbox/images/tau1.png`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.0/src/rtb_toolbox/images/tau2.png` & `rtb_toolbox-0.1.1/src/rtb_toolbox/images/tau2.png`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.0/src/rtb_toolbox/images/trajectories.png` & `rtb_toolbox-0.1.1/src/rtb_toolbox/images/trajectories.png`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.0/src/rtb_toolbox/inverse_kinematics/__init__.py` & `rtb_toolbox-0.1.1/src/rtb_toolbox/inverse_kinematics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
 import sympy as sp
 
 from pymoo.core.problem import Problem
 from pymoo.optimize import minimize
 from pymoo.termination.default import MaximumGenerationTermination
 
-from lib.forward_kinematics import ForwardKinematic
-from lib.frame import x_y_z_rotation_matrix, translation_matrix
-from lib.utils import matrix_log6, inverse_transformation, se3_to_vec, normalize_angle_between_limits
+from rtb_toolbox.forward_kinematics import ForwardKinematic
+from rtb_toolbox.frame import x_y_z_rotation_matrix, translation_matrix
+from rtb_toolbox.utils import matrix_log6, inverse_transformation, se3_to_vec, normalize_angle_between_limits
 
 
 class InverseKinematicProblem(Problem):
     def __init__(
             self,
             desired_pose=None,
             fk: ForwardKinematic = None,
```

### Comparing `rtb_toolbox-0.1.0/src/rtb_toolbox/link/__init__.py` & `rtb_toolbox-0.1.1/src/rtb_toolbox/link/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from lib.utils import compute_link_transformation, np
+from rtb_toolbox.utils import compute_link_transformation, np
 
 
 class Link:
     def __init__(
             self,
             dhp=None,
             generalized_coordinate=None,
```

### Comparing `rtb_toolbox-0.1.0/src/rtb_toolbox/trajectory/__init__.py` & `rtb_toolbox-0.1.1/src/rtb_toolbox/trajectory/__init__.py`

 * *Files identical despite different names*

### Comparing `rtb_toolbox-0.1.0/src/rtb_toolbox/utils/__init__.py` & `rtb_toolbox-0.1.1/src/rtb_toolbox/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import sympy as sp
 
-from lib.frame import z_rotation_matrix, translation_matrix, x_rotation_matrix
+from rtb_toolbox.frame import z_rotation_matrix, translation_matrix, x_rotation_matrix
 
 
 def near_zero(s, epsilon=1e-6):
     """
       Returns True if the value is small enough to be considered zero.
 
     :param s: The value to check.
```

### Comparing `rtb_toolbox-0.1.0/setup.py` & `rtb_toolbox-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'rtb_toolbox.utils']
 
 package_data = \
 {'': ['*'], 'rtb_toolbox': ['images/*']}
 
 setup_kwargs = {
     'name': 'rtb-toolbox',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': '',
     'author': 'Miguel',
     'author_email': 'miguellukas52@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

