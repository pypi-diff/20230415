# Comparing `tmp/transformers_gradients-0.0.6.tar.gz` & `tmp/transformers_gradients-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformers_gradients-0.0.6.tar", last modified: Thu Apr 13 18:05:24 2023, max compression
+gzip compressed data, was "transformers_gradients-0.0.7.tar", last modified: Sat Apr 15 18:28:54 2023, max compression
```

## Comparing `transformers_gradients-0.0.6.tar` & `transformers_gradients-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0    48165 2023-04-13 18:05:13.636379 transformers_gradients-0.0.6/Readme.md
--rw-r--r--   0        0        0     4429 2023-04-13 18:05:13.636379 transformers_gradients-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      357 2023-04-13 18:05:13.640379 transformers_gradients-0.0.6/src/transformers_gradients/__init__.py
--rw-r--r--   0        0        0     5241 2023-04-13 18:05:13.640379 transformers_gradients-0.0.6/src/transformers_gradients/config.py
--rw-r--r--   0        0        0     7351 2023-04-13 18:05:13.640379 transformers_gradients-0.0.6/src/transformers_gradients/plotting.py
--rw-r--r--   0        0        0       64 2023-04-13 18:05:13.640379 transformers_gradients-0.0.6/src/transformers_gradients/py.typed
--rw-r--r--   0        0        0        0 2023-04-13 18:05:13.640379 transformers_gradients-0.0.6/src/transformers_gradients/text_classification/__init__.py
--rw-r--r--   0        0        0    17328 2023-04-13 18:05:13.640379 transformers_gradients-0.0.6/src/transformers_gradients/text_classification/explanation_func.py
--rw-r--r--   0        0        0     2610 2023-04-13 18:05:13.640379 transformers_gradients-0.0.6/src/transformers_gradients/text_classification/explanation_func.pyi
--rw-r--r--   0        0        0     1179 2023-04-13 18:05:13.640379 transformers_gradients-0.0.6/src/transformers_gradients/types.py
--rw-r--r--   0        0        0     1059 2023-04-13 18:05:13.640379 transformers_gradients-0.0.6/src/transformers_gradients/util.py
--rw-r--r--   0        0        0    49423 1970-01-01 00:00:00.000000 transformers_gradients-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     8893 2023-04-15 18:28:44.676173 transformers_gradients-0.0.7/Readme.md
+-rw-r--r--   0        0        0     4439 2023-04-15 18:28:44.676173 transformers_gradients-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      597 2023-04-15 18:28:44.676173 transformers_gradients-0.0.7/src/transformers_gradients/__init__.py
+-rw-r--r--   0        0        0     3135 2023-04-15 18:28:44.676173 transformers_gradients-0.0.7/src/transformers_gradients/functions.py
+-rw-r--r--   0        0        0      792 2023-04-15 18:28:44.676173 transformers_gradients-0.0.7/src/transformers_gradients/logging_utils.py
+-rw-r--r--   0        0        0     2690 2023-04-15 18:28:44.676173 transformers_gradients-0.0.7/src/transformers_gradients/model_utils.py
+-rw-r--r--   0        0        0     7351 2023-04-15 18:28:44.676173 transformers_gradients-0.0.7/src/transformers_gradients/plotting.py
+-rw-r--r--   0        0        0       64 2023-04-15 18:28:44.676173 transformers_gradients-0.0.7/src/transformers_gradients/py.typed
+-rw-r--r--   0        0        0        0 2023-04-15 18:28:44.676173 transformers_gradients-0.0.7/src/transformers_gradients/text_classification/__init__.py
+-rw-r--r--   0        0        0    16496 2023-04-15 18:28:44.676173 transformers_gradients-0.0.7/src/transformers_gradients/text_classification/huggingface.py
+-rw-r--r--   0        0        0     8777 2023-04-15 18:28:44.676173 transformers_gradients-0.0.7/src/transformers_gradients/text_classification/tensor_rt.py
+-rw-r--r--   0        0        0     5775 2023-04-15 18:28:44.676173 transformers_gradients-0.0.7/src/transformers_gradients/types.py
+-rw-r--r--   0        0        0     1677 2023-04-15 18:28:44.676173 transformers_gradients-0.0.7/src/transformers_gradients/util.py
+-rw-r--r--   0        0        0    10161 1970-01-01 00:00:00.000000 transformers_gradients-0.0.7/PKG-INFO
```

### Comparing `transformers_gradients-0.0.6/pyproject.toml` & `transformers_gradients-0.0.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "transformers_gradients"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.6"  # Required
+version = "0.0.7"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Gradient-based XAI methods for TensorFlow transformers."  # Optional
 
 # This is an optional longer description of your project that represents
@@ -87,17 +87,17 @@
 # This field lists other packages that your project depends on to run.
 # Any package you put here will be installed by pip when your project is
 # installed, so they must be valid existing projects.
 #
 # For an analysis of this field vs pip's requirements files see:
 # https://packaging.python.org/discussions/install-requires-vs-requirements/
 dependencies = [
-    "tensorflow >= 2.12.0; sys_platform != 'darwin'",
-    "tensorflow_macos >= 2.12.0; sys_platform == 'darwin'",
-    "tensorflow_probability"
+    "tensorflow >= 2.10.0; sys_platform != 'darwin'",
+    "tensorflow_macos >= 2.10.0; sys_platform == 'darwin'",
+    "tensorflow_probability >= 0.18.0"
 ]
 [project.optional-dependencies] # Optional
 transformers = [
     "transformers >= 4.27.4",
 ]
 test = [
     "pytest",
```

### Comparing `transformers_gradients-0.0.6/src/transformers_gradients/config.py` & `transformers_gradients-0.0.7/src/transformers_gradients/types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,112 @@
-from typing import NamedTuple, Union, Callable
-import tensorflow as tf
+from __future__ import annotations
+
+from typing import (
+    Callable,
+    Protocol,
+    overload,
+    runtime_checkable,
+    Tuple,
+    List,
+    Literal,
+    NamedTuple,
+)
 
+import tensorflow as tf
+from tensorflow.python.trackable.data_structures import ListWrapper
+from transformers import TFPreTrainedModel, PreTrainedTokenizerBase
 
-from transformers_gradients.types import BaselineFn, ExplainFn, ApplyNoiseFn
-from transformers_gradients.util import is_xla_compatible_platform
+BaselineFn = Callable[[tf.Tensor], tf.Tensor]
+Explanation = Tuple[List[str], tf.Tensor]
+ApplyNoiseFn = Callable[[tf.Tensor, tf.Tensor], tf.Tensor]
+BaselineExplainFn = Literal["GradNorm", "GradXInput", "IntGrad"]
+
+
+@runtime_checkable
+class ModelFn(Protocol):
+    def __call__(
+        self, *, inputs_embeds: tf.Tensor, attention_mask: tf.Tensor
+    ) -> Mapping[str, tf.Tensor]:
+        ...
+
+
+@runtime_checkable
+class UserObject(Protocol):
+    signatures: Mapping[str, ModelFn]
+    variables: ListWrapper[tf.Variable]
+
+
+@runtime_checkable
+class ExplainFn(Protocol):
+    @overload
+    def __call__(
+        self,
+        model: TFPreTrainedModel,
+        x_batch: tf.Tensor,
+        y_batch: tf.Tensor,
+        attention_mask: tf.Tensor | None,
+        tokenizer: None = None,
+        *args,
+        **kwargs,
+    ) -> tf.Tensor:
+        ...
+
+    @overload
+    def __call__(
+        self,
+        model: TFPreTrainedModel,
+        x_batch: List[str],
+        y_batch: tf.Tensor,
+        tokenizer: PreTrainedTokenizerBase,
+        *args,
+        **kwargs,
+    ) -> List[Explanation]:
+        ...
+
+    def __call__(  # type: ignore
+        self,
+        model: TFPreTrainedModel,
+        x_batch: List[str] | tf.Tensor,
+        y_batch: tf.Tensor,
+        tokenizer: PreTrainedTokenizerBase | None,
+        *args,
+        **kwargs,
+    ) -> List[Explanation] | tf.Tensor:
+        ...
 
 
 class LibConfig(NamedTuple):
-    seed: int = 42
+    prng_seed: int = 42
     log_level: str = "INFO"
+    log_format: str = "%(asctime)s:[%(filename)s:%(lineno)s->%(funcName)s()]:%(levelname)s: %(message)s"
+
 
+class ModelConfig(tf.experimental.ExtensionType):
+    model_family: str
+    num_hidden_layers: int
+    embeddings_dim: int
 
-class IntGradConfig(NamedTuple):
+
+class IntGradConfig(tf.experimental.ExtensionType):
     """
     num_steps:
         Number of interpolated samples, which should be generated, default=10.
     baseline_fn:
         Function used to created baseline values, by default will create zeros tensor. Alternatively, e.g.,
         embedding for [UNK] token could be used.
     batch_interpolated_inputs:
         Indicates if interpolated inputs should be stacked into 1 bigger batch.
         This speeds up the explanation, however can be very memory intensive.
     """
 
     num_steps: int = 10
-    baseline_fn: BaselineFn = tf.function(
-        reduce_retracing=True, jit_compile=is_xla_compatible_platform()
-    )(lambda x: tf.zeros_like(x, dtype=x.dtype))
     batch_interpolated_inputs: bool = True
 
 
-class NoiseGradConfig(NamedTuple):
+class NoiseGradConfig(tf.experimental.ExtensionType):
     """
     mean:
         Mean of normal distribution, from which noise applied to model's weights is sampled, default=1.0.
     std:
         Standard deviation of normal distribution, from which noise applied to model's weights is sampled, default=0.2.
     n:
         Number of times noise is applied to weights, default=10.
@@ -46,21 +118,17 @@
     seed:
         PRNG seed used for noise generating distributions.
     """
 
     n: int = 10
     mean: float = 1.0
     std: float = 0.0055
-    explain_fn: Union[ExplainFn, str] = "IntGrad"
-    noise_fn: ApplyNoiseFn = tf.function(
-        reduce_retracing=True, jit_compile=is_xla_compatible_platform()
-    )(lambda a, b: a * b)
 
 
-class SmoothGradConfing(NamedTuple):
+class SmoothGradConfing(tf.experimental.ExtensionType):
     """
     mean:
         Mean of normal distribution, from which noise applied to input embeddings is sampled, default=0.0.
     std:
         Standard deviation of normal distribution, from which noise applied to input embeddings is sampled, default=0.4.
     n:
         Number of times noise is applied to input embeddings, default=10
@@ -72,21 +140,17 @@
     seed:
         PRNG seed used for noise generating distributions.
     """
 
     n: int = 10
     mean: float = 1.0
     std: float = 0.0055
-    explain_fn: Union[ExplainFn, str] = "IntGrad"
-    noise_fn: ApplyNoiseFn = tf.function(
-        reduce_retracing=True, jit_compile=is_xla_compatible_platform()
-    )(lambda a, b: a * b)
 
 
-class NoiseGradPlusPlusConfig(NamedTuple):
+class NoiseGradPlusPlusConfig(tf.experimental.ExtensionType):
     """
     mean:
         Mean of normal distribution, from which noise applied to model's weights is sampled, default=1.0.
     sg_mean:
         Mean of normal distribution, from which noise applied to input embeddings is sampled, default=0.0.
     std:
         Standard deviation of normal distribution, from which noise applied to model's weights is sampled, default=0.2.
@@ -108,38 +172,15 @@
 
     n: int = 10
     m: int = 10
     mean: float = 1.0
     sg_mean: float = 0.0
     std: float = 0.0055
     sg_std: float = 0.05
-    explain_fn: Union[ExplainFn, str] = "IntGrad"
-    noise_fn: ApplyNoiseFn = tf.function(
-        reduce_retracing=True, jit_compile=is_xla_compatible_platform()
-    )(lambda a, b: a * b)
-
-
-def update_config(**kwargs):
-    config = LibConfig()
-    tf.random.set_seed(config.seed)
-
-
-def resolve_baseline_explain_fn(explain_fn):
-    if isinstance(explain_fn, Callable):
-        return explain_fn  # type: ignore
-
-    from transformers_gradients.text_classification.explanation_func import (
-        integrated_gradients,
-        gradient_norm,
-        gradient_x_input,
-    )
-
-    method_mapping = {
-        "IntGrad": integrated_gradients,
-        "GradNorm": gradient_norm,
-        "GradXInput": gradient_x_input,
-    }
-    if explain_fn not in method_mapping:
-        raise ValueError(
-            f"Unknown XAI method {explain_fn}, supported are {list(method_mapping.keys())}"
-        )
-    return method_mapping[explain_fn]
+
+
+class LimeConfig(tf.experimental.ExtensionType):
+    alpha: float = 1.0
+    solver: str = "cholesky"
+    num_samples: int = 1000
+    mask_token: str = "[UNK]"
+    distance_scale: float = 100.0
```

### Comparing `transformers_gradients-0.0.6/src/transformers_gradients/plotting.py` & `transformers_gradients-0.0.7/src/transformers_gradients/plotting.py`

 * *Files identical despite different names*

### Comparing `transformers_gradients-0.0.6/src/transformers_gradients/text_classification/explanation_func.py` & `transformers_gradients-0.0.7/src/transformers_gradients/text_classification/huggingface.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,65 +1,76 @@
 from __future__ import annotations
 
-import gc
 from functools import wraps, partial
-from operator import itemgetter
-from typing import List
+from typing import List, Callable
 
 import tensorflow as tf
 import tensorflow_probability as tfp
 from tensorflow_probability.python.distributions.normal import Normal
 from transformers import TFPreTrainedModel, PreTrainedTokenizerBase
 
-from transformers_gradients.config import (
+from transformers_gradients.functions import (
+    logits_for_labels,
+    interpolate_inputs,
+    zeros_baseline,
+    multiplicative_noise,
+    pseudo_interpolate,
+    broadcast_expand_dims,
+)
+from transformers_gradients.types import (
     IntGradConfig,
     NoiseGradPlusPlusConfig,
     NoiseGradConfig,
     SmoothGradConfing,
-    resolve_baseline_explain_fn,
+    BaselineFn,
+    BaselineExplainFn,
+    ExplainFn,
+    ApplyNoiseFn,
 )
 from transformers_gradients.util import (
     value_or_default,
-    is_xla_compatible_platform,
-    get_input_ids,
+    encode_inputs,
     as_tensor,
+    tensor_inputs,
 )
 
 
 def plain_text_hook(func):
     @wraps(func)
     def wrapper(
         model: TFPreTrainedModel,
         x_batch: List[str] | tf.Tensor,
         y_batch: tf.Tensor,
+        attention_mask: tf.Tensor | None = None,
         tokenizer: PreTrainedTokenizerBase | None = None,
         **kwargs,
     ):
-        if isinstance(x_batch[0], str):
-            input_ids, predict_kwargs = get_input_ids(tokenizer, x_batch)
-            embeddings = model.get_input_embeddings()(input_ids)
-            scores = func(
-                model, embeddings, as_tensor(y_batch), **kwargs, **predict_kwargs
+        if not isinstance(x_batch[0], str):
+            return func(
+                model, as_tensor(x_batch), as_tensor(y_batch), attention_mask, **kwargs
             )
-            return [
-                (tokenizer.convert_ids_to_tokens(list(i)), j)
-                for i, j in zip(input_ids, scores)
-            ]
-        else:
-            return func(model, as_tensor(x_batch), as_tensor(y_batch), **kwargs)
+
+        input_ids, attention_mask = encode_inputs(tokenizer, x_batch)
+        embeddings = model.get_input_embeddings()(input_ids)
+        scores = func(model, embeddings, as_tensor(y_batch), attention_mask, **kwargs)
+        return [
+            (tokenizer.convert_ids_to_tokens(list(i)), j)
+            for i, j in zip(input_ids, scores)
+        ]
 
     return wrapper
 
 
 @plain_text_hook
+@tensor_inputs
 def gradient_norm(
     model: TFPreTrainedModel,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
-    **kwargs,
+    attention_mask: tf.Tensor | None = None,
 ) -> tf.Tensor:
     """
     A baseline GradientNorm text-classification explainer.
     The implementation is based on https://github.com/PAIR-code/lit/blob/main/lit_nlp/components/gradient_maps.py#L38.
     GradientNorm explanation algorithm is:
         - Convert inputs to models latent representations.
         - Execute forwards pass
@@ -76,38 +87,38 @@
     model:
         A model, which is subject to explanation.
     x_batch:
         A batch of plain text inputs or their embeddings, which are subjects to explanation.
     y_batch:
         A batch of labels, which are subjects to explanation.
 
-    kwargs:
-        If x_batch is embeddings, kwargs can be used to pass, additional forward pass kwargs, e.g., attention mask.
-
     Returns
     -------
     a_batch:
         List of tuples, where 1st element is tokens and 2nd is the scores assigned to the tokens.
 
     """
     with tf.GradientTape() as tape:
         tape.watch(x_batch)
-        logits = model(None, inputs_embeds=x_batch, training=False, **kwargs).logits
+        logits = model(
+            None, inputs_embeds=x_batch, training=False, attention_mask=attention_mask
+        ).logits
         logits_for_label = logits_for_labels(logits, y_batch)
 
     grads = tape.gradient(logits_for_label, x_batch)
     return tf.linalg.norm(grads, axis=-1)
 
 
 @plain_text_hook
+@tensor_inputs
 def gradient_x_input(
     model: TFPreTrainedModel,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
-    **kwargs,
+    attention_mask: tf.Tensor | None = None,
 ) -> tf.Tensor:
     """
     A baseline GradientXInput text-classification explainer.
      The implementation is based on https://github.com/PAIR-code/lit/blob/main/lit_nlp/components/gradient_maps.py#L108.
      GradientXInput explanation algorithm is:
         - Convert inputs to models latent representations.
         - Execute forwards pass
@@ -124,38 +135,40 @@
     ----------
     model:
         A model, which is subject to explanation.
     x_batch:
         A batch of plain text inputs or their embeddings, which are subjects to explanation.
     y_batch:
         A batch of labels, which are subjects to explanation.
-    kwargs:
-        If x_batch is embeddings, kwargs can be used to pass, additional forward pass kwargs, e.g., attention mask.
 
     Returns
     -------
     a_batch:
         List of tuples, where 1st element is tokens and 2nd is the scores assigned to the tokens.
 
     """
     with tf.GradientTape() as tape:
         tape.watch(x_batch)
-        logits = model(None, inputs_embeds=x_batch, training=False, **kwargs).logits
+        logits = model(
+            None, inputs_embeds=x_batch, training=False, attention_mask=attention_mask
+        ).logits
         logits_for_label = logits_for_labels(logits, y_batch)
     grads = tape.gradient(logits_for_label, x_batch)
     return tf.math.reduce_sum(x_batch * grads, axis=-1)
 
 
 @plain_text_hook
+@tensor_inputs
 def integrated_gradients(
     model: TFPreTrainedModel,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
+    attention_mask: tf.Tensor | None = None,
     config: IntGradConfig | None = None,
-    **kwargs,
+    baseline_fn: BaselineFn | None = None,
 ) -> tf.Tensor:
     """
     A baseline Integrated Gradients text-classification explainer. Integrated Gradients explanation algorithm is:
         - Convert inputs to models latent representations.
         - For each x, y in x_batch, y_batch
         - Generate num_steps samples interpolated from baseline to x.
         - Execute forwards pass.
@@ -174,18 +187,14 @@
     ----------
     model:
         A model, which is subject to explanation.
     x_batch:
         A batch of plain text inputs or their embeddings, which are subjects to explanation.
     y_batch:
         A batch of labels, which are subjects to explanation.
-    config:
-
-    kwargs:
-        If x_batch is embeddings, kwargs can be used to pass, additional forward pass kwargs, e.g., attention mask.
 
     Returns
     -------
     a_batch:
         List of tuples, where 1st element is tokens and 2nd is the scores assigned to the tokens.
 
     Examples
@@ -195,99 +204,96 @@
     >>> unk_token_embedding = model.embedding_lookup([model.tokenizer.unk_token_id])[0, 0]
     >>> unknown_token_baseline_function = tf.function(lambda x: unk_token_embedding)
     >>> config = IntGradConfig(baseline_fn=unknown_token_baseline_function)
     >>> integrated_gradients(..., ..., ..., config=config)
 
     """
     config = value_or_default(config, lambda: IntGradConfig())
-    interpolated_embeddings = tf.map_fn(
-        lambda i: interpolate_inputs(
-            config.baseline_fn(i), i, tf.constant(config.num_steps)
-        ),
-        x_batch,
-    )
-    kwargs = tf.nest.map_structure(as_tensor, kwargs)
+    baseline_fn = value_or_default(baseline_fn, lambda: zeros_baseline)
+    interpolated_embeddings = interpolate_inputs(x_batch, config.num_steps, baseline_fn)
 
     if config.batch_interpolated_inputs:
         return _integrated_gradients_batched(
             model,
             interpolated_embeddings,
             y_batch,
+            attention_mask,
             tf.constant(config.num_steps),
-            **tf.nest.map_structure(as_tensor, kwargs),
         )
     else:
         return _integrated_gradients_iterative(
             model,
             interpolated_embeddings,
             y_batch,
-            **kwargs,
+            attention_mask,
         )
 
 
 @plain_text_hook
+@tensor_inputs
 def smooth_grad(
     model: TFPreTrainedModel,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
+    attention_mask: tf.Tensor | None = None,
     config: SmoothGradConfing | None = None,
-    **kwargs,
+    explain_fn: ExplainFn | BaselineExplainFn = "IntGrad",
+    noise_fn: ApplyNoiseFn | None = None,
 ) -> tf.Tensor:
     config = value_or_default(config, lambda: SmoothGradConfing())
-    explain_fn = resolve_baseline_explain_fn(config.explain_fn)
+    explain_fn = resolve_baseline_explain_fn(explain_fn)
+    apply_noise_fn = value_or_default(noise_fn, lambda: multiplicative_noise)
 
     explanations_array = tf.TensorArray(
         x_batch.dtype,
         size=config.n,
         clear_after_read=True,
         colocate_with_first_write_call=True,
     )
 
     noise_dist = Normal(config.mean, config.std)
 
     def noise_fn(x):
         noise = noise_dist.sample(tf.shape(x))
-        return config.noise_fn(x, noise)
+        return apply_noise_fn(x, noise)
 
     for n in tf.range(config.n):
         noisy_x = noise_fn(x_batch)
-        explanation = explain_fn(model, noisy_x, y_batch, **kwargs)
+        explanation = explain_fn(model, noisy_x, y_batch, attention_mask)
         explanations_array = explanations_array.write(n, explanation)
 
     scores = tf.reduce_mean(explanations_array.stack(), axis=0)
     explanations_array.close()
     return scores
 
 
 @plain_text_hook
+@tensor_inputs
 def noise_grad(
     model: TFPreTrainedModel,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
+    attention_mask: tf.Tensor | None = None,
     config: NoiseGradConfig | None = None,
-    **kwargs,
+    explain_fn: ExplainFn | BaselineExplainFn = "IntGrad",
+    noise_fn: ApplyNoiseFn | None = None,
 ) -> tf.Tensor:
     """
     NoiseGrad++ is a state-of-the-art gradient based XAI method, which enhances baseline explanation function
     by adding stochasticity to model's weights. The implementation is based
     on https://github.com/understandable-machine-intelligence-lab/NoiseGrad/blob/master/src/noisegrad.py#L80.
 
     Parameters
     ----------
     model:
         A model, which is subject to explanation.
     x_batch:
         A batch of plain text inputs or their embeddings, which are subjects to explanation.
     y_batch:
         A batch of labels, which are subjects to explanation.
-    config:
-
-    kwargs:
-        If x_batch is embeddings, kwargs can be used to pass, additional forward pass kwargs, e.g., attention mask.
-
     Returns
     -------
     a_batch:
         List of tuples, where 1st element is tokens and 2nd is the scores assigned to the tokens.
 
 
     Examples
@@ -304,55 +310,57 @@
     -------
     - https://github.com/understandable-machine-intelligence-lab/NoiseGrad/blob/master/src/noisegrad.py#L80.
     - Kirill Bykov and Anna Hedström and Shinichi Nakajima and Marina M. -C. Höhne, 2021, NoiseGrad: enhancing explanations by introducing stochasticity to model weights, https://arxiv.org/abs/2106.10185
 
     """
 
     config = value_or_default(config, lambda: NoiseGradConfig())
-    explain_fn = resolve_baseline_explain_fn(config.explain_fn)
+    explain_fn = resolve_baseline_explain_fn(explain_fn)
+    apply_noise_fn = value_or_default(noise_fn, lambda: multiplicative_noise)
     original_weights = model.weights.copy()
 
     explanations_array = tf.TensorArray(
         x_batch.dtype,
         size=config.n,
         clear_after_read=True,
         colocate_with_first_write_call=True,
     )
 
     noise_dist = Normal(config.mean, config.std)
 
     def noise_fn(x):
         noise = noise_dist.sample(tf.shape(x))
-        return config.noise_fn(x, noise)
+        return apply_noise_fn(x, noise)
 
     for n in tf.range(config.n):
         noisy_weights = tf.nest.map_structure(
             noise_fn,
             original_weights,
         )
         model.set_weights(noisy_weights)
 
-        explanation = explain_fn(model, x_batch, y_batch, **kwargs)
+        explanation = explain_fn(model, x_batch, y_batch, attention_mask)
         explanations_array = explanations_array.write(n, explanation)
 
     scores = tf.reduce_mean(explanations_array.stack(), axis=0)
-    model.set_weights(original_weights)
     explanations_array.close()
-    tf.keras.backend.clear_session()
-    gc.collect()
+    model.set_weights(original_weights)
     return scores
 
 
 @plain_text_hook
+@tensor_inputs
 def noise_grad_plus_plus(
     model: TFPreTrainedModel,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
+    attention_mask: tf.Tensor | None = None,
     config: NoiseGradPlusPlusConfig | None = None,
-    **kwargs,
+    explain_fn="IntGrad",
+    noise_fn=None,
 ) -> tf.Tensor:
     """
     NoiseGrad++ is a state-of-the-art gradient based XAI method, which enhances baseline explanation function
     by adding stochasticity to model's weights and model's inputs. The implementation is based
     on https://github.com/understandable-machine-intelligence-lab/NoiseGrad/blob/master/src/noisegrad.py#L80.
 
     Parameters
@@ -360,18 +368,14 @@
     model:
         A model, which is subject to explanation.
     x_batch:
         A batch of plain text inputs or their embeddings, which are subjects to explanation.
     y_batch:
         A batch of labels, which are subjects to explanation.
     config:
-
-    kwargs:
-        If x_batch is embeddings, kwargs can be used to pass, additional forward pass kwargs, e.g., attention mask.
-
     Returns
     -------
     a_batch:
         List of tuples, where 1st element is tokens and 2nd is the scores assigned to the tokens.
 
 
     Examples
@@ -385,62 +389,61 @@
 
     """
     config = value_or_default(config, lambda: NoiseGradPlusPlusConfig())
     sg_config = SmoothGradConfing(
         n=config.m,
         mean=config.sg_mean,
         std=config.sg_std,
-        explain_fn=config.explain_fn,
-        noise_fn=config.noise_fn,
+    )
+    sg_explain_fn = partial(
+        smooth_grad, config=sg_config, explain_fn=explain_fn, noise_fn=noise_fn
     )
     ng_config = NoiseGradConfig(
         n=config.n,
         mean=config.mean,
-        noise_fn=config.noise_fn,
-        explain_fn=partial(smooth_grad, config=sg_config),
     )
-    return noise_grad(model, x_batch, y_batch, config=ng_config, **kwargs)
+    return noise_grad(
+        model,
+        x_batch,
+        y_batch,
+        attention_mask,
+        config=ng_config,
+        explain_fn=sg_explain_fn,
+        noise_fn=noise_fn,
+    )
 
 
 # ----------------------- IntGrad ------------------------
 
 
 def _integrated_gradients_batched(
     model: TFPreTrainedModel,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
+    attention_mask: tf.Tensor,
     num_steps: tf.Tensor,
-    **kwargs,
 ) -> tf.Tensor:
+    num_steps = tf.constant(num_steps)
     shape = tf.shape(x_batch)
     batch_size = shape[0]
 
     interpolated_embeddings = tf.reshape(
         tf.cast(x_batch, dtype=tf.float32),
         [-1, shape[2], shape[3]],
     )
-
-    def pseudo_interpolate(x):
-        og_shape = tf.convert_to_tensor(tf.shape(x))
-        new_shape = tf.concat([[num_steps + 1], og_shape], axis=0)
-        x = tf.broadcast_to(x, new_shape)
-        flat_shape = tf.concat([tf.constant([-1]), og_shape[1:]], axis=0)
-        x = tf.reshape(x, flat_shape)
-        return x
-
-    interpolated_kwargs = tf.nest.map_structure(pseudo_interpolate, kwargs)
-    interpolated_y_batch = pseudo_interpolate(y_batch)
+    interpolated_y_batch = pseudo_interpolate(y_batch, num_steps)
+    interpolated_mask = pseudo_interpolate(attention_mask, num_steps)
 
     with tf.GradientTape() as tape:
         tape.watch(interpolated_embeddings)
         logits = model(
             None,
             inputs_embeds=interpolated_embeddings,
             training=False,
-            **interpolated_kwargs,
+            attention_mask=interpolated_mask,
         ).logits
         logits_for_label = logits_for_labels(logits, interpolated_y_batch)
 
     grads = tape.gradient(logits_for_label, interpolated_embeddings)
     grads_shape = tf.shape(grads)
     grads = tf.reshape(
         grads, [batch_size, num_steps + 1, grads_shape[1], grads_shape[2]]
@@ -448,44 +451,38 @@
     return tf.linalg.norm(tfp.math.trapz(grads, axis=1), axis=-1)
 
 
 def _integrated_gradients_iterative(
     model: TFPreTrainedModel,
     x_batch: tf.Tensor,
     y_batch: tf.Tensor,
-    **kwargs,
+    attention_mask: tf.Tensor,
 ) -> tf.Tensor:
     batch_size = tf.shape(x_batch)[0]
     scores = tf.TensorArray(
         x_batch.dtype,
         size=batch_size,
         clear_after_read=True,
         colocate_with_first_write_call=True,
     )
 
-    def pseudo_interpolate(x, embeds):
-        x_shape = tf.shape(x)
-        return tf.broadcast_to(x, (tf.shape(embeds)[0], *x_shape))
-
     for i in tf.range(batch_size):
         interpolated_embeddings = x_batch[i]
 
-        kwargs_i = tf.nest.map_structure(itemgetter(i), kwargs)
-
-        interpolated_kwargs = tf.nest.map_structure(
-            partial(pseudo_interpolate, embeds=interpolated_embeddings),
-            kwargs_i,
+        attention_mask_i = broadcast_expand_dims(
+            attention_mask[i], interpolated_embeddings
         )
+
         with tf.GradientTape() as tape:
             tape.watch(interpolated_embeddings)
             logits = model(
                 None,
                 inputs_embeds=interpolated_embeddings,
                 training=False,
-                **interpolated_kwargs,
+                attention_mask=attention_mask_i,
             ).logits
             logits_for_label = logits[:, y_batch[i]]
 
         grads = tape.gradient(logits_for_label, interpolated_embeddings)
         score = tf.linalg.norm(tfp.math.trapz(grads, axis=0), axis=-1)
         scores = scores.write(i, score)
 
@@ -493,36 +490,21 @@
     scores.close()
     return scores_stack
 
 
 # --------------------- utils ----------------------
 
 
-@tf.function(reduce_retracing=True, jit_compile=is_xla_compatible_platform())
-def logits_for_labels(logits: tf.Tensor, y_batch: tf.Tensor) -> tf.Tensor:
-    # Matrix with indexes like [ [0,y_0], [1, y_1], ...]
-    indexes = tf.transpose(
-        tf.stack(
-            [
-                tf.range(tf.shape(logits)[0], dtype=tf.int32),
-                tf.cast(y_batch, tf.int32),
-            ]
-        ),
-        [1, 0],
-    )
-    return tf.gather_nd(logits, indexes)
-
-
-@tf.function(reduce_retracing=True, jit_compile=is_xla_compatible_platform())
-def interpolate_inputs(
-    baseline: tf.Tensor, target: tf.Tensor, num_steps: int
-) -> tf.Tensor:
-    """Gets num_step linearly interpolated inputs from baseline to target."""
-    delta = target - baseline
-    scales = tf.linspace(0, 1, num_steps + 1)[:, tf.newaxis, tf.newaxis]
-    scales = tf.cast(scales, dtype=delta.dtype)
-    shape = tf.convert_to_tensor(
-        [num_steps + 1, tf.shape(delta)[0], tf.shape(delta)[1]]
-    )
-    deltas = scales * tf.broadcast_to(delta, shape)
-    interpolated_inputs = baseline + deltas
-    return interpolated_inputs
+def resolve_baseline_explain_fn(explain_fn):
+    if isinstance(explain_fn, Callable):
+        return explain_fn  # type: ignore
+
+    method_mapping = {
+        "IntGrad": integrated_gradients,
+        "GradNorm": gradient_norm,
+        "GradXInput": gradient_x_input,
+    }
+    if explain_fn not in method_mapping:
+        raise ValueError(
+            f"Unknown XAI method {explain_fn}, supported are {list(method_mapping.keys())}"
+        )
+    return method_mapping[explain_fn]
```

### Comparing `transformers_gradients-0.0.6/src/transformers_gradients/util.py` & `transformers_gradients-0.0.7/src/transformers_gradients/util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from __future__ import annotations
 
 import platform
+from functools import wraps
 from typing import TypeVar, Callable, Dict, List, Tuple
 
 import tensorflow as tf
 from transformers import PreTrainedTokenizerBase
 
 T = TypeVar("T")
 
 
-def get_input_ids(
+def encode_inputs(
     tokenizer: PreTrainedTokenizerBase, x_batch: List[str]
-) -> Tuple[tf.Tensor, Dict[str, tf.Tensor]]:
+) -> Tuple[tf.Tensor, tf.Tensor | None]:
     """Do batch encode, unpack input ids and other forward-pass kwargs."""
     encoded_input = tokenizer(x_batch, padding="longest", return_tensors="tf").data
-    return encoded_input.pop("input_ids"), encoded_input
+    return encoded_input.pop("input_ids"), encoded_input.get("attention_mask")
 
 
 def value_or_default(value: T | None, default_factory: Callable[[], T]) -> T:
     if value is not None:
         return value
     else:
         return default_factory()
@@ -30,7 +31,27 @@
 
 
 def as_tensor(arr) -> tf.Tensor:
     if isinstance(arr, (tf.Tensor, Callable)):  # type: ignore
         return arr
     else:
         return tf.convert_to_tensor(arr)
+
+
+def tensor_inputs(func):
+    @wraps(func)
+    def wrapper(
+        model: UserObject,
+        x_batch: tf.Tensor,
+        y_batch: tf.Tensor,
+        attention_mask: tf.Tensor | None = None,
+        **kwargs,
+    ):
+        x_batch = as_tensor(x_batch)
+        y_batch = as_tensor(y_batch)
+        attention_mask = value_or_default(
+            attention_mask, lambda: tf.ones(bounding_shape(x_batch), dtype=tf.int32)
+        )
+        attention_mask = as_tensor(attention_mask)
+        return func(model, x_batch, y_batch, attention_mask, **kwargs)
+
+    return wrapper
```

