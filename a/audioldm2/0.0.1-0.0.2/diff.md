# Comparing `tmp/audioldm2-0.0.1.tar.gz` & `tmp/audioldm2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioldm2-0.0.1.tar", last modified: Fri Aug  4 16:19:29 2023, max compression
+gzip compressed data, was "audioldm2-0.0.2.tar", last modified: Fri Aug  4 17:03:36 2023, max compression
```

## Comparing `audioldm2-0.0.1.tar` & `audioldm2-0.0.2.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:19:29.305359 audioldm2-0.0.1/
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    20845 2023-08-04 16:01:51.000000 audioldm2-0.0.1/LICENSE
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       87 2023-08-04 16:01:51.000000 audioldm2-0.0.1/MANIFEST.in
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      731 2023-08-04 16:19:29.300877 audioldm2-0.0.1/PKG-INFO
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       73 2023-08-04 16:12:39.000000 audioldm2-0.0.1/README.md
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    14066 2023-08-04 16:08:46.000000 audioldm2-0.0.1/app.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:19:29.181208 audioldm2-0.0.1/audioldm2/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       94 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/__init__.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:19:29.190615 audioldm2-0.0.1/audioldm2/audiomae_gen/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       46 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/audiomae_gen/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    16876 2023-08-04 16:07:32.000000 audioldm2-0.0.1/audioldm2/audiomae_gen/sequence_input.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      730 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/audiomae_gen/utils.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:19:29.194190 audioldm2-0.0.1/audioldm2/clap/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/__init__.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:19:29.211632 audioldm2-0.0.1/audioldm2/clap/open_clip/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      639 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)  1356917 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/bpe_simple_vocab_16e6.txt.gz
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    10985 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/factory.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     7177 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/feature_fusion.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    48069 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/htsat.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    16096 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/loss.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    32924 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/model.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:19:29.236774 audioldm2-0.0.1/audioldm2/clap/open_clip/model_configs/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/model_configs/HTSAT-base.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      498 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/model_configs/HTSAT-large.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/model_configs/HTSAT-tiny.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/model_configs/PANN-10.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/model_configs/PANN-14-fmax-18k.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/model_configs/PANN-14-tiny-transformer.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/model_configs/PANN-14-win-1536.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/model_configs/PANN-14.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      495 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/model_configs/PANN-6.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      388 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/model_configs/RN101-quickgelu.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      364 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/model_configs/RN101.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      389 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/model_configs/RN50-quickgelu.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      364 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/model_configs/RN50.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      365 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/model_configs/RN50x16.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      365 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/model_configs/RN50x4.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      294 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/model_configs/ViT-B-16.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      318 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/model_configs/ViT-B-32-quickgelu.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      294 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/model_configs/ViT-B-32.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      296 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/model_configs/ViT-L-14.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5023 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/openai.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    23369 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/pann_model.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6440 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/pretrained.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     4332 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/timm_model.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6400 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/tokenizer.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1051 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/transform.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    11952 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/open_clip/utils.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:19:29.244935 audioldm2-0.0.1/audioldm2/clap/training/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/training/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    84448 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/training/audioset_textmap.npy
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)  1356917 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/training/bpe_simple_vocab_16e6.txt.gz
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    29418 2023-08-04 16:06:43.000000 audioldm2-0.0.1/audioldm2/clap/training/data.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    17202 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/clap/training/params.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:19:29.249043 audioldm2-0.0.1/audioldm2/hifigan/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      230 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/hifigan/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5524 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/hifigan/models.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    12819 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/hifigan/models_v2.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:19:29.252672 audioldm2-0.0.1/audioldm2/latent_diffusion/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/__init__.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:19:29.255112 audioldm2-0.0.1/audioldm2/latent_diffusion/models/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/models/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    17259 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/models/ddim.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    65479 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/models/ddpm.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    12849 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/models/plms.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:19:29.259582 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    15753 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/attention.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:19:29.263007 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5381 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/AudioMAE.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    21105 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/models_mae.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     7684 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/models_vit.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:19:29.274728 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/util/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1363 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/util/crop.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1924 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/util/datasets.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2026 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/util/lars.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2445 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/util/lr_decay.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      885 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/util/lr_sched.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    14517 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/util/misc.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     4381 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/util/patch_embed.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     8632 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/util/pos_embed.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2259 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/util/stat.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:19:29.278198 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/diffusionmodules/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/diffusionmodules/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    34452 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/diffusionmodules/model.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    40223 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/diffusionmodules/openaimodel.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     9870 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/diffusionmodules/util.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:19:29.282700 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/distributions/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/distributions/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3097 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/distributions/distributions.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3066 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/ema.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:19:29.285159 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/encoders/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/encoders/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    27449 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/encoders/modules.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:19:29.287191 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/phoneme_encoder/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/phoneme_encoder/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    14860 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/phoneme_encoder/attentions.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     4960 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/phoneme_encoder/commons.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1590 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/modules/phoneme_encoder/encoder.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6022 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_diffusion/util.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:19:29.290945 audioldm2-0.0.1/audioldm2/latent_encoder/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_encoder/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    11286 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/latent_encoder/autoencoder.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6375 2023-08-04 16:12:00.000000 audioldm2-0.0.1/audioldm2/pipeline.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:19:29.292819 audioldm2-0.0.1/audioldm2/utilities/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       62 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/utilities/__init__.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:19:29.297221 audioldm2-0.0.1/audioldm2/utilities/audio/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       73 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/utilities/audio/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2642 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/utilities/audio/audio_processing.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6312 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/utilities/audio/stft.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2528 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/utilities/audio/tools.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:19:29.301647 audioldm2-0.0.1/audioldm2/utilities/data/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       29 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/utilities/data/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    15063 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/utilities/data/add_on.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    20175 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/utilities/data/dataset.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3589 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/utilities/model.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    19538 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/utilities/sampler.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    18077 2023-08-04 16:01:51.000000 audioldm2-0.0.1/audioldm2/utilities/tools.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    12780 2023-08-04 16:13:23.000000 audioldm2-0.0.1/audioldm2/utils.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:19:29.185492 audioldm2-0.0.1/audioldm2.egg-info/
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      731 2023-08-04 16:19:29.000000 audioldm2-0.0.1/audioldm2.egg-info/PKG-INFO
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     4806 2023-08-04 16:19:29.000000 audioldm2-0.0.1/audioldm2.egg-info/SOURCES.txt
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)        1 2023-08-04 16:19:29.000000 audioldm2-0.0.1/audioldm2.egg-info/dependency_links.txt
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      189 2023-08-04 16:19:29.000000 audioldm2-0.0.1/audioldm2.egg-info/requires.txt
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       10 2023-08-04 16:19:29.000000 audioldm2-0.0.1/audioldm2.egg-info/top_level.txt
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:19:29.304861 audioldm2-0.0.1/bin/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     4139 2023-08-04 16:19:01.000000 audioldm2-0.0.1/bin/audioldm2
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       32 2023-08-04 16:01:51.000000 audioldm2-0.0.1/bin/audioldm2.cmd
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       38 2023-08-04 16:19:29.301610 audioldm2-0.0.1/setup.cfg
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     4403 2023-08-04 16:08:36.000000 audioldm2-0.0.1/setup.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     6448 2023-08-04 16:01:51.000000 audioldm2-0.0.1/share_btn.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.948281 audioldm2-0.0.2/
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    20845 2023-08-04 16:01:51.000000 audioldm2-0.0.2/LICENSE
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       87 2023-08-04 16:01:51.000000 audioldm2-0.0.2/MANIFEST.in
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      828 2023-08-04 17:03:36.945016 audioldm2-0.0.2/PKG-INFO
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      151 2023-08-04 17:03:11.000000 audioldm2-0.0.2/README.md
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    14066 2023-08-04 16:59:32.000000 audioldm2-0.0.2/app.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:34.686800 audioldm2-0.0.2/audioldm2/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      105 2023-08-04 16:21:31.000000 audioldm2-0.0.2/audioldm2/__init__.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:34.702016 audioldm2-0.0.2/audioldm2/audiomae_gen/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       46 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/audiomae_gen/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    16876 2023-08-04 16:07:32.000000 audioldm2-0.0.2/audioldm2/audiomae_gen/sequence_input.py
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      730 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/audiomae_gen/utils.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:34.707540 audioldm2-0.0.2/audioldm2/clap/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/__init__.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:34.732854 audioldm2-0.0.2/audioldm2/clap/open_clip/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      639 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)  1356917 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/bpe_simple_vocab_16e6.txt.gz
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    10985 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/factory.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     7177 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/feature_fusion.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    48069 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/htsat.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    16096 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/loss.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    32924 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.827837 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/HTSAT-base.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      498 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/HTSAT-large.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/HTSAT-tiny.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/PANN-10.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/PANN-14-fmax-18k.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/PANN-14-tiny-transformer.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/PANN-14-win-1536.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/PANN-14.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      495 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/PANN-6.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      388 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/RN101-quickgelu.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      364 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/RN101.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      389 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/RN50-quickgelu.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      364 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/RN50.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      365 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/RN50x16.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      365 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/RN50x4.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      294 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/ViT-B-16.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      318 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/ViT-B-32-quickgelu.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      294 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/ViT-B-32.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      296 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/ViT-L-14.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5023 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/openai.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    23369 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/pann_model.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6440 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/pretrained.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     4332 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/timm_model.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6400 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/tokenizer.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1051 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/transform.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    11952 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/utils.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.845663 audioldm2-0.0.2/audioldm2/clap/training/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/training/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    84448 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/training/audioset_textmap.npy
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)  1356917 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/training/bpe_simple_vocab_16e6.txt.gz
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    29418 2023-08-04 16:06:43.000000 audioldm2-0.0.2/audioldm2/clap/training/data.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    17202 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/training/params.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.850367 audioldm2-0.0.2/audioldm2/hifigan/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      230 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/hifigan/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5524 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/hifigan/models.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    12819 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/hifigan/models_v2.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.855969 audioldm2-0.0.2/audioldm2/latent_diffusion/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/__init__.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.859732 audioldm2-0.0.2/audioldm2/latent_diffusion/models/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/models/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    17259 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/models/ddim.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    65611 2023-08-04 16:47:57.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/models/ddpm.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    12849 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/models/plms.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.867241 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    15753 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/attention.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.873412 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5381 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/AudioMAE.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    21105 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/models_mae.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     7684 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/models_vit.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.894510 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1363 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/crop.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1924 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/datasets.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2026 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/lars.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2445 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/lr_decay.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      885 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/lr_sched.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    14517 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/misc.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     4381 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/patch_embed.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     8632 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/pos_embed.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2259 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/stat.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.896852 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/diffusionmodules/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/diffusionmodules/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    34452 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/diffusionmodules/model.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    40223 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/diffusionmodules/openaimodel.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     9870 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/diffusionmodules/util.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.904454 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/distributions/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/distributions/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3097 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/distributions/distributions.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3066 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/ema.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.908410 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/encoders/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/encoders/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    27449 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/encoders/modules.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.912846 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/phoneme_encoder/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/phoneme_encoder/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    14860 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/phoneme_encoder/attentions.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     4960 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/phoneme_encoder/commons.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1590 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/phoneme_encoder/encoder.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6022 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/util.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.921017 audioldm2-0.0.2/audioldm2/latent_encoder/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_encoder/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    11286 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_encoder/autoencoder.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5805 2023-08-04 16:58:20.000000 audioldm2-0.0.2/audioldm2/pipeline.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.924642 audioldm2-0.0.2/audioldm2/utilities/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       62 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/utilities/__init__.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.933509 audioldm2-0.0.2/audioldm2/utilities/audio/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       73 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/utilities/audio/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2642 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/utilities/audio/audio_processing.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6312 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/utilities/audio/stft.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2528 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/utilities/audio/tools.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.941172 audioldm2-0.0.2/audioldm2/utilities/data/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       29 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/utilities/data/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    15063 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/utilities/data/add_on.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    20175 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/utilities/data/dataset.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3589 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/utilities/model.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    19538 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/utilities/sampler.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    18077 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/utilities/tools.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    12780 2023-08-04 16:13:23.000000 audioldm2-0.0.2/audioldm2/utils.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:34.699806 audioldm2-0.0.2/audioldm2.egg-info/
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      828 2023-08-04 17:03:34.000000 audioldm2-0.0.2/audioldm2.egg-info/PKG-INFO
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     4806 2023-08-04 17:03:34.000000 audioldm2-0.0.2/audioldm2.egg-info/SOURCES.txt
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)        1 2023-08-04 17:03:34.000000 audioldm2-0.0.2/audioldm2.egg-info/dependency_links.txt
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      189 2023-08-04 17:03:34.000000 audioldm2-0.0.2/audioldm2.egg-info/requires.txt
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       10 2023-08-04 17:03:34.000000 audioldm2-0.0.2/audioldm2.egg-info/top_level.txt
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.946898 audioldm2-0.0.2/bin/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3065 2023-08-04 17:02:32.000000 audioldm2-0.0.2/bin/audioldm2
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       32 2023-08-04 16:01:51.000000 audioldm2-0.0.2/bin/audioldm2.cmd
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       38 2023-08-04 17:03:36.946471 audioldm2-0.0.2/setup.cfg
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     4403 2023-08-04 17:03:22.000000 audioldm2-0.0.2/setup.py
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     6448 2023-08-04 16:01:51.000000 audioldm2-0.0.2/share_btn.py
```

### Comparing `audioldm2-0.0.1/LICENSE` & `audioldm2-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/PKG-INFO` & `audioldm2-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 Metadata-Version: 2.1
 Name: audioldm2
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package is written for text-to-audio/music generation.
 Home-page: https://github.com/haoheliu/audioldm2
 Author: Haohe Liu
 Author-email: haoheliu@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # AudioLDM 2
 
 A proper choice of seed is important for model performance.
+
+# Usage
+
+1. Install AudioLDM 2 
+
+```shell
+    pip install audioldm=0.0.2
+```
+
```

### Comparing `audioldm2-0.0.1/app.py` & `audioldm2-0.0.2/app.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/audiomae_gen/sequence_input.py` & `audioldm2-0.0.2/audioldm2/audiomae_gen/sequence_input.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/audiomae_gen/utils.py` & `audioldm2-0.0.2/audioldm2/audiomae_gen/utils.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/clap/open_clip/__init__.py` & `audioldm2-0.0.2/audioldm2/clap/open_clip/__init__.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/clap/open_clip/bpe_simple_vocab_16e6.txt.gz` & `audioldm2-0.0.2/audioldm2/clap/open_clip/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/clap/open_clip/factory.py` & `audioldm2-0.0.2/audioldm2/clap/open_clip/factory.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/clap/open_clip/feature_fusion.py` & `audioldm2-0.0.2/audioldm2/clap/open_clip/feature_fusion.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/clap/open_clip/htsat.py` & `audioldm2-0.0.2/audioldm2/clap/open_clip/htsat.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/clap/open_clip/loss.py` & `audioldm2-0.0.2/audioldm2/clap/open_clip/loss.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/clap/open_clip/model.py` & `audioldm2-0.0.2/audioldm2/clap/open_clip/model.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/clap/open_clip/openai.py` & `audioldm2-0.0.2/audioldm2/clap/open_clip/openai.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/clap/open_clip/pann_model.py` & `audioldm2-0.0.2/audioldm2/clap/open_clip/pann_model.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/clap/open_clip/pretrained.py` & `audioldm2-0.0.2/audioldm2/clap/open_clip/pretrained.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/clap/open_clip/timm_model.py` & `audioldm2-0.0.2/audioldm2/clap/open_clip/timm_model.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/clap/open_clip/tokenizer.py` & `audioldm2-0.0.2/audioldm2/clap/open_clip/tokenizer.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/clap/open_clip/transform.py` & `audioldm2-0.0.2/audioldm2/clap/open_clip/transform.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/clap/open_clip/utils.py` & `audioldm2-0.0.2/audioldm2/clap/open_clip/utils.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/clap/training/audioset_textmap.npy` & `audioldm2-0.0.2/audioldm2/clap/training/audioset_textmap.npy`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/clap/training/bpe_simple_vocab_16e6.txt.gz` & `audioldm2-0.0.2/audioldm2/clap/training/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/clap/training/data.py` & `audioldm2-0.0.2/audioldm2/clap/training/data.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/clap/training/params.py` & `audioldm2-0.0.2/audioldm2/clap/training/params.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/hifigan/models.py` & `audioldm2-0.0.2/audioldm2/hifigan/models.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/hifigan/models_v2.py` & `audioldm2-0.0.2/audioldm2/hifigan/models_v2.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/models/ddim.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/models/ddim.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/models/ddpm.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/models/ddpm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1485,15 +1485,16 @@
         assert x_T is None
 
         if use_plms:
             assert ddim_steps is not None
 
         use_ddim = ddim_steps is not None
 
-        with self.ema_scope("Plotting"):
+        # with self.ema_scope("Plotting"):
+        for i in range(1):
             z, c = self.get_input(
                 batch,
                 self.first_stage_key,
                 unconditional_prob_cfg=0.0,  # Do not output unconditional information in the c
             )
 
             c = self.filter_useful_cond_dict(c)
@@ -1552,16 +1553,17 @@
                 for i in range(z.shape[0]):
                     candidates = similarity[i :: z.shape[0]]
                     max_index = torch.argmax(candidates).item()
                     best_index.append(i + max_index * z.shape[0])
 
                 waveform = waveform[best_index]
 
-                print("Similarity between generated audio and text", similarity)
-                print("Choose the following indexes:", best_index)
+                print("Similarity between generated audio and text:")
+                print(' '.join('{:.2f}'.format(num) for num in similarity.detach().cpu().tolist()))
+                print("Choose the following indexes as the output:", best_index)
 
             return waveform
 
     @torch.no_grad()
     def generate_sample(
         self,
         batchs,
```

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/models/plms.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/models/plms.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/modules/attention.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/attention.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/AudioMAE.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/AudioMAE.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/models_mae.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/models_mae.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/models_vit.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/models_vit.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/util/crop.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/crop.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/util/datasets.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/datasets.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/util/lars.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/lars.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/util/lr_decay.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/lr_decay.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/util/lr_sched.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/lr_sched.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/util/misc.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/misc.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/util/patch_embed.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/patch_embed.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/util/pos_embed.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/pos_embed.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/modules/audiomae/util/stat.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/stat.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/modules/diffusionmodules/model.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/diffusionmodules/model.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/modules/diffusionmodules/openaimodel.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/diffusionmodules/openaimodel.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/modules/diffusionmodules/util.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/diffusionmodules/util.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/modules/distributions/distributions.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/modules/ema.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/ema.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/modules/encoders/modules.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/encoders/modules.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/modules/phoneme_encoder/attentions.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/phoneme_encoder/attentions.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/modules/phoneme_encoder/commons.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/phoneme_encoder/commons.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/modules/phoneme_encoder/encoder.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/phoneme_encoder/encoder.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_diffusion/util.py` & `audioldm2-0.0.2/audioldm2/latent_diffusion/util.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/latent_encoder/autoencoder.py` & `audioldm2-0.0.2/audioldm2/latent_encoder/autoencoder.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/pipeline.py` & `audioldm2-0.0.2/audioldm2/pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -139,76 +139,60 @@
         device = torch.device("cuda:0")
     else:
         device = torch.device("cpu")
 
     if config is not None:
         assert type(config) is str
         config = yaml.load(open(config, "r"), Loader=yaml.FullLoader)
-    else:
+    else: 
         config = default_audioldm_config(model_name)
 
     # # Use text as condition instead of using waveform during training
     config["model"]["params"]["device"] = device
     # config["model"]["params"]["cond_stage_key"] = "text"
 
     # No normalization here
     latent_diffusion = LatentDiffusion(**config["model"]["params"])
 
     resume_from_checkpoint = ckpt_path
 
     checkpoint = torch.load(resume_from_checkpoint, map_location=device)
 
     latent_diffusion.load_state_dict(checkpoint["state_dict"])
-
+    
     latent_diffusion.eval()
     latent_diffusion = latent_diffusion.to(device)
-
-    # latent_diffusion.cond_stage_model.embed_mode = "text"
+    
     return latent_diffusion
 
-
 def duration_to_latent_t_size(duration):
     return int(duration * 25.6)
 
-
 def text_to_audio(
     latent_diffusion,
     text,
-    original_audio_file_path=None,
     seed=42,
     ddim_steps=200,
     duration=10,
     batchsize=1,
     guidance_scale=3.5,
     n_candidate_gen_per_text=3,
     config=None,
 ):
     assert (
         duration == 10
     ), "Error: Currently we only support 10 seconds of generation. Generating longer files requires some extra coding, which would be a part of the future work."
 
     seed_everything(int(seed))
     waveform = None
-    
-    # if original_audio_file_path is not None:
-    #     waveform = read_wav_file(original_audio_file_path, int(duration * 102.4) * 160)
 
     batch = make_batch_for_text_to_audio(text, waveform=waveform, batchsize=batchsize)
 
     latent_diffusion.latent_t_size = duration_to_latent_t_size(duration)
 
-    # if waveform is not None:
-    #     print(
-    #         "Generate audio that has similar content as %s" % original_audio_file_path
-    #     )
-        # latent_diffusion = set_cond_audio(latent_diffusion)
-    # else:
-    #     print("Generate audio using text %s" % text)
-        # latent_diffusion = set_cond_text(latent_diffusion)
-
     with torch.no_grad():
         waveform = latent_diffusion.generate_batch(
             batch,
             unconditional_guidance_scale=guidance_scale,
             ddim_steps=ddim_steps,
             n_gen=n_candidate_gen_per_text,
             duration=duration,
```

### Comparing `audioldm2-0.0.1/audioldm2/utilities/audio/audio_processing.py` & `audioldm2-0.0.2/audioldm2/utilities/audio/audio_processing.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/utilities/audio/stft.py` & `audioldm2-0.0.2/audioldm2/utilities/audio/stft.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/utilities/audio/tools.py` & `audioldm2-0.0.2/audioldm2/utilities/audio/tools.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/utilities/data/add_on.py` & `audioldm2-0.0.2/audioldm2/utilities/data/add_on.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/utilities/data/dataset.py` & `audioldm2-0.0.2/audioldm2/utilities/data/dataset.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/utilities/model.py` & `audioldm2-0.0.2/audioldm2/utilities/model.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/utilities/sampler.py` & `audioldm2-0.0.2/audioldm2/utilities/sampler.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/utilities/tools.py` & `audioldm2-0.0.2/audioldm2/utilities/tools.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2/utils.py` & `audioldm2-0.0.2/audioldm2/utils.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/audioldm2.egg-info/PKG-INFO` & `audioldm2-0.0.2/audioldm2.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 Metadata-Version: 2.1
 Name: audioldm2
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package is written for text-to-audio/music generation.
 Home-page: https://github.com/haoheliu/audioldm2
 Author: Haohe Liu
 Author-email: haoheliu@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # AudioLDM 2
 
 A proper choice of seed is important for model performance.
+
+# Usage
+
+1. Install AudioLDM 2 
+
+```shell
+    pip install audioldm=0.0.2
+```
+
```

### Comparing `audioldm2-0.0.1/audioldm2.egg-info/SOURCES.txt` & `audioldm2-0.0.2/audioldm2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.1/bin/audioldm2` & `audioldm2-0.0.2/bin/audioldm2`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 #!/usr/bin/python3
-import sys
-sys.path.append("/mnt/fast/nobackup/scratch4weeks/hl01486/project/audioldm-text-to-audio-generation")
-
 import os
 import torch
-
 import logging
+from audioldm2 import text_to_audio, build_model, save_wave, get_time, read_list
+import argparse
 
+os.environ["TOKENIZERS_PARALLELISM"] = "true"
 matplotlib_logger = logging.getLogger('matplotlib')
 matplotlib_logger.setLevel(logging.WARNING)
 
-from audioldm2 import text_to_audio, build_model, save_wave, get_time, read_list
-import argparse
 
 CACHE_DIR = os.getenv(
     "AUDIOLDM_CACHE_DIR",
     os.path.join(os.path.expanduser("~"), ".cache/audioldm2"))
 
 parser = argparse.ArgumentParser()
 
@@ -52,23 +49,14 @@
     required=False,
     help="The checkpoint you gonna use",
     default="audioldm2-full",
     choices=["audioldm2-full"]
 )
 
 parser.add_argument(
-    "-ckpt",
-    "--ckpt_path",
-    type=str,
-    required=False,
-    help="The path to the pretrained .ckpt model",
-    default=None,
-)
-
-parser.add_argument(
     "-b",
     "--batchsize",
     type=int,
     required=False,
     default=1,
     help="Generate how many samples at the same time",
 )
@@ -103,64 +91,41 @@
     "--seed",
     type=int,
     required=False,
     default=0,
     help="Change this value (any integer number) will lead to a different generation result.",
 )
 
-parser.add_argument('--disable_time_stamp', 
-                    action='store_true', 
-                    help="If set, do not use the timestamp as file name when saving the generated audio file.")
-
 args = parser.parse_args()
 
 torch.set_float32_matmul_precision("high")
-
-if(args.ckpt_path is not None):
-    print("Warning: ckpt_path has no effect after version 0.0.20.")
-
-mode = args.mode
-if(mode == "generation" and args.file_path is not None):
-    mode = "generation_audio_to_audio"
-    if(len(args.text) > 0):
-        print("Warning: You have specified the --file_path. --text will be ignored")
-        args.text = ""
         
-save_path = os.path.join(args.save_path, mode)
-
-if(args.file_path is not None):
-    save_path = os.path.join(save_path, os.path.basename(args.file_path.split(".")[0]))
+save_path = os.path.join(args.save_path, get_time())
 
 text = args.text
 random_seed = args.seed
 duration = 10
 guidance_scale = args.guidance_scale
 n_candidate_gen_per_text = args.n_candidate_gen_per_text
 
 os.makedirs(save_path, exist_ok=True)
 audioldm2 = build_model(model_name=args.model_name)
 
 if(args.text_list):
     print("Generate audio based on the text prompts in %s" % args.text_list)
     prompt_todo = read_list(args.text_list)
-else:
+else: 
     prompt_todo = [text]
     
 for text in prompt_todo:
     waveform = text_to_audio(
         audioldm2,
         text,
-        original_audio_file_path=args.file_path,
         seed=random_seed,
         duration=duration,
         guidance_scale=guidance_scale,
         ddim_steps=args.ddim_steps,
         n_candidate_gen_per_text=n_candidate_gen_per_text,
         batchsize=args.batchsize,
     )
-    
-    if(not disable_time_stamp):
-        name = "%s_%s" % (get_time(), text)
-    else:
-        name = "%s" % (get_time(), text)
         
-    save_wave(waveform, save_path, name=name)
+    save_wave(waveform, save_path, name=text)
```

### Comparing `audioldm2-0.0.1/setup.py` & `audioldm2-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # Package meta-data.
 NAME = "audioldm2"
 DESCRIPTION = "This package is written for text-to-audio/music generation."
 URL = "https://github.com/haoheliu/audioldm2"
 EMAIL = "haoheliu@gmail.com"
 AUTHOR = "Haohe Liu"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "torch>=1.13.0",
     "torchaudio>=0.13.0",
     "torchvision>=0.14.0",
     "tqdm",
```

### Comparing `audioldm2-0.0.1/share_btn.py` & `audioldm2-0.0.2/share_btn.py`

 * *Files identical despite different names*

