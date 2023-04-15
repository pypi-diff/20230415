# Comparing `tmp/CoLT5-attention-0.1.6.tar.gz` & `tmp/CoLT5-attention-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.1.6.tar", last modified: Thu Mar 23 23:31:04 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.2.0.tar", last modified: Sat Apr 15 15:09:05 2023, max compression
```

## Comparing `CoLT5-attention-0.1.6.tar` & `CoLT5-attention-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 23:31:04.178679 CoLT5-attention-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 23:31:04.174679 CoLT5-attention-0.1.6/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-23 23:31:04.000000 CoLT5-attention-0.1.6/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-23 23:31:04.000000 CoLT5-attention-0.1.6/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 23:31:04.000000 CoLT5-attention-0.1.6/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-23 23:31:04.000000 CoLT5-attention-0.1.6/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-23 23:31:04.000000 CoLT5-attention-0.1.6/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-23 23:30:50.000000 CoLT5-attention-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-23 23:31:04.178679 CoLT5-attention-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-03-23 23:30:50.000000 CoLT5-attention-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 23:31:04.178679 CoLT5-attention-0.1.6/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-23 23:30:50.000000 CoLT5-attention-0.1.6/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-03-23 23:30:50.000000 CoLT5-attention-0.1.6/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-23 23:30:50.000000 CoLT5-attention-0.1.6/colt5_attention/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    16564 2023-03-23 23:30:50.000000 CoLT5-attention-0.1.6/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 23:31:04.178679 CoLT5-attention-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-03-23 23:30:50.000000 CoLT5-attention-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:09:05.364228 CoLT5-attention-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:09:05.360228 CoLT5-attention-0.2.0/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-15 15:09:05.000000 CoLT5-attention-0.2.0/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-15 15:09:05.000000 CoLT5-attention-0.2.0/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 15:09:05.000000 CoLT5-attention-0.2.0/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-15 15:09:05.000000 CoLT5-attention-0.2.0/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-15 15:09:05.000000 CoLT5-attention-0.2.0/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-15 15:08:45.000000 CoLT5-attention-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-15 15:09:05.364228 CoLT5-attention-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-04-15 15:08:45.000000 CoLT5-attention-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:09:05.364228 CoLT5-attention-0.2.0/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-15 15:08:45.000000 CoLT5-attention-0.2.0/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-15 15:08:45.000000 CoLT5-attention-0.2.0/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-15 15:08:45.000000 CoLT5-attention-0.2.0/colt5_attention/sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-04-15 15:08:45.000000 CoLT5-attention-0.2.0/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 15:09:05.364228 CoLT5-attention-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-15 15:08:45.000000 CoLT5-attention-0.2.0/setup.py
```

### Comparing `CoLT5-attention-0.1.6/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.2.0/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.1.6
+Version: 0.2.0
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.1.6/LICENSE` & `CoLT5-attention-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.1.6/PKG-INFO` & `CoLT5-attention-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.1.6
+Version: 0.2.0
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.1.6/README.md` & `CoLT5-attention-0.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ## CoLT5 Attention - Pytorch
 
 Implementation of the conditionally routed efficient attention in the proposed <a href="https://arxiv.org/abs/2303.09752">CoLT5</a> architecture, in Pytorch.
 
 Besides their use of coordinate descent from <a href="https://arxiv.org/abs/2211.01267">this paper</a> (main algorithm originally from <a href="https://arxiv.org/abs/1502.04759">Wright et al</a>), will also add two other approaches, one based on cumulative softmax, the other gumbel sinkhorn (optimal transport).
 
-Update: unsure of how the routing normalized scores for the key-values are used. Did some improvising there, multiplying it into the projected values, but if you think you know the answer, please open an issue
+Update: unsure of how the routing normalized scores for the key-values are used. Did some improvising there, <a href="https://github.com/lucidrains/CoLT5-attention/blob/main/colt5_attention/transformer_block.py#L86">scaling the projected values</a>, but if you think you know the answer, please open an issue
 
 ## Appreciation
 
 - <a href="https://stability.ai/">Stability.ai</a> for the generous sponsorship to work on cutting edge artificial intelligence research
 
 ## Install
 
@@ -78,19 +78,55 @@
     num_heavy_attn_tokens_kv = 1024,
     router_type = 'coor_descent'  # you have your choice of coordinate descent, as in paper - or 'sinkhorn' or 'cum_softmax'
 )
 
 block_out = block(tokens, mask = mask) # (2, 32768, 512)
 ```
 
+Also included a variation of the conditionally routed attention for cross attention, to be tried with long context memories in a transformer-xl
+
+```python
+import torch
+from colt5_attention import ConditionalRoutedCrossAttention
+
+# mock input, let us say it is a transformer of 1024 length attending to 1 million context past memories
+
+tokens = torch.randn(2, 1024, 512).cuda()
+tokens_mask = torch.ones(2, 1024).bool().cuda()
+
+memories = torch.randn(2, int(1e6), 512).cuda()
+memories_mask = torch.ones(2, int(1e6)).bool().cuda()
+
+# conditionally routed cross attention
+
+cross_attn = ConditionalRoutedCrossAttention(
+    dim = 512,
+    dim_head = 64,
+    heads = 8,
+    num_tokens_q = 512,   # only 512 routed from 1024
+    num_tokens_kv = 1024, # only 1024 routed from 1 million
+).cuda()
+
+cross_attn_out = cross_attn(
+    tokens,
+    context = memories,
+    mask = tokens_mask,
+    context_mask = memories_mask
+)
+
+cross_attn_out.shape # (2, 1024, 512) - same as tokens
+```
+
 ## Todo
 
 - [x] add the coordinate descent method as another router
+- [x] figure out if it can be done autoregressively and try it out - moving to <a href="https://github.com/lucidrains/coordinate-descent-attention">this repo</a>
+
 - [ ] for variable sequence lengths, allow for setting k as a function of sequence lengths per sample in batch
-- [ ] figure out if it can be done autoregressively and try it out
+- [ ] create a variant of CoLT5 for high resolution feature maps (image attention) - then try out for diffusion
 
 ## Citations
 
 ```bibtex
 @inproceedings{Ainslie2023CoLT5FL,
     title   = {CoLT5: Faster Long-Range Transformers with Conditional Computation},
     author  = {Joshua Ainslie and Tao Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit Sanghai},
```

#### html2text {}

```diff
@@ -1,44 +1,57 @@
 [./colt5.png] ## CoLT5 Attention - Pytorch Implementation of the conditionally
 routed efficient attention in the proposed CoLT5 architecture, in Pytorch.
 Besides their use of coordinate descent from this_paper (main algorithm
 originally from Wright_et_al), will also add two other approaches, one based on
 cumulative softmax, the other gumbel sinkhorn (optimal transport). Update:
 unsure of how the routing normalized scores for the key-values are used. Did
-some improvising there, multiplying it into the projected values, but if you
-think you know the answer, please open an issue ## Appreciation - Stability.ai
-for the generous sponsorship to work on cutting edge artificial intelligence
-research ## Install ```bash $ pip install colt5-attention ``` ## Usage
-```python import torch from colt5_attention import
-( ConditionalRoutedFeedForward, ConditionalRoutedAttention,
-ConditionalRoutedTransformerBlock ) # mock input, say it is 32768 length tokens
-= torch.randn(2, 32768, 512) mask = torch.ones(2, 32768).bool() # can handle
-variable lengthed sequences # feedforward ff = ConditionalRoutedFeedForward
-( dim = 512, light_ff_mult = 0.5, # hidden dimension ratio of light branch
-heavy_ff_mult = 4, # hidden dimension ratio of heavy branch num_heavy_tokens =
-1024 # heavy branch receives only 1024 routed tokens of 32768 ) ff_out = ff
-(tokens, mask = mask) # (2, 32768, 512) - light and heavy branch summed #
-attention attn = ConditionalRoutedAttention( dim = 512, light_dim_head = 64, #
-attention head dimension of light branch light_heads = 8, # number of attention
-heads for light branch light_window_size = 128, # local attention receptive
-field for light heavy_dim_head = 64, # attention head dimension of heavy branch
-heavy_heads = 8, # number of attention heads for heavy branch
-num_heavy_tokens_q = 1024, # heavy branch receives only 1024 routed tokens of
-32768 num_heavy_tokens_kv = 1024 # heavy branch receives only 1024 routed
-tokens of 32768 ) attn_out = attn(tokens, mask = mask) # (2, 32768, 512) -
-light and heavy branch summed # both attention and feedforward with residual #
-the complete transformer block # a stack of these would constitute the encoder
-of CoLT5 block = ConditionalRoutedTransformerBlock( dim = 512, light_dim_head =
-64, light_heads = 8, light_window_size = 128, heavy_dim_head = 64, heavy_heads
-= 8, light_ff_mult = 0.5, heavy_ff_mult = 4, num_heavy_ff_tokens = 1024,
-num_heavy_attn_tokens_q = 1024, num_heavy_attn_tokens_kv = 1024, router_type =
-'coor_descent' # you have your choice of coordinate descent, as in paper - or
-'sinkhorn' or 'cum_softmax' ) block_out = block(tokens, mask = mask) # (2,
-32768, 512) ``` ## Todo - [x] add the coordinate descent method as another
-router - [ ] for variable sequence lengths, allow for setting k as a function
-of sequence lengths per sample in batch - [ ] figure out if it can be done
-autoregressively and try it out ## Citations ```bibtex @inproceedings
-{Ainslie2023CoLT5FL, title = {CoLT5: Faster Long-Range Transformers with
-Conditional Computation}, author = {Joshua Ainslie and Tao Lei and Michiel de
-Jong and Santiago Ontan'on and Siddhartha Brahma and Yury Zemlyanskiy and David
-Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit
-Sanghai}, year = {2023} } ```
+some improvising there, scaling_the_projected_values, but if you think you know
+the answer, please open an issue ## Appreciation - Stability.ai for the
+generous sponsorship to work on cutting edge artificial intelligence research
+## Install ```bash $ pip install colt5-attention ``` ## Usage ```python import
+torch from colt5_attention import ( ConditionalRoutedFeedForward,
+ConditionalRoutedAttention, ConditionalRoutedTransformerBlock ) # mock input,
+say it is 32768 length tokens = torch.randn(2, 32768, 512) mask = torch.ones(2,
+32768).bool() # can handle variable lengthed sequences # feedforward ff =
+ConditionalRoutedFeedForward( dim = 512, light_ff_mult = 0.5, # hidden
+dimension ratio of light branch heavy_ff_mult = 4, # hidden dimension ratio of
+heavy branch num_heavy_tokens = 1024 # heavy branch receives only 1024 routed
+tokens of 32768 ) ff_out = ff(tokens, mask = mask) # (2, 32768, 512) - light
+and heavy branch summed # attention attn = ConditionalRoutedAttention( dim =
+512, light_dim_head = 64, # attention head dimension of light branch
+light_heads = 8, # number of attention heads for light branch light_window_size
+= 128, # local attention receptive field for light heavy_dim_head = 64, #
+attention head dimension of heavy branch heavy_heads = 8, # number of attention
+heads for heavy branch num_heavy_tokens_q = 1024, # heavy branch receives only
+1024 routed tokens of 32768 num_heavy_tokens_kv = 1024 # heavy branch receives
+only 1024 routed tokens of 32768 ) attn_out = attn(tokens, mask = mask) # (2,
+32768, 512) - light and heavy branch summed # both attention and feedforward
+with residual # the complete transformer block # a stack of these would
+constitute the encoder of CoLT5 block = ConditionalRoutedTransformerBlock( dim
+= 512, light_dim_head = 64, light_heads = 8, light_window_size = 128,
+heavy_dim_head = 64, heavy_heads = 8, light_ff_mult = 0.5, heavy_ff_mult = 4,
+num_heavy_ff_tokens = 1024, num_heavy_attn_tokens_q = 1024,
+num_heavy_attn_tokens_kv = 1024, router_type = 'coor_descent' # you have your
+choice of coordinate descent, as in paper - or 'sinkhorn' or 'cum_softmax' )
+block_out = block(tokens, mask = mask) # (2, 32768, 512) ``` Also included a
+variation of the conditionally routed attention for cross attention, to be
+tried with long context memories in a transformer-xl ```python import torch
+from colt5_attention import ConditionalRoutedCrossAttention # mock input, let
+us say it is a transformer of 1024 length attending to 1 million context past
+memories tokens = torch.randn(2, 1024, 512).cuda() tokens_mask = torch.ones(2,
+1024).bool().cuda() memories = torch.randn(2, int(1e6), 512).cuda()
+memories_mask = torch.ones(2, int(1e6)).bool().cuda() # conditionally routed
+cross attention cross_attn = ConditionalRoutedCrossAttention( dim = 512,
+dim_head = 64, heads = 8, num_tokens_q = 512, # only 512 routed from 1024
+num_tokens_kv = 1024, # only 1024 routed from 1 million ).cuda() cross_attn_out
+= cross_attn( tokens, context = memories, mask = tokens_mask, context_mask =
+memories_mask ) cross_attn_out.shape # (2, 1024, 512) - same as tokens ``` ##
+Todo - [x] add the coordinate descent method as another router - [x] figure out
+if it can be done autoregressively and try it out - moving to this_repo - [ ]
+for variable sequence lengths, allow for setting k as a function of sequence
+lengths per sample in batch - [ ] create a variant of CoLT5 for high resolution
+feature maps (image attention) - then try out for diffusion ## Citations
+```bibtex @inproceedings{Ainslie2023CoLT5FL, title = {CoLT5: Faster Long-Range
+Transformers with Conditional Computation}, author = {Joshua Ainslie and Tao
+Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury
+Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and
+Yun-Hsuan Sung and Sumit Sanghai}, year = {2023} } ```
```

### Comparing `CoLT5-attention-0.1.6/colt5_attention/coor_descent.py` & `CoLT5-attention-0.2.0/colt5_attention/coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.1.6/colt5_attention/sinkhorn.py` & `CoLT5-attention-0.2.0/colt5_attention/sinkhorn.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.1.6/colt5_attention/transformer_block.py` & `CoLT5-attention-0.2.0/colt5_attention/transformer_block.py`

 * *Files 3% similar despite different names*

```diff
@@ -391,16 +391,14 @@
             prenorm = True,
             causal = False,
             use_rotary_pos_emb = False,
             look_backward = 1,
             look_forward = 1
         )
 
-        # for now, just do qkv for starters, need to separate to q and kv
-
         self.q_router = router_klass(
             dim = dim,
             straight_through = router_straight_through,
             **router_kwargs
         )
 
         self.kv_router = router_klass(
@@ -427,24 +425,24 @@
 
         num_heavy_tokens_q = default(num_heavy_tokens_q, self.num_heavy_tokens_q)
         num_heavy_tokens_kv = default(num_heavy_tokens_kv, self.num_heavy_tokens_kv)
 
         batch_range = torch.arange(batch, device = device)
         batch_range = rearrange(batch_range, 'b -> b 1')
 
-        # light local attention sees all tokens
+        # light local attention sees all tokens in a limited context
 
         light_out = self.light_attn(x, mask = mask)
 
         # route tokens appropriately for heavy branch
 
         normalized_scores_q, indices_q = self.q_router(x, num_tokens = num_heavy_tokens_q, mask = mask)
         normalized_scores_kv, indices_kv = self.kv_router(x, num_tokens = num_heavy_tokens_kv, mask = mask)
 
-        # select the tokens to be routed to heavier feedforward (hidden dimension is 4 times model dimensions)
+        # select the tokens to be routed to full attention
 
         routed_tokens_q = x[batch_range, indices_q]
         routed_tokens_kv = x[batch_range, indices_kv]
 
         # calculate key padding mask
 
         routed_tokens_kv_mask = None
@@ -458,27 +456,126 @@
             mask = routed_tokens_kv_mask,
             context = routed_tokens_kv,
             normalized_scores_kv = normalized_scores_kv
         )
 
         routed_tokens_out = routed_tokens_out * rearrange(normalized_scores_q, '... -> ... 1')
 
-        # scatter back the output of the heavy feedforward branch
+        # scatter back the output of the heavy branch
 
         heavy_out = torch.zeros_like(x)
 
         if self.router_type == 'sinkhorn':
             heavy_out = scatter_mean(heavy_out, routed_tokens_out, indices_q, dim = 1)
         else:
             heavy_out[batch_range, indices_q] = routed_tokens_out
 
         # sum light and heavy branches
 
         return light_out + heavy_out
 
+# adapting the conditional routed self attention to cross attention
+
+class ConditionalRoutedCrossAttention(nn.Module):
+    def __init__(
+        self,
+        dim,
+        *,
+        num_tokens_q,
+        num_tokens_kv,
+        dim_head = 64,
+        heads = 8,
+        router_straight_through = True, # would make sure all normalized scores are 1., still differentiable
+        router_type = 'coor_descent',
+        router_kwargs: dict = {}
+    ):
+        super().__init__()
+        assert router_type in ROUTERS.keys()
+
+        self.router_type = router_type
+
+        router_klass = ROUTERS.get(router_type)
+
+        self.num_tokens_q = num_tokens_q
+        self.num_tokens_kv = num_tokens_kv
+
+        self.q_router = router_klass(
+            dim = dim,
+            straight_through = router_straight_through,
+            **router_kwargs
+        )
+
+        self.kv_router = router_klass(
+            dim = dim,
+            straight_through = router_straight_through,
+            **router_kwargs
+        )
+
+        self.heavy_attn = Attention(
+            dim = dim,
+            dim_head = dim_head,
+            heads = heads
+        )
+
+    def forward(
+        self,
+        x,
+        context,
+        *,
+        num_tokens_q = None,
+        num_tokens_kv = None,
+        mask = None,
+        context_mask = None
+    ):
+        batch, device = x.shape[0], x.device
+
+        num_tokens_q = default(num_tokens_q, self.num_tokens_q)
+        num_tokens_kv = default(num_tokens_kv, self.num_tokens_kv)
+
+        batch_range = torch.arange(batch, device = device)
+        batch_range = rearrange(batch_range, 'b -> b 1')
+
+        # route tokens appropriately
+
+        normalized_scores_q, indices_q = self.q_router(x, num_tokens = num_tokens_q, mask = mask)
+        normalized_scores_kv, indices_kv = self.kv_router(context, num_tokens = num_tokens_kv, mask = context_mask)
+
+        # select the tokens to be routed
+
+        routed_tokens_q = x[batch_range, indices_q]
+        routed_tokens_kv = x[batch_range, indices_kv]
+
+        # calculate key padding mask
+
+        routed_tokens_kv_mask = None
+        if exists(mask):
+            routed_tokens_kv_mask = context_mask[batch_range, indices_kv]
+
+        # do the heavier branch with only routed tokens
+
+        routed_tokens_out = self.heavy_attn(
+            routed_tokens_q,
+            mask = routed_tokens_kv_mask,
+            context = routed_tokens_kv,
+            normalized_scores_kv = normalized_scores_kv
+        )
+
+        routed_tokens_out = routed_tokens_out * rearrange(normalized_scores_q, '... -> ... 1')
+
+        # scatter back the output
+
+        out = torch.zeros_like(x)
+
+        if self.router_type == 'sinkhorn':
+            out = scatter_mean(heavy_out, routed_tokens_out, indices_q, dim = 1)
+        else:
+            out[batch_range, indices_q] = routed_tokens_out
+
+        return out
+
 # block
 
 class ConditionalRoutedTransformerBlock(nn.Module):
     def __init__(
         self,
         dim,
         *,
```

### Comparing `CoLT5-attention-0.1.6/setup.py` & `CoLT5-attention-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.1.6',
+  version = '0.2.0',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```

