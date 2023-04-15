# Comparing `tmp/hordelib-0.8.5.tar.gz` & `tmp/hordelib-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hordelib-0.8.5.tar", last modified: Fri Apr 14 18:01:02 2023, max compression
+gzip compressed data, was "hordelib-0.8.6.tar", last modified: Sat Apr 15 04:32:42 2023, max compression
```

## Comparing `hordelib-0.8.5.tar` & `hordelib-0.8.6.tar`

### file list

```diff
@@ -1,884 +1,885 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.235533 hordelib-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-14 18:00:47.000000 hordelib-0.8.5/.changelog
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-14 18:00:47.000000 hordelib-0.8.5/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.115531 hordelib-0.8.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.131531 hordelib-0.8.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-14 18:00:47.000000 hordelib-0.8.5/.github/workflows/maintests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-14 18:00:47.000000 hordelib-0.8.5/.github/workflows/prtests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-14 18:00:47.000000 hordelib-0.8.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-14 18:00:47.000000 hordelib-0.8.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20600 2023-04-14 18:00:52.000000 hordelib-0.8.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-14 18:00:47.000000 hordelib-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-14 18:00:47.000000 hordelib-0.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    50219 2023-04-14 18:01:02.235533 hordelib-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-04-14 18:00:47.000000 hordelib-0.8.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-14 18:00:47.000000 hordelib-0.8.5/build_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.131531 hordelib-0.8.5/hordelib/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.135532 hordelib-0.8.5/hordelib/_comfyui/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.135532 hordelib-0.8.5/hordelib/_comfyui/comfy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.135532 hordelib-0.8.5/hordelib/_comfyui/comfy/cldm/
--rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/cldm/cldm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/cli_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/clip_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/clip_vision_config_h.json
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/clip_vision_config_vitl.json
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/diffusers_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.135532 hordelib-0.8.5/hordelib/_comfyui/comfy/extra_samplers/
--rw-r--r--   0 runner    (1001) docker     (123)    38450 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.139531 hordelib-0.8.5/hordelib/_comfyui/comfy/k_diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/k_diffusion/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/k_diffusion/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/k_diffusion/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/k_diffusion/external.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/k_diffusion/gns.py
--rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/k_diffusion/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.139531 hordelib-0.8.5/hordelib/_comfyui/comfy/k_diffusion/models/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/k_diffusion/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    26723 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/k_diffusion/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    13168 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/k_diffusion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.139531 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.139531 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/data/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.139531 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/models/
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/models/autoencoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.139531 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/models/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/models/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21367 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py
--rw-r--r--   0 runner    (1001) docker     (123)    89269 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.139531 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66501 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.139531 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/
--rw-r--r--   0 runner    (1001) docker     (123)    21561 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.139531 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37802 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    31860 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.143532 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/ema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.143532 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.143532 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    22341 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.143532 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/
--rw-r--r--   0 runner    (1001) docker     (123)   441072 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png
--rw-r--r--   0 runner    (1001) docker     (123)    29024 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.143532 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/midas/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.143532 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8766 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/tomesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/model_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    23311 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)    38675 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/sd.py
--rw-r--r--   0 runner    (1001) docker     (123)    10816 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/sd1_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/sd1_clip_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.147532 hordelib-0.8.5/hordelib/_comfyui/comfy/sd1_tokenizer/
--rw-r--r--   0 runner    (1001) docker     (123)   524619 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/sd1_tokenizer/special_tokens_map.json
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json
--rw-r--r--   0 runner    (1001) docker     (123)  1059962 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/sd2_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/sd2_clip_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.147532 hordelib-0.8.5/hordelib/_comfyui/comfy/t2i_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/t2i_adapter/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.147532 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.147532 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.151532 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/
--rw-r--r--   0 runner    (1001) docker     (123)    44849 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama
--rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat
--rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py
--rw-r--r--   0 runner    (1001) docker     (123)    52744 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py
--rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py
--rw-r--r--   0 runner    (1001) docker     (123)    51124 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py
--rw-r--r--   0 runner    (1001) docker     (123)    42740 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13485 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.151532 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/
--rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN
--rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    26761 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    24279 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    28520 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    23283 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.151532 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/
--rw-r--r--   0 runner    (1001) docker     (123)    25609 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.155532 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/nodes_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   118577 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/comfyui_screenshot.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.155532 hordelib-0.8.5/hordelib/_comfyui/custom_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/custom_nodes/example_node.py.example
--rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/extra_model_paths.yaml.example
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/folder_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.155532 hordelib-0.8.5/hordelib/_comfyui/input/
--rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/input/example.png
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.119531 hordelib-0.8.5/hordelib/_comfyui/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.155532 hordelib-0.8.5/hordelib/_comfyui/models/checkpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/models/checkpoints/put_checkpoints_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.155532 hordelib-0.8.5/hordelib/_comfyui/models/clip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/models/clip/put_clip_or_text_encoder_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.155532 hordelib-0.8.5/hordelib/_comfyui/models/clip_vision/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/models/clip_vision/put_clip_vision_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.155532 hordelib-0.8.5/hordelib/_comfyui/models/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/models/configs/anything_v3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/models/configs/v1-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/models/configs/v2-inference-v.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/models/configs/v2-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.155532 hordelib-0.8.5/hordelib/_comfyui/models/controlnet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/models/controlnet/put_controlnets_and_t2i_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.155532 hordelib-0.8.5/hordelib/_comfyui/models/diffusers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/models/diffusers/put_diffusers_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.155532 hordelib-0.8.5/hordelib/_comfyui/models/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/models/embeddings/put_embeddings_or_textual_inversion_concepts_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.155532 hordelib-0.8.5/hordelib/_comfyui/models/loras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/models/loras/put_loras_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.155532 hordelib-0.8.5/hordelib/_comfyui/models/style_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/models/style_models/put_t2i_style_model_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.155532 hordelib-0.8.5/hordelib/_comfyui/models/upscale_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/models/upscale_models/put_esrgan_and_other_upscale_models_here
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.155532 hordelib-0.8.5/hordelib/_comfyui/models/vae/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/models/vae/put_vae_here
--rw-r--r--   0 runner    (1001) docker     (123)    43502 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.155532 hordelib-0.8.5/hordelib/_comfyui/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/notebooks/comfyui_colab.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.155532 hordelib-0.8.5/hordelib/_comfyui/output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/output/_output_images_will_be_put_here
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.155532 hordelib-0.8.5/hordelib/_comfyui/script_examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/script_examples/basic_api_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.155532 hordelib-0.8.5/hordelib/_comfyui/web/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.155532 hordelib-0.8.5/hordelib/_comfyui/web/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.159532 hordelib-0.8.5/hordelib/_comfyui/web/extensions/core/
--rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/web/extensions/core/colorPalette.js
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/web/extensions/core/nodeTemplates.js
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/web/extensions/core/rerouteNode.js
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/web/extensions/core/slotDefaults.js
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/web/extensions/core/snapToGrid.js
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/web/extensions/core/uploadImage.js
--rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/web/extensions/core/widgetInputs.js
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/web/extensions/logging.js.example
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/web/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/web/jsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.159532 hordelib-0.8.5/hordelib/_comfyui/web/lib/
--rw-r--r--   0 runner    (1001) docker     (123)   480383 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/web/lib/litegraph.core.js
--rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/web/lib/litegraph.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.159532 hordelib-0.8.5/hordelib/_comfyui/web/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/web/scripts/api.js
--rw-r--r--   0 runner    (1001) docker     (123)    30442 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/web/scripts/app.js
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/web/scripts/defaultGraph.js
--rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/web/scripts/pnginfo.js
--rw-r--r--   0 runner    (1001) docker     (123)    14298 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/web/scripts/ui.js
--rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/web/scripts/widgets.js
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-14 18:00:54.000000 hordelib-0.8.5/hordelib/_comfyui/web/style.css
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-14 18:01:01.000000 hordelib-0.8.5/hordelib/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.159532 hordelib-0.8.5/hordelib/blip/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/blip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/blip/caption.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.159532 hordelib-0.8.5/hordelib/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/cache/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.163532 hordelib-0.8.5/hordelib/clip/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/clip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/clip/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/clip/coca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/clip/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/clip/interrogate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.163532 hordelib-0.8.5/hordelib/clip/ranking_lists/
--rw-r--r--   0 runner    (1001) docker     (123)    80572 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/clip/ranking_lists/artists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/clip/ranking_lists/flavors.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/clip/ranking_lists/mediums.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/clip/ranking_lists/movements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/clip/ranking_lists/sites.txt
--rw-r--r--   0 runner    (1001) docker     (123)    22260 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/clip/ranking_lists/tags.txt
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/clip/ranking_lists/techniques.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/clip/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    16450 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/comfy_horde.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/config_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13522 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/horde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/initialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/install_comfy.patch
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/install_comfy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.163532 hordelib-0.8.5/hordelib/model_database/
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_database/aitemplate.json
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_database/blip.json
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_database/clip.json
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_database/codeformer.json
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_database/controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)   218801 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_database/db.json
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_database/db_dep.json
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_database/db_embeds.json
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_database/diffusers.json
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_database/esrgan.json
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_database/gfpgan.json
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_database/med_config.json
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_database/safety_checker.json
--rw-r--r--   0 runner    (1001) docker     (123)   243306 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_database/stable_diffusion.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.167532 hordelib-0.8.5/hordelib/model_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26498 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_manager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_manager/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_manager/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_manager/codeformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_manager/compvis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_manager/controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_manager/diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_manager/esrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_manager/gfpgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    16620 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_manager/hyper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_manager/safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/model_manager/torch_hijack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.167532 hordelib-0.8.5/hordelib/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.167532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.167532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/binary/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.167532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/canny/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/canny/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.167532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/color/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.167532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/hed/
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/install.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.167532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.171532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    22985 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.171532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.171532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py
--rw-r--r--   0 runner    (1001) docker     (123)    28960 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.171532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.171532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.171532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.171532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.175532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.175532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/
--rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)    24104 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.175532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.175532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.175532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.175532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20432 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.175532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.123531 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.175532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.175532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.179532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.179532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_160k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_20k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_40k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_80k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.123531 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.179532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.183532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.183532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.183532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.183532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)    15999 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/swish.py
--rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.187532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)    26048 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.187532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.187532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41996 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.187532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.187532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    25196 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py
--rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.187532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/deprecated.json
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.199532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15624 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py
--rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.199532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.199532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    20867 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.203532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/closure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)    22532 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/iter_timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.203532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.203532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.207533 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.207533 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.207533 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.207533 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19217 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.127531 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.207533 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.207533 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.207533 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13100 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.207533 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.207533 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/base_pixel_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.207533 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.211532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.211532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)    31035 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.211532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.211532 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24415 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py
--rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18518 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18169 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.215533 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.215533 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.215533 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.219533 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.219533 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.219533 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.219533 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.219533 hordelib-0.8.5/hordelib/nodes/facerestore/
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.219533 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.219533 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/align_trans.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.219533 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/retinaface/
--rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py
--rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.219533 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.223533 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.223533 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/autoanchor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/extract_ckpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.223533 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/parsing/bisenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/parsing/parsenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/parsing/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.223533 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23302 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/utils/face_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/facerestore/facelib/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/node_clip_similarities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/node_controlnet_model_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/node_image_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/node_image_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/node_model_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/nodes/node_upscale_model_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.223533 hordelib-0.8.5/hordelib/pipeline_designs/
--rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/pipeline_designs/pipeline_controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/pipeline_designs/pipeline_controlnet_annotator.json
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/pipeline_designs/pipeline_image_facefix.json
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/pipeline_designs/pipeline_image_upscale.json
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/pipeline_designs/pipeline_stable_diffusion.json
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json
--rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.223533 hordelib-0.8.5/hordelib/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/pipelines/pipeline_controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/pipelines/pipeline_controlnet_annotator.json
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/pipelines/pipeline_image_facefix.json
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/pipelines/pipeline_image_upscale.json
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/pipelines/pipeline_stable_diffusion.json
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/pipelines/pipeline_stable_diffusion_paint.json
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/run_comfyui.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/shared_model_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.227533 hordelib-0.8.5/hordelib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.227533 hordelib-0.8.5/hordelib/utils/blip/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/utils/blip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/utils/blip/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)    41379 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/utils/blip/med.py
--rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/utils/blip/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/utils/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/utils/ioredirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-14 18:00:47.000000 hordelib-0.8.5/hordelib/utils/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.131531 hordelib-0.8.5/hordelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    50219 2023-04-14 18:01:01.000000 hordelib-0.8.5/hordelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    49218 2023-04-14 18:01:02.000000 hordelib-0.8.5/hordelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:01:01.000000 hordelib-0.8.5/hordelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-14 18:01:01.000000 hordelib-0.8.5/hordelib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 18:01:01.000000 hordelib-0.8.5/hordelib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.231533 hordelib-0.8.5/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71522 2023-04-14 18:00:47.000000 hordelib-0.8.5/images/test_annotator.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    36815 2023-04-14 18:00:47.000000 hordelib-0.8.5/images/test_db0.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   538159 2023-04-14 18:00:47.000000 hordelib-0.8.5/images/test_facefix.png
--rw-r--r--   0 runner    (1001) docker     (123)  1474994 2023-04-14 18:00:47.000000 hordelib-0.8.5/images/test_inpaint.png
--rw-r--r--   0 runner    (1001) docker     (123)   411844 2023-04-14 18:00:47.000000 hordelib-0.8.5/images/test_inpaint_alpha.png
--rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-04-14 18:00:47.000000 hordelib-0.8.5/images/test_inpaint_mask.png
--rw-r--r--   0 runner    (1001) docker     (123)   407128 2023-04-14 18:00:47.000000 hordelib-0.8.5/images/test_inpaint_original.png
--rw-r--r--   0 runner    (1001) docker     (123)  1467500 2023-04-14 18:00:47.000000 hordelib-0.8.5/images/test_outpaint.png
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-14 18:00:54.000000 hordelib-0.8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-14 18:00:47.000000 hordelib-0.8.5/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-14 18:00:54.000000 hordelib-0.8.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:01:02.235533 hordelib-0.8.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.235533 hordelib-0.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/make_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:01:02.235533 hordelib-0.8.5/tests/model_managers/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/model_managers/test_comvis.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/model_managers/test_diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/model_managers/test_safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/run_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/run_controlnet_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/run_facefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/run_img2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/run_img2img_hires.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/run_img2img_inpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/run_img2img_inpaint_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/run_img2img_outpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/run_inpainting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/run_performance_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/run_txt2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/run_txt2img_hires.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/run_upscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/test_blip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/test_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/test_comfy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/test_horde_controlnet_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/test_horde_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/test_horde_inference_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/test_horde_inference_img2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/test_horde_inference_painting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/test_horde_pp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/test_initialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/test_safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/test_shared_model_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-14 18:00:47.000000 hordelib-0.8.5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-14 18:00:47.000000 hordelib-0.8.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.171921 hordelib-0.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-15 04:32:27.000000 hordelib-0.8.6/.changelog
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-15 04:32:27.000000 hordelib-0.8.6/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.055919 hordelib-0.8.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.067920 hordelib-0.8.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-15 04:32:27.000000 hordelib-0.8.6/.github/workflows/maintests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-15 04:32:27.000000 hordelib-0.8.6/.github/workflows/prtests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-15 04:32:27.000000 hordelib-0.8.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-04-15 04:32:27.000000 hordelib-0.8.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-04-15 04:32:32.000000 hordelib-0.8.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-15 04:32:27.000000 hordelib-0.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-15 04:32:27.000000 hordelib-0.8.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    50219 2023-04-15 04:32:42.171921 hordelib-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-04-15 04:32:27.000000 hordelib-0.8.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-15 04:32:27.000000 hordelib-0.8.6/build_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.067920 hordelib-0.8.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-15 04:32:27.000000 hordelib-0.8.6/examples/run_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-15 04:32:27.000000 hordelib-0.8.6/examples/run_controlnet_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-15 04:32:27.000000 hordelib-0.8.6/examples/run_facefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-15 04:32:27.000000 hordelib-0.8.6/examples/run_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-15 04:32:27.000000 hordelib-0.8.6/examples/run_img2img_hires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-15 04:32:27.000000 hordelib-0.8.6/examples/run_img2img_inpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-15 04:32:27.000000 hordelib-0.8.6/examples/run_img2img_inpaint_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-15 04:32:27.000000 hordelib-0.8.6/examples/run_img2img_outpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-15 04:32:27.000000 hordelib-0.8.6/examples/run_inpainting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-04-15 04:32:27.000000 hordelib-0.8.6/examples/run_performance_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-15 04:32:27.000000 hordelib-0.8.6/examples/run_txt2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-15 04:32:27.000000 hordelib-0.8.6/examples/run_txt2img_hires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-15 04:32:27.000000 hordelib-0.8.6/examples/run_upscale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.071920 hordelib-0.8.6/hordelib/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.071920 hordelib-0.8.6/hordelib/_comfyui/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.075919 hordelib-0.8.6/hordelib/_comfyui/comfy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.075919 hordelib-0.8.6/hordelib/_comfyui/comfy/cldm/
+-rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/cldm/cldm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/cli_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/clip_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/clip_vision_config_h.json
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/clip_vision_config_vitl.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/diffusers_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.075919 hordelib-0.8.6/hordelib/_comfyui/comfy/extra_samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)    38450 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.075919 hordelib-0.8.6/hordelib/_comfyui/comfy/k_diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/k_diffusion/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/k_diffusion/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/k_diffusion/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/k_diffusion/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/k_diffusion/gns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/k_diffusion/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.075919 hordelib-0.8.6/hordelib/_comfyui/comfy/k_diffusion/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/k_diffusion/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26723 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/k_diffusion/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13168 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/k_diffusion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.075919 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.075919 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/data/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.075919 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/models/autoencoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.079920 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/models/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/models/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21367 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89269 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.079920 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66501 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.079920 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)    21561 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.079920 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37802 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31860 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.079920 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/ema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.079920 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.079920 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/image_degradation/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/image_degradation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22341 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.079920 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)   441072 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29024 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.083920 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/midas/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.083920 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/midas/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/midas/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/midas/midas/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8766 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/tomesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/model_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23311 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38675 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/sd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10816 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/sd1_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/sd1_clip_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.083920 hordelib-0.8.6/hordelib/_comfyui/comfy/sd1_tokenizer/
+-rw-r--r--   0 runner    (1001) docker     (123)   524619 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/sd1_tokenizer/special_tokens_map.json
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1059962 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/sd2_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/sd2_clip_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.083920 hordelib-0.8.6/hordelib/_comfyui/comfy/t2i_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/t2i_adapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.087920 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.087920 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.087920 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/
+-rw-r--r--   0 runner    (1001) docker     (123)    44849 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama
+-rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat
+-rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52744 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51124 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42740 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13485 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.091920 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/
+-rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN
+-rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26761 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24279 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28520 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23283 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.091920 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)    25609 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.091920 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/nodes_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118577 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/comfyui_screenshot.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.091920 hordelib-0.8.6/hordelib/_comfyui/custom_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/custom_nodes/example_node.py.example
+-rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/extra_model_paths.yaml.example
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/folder_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.091920 hordelib-0.8.6/hordelib/_comfyui/input/
+-rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/input/example.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.055919 hordelib-0.8.6/hordelib/_comfyui/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.091920 hordelib-0.8.6/hordelib/_comfyui/models/checkpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/models/checkpoints/put_checkpoints_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.091920 hordelib-0.8.6/hordelib/_comfyui/models/clip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/models/clip/put_clip_or_text_encoder_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.091920 hordelib-0.8.6/hordelib/_comfyui/models/clip_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/models/clip_vision/put_clip_vision_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.095920 hordelib-0.8.6/hordelib/_comfyui/models/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/models/configs/anything_v3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/models/configs/v1-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/models/configs/v2-inference-v.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/models/configs/v2-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.095920 hordelib-0.8.6/hordelib/_comfyui/models/controlnet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/models/controlnet/put_controlnets_and_t2i_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.095920 hordelib-0.8.6/hordelib/_comfyui/models/diffusers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/models/diffusers/put_diffusers_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.095920 hordelib-0.8.6/hordelib/_comfyui/models/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/models/embeddings/put_embeddings_or_textual_inversion_concepts_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.095920 hordelib-0.8.6/hordelib/_comfyui/models/loras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/models/loras/put_loras_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.095920 hordelib-0.8.6/hordelib/_comfyui/models/style_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/models/style_models/put_t2i_style_model_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.095920 hordelib-0.8.6/hordelib/_comfyui/models/upscale_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/models/upscale_models/put_esrgan_and_other_upscale_models_here
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.095920 hordelib-0.8.6/hordelib/_comfyui/models/vae/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/models/vae/put_vae_here
+-rw-r--r--   0 runner    (1001) docker     (123)    43502 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.095920 hordelib-0.8.6/hordelib/_comfyui/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/notebooks/comfyui_colab.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.095920 hordelib-0.8.6/hordelib/_comfyui/output/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/output/_output_images_will_be_put_here
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.095920 hordelib-0.8.6/hordelib/_comfyui/script_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/script_examples/basic_api_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.095920 hordelib-0.8.6/hordelib/_comfyui/web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.095920 hordelib-0.8.6/hordelib/_comfyui/web/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.095920 hordelib-0.8.6/hordelib/_comfyui/web/extensions/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/web/extensions/core/colorPalette.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/web/extensions/core/nodeTemplates.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/web/extensions/core/rerouteNode.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/web/extensions/core/slotDefaults.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/web/extensions/core/snapToGrid.js
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/web/extensions/core/uploadImage.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/web/extensions/core/widgetInputs.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/web/extensions/logging.js.example
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/web/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/web/jsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.099920 hordelib-0.8.6/hordelib/_comfyui/web/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)   480383 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/web/lib/litegraph.core.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/web/lib/litegraph.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.099920 hordelib-0.8.6/hordelib/_comfyui/web/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/web/scripts/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)    30442 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/web/scripts/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/web/scripts/defaultGraph.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/web/scripts/pnginfo.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14298 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/web/scripts/ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/web/scripts/widgets.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-15 04:32:34.000000 hordelib-0.8.6/hordelib/_comfyui/web/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-15 04:32:41.000000 hordelib-0.8.6/hordelib/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.099920 hordelib-0.8.6/hordelib/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/blip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/blip/caption.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.099920 hordelib-0.8.6/hordelib/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/cache/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.099920 hordelib-0.8.6/hordelib/clip/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/clip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/clip/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/clip/coca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/clip/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/clip/interrogate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.099920 hordelib-0.8.6/hordelib/clip/ranking_lists/
+-rw-r--r--   0 runner    (1001) docker     (123)    80572 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/clip/ranking_lists/artists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/clip/ranking_lists/flavors.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/clip/ranking_lists/mediums.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/clip/ranking_lists/movements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/clip/ranking_lists/sites.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    22260 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/clip/ranking_lists/tags.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/clip/ranking_lists/techniques.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/clip/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16450 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/comfy_horde.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/config_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13522 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/horde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/install_comfy.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/install_comfy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.103920 hordelib-0.8.6/hordelib/model_database/
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_database/aitemplate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_database/blip.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_database/clip.json
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_database/codeformer.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_database/controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)   218801 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_database/db.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_database/db_dep.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_database/db_embeds.json
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_database/diffusers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_database/esrgan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_database/gfpgan.json
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_database/med_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_database/safety_checker.json
+-rw-r--r--   0 runner    (1001) docker     (123)   243306 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_database/stable_diffusion.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.103920 hordelib-0.8.6/hordelib/model_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28045 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_manager/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_manager/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_manager/codeformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_manager/compvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_manager/controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_manager/diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_manager/esrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_manager/gfpgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16866 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_manager/hyper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_manager/safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/model_manager/torch_hijack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.107920 hordelib-0.8.6/hordelib/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.107920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.107920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/binary/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.107920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/canny/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/canny/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.107920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/color/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.107920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/hed/
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/install.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.107920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.107920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22985 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.107920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.107920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28960 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.111920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.111920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.111920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.111920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.111920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.111920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24104 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.111920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.111920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.111920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/openpose/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.115920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20432 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.115920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.059919 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.115920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.115920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.119920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.119920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_160k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_40k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_80k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.059919 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.119920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.119920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.119920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.119920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.123920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15999 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/swish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.123920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26048 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.123920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.127920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41996 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.127920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.127920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25196 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.127920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/deprecated.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.135920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15624 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.135920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.135920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20867 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.139920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/closure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22532 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/iter_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.139920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.139920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.143920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.143920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.143920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.143920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19217 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.063919 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.143920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.143920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.143920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13100 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.143920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.143920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/base_pixel_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.147920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.147920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.147920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31035 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.147920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.151920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24415 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18518 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18169 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.151920 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.155921 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.155921 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.155921 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.155921 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.155921 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.155921 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.155921 hordelib-0.8.6/hordelib/nodes/facerestore/
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.155921 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.155921 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/align_trans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.159921 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/retinaface/
+-rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.159921 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.159921 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.159921 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/autoanchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/extract_ckpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.159921 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/parsing/bisenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/parsing/parsenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/parsing/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.159921 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23302 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/utils/face_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/facerestore/facelib/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/node_clip_similarities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/node_controlnet_model_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/node_image_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/node_image_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/node_model_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/nodes/node_upscale_model_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.159921 hordelib-0.8.6/hordelib/pipeline_designs/
+-rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/pipeline_designs/pipeline_controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/pipeline_designs/pipeline_controlnet_annotator.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/pipeline_designs/pipeline_image_facefix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/pipeline_designs/pipeline_image_upscale.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/pipeline_designs/pipeline_stable_diffusion.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.163920 hordelib-0.8.6/hordelib/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/pipelines/pipeline_controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/pipelines/pipeline_controlnet_annotator.json
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/pipelines/pipeline_image_facefix.json
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/pipelines/pipeline_image_upscale.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/pipelines/pipeline_stable_diffusion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/pipelines/pipeline_stable_diffusion_paint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/run_comfyui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/shared_model_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.163920 hordelib-0.8.6/hordelib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.163920 hordelib-0.8.6/hordelib/utils/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/utils/blip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/utils/blip/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41379 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/utils/blip/med.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/utils/blip/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/utils/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/utils/ioredirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-15 04:32:27.000000 hordelib-0.8.6/hordelib/utils/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.071920 hordelib-0.8.6/hordelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    50219 2023-04-15 04:32:41.000000 hordelib-0.8.6/hordelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    49257 2023-04-15 04:32:42.000000 hordelib-0.8.6/hordelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 04:32:41.000000 hordelib-0.8.6/hordelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-15 04:32:41.000000 hordelib-0.8.6/hordelib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-15 04:32:41.000000 hordelib-0.8.6/hordelib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.167921 hordelib-0.8.6/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71522 2023-04-15 04:32:27.000000 hordelib-0.8.6/images/test_annotator.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    36815 2023-04-15 04:32:27.000000 hordelib-0.8.6/images/test_db0.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   538159 2023-04-15 04:32:27.000000 hordelib-0.8.6/images/test_facefix.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1474994 2023-04-15 04:32:27.000000 hordelib-0.8.6/images/test_inpaint.png
+-rw-r--r--   0 runner    (1001) docker     (123)   411844 2023-04-15 04:32:27.000000 hordelib-0.8.6/images/test_inpaint_alpha.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-04-15 04:32:27.000000 hordelib-0.8.6/images/test_inpaint_mask.png
+-rw-r--r--   0 runner    (1001) docker     (123)   407128 2023-04-15 04:32:27.000000 hordelib-0.8.6/images/test_inpaint_original.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1467500 2023-04-15 04:32:27.000000 hordelib-0.8.6/images/test_outpaint.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-15 04:32:34.000000 hordelib-0.8.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-15 04:32:27.000000 hordelib-0.8.6/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-15 04:32:34.000000 hordelib-0.8.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 04:32:42.171921 hordelib-0.8.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.171921 hordelib-0.8.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-15 04:32:27.000000 hordelib-0.8.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-15 04:32:27.000000 hordelib-0.8.6/tests/make_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 04:32:42.171921 hordelib-0.8.6/tests/model_managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-15 04:32:27.000000 hordelib-0.8.6/tests/model_managers/test_comvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-15 04:32:27.000000 hordelib-0.8.6/tests/model_managers/test_diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-15 04:32:27.000000 hordelib-0.8.6/tests/model_managers/test_safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-15 04:32:27.000000 hordelib-0.8.6/tests/test_blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-15 04:32:27.000000 hordelib-0.8.6/tests/test_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-04-15 04:32:27.000000 hordelib-0.8.6/tests/test_comfy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-15 04:32:27.000000 hordelib-0.8.6/tests/test_horde_controlnet_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-15 04:32:27.000000 hordelib-0.8.6/tests/test_horde_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-15 04:32:27.000000 hordelib-0.8.6/tests/test_horde_inference_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-04-15 04:32:27.000000 hordelib-0.8.6/tests/test_horde_inference_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-15 04:32:27.000000 hordelib-0.8.6/tests/test_horde_inference_painting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-04-15 04:32:27.000000 hordelib-0.8.6/tests/test_horde_pp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-15 04:32:27.000000 hordelib-0.8.6/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-15 04:32:27.000000 hordelib-0.8.6/tests/test_initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-15 04:32:27.000000 hordelib-0.8.6/tests/test_safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-15 04:32:27.000000 hordelib-0.8.6/tests/test_shared_model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-15 04:32:27.000000 hordelib-0.8.6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-15 04:32:27.000000 hordelib-0.8.6/tox.ini
```

### Comparing `hordelib-0.8.5/.changelog` & `hordelib-0.8.6/.changelog`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/.github/workflows/maintests.yml` & `hordelib-0.8.6/.github/workflows/prtests.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-name: Tests
+name: Unstable Tests
 
 on:
-  push:
+  pull_request_target:
     branches:
       - main
+    types:
+      - opened
+      - synchronize
     paths:
       - '**.py'
       - '**.json'
 jobs:
   build:
 
     runs-on: self-hosted
@@ -15,28 +18,32 @@
       HORDELIB_TESTING: "no-cuda"
     strategy:
       matrix:
         python: ["3.10"]
 
     steps:
       - uses: actions/checkout@v3
+        with:
+          ref: ${{ github.event.pull_request.head.sha }}
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
       - name: Install tox and any other packages
         run: pip install --upgrade -r requirements.dev.txt
+      - name: Run lint/format check
+        run: tox -e lint-weak-check
       - name: Run tox
         run: tox -e tests
       - name: Run a direct run test
-        run: python -m tests.run_upscale
+        run: python -m examples.run_upscale
       - name: Create CI webpage of results
         run: python -m tests.make_index
       - name: Upload to S3
         uses: shallwefootball/s3-upload-action@master
         id: S3
         with:
           aws_key_id: ${{secrets.S3_BUILD_ARTIFACTS_ACCESS_KEY_ID}}
           aws_secret_access_key: ${{secrets.S3_BUILD_ARTIFACTS_SECRET_ACCESS_KEY}}
           aws_bucket: hordelib
           source_dir: images/
-          destination_dir: ''
+          destination_dir: 'unstable/'
```

### Comparing `hordelib-0.8.5/.github/workflows/prtests.yml` & `hordelib-0.8.6/.github/workflows/maintests.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-name: Unstable Tests
+name: Tests
 
 on:
-  pull_request_target:
+  push:
     branches:
       - main
-    types:
-      - opened
-      - synchronize
     paths:
       - '**.py'
       - '**.json'
 jobs:
   build:
 
     runs-on: self-hosted
@@ -24,22 +21,24 @@
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
       - name: Install tox and any other packages
         run: pip install --upgrade -r requirements.dev.txt
+      - name: Run lint/format check
+        run: tox -e lint-weak-check
       - name: Run tox
         run: tox -e tests
       - name: Run a direct run test
-        run: python -m tests.run_upscale
+        run: python -m examples.run_upscale
       - name: Create CI webpage of results
         run: python -m tests.make_index
       - name: Upload to S3
         uses: shallwefootball/s3-upload-action@master
         id: S3
         with:
           aws_key_id: ${{secrets.S3_BUILD_ARTIFACTS_ACCESS_KEY_ID}}
           aws_secret_access_key: ${{secrets.S3_BUILD_ARTIFACTS_SECRET_ACCESS_KEY}}
           aws_bucket: hordelib
           source_dir: images/
-          destination_dir: 'unstable/'
+          destination_dir: ''
```

### Comparing `hordelib-0.8.5/.github/workflows/release.yml` & `hordelib-0.8.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/.gitignore` & `hordelib-0.8.6/.gitignore`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/CHANGELOG.md` & `hordelib-0.8.6/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 ## hordelib Changelog
 
+## [v0.8.6](https://github.com/jug-dev/hordelib/compare/v0.8.5...v0.8.6)
+
+15 April 2023
+
+- fix: Sha validation fix [`#139`](https://github.com/jug-dev/hordelib/pull/139) (tazlin)
+- fix: pytest discovery, broken by non-tests in test folder [`534695e`](https://github.com/jug-dev/hordelib/commit/534695e10e5f6a94571059a6916d9798867860fa)  (tazlin)
+- fix: switches pr CI to use example/ run_* [`e6ba23e`](https://github.com/jug-dev/hordelib/commit/e6ba23e62bc44eaebe0996201baf807a150a389e)  (tazlin)
+- build: update CI to do a weak lint/formatting check [`6d09423`](https://github.com/jug-dev/hordelib/commit/6d09423e3c8028bc17d0be36f460b9a1963207f1)  (tazlin)
+
 ## [v0.8.5](https://github.com/jug-dev/hordelib/compare/v0.8.4...v0.8.5)
 
 14 April 2023
 
 - test: add threaded torture test [`03bd56a`](https://github.com/jug-dev/hordelib/commit/03bd56a3c40d8ace9dbbb94c0747e207c8442e4a)  (Jug)
 - fix: assert parameter bounds to stop errors [`d1a18f7`](https://github.com/jug-dev/hordelib/commit/d1a18f7659336614738d9106f7ffccc72c1b9de0)  (Jug)
```

### Comparing `hordelib-0.8.5/LICENSE` & `hordelib-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/PKG-INFO` & `hordelib-0.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hordelib
-Version: 0.8.5
+Version: 0.8.6
 Summary: A thin wrapper around ComfyUI to allow use by AI Horde.
 Author-email: Jug <jugdev@proton.me>, db0 <mail@dbzer0.com>, tazlin <tazlin.on.github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hordelib-0.8.5/README.md` & `hordelib-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/build_helper.py` & `hordelib-0.8.6/build_helper.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/LICENSE` & `hordelib-0.8.6/hordelib/_comfyui/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/README.md` & `hordelib-0.8.6/hordelib/_comfyui/README.md`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/cldm/cldm.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/cldm/cldm.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/cli_args.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/cli_args.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/clip_vision.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/clip_vision.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/diffusers_convert.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/diffusers_convert.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/extra_samplers/uni_pc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/k_diffusion/augmentation.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/k_diffusion/augmentation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/k_diffusion/config.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/k_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/k_diffusion/evaluation.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/k_diffusion/evaluation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/k_diffusion/external.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/k_diffusion/external.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/k_diffusion/gns.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/k_diffusion/gns.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/k_diffusion/layers.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/k_diffusion/layers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/k_diffusion/models/image_v1.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/k_diffusion/sampling.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/k_diffusion/sampling.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/k_diffusion/utils.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/k_diffusion/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/data/util.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/data/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/models/autoencoder.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/models/diffusion/ddim.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/models/diffusion/ddpm.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/dpm_solver.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/models/diffusion/dpm_solver/sampler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/models/diffusion/plms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/models/diffusion/sampling_util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/attention.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/openaimodel.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/upscaling.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/diffusionmodules/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/ema.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/ema.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/encoders/kornia_functions.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/encoders/modules.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/encoders/noise_aug_modules.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/image_degradation/bsrgan_light.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils/test.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/image_degradation/utils_image.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/midas/api.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/midas/api.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/midas/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/sub_quadratic_attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/modules/tomesd.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/modules/tomesd.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/ldm/util.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/ldm/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/model_management.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/model_management.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/samplers.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/samplers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/sd.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/sd.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/sd1_clip.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/sd1_clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/sd1_clip_config.json` & `hordelib-0.8.6/hordelib/_comfyui/comfy/sd1_clip_config.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt` & `hordelib-0.8.6/hordelib/_comfyui/comfy/sd1_tokenizer/merges.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json` & `hordelib-0.8.6/hordelib/_comfyui/comfy/sd1_tokenizer/tokenizer_config.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json` & `hordelib-0.8.6/hordelib/_comfyui/comfy/sd1_tokenizer/vocab.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/sd2_clip.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/sd2_clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/sd2_clip_config.json` & `hordelib-0.8.6/hordelib/_comfyui/comfy/sd2_clip_config.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/t2i_adapter/adapter.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/t2i_adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy/utils.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/HAT.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-ESRGAN`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-HAT`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-RealESRGAN`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SPSR`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwiftSRGAN`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-Swin2SR`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-SwinIR`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-lama`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LICENSE-mat`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/LaMa.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/MAT.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/RRDB.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SPSR.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SRVGG.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwiftSRGAN.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/Swin2SR.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/SwinIR.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-GFPGAN`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-RestoreFormer`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/LICENSE-codeformer`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/arcface_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/codeformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/fused_act.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpgan_bilinear_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/gfpganv1_clean_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/restoreformer_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_bilinear_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/stylegan2_clean_arch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/face/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/mat/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/drop.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/helpers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/architecture/timm/weight_init.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/model_loading.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/chainner_models/types.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/chainner_models/types.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/nodes_post_processing.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/nodes_post_processing.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py` & `hordelib-0.8.6/hordelib/_comfyui/comfy_extras/nodes_upscale_model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/comfyui_screenshot.png` & `hordelib-0.8.6/hordelib/_comfyui/comfyui_screenshot.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/custom_nodes/example_node.py.example` & `hordelib-0.8.6/hordelib/_comfyui/custom_nodes/example_node.py.example`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/execution.py` & `hordelib-0.8.6/hordelib/_comfyui/execution.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/extra_model_paths.yaml.example` & `hordelib-0.8.6/hordelib/_comfyui/extra_model_paths.yaml.example`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/folder_paths.py` & `hordelib-0.8.6/hordelib/_comfyui/folder_paths.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/input/example.png` & `hordelib-0.8.6/hordelib/_comfyui/input/example.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/main.py` & `hordelib-0.8.6/hordelib/_comfyui/main.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/models/configs/anything_v3.yaml` & `hordelib-0.8.6/hordelib/_comfyui/models/configs/anything_v3.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/models/configs/v1-inference.yaml` & `hordelib-0.8.6/hordelib/_comfyui/models/configs/v1-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml` & `hordelib-0.8.6/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml` & `hordelib-0.8.6/hordelib/_comfyui/models/configs/v1-inference_clip_skip_2_fp16.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml` & `hordelib-0.8.6/hordelib/_comfyui/models/configs/v1-inference_fp16.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml` & `hordelib-0.8.6/hordelib/_comfyui/models/configs/v1-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/models/configs/v2-inference-v.yaml` & `hordelib-0.8.6/hordelib/_comfyui/models/configs/v2-inference-v.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml` & `hordelib-0.8.6/hordelib/_comfyui/models/configs/v2-inference-v_fp32.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/models/configs/v2-inference.yaml` & `hordelib-0.8.6/hordelib/_comfyui/models/configs/v2-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml` & `hordelib-0.8.6/hordelib/_comfyui/models/configs/v2-inference_fp32.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml` & `hordelib-0.8.6/hordelib/_comfyui/models/configs/v2-inpainting-inference.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/nodes.py` & `hordelib-0.8.6/hordelib/_comfyui/nodes.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/notebooks/comfyui_colab.ipynb` & `hordelib-0.8.6/hordelib/_comfyui/notebooks/comfyui_colab.ipynb`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/script_examples/basic_api_example.py` & `hordelib-0.8.6/hordelib/_comfyui/script_examples/basic_api_example.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/server.py` & `hordelib-0.8.6/hordelib/_comfyui/server.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/web/extensions/core/colorPalette.js` & `hordelib-0.8.6/hordelib/_comfyui/web/extensions/core/colorPalette.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js` & `hordelib-0.8.6/hordelib/_comfyui/web/extensions/core/contextMenuFilter.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js` & `hordelib-0.8.6/hordelib/_comfyui/web/extensions/core/dynamicPrompts.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js` & `hordelib-0.8.6/hordelib/_comfyui/web/extensions/core/invertMenuScrolling.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/web/extensions/core/nodeTemplates.js` & `hordelib-0.8.6/hordelib/_comfyui/web/extensions/core/nodeTemplates.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/web/extensions/core/rerouteNode.js` & `hordelib-0.8.6/hordelib/_comfyui/web/extensions/core/rerouteNode.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js` & `hordelib-0.8.6/hordelib/_comfyui/web/extensions/core/saveImageExtraOutput.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/web/extensions/core/snapToGrid.js` & `hordelib-0.8.6/hordelib/_comfyui/web/extensions/core/snapToGrid.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/web/extensions/core/widgetInputs.js` & `hordelib-0.8.6/hordelib/_comfyui/web/extensions/core/widgetInputs.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/web/extensions/logging.js.example` & `hordelib-0.8.6/hordelib/_comfyui/web/extensions/logging.js.example`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/web/index.html` & `hordelib-0.8.6/hordelib/_comfyui/web/index.html`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/web/lib/litegraph.core.js` & `hordelib-0.8.6/hordelib/_comfyui/web/lib/litegraph.core.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/web/lib/litegraph.css` & `hordelib-0.8.6/hordelib/_comfyui/web/lib/litegraph.css`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/web/scripts/api.js` & `hordelib-0.8.6/hordelib/_comfyui/web/scripts/api.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/web/scripts/app.js` & `hordelib-0.8.6/hordelib/_comfyui/web/scripts/app.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/web/scripts/defaultGraph.js` & `hordelib-0.8.6/hordelib/_comfyui/web/scripts/defaultGraph.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/web/scripts/pnginfo.js` & `hordelib-0.8.6/hordelib/_comfyui/web/scripts/pnginfo.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/web/scripts/ui.js` & `hordelib-0.8.6/hordelib/_comfyui/web/scripts/ui.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/web/scripts/widgets.js` & `hordelib-0.8.6/hordelib/_comfyui/web/scripts/widgets.js`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/_comfyui/web/style.css` & `hordelib-0.8.6/hordelib/_comfyui/web/style.css`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/blip/caption.py` & `hordelib-0.8.6/hordelib/blip/caption.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/cache/cache.py` & `hordelib-0.8.6/hordelib/cache/cache.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/clip/bulk.py` & `hordelib-0.8.6/hordelib/clip/bulk.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/clip/coca.py` & `hordelib-0.8.6/hordelib/clip/coca.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/clip/image.py` & `hordelib-0.8.6/hordelib/clip/image.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/clip/interrogate.py` & `hordelib-0.8.6/hordelib/clip/interrogate.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/clip/ranking_lists/artists.txt` & `hordelib-0.8.6/hordelib/clip/ranking_lists/artists.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/clip/ranking_lists/flavors.txt` & `hordelib-0.8.6/hordelib/clip/ranking_lists/flavors.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/clip/ranking_lists/mediums.txt` & `hordelib-0.8.6/hordelib/clip/ranking_lists/mediums.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/clip/ranking_lists/movements.txt` & `hordelib-0.8.6/hordelib/clip/ranking_lists/movements.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/clip/ranking_lists/tags.txt` & `hordelib-0.8.6/hordelib/clip/ranking_lists/tags.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/clip/ranking_lists/techniques.txt` & `hordelib-0.8.6/hordelib/clip/ranking_lists/techniques.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/clip/text.py` & `hordelib-0.8.6/hordelib/clip/text.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/comfy_horde.py` & `hordelib-0.8.6/hordelib/comfy_horde.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/config_path.py` & `hordelib-0.8.6/hordelib/config_path.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/consts.py` & `hordelib-0.8.6/hordelib/consts.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/horde.py` & `hordelib-0.8.6/hordelib/horde.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/initialisation.py` & `hordelib-0.8.6/hordelib/initialisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,8 +40,10 @@
 
     # Modify python path to include comfyui
     set_system_path()
 
     # Initialise model manager
     from hordelib.shared_model_manager import SharedModelManager
 
+    SharedModelManager()
+
     sys.argv = sys_arg_bkp
```

### Comparing `hordelib-0.8.5/hordelib/install_comfy.patch` & `hordelib-0.8.6/hordelib/install_comfy.patch`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/install_comfy.py` & `hordelib-0.8.6/hordelib/install_comfy.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/model_database/aitemplate.json` & `hordelib-0.8.6/hordelib/model_database/aitemplate.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/model_database/blip.json` & `hordelib-0.8.6/hordelib/model_database/blip.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9921875%*

 * *Differences: {"'BLIP'": "{'config': {'files': {0: {'sha256sum': "*

 * *           "'96ac8749bd0a568c274ebe302b3a3748ab9be614c737f3d8c529697139174086'}}}}",*

 * * "'BLIP_Large'": "{'config': {'files': {0: {'sha256sum': "*

 * *                 "'0d79b3b7c41478b5fe55c35b73ca6f3525a09708289371c6c0fac641e588287e'}}}}"}*

```diff
@@ -7,15 +7,16 @@
                     "file_name": "model__base_caption.pth",
                     "file_path": "",
                     "file_url": "https://storage.googleapis.com/sfr-vision-language-research/BLIP/models/model*_base_caption.pth"
                 }
             ],
             "files": [
                 {
-                    "path": "model__base_caption.pth"
+                    "path": "model__base_caption.pth",
+                    "sha256sum": "96ac8749bd0a568c274ebe302b3a3748ab9be614c737f3d8c529697139174086"
                 }
             ]
         },
         "name": "BLIP",
         "type": "blip"
     },
     "BLIP_Large": {
@@ -26,15 +27,16 @@
                     "file_name": "model_large_caption.pth",
                     "file_path": "",
                     "file_url": "https://storage.googleapis.com/sfr-vision-language-research/BLIP/models/model_large_caption.pth"
                 }
             ],
             "files": [
                 {
-                    "path": "model_large_caption.pth"
+                    "path": "model_large_caption.pth",
+                    "sha256sum": "0d79b3b7c41478b5fe55c35b73ca6f3525a09708289371c6c0fac641e588287e"
                 }
             ]
         },
         "name": "BLIP_Large",
         "type": "blip"
     }
 }
```

### Comparing `hordelib-0.8.5/hordelib/model_database/clip.json` & `hordelib-0.8.6/hordelib/model_database/clip.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984375%*

 * *Differences: {"'ViT-L/14'": "{'config': {'files': {0: {'sha256sum': "*

 * *               "'b8cca3fd41ae0c99ba7e8951adf17d267cdb84cd88be6f7c2e0eca1737a03836'}}}}"}*

```diff
@@ -37,15 +37,16 @@
                     "file_name": "ViT-L-14.pt",
                     "file_path": "",
                     "file_url": "https://openaipublic.azureedge.net/clip/models/b8cca3fd41ae0c99ba7e8951adf17d267cdb84cd88be6f7c2e0eca1737a03836/ViT-L-14.pt"
                 }
             ],
             "files": [
                 {
-                    "path": "ViT-L-14.pt"
+                    "path": "ViT-L-14.pt",
+                    "sha256sum": "b8cca3fd41ae0c99ba7e8951adf17d267cdb84cd88be6f7c2e0eca1737a03836"
                 }
             ]
         },
         "name": "ViT-L/14",
         "type": "clip"
     },
     "ViT-bigG-14": {
```

### Comparing `hordelib-0.8.5/hordelib/model_database/controlnet.json` & `hordelib-0.8.6/hordelib/model_database/controlnet.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982638888888892%*

 * *Differences: {"'control_canny'": "{'config': {'files': {0: {'sha256sum': "*

 * *                    "'231ce6b2760538a3fb77b7cdc40983d460a91a95ab526f920b08f5e750748d9c'}}}}",*

 * * "'control_canny_sd2'": "{'config': {'files': {0: {'sha256sum': "*

 * *                        "'7b2c5d972b6212bb9185e5860e66edd29eeeaeb98d43877688e20c156e196ce4'}}}}",*

 * * "'control_depth'": "{'config': {'files': {0: {'sha256sum': "*

 * *                    "'8b00f19f3f400e3791081ba35c1c615e975d88f5338e7f1bbe09e06465dabc00'}}}}",*

 * * "'control_depth_sd2'": "{'config':  […]*

```diff
@@ -7,15 +7,16 @@
                     "file_name": "diff_control_sd15_canny_fp16.safetensors",
                     "file_path": "",
                     "file_url": "https://huggingface.co/kohya-ss/ControlNet-diff-modules/resolve/main/diff_control_sd15_canny_fp16.safetensors"
                 }
             ],
             "files": [
                 {
-                    "path": "diff_control_sd15_canny_fp16.safetensors"
+                    "path": "diff_control_sd15_canny_fp16.safetensors",
+                    "sha256sum": "231ce6b2760538a3fb77b7cdc40983d460a91a95ab526f920b08f5e750748d9c"
                 },
                 {
                     "path": "cldm_v15.yaml"
                 }
             ]
         },
         "description": "control_canny",
@@ -34,15 +35,16 @@
                     "file_name": "diff_control_sd21_canny_fp16.safetensors",
                     "file_path": "",
                     "file_url": "https://huggingface.co/thibaud/controlnet-sd21/resolve/main/canny-sd21-safe.safetensors"
                 }
             ],
             "files": [
                 {
-                    "path": "diff_control_sd21_canny_fp16.safetensors"
+                    "path": "diff_control_sd21_canny_fp16.safetensors",
+                    "sha256sum": "7b2c5d972b6212bb9185e5860e66edd29eeeaeb98d43877688e20c156e196ce4"
                 },
                 {
                     "path": "cldm_v21.yaml"
                 }
             ]
         },
         "description": "control_canny for sd2.x",
@@ -61,15 +63,16 @@
                     "file_name": "diff_control_sd15_depth_fp16.safetensors",
                     "file_path": "",
                     "file_url": "https://huggingface.co/kohya-ss/ControlNet-diff-modules/resolve/main/diff_control_sd15_depth_fp16.safetensors"
                 }
             ],
             "files": [
                 {
-                    "path": "diff_control_sd15_depth_fp16.safetensors"
+                    "path": "diff_control_sd15_depth_fp16.safetensors",
+                    "sha256sum": "8b00f19f3f400e3791081ba35c1c615e975d88f5338e7f1bbe09e06465dabc00"
                 },
                 {
                     "path": "cldm_v15.yaml"
                 }
             ]
         },
         "description": "control_depth",
@@ -88,15 +91,16 @@
                     "file_name": "diff_control_sd21_depth_fp16.safetensors",
                     "file_path": "",
                     "file_url": "https://huggingface.co/thibaud/controlnet-sd21/resolve/main/depth-sd21-safe.safetensors"
                 }
             ],
             "files": [
                 {
-                    "path": "diff_control_sd21_depth_fp16.safetensors"
+                    "path": "diff_control_sd21_depth_fp16.safetensors",
+                    "sha256sum": "ed33ec158b6ea3bf61494ee71adc16d45886d5f6611d108345a184ebe7d08d81"
                 },
                 {
                     "path": "cldm_v21.yaml"
                 }
             ]
         },
         "description": "control_depth for sd2.x",
@@ -115,15 +119,16 @@
                     "file_name": "control_scribble_fp16.safetensors",
                     "file_path": "",
                     "file_url": "https://huggingface.co/kohya-ss/ControlNet-diff-modules/resolve/main/diff_control_sd15_scribble_fp16.safetensors"
                 }
             ],
             "files": [
                 {
-                    "path": "control_scribble_fp16.safetensors"
+                    "path": "control_scribble_fp16.safetensors",
+                    "sha256sum": "b8be265a72b739f809e461adf985051c925c21e9e22e86987a1519191916fc8d"
                 },
                 {
                     "path": "cldm_v15.yaml"
                 }
             ]
         },
         "description": "control_fakescribbles",
@@ -142,15 +147,16 @@
                     "file_name": "control_scribble_fp21.safetensors",
                     "file_path": "",
                     "file_url": "https://huggingface.co/thibaud/controlnet-sd21/resolve/main/scribble-sd21-safe.safetensors"
                 }
             ],
             "files": [
                 {
-                    "path": "control_scribble_fp21.safetensors"
+                    "path": "control_scribble_fp21.safetensors",
+                    "sha256sum": "7b2ec6479676b52beb8bd22041f6cabbd1a8a16aac7d2d1a3f0e9121edef7b5e"
                 },
                 {
                     "path": "cldm_v21.yaml"
                 }
             ]
         },
         "description": "control_fakescribbles",
@@ -169,15 +175,16 @@
                     "file_name": "diff_control_sd15_hed_fp16.safetensors",
                     "file_path": "",
                     "file_url": "https://huggingface.co/kohya-ss/ControlNet-diff-modules/resolve/main/diff_control_sd15_hed_fp16.safetensors"
                 }
             ],
             "files": [
                 {
-                    "path": "diff_control_sd15_hed_fp16.safetensors"
+                    "path": "diff_control_sd15_hed_fp16.safetensors",
+                    "sha256sum": "b0d250e550cedad78abf96431bb298f23573c6739b57b93475390a5529b85e52"
                 },
                 {
                     "path": "cldm_v15.yaml"
                 }
             ]
         },
         "description": "control_hed",
@@ -196,15 +203,16 @@
                     "file_name": "diff_control_sd21_hed_fp16.safetensors",
                     "file_path": "",
                     "file_url": "https://huggingface.co/thibaud/controlnet-sd21/resolve/main/hed-sd21-safe.safetensors"
                 }
             ],
             "files": [
                 {
-                    "path": "diff_control_sd21_hed_fp16.safetensors"
+                    "path": "diff_control_sd21_hed_fp16.safetensors",
+                    "sha256sum": "c2f7b28a3ba62c372ad8a1baa875ddbecbd0f9f28b899ecd1c6add2c7b71f7cf"
                 },
                 {
                     "path": "cldm_v21.yaml"
                 }
             ]
         },
         "description": "control_hed for sd2.x",
@@ -223,15 +231,16 @@
                     "file_name": "control_mlsd_fp16.safetensors",
                     "file_path": "",
                     "file_url": "https://huggingface.co/kohya-ss/ControlNet-diff-modules/resolve/main/diff_control_sd15_mlsd_fp16.safetensors"
                 }
             ],
             "files": [
                 {
-                    "path": "control_mlsd_fp16.safetensors"
+                    "path": "control_mlsd_fp16.safetensors",
+                    "sha256sum": "948fe030361fad35b974e4d112b0ac94df41d7ab61d7847ad7e7b9a98648cf25"
                 },
                 {
                     "path": "cldm_v15.yaml"
                 }
             ]
         },
         "description": "control_hough",
@@ -250,15 +259,16 @@
                     "file_name": "control_mlsd_fp16.safetensors",
                     "file_path": "",
                     "file_url": "https://huggingface.co/kohya-ss/ControlNet-diff-modules/resolve/main/diff_control_sd15_mlsd_fp16.safetensors"
                 }
             ],
             "files": [
                 {
-                    "path": "control_mlsd_fp16.safetensors"
+                    "path": "control_mlsd_fp16.safetensors",
+                    "sha256sum": "948fe030361fad35b974e4d112b0ac94df41d7ab61d7847ad7e7b9a98648cf25"
                 },
                 {
                     "path": "cldm_v15.yaml"
                 }
             ]
         },
         "description": "control_mlsd",
@@ -277,15 +287,16 @@
                     "file_name": "control_normal_fp16.safetensors",
                     "file_path": "",
                     "file_url": "https://huggingface.co/kohya-ss/ControlNet-diff-modules/resolve/main/diff_control_sd15_normal_fp16.safetensors"
                 }
             ],
             "files": [
                 {
-                    "path": "control_normal_fp16.safetensors"
+                    "path": "control_normal_fp16.safetensors",
+                    "sha256sum": "1007949f163820f5ba324fd78b674fd04423c62ac6b8db1e896b7bf0ab24422c"
                 },
                 {
                     "path": "cldm_v15.yaml"
                 }
             ]
         },
         "description": "control_normal",
@@ -304,15 +315,16 @@
                     "file_name": "control_openpose_fp16.safetensors",
                     "file_path": "",
                     "file_url": "https://huggingface.co/kohya-ss/ControlNet-diff-modules/resolve/main/diff_control_sd15_openpose_fp16.safetensors"
                 }
             ],
             "files": [
                 {
-                    "path": "control_openpose_fp16.safetensors"
+                    "path": "control_openpose_fp16.safetensors",
+                    "sha256sum": "ac1d356292486bbb8d88c67b1099a2b254008b7213149cd874f9506dff81d8da"
                 },
                 {
                     "path": "cldm_v15.yaml"
                 }
             ]
         },
         "description": "control_openpose",
@@ -331,15 +343,16 @@
                     "file_name": "control_openpose_fp21.safetensors",
                     "file_path": "",
                     "file_url": "https://huggingface.co/thibaud/controlnet-sd21/resolve/main/openpose-sd21-safe.safetensors"
                 }
             ],
             "files": [
                 {
-                    "path": "control_openpose_fp21.safetensors"
+                    "path": "control_openpose_fp21.safetensors",
+                    "sha256sum": "9d78ae69920502b7dcbf39cd2ec55c9b91b8852ef0248c9bce1624d972f830c5"
                 },
                 {
                     "path": "cldm_v21.yaml"
                 }
             ]
         },
         "description": "control_openpose for sd2.x",
@@ -358,15 +371,16 @@
                     "file_name": "control_scribble_fp16.safetensors",
                     "file_path": "",
                     "file_url": "https://huggingface.co/kohya-ss/ControlNet-diff-modules/resolve/main/diff_control_sd15_scribble_fp16.safetensors"
                 }
             ],
             "files": [
                 {
-                    "path": "control_scribble_fp16.safetensors"
+                    "path": "control_scribble_fp16.safetensors",
+                    "sha256sum": "b8be265a72b739f809e461adf985051c925c21e9e22e86987a1519191916fc8d"
                 },
                 {
                     "path": "cldm_v15.yaml"
                 }
             ]
         },
         "description": "control_scribble",
@@ -385,15 +399,16 @@
                     "file_name": "control_scribble_fp21.safetensors",
                     "file_path": "",
                     "file_url": "https://huggingface.co/thibaud/controlnet-sd21/resolve/main/scribble-sd21-safe.safetensors"
                 }
             ],
             "files": [
                 {
-                    "path": "control_scribble_fp21.safetensors"
+                    "path": "control_scribble_fp21.safetensors",
+                    "sha256sum": "7b2ec6479676b52beb8bd22041f6cabbd1a8a16aac7d2d1a3f0e9121edef7b5e"
                 },
                 {
                     "path": "cldm_v21.yaml"
                 }
             ]
         },
         "description": "control_scribble for sd2.x",
@@ -412,15 +427,16 @@
                     "file_name": "control_seg_fp16.safetensors",
                     "file_path": "",
                     "file_url": "https://huggingface.co/kohya-ss/ControlNet-diff-modules/resolve/main/diff_control_sd15_seg_fp16.safetensors"
                 }
             ],
             "files": [
                 {
-                    "path": "control_seg_fp16.safetensors"
+                    "path": "control_seg_fp16.safetensors",
+                    "sha256sum": "2471479e29acd24f426ab4aa9cc1598d98d261c3621c91ac70042cdab6cded85"
                 },
                 {
                     "path": "cldm_v15.yaml"
                 }
             ]
         },
         "description": "control_seg",
```

### Comparing `hordelib-0.8.5/hordelib/model_database/db.json` & `hordelib-0.8.6/hordelib/model_database/db.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/model_database/db_dep.json` & `hordelib-0.8.6/hordelib/model_database/db_dep.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/model_database/db_embeds.json` & `hordelib-0.8.6/hordelib/model_database/db_embeds.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/model_database/diffusers.json` & `hordelib-0.8.6/hordelib/model_database/diffusers.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/model_database/safety_checker.json` & `hordelib-0.8.6/hordelib/model_database/safety_checker.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/model_database/stable_diffusion.json` & `hordelib-0.8.6/hordelib/model_database/stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/model_manager/base.py` & `hordelib-0.8.6/hordelib/model_manager/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -147,24 +147,30 @@
         **kwargs,
     ):  # XXX # FIXME
         if model_name not in self.model_reference:
             logger.error(f"{model_name} not found")
             return False
         if model_name not in self.available_models:
             logger.error(f"{model_name} not available")
-            self.download_model(model_name)
+            download_succeeded = self.download_model(model_name)
+            if not download_succeeded:
+                logger.init_err(f"{model_name} failed to download", status="Error")
+                return False
             logger.init_ok(f"{model_name}", status="Downloaded")
         if model_name not in self.loaded_models:
+            model_validated = self.validate_model(model_name)
+            if not model_validated:
+                return False
             logger.init(f"{model_name}", status="Loading")
 
             tic = time.time()
             logger.init(f"{model_name}", status="Loading")
 
             self.loaded_models[model_name] = self.modelToRam(
-                model_name,
+                model_name=model_name,
                 half_precision=half_precision,
                 gpu_id=gpu_id,
                 cpu_only=cpu_only,
                 **kwargs,
             )
             toc = time.time()
 
@@ -317,15 +323,22 @@
         for file_details in files:
             if ".yaml" in file_details["path"]:
                 continue
             if not self.check_file_available(file_details["path"]):
                 logger.debug(f"File {file_details['path']} not found")
                 return False
             if not skip_checksum and not self.validate_file(file_details):
-                logger.debug(f"File {file_details['path']} has invalid checksum")
+                logger.error(f"File {file_details['path']} has invalid checksum")
+                try:
+                    modelPath = Path(self.modelFolderPath).joinpath(file_details["path"])
+                    logger.error(f"Deleting {file_details['path']}.")
+                    modelPath.unlink(True)
+                except OSError as e:
+                    logger.error(f"Unable to delete {file_details['path']}: {e}.")
+                    logger.error(f"Please delete {file_details['path']} if this error persists.")
                 return False
         return True
 
     @staticmethod
     def get_file_md5sum_hash(file_name):  # XXX Convert to path?
         # XXX There *must* be a library for this.
         # Bail out if the source file doesn't exist
@@ -453,39 +466,53 @@
         for file in files:
             if ".yaml" in file["path"]:
                 continue
             if not self.check_file_available(file["path"]):
                 available = False
         return available
 
-    def download_file(self, url: str, filename: str):
+    def download_file(self, url: str, filename: str) -> bool:
         """
         :param url: URL of the file to download. URL is from the model's download list.
         :param file_path: Path of the model's file. File is from the model's files list.
         Downloads a file
         """
         # XXX convert the path nonsense to pathlib
         full_path = f"{self.modelFolderPath}/{filename}"
         os.makedirs(os.path.dirname(full_path), exist_ok=True)
         pbar_desc = full_path.split("/")[-1]
-        r = requests.get(url, stream=True, allow_redirects=True)
-        with open(full_path, "wb") as f, tqdm(
-            # all optional kwargs
-            unit="B",
-            unit_scale=True,
-            unit_divisor=1024,
-            miniters=1,
-            desc=pbar_desc,
-            total=int(r.headers.get("content-length", 0)),
-            disable=WorkerSettings.disable_download_progress.active,
-        ) as pbar:
-            for chunk in r.iter_content(chunk_size=16 * 1024):
-                if chunk:
-                    f.write(chunk)
-                    pbar.update(len(chunk))
+        try:
+            response = requests.get(url, stream=True, allow_redirects=True)
+            with open(full_path, "wb") as f, tqdm(
+                # all optional kwargs
+                unit="B",
+                unit_scale=True,
+                unit_divisor=1024,
+                miniters=1,
+                desc=pbar_desc,
+                total=int(response.headers.get("content-length", 0)),
+                disable=WorkerSettings.disable_download_progress.active,
+            ) as pbar:
+                for chunk in response.iter_content(chunk_size=16 * 1024):
+                    response.raise_for_status()
+                    if chunk:
+                        f.write(chunk)
+                        pbar.update(len(chunk))
+            return True
+        except requests.exceptions.HTTPError as e:
+            logger.error(f"Error downloading {url}: {e}")
+            if os.path.exists(full_path):
+                os.remove(full_path)
+            return False
+        except requests.exceptions.RequestException as e:
+            logger.error(f"Error downloading {url}: {e}")
+            logger.error("Are you connected to the internet?")
+            if os.path.exists(full_path):
+                os.remove(full_path)
+            return False
 
     def download_model(self, model_name: str):
         """
         :param model_name: Name of the model
         Checks if the model is available, downloads the model if it is not available.
         After download, validates the model.
         Returns True if the model is available, False otherwise.
@@ -498,15 +525,15 @@
         - write content to file
         - symlink file
         - delete file
         - unzip file
         """
         # XXX this function is wacky in its premise and needs to be reworked
         if model_name in self.available_models and model_name not in self.tainted_models:
-            logger.info(f"{model_name} is already available.")
+            logger.debug(f"{model_name} is already available.")
             return True
         download = self.get_model_download(model_name)
         files = self.get_model_files(model_name)
         for i in range(len(download)):
             file_path = (
                 f"{download[i]['file_path']}/{download[i]['file_name']}"
                 if "file_path" in download[i]
@@ -532,18 +559,15 @@
                 file_content = download[i]["file_content"]
                 logger.info(f"writing {file_content} to {file_path}")
                 os.makedirs(
                     os.path.join(self.modelFolderPath, download_path),
                     exist_ok=True,
                 )
                 with open(
-                    os.path.join(
-                        self.modelFolderPath,
-                        os.path.join(download_path, download_name),
-                    ),
+                    os.path.join(self.modelFolderPath, os.path.join(download_path, download_name)),
                     "w",
                 ) as f:
                     f.write(file_content)
             elif "symlink" in download[i]:
                 logger.info(f"symlink {file_path} to {download[i]['symlink']}")
                 symlink = download[i]["symlink"]
                 os.makedirs(
@@ -566,34 +590,42 @@
                 git.Git(os.path.join(self.modelFolderPath, file_path)).clone(
                     download_url,
                 )
             elif "unzip" in download[i]:
                 zip_path = f"{self.modelFolderPath}/{download_name}.zip"
                 temp_path = f"{self.modelFolderPath}/{str(uuid4())}/"
                 os.makedirs(temp_path, exist_ok=True)
-                self.download_file(download_url, zip_path)
+
+                download_succeeded = self.download_file(download_url, zip_path)
+                if not download_succeeded:
+                    return False
+
                 logger.info(f"unzip {zip_path}")
                 with zipfile.ZipFile(zip_path, "r") as zip_ref:
                     zip_ref.extractall(temp_path)
+
                 logger.info(f"moving {temp_path} to {download_path}")
                 shutil.move(
                     temp_path,
                     os.path.join(self.modelFolderPath, download_path),
                 )
+
                 logger.info(f"delete {zip_path}")
                 os.remove(zip_path)
+
                 logger.info(f"delete {temp_path}")
                 shutil.rmtree(temp_path)
             else:
                 if not self.check_file_available(file_path) or model_name in self.tainted_models:
                     logger.debug(f"Downloading {download_url} to {file_path}")
-                    self.download_file(download_url, file_path)
-        if not self.validate_model(model_name):
-            return False
-        return True
+                    download_succeeded = self.download_file(download_url, file_path)
+                    if not download_succeeded:
+                        return False
+
+        return self.validate_model(model_name)
 
     def download_all_models(self) -> bool:
         """
         Downloads all models
         """
         # XXX this has no fall back and always returns true
         for model in self.get_filtered_model_names(download_all=True):
```

### Comparing `hordelib-0.8.5/hordelib/model_manager/blip.py` & `hordelib-0.8.6/hordelib/model_manager/blip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/model_manager/clip.py` & `hordelib-0.8.6/hordelib/model_manager/clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/model_manager/codeformer.py` & `hordelib-0.8.6/hordelib/model_manager/codeformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/model_manager/compvis.py` & `hordelib-0.8.6/hordelib/model_manager/compvis.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/model_manager/controlnet.py` & `hordelib-0.8.6/hordelib/model_manager/controlnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/model_manager/diffusers.py` & `hordelib-0.8.6/hordelib/model_manager/diffusers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/model_manager/esrgan.py` & `hordelib-0.8.6/hordelib/model_manager/esrgan.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/model_manager/gfpgan.py` & `hordelib-0.8.6/hordelib/model_manager/gfpgan.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/model_manager/hyper.py` & `hordelib-0.8.6/hordelib/model_manager/hyper.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,17 @@
 
     models: dict  # XXX unclear as to purpose... unused in AI-Horde-Worker?
     available_models: list
     """All models for which information exists, and for which a download attempt could be made."""
     loaded_models: dict
     """All models for which have successfully loaded across all `BaseModelManager` types."""
 
+    active_model_managers: list[BaseModelManager] | None = None
+    """All loaded model managers."""
+
     def __init__(
         self,
     ):
         """Create a new instance of model manager."""
         # logger.initialise_voodoo()
         self.cuda_available = torch.cuda.is_available()
         self.models = {}
@@ -100,36 +103,38 @@
             # at runtime modelmanager() will be CompVisModelManager(), ClipModelManager(), etc
             setattr(
                 self,
                 argName,
                 modelmanager(download_reference=False),
             )  # XXX # FIXME # HACK
 
+        self.active_model_managers = []
         self.refreshManagers()
 
     def refreshManagers(self) -> None:  # XXX rename + docstring rewrite
         """Called when one of the `BaseModelManager` changes, updating `available_models`."""
-        model_types = [
+        _active_model_managers = [
             # self.aitemplate, # XXX TODO
             self.blip,
             self.clip,
             self.compvis,
             self.diffusers,
             self.esrgan,
             self.gfpgan,
             self.safety_checker,
             self.codeformer,
             self.controlnet,
         ]
         # reset available models
         self.available_models = []
-        for model_type in model_types:
-            if model_type is not None:
-                self.models.update(model_type.model_reference)
-                self.available_models.extend(model_type.available_models)
+        for model_manager in _active_model_managers:
+            if model_manager is not None:
+                self.active_model_managers.append(model_manager)
+                self.models.update(model_manager.model_reference)
+                self.available_models.extend(model_manager.available_models)
 
     def reload_database(self) -> None:
         """Completely resets the `BaseModelManager` classes, and forces each to re-init."""
         model_managers: list[BaseModelManager] = []
         for model_manager_type in MODEL_MANAGERS_TYPE_LOOKUP:
             model_managers.append(getattr(self, model_manager_type))
```

### Comparing `hordelib-0.8.5/hordelib/model_manager/safety_checker.py` & `hordelib-0.8.6/hordelib/model_manager/safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/model_manager/torch_hijack.py` & `hordelib-0.8.6/hordelib/model_manager/torch_hijack.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/README.md` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/README.md`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/install.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/install.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/comfy_controlnet_preprocessors/util.py` & `hordelib-0.8.6/hordelib/nodes/comfy_controlnet_preprocessors/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/facerestore/__init__.py` & `hordelib-0.8.6/hordelib/nodes/facerestore/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/__init__.py` & `hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/align_trans.py` & `hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/align_trans.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py` & `hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py` & `hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py` & `hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py` & `hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py` & `hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py` & `hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py` & `hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py` & `hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml` & `hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml` & `hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py` & `hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py` & `hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py` & `hordelib-0.8.6/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/facerestore/facelib/parsing/__init__.py` & `hordelib-0.8.6/hordelib/nodes/facerestore/facelib/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/facerestore/facelib/parsing/bisenet.py` & `hordelib-0.8.6/hordelib/nodes/facerestore/facelib/parsing/bisenet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/facerestore/facelib/parsing/parsenet.py` & `hordelib-0.8.6/hordelib/nodes/facerestore/facelib/parsing/parsenet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/facerestore/facelib/parsing/resnet.py` & `hordelib-0.8.6/hordelib/nodes/facerestore/facelib/parsing/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py` & `hordelib-0.8.6/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/facerestore/facelib/utils/face_utils.py` & `hordelib-0.8.6/hordelib/nodes/facerestore/facelib/utils/face_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/facerestore/facelib/utils/misc.py` & `hordelib-0.8.6/hordelib/nodes/facerestore/facelib/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/node_clip_similarities.py` & `hordelib-0.8.6/hordelib/nodes/node_clip_similarities.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/node_controlnet_model_loader.py` & `hordelib-0.8.6/hordelib/nodes/node_controlnet_model_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/node_image_loader.py` & `hordelib-0.8.6/hordelib/nodes/node_image_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/node_image_output.py` & `hordelib-0.8.6/hordelib/nodes/node_image_output.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/node_model_loader.py` & `hordelib-0.8.6/hordelib/nodes/node_model_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/nodes/node_upscale_model_loader.py` & `hordelib-0.8.6/hordelib/nodes/node_upscale_model_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/pipeline_designs/pipeline_controlnet.json` & `hordelib-0.8.6/hordelib/pipeline_designs/pipeline_controlnet.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/pipeline_designs/pipeline_controlnet_annotator.json` & `hordelib-0.8.6/hordelib/pipeline_designs/pipeline_controlnet_annotator.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/pipeline_designs/pipeline_image_facefix.json` & `hordelib-0.8.6/hordelib/pipeline_designs/pipeline_image_facefix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/pipeline_designs/pipeline_image_upscale.json` & `hordelib-0.8.6/hordelib/pipeline_designs/pipeline_image_upscale.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/pipeline_designs/pipeline_stable_diffusion.json` & `hordelib-0.8.6/hordelib/pipeline_designs/pipeline_stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json` & `hordelib-0.8.6/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json` & `hordelib-0.8.6/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/pipelines/pipeline_controlnet.json` & `hordelib-0.8.6/hordelib/pipelines/pipeline_controlnet.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/pipelines/pipeline_controlnet_annotator.json` & `hordelib-0.8.6/hordelib/pipelines/pipeline_controlnet_annotator.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/pipelines/pipeline_image_facefix.json` & `hordelib-0.8.6/hordelib/pipelines/pipeline_image_facefix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/pipelines/pipeline_image_upscale.json` & `hordelib-0.8.6/hordelib/pipelines/pipeline_image_upscale.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/pipelines/pipeline_stable_diffusion.json` & `hordelib-0.8.6/hordelib/pipelines/pipeline_stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json` & `hordelib-0.8.6/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/pipelines/pipeline_stable_diffusion_paint.json` & `hordelib-0.8.6/hordelib/pipelines/pipeline_stable_diffusion_paint.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/run_comfyui.py` & `hordelib-0.8.6/hordelib/run_comfyui.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/safety_checker.py` & `hordelib-0.8.6/hordelib/safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/shared_model_manager.py` & `hordelib-0.8.6/hordelib/shared_model_manager.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/utils/blip/blip.py` & `hordelib-0.8.6/hordelib/utils/blip/blip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/utils/blip/med.py` & `hordelib-0.8.6/hordelib/utils/blip/med.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/utils/blip/vit.py` & `hordelib-0.8.6/hordelib/utils/blip/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/utils/cast.py` & `hordelib-0.8.6/hordelib/utils/cast.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/utils/ioredirect.py` & `hordelib-0.8.6/hordelib/utils/ioredirect.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib/utils/logger.py` & `hordelib-0.8.6/hordelib/utils/logger.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/hordelib.egg-info/PKG-INFO` & `hordelib-0.8.6/hordelib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hordelib
-Version: 0.8.5
+Version: 0.8.6
 Summary: A thin wrapper around ComfyUI to allow use by AI Horde.
 Author-email: Jug <jugdev@proton.me>, db0 <mail@dbzer0.com>, tazlin <tazlin.on.github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hordelib-0.8.5/hordelib.egg-info/SOURCES.txt` & `hordelib-0.8.6/hordelib.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,27 @@
 pyproject.toml
 requirements.dev.txt
 requirements.txt
 tox.ini
 .github/workflows/maintests.yml
 .github/workflows/prtests.yml
 .github/workflows/release.yml
+examples/run_controlnet.py
+examples/run_controlnet_annotator.py
+examples/run_facefix.py
+examples/run_img2img.py
+examples/run_img2img_hires.py
+examples/run_img2img_inpaint.py
+examples/run_img2img_inpaint_mask.py
+examples/run_img2img_outpaint.py
+examples/run_inpainting.py
+examples/run_performance_test.py
+examples/run_txt2img.py
+examples/run_txt2img_hires.py
+examples/run_upscale.py
 hordelib/__init__.py
 hordelib/_version.py
 hordelib/comfy_horde.py
 hordelib/config_path.py
 hordelib/consts.py
 hordelib/horde.py
 hordelib/initialisation.py
@@ -704,27 +717,14 @@
 images/test_inpaint.png
 images/test_inpaint_alpha.png
 images/test_inpaint_mask.png
 images/test_inpaint_original.png
 images/test_outpaint.png
 tests/__init__.py
 tests/make_index.py
-tests/run_controlnet.py
-tests/run_controlnet_annotator.py
-tests/run_facefix.py
-tests/run_img2img.py
-tests/run_img2img_hires.py
-tests/run_img2img_inpaint.py
-tests/run_img2img_inpaint_mask.py
-tests/run_img2img_outpaint.py
-tests/run_inpainting.py
-tests/run_performance_test.py
-tests/run_txt2img.py
-tests/run_txt2img_hires.py
-tests/run_upscale.py
 tests/test_blip.py
 tests/test_clip.py
 tests/test_comfy.py
 tests/test_horde_controlnet_annotator.py
 tests/test_horde_inference.py
 tests/test_horde_inference_controlnet.py
 tests/test_horde_inference_img2img.py
```

### Comparing `hordelib-0.8.5/images/test_annotator.jpg` & `hordelib-0.8.6/images/test_annotator.jpg`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/images/test_db0.jpg` & `hordelib-0.8.6/images/test_db0.jpg`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/images/test_facefix.png` & `hordelib-0.8.6/images/test_facefix.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/images/test_inpaint.png` & `hordelib-0.8.6/images/test_inpaint.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/images/test_inpaint_alpha.png` & `hordelib-0.8.6/images/test_inpaint_alpha.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/images/test_inpaint_mask.png` & `hordelib-0.8.6/images/test_inpaint_mask.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/images/test_inpaint_original.png` & `hordelib-0.8.6/images/test_inpaint_original.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/images/test_outpaint.png` & `hordelib-0.8.6/images/test_outpaint.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/pyproject.toml` & `hordelib-0.8.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/requirements.txt` & `hordelib-0.8.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/tests/make_index.py` & `hordelib-0.8.6/tests/make_index.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/tests/model_managers/test_comvis.py` & `hordelib-0.8.6/tests/model_managers/test_comvis.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,10 +14,10 @@
         from hordelib.model_manager.compvis import CompVisModelManager
 
         self.compvis_model_manager = CompVisModelManager()
         assert self.compvis_model_manager is not None
         yield
         del self.compvis_model_manager
 
-    def test_safety_checker_load_defaults(self):
+    def test_compvis_load_defaults(self):
         success = self.compvis_model_manager.load("Deliberate")
         assert success
```

### Comparing `hordelib-0.8.5/tests/model_managers/test_diffusers.py` & `hordelib-0.8.6/tests/model_managers/test_diffusers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/tests/model_managers/test_safety_checker.py` & `hordelib-0.8.6/tests/model_managers/test_safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/tests/run_controlnet.py` & `hordelib-0.8.6/examples/run_img2img_hires.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 # This tests running hordelib standalone, as an external caller would use it.
-# Call with: python -m test.run_controlnet
+# Call with: python -m test.run_img2img_hires
 # You need all the deps in whatever environment you are running this.
 import os
 
 import hordelib
 
-hordelib.initialise()
 
-from PIL import Image
+def main():
 
-from hordelib.horde import HordeLib
-from hordelib.shared_model_manager import SharedModelManager
+    hordelib.initialise()
 
-generate = HordeLib()
-SharedModelManager.loadModelManagers(compvis=True, controlnet=True)
-SharedModelManager.manager.load("Deliberate")
-
-data = {
-    "sampler_name": "k_dpmpp_2m",
-    "cfg_scale": 7.5,
-    "denoising_strength": 1.0,
-    "seed": 123456789,
-    "height": 512,
-    "width": 512,
-    "karras": True,
-    "tiling": False,
-    "hires_fix": False,
-    "clip_skip": 1,
-    "control_type": "",
-    "image_is_control": False,
-    "return_control_map": False,
-    "prompt": "a man walking in the snow",
-    "ddim_steps": 25,
-    "n_iter": 1,
-    "model": "Deliberate",
-    "source_image": Image.open("images/test_db0.jpg"),
-    "source_processing": "img2img",
-}
-for preproc in HordeLib.CONTROLNET_IMAGE_PREPROCESSOR_MAP.keys():
-    if preproc == "scribble":
-        # Not valid for normal image input test
-        continue
-    data["control_type"] = preproc
+    from PIL import Image
+
+    from hordelib.horde import HordeLib
+    from hordelib.shared_model_manager import SharedModelManager
+
+    generate = HordeLib()
+    SharedModelManager.loadModelManagers(compvis=True)
+    SharedModelManager.manager.load("Deliberate")
+
+    data = {
+        "sampler_name": "k_dpmpp_2m",
+        "cfg_scale": 7.5,
+        "denoising_strength": 0.3,
+        "seed": 250636385744582,
+        "height": 1024,
+        "width": 1024,
+        "karras": False,
+        "tiling": False,
+        "hires_fix": True,
+        "clip_skip": 1,
+        "control_type": None,
+        "image_is_control": False,
+        "return_control_map": False,
+        "prompt": "a dinosaur",
+        "ddim_steps": 25,
+        "n_iter": 1,
+        "model": "Deliberate",
+        "source_image": Image.open("images/test_db0.jpg"),
+    }
     pil_image = generate.basic_inference(data)
-    pil_image.save(f"images/run_controlnet_{preproc}.webp", quality=90)
+    pil_image.save("images/run_img2img_hires.webp", quality=90)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `hordelib-0.8.5/tests/run_controlnet_annotator.py` & `hordelib-0.8.6/examples/run_controlnet_annotator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,52 @@
 # This tests running hordelib standalone, as an external caller would use it.
 # Call with: python -m test.run_controlnet
 # You need all the deps in whatever environment you are running this.
 import os
 
 import hordelib
 
-hordelib.initialise()
 
-from PIL import Image
+def main():
 
-from hordelib.horde import HordeLib
-from hordelib.shared_model_manager import SharedModelManager
+    hordelib.initialise()
 
-generate = HordeLib()
-SharedModelManager.loadModelManagers(compvis=True, controlnet=True)
-
-data = {
-    "sampler_name": "k_dpmpp_2m",
-    "cfg_scale": 7.5,
-    "denoising_strength": 1.0,
-    "seed": 123456789,
-    "height": 512,
-    "width": 512,
-    "karras": True,
-    "tiling": False,
-    "hires_fix": False,
-    "clip_skip": 1,
-    "control_type": "",
-    "image_is_control": False,
-    "return_control_map": True,
-    "prompt": "a man walking in the snow",
-    "ddim_steps": 25,
-    "n_iter": 1,
-    "model": "Deliberate",
-    "source_image": Image.open("images/test_annotator.jpg"),
-    "source_processing": "img2img",
-}
-for preproc in HordeLib.CONTROLNET_IMAGE_PREPROCESSOR_MAP.keys():
-    if preproc == "scribble":
-        # Not valid for normal image input test
-        continue
-    data["control_type"] = preproc
-    pil_image = generate.basic_inference(data)
-    pil_image.save(f"images/run_annotator_{preproc}.webp", quality=90)
+    from PIL import Image
+
+    from hordelib.horde import HordeLib
+    from hordelib.shared_model_manager import SharedModelManager
+
+    generate = HordeLib()
+    SharedModelManager.loadModelManagers(compvis=True, controlnet=True)
+
+    data = {
+        "sampler_name": "k_dpmpp_2m",
+        "cfg_scale": 7.5,
+        "denoising_strength": 1.0,
+        "seed": 123456789,
+        "height": 512,
+        "width": 512,
+        "karras": True,
+        "tiling": False,
+        "hires_fix": False,
+        "clip_skip": 1,
+        "control_type": "",
+        "image_is_control": False,
+        "return_control_map": True,
+        "prompt": "a man walking in the snow",
+        "ddim_steps": 25,
+        "n_iter": 1,
+        "model": "Deliberate",
+        "source_image": Image.open("images/test_annotator.jpg"),
+        "source_processing": "img2img",
+    }
+    for preproc in HordeLib.CONTROLNET_IMAGE_PREPROCESSOR_MAP.keys():
+        if preproc == "scribble":
+            # Not valid for normal image input test
+            continue
+        data["control_type"] = preproc
+        pil_image = generate.basic_inference(data)
+        pil_image.save(f"images/run_annotator_{preproc}.webp", quality=90)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `hordelib-0.8.5/tests/run_facefix.py` & `hordelib-0.8.6/examples/run_facefix.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 # This tests running hordelib standalone, as an external caller would use it.
 # Call with: python -m test.run_facefix
 # You need all the deps in whatever environment you are running this.
 import os
 
 import hordelib
 
-hordelib.initialise()
 
-from PIL import Image
+def main():
 
-from hordelib.horde import HordeLib
-from hordelib.shared_model_manager import SharedModelManager
+    hordelib.initialise()
 
-generate = HordeLib()
-modeltypes = {
-    # aitemplate
-    "blip": True,
-    "clip": True,
-    "codeformer": True,
-    "compvis": True,
-    "controlnet": True,
-    "diffusers": True,
-    "esrgan": True,
-    "gfpgan": True,
-    "safety_checker": True,
-}
-
-SharedModelManager.loadModelManagers(**modeltypes)
-SharedModelManager.manager.load("CodeFormers")
-
-data = {
-    "model": "CodeFormers",
-    "source_image": Image.open("images/test_facefix.png"),
-}
-pil_image = generate.image_facefix(data)
-pil_image.save("images/run_facefix.webp", quality=90)
+    from PIL import Image
+
+    from hordelib.horde import HordeLib
+    from hordelib.shared_model_manager import SharedModelManager
+
+    generate = HordeLib()
+    modeltypes = {
+        # aitemplate
+        "blip": True,
+        "clip": True,
+        "codeformer": True,
+        "compvis": True,
+        "controlnet": True,
+        "diffusers": True,
+        "esrgan": True,
+        "gfpgan": True,
+        "safety_checker": True,
+    }
+
+    SharedModelManager.loadModelManagers(**modeltypes)
+    SharedModelManager.manager.load("CodeFormers")
+
+    data = {
+        "model": "CodeFormers",
+        "source_image": Image.open("images/test_facefix.png"),
+    }
+    pil_image = generate.image_facefix(data)
+    pil_image.save("images/run_facefix.webp", quality=90)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `hordelib-0.8.5/tests/run_img2img.py` & `hordelib-0.8.6/examples/run_img2img.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 # This tests running hordelib standalone, as an external caller would use it.
 # Call with: python -m test.run_img2img
 # You need all the deps in whatever environment you are running this.
 import os
 
 import hordelib
 
-hordelib.initialise()
 
-from PIL import Image
+def main():
+    hordelib.initialise()
 
-from hordelib.horde import HordeLib
-from hordelib.shared_model_manager import SharedModelManager
+    from PIL import Image
 
-generate = HordeLib()
-SharedModelManager.loadModelManagers(compvis=True)
-SharedModelManager.manager.load("Deliberate")
-
-data = {
-    "sampler_name": "k_dpmpp_2m",
-    "cfg_scale": 7.5,
-    "denoising_strength": 0.4,
-    "seed": 250636385744582,
-    "height": 512,
-    "width": 512,
-    "karras": False,
-    "tiling": False,
-    "hires_fix": False,
-    "clip_skip": 1,
-    "control_type": None,
-    "image_is_control": False,
-    "return_control_map": False,
-    "prompt": "a dinosaur",
-    "ddim_steps": 25,
-    "n_iter": 1,
-    "model": "Deliberate",
-    "source_image": Image.open("images/test_db0.jpg"),
-}
-pil_image = generate.basic_inference(data)
-pil_image.save("images/run_img2img.webp", quality=90)
+    from hordelib.horde import HordeLib
+    from hordelib.shared_model_manager import SharedModelManager
+
+    generate = HordeLib()
+    SharedModelManager.loadModelManagers(compvis=True)
+    SharedModelManager.manager.load("Deliberate")
+
+    data = {
+        "sampler_name": "k_dpmpp_2m",
+        "cfg_scale": 7.5,
+        "denoising_strength": 0.4,
+        "seed": 250636385744582,
+        "height": 512,
+        "width": 512,
+        "karras": False,
+        "tiling": False,
+        "hires_fix": False,
+        "clip_skip": 1,
+        "control_type": None,
+        "image_is_control": False,
+        "return_control_map": False,
+        "prompt": "a dinosaur",
+        "ddim_steps": 25,
+        "n_iter": 1,
+        "model": "Deliberate",
+        "source_image": Image.open("images/test_db0.jpg"),
+    }
+    pil_image = generate.basic_inference(data)
+    pil_image.save("images/run_img2img.webp", quality=90)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `hordelib-0.8.5/tests/run_img2img_hires.py` & `hordelib-0.8.6/examples/run_inpainting.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 # This tests running hordelib standalone, as an external caller would use it.
-# Call with: python -m test.run_img2img_hires
+# Call with: python -m test.run_img2img_inpaint
 # You need all the deps in whatever environment you are running this.
 import os
 
 import hordelib
 
-hordelib.initialise()
 
-from PIL import Image
+def main():
 
-from hordelib.horde import HordeLib
-from hordelib.shared_model_manager import SharedModelManager
+    hordelib.initialise()
 
-generate = HordeLib()
-SharedModelManager.loadModelManagers(compvis=True)
-SharedModelManager.manager.load("Deliberate")
-
-data = {
-    "sampler_name": "k_dpmpp_2m",
-    "cfg_scale": 7.5,
-    "denoising_strength": 0.3,
-    "seed": 250636385744582,
-    "height": 1024,
-    "width": 1024,
-    "karras": False,
-    "tiling": False,
-    "hires_fix": True,
-    "clip_skip": 1,
-    "control_type": None,
-    "image_is_control": False,
-    "return_control_map": False,
-    "prompt": "a dinosaur",
-    "ddim_steps": 25,
-    "n_iter": 1,
-    "model": "Deliberate",
-    "source_image": Image.open("images/test_db0.jpg"),
-}
-pil_image = generate.basic_inference(data)
-pil_image.save("images/run_img2img_hires.webp", quality=90)
+    from PIL import Image
+
+    from hordelib.horde import HordeLib
+    from hordelib.shared_model_manager import SharedModelManager
+
+    generate = HordeLib()
+    SharedModelManager.loadModelManagers(diffusers=True)
+    SharedModelManager.manager.load("stable_diffusion_inpainting")
+
+    data = {
+        "sampler_name": "euler",
+        "cfg_scale": 8,
+        "denoising_strength": 0.72,
+        "seed": 836913938046008,
+        "height": 512,
+        "width": 512,
+        "karras": False,
+        "tiling": False,
+        "hires_fix": False,
+        "clip_skip": 1,
+        "control_type": None,
+        "image_is_control": False,
+        "return_control_map": False,
+        "prompt": "a dinosaur",
+        "ddim_steps": 20,
+        "n_iter": 1,
+        "model": "stable_diffusion_inpainting",
+        "source_image": Image.open("images/test_inpaint.png"),
+        "source_processing": "inpainting",
+    }
+    pil_image = generate.basic_inference(data)
+    pil_image.save("images/run_inpainting.webp", quality=90)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `hordelib-0.8.5/tests/run_img2img_inpaint.py` & `hordelib-0.8.6/examples/run_img2img_inpaint_mask.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 # This tests running hordelib standalone, as an external caller would use it.
-# Call with: python -m test.run_img2img_inpaint
+# Call with: python -m test.run_img2img_inpaint_separate_mask
 # You need all the deps in whatever environment you are running this.
 import os
 
 import hordelib
 
-hordelib.initialise()
 
-from PIL import Image
+def main():
+    hordelib.initialise()
 
-from hordelib.horde import HordeLib
-from hordelib.shared_model_manager import SharedModelManager
+    from PIL import Image
 
-generate = HordeLib()
-SharedModelManager.loadModelManagers(compvis=True)
-SharedModelManager.manager.load("Deliberate")
-
-data = {
-    "sampler_name": "euler",
-    "cfg_scale": 8,
-    "denoising_strength": 0.72,
-    "seed": 836913938046008,
-    "height": 512,
-    "width": 512,
-    "karras": False,
-    "tiling": False,
-    "hires_fix": False,
-    "clip_skip": 1,
-    "control_type": None,
-    "image_is_control": False,
-    "return_control_map": False,
-    "prompt": "a dinosaur",
-    "ddim_steps": 20,
-    "n_iter": 1,
-    "model": "Deliberate",
-    "source_image": Image.open("images/test_inpaint.png"),
-    "source_processing": "inpainting",
-}
-pil_image = generate.basic_inference(data)
-pil_image.save("images/run_img2img_inpaint.webp", quality=90)
+    from hordelib.horde import HordeLib
+    from hordelib.shared_model_manager import SharedModelManager
+
+    generate = HordeLib()
+    SharedModelManager.loadModelManagers(compvis=True, diffusers=True)
+    SharedModelManager.manager.load("stable_diffusion_inpainting")
+
+    data = {
+        "sampler_name": "euler",
+        "cfg_scale": 8,
+        "denoising_strength": 1,
+        "seed": 8369138046008,
+        "height": 512,
+        "width": 512,
+        "karras": False,
+        "tiling": False,
+        "hires_fix": False,
+        "clip_skip": 1,
+        "control_type": None,
+        "image_is_control": False,
+        "return_control_map": False,
+        "prompt": "a dinosaur",
+        "ddim_steps": 20,
+        "n_iter": 1,
+        "model": "stable_diffusion_inpainting",
+        "source_image": Image.open("images/test_inpaint_original.png"),
+        "source_mask": Image.open("images/test_inpaint_mask.png"),
+        "source_processing": "inpainting",
+    }
+    pil_image = generate.basic_inference(data)
+    pil_image.save("images/run_img2img_inpaint_mask.webp", quality=90)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `hordelib-0.8.5/tests/run_img2img_inpaint_mask.py` & `hordelib-0.8.6/examples/run_txt2img.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 # This tests running hordelib standalone, as an external caller would use it.
-# Call with: python -m test.run_img2img_inpaint_separate_mask
+# Call with: python -m test.run_txt2img
 # You need all the deps in whatever environment you are running this.
 import os
 
 import hordelib
 
-hordelib.initialise()
 
-from PIL import Image
+def main():
+    hordelib.initialise()
 
-from hordelib.horde import HordeLib
-from hordelib.shared_model_manager import SharedModelManager
+    from hordelib.horde import HordeLib
+    from hordelib.shared_model_manager import SharedModelManager
 
-generate = HordeLib()
-SharedModelManager.loadModelManagers(compvis=True, diffusers=True)
-SharedModelManager.manager.load("stable_diffusion_inpainting")
-
-data = {
-    "sampler_name": "euler",
-    "cfg_scale": 8,
-    "denoising_strength": 1,
-    "seed": 8369138046008,
-    "height": 512,
-    "width": 512,
-    "karras": False,
-    "tiling": False,
-    "hires_fix": False,
-    "clip_skip": 1,
-    "control_type": None,
-    "image_is_control": False,
-    "return_control_map": False,
-    "prompt": "a dinosaur",
-    "ddim_steps": 20,
-    "n_iter": 1,
-    "model": "stable_diffusion_inpainting",
-    "source_image": Image.open("images/test_inpaint_original.png"),
-    "source_mask": Image.open("images/test_inpaint_mask.png"),
-    "source_processing": "inpainting",
-}
-pil_image = generate.basic_inference(data)
-pil_image.save("images/run_img2img_inpaint_mask.webp", quality=90)
+    generate = HordeLib()
+    SharedModelManager.loadModelManagers(compvis=True)
+    SharedModelManager.manager.load("Deliberate")
+
+    data = {
+        "sampler_name": "k_dpmpp_2m",
+        "cfg_scale": 7.5,
+        "denoising_strength": 1.0,
+        "seed": 123456789,
+        "height": 512,
+        "width": 512,
+        "karras": True,
+        "tiling": False,
+        "hires_fix": False,
+        "clip_skip": 1,
+        "control_type": None,
+        "image_is_control": False,
+        "return_control_map": False,
+        "prompt": "an ancient llamia monster",
+        "ddim_steps": 25,
+        "n_iter": 1,
+        "model": "Deliberate",
+    }
+    pil_image = generate.basic_inference(data)
+    pil_image.save("images/run_txt2img.webp", quality=90)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `hordelib-0.8.5/tests/run_img2img_outpaint.py` & `hordelib-0.8.6/examples/run_controlnet.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,53 @@
 # This tests running hordelib standalone, as an external caller would use it.
-# Call with: python -m test.run_img2img_outpaint
+# Call with: python -m test.run_controlnet
 # You need all the deps in whatever environment you are running this.
 import os
 
 import hordelib
 
-hordelib.initialise()
 
-from PIL import Image
+def main():
 
-from hordelib.horde import HordeLib
-from hordelib.shared_model_manager import SharedModelManager
+    hordelib.initialise()
 
-generate = HordeLib()
-SharedModelManager.loadModelManagers(compvis=True)
-SharedModelManager.manager.load("Deliberate")
-
-data = {
-    "sampler_name": "euler",
-    "cfg_scale": 8.0,
-    "denoising_strength": 1.0,
-    "seed": 836913938046008,
-    "height": 512,
-    "width": 512,
-    "karras": False,
-    "tiling": False,
-    "hires_fix": False,
-    "clip_skip": 1,
-    "control_type": None,
-    "image_is_control": False,
-    "return_control_map": False,
-    "prompt": "a river through the mountains, blue sky with clouds.",
-    "ddim_steps": 20,
-    "n_iter": 1,
-    "model": "Deliberate",
-    "source_image": Image.open("images/test_outpaint.png"),
-    "source_processing": "outpainting",
-}
-pil_image = generate.basic_inference(data)
-pil_image.save("images/run_img2img_outpaint.webp", quality=90)
+    from PIL import Image
+
+    from hordelib.horde import HordeLib
+    from hordelib.shared_model_manager import SharedModelManager
+
+    generate = HordeLib()
+    SharedModelManager.loadModelManagers(compvis=True, controlnet=True)
+    SharedModelManager.manager.load("Deliberate")
+
+    data = {
+        "sampler_name": "k_dpmpp_2m",
+        "cfg_scale": 7.5,
+        "denoising_strength": 1.0,
+        "seed": 123456789,
+        "height": 512,
+        "width": 512,
+        "karras": True,
+        "tiling": False,
+        "hires_fix": False,
+        "clip_skip": 1,
+        "control_type": "",
+        "image_is_control": False,
+        "return_control_map": False,
+        "prompt": "a man walking in the snow",
+        "ddim_steps": 25,
+        "n_iter": 1,
+        "model": "Deliberate",
+        "source_image": Image.open("images/test_db0.jpg"),
+        "source_processing": "img2img",
+    }
+    for preproc in HordeLib.CONTROLNET_IMAGE_PREPROCESSOR_MAP.keys():
+        if preproc == "scribble":
+            # Not valid for normal image input test
+            continue
+        data["control_type"] = preproc
+        pil_image = generate.basic_inference(data)
+        pil_image.save(f"images/run_controlnet_{preproc}.webp", quality=90)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `hordelib-0.8.5/tests/run_performance_test.py` & `hordelib-0.8.6/examples/run_performance_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,168 +2,173 @@
 # Call with: python -m test.run_performance_test
 # You need all the deps in whatever environment you are running this.
 import os
 import time
 
 import hordelib
 
-hordelib.initialise()
 
-import threading
+def main():
+    hordelib.initialise()
 
-from loguru import logger
-from PIL import Image
-
-from hordelib.horde import HordeLib
-from hordelib.shared_model_manager import SharedModelManager
-
-generate = HordeLib()
-SharedModelManager.loadModelManagers(compvis=True)
-SharedModelManager.manager.load("Deliberate")
-SharedModelManager.manager.load("Anything Diffusion")
-SharedModelManager.manager.load("Realistic Vision")
-SharedModelManager.manager.load("Papercutcraft")
-
-
-def generate_images(model, threadid, count):
-    data = {
-        "sampler_name": "k_dpmpp_2m",
-        "cfg_scale": 7.5,
-        "denoising_strength": 1.0,
-        "seed": 123456789,
-        "height": 512,
-        "width": 512,
-        "karras": True,
-        "tiling": False,
-        "hires_fix": False,
-        "clip_skip": 1,
-        "control_type": None,
-        "image_is_control": False,
-        "return_control_map": False,
-        "prompt": "an ancient llamia monster",
-        "ddim_steps": 25,
-        "n_iter": 1,
-        "model": model,
-    }
-    horde = HordeLib()
-    for i in range(count):
-        pil_image = horde.basic_inference(data)
-        pil_image.save(f"images/perftest/image_{threadid}_iter_{i}.webp", quality=90)
-
-
-def generate_images_portrait(model, threadid, count):
-    data = {
-        "sampler_name": "k_dpmpp_2m",
-        "cfg_scale": 7.5,
-        "denoising_strength": 1.0,
-        "seed": 123456789,
-        "height": 512,
-        "width": 768,
-        "karras": True,
-        "tiling": False,
-        "hires_fix": False,
-        "clip_skip": 1,
-        "control_type": None,
-        "image_is_control": False,
-        "return_control_map": False,
-        "prompt": "an ancient llamia monster",
-        "ddim_steps": 25,
-        "n_iter": 1,
-        "model": model,
-    }
-    horde = HordeLib()
-    for i in range(count):
-        pil_image = horde.basic_inference(data)
-        pil_image.save(f"images/perftest/image_{threadid}_iter_{i}.webp", quality=90)
-
-
-def generate_images_cnet(model, threadid, count):
-    data = {
-        "sampler_name": "k_dpmpp_2m",
-        "cfg_scale": 7.5,
-        "denoising_strength": 1.0,
-        "seed": 123456789,
-        "height": 512,
-        "width": 768,
-        "karras": True,
-        "tiling": False,
-        "hires_fix": False,
-        "clip_skip": 1,
-        "control_type": "",
-        "image_is_control": False,
-        "return_control_map": False,
-        "prompt": "a man walking in the snow",
-        "ddim_steps": 25,
-        "n_iter": 1,
-        "model": model,
-        "source_image": Image.open("images/test_db0.jpg"),
-        "source_processing": "img2img",
-    }
-    for i in range(count):
-        horde = HordeLib()
-        pil_image = horde.basic_inference(data)
-        pil_image.save(f"images/perftest/image_{threadid}_iter_{i}.webp", quality=90)
+    import threading
 
+    from loguru import logger
+    from PIL import Image
 
-def generate_images_img2img(model, threadid, count):
-    data = {
-        "sampler_name": "k_dpmpp_2m",
-        "cfg_scale": 7.5,
-        "denoising_strength": 0.4,
-        "seed": 666,
-        "height": 768,
-        "width": 512,
-        "karras": False,
-        "tiling": False,
-        "hires_fix": False,
-        "clip_skip": 1,
-        "control_type": None,
-        "image_is_control": False,
-        "return_control_map": False,
-        "prompt": "a dinosaur",
-        "ddim_steps": 25,
-        "n_iter": 1,
-        "model": "Deliberate",
-        "source_image": Image.open("images/test_db0.jpg"),
-        "source_processing": "img2img",
-    }
-    for i in range(count):
+    from hordelib.horde import HordeLib
+    from hordelib.shared_model_manager import SharedModelManager
+
+    generate = HordeLib()
+    SharedModelManager.loadModelManagers(compvis=True)
+    SharedModelManager.manager.load("Deliberate")
+    SharedModelManager.manager.load("Anything Diffusion")
+    SharedModelManager.manager.load("Realistic Vision")
+    SharedModelManager.manager.load("Papercutcraft")
+
+    def generate_images(model, threadid, count):
+        data = {
+            "sampler_name": "k_dpmpp_2m",
+            "cfg_scale": 7.5,
+            "denoising_strength": 1.0,
+            "seed": 123456789,
+            "height": 512,
+            "width": 512,
+            "karras": True,
+            "tiling": False,
+            "hires_fix": False,
+            "clip_skip": 1,
+            "control_type": None,
+            "image_is_control": False,
+            "return_control_map": False,
+            "prompt": "an ancient llamia monster",
+            "ddim_steps": 25,
+            "n_iter": 1,
+            "model": model,
+        }
         horde = HordeLib()
-        pil_image = horde.basic_inference(data)
-        pil_image.save(f"images/perftest/image_{threadid}_iter_{i}.webp", quality=90)
-
+        for i in range(count):
+            pil_image = horde.basic_inference(data)
+            pil_image.save(f"images/perftest/image_{threadid}_iter_{i}.webp", quality=90)
+
+    def generate_images_portrait(model, threadid, count):
+        data = {
+            "sampler_name": "k_dpmpp_2m",
+            "cfg_scale": 7.5,
+            "denoising_strength": 1.0,
+            "seed": 123456789,
+            "height": 512,
+            "width": 768,
+            "karras": True,
+            "tiling": False,
+            "hires_fix": False,
+            "clip_skip": 1,
+            "control_type": None,
+            "image_is_control": False,
+            "return_control_map": False,
+            "prompt": "an ancient llamia monster",
+            "ddim_steps": 25,
+            "n_iter": 1,
+            "model": model,
+        }
+        horde = HordeLib()
+        for i in range(count):
+            pil_image = horde.basic_inference(data)
+            pil_image.save(f"images/perftest/image_{threadid}_iter_{i}.webp", quality=90)
+
+    def generate_images_cnet(model, threadid, count):
+        data = {
+            "sampler_name": "k_dpmpp_2m",
+            "cfg_scale": 7.5,
+            "denoising_strength": 1.0,
+            "seed": 123456789,
+            "height": 512,
+            "width": 768,
+            "karras": True,
+            "tiling": False,
+            "hires_fix": False,
+            "clip_skip": 1,
+            "control_type": "",
+            "image_is_control": False,
+            "return_control_map": False,
+            "prompt": "a man walking in the snow",
+            "ddim_steps": 25,
+            "n_iter": 1,
+            "model": model,
+            "source_image": Image.open("images/test_db0.jpg"),
+            "source_processing": "img2img",
+        }
+        for i in range(count):
+            horde = HordeLib()
+            pil_image = horde.basic_inference(data)
+            pil_image.save(f"images/perftest/image_{threadid}_iter_{i}.webp", quality=90)
+
+    def generate_images_img2img(model, threadid, count):
+        data = {
+            "sampler_name": "k_dpmpp_2m",
+            "cfg_scale": 7.5,
+            "denoising_strength": 0.4,
+            "seed": 666,
+            "height": 768,
+            "width": 512,
+            "karras": False,
+            "tiling": False,
+            "hires_fix": False,
+            "clip_skip": 1,
+            "control_type": None,
+            "image_is_control": False,
+            "return_control_map": False,
+            "prompt": "a dinosaur",
+            "ddim_steps": 25,
+            "n_iter": 1,
+            "model": "Deliberate",
+            "source_image": Image.open("images/test_db0.jpg"),
+            "source_processing": "img2img",
+        }
+        for i in range(count):
+            horde = HordeLib()
+            pil_image = horde.basic_inference(data)
+            pil_image.save(f"images/perftest/image_{threadid}_iter_{i}.webp", quality=90)
+
+    if not os.path.exists("images/perftest"):
+        os.makedirs("images/perftest")
+
+    start_time = time.time()
+    threads = []
+    threads.append(
+        threading.Thread(
+            daemon=True,
+            target=generate_images,
+            kwargs={"model": "Deliberate", "threadid": 1, "count": 10},
+        ),
+    )
+    threads.append(
+        threading.Thread(
+            daemon=True,
+            target=generate_images_portrait,
+            kwargs={"model": "Anything Diffusion", "threadid": 2, "count": 10},
+        ),
+    )
+    threads.append(
+        threading.Thread(
+            daemon=True,
+            target=generate_images_cnet,
+            kwargs={"model": "Realistic Vision", "threadid": 3, "count": 10},
+        ),
+    )
+    threads.append(
+        threading.Thread(
+            daemon=True,
+            target=generate_images_img2img,
+            kwargs={"model": "Papercutcraft", "threadid": 4, "count": 10},
+        ),
+    )
+    for t in threads:
+        t.start()
+    for t in threads:
+        t.join()
 
-if not os.path.exists("images/perftest"):
-    os.makedirs("images/perftest")
+    logger.warning(f"Testing completed in {round(time.time()-start_time)} seconds")
 
-start_time = time.time()
-threads = []
-threads.append(
-    threading.Thread(daemon=True, target=generate_images, kwargs={"model": "Deliberate", "threadid": 1, "count": 10}),
-)
-threads.append(
-    threading.Thread(
-        daemon=True,
-        target=generate_images_portrait,
-        kwargs={"model": "Anything Diffusion", "threadid": 2, "count": 10},
-    ),
-)
-threads.append(
-    threading.Thread(
-        daemon=True,
-        target=generate_images_cnet,
-        kwargs={"model": "Realistic Vision", "threadid": 3, "count": 10},
-    ),
-)
-threads.append(
-    threading.Thread(
-        daemon=True,
-        target=generate_images_img2img,
-        kwargs={"model": "Papercutcraft", "threadid": 4, "count": 10},
-    ),
-)
-for t in threads:
-    t.start()
-for t in threads:
-    t.join()
 
-logger.warning(f"Testing completed in {round(time.time()-start_time)} seconds")
+if __name__ == "__main__":
+    main()
```

### Comparing `hordelib-0.8.5/tests/run_txt2img.py` & `hordelib-0.8.6/examples/run_img2img_inpaint.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,47 @@
 # This tests running hordelib standalone, as an external caller would use it.
-# Call with: python -m test.run_txt2img
+# Call with: python -m test.run_img2img_inpaint
 # You need all the deps in whatever environment you are running this.
 import os
 
 import hordelib
 
-hordelib.initialise()
 
-from hordelib.horde import HordeLib
-from hordelib.shared_model_manager import SharedModelManager
+def main():
+    hordelib.initialise()
 
-generate = HordeLib()
-SharedModelManager.loadModelManagers(compvis=True)
-SharedModelManager.manager.load("Deliberate")
-
-data = {
-    "sampler_name": "k_dpmpp_2m",
-    "cfg_scale": 7.5,
-    "denoising_strength": 1.0,
-    "seed": 123456789,
-    "height": 512,
-    "width": 512,
-    "karras": True,
-    "tiling": False,
-    "hires_fix": False,
-    "clip_skip": 1,
-    "control_type": None,
-    "image_is_control": False,
-    "return_control_map": False,
-    "prompt": "an ancient llamia monster",
-    "ddim_steps": 25,
-    "n_iter": 1,
-    "model": "Deliberate",
-}
-pil_image = generate.basic_inference(data)
-pil_image.save("images/run_txt2img.webp", quality=90)
+    from PIL import Image
+
+    from hordelib.horde import HordeLib
+    from hordelib.shared_model_manager import SharedModelManager
+
+    generate = HordeLib()
+    SharedModelManager.loadModelManagers(compvis=True)
+    SharedModelManager.manager.load("Deliberate")
+
+    data = {
+        "sampler_name": "euler",
+        "cfg_scale": 8,
+        "denoising_strength": 0.72,
+        "seed": 836913938046008,
+        "height": 512,
+        "width": 512,
+        "karras": False,
+        "tiling": False,
+        "hires_fix": False,
+        "clip_skip": 1,
+        "control_type": None,
+        "image_is_control": False,
+        "return_control_map": False,
+        "prompt": "a dinosaur",
+        "ddim_steps": 20,
+        "n_iter": 1,
+        "model": "Deliberate",
+        "source_image": Image.open("images/test_inpaint.png"),
+        "source_processing": "inpainting",
+    }
+    pil_image = generate.basic_inference(data)
+    pil_image.save("images/run_img2img_inpaint.webp", quality=90)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `hordelib-0.8.5/tests/run_txt2img_hires.py` & `hordelib-0.8.6/examples/run_txt2img_hires.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 # This tests running hordelib standalone, as an external caller would use it.
 # Call with: python -m test.run_txt2img_hires
 # You need all the deps in whatever environment you are running this.
 import os
 
 import hordelib
 
-hordelib.initialise()
 
-from hordelib.horde import HordeLib
-from hordelib.shared_model_manager import SharedModelManager
+def main():
+    hordelib.initialise()
 
-generate = HordeLib()
-SharedModelManager.loadModelManagers(compvis=True)
-SharedModelManager.manager.load("Deliberate")
-
-data = {
-    "sampler_name": "k_dpmpp_2m",
-    "cfg_scale": 7.5,
-    "denoising_strength": 1.0,
-    "seed": 123456789,
-    "height": 512,
-    "width": 512,
-    "karras": True,
-    "tiling": False,
-    "hires_fix": True,
-    "clip_skip": 1,
-    "control_type": None,
-    "image_is_control": False,
-    "return_control_map": False,
-    "prompt": "an ancient llamia monster",
-    "ddim_steps": 25,
-    "n_iter": 1,
-    "model": "Deliberate",
-}
-pil_image = generate.basic_inference(data)
-pil_image.save("images/run_txt2img_hires.webp", quality=90)
+    from hordelib.horde import HordeLib
+    from hordelib.shared_model_manager import SharedModelManager
+
+    generate = HordeLib()
+    SharedModelManager.loadModelManagers(compvis=True)
+    SharedModelManager.manager.load("Deliberate")
+
+    data = {
+        "sampler_name": "k_dpmpp_2m",
+        "cfg_scale": 7.5,
+        "denoising_strength": 1.0,
+        "seed": 123456789,
+        "height": 512,
+        "width": 512,
+        "karras": True,
+        "tiling": False,
+        "hires_fix": True,
+        "clip_skip": 1,
+        "control_type": None,
+        "image_is_control": False,
+        "return_control_map": False,
+        "prompt": "an ancient llamia monster",
+        "ddim_steps": 25,
+        "n_iter": 1,
+        "model": "Deliberate",
+    }
+    pil_image = generate.basic_inference(data)
+    pil_image.save("images/run_txt2img_hires.webp", quality=90)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `hordelib-0.8.5/tests/run_upscale.py` & `hordelib-0.8.6/examples/run_upscale.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 # This tests running hordelib standalone, as an external caller would use it.
 # Call with: python -m test.run_upscale
 # You need all the deps in whatever environment you are running this.
 import os
 
 import hordelib
 
-hordelib.initialise()
 
-from PIL import Image
+def main():
+    hordelib.initialise()
 
-from hordelib.horde import HordeLib
-from hordelib.shared_model_manager import SharedModelManager
+    from PIL import Image
 
-generate = HordeLib()
-modeltypes = {
-    # aitemplate
-    "blip": True,
-    "clip": True,
-    "codeformer": True,
-    "compvis": True,
-    "controlnet": True,
-    "diffusers": True,
-    "esrgan": True,
-    "gfpgan": True,
-    "safety_checker": True,
-}
-
-SharedModelManager.loadModelManagers(**modeltypes)
-SharedModelManager.manager.load("RealESRGAN_x4plus")
-
-data = {
-    "model": "RealESRGAN_x4plus",
-    "source_image": Image.open("images/test_db0.jpg"),
-}
-pil_image = generate.image_upscale(data)
-pil_image.save("images/run_upscale.webp", quality=90)
+    from hordelib.horde import HordeLib
+    from hordelib.shared_model_manager import SharedModelManager
+
+    generate = HordeLib()
+    modeltypes = {
+        # aitemplate
+        "blip": True,
+        "clip": True,
+        "codeformer": True,
+        "compvis": True,
+        "controlnet": True,
+        "diffusers": True,
+        "esrgan": True,
+        "gfpgan": True,
+        "safety_checker": True,
+    }
+
+    SharedModelManager.loadModelManagers(**modeltypes)
+    SharedModelManager.manager.load("RealESRGAN_x4plus")
+
+    data = {
+        "model": "RealESRGAN_x4plus",
+        "source_image": Image.open("images/test_db0.jpg"),
+    }
+    pil_image = generate.image_upscale(data)
+    pil_image.save("images/run_upscale.webp", quality=90)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `hordelib-0.8.5/tests/test_blip.py` & `hordelib-0.8.6/tests/test_blip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/tests/test_clip.py` & `hordelib-0.8.6/tests/test_clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/tests/test_comfy.py` & `hordelib-0.8.6/tests/test_comfy.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/tests/test_horde_controlnet_annotator.py` & `hordelib-0.8.6/tests/test_horde_controlnet_annotator.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/tests/test_horde_inference.py` & `hordelib-0.8.6/tests/test_horde_inference.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/tests/test_horde_inference_controlnet.py` & `hordelib-0.8.6/tests/test_horde_inference_controlnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/tests/test_horde_inference_img2img.py` & `hordelib-0.8.6/tests/test_horde_inference_img2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/tests/test_horde_inference_painting.py` & `hordelib-0.8.6/tests/test_horde_inference_painting.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/tests/test_horde_pp.py` & `hordelib-0.8.6/tests/test_horde_pp.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/tests/test_inference.py` & `hordelib-0.8.6/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/tests/test_safety_checker.py` & `hordelib-0.8.6/tests/test_safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.8.5/tox.ini` & `hordelib-0.8.6/tox.ini`

 * *Files identical despite different names*

