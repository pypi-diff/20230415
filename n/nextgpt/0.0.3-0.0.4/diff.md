# Comparing `tmp/nextgpt-0.0.3.tar.gz` & `tmp/nextgpt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextgpt-0.0.3.tar", last modified: Mon Apr 10 20:56:49 2023, max compression
+gzip compressed data, was "nextgpt-0.0.4.tar", last modified: Sat Apr 15 16:26:55 2023, max compression
```

## Comparing `nextgpt-0.0.3.tar` & `nextgpt-0.0.4.tar`

### file list

```diff
@@ -1,85 +1,86 @@
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.928187 nextgpt-0.0.3/
--rw-r--r--   0 ybae2      (502) staff       (20)    11396 2023-04-10 16:51:37.000000 nextgpt-0.0.3/LICENSE
--rw-r--r--   0 ybae2      (502) staff       (20)       60 2023-04-10 19:51:51.000000 nextgpt-0.0.3/MANIFEST.in
--rw-r--r--   0 ybae2      (502) staff       (20)     1584 2023-04-10 20:56:49.928496 nextgpt-0.0.3/PKG-INFO
--rw-r--r--   0 ybae2      (502) staff       (20)     1359 2023-04-10 18:26:51.000000 nextgpt-0.0.3/README.md
--rw-r--r--   0 ybae2      (502) staff       (20)      254 2023-04-10 16:58:44.000000 nextgpt-0.0.3/requirements.txt
--rw-r--r--   0 ybae2      (502) staff       (20)      103 2023-04-10 20:56:49.931403 nextgpt-0.0.3/setup.cfg
--rw-r--r--   0 ybae2      (502) staff       (20)      888 2023-04-10 20:56:43.000000 nextgpt-0.0.3/setup.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.733049 nextgpt-0.0.3/src/
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.747668 nextgpt-0.0.3/src/nextgpt/
--rw-r--r--   0 ybae2      (502) staff       (20)        0 2023-04-02 22:26:04.000000 nextgpt-0.0.3/src/nextgpt/__init__.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.765299 nextgpt-0.0.3/src/nextgpt/dataset/
--rw-rw-r--   0 ybae2      (502) staff       (20)      384 2023-04-09 23:18:51.000000 nextgpt-0.0.3/src/nextgpt/dataset/__init__.py
--rw-r--r--   0 ybae2      (502) staff       (20)     1557 2023-04-09 23:42:09.000000 nextgpt-0.0.3/src/nextgpt/dataset/prompt_dataset.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     2077 2023-04-08 05:42:58.000000 nextgpt-0.0.3/src/nextgpt/dataset/reward_dataset.py
--rw-r--r--   0 ybae2      (502) staff       (20)     5903 2023-04-08 23:30:05.000000 nextgpt-0.0.3/src/nextgpt/dataset/sft_dataset.py
--rw-rw-r--   0 ybae2      (502) staff       (20)      121 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/dataset/utils.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.770291 nextgpt-0.0.3/src/nextgpt/experience_maker/
--rw-rw-r--   0 ybae2      (502) staff       (20)      155 2023-04-07 03:39:09.000000 nextgpt-0.0.3/src/nextgpt/experience_maker/__init__.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     2455 2023-04-08 19:18:09.000000 nextgpt-0.0.3/src/nextgpt/experience_maker/base.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1421 2023-04-08 19:18:19.000000 nextgpt-0.0.3/src/nextgpt/experience_maker/naive.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.776202 nextgpt-0.0.3/src/nextgpt/finetuning/
--rw-r--r--   0 ybae2      (502) staff       (20)      130 2023-04-10 17:22:26.000000 nextgpt-0.0.3/src/nextgpt/finetuning/__init__.py
--rw-r--r--   0 ybae2      (502) staff       (20)     1872 2023-04-01 19:32:10.000000 nextgpt-0.0.3/src/nextgpt/finetuning/callbacks.py
--rw-r--r--   0 ybae2      (502) staff       (20)     1038 2023-04-01 19:32:10.000000 nextgpt-0.0.3/src/nextgpt/finetuning/trainer.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.787798 nextgpt-0.0.3/src/nextgpt/models/
--rw-rw-r--   0 ybae2      (502) staff       (20)      245 2023-04-04 17:08:15.000000 nextgpt-0.0.3/src/nextgpt/models/__init__.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.802292 nextgpt-0.0.3/src/nextgpt/models/base/
--rw-rw-r--   0 ybae2      (502) staff       (20)      161 2023-04-08 06:54:54.000000 nextgpt-0.0.3/src/nextgpt/models/base/__init__.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     2480 2023-04-09 23:51:32.000000 nextgpt-0.0.3/src/nextgpt/models/base/actor.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1624 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/models/base/critic.py
--rw-rw-r--   0 ybae2      (502) staff       (20)      919 2023-04-08 06:34:00.000000 nextgpt-0.0.3/src/nextgpt/models/base/lm.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1419 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/models/base/reward_model.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.814100 nextgpt-0.0.3/src/nextgpt/models/bloom/
--rw-rw-r--   0 ybae2      (502) staff       (20)      197 2023-04-08 06:56:20.000000 nextgpt-0.0.3/src/nextgpt/models/bloom/__init__.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1097 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/models/bloom/bloom_actor.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1214 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/models/bloom/bloom_critic.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1091 2023-04-03 09:12:22.000000 nextgpt-0.0.3/src/nextgpt/models/bloom/bloom_lm.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1170 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/models/bloom/bloom_rm.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     6951 2023-04-08 19:12:37.000000 nextgpt-0.0.3/src/nextgpt/models/generation.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     3552 2023-04-08 19:13:03.000000 nextgpt-0.0.3/src/nextgpt/models/generation_utils.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.834428 nextgpt-0.0.3/src/nextgpt/models/gpt/
--rw-rw-r--   0 ybae2      (502) staff       (20)      173 2023-04-08 06:56:00.000000 nextgpt-0.0.3/src/nextgpt/models/gpt/__init__.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1182 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/models/gpt/gpt_actor.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1242 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/models/gpt/gpt_critic.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1347 2023-04-08 20:49:49.000000 nextgpt-0.0.3/src/nextgpt/models/gpt/gpt_lm.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1456 2023-04-06 18:56:26.000000 nextgpt-0.0.3/src/nextgpt/models/gpt/gpt_rm.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     4792 2023-04-08 19:13:30.000000 nextgpt-0.0.3/src/nextgpt/models/lora.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     3633 2023-04-10 16:48:50.000000 nextgpt-0.0.3/src/nextgpt/models/loss.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.848555 nextgpt-0.0.3/src/nextgpt/models/opt/
--rw-rw-r--   0 ybae2      (502) staff       (20)      173 2023-04-08 06:56:42.000000 nextgpt-0.0.3/src/nextgpt/models/opt/__init__.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1164 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/models/opt/opt_actor.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1283 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/models/opt/opt_critic.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1158 2023-04-03 09:12:22.000000 nextgpt-0.0.3/src/nextgpt/models/opt/opt_lm.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1176 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/models/opt/opt_rm.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     3483 2023-04-08 19:14:21.000000 nextgpt-0.0.3/src/nextgpt/models/utils.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.861828 nextgpt-0.0.3/src/nextgpt/replay_buffer/
--rw-rw-r--   0 ybae2      (502) staff       (20)      117 2023-04-07 03:39:09.000000 nextgpt-0.0.3/src/nextgpt/replay_buffer/__init__.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1050 2023-04-08 19:18:33.000000 nextgpt-0.0.3/src/nextgpt/replay_buffer/base.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1997 2023-04-08 19:18:40.000000 nextgpt-0.0.3/src/nextgpt/replay_buffer/naive.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     2376 2023-04-08 19:18:49.000000 nextgpt-0.0.3/src/nextgpt/replay_buffer/utils.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.881883 nextgpt-0.0.3/src/nextgpt/trainer/
--rw-rw-r--   0 ybae2      (502) staff       (20)      190 2023-04-08 06:57:54.000000 nextgpt-0.0.3/src/nextgpt/trainer/__init__.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     8730 2023-04-08 19:32:33.000000 nextgpt-0.0.3/src/nextgpt/trainer/base.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.907237 nextgpt-0.0.3/src/nextgpt/trainer/callbacks/
--rw-rw-r--   0 ybae2      (502) staff       (20)      193 2023-04-07 03:39:09.000000 nextgpt-0.0.3/src/nextgpt/trainer/callbacks/__init__.py
--rw-rw-r--   0 ybae2      (502) staff       (20)      841 2023-04-08 19:20:17.000000 nextgpt-0.0.3/src/nextgpt/trainer/callbacks/base.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     5402 2023-04-08 19:20:52.000000 nextgpt-0.0.3/src/nextgpt/trainer/callbacks/performance_evaluator.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     2840 2023-04-08 19:20:48.000000 nextgpt-0.0.3/src/nextgpt/trainer/callbacks/save_checkpoint.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     6980 2023-04-10 01:27:30.000000 nextgpt-0.0.3/src/nextgpt/trainer/ppo.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     6121 2023-04-08 19:08:44.000000 nextgpt-0.0.3/src/nextgpt/trainer/rm.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     7045 2023-04-10 20:54:20.000000 nextgpt-0.0.3/src/nextgpt/trainer/sft.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.926174 nextgpt-0.0.3/src/nextgpt/trainer/strategies/
--rw-rw-r--   0 ybae2      (502) staff       (20)      145 2023-04-03 20:19:30.000000 nextgpt-0.0.3/src/nextgpt/trainer/strategies/__init__.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     4758 2023-04-08 18:37:38.000000 nextgpt-0.0.3/src/nextgpt/trainer/strategies/base.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     4537 2023-04-08 18:42:20.000000 nextgpt-0.0.3/src/nextgpt/trainer/strategies/ddp.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     3077 2023-04-08 18:45:13.000000 nextgpt-0.0.3/src/nextgpt/trainer/strategies/naive.py
--rw-rw-r--   0 ybae2      (502) staff       (20)     1108 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/trainer/strategies/sampler.py
--rw-rw-r--   0 ybae2      (502) staff       (20)      121 2023-03-28 02:52:31.000000 nextgpt-0.0.3/src/nextgpt/trainer/utils.py
-drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-10 20:56:49.755478 nextgpt-0.0.3/src/nextgpt.egg-info/
--rw-r--r--   0 ybae2      (502) staff       (20)     1584 2023-04-10 20:56:49.000000 nextgpt-0.0.3/src/nextgpt.egg-info/PKG-INFO
--rw-r--r--   0 ybae2      (502) staff       (20)     2251 2023-04-10 20:56:49.000000 nextgpt-0.0.3/src/nextgpt.egg-info/SOURCES.txt
--rw-r--r--   0 ybae2      (502) staff       (20)        1 2023-04-10 20:56:49.000000 nextgpt-0.0.3/src/nextgpt.egg-info/dependency_links.txt
--rw-r--r--   0 ybae2      (502) staff       (20)       54 2023-04-10 20:56:49.000000 nextgpt-0.0.3/src/nextgpt.egg-info/requires.txt
--rw-r--r--   0 ybae2      (502) staff       (20)        8 2023-04-10 20:56:49.000000 nextgpt-0.0.3/src/nextgpt.egg-info/top_level.txt
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-15 16:26:55.507712 nextgpt-0.0.4/
+-rw-r--r--   0 ybae2      (502) staff       (20)    11396 2023-04-10 16:51:37.000000 nextgpt-0.0.4/LICENSE
+-rw-r--r--   0 ybae2      (502) staff       (20)       60 2023-04-10 19:51:51.000000 nextgpt-0.0.4/MANIFEST.in
+-rw-r--r--   0 ybae2      (502) staff       (20)     1844 2023-04-15 16:26:55.508087 nextgpt-0.0.4/PKG-INFO
+-rw-r--r--   0 ybae2      (502) staff       (20)     1619 2023-04-15 16:24:39.000000 nextgpt-0.0.4/README.md
+-rw-r--r--   0 ybae2      (502) staff       (20)      254 2023-04-10 16:58:44.000000 nextgpt-0.0.4/requirements.txt
+-rw-r--r--   0 ybae2      (502) staff       (20)      103 2023-04-15 16:26:55.512674 nextgpt-0.0.4/setup.cfg
+-rw-r--r--   0 ybae2      (502) staff       (20)      888 2023-04-15 16:17:25.000000 nextgpt-0.0.4/setup.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-15 16:26:55.082688 nextgpt-0.0.4/src/
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-15 16:26:55.101088 nextgpt-0.0.4/src/nextgpt/
+-rw-r--r--   0 ybae2      (502) staff       (20)        0 2023-04-02 22:26:04.000000 nextgpt-0.0.4/src/nextgpt/__init__.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-15 16:26:55.173184 nextgpt-0.0.4/src/nextgpt/dataset/
+-rw-rw-r--   0 ybae2      (502) staff       (20)      384 2023-04-09 23:18:51.000000 nextgpt-0.0.4/src/nextgpt/dataset/__init__.py
+-rw-r--r--   0 ybae2      (502) staff       (20)     1557 2023-04-09 23:42:09.000000 nextgpt-0.0.4/src/nextgpt/dataset/prompt_dataset.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     2077 2023-04-08 05:42:58.000000 nextgpt-0.0.4/src/nextgpt/dataset/reward_dataset.py
+-rw-r--r--   0 ybae2      (502) staff       (20)     5903 2023-04-08 23:30:05.000000 nextgpt-0.0.4/src/nextgpt/dataset/sft_dataset.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)      121 2023-03-28 02:52:31.000000 nextgpt-0.0.4/src/nextgpt/dataset/utils.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-15 16:26:55.189956 nextgpt-0.0.4/src/nextgpt/experience_maker/
+-rw-rw-r--   0 ybae2      (502) staff       (20)      155 2023-04-07 03:39:09.000000 nextgpt-0.0.4/src/nextgpt/experience_maker/__init__.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     2455 2023-04-08 19:18:09.000000 nextgpt-0.0.4/src/nextgpt/experience_maker/base.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1421 2023-04-08 19:18:19.000000 nextgpt-0.0.4/src/nextgpt/experience_maker/naive.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-15 16:26:55.198259 nextgpt-0.0.4/src/nextgpt/finetuning/
+-rw-r--r--   0 ybae2      (502) staff       (20)      130 2023-04-10 17:22:26.000000 nextgpt-0.0.4/src/nextgpt/finetuning/__init__.py
+-rw-r--r--   0 ybae2      (502) staff       (20)     1994 2023-04-11 23:01:58.000000 nextgpt-0.0.4/src/nextgpt/finetuning/callbacks.py
+-rw-r--r--   0 ybae2      (502) staff       (20)     1038 2023-04-01 19:32:10.000000 nextgpt-0.0.4/src/nextgpt/finetuning/trainer.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-15 16:26:55.233175 nextgpt-0.0.4/src/nextgpt/models/
+-rw-rw-r--   0 ybae2      (502) staff       (20)      245 2023-04-04 17:08:15.000000 nextgpt-0.0.4/src/nextgpt/models/__init__.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-15 16:26:55.258284 nextgpt-0.0.4/src/nextgpt/models/base/
+-rw-rw-r--   0 ybae2      (502) staff       (20)      161 2023-04-08 06:54:54.000000 nextgpt-0.0.4/src/nextgpt/models/base/__init__.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     2480 2023-04-09 23:51:32.000000 nextgpt-0.0.4/src/nextgpt/models/base/actor.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1624 2023-03-28 02:52:31.000000 nextgpt-0.0.4/src/nextgpt/models/base/critic.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)      919 2023-04-08 06:34:00.000000 nextgpt-0.0.4/src/nextgpt/models/base/lm.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1419 2023-03-28 02:52:31.000000 nextgpt-0.0.4/src/nextgpt/models/base/reward_model.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-15 16:26:55.296682 nextgpt-0.0.4/src/nextgpt/models/bloom/
+-rw-rw-r--   0 ybae2      (502) staff       (20)      197 2023-04-08 06:56:20.000000 nextgpt-0.0.4/src/nextgpt/models/bloom/__init__.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1097 2023-03-28 02:52:31.000000 nextgpt-0.0.4/src/nextgpt/models/bloom/bloom_actor.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1214 2023-03-28 02:52:31.000000 nextgpt-0.0.4/src/nextgpt/models/bloom/bloom_critic.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1091 2023-04-03 09:12:22.000000 nextgpt-0.0.4/src/nextgpt/models/bloom/bloom_lm.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1170 2023-03-28 02:52:31.000000 nextgpt-0.0.4/src/nextgpt/models/bloom/bloom_rm.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     6951 2023-04-08 19:12:37.000000 nextgpt-0.0.4/src/nextgpt/models/generation.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     3552 2023-04-08 19:13:03.000000 nextgpt-0.0.4/src/nextgpt/models/generation_utils.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-15 16:26:55.330203 nextgpt-0.0.4/src/nextgpt/models/gpt/
+-rw-rw-r--   0 ybae2      (502) staff       (20)      173 2023-04-08 06:56:00.000000 nextgpt-0.0.4/src/nextgpt/models/gpt/__init__.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1398 2023-04-12 05:43:21.000000 nextgpt-0.0.4/src/nextgpt/models/gpt/gpt_actor.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1242 2023-03-28 02:52:31.000000 nextgpt-0.0.4/src/nextgpt/models/gpt/gpt_critic.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1788 2023-04-12 05:44:01.000000 nextgpt-0.0.4/src/nextgpt/models/gpt/gpt_lm.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1456 2023-04-06 18:56:26.000000 nextgpt-0.0.4/src/nextgpt/models/gpt/gpt_rm.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     4792 2023-04-08 19:13:30.000000 nextgpt-0.0.4/src/nextgpt/models/lora.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     3661 2023-04-11 05:09:57.000000 nextgpt-0.0.4/src/nextgpt/models/loss.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-15 16:26:55.368412 nextgpt-0.0.4/src/nextgpt/models/opt/
+-rw-rw-r--   0 ybae2      (502) staff       (20)      173 2023-04-08 06:56:42.000000 nextgpt-0.0.4/src/nextgpt/models/opt/__init__.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1164 2023-03-28 02:52:31.000000 nextgpt-0.0.4/src/nextgpt/models/opt/opt_actor.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1283 2023-03-28 02:52:31.000000 nextgpt-0.0.4/src/nextgpt/models/opt/opt_critic.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1158 2023-04-03 09:12:22.000000 nextgpt-0.0.4/src/nextgpt/models/opt/opt_lm.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1176 2023-03-28 02:52:31.000000 nextgpt-0.0.4/src/nextgpt/models/opt/opt_rm.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     3483 2023-04-08 19:14:21.000000 nextgpt-0.0.4/src/nextgpt/models/utils.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-15 16:26:55.400375 nextgpt-0.0.4/src/nextgpt/replay_buffer/
+-rw-rw-r--   0 ybae2      (502) staff       (20)      117 2023-04-07 03:39:09.000000 nextgpt-0.0.4/src/nextgpt/replay_buffer/__init__.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1050 2023-04-08 19:18:33.000000 nextgpt-0.0.4/src/nextgpt/replay_buffer/base.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1997 2023-04-08 19:18:40.000000 nextgpt-0.0.4/src/nextgpt/replay_buffer/naive.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     2376 2023-04-08 19:18:49.000000 nextgpt-0.0.4/src/nextgpt/replay_buffer/utils.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-15 16:26:55.456694 nextgpt-0.0.4/src/nextgpt/trainer/
+-rw-rw-r--   0 ybae2      (502) staff       (20)      190 2023-04-08 06:57:54.000000 nextgpt-0.0.4/src/nextgpt/trainer/__init__.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     7509 2023-04-12 23:34:32.000000 nextgpt-0.0.4/src/nextgpt/trainer/base.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-15 16:26:55.483857 nextgpt-0.0.4/src/nextgpt/trainer/callbacks/
+-rw-rw-r--   0 ybae2      (502) staff       (20)      243 2023-04-10 23:49:07.000000 nextgpt-0.0.4/src/nextgpt/trainer/callbacks/__init__.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)      930 2023-04-10 23:13:43.000000 nextgpt-0.0.4/src/nextgpt/trainer/callbacks/base.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1053 2023-04-10 23:47:18.000000 nextgpt-0.0.4/src/nextgpt/trainer/callbacks/log_metrics.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     5402 2023-04-08 19:20:52.000000 nextgpt-0.0.4/src/nextgpt/trainer/callbacks/performance_evaluator.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     2853 2023-04-10 22:20:52.000000 nextgpt-0.0.4/src/nextgpt/trainer/callbacks/save_checkpoint.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     7525 2023-04-13 00:59:15.000000 nextgpt-0.0.4/src/nextgpt/trainer/ppo.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     7665 2023-04-12 22:50:20.000000 nextgpt-0.0.4/src/nextgpt/trainer/rm.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)    11341 2023-04-12 23:23:07.000000 nextgpt-0.0.4/src/nextgpt/trainer/sft.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-15 16:26:55.505947 nextgpt-0.0.4/src/nextgpt/trainer/strategies/
+-rw-rw-r--   0 ybae2      (502) staff       (20)      145 2023-04-03 20:19:30.000000 nextgpt-0.0.4/src/nextgpt/trainer/strategies/__init__.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     4758 2023-04-08 18:37:38.000000 nextgpt-0.0.4/src/nextgpt/trainer/strategies/base.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     4537 2023-04-11 05:26:34.000000 nextgpt-0.0.4/src/nextgpt/trainer/strategies/ddp.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     3077 2023-04-08 18:45:13.000000 nextgpt-0.0.4/src/nextgpt/trainer/strategies/naive.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)     1108 2023-03-28 02:52:31.000000 nextgpt-0.0.4/src/nextgpt/trainer/strategies/sampler.py
+-rw-rw-r--   0 ybae2      (502) staff       (20)      121 2023-03-28 02:52:31.000000 nextgpt-0.0.4/src/nextgpt/trainer/utils.py
+drwxr-xr-x   0 ybae2      (502) staff       (20)        0 2023-04-15 16:26:55.157307 nextgpt-0.0.4/src/nextgpt.egg-info/
+-rw-r--r--   0 ybae2      (502) staff       (20)     1844 2023-04-15 16:26:54.000000 nextgpt-0.0.4/src/nextgpt.egg-info/PKG-INFO
+-rw-r--r--   0 ybae2      (502) staff       (20)     2296 2023-04-15 16:26:55.000000 nextgpt-0.0.4/src/nextgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 ybae2      (502) staff       (20)        1 2023-04-15 16:26:54.000000 nextgpt-0.0.4/src/nextgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 ybae2      (502) staff       (20)       54 2023-04-15 16:26:54.000000 nextgpt-0.0.4/src/nextgpt.egg-info/requires.txt
+-rw-r--r--   0 ybae2      (502) staff       (20)        8 2023-04-15 16:26:54.000000 nextgpt-0.0.4/src/nextgpt.egg-info/top_level.txt
```

### Comparing `nextgpt-0.0.3/LICENSE` & `nextgpt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/PKG-INFO` & `nextgpt-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: nextgpt
-Version: 0.0.3
+Version: 0.0.4
 Summary: nextGPT
 Home-page: https://github.com/louiezzang/next-gpt
 Author: Younggue Bae
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nextGPT
 > 📢 Open source implementation for ChatGPT replica to build the end-to-end pipeline from SFT to RLHF.
 
 - 🔥 Step 1) SFT: Surpervised Fine-tuning
 - 🔥 Step 2) RM: Reward Model
 - 🔥 Step 3) PPO: Proximal Policy Optimization
 
+![ChatGPT Diagram](https://openaicom.imgix.net/cf717bdb-0c8c-428a-b82b-3c3add87a600/ChatGPT_Diagram.svg?fm=auto&auto=compress,format&fit=min&w=1919&h=1138)
+
 # Installation
 ```
 $ pip install nextgpt
 ```
-or
+or install from git repo to the get always the latest version.
 ```
 $ git clone https://github.com/louiezzang/next-gpt.git
 $ cd next-gpt/
 $ pip install .
 $ cd ../
 ```
 
@@ -39,10 +41,12 @@
 - https://github.com/airobotlab/KoChatGPT/tree/main/colossalai_ChatGPT_230319
 - https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat
 
 # References
 - https://github.com/airobotlab/KoChatGPT
 - https://github.com/airobotlab/KoChatGPT/tree/main/colossalai_ChatGPT_230319
 - https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat
+- https://github.com/juncongmoo/chatllama
 - https://github.com/huggingface/peft
 - https://github.com/dredwardhyde/gpt-neo-fine-tuning-example/blob/main/gpt_neo.py
 - https://github.com/databrickslabs/dolly
+
```

### Comparing `nextgpt-0.0.3/README.md` & `nextgpt-0.0.4/src/nextgpt.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,31 @@
+Metadata-Version: 2.1
+Name: nextgpt
+Version: 0.0.4
+Summary: nextGPT
+Home-page: https://github.com/louiezzang/next-gpt
+Author: Younggue Bae
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # nextGPT
 > 📢 Open source implementation for ChatGPT replica to build the end-to-end pipeline from SFT to RLHF.
 
 - 🔥 Step 1) SFT: Surpervised Fine-tuning
 - 🔥 Step 2) RM: Reward Model
 - 🔥 Step 3) PPO: Proximal Policy Optimization
 
+![ChatGPT Diagram](https://openaicom.imgix.net/cf717bdb-0c8c-428a-b82b-3c3add87a600/ChatGPT_Diagram.svg?fm=auto&auto=compress,format&fit=min&w=1919&h=1138)
+
 # Installation
 ```
 $ pip install nextgpt
 ```
-or
+or install from git repo to the get always the latest version.
 ```
 $ git clone https://github.com/louiezzang/next-gpt.git
 $ cd next-gpt/
 $ pip install .
 $ cd ../
 ```
 
@@ -29,10 +41,12 @@
 - https://github.com/airobotlab/KoChatGPT/tree/main/colossalai_ChatGPT_230319
 - https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat
 
 # References
 - https://github.com/airobotlab/KoChatGPT
 - https://github.com/airobotlab/KoChatGPT/tree/main/colossalai_ChatGPT_230319
 - https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat
+- https://github.com/juncongmoo/chatllama
 - https://github.com/huggingface/peft
 - https://github.com/dredwardhyde/gpt-neo-fine-tuning-example/blob/main/gpt_neo.py
 - https://github.com/databrickslabs/dolly
+
```

### Comparing `nextgpt-0.0.3/setup.py` & `nextgpt-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 import os
 import sys
 import pkg_resources
 from setuptools import setup, find_packages
 
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 DESCRIPTION = "nextGPT"
 
 setup(
     name="nextgpt",
     version=VERSION,
     description=DESCRIPTION,
     long_description=open("README.md", "r", encoding="utf-8").read(),
```

### Comparing `nextgpt-0.0.3/src/nextgpt/dataset/prompt_dataset.py` & `nextgpt-0.0.4/src/nextgpt/dataset/prompt_dataset.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/dataset/reward_dataset.py` & `nextgpt-0.0.4/src/nextgpt/dataset/reward_dataset.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/dataset/sft_dataset.py` & `nextgpt-0.0.4/src/nextgpt/dataset/sft_dataset.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/experience_maker/base.py` & `nextgpt-0.0.4/src/nextgpt/experience_maker/base.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/experience_maker/naive.py` & `nextgpt-0.0.4/src/nextgpt/experience_maker/naive.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/finetuning/callbacks.py` & `nextgpt-0.0.4/src/nextgpt/finetuning/callbacks.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 )   
 
 class LoggingCallback(TrainerCallback):
     """
     A [`TrainerCallback`] that handles the custom logging by such as model logger.
     """
 
-    def __init__(self, logger):
+    def __init__(self, logger, verbose: bool = False):
         self.logger = logger
+        self.verbose = verbose
     
     def on_epoch_end(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs):
         """
         Event called at the end of an epoch.
         """
         #print(f"*** on_epoch_end: {state}")
         pass
@@ -27,30 +28,32 @@
         #print(f"*** on_step_end: {state}")
         pass
         
     def on_evaluate(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs):
         """
         Event called after an evaluation phase.
         """
-        print(f"*** on_evaluate: {state}")
+        if self.verbose:
+            print(f"*** on_evaluate: {state}")
 
     def on_save(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs):
         """
         Event called after a checkpoint save.
         """
-        print(f"*** on_save: {state}")
+        # print(f"*** on_save: {state}")
         if self.logger:
             step = state.global_step
             log_history = state.log_history
 
             log = None
             for x in log_history:
                 if x["step"] == step:
                     log = x
                     break
             if hasattr(self.logger, "log_metrics") and log:
-                print(f"*** log metrics by model logger: {log}")
+                if self.verbose:
+                    print(f"*** log metrics by model logger: {log}")
                 metrics = {
                     "train_loss": log["loss"]
                 }
                 self.logger.log_metrics(metrics, step)
```

### Comparing `nextgpt-0.0.3/src/nextgpt/finetuning/trainer.py` & `nextgpt-0.0.4/src/nextgpt/finetuning/trainer.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/models/base/actor.py` & `nextgpt-0.0.4/src/nextgpt/models/base/actor.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/models/base/critic.py` & `nextgpt-0.0.4/src/nextgpt/models/base/critic.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/models/base/lm.py` & `nextgpt-0.0.4/src/nextgpt/models/base/lm.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/models/base/reward_model.py` & `nextgpt-0.0.4/src/nextgpt/models/base/reward_model.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/models/bloom/bloom_actor.py` & `nextgpt-0.0.4/src/nextgpt/models/bloom/bloom_actor.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/models/bloom/bloom_critic.py` & `nextgpt-0.0.4/src/nextgpt/models/bloom/bloom_critic.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/models/bloom/bloom_lm.py` & `nextgpt-0.0.4/src/nextgpt/models/bloom/bloom_lm.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/models/bloom/bloom_rm.py` & `nextgpt-0.0.4/src/nextgpt/models/bloom/bloom_rm.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/models/generation.py` & `nextgpt-0.0.4/src/nextgpt/models/generation.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/models/generation_utils.py` & `nextgpt-0.0.4/src/nextgpt/models/generation_utils.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/models/gpt/gpt_actor.py` & `nextgpt-0.0.4/src/nextgpt/models/gpt/gpt_actor.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,16 +10,18 @@
     """
     GPT Actor model.
 
     Args:
         pretrained (str): Pretrained model name or path.
         config (GPT2Config): Model config.
         checkpoint (bool): Enable gradient checkpointing.
-        lora_rank (int): Rank of the LoRa layer.
+        lora_rank (int): Rank of the LoRa layer. 0 means LoRA is not applied. Defaults to 0.
         lora_train_bias (str): Bias training strategy for the LoRa layer.
+            'none' means it doesn't train biases. 'all' means it trains all biases. 'lora_only' means it only trains biases of LoRA layers.
+            Defaults to 'none'.
     """
 
     def __init__(self,
                  pretrained: Optional[str] = None,
                  config: Optional[GPT2Config] = None,
                  checkpoint: bool = False,
                  lora_rank: int = 0,
```

### Comparing `nextgpt-0.0.3/src/nextgpt/models/gpt/gpt_critic.py` & `nextgpt-0.0.4/src/nextgpt/models/gpt/gpt_critic.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/models/gpt/gpt_lm.py` & `nextgpt-0.0.4/src/nextgpt/models/gpt/gpt_rm.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 from typing import Optional
 
+import torch.nn as nn
 from transformers.models.gpt2.configuration_gpt2 import GPT2Config
-from transformers.models.gpt2.modeling_gpt2 import GPT2LMHeadModel
+from transformers.models.gpt2.modeling_gpt2 import GPT2Model
 
-from ..base import LM
+from ..base import RewardModel
 
 
-class GPTLM(LM):
+class GPTRM(RewardModel):
     """
-    GPT language model.
+    GPT Reward model.
+
     Args:
         pretrained (str): Pretrained model name or path.
         config (GPT2Config): Model config.
         checkpoint (bool): Enable gradient checkpointing.
-        lora_rank (int): Rank of the LoRa layer.
-        lora_train_bias (str): Bias training strategy for the LoRa layer.
+        lora_rank (int): Rank of the low-rank approximation.
+        lora_train_bias (str): LoRA bias training mode.
     """
 
     def __init__(self,
                  pretrained: Optional[str] = None,
                  config: Optional[GPT2Config] = None,
                  checkpoint: bool = False,
                  lora_rank: int = 0,
                  lora_train_bias: str = 'none') -> None:
         if pretrained is not None:
-            model = GPT2LMHeadModel.from_pretrained(pretrained)
+            model = GPT2Model.from_pretrained(pretrained)
         elif config is not None:
-            model = GPT2LMHeadModel(config)
+            model = GPT2Model(config)
         else:
-            model = GPT2LMHeadModel(GPT2Config())
+            model = GPT2Model(GPT2Config())
         if checkpoint:
             model.gradient_checkpointing_enable()
-        super().__init__(model, lora_rank, lora_train_bias)
 
-    def forward(self, input_ids, attention_mask=None, labels=None, **kwargs):
-        return self.model(input_ids, attention_mask=attention_mask, labels=labels, **kwargs)
+        value_head = nn.Linear(model.config.n_embd, 1)
+        value_head.weight.data.normal_(mean=0.0, std=1 / (model.config.n_embd + 1))
+        super().__init__(model, value_head, lora_rank, lora_train_bias)
+
+    def resize_token_embeddings(self, new_num_tokens: int):
+        self.model.resize_token_embeddings(new_num_tokens)
```

### Comparing `nextgpt-0.0.3/src/nextgpt/models/gpt/gpt_rm.py` & `nextgpt-0.0.4/src/nextgpt/models/gpt/gpt_lm.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 from typing import Optional
 
-import torch.nn as nn
 from transformers.models.gpt2.configuration_gpt2 import GPT2Config
-from transformers.models.gpt2.modeling_gpt2 import GPT2Model
+from transformers.models.gpt2.modeling_gpt2 import GPT2LMHeadModel
+from transformers import AutoModelForCausalLM
 
-from ..base import RewardModel
+from ..base import LM
 
 
-class GPTRM(RewardModel):
+class GPTLM(LM):
     """
-    GPT Reward model.
-
+    GPT language model.
     Args:
         pretrained (str): Pretrained model name or path.
         config (GPT2Config): Model config.
         checkpoint (bool): Enable gradient checkpointing.
-        lora_rank (int): Rank of the low-rank approximation.
-        lora_train_bias (str): LoRA bias training mode.
+        lora_rank (int): Rank of the LoRa layer. 0 means LoRA is not applied. Defaults to 0.
+        lora_train_bias (str): Bias training strategy for the LoRa layer.
+            'none' means it doesn't train biases. 'all' means it trains all biases. 'lora_only' means it only trains biases of LoRA layers.
+            Defaults to 'none'.
     """
 
     def __init__(self,
                  pretrained: Optional[str] = None,
                  config: Optional[GPT2Config] = None,
                  checkpoint: bool = False,
                  lora_rank: int = 0,
                  lora_train_bias: str = 'none') -> None:
         if pretrained is not None:
-            model = GPT2Model.from_pretrained(pretrained)
+            model = GPT2LMHeadModel.from_pretrained(pretrained)
+            # model = AutoModelForCausalLM.from_pretrained(pretrained)
         elif config is not None:
-            model = GPT2Model(config)
+            model = GPT2LMHeadModel(config)
+            # model = AutoModelForCausalLM(config)
         else:
-            model = GPT2Model(GPT2Config())
+            model = GPT2LMHeadModel(GPT2Config())
+            # model = AutoModelForCausalLM(GPT2Config())
         if checkpoint:
             model.gradient_checkpointing_enable()
+        super().__init__(model, lora_rank, lora_train_bias)
 
-        value_head = nn.Linear(model.config.n_embd, 1)
-        value_head.weight.data.normal_(mean=0.0, std=1 / (model.config.n_embd + 1))
-        super().__init__(model, value_head, lora_rank, lora_train_bias)
-
-    def resize_token_embeddings(self, new_num_tokens: int):
-        self.model.resize_token_embeddings(new_num_tokens)
+    def forward(self, input_ids, attention_mask=None, labels=None, **kwargs):
+        return self.model(input_ids, attention_mask=attention_mask, labels=labels, **kwargs)
```

### Comparing `nextgpt-0.0.3/src/nextgpt/models/lora.py` & `nextgpt-0.0.4/src/nextgpt/models/lora.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/models/loss.py` & `nextgpt-0.0.4/src/nextgpt/models/loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,16 @@
                 reward: torch.Tensor,
                 action_mask: Optional[torch.Tensor] = None) -> torch.Tensor:
         values_clipped = old_values + (values - old_values).clamp(-self.clip_eps, self.clip_eps)
         surr1 = (values_clipped - reward)**2
         surr2 = (values - reward)**2
         loss = torch.max(surr1, surr2)
         loss = loss.mean()
-        return loss
+        # return loss
+        return 0.5 * loss
 
 
 class PPOPtxActorLoss(nn.Module):
     """
     To Do:
     PPO-ptx Actor Loss
     """
```

### Comparing `nextgpt-0.0.3/src/nextgpt/models/opt/opt_actor.py` & `nextgpt-0.0.4/src/nextgpt/models/opt/opt_actor.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/models/opt/opt_critic.py` & `nextgpt-0.0.4/src/nextgpt/models/opt/opt_critic.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/models/opt/opt_lm.py` & `nextgpt-0.0.4/src/nextgpt/models/opt/opt_lm.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/models/opt/opt_rm.py` & `nextgpt-0.0.4/src/nextgpt/models/opt/opt_rm.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/models/utils.py` & `nextgpt-0.0.4/src/nextgpt/models/utils.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/replay_buffer/base.py` & `nextgpt-0.0.4/src/nextgpt/replay_buffer/base.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/replay_buffer/naive.py` & `nextgpt-0.0.4/src/nextgpt/replay_buffer/naive.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/replay_buffer/utils.py` & `nextgpt-0.0.4/src/nextgpt/replay_buffer/utils.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/trainer/base.py` & `nextgpt-0.0.4/src/nextgpt/trainer/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from abc import ABC, abstractmethod
 from typing import Any, Callable, Dict, List, Optional, Union
+from tqdm import tqdm
 
 import torch
-from ..experience_maker import Experience, ExperienceMaker
-from ..replay_buffer import ReplayBuffer
 from torch import Tensor
-from torch.utils.data import DistributedSampler
-from tqdm import tqdm
+from torch.utils.data import DataLoader
+from torch.utils.data.distributed import DistributedSampler
 
+from ..experience_maker import Experience, ExperienceMaker
+from ..replay_buffer import ReplayBuffer
 from .callbacks import Callback
 from .strategies import Strategy
 from .utils import is_rank_0
 
 
 class Trainer(ABC):
     """
@@ -90,46 +91,17 @@
                     self._on_learn_batch_start()
                     experience.to_device(device)
                     metrics = self.training_step(experience)
                     self._on_learn_batch_end(metrics, experience)
                     pbar.set_postfix(metrics)
                 self._on_learn_epoch_end(epoch)
 
-    # def fit(self, 
-    #         prompts, 
-    #         num_episodes: int = 50000, 
-    #         max_timesteps: int = 500, 
-    #         update_timesteps: int = 5000) -> None:
-    #     time = 0
-    #     sampler = self.strategy.setup_sampler(prompts)
-    #     self._on_fit_start()
-    #     for episode in range(num_episodes):
-    #         self._on_episode_start(episode)
-    #         for timestep in tqdm(range(max_timesteps),
-    #                              desc=f'Episode [{episode+1}/{num_episodes}]',
-    #                              disable=not is_rank_0()):
-    #             time += 1
-    #             rand_prompts = sampler.sample(self.experience_batch_size)
-    #             if self.tokenizer is not None:
-    #                 inputs = self.tokenizer(rand_prompts)
-    #             else:
-    #                 inputs = rand_prompts
-    #             self._on_make_experience_start()
-    #             experience = self._make_experience(inputs)
-    #             self._on_make_experience_end(experience)
-    #             self.replay_buffer.append(experience)
-    #             if time % update_timesteps == 0:
-    #                 self._learn()
-    #                 self.replay_buffer.clear()
-    #         self._on_episode_end(episode)
-    #     self._on_fit_end()
-
     def fit(self,
-            prompt_dataloader,
-            pretrain_dataloader,
+            prompt_dataloader: DataLoader,
+            pretrain_dataloader: DataLoader,
             num_episodes: int = 50000,
             max_timesteps: int = 500,
             update_timesteps: int = 5000) -> None:
         time = 0
         self.pretrain_dataloader = pretrain_dataloader
         self.prompt_dataloader = prompt_dataloader
         self._on_fit_start()
```

### Comparing `nextgpt-0.0.3/src/nextgpt/trainer/callbacks/base.py` & `nextgpt-0.0.4/src/nextgpt/trainer/callbacks/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,7 +33,11 @@
         pass
 
     def on_learn_batch_start(self) -> None:
         pass
 
     def on_learn_batch_end(self, metrics: dict, experience: Experience) -> None:
         pass
+
+    # Added
+    def on_log_metrics(self, metrics: dict, **kwargs) -> None:
+        pass
```

### Comparing `nextgpt-0.0.3/src/nextgpt/trainer/callbacks/performance_evaluator.py` & `nextgpt-0.0.4/src/nextgpt/trainer/callbacks/performance_evaluator.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/trainer/callbacks/save_checkpoint.py` & `nextgpt-0.0.4/src/nextgpt/trainer/callbacks/save_checkpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,11 +65,11 @@
                 continue
             model_path = os.path.join(base_path, f'{model}.pt')
             self.strategy.save_model(model=self.model_dict[model][0], path=model_path, only_rank0=True)
 
             # save optimizer
             if self.model_dict[model][1] is None:
                 continue
-            only_rank0 = not isinstance(self.strategy, ColossalAIStrategy)
+            only_rank0 = True # only_rank0 = not isinstance(self.strategy, XXXStrategy)
             rank = 0 if is_rank_0() else dist.get_rank()
             optim_path = os.path.join(base_path, f'{model}-optim-rank-{rank}.pt')
             self.strategy.save_optimizer(optimizer=self.model_dict[model][1], path=optim_path, only_rank0=only_rank0)
```

### Comparing `nextgpt-0.0.3/src/nextgpt/trainer/ppo.py` & `nextgpt-0.0.4/src/nextgpt/trainer/ppo.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,86 +1,100 @@
 from typing import Any, Callable, Dict, List, Optional
 
 import torch
 import torch.nn as nn
+from torch.optim import Adam, AdamW, Optimizer
+from transformers.tokenization_utils_base import PreTrainedTokenizerBase
+
 from ..experience_maker import Experience, NaiveExperienceMaker
 from ..models.base import Actor, Critic
 from ..models.generation_utils import update_model_kwargs_fn
 from ..models.loss import PolicyLoss, ValueLoss
 from ..replay_buffer import NaiveReplayBuffer
-from torch.optim import Optimizer
-from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 
 from .base import Trainer
 from .callbacks import Callback
 from .strategies import Strategy
 
 
 class PPOTrainer(Trainer):
     """
         Trainer for PPO algorithm.
-    Args:
+ 
+       Args:
         strategy (Strategy): the strategy to use for training
         actor (Actor): the actor model in ppo algorithm
         critic (Critic): the critic model in ppo algorithm
+        actor_lr (float, defaults to 1e-7): the learning rate for actor
+        critic_lr (float, defaults to 1e-7): the learning rate for critic
         reward_model (nn.Module): the reward model in rlhf algorithm to make reward of sentences
         initial_model (Actor): the initial model in rlhf algorithm to generate reference logits to limit the update of actor
-        actor_optim (Optimizer): the optimizer to use for actor model
-        critic_optim (Optimizer): the optimizer to use for critic model
         kl_coef (float, defaults to 0.1): the coefficient of kl divergence loss
         train_batch_size (int, defaults to 8): the batch size to use for training
         buffer_limit (int, defaults to 0): the max_size limitaiton of replay buffer
         buffer_cpu_offload (bool, defaults to True): whether to offload replay buffer to cpu
         eps_clip (float, defaults to 0.2): the clip coefficient of policy loss
+        vf_coef (float, defaults to 1.0): the coefficient of value loss
         value_clip (float, defaults to 0.4): the clip coefficient of value loss
         experience_batch_size (int, defaults to 8): the batch size to use for experience generation
         max_epochs (int, defaults to 1): the number of epochs of training process
-        tokenier (Callable, optional): the tokenizer to use for tokenizing the input
+        tokenizer (Callable, optional): the tokenizer to use for tokenizing the input
         sample_replay_buffer (bool, defaults to False): whether to sample from replay buffer
         dataloader_pin_memory (bool, defaults to True): whether to pin memory for data loader
         callbacks (List[Callback], defaults to []): the callbacks to call during training process
         generate_kwargs (dict, optional): the kwargs to use while model generating
     """
 
     def __init__(self,
                  strategy: Strategy,
                  actor: Actor,
                  critic: Critic,
                  reward_model: nn.Module,
                  initial_model: Actor,
-                 actor_optim: Optimizer,
-                 critic_optim: Optimizer,
+                 actor_lr: float = 1e-7,
+                 critic_lr: float = 1e-7,
                  kl_coef: float = 0.1,
                  ptx_coef: float = 0.9,
                  train_batch_size: int = 8,
                  buffer_limit: int = 0,
                  buffer_cpu_offload: bool = True,
                  eps_clip: float = 0.2,
+                 vf_coef: float = 1.0,
                  value_clip: float = 0.4,
                  experience_batch_size: int = 8,
                  max_epochs: int = 1,
                  tokenizer: Optional[Callable[[Any], dict]] = None,
                  sample_replay_buffer: bool = False,
                  dataloader_pin_memory: bool = True,
                  callbacks: List[Callback] = [],
                  **generate_kwargs) -> None:
+        
+        # Configure optimizer.
+        actor_optim = Adam(actor.parameters(), lr=actor_lr)
+        critic_optim = Adam(critic.parameters(), lr=critic_lr)
+
+        # Setting the models.
+        (actor, actor_optim), (critic, critic_optim) = strategy.prepare((actor, actor_optim), (critic, critic_optim))
+
         experience_maker = NaiveExperienceMaker(actor, critic, reward_model, initial_model, kl_coef)
         replay_buffer = NaiveReplayBuffer(train_batch_size, buffer_limit, buffer_cpu_offload)
         generate_kwargs = _set_default_generate_kwargs(strategy, generate_kwargs, actor)
         super().__init__(strategy, experience_maker, replay_buffer, experience_batch_size, max_epochs, tokenizer,
                          sample_replay_buffer, dataloader_pin_memory, callbacks, **generate_kwargs)
+        
         self.actor = actor
         self.critic = critic
-
+        self.actor_optim = actor_optim
+        self.critic_optim = critic_optim
         self.actor_loss_fn = PolicyLoss(eps_clip)
         self.critic_loss_fn = ValueLoss(value_clip)
+        self.vf_coef = vf_coef
         self.ptx_loss_fn = nn.CrossEntropyLoss(ignore_index=-100)
         self.ptx_coef = ptx_coef
-        self.actor_optim = actor_optim
-        self.critic_optim = critic_optim
+        
 
     def training_step(self, experience: Experience) -> Dict[str, float]:
         self.actor.train()
         self.critic.train()
         # policy loss
         num_actions = experience.action_mask.size(1)
         action_log_probs = self.actor(experience.sequences, num_actions, attention_mask=experience.attention_mask)
@@ -107,14 +121,15 @@
         values = self.critic(experience.sequences,
                              action_mask=experience.action_mask,
                              attention_mask=experience.attention_mask)
         critic_loss = self.critic_loss_fn(values,
                                           experience.values,
                                           experience.reward,
                                           action_mask=experience.action_mask)
+        critic_loss = critic_loss * self.vf_coef
         self.strategy.backward(critic_loss, self.critic, self.critic_optim)
         self.strategy.optimizer_step(self.critic_optim)
         self.critic_optim.zero_grad()
 
         return {'reward': experience.reward.mean().item()}
     
     def save_model(self, path: str, only_rank0: bool = False, tokenizer: Optional[PreTrainedTokenizerBase] = None) -> None:
```

### Comparing `nextgpt-0.0.3/src/nextgpt/trainer/rm.py` & `nextgpt-0.0.4/src/nextgpt/trainer/rm.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,69 +1,102 @@
 from abc import ABC
 from datetime import datetime
 from typing import Optional
 
 import pandas as pd
 import torch
+from torch import nn
 import torch.distributed as dist
-from torch.optim import Optimizer, lr_scheduler
+from torch.optim import Adam, AdamW, Optimizer, lr_scheduler
 from torch.utils.data import DataLoader, Dataset, DistributedSampler
 from tqdm import tqdm
 from transformers.tokenization_utils_base import PreTrainedTokenizerBase
 
 from .strategies import Strategy
+from ..models import LogExpLoss, LogSigLoss
 from .utils import is_rank_0
 
 
 class RewardModelTrainer(ABC):
     """
         Trainer to use while training reward model.
     Args:
         model (torch.nn.Module): the model to train
         strategy (Strategy): the strategy to use for training
-        optim(Optimizer): the optimizer to use for training
-        loss_fn (callable): the loss function to use for training
         train_dataset (Dataset): the dataset to use for training
         valid_dataset (Dataset): the dataset to use for validation
         eval_dataset (Dataset): the dataset to use for evaluation
         batch_size (int, defaults to 1): the batch size while training
         max_epochs (int, defaults to 2): the number of epochs to train
+        loss_fn (str, defaults to 'log_sig'): the loss function name to use for training ('log_sig', 'log_exp')
+        lr (float, defaults to 5e-5): the learning rate
     """
 
     def __init__(
         self,
         model,
         strategy: Strategy,
-        optim: Optimizer,
-        loss_fn,
         train_dataset: Dataset,
         valid_dataset: Dataset,
         eval_dataset: Dataset,
         batch_size: int = 1,
         max_epochs: int = 1,
+        loss_fn: str = "log_sig",
+        lr: float = 5e-5
     ) -> None:
         super().__init__()
         self.strategy = strategy
         self.epochs = max_epochs
+        self.lr = lr
         train_sampler = None
 
         if dist.is_initialized() and dist.get_world_size() > 1:
             train_sampler = DistributedSampler(train_dataset, shuffle=True, seed=42, drop_last=True)
         self.train_dataloader = DataLoader(train_dataset,
                                            shuffle=(train_sampler is None),
                                            sampler=train_sampler,
                                            batch_size=batch_size)
         self.valid_dataloader = DataLoader(valid_dataset, batch_size=batch_size, shuffle=True)
         self.eval_dataloader = DataLoader(eval_dataset, batch_size=batch_size, shuffle=True)
 
         self.model = strategy.setup_model(model)
-        self.loss_fn = loss_fn
+        if "DDP" in str(self.strategy):
+            self.model = self.model.module
+
+        self.loss_fn = self.get_loss_fn(loss_fn)
+        optim = self.get_optimizer()
         self.optimizer = strategy.setup_optimizer(optim, self.model)
         self.scheduler = lr_scheduler.CosineAnnealingLR(self.optimizer, self.train_dataloader.__len__() // 100)
 
+    def get_optimizer(self) -> Optimizer:
+        # optim = Adam(self.model.parameters(), lr=self.lr)
+
+        # TODO: Need to define as arguments.
+        # weight_decay (`float`, *optional*, defaults to 0): The weight decay to apply (if not zero) to all layers except all bias and LayerNorm weights.
+        # adam_beta1 (`float`, *optional*, defaults to 0.9): The beta1 hyperparameter for the [`AdamW`] optimizer.
+        # adam_beta2 (`float`, *optional*, defaults to 0.999): The beta2 hyperparameter for the [`AdamW`] optimizer.
+        # adam_epsilon (`float`, *optional*, defaults to 1e-8):The epsilon hyperparameter for the [`AdamW`] optimizer.
+        weight_decay = 0.0
+        adam_beta1 = 0.9
+        adam_beta2 = 0.999
+        adam_epsilon = 1e-8
+        optim = AdamW(self.model.parameters(), lr=self.lr, betas=(adam_beta1, adam_beta2), eps=adam_epsilon, weight_decay=weight_decay)
+
+        return optim
+    
+    def get_loss_fn(self, loss_fn_name: str) -> nn.Module:
+        if loss_fn_name == "log_sig":
+            loss_fn = LogSigLoss()
+        elif loss_fn_name == "log_exp":
+            loss_fn = LogExpLoss()
+        else:
+            raise ValueError(f"Unsupported loss function: {loss_fn_name}")
+
+        return loss_fn
+    
     def eval_acc(self, dataloader):
         dist = 0
         on = 0
         cnt = 0
         self.model.eval()
         with torch.no_grad():
             for chosen_ids, c_mask, reject_ids, r_mask in dataloader:
```

### Comparing `nextgpt-0.0.3/src/nextgpt/trainer/strategies/base.py` & `nextgpt-0.0.4/src/nextgpt/trainer/strategies/base.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/trainer/strategies/ddp.py` & `nextgpt-0.0.4/src/nextgpt/trainer/strategies/ddp.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/trainer/strategies/naive.py` & `nextgpt-0.0.4/src/nextgpt/trainer/strategies/naive.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt/trainer/strategies/sampler.py` & `nextgpt-0.0.4/src/nextgpt/trainer/strategies/sampler.py`

 * *Files identical despite different names*

### Comparing `nextgpt-0.0.3/src/nextgpt.egg-info/PKG-INFO` & `nextgpt-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,21 @@
-Metadata-Version: 2.1
-Name: nextgpt
-Version: 0.0.3
-Summary: nextGPT
-Home-page: https://github.com/louiezzang/next-gpt
-Author: Younggue Bae
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # nextGPT
 > 📢 Open source implementation for ChatGPT replica to build the end-to-end pipeline from SFT to RLHF.
 
 - 🔥 Step 1) SFT: Surpervised Fine-tuning
 - 🔥 Step 2) RM: Reward Model
 - 🔥 Step 3) PPO: Proximal Policy Optimization
 
+![ChatGPT Diagram](https://openaicom.imgix.net/cf717bdb-0c8c-428a-b82b-3c3add87a600/ChatGPT_Diagram.svg?fm=auto&auto=compress,format&fit=min&w=1919&h=1138)
+
 # Installation
 ```
 $ pip install nextgpt
 ```
-or
+or install from git repo to the get always the latest version.
 ```
 $ git clone https://github.com/louiezzang/next-gpt.git
 $ cd next-gpt/
 $ pip install .
 $ cd ../
 ```
 
@@ -39,10 +31,12 @@
 - https://github.com/airobotlab/KoChatGPT/tree/main/colossalai_ChatGPT_230319
 - https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat
 
 # References
 - https://github.com/airobotlab/KoChatGPT
 - https://github.com/airobotlab/KoChatGPT/tree/main/colossalai_ChatGPT_230319
 - https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat
+- https://github.com/juncongmoo/chatllama
 - https://github.com/huggingface/peft
 - https://github.com/dredwardhyde/gpt-neo-fine-tuning-example/blob/main/gpt_neo.py
 - https://github.com/databrickslabs/dolly
+
```

### Comparing `nextgpt-0.0.3/src/nextgpt.egg-info/SOURCES.txt` & `nextgpt-0.0.4/src/nextgpt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 src/nextgpt/trainer/base.py
 src/nextgpt/trainer/ppo.py
 src/nextgpt/trainer/rm.py
 src/nextgpt/trainer/sft.py
 src/nextgpt/trainer/utils.py
 src/nextgpt/trainer/callbacks/__init__.py
 src/nextgpt/trainer/callbacks/base.py
+src/nextgpt/trainer/callbacks/log_metrics.py
 src/nextgpt/trainer/callbacks/performance_evaluator.py
 src/nextgpt/trainer/callbacks/save_checkpoint.py
 src/nextgpt/trainer/strategies/__init__.py
 src/nextgpt/trainer/strategies/base.py
 src/nextgpt/trainer/strategies/ddp.py
 src/nextgpt/trainer/strategies/naive.py
 src/nextgpt/trainer/strategies/sampler.py
```

