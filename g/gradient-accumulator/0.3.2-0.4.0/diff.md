# Comparing `tmp/gradient-accumulator-0.3.2.tar.gz` & `tmp/gradient-accumulator-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gradient-accumulator-0.3.2.tar", last modified: Thu Apr  6 21:50:02 2023, max compression
+gzip compressed data, was "dist/gradient-accumulator-0.4.0.tar", last modified: Sat Apr 15 11:02:33 2023, max compression
```

## Comparing `gradient-accumulator-0.3.2.tar` & `gradient-accumulator-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:50:02.000000 gradient-accumulator-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (122)    15309 2023-04-06 21:50:02.000000 gradient-accumulator-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    12093 2023-04-06 21:49:17.000000 gradient-accumulator-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:50:02.000000 gradient-accumulator-0.3.2/gradient_accumulator/
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-04-06 21:49:17.000000 gradient-accumulator-0.3.2/gradient_accumulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10916 2023-04-06 21:49:17.000000 gradient-accumulator-0.3.2/gradient_accumulator/accumulators.py
--rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-04-06 21:49:17.000000 gradient-accumulator-0.3.2/gradient_accumulator/agc.py
--rw-r--r--   0 runner    (1001) docker     (122)     2949 2023-04-06 21:49:17.000000 gradient-accumulator-0.3.2/gradient_accumulator/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 21:50:02.000000 gradient-accumulator-0.3.2/gradient_accumulator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    15309 2023-04-06 21:50:02.000000 gradient-accumulator-0.3.2/gradient_accumulator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      376 2023-04-06 21:50:02.000000 gradient-accumulator-0.3.2/gradient_accumulator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-06 21:50:02.000000 gradient-accumulator-0.3.2/gradient_accumulator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-06 21:50:02.000000 gradient-accumulator-0.3.2/gradient_accumulator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-04-06 21:50:02.000000 gradient-accumulator-0.3.2/gradient_accumulator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-06 21:50:02.000000 gradient-accumulator-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1255 2023-04-06 21:49:17.000000 gradient-accumulator-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-15 11:02:33.000000 gradient-accumulator-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     8328 2023-04-15 11:02:33.000000 gradient-accumulator-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6420 2023-04-15 11:01:54.000000 gradient-accumulator-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-15 11:02:33.000000 gradient-accumulator-0.4.0/gradient_accumulator/
+-rw-r--r--   0 runner    (1001) docker     (122)      166 2023-04-15 11:01:54.000000 gradient-accumulator-0.4.0/gradient_accumulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14947 2023-04-15 11:01:54.000000 gradient-accumulator-0.4.0/gradient_accumulator/accumulators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2538 2023-04-15 11:01:54.000000 gradient-accumulator-0.4.0/gradient_accumulator/agc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6463 2023-04-15 11:01:54.000000 gradient-accumulator-0.4.0/gradient_accumulator/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-15 11:02:33.000000 gradient-accumulator-0.4.0/gradient_accumulator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8328 2023-04-15 11:02:33.000000 gradient-accumulator-0.4.0/gradient_accumulator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      376 2023-04-15 11:02:33.000000 gradient-accumulator-0.4.0/gradient_accumulator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-15 11:02:33.000000 gradient-accumulator-0.4.0/gradient_accumulator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-15 11:02:33.000000 gradient-accumulator-0.4.0/gradient_accumulator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-04-15 11:02:33.000000 gradient-accumulator-0.4.0/gradient_accumulator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-15 11:02:33.000000 gradient-accumulator-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1302 2023-04-15 11:01:54.000000 gradient-accumulator-0.4.0/setup.py
```

### Comparing `gradient-accumulator-0.3.2/gradient_accumulator/accumulators.py` & `gradient-accumulator-0.4.0/gradient_accumulator/accumulators.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,55 @@
 import tensorflow as tf
 from . import agc
-#from tensorflow_addons.utils import types
-#from typeguard import typechecked
 
 
 # need to dynamically handle which Optimizer class to use dependent on tf version
 opt = tf.keras.optimizers.Optimizer
 if int(tf.version.VERSION.split(".")[1]) > 10:
     opt = tf.keras.optimizers.legacy.Optimizer
 
 
 # https://stackoverflow.com/a/66524901
 # https://keras.io/guides/customizing_what_happens_in_fit/
 @tf.keras.utils.register_keras_serializable()  # adding this avoids needing to use custom_objects when loading model
 class GradientAccumulateModel(tf.keras.Model):
-    def __init__(self, accum_steps=1, mixed_precision=False, use_agc=False, clip_factor=0.01, eps=1e-3, *args, **kwargs):
+    """Model wrapper for gradient accumulation."""
+    def __init__(self, accum_steps:int = 1, mixed_precision:bool = False, use_agc:bool = False,
+                 clip_factor:float = 0.01, eps:float = 1e-3, *args, **kwargs):
+        """Adds gradient accumulation support to existing Keras Model.
+
+        Args:
+            accum_steps: int > 0. Update gradient in every accumulation steps.
+            mixed_precision: bool. Whether to enable mixed precision.
+            use_agc: bool. Whether to enable adaptive gradient clipping.
+            clip_factor: float > 0. Upper limit to gradient clipping.
+            eps: float > 0. Small value to aid numerical stability.
+            **kwargs: keyword arguments.
+        """
         super().__init__(*args, **kwargs)
         self.accum_steps = tf.constant(accum_steps, dtype=tf.int32, name="accum_steps")
         self.accum_step_counter = tf.Variable(0, dtype=tf.int32, trainable=False, name="accum_counter",
                                               synchronization=tf.VariableSynchronization.ON_READ,
                                               aggregation=tf.VariableAggregation.ONLY_FIRST_REPLICA,
                                               )
         self.first_call = True
-        self.gradient_accumulation = None
-        self.reinit_grad_accum()
         self.mixed_precision = mixed_precision
         self.use_agc = use_agc
         self.clip_factor = clip_factor
         self.eps = eps
+        
+        self.dtype_value = tf.float32  # @TODO: This is probably not suited when tf.bloat32
+        #if mixed_precision:
+        #    self.dtype_value = tf.float16
+        
+        self.gradient_accumulation = None
+        self.reinit_grad_accum()
 
     def train_step(self, data):
+        """Performs single train step."""
         # need to reinit accumulator for models subclassed from tf.keras.Model
         if self.first_call:
             self.reinit_grad_accum()
             self.first_call = False
 
         self.accum_step_counter.assign_add(1)
 
@@ -55,15 +71,15 @@
             # The loss function is configured in `compile()`.
             loss = self.compiled_loss(
                 y,
                 y_pred,
                 sample_weight=sample_weight,
                 regularization_losses=self.losses,
             )
-            loss = loss / tf.cast(self.accum_steps, tf.float32)  # MEAN reduction here IMPORTANT! Don't use SUM!
+            loss = loss / tf.cast(self.accum_steps, loss.dtype)  # MEAN reduction here IMPORTANT! Don't use SUM!
 
             # scale loss if mixed precision is enabled
             if self.mixed_precision:
                 loss = self.optimizer.get_scaled_loss(loss)
 
         # Calculate batch gradients -> these are scaled gradients if mixed precision is enabled
         gradients = tape.gradient(loss, self.trainable_variables, unconnected_gradients=tf.UnconnectedGradients.ZERO)
@@ -87,41 +103,50 @@
                 false_fn=lambda: None)
 
         # update metrics
         self.compiled_metrics.update_state(y, y_pred, sample_weight=sample_weight)
         return {m.name: m.result() for m in self.metrics}
 
     def apply_accu_gradients(self):
+        """Performs gradient update and resets slots afterwards."""
         # apply accumulated gradients
         self.optimizer.apply_gradients(zip(self.gradient_accumulation, self.trainable_variables))
 
         # reset
         self.accum_step_counter.assign(0)
         for i in range(len(self.gradient_accumulation)):
             self.gradient_accumulation[i].assign(
-                tf.zeros_like(self.trainable_variables[i], dtype=tf.float32), read_value=False)
+                tf.zeros_like(self.trainable_variables[i], dtype=self.dtype_value), read_value=False)
     
     def reinit_grad_accum(self):
+        """Reinitialized gradient accumulator slots."""
         # reinitialize gradient accumulator
         self.gradient_accumulation = [
-            tf.Variable(tf.zeros_like(v, dtype=tf.float32), trainable=False,
+            tf.Variable(tf.zeros_like(v, dtype=self.dtype_value), trainable=False,
             name="accum_" + str(i),
             synchronization=tf.VariableSynchronization.ON_READ,
             aggregation=tf.VariableAggregation.ONLY_FIRST_REPLICA,
             ) for i, v in enumerate(self.trainable_variables)
         ]
 
 
 # Implementation was derived from:
 # https://github.com/fsx950223/addons/blob/67c1e8ea19e82c3f2a5706674dd81f15ab5002a2/tensorflow_addons/optimizers/gradient_accumulator.py
 @tf.keras.utils.register_keras_serializable()
 class GradientAccumulateOptimizer(opt):
     """Optimizer wrapper for gradient accumulation."""
     def __init__(self, optimizer="SGD", accum_steps=1, reduction: str = "MEAN", name: str = "GradientAccumulateOptimizer", **kwargs):
-        r"""Construct a new GradientAccumulateOptimizer optimizer.
+        """Construct a new GradientAccumulateOptimizer optimizer.
+
+        Adding support for sparse tensors was tricky, but this resource was helpful.
+        Note that you need to implement both _resource_apply_sparse() and
+        _resource_apply_sparse_duplicate_indices() for it to work as intended.
+
+        See here for more information regarding implementation:
+        * https://github.com/tensorflow/addons/blob/master/tensorflow_addons/optimizers/average_wrapper.py#L93
 
         Args:
             optimizer: str or `tf.keras.optimizers.Optimizer` that will be
                 used to compute and apply gradients.
             accum_steps: int > 0. Update gradient in every accumulation steps.
             reduction: str. Which gradient reduction method to use. Defaults to 'SUM'.
             name: Optional name for the operations created when applying
@@ -135,38 +160,65 @@
         """
         self.optimizer = tf.keras.optimizers.get(optimizer)
         self.accum_steps = accum_steps
         self.reduction = reduction
         super().__init__(name, **kwargs)
 
     def _create_slots(self, var_list):
+        """Creates slots for optimizer gradients.
+        
+        Args:
+            List of trainable variables.
+        """
         self.optimizer._create_slots(var_list=var_list)
         for var in var_list:
             self.add_slot(var, "ga")
 
         self._gradients = [self.get_slot(var, "ga") for var in var_list]
 
     @property
-    def gradients(self):
-        """The accumulated gradients on the current replica."""
+    def gradients(self):  # pragma: no cover
+        """The accumulated gradients on the current replica.
+        
+        Returns:
+            Current gradients in optimizer.
+        """
         if not self._gradients:
             raise ValueError(
                 "The accumulator should be called first to initialize the gradients"
             )
         return list(
             gradient.read_value() if gradient is not None else gradient
             for gradient in self._gradients
         )
 
     def apply_gradients(self, grads_and_vars, name=None, **kwargs):
+        """Updates weights using gradients.
+        
+        Args:
+            grads_and_vars: dict containing variables and corresponding gradients.
+            name: name to set when applying gradients.
+            **kwargs: keyword arguments.
+        Return:
+            Updated weights.
+        """
         self.optimizer._iterations = self.iterations
         return super().apply_gradients(grads_and_vars, name, **kwargs)
 
     @tf.function
-    def _resource_apply_dense(self, grad, var, apply_state=None):
+    def _resource_apply_dense(self, grad, var, apply_state=None):  # pragma: no cover
+        """Performs gradient update on dense tensor.
+        
+        Args:
+            grad: current gradient.
+            var: current variable.
+            apply_state: whether to apply X.
+        Returns:
+            apply_op.
+        """
         accum_gradient = self.get_slot(var, "ga")
 
         if accum_gradient is not None and grad is not None:
             if self.reduction == "MEAN":
                 grad /= tf.cast(self.accum_steps, grad.dtype)
 
             accum_gradient.assign_add(
@@ -178,83 +230,142 @@
                 train_op = self.optimizer._resource_apply_dense(
                     accum_gradient.read_value(), var, apply_state=apply_state
                 )
             else:
                 train_op = self.optimizer._resource_apply_dense(
                     accum_gradient.read_value(), var
                 )
+
             reset_op = accum_gradient.assign(
-                        tf.zeros_like(accum_gradient),
-                        use_locking=self._use_locking,
-                        read_value=False,
-                    )
+                tf.zeros_like(accum_gradient),
+                use_locking=self._use_locking,
+                read_value=False,
+            )
+
             return tf.group(train_op, reset_op)
 
         apply_op = tf.cond(
             (self.iterations + 1) % self.accum_steps == 0, _apply, lambda: tf.no_op()
         )
         return apply_op
 
     @tf.function
-    def _resource_apply_sparse(self, grad, var, indices, apply_state):
+    def _resource_apply_sparse(self, grad, var, indices, apply_state=None):  # pragma: no cover
+        """Performs gradient update on sparse tensor.
+        
+        Args:
+            grad: current gradient.
+            var: current variable.
+            indices: relevant indices to be used for masking the sparse tensor during update.
+        Returns:
+            apply_op.
+        """
+        
         accum_gradient = self.get_slot(var, "ga")
+        
         if accum_gradient is not None and grad is not None:
+            if self.reduction == "MEAN":
+                grad /= tf.cast(self.accum_steps, grad.dtype)
+
             self._resource_scatter_add(accum_gradient, indices, grad)
 
         def _apply():
             if "apply_state" in self.optimizer._sparse_apply_args:
                 train_op = self.optimizer._resource_apply_sparse(
                     accum_gradient.sparse_read(indices),
                     var,
                     indices,
                     apply_state=apply_state,
                 )
             else:
                 train_op = self.optimizer._resource_apply_sparse(
                     accum_gradient.sparse_read(indices), var, indices
                 )
+
             reset_op = accum_gradient.assign(
-                        tf.zeros_like(accum_gradient),
-                        use_locking=self._use_locking,
-                        read_value=False,
-                    )
+                tf.zeros_like(accum_gradient),
+                use_locking=self._use_locking,
+                read_value=False,
+            )
+
             return tf.group(train_op, reset_op)
 
         apply_op = tf.cond(
             (self.iterations + 1) % self.accum_steps == 0, _apply, lambda: tf.no_op()  # tf.no_op: Does nothing - placeholder
         )
         return apply_op
 
-    def reset(self):
-        """Resets the accumulated gradients on the current replica."""
-        assign_ops = []
-        if not self._gradients:
-            return assign_ops
+    @tf.function
+    def _resource_apply_sparse_duplicate_indices(self, grad, var, indices, apply_state=None):  # pragma: no cover
+        """Performs gradient update on sparse tensor.
+        
+        Args:
+            grad: current gradient.
+            var: current variable.
+            indices: relevant indices to be used for masking the sparse tensor during update.
+        Returns:
+            apply_op.
+        """
+        
+        accum_gradient = self.get_slot(var, "ga")
+        
+        if accum_gradient is not None and grad is not None:
+            if self.reduction == "MEAN":
+                grad /= tf.cast(self.accum_steps, grad.dtype)
+
+            self._resource_scatter_add(accum_gradient, indices, grad)
 
-        for gradient in self._gradients:
-            if gradient is not None:
-                assign_ops.append(
-                    gradient.assign(
-                        tf.zeros_like(gradient),
-                        use_locking=self._use_locking,
-                        read_value=False,
-                    )
+        def _apply():
+            if "apply_state" in self.optimizer._sparse_apply_args:
+                train_op = self.optimizer._resource_apply_sparse_duplicate_indices(
+                    accum_gradient.sparse_read(indices),
+                    var,
+                    indices,
+                    apply_state=apply_state,
+                )
+            else:
+                train_op = self.optimizer._resource_apply_sparse_duplicate_indices(
+                    accum_gradient.sparse_read(indices),
+                    var,
+                    indices,
                 )
 
-        return tf.group(assign_ops)
+            reset_op = accum_gradient.assign(
+                tf.zeros_like(accum_gradient),
+                use_locking=self._use_locking,
+                read_value=False,
+            )
+
+            return tf.group(train_op, reset_op)
+
+        apply_op = tf.cond(
+            (self.iterations + 1) % self.accum_steps == 0, _apply, lambda: tf.no_op()  # tf.no_op: Does nothing - placeholder
+        )
+        return apply_op
 
     @property
-    def learning_rate(self):
+    def learning_rate(self):  # pragma: no cover
+        """Returns the learning rate of the optimizer.
+        
+        Returns:
+            learning rate of optimizer.
+        """
         return self.optimizer._get_hyper("learning_rate")
 
     @learning_rate.setter
-    def learning_rate(self, learning_rate):
+    def learning_rate(self, learning_rate):  # pragma: no cover
+        """Sets the learning rate of the optimizer.
+        
+        Args:
+            learning_rate: which learning rate to set in the optimizer.
+        """
         self.optimizer._set_hyper("learning_rate", learning_rate)
 
     def get_config(self):
+        """Returns the configuration as dict."""
         config = {
             "optimizer": tf.keras.optimizers.get(self.optimizer),
             "accum_steps": self.accum_steps,
             "reduction": self.reduction,
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
```

### Comparing `gradient-accumulator-0.3.2/gradient_accumulator/agc.py` & `gradient-accumulator-0.4.0/gradient_accumulator/agc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,37 @@
-""" An implementation of Adaptive Gradient Clipping
-@article{brock2021high,
-  author={Andrew Brock and Soham De and Samuel L. Smith and Karen Simonyan},
-  title={High-Performance Large-Scale Image Recognition Without Normalization},
-  journal={arXiv preprint arXiv:},
-  year={2021}
-}
-Code references:
-  * Official JAX implementation (paper authors): https://github.com/deepmind/deepmind-research/tree/master/nfnets
-  * Ross Wightman's implementation https://github.com/rwightman/pytorch-image-models/blob/master/timm/utils/agc.py
-"""
 import tensorflow as tf
 
 
 # implementation from: https://github.com/sayakpaul/Adaptive-Gradient-Clipping/blob/main/agc.py
 def compute_norm(x, axis, keepdims):
+    """
+    Computes the euclidean norm of a tensor :math:`x`.
+
+    Args:
+        x: input tensor.
+        axis: which axis to compute norm across.
+        keepdims: whether to keep dimension after applying along axis.
+    
+    Returns:
+        Euclidean norm.
+    """
     return tf.math.reduce_sum(x ** 2, axis=axis, keepdims=keepdims) ** 0.5
 
 
 def unitwise_norm(x):
+    """
+    Wrapper class which dynamically sets `axis` and `keepdims` given an
+    input `x` for calculating euclidean norm.
+
+    Args:
+        x: input tensor.
+
+    Returns:
+        Euclidean norm.
+    """
     if len(x.get_shape()) <= 1:  # Scalars and vectors
         axis = None
         keepdims = False
     elif len(x.get_shape()) in [2, 3]:  # Linear layers of shape IO or multihead linear
         axis = 0
         keepdims = True
     elif len(x.get_shape()) == 4:  # Conv kernels of shape HWIO
@@ -31,15 +41,30 @@
         axis = [0, 1, 2, 3]
         keepdims = True
     else:
         raise ValueError(f"Got a parameter with shape not in [1, 2, 4, 5]! {x}")
     return compute_norm(x, axis, keepdims)
 
 
-def adaptive_clip_grad(parameters, gradients, clip_factor=0.01, eps=1e-3):
+def adaptive_clip_grad(parameters, gradients, clip_factor: float = 0.01, eps: float = 1e-3):
+    """
+    Performs adaptive gradient clipping on a given set of parameters and gradients.
+
+    * Official JAX implementation (paper authors): https://github.com/deepmind/deepmind-research/tree/master/nfnets
+    * Ross Wightman's implementation https://github.com/rwightman/pytorch-image-models/blob/master/timm/utils/agc.py
+
+    Args:
+        parameters: Which parameters to apply method on.
+        gradients: Which gradients to apply clipping on.
+        clip_factor: Sets upper limit for gradient clipping.
+        eps: Epsilon - small number in :math:`max()` to avoid zero norm and preserve numerical stability.
+    
+    Returns:
+        Updated gradients after gradient clipping.
+    """
     new_grads = []
     for (params, grads) in zip(parameters, gradients):
         p_norm = unitwise_norm(params)
         max_norm = tf.math.maximum(p_norm, eps) * clip_factor
         grad_norm = unitwise_norm(grads)
         clipped_grad = grads * (max_norm / tf.math.maximum(grad_norm, 1e-6))
         new_grad = tf.where(grad_norm < max_norm, grads, clipped_grad)
```

### Comparing `gradient-accumulator-0.3.2/setup.py` & `gradient-accumulator-0.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gradient-accumulator",
-    version="0.3.2",
-    author="André Pedersen and David Bouget",
+    version="0.4.0",
+    author="André Pedersen and David Bouget and Javier Pérez de Frutos",
     author_email="andrped94@gmail.com",
     description="Package for gradient accumulation in TensorFlow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/andreped/GradientAccumulator",
-    packages=setuptools.find_packages(exclude=('tests', 'notebooks')),
+    packages=setuptools.find_packages(exclude=('tests', 'notebooks', 'assets', 'docs')),
     install_requires=[
-        "tensorflow"
+        "tensorflow",
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
```

