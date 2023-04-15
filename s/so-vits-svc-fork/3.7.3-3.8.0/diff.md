# Comparing `tmp/so_vits_svc_fork-3.7.3.tar.gz` & `tmp/so_vits_svc_fork-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "so_vits_svc_fork-3.7.3.tar", max compression
+gzip compressed data, was "so_vits_svc_fork-3.8.0.tar", max compression
```

## Comparing `so_vits_svc_fork-3.7.3.tar` & `so_vits_svc_fork-3.8.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    12463 2023-04-15 13:39:05.149662 so_vits_svc_fork-3.7.3/LICENSE
--rw-r--r--   0        0        0    17996 2023-04-15 13:39:05.149662 so_vits_svc_fork-3.7.3/README.md
--rw-r--r--   0        0        0     3092 2023-04-15 13:39:06.461681 so_vits_svc_fork-3.7.3/pyproject.toml
--rw-r--r--   0        0        0       70 2023-04-15 13:39:06.397681 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/__init__.py
--rw-r--r--   0        0        0    22740 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/__main__.py
--rw-r--r--   0        0        0     1352 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/cluster/__init__.py
--rw-r--r--   0        0        0     2844 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/cluster/train_cluster.py
--rw-r--r--   0        0        0     2868 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/dataset.py
--rw-r--r--   0        0        0     2454 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/default_gui_presets.json
--rw-r--r--   0        0        0     7267 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/f0.py
--rw-r--r--   0        0        0    25663 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/gui.py
--rw-r--r--   0        0        0      864 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/hparams.py
--rw-r--r--   0        0        0        0 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/inference/__init__.py
--rw-r--r--   0        0        0    24054 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/inference/core.py
--rw-r--r--   0        0        0     7485 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/inference/main.py
--rw-r--r--   0        0        0     1341 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/logger.py
--rw-r--r--   0        0        0        0 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/__init__.py
--rw-r--r--   0        0        0    16683 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/attentions.py
--rw-r--r--   0        0        0     5854 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/commons.py
--rw-r--r--   0        0        0        0 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/decoders/__init__.py
--rw-r--r--   0        0        0     1419 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/decoders/f0.py
--rw-r--r--   0        0        0       76 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
--rw-r--r--   0        0        0    11618 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
--rw-r--r--   0        0        0      340 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
--rw-r--r--   0        0        0      318 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
--rw-r--r--   0        0        0    12477 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
--rw-r--r--   0        0        0      419 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
--rw-r--r--   0        0        0     4725 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
--rw-r--r--   0        0        0     8954 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
--rw-r--r--   0        0        0     4879 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
--rw-r--r--   0        0        0     5604 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/descriminators.py
--rw-r--r--   0        0        0     4400 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/encoders.py
--rw-r--r--   0        0        0     1390 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/flows.py
--rw-r--r--   0        0        0     1405 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/losses.py
--rw-r--r--   0        0        0     5753 2023-04-15 13:39:05.153662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/mel_processing.py
--rw-r--r--   0        0        0    14435 2023-04-15 13:39:05.157662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/modules.py
--rw-r--r--   0        0        0     8178 2023-04-15 13:39:05.157662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/synthesizers.py
--rw-r--r--   0        0        0        0 2023-04-15 13:39:05.157662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/preprocessing/__init__.py
--rw-r--r--   0        0        0     1671 2023-04-15 13:39:05.157662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
--rw-r--r--   0        0        0     1421 2023-04-15 13:39:05.157662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
--rw-r--r--   0        0        0     1482 2023-04-15 13:39:05.157662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
--rw-r--r--   0        0        0     2793 2023-04-15 13:39:05.157662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
--rw-r--r--   0        0        0     4646 2023-04-15 13:39:05.157662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
--rw-r--r--   0        0        0     4382 2023-04-15 13:39:05.157662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
--rw-r--r--   0        0        0     2948 2023-04-15 13:39:05.157662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
--rw-r--r--   0        0        0     1878 2023-04-15 13:39:05.157662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/preprocessing/preprocess_split.py
--rw-r--r--   0        0        0      126 2023-04-15 13:39:05.157662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
--rw-r--r--   0        0        0        0 2023-04-15 13:39:05.157662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/py.typed
--rw-r--r--   0        0        0    18464 2023-04-15 13:39:05.157662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/train.py
--rw-r--r--   0        0        0    13208 2023-04-15 13:39:05.157662 so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/utils.py
--rw-r--r--   0        0        0    19923 1970-01-01 00:00:00.000000 so_vits_svc_fork-3.7.3/PKG-INFO
+-rw-r--r--   0        0        0    12463 2023-04-15 15:04:18.858526 so_vits_svc_fork-3.8.0/LICENSE
+-rw-r--r--   0        0        0    18160 2023-04-15 15:04:18.858526 so_vits_svc_fork-3.8.0/README.md
+-rw-r--r--   0        0        0     3092 2023-04-15 15:04:19.878532 so_vits_svc_fork-3.8.0/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-04-15 15:04:19.830532 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/__init__.py
+-rw-r--r--   0        0        0    22740 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/__main__.py
+-rw-r--r--   0        0        0     1352 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/cluster/__init__.py
+-rw-r--r--   0        0        0     2844 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/cluster/train_cluster.py
+-rw-r--r--   0        0        0     2868 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/dataset.py
+-rw-r--r--   0        0        0     2454 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/default_gui_presets.json
+-rw-r--r--   0        0        0     7267 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/f0.py
+-rw-r--r--   0        0        0    25663 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/gui.py
+-rw-r--r--   0        0        0      864 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/hparams.py
+-rw-r--r--   0        0        0        0 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/inference/__init__.py
+-rw-r--r--   0        0        0    24054 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/inference/core.py
+-rw-r--r--   0        0        0     7485 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/inference/main.py
+-rw-r--r--   0        0        0     1341 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/logger.py
+-rw-r--r--   0        0        0        0 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/__init__.py
+-rw-r--r--   0        0        0    16683 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/attentions.py
+-rw-r--r--   0        0        0     5854 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/commons.py
+-rw-r--r--   0        0        0        0 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/decoders/__init__.py
+-rw-r--r--   0        0        0     1419 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/decoders/f0.py
+-rw-r--r--   0        0        0       76 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
+-rw-r--r--   0        0        0    11618 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
+-rw-r--r--   0        0        0      340 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
+-rw-r--r--   0        0        0      318 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
+-rw-r--r--   0        0        0    12477 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
+-rw-r--r--   0        0        0      419 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
+-rw-r--r--   0        0        0     4725 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
+-rw-r--r--   0        0        0     8954 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
+-rw-r--r--   0        0        0     4879 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
+-rw-r--r--   0        0        0     5604 2023-04-15 15:04:18.862526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/descriminators.py
+-rw-r--r--   0        0        0     4400 2023-04-15 15:04:18.866526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/encoders.py
+-rw-r--r--   0        0        0     1390 2023-04-15 15:04:18.866526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/flows.py
+-rw-r--r--   0        0        0     1405 2023-04-15 15:04:18.866526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/losses.py
+-rw-r--r--   0        0        0     5753 2023-04-15 15:04:18.866526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/mel_processing.py
+-rw-r--r--   0        0        0    14435 2023-04-15 15:04:18.866526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/modules.py
+-rw-r--r--   0        0        0     8178 2023-04-15 15:04:18.866526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/synthesizers.py
+-rw-r--r--   0        0        0        0 2023-04-15 15:04:18.866526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/preprocessing/__init__.py
+-rw-r--r--   0        0        0     1671 2023-04-15 15:04:18.866526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
+-rw-r--r--   0        0        0     1421 2023-04-15 15:04:18.866526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
+-rw-r--r--   0        0        0     1482 2023-04-15 15:04:18.866526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
+-rw-r--r--   0        0        0     2793 2023-04-15 15:04:18.866526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
+-rw-r--r--   0        0        0     4646 2023-04-15 15:04:18.866526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
+-rw-r--r--   0        0        0     4382 2023-04-15 15:04:18.866526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
+-rw-r--r--   0        0        0     2948 2023-04-15 15:04:18.866526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
+-rw-r--r--   0        0        0     1878 2023-04-15 15:04:18.866526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py
+-rw-r--r--   0        0        0      126 2023-04-15 15:04:18.866526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
+-rw-r--r--   0        0        0        0 2023-04-15 15:04:18.866526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/py.typed
+-rw-r--r--   0        0        0    19816 2023-04-15 15:04:18.866526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/train.py
+-rw-r--r--   0        0        0    13208 2023-04-15 15:04:18.866526 so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/utils.py
+-rw-r--r--   0        0        0    20087 1970-01-01 00:00:00.000000 so_vits_svc_fork-3.8.0/PKG-INFO
```

### Comparing `so_vits_svc_fork-3.7.3/LICENSE` & `so_vits_svc_fork-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/README.md` & `so_vits_svc_fork-3.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -176,16 +176,16 @@
 svc pre-config
 svc pre-hubert
 svc train -t
 ```
 
 #### Notes
 
-- Dataset audio duration per file should be <~ 10s or VRAM will run out.
-- It is recommended to increase the `batch_size` as much as possible in `config.json` before the `train` command to match the VRAM capacity.
+- Dataset audio duration per file should be <~ 10s.
+- It is recommended to increase the `batch_size` as much as possible in `config.json` before the `train` command to match the VRAM capacity. Setting `batch_size` to `auto-{init_batch_size}-{max_n_trials}` (or simply `auto`) will automatically increase `batch_size` until OOM error occurs, but may not be useful in some cases.
 - To use `CREPE`, replace `svc pre-hubert` with `svc pre-hubert -fm crepe`.
 - To use `QuickVC`, replace `svc pre-config` with `svc pre-config -t quickvc`.
 - Silence removal and volume normalization are automatically performed (as in the upstream repo) and are not required.
 
 ### Further help
 
 For more details, run `svc -h` or `svc <subcommand> -h`.
```

#### html2text {}

```diff
@@ -70,18 +70,20 @@
 code and then add a payment method, you may save about $5 on your first month's
 monthly billing. Note that both referral rewards are Paperspace credits and not
 cash. It was a tough decision but inserted because debugging and training the
 initial model requires a large amount of computing power and the developer is a
 student. #### Local Place your dataset like `dataset_raw/{speaker_id}/**/
 {wav_file}.{any_format}` (subfolders and non-ASCII filenames are acceptable)
 and run: ```shell svc pre-resample svc pre-config svc pre-hubert svc train -
-t ``` #### Notes - Dataset audio duration per file should be <~ 10s or VRAM
-will run out. - It is recommended to increase the `batch_size` as much as
-possible in `config.json` before the `train` command to match the VRAM
-capacity. - To use `CREPE`, replace `svc pre-hubert` with `svc pre-hubert -fm
+t ``` #### Notes - Dataset audio duration per file should be <~ 10s. - It is
+recommended to increase the `batch_size` as much as possible in `config.json`
+before the `train` command to match the VRAM capacity. Setting `batch_size` to
+`auto-{init_batch_size}-{max_n_trials}` (or simply `auto`) will automatically
+increase `batch_size` until OOM error occurs, but may not be useful in some
+cases. - To use `CREPE`, replace `svc pre-hubert` with `svc pre-hubert -fm
 crepe`. - To use `QuickVC`, replace `svc pre-config` with `svc pre-config -
 t quickvc`. - Silence removal and volume normalization are automatically
 performed (as in the upstream repo) and are not required. ### Further help For
 more details, run `svc -h` or `svc  -h`. ```shell > svc -h Usage: svc [OPTIONS]
 COMMAND [ARGS]... so-vits-svc allows any folder structure for training data.
 However, the following folder structure is recommended. When training:
 dataset_raw/{speaker_name}/**/{wav_name}.{any_format} When inference: configs/
```

### Comparing `so_vits_svc_fork-3.7.3/pyproject.toml` & `so_vits_svc_fork-3.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "so-vits-svc-fork"
-version = "3.7.3"
+version = "3.8.0"
 description = "A fork of so-vits-svc."
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/so-vits-svc-fork"
 documentation = "https://so-vits-svc-fork.readthedocs.io"
 classifiers = [
```

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/__main__.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/__main__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/cluster/__init__.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/cluster/train_cluster.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/cluster/train_cluster.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/dataset.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/dataset.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/default_gui_presets.json` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/default_gui_presets.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/f0.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/gui.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/gui.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/hparams.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/hparams.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/inference/core.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/inference/core.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/inference/main.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/inference/main.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/logger.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/logger.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/attentions.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/attentions.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/commons.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/commons.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/decoders/f0.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/decoders/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/descriminators.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/descriminators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/encoders.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/flows.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/flows.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/losses.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/losses.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/mel_processing.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/mel_processing.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/modules.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/modules.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/modules/synthesizers.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/modules/synthesizers.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/preprocessing/preprocess_resample.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/preprocessing/preprocess_split.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/train.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/train.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pathlib import Path
 from typing import Any
 
 import lightning.pytorch as pl
 import torch
 from lightning.pytorch.accelerators import TPUAccelerator
 from lightning.pytorch.loggers import TensorBoardLogger
+from lightning.pytorch.tuner import Tuner
 from torch.cuda.amp import autocast
 from torch.nn import functional as F
 from torch.utils.data import DataLoader
 from torch.utils.tensorboard.writer import SummaryWriter
 
 import so_vits_svc_fork.f0
 import so_vits_svc_fork.modules.commons as commons
@@ -29,29 +30,34 @@
 
 LOG = getLogger(__name__)
 torch.backends.cudnn.benchmark = True
 torch.set_float32_matmul_precision("high")
 
 
 class VCDataModule(pl.LightningDataModule):
+    batch_size: int
+
     def __init__(self, hparams: Any):
         super().__init__()
         self.__hparams = hparams
+        self.batch_size = hparams.train.batch_size
+        if not isinstance(self.batch_size, int):
+            self.batch_size = 1
         self.collate_fn = TextAudioCollate()
 
         # these should be called in setup(), but we need to calculate check_val_every_n_epoch
         self.train_dataset = TextAudioDataset(self.__hparams, is_validation=False)
         self.val_dataset = TextAudioDataset(self.__hparams, is_validation=True)
 
     def train_dataloader(self):
         return DataLoader(
             self.train_dataset,
             # pin_memory=False,
             num_workers=min(cpu_count(), self.__hparams.train.get("num_workers", 4)),
-            batch_size=self.__hparams.train.batch_size,
+            batch_size=self.batch_size,
             collate_fn=self.collate_fn,
         )
 
     def val_dataloader(self):
         return DataLoader(
             self.val_dataset,
             # pin_memory=False,
@@ -86,15 +92,45 @@
         if hparams.train.fp16_run
         else "bf16-mixed"
         if hparams.train.get("bf16_run", False)
         else 32,
         strategy=strategy,
         callbacks=[pl.callbacks.RichProgressBar()] if not is_notebook() else None,
     )
+    tuner = Tuner(trainer)
     model = VitsLightning(reset_optimizer=reset_optimizer, **hparams)
+
+    # automatic batch size scaling
+    batch_size = hparams.train.batch_size
+    batch_split = str(batch_size).split("-")
+    batch_size = batch_split[0]
+    init_val = 2 if len(batch_split) <= 1 else int(batch_split[1])
+    max_trials = 25 if len(batch_split) <= 2 else int(batch_split[2])
+    if batch_size == "auto":
+        batch_size = "binsearch"
+    if batch_size in ["power", "binsearch"]:
+        model.tuning = True
+        tuner.scale_batch_size(
+            model,
+            mode=batch_size,
+            datamodule=datamodule,
+            steps_per_trial=1,
+            init_val=init_val,
+            max_trials=max_trials,
+        )
+        model.tuning = False
+    else:
+        batch_size = int(batch_size)
+    # automatic learning rate scaling is not supported for multiple optimizers
+    """if hparams.train.learning_rate  == "auto":
+    lr_finder = tuner.lr_find(model)
+    LOG.info(lr_finder.results)
+    fig = lr_finder.plot(suggest=True)
+    fig.savefig(model_path / "lr_finder.png")"""
+
     trainer.fit(model, datamodule=datamodule)
 
 
 class VitsLightning(pl.LightningModule):
     def __init__(self, reset_optimizer: bool = False, **hparams: Any):
         super().__init__()
         self._temp_epoch = 0  # Add this line to initialize the _temp_epoch attribute
@@ -104,41 +140,44 @@
         self.net_g = SynthesizerTrn(
             self.hparams.data.filter_length // 2 + 1,
             self.hparams.train.segment_size // self.hparams.data.hop_length,
             **self.hparams.model,
         )
         self.net_d = MultiPeriodDiscriminator(self.hparams.model.use_spectral_norm)
         self.automatic_optimization = False
+        self.learning_rate = self.hparams.train.learning_rate
         self.optim_g = torch.optim.AdamW(
             self.net_g.parameters(),
-            self.hparams.train.learning_rate,
+            self.learning_rate,
             betas=self.hparams.train.betas,
             eps=self.hparams.train.eps,
         )
         self.optim_d = torch.optim.AdamW(
             self.net_d.parameters(),
-            self.hparams.train.learning_rate,
+            self.learning_rate,
             betas=self.hparams.train.betas,
             eps=self.hparams.train.eps,
         )
         self.scheduler_g = torch.optim.lr_scheduler.ExponentialLR(
             self.optim_g, gamma=self.hparams.train.lr_decay
         )
         self.scheduler_d = torch.optim.lr_scheduler.ExponentialLR(
             self.optim_d, gamma=self.hparams.train.lr_decay
         )
         self.optimizers_count = 2
         self.load(reset_optimizer)
+        self.tuning = False
 
     def on_train_start(self) -> None:
-        self.set_current_epoch(self._temp_epoch)
-        total_batch_idx = self._temp_epoch * len(self.trainer.train_dataloader)
-        self.set_total_batch_idx(total_batch_idx)
-        global_step = total_batch_idx * self.optimizers_count
-        self.set_global_step(global_step)
+        if not self.tuning:
+            self.set_current_epoch(self._temp_epoch)
+            total_batch_idx = self._temp_epoch * len(self.trainer.train_dataloader)
+            self.set_total_batch_idx(total_batch_idx)
+            global_step = total_batch_idx * self.optimizers_count
+            self.set_global_step(global_step)
 
         # check if using tpu
         if isinstance(self.trainer.accelerator, TPUAccelerator):
             # patch torch.stft to use cpu
             LOG.warning("Using TPU. Patching torch.stft to use cpu.")
 
             def stft(
@@ -393,15 +432,17 @@
                         lf0[0, 0, :].cpu().float().numpy(),
                         norm_lf0[0, 0, :].detach().cpu().float().numpy(),
                     ),
                 }
             )
 
         accumulate_grad_batches = self.hparams.train.get("accumulate_grad_batches", 1)
-        should_update = (batch_idx + 1) % accumulate_grad_batches == 0
+        should_update = (
+            batch_idx + 1
+        ) % accumulate_grad_batches == 0 or self.trainer.is_last_batch
         # optimizer
         self.manual_backward(loss_gen_all / accumulate_grad_batches)
         if should_update:
             self.log_(
                 "grad_norm_g", commons.clip_grad_value_(self.net_g.parameters(), None)
             )
             optim_g.step()
@@ -458,22 +499,22 @@
                 }
             )
             if self.current_epoch == 0 or batch_idx != 0:
                 return
             utils.save_checkpoint(
                 self.net_g,
                 self.optim_g,
-                self.hparams.train.learning_rate,
+                self.learning_rate,
                 self.current_epoch + 1,  # prioritize prevention of undervaluation
                 Path(self.hparams.model_dir) / f"G_{self.total_batch_idx}.pth",
             )
             utils.save_checkpoint(
                 self.net_d,
                 self.optim_d,
-                self.hparams.train.learning_rate,
+                self.learning_rate,
                 self.current_epoch + 1,
                 Path(self.hparams.model_dir) / f"D_{self.total_batch_idx}.pth",
             )
             keep_ckpts = self.hparams.train.get("keep_ckpts", 0)
             if keep_ckpts > 0:
                 utils.clean_checkpoints(
                     path_to_models=self.hparams.model_dir,
```

### Comparing `so_vits_svc_fork-3.7.3/src/so_vits_svc_fork/utils.py` & `so_vits_svc_fork-3.8.0/src/so_vits_svc_fork/utils.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.7.3/PKG-INFO` & `so_vits_svc_fork-3.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: so-vits-svc-fork
-Version: 3.7.3
+Version: 3.8.0
 Summary: A fork of so-vits-svc.
 Home-page: https://github.com/34j/so-vits-svc-fork
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -233,16 +233,16 @@
 svc pre-config
 svc pre-hubert
 svc train -t
 ```
 
 #### Notes
 
-- Dataset audio duration per file should be <~ 10s or VRAM will run out.
-- It is recommended to increase the `batch_size` as much as possible in `config.json` before the `train` command to match the VRAM capacity.
+- Dataset audio duration per file should be <~ 10s.
+- It is recommended to increase the `batch_size` as much as possible in `config.json` before the `train` command to match the VRAM capacity. Setting `batch_size` to `auto-{init_batch_size}-{max_n_trials}` (or simply `auto`) will automatically increase `batch_size` until OOM error occurs, but may not be useful in some cases.
 - To use `CREPE`, replace `svc pre-hubert` with `svc pre-hubert -fm crepe`.
 - To use `QuickVC`, replace `svc pre-config` with `svc pre-config -t quickvc`.
 - Silence removal and volume normalization are automatically performed (as in the upstream repo) and are not required.
 
 ### Further help
 
 For more details, run `svc -h` or `svc <subcommand> -h`.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 3.7.3 Summary: A fork of
+Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 3.8.0 Summary: A fork of
 so-vits-svc. Home-page: https://github.com/34j/so-vits-svc-fork License: MIT
 Author: 34j Author-email: 34j.95a2p@simplelogin.com Requires-Python:
 >=3.8,<3.11 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
@@ -96,18 +96,20 @@
 code and then add a payment method, you may save about $5 on your first month's
 monthly billing. Note that both referral rewards are Paperspace credits and not
 cash. It was a tough decision but inserted because debugging and training the
 initial model requires a large amount of computing power and the developer is a
 student. #### Local Place your dataset like `dataset_raw/{speaker_id}/**/
 {wav_file}.{any_format}` (subfolders and non-ASCII filenames are acceptable)
 and run: ```shell svc pre-resample svc pre-config svc pre-hubert svc train -
-t ``` #### Notes - Dataset audio duration per file should be <~ 10s or VRAM
-will run out. - It is recommended to increase the `batch_size` as much as
-possible in `config.json` before the `train` command to match the VRAM
-capacity. - To use `CREPE`, replace `svc pre-hubert` with `svc pre-hubert -fm
+t ``` #### Notes - Dataset audio duration per file should be <~ 10s. - It is
+recommended to increase the `batch_size` as much as possible in `config.json`
+before the `train` command to match the VRAM capacity. Setting `batch_size` to
+`auto-{init_batch_size}-{max_n_trials}` (or simply `auto`) will automatically
+increase `batch_size` until OOM error occurs, but may not be useful in some
+cases. - To use `CREPE`, replace `svc pre-hubert` with `svc pre-hubert -fm
 crepe`. - To use `QuickVC`, replace `svc pre-config` with `svc pre-config -
 t quickvc`. - Silence removal and volume normalization are automatically
 performed (as in the upstream repo) and are not required. ### Further help For
 more details, run `svc -h` or `svc  -h`. ```shell > svc -h Usage: svc [OPTIONS]
 COMMAND [ARGS]... so-vits-svc allows any folder structure for training data.
 However, the following folder structure is recommended. When training:
 dataset_raw/{speaker_name}/**/{wav_name}.{any_format} When inference: configs/
```

