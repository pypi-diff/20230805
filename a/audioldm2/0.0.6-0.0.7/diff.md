# Comparing `tmp/audioldm2-0.0.6.tar.gz` & `tmp/audioldm2-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioldm2-0.0.6.tar", last modified: Sat Aug  5 12:35:02 2023, max compression
+gzip compressed data, was "audioldm2-0.0.7.tar", last modified: Sat Aug  5 16:22:48 2023, max compression
```

## Comparing `audioldm2-0.0.6.tar` & `audioldm2-0.0.7.tar`

### file list

```diff
@@ -1,136 +1,135 @@
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 12:35:02.740178 audioldm2-0.0.6/
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    20845 2023-08-04 16:01:51.000000 audioldm2-0.0.6/LICENSE
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       87 2023-08-04 16:01:51.000000 audioldm2-0.0.6/MANIFEST.in
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     3690 2023-08-05 12:35:02.736736 audioldm2-0.0.6/PKG-INFO
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     3013 2023-08-05 12:34:39.000000 audioldm2-0.0.6/README.md
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    13904 2023-08-05 12:25:24.000000 audioldm2-0.0.6/app.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 12:35:02.543223 audioldm2-0.0.6/audioldm2/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      105 2023-08-04 16:21:31.000000 audioldm2-0.0.6/audioldm2/__init__.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 12:35:02.556340 audioldm2-0.0.6/audioldm2/audiomae_gen/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       46 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/audiomae_gen/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    16876 2023-08-04 16:07:32.000000 audioldm2-0.0.6/audioldm2/audiomae_gen/sequence_input.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      730 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/audiomae_gen/utils.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 12:35:02.561236 audioldm2-0.0.6/audioldm2/clap/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/__init__.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 12:35:02.586831 audioldm2-0.0.6/audioldm2/clap/open_clip/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      639 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)  1356917 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/bpe_simple_vocab_16e6.txt.gz
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    10985 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/factory.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     7177 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/feature_fusion.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    48069 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/htsat.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    16096 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/loss.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    32924 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/model.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 12:35:02.629606 audioldm2-0.0.6/audioldm2/clap/open_clip/model_configs/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/model_configs/HTSAT-base.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      498 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/model_configs/HTSAT-large.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/model_configs/HTSAT-tiny.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/model_configs/PANN-10.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/model_configs/PANN-14-fmax-18k.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/model_configs/PANN-14-tiny-transformer.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/model_configs/PANN-14-win-1536.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/model_configs/PANN-14.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      495 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/model_configs/PANN-6.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      388 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/model_configs/RN101-quickgelu.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      364 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/model_configs/RN101.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      389 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/model_configs/RN50-quickgelu.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      364 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/model_configs/RN50.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      365 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/model_configs/RN50x16.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      365 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/model_configs/RN50x4.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      294 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/model_configs/ViT-B-16.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      318 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/model_configs/ViT-B-32-quickgelu.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      294 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/model_configs/ViT-B-32.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      296 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/model_configs/ViT-L-14.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5023 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/openai.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    23369 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/pann_model.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6440 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/pretrained.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     4332 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/timm_model.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6400 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/tokenizer.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1051 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/transform.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    11963 2023-08-05 10:50:27.000000 audioldm2-0.0.6/audioldm2/clap/open_clip/utils.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 12:35:02.642901 audioldm2-0.0.6/audioldm2/clap/training/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/training/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    84448 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/training/audioset_textmap.npy
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)  1356917 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/training/bpe_simple_vocab_16e6.txt.gz
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    29672 2023-08-04 17:59:22.000000 audioldm2-0.0.6/audioldm2/clap/training/data.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    17202 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/clap/training/params.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 12:35:02.648222 audioldm2-0.0.6/audioldm2/hifigan/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      230 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/hifigan/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5524 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/hifigan/models.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    12819 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/hifigan/models_v2.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 12:35:02.653279 audioldm2-0.0.6/audioldm2/latent_diffusion/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/__init__.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 12:35:02.656894 audioldm2-0.0.6/audioldm2/latent_diffusion/models/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/models/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    17259 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/models/ddim.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    65617 2023-08-05 12:19:53.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/models/ddpm.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    12849 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/models/plms.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 12:35:02.665127 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    15753 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/attention.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 12:35:02.670647 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5381 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/AudioMAE.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    21105 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/models_mae.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     7684 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/models_vit.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 12:35:02.691957 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/util/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1363 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/util/crop.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1924 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/util/datasets.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2026 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/util/lars.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2445 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/util/lr_decay.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      885 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/util/lr_sched.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    14517 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/util/misc.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     4381 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/util/patch_embed.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     8632 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/util/pos_embed.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2259 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/util/stat.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 12:35:02.694002 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/diffusionmodules/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/diffusionmodules/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    34452 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/diffusionmodules/model.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    40223 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/diffusionmodules/openaimodel.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     9870 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/diffusionmodules/util.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 12:35:02.701099 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/distributions/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/distributions/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3097 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/distributions/distributions.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3066 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/ema.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 12:35:02.704603 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/encoders/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/encoders/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    27449 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/encoders/modules.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 12:35:02.708477 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/phoneme_encoder/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/phoneme_encoder/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    14860 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/phoneme_encoder/attentions.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     4960 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/phoneme_encoder/commons.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1590 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/modules/phoneme_encoder/encoder.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6022 2023-08-05 11:39:27.000000 audioldm2-0.0.6/audioldm2/latent_diffusion/util.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 12:35:02.715760 audioldm2-0.0.6/audioldm2/latent_encoder/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_encoder/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    11286 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/latent_encoder/autoencoder.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5657 2023-08-05 12:23:19.000000 audioldm2-0.0.6/audioldm2/pipeline.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 12:35:02.718957 audioldm2-0.0.6/audioldm2/utilities/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       62 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/utilities/__init__.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 12:35:02.726576 audioldm2-0.0.6/audioldm2/utilities/audio/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       73 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/utilities/audio/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2642 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/utilities/audio/audio_processing.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6312 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/utilities/audio/stft.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2528 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/utilities/audio/tools.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 12:35:02.733817 audioldm2-0.0.6/audioldm2/utilities/data/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       29 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/utilities/data/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    15063 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/utilities/data/add_on.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    20175 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/utilities/data/dataset.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3589 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/utilities/model.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    19538 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/utilities/sampler.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    18077 2023-08-04 16:01:51.000000 audioldm2-0.0.6/audioldm2/utilities/tools.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    12389 2023-08-05 12:25:46.000000 audioldm2-0.0.6/audioldm2/utils.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 12:35:02.554356 audioldm2-0.0.6/audioldm2.egg-info/
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     3690 2023-08-05 12:35:01.000000 audioldm2-0.0.6/audioldm2.egg-info/PKG-INFO
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     4814 2023-08-05 12:35:02.000000 audioldm2-0.0.6/audioldm2.egg-info/SOURCES.txt
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)        1 2023-08-05 12:35:01.000000 audioldm2-0.0.6/audioldm2.egg-info/dependency_links.txt
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      218 2023-08-05 12:35:01.000000 audioldm2-0.0.6/audioldm2.egg-info/requires.txt
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       10 2023-08-05 12:35:01.000000 audioldm2-0.0.6/audioldm2.egg-info/top_level.txt
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 12:35:02.739654 audioldm2-0.0.6/bin/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3001 2023-08-05 12:22:40.000000 audioldm2-0.0.6/bin/audioldm2
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       32 2023-08-04 16:01:51.000000 audioldm2-0.0.6/bin/audioldm2.cmd
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       38 2023-08-05 12:35:02.738343 audioldm2-0.0.6/setup.cfg
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     4445 2023-08-05 12:34:54.000000 audioldm2-0.0.6/setup.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     6448 2023-08-04 16:01:51.000000 audioldm2-0.0.6/share_btn.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      165 2023-08-05 12:17:32.000000 audioldm2-0.0.6/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.647388 audioldm2-0.0.7/
+-rw-r--r--   0 root         (0) root         (0)    20845 2023-08-05 14:48:09.000000 audioldm2-0.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       87 2023-08-05 14:48:09.000000 audioldm2-0.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-08-05 16:22:48.644195 audioldm2-0.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4354 2023-08-05 16:03:02.000000 audioldm2-0.0.7/README.md
+-rw-r--r--   0 root         (0) root         (0)    13995 2023-08-05 14:49:05.000000 audioldm2-0.0.7/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.032657 audioldm2-0.0.7/audioldm2/
+-rwxr-xr-x   0 root         (0) root         (0)      105 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.077152 audioldm2-0.0.7/audioldm2/audiomae_gen/
+-rwxr-xr-x   0 root         (0) root         (0)       46 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/audiomae_gen/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    16876 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/audiomae_gen/sequence_input.py
+-rw-r--r--   0 root         (0) root         (0)      730 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/audiomae_gen/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.082058 audioldm2-0.0.7/audioldm2/clap/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.194959 audioldm2-0.0.7/audioldm2/clap/open_clip/
+-rwxr-xr-x   0 root         (0) root         (0)      639 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)  1356917 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/bpe_simple_vocab_16e6.txt.gz
+-rwxr-xr-x   0 root         (0) root         (0)    10985 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/factory.py
+-rwxr-xr-x   0 root         (0) root         (0)     7177 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/feature_fusion.py
+-rwxr-xr-x   0 root         (0) root         (0)    48069 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/htsat.py
+-rwxr-xr-x   0 root         (0) root         (0)    16096 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/loss.py
+-rwxr-xr-x   0 root         (0) root         (0)    32924 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.328551 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/
+-rwxr-xr-x   0 root         (0) root         (0)      497 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/HTSAT-base.json
+-rwxr-xr-x   0 root         (0) root         (0)      498 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/HTSAT-large.json
+-rwxr-xr-x   0 root         (0) root         (0)      496 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json
+-rwxr-xr-x   0 root         (0) root         (0)      496 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/HTSAT-tiny.json
+-rwxr-xr-x   0 root         (0) root         (0)      497 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/PANN-10.json
+-rwxr-xr-x   0 root         (0) root         (0)      497 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/PANN-14-fmax-18k.json
+-rwxr-xr-x   0 root         (0) root         (0)      496 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json
+-rwxr-xr-x   0 root         (0) root         (0)      496 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/PANN-14-tiny-transformer.json
+-rwxr-xr-x   0 root         (0) root         (0)      497 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/PANN-14-win-1536.json
+-rwxr-xr-x   0 root         (0) root         (0)      497 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/PANN-14.json
+-rwxr-xr-x   0 root         (0) root         (0)      495 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/PANN-6.json
+-rwxr-xr-x   0 root         (0) root         (0)      388 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/RN101-quickgelu.json
+-rwxr-xr-x   0 root         (0) root         (0)      364 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/RN101.json
+-rwxr-xr-x   0 root         (0) root         (0)      389 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/RN50-quickgelu.json
+-rwxr-xr-x   0 root         (0) root         (0)      364 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/RN50.json
+-rwxr-xr-x   0 root         (0) root         (0)      365 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/RN50x16.json
+-rwxr-xr-x   0 root         (0) root         (0)      365 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/RN50x4.json
+-rwxr-xr-x   0 root         (0) root         (0)      294 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/ViT-B-16.json
+-rwxr-xr-x   0 root         (0) root         (0)      318 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/ViT-B-32-quickgelu.json
+-rwxr-xr-x   0 root         (0) root         (0)      294 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/ViT-B-32.json
+-rwxr-xr-x   0 root         (0) root         (0)      296 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/model_configs/ViT-L-14.json
+-rwxr-xr-x   0 root         (0) root         (0)     5023 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/openai.py
+-rwxr-xr-x   0 root         (0) root         (0)    23369 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/pann_model.py
+-rwxr-xr-x   0 root         (0) root         (0)     6440 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/pretrained.py
+-rwxr-xr-x   0 root         (0) root         (0)     4332 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/timm_model.py
+-rwxr-xr-x   0 root         (0) root         (0)     6400 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/tokenizer.py
+-rwxr-xr-x   0 root         (0) root         (0)     1051 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/transform.py
+-rwxr-xr-x   0 root         (0) root         (0)    11963 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/open_clip/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.361736 audioldm2-0.0.7/audioldm2/clap/training/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/training/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    84448 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/training/audioset_textmap.npy
+-rw-r--r--   0 root         (0) root         (0)  1356917 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/training/bpe_simple_vocab_16e6.txt.gz
+-rwxr-xr-x   0 root         (0) root         (0)    29672 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/training/data.py
+-rwxr-xr-x   0 root         (0) root         (0)    17202 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/clap/training/params.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.379886 audioldm2-0.0.7/audioldm2/hifigan/
+-rwxr-xr-x   0 root         (0) root         (0)      230 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/hifigan/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     5524 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/hifigan/models.py
+-rwxr-xr-x   0 root         (0) root         (0)    12819 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/hifigan/models_v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.390679 audioldm2-0.0.7/audioldm2/latent_diffusion/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.411725 audioldm2-0.0.7/audioldm2/latent_diffusion/models/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/models/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    17259 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/models/ddim.py
+-rwxr-xr-x   0 root         (0) root         (0)    65617 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/models/ddpm.py
+-rwxr-xr-x   0 root         (0) root         (0)    12849 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/models/plms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.427396 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    15753 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/attention.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.448757 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/
+-rwxr-xr-x   0 root         (0) root         (0)     5381 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/AudioMAE.py
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    21105 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/models_mae.py
+-rwxr-xr-x   0 root         (0) root         (0)     7684 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/models_vit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.498199 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/
+-rwxr-xr-x   0 root         (0) root         (0)     1363 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/crop.py
+-rwxr-xr-x   0 root         (0) root         (0)     1924 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/datasets.py
+-rwxr-xr-x   0 root         (0) root         (0)     2026 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/lars.py
+-rwxr-xr-x   0 root         (0) root         (0)     2445 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/lr_decay.py
+-rwxr-xr-x   0 root         (0) root         (0)      885 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/lr_sched.py
+-rwxr-xr-x   0 root         (0) root         (0)    14517 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/misc.py
+-rwxr-xr-x   0 root         (0) root         (0)     4381 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/patch_embed.py
+-rwxr-xr-x   0 root         (0) root         (0)     8632 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/pos_embed.py
+-rwxr-xr-x   0 root         (0) root         (0)     2259 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/stat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.520019 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/diffusionmodules/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/diffusionmodules/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    34452 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/diffusionmodules/model.py
+-rwxr-xr-x   0 root         (0) root         (0)    40223 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/diffusionmodules/openaimodel.py
+-rwxr-xr-x   0 root         (0) root         (0)     9870 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/diffusionmodules/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.530202 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/distributions/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/distributions/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     3097 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/distributions/distributions.py
+-rwxr-xr-x   0 root         (0) root         (0)     3066 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/ema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.540312 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/encoders/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/encoders/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    27449 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/encoders/modules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.561139 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/phoneme_encoder/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/phoneme_encoder/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    14860 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/phoneme_encoder/attentions.py
+-rwxr-xr-x   0 root         (0) root         (0)     4960 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/phoneme_encoder/commons.py
+-rwxr-xr-x   0 root         (0) root         (0)     1590 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/modules/phoneme_encoder/encoder.py
+-rwxr-xr-x   0 root         (0) root         (0)     6022 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_diffusion/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.570904 audioldm2-0.0.7/audioldm2/latent_encoder/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_encoder/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    11286 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/latent_encoder/autoencoder.py
+-rwxr-xr-x   0 root         (0) root         (0)     5657 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.592930 audioldm2-0.0.7/audioldm2/utilities/
+-rwxr-xr-x   0 root         (0) root         (0)       62 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/utilities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.614077 audioldm2-0.0.7/audioldm2/utilities/audio/
+-rwxr-xr-x   0 root         (0) root         (0)       73 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/utilities/audio/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2642 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/utilities/audio/audio_processing.py
+-rwxr-xr-x   0 root         (0) root         (0)     6312 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/utilities/audio/stft.py
+-rwxr-xr-x   0 root         (0) root         (0)     2528 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/utilities/audio/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.629353 audioldm2-0.0.7/audioldm2/utilities/data/
+-rwxr-xr-x   0 root         (0) root         (0)       29 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/utilities/data/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    15063 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/utilities/data/add_on.py
+-rwxr-xr-x   0 root         (0) root         (0)    20175 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/utilities/data/dataset.py
+-rwxr-xr-x   0 root         (0) root         (0)     3589 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/utilities/model.py
+-rwxr-xr-x   0 root         (0) root         (0)    19538 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/utilities/sampler.py
+-rwxr-xr-x   0 root         (0) root         (0)    18077 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/utilities/tools.py
+-rwxr-xr-x   0 root         (0) root         (0)    12389 2023-08-05 14:48:09.000000 audioldm2-0.0.7/audioldm2/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.060819 audioldm2-0.0.7/audioldm2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5011 2023-08-05 16:22:46.000000 audioldm2-0.0.7/audioldm2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4806 2023-08-05 16:22:47.000000 audioldm2-0.0.7/audioldm2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-05 16:22:46.000000 audioldm2-0.0.7/audioldm2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      218 2023-08-05 16:22:46.000000 audioldm2-0.0.7/audioldm2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-08-05 16:22:46.000000 audioldm2-0.0.7/audioldm2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 16:22:48.640820 audioldm2-0.0.7/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     3007 2023-08-05 16:22:02.000000 audioldm2-0.0.7/bin/audioldm2
+-rwxr-xr-x   0 root         (0) root         (0)       32 2023-08-05 14:48:09.000000 audioldm2-0.0.7/bin/audioldm2.cmd
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-05 16:22:48.646195 audioldm2-0.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4445 2023-08-05 16:22:46.000000 audioldm2-0.0.7/setup.py
+-rw-r--r--   0 root         (0) root         (0)     6448 2023-08-05 14:48:09.000000 audioldm2-0.0.7/share_btn.py
```

### Comparing `audioldm2-0.0.6/LICENSE` & `audioldm2-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/PKG-INFO` & `audioldm2-0.0.7/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,10 @@
-Metadata-Version: 2.1
-Name: audioldm2
-Version: 0.0.6
-Summary: This package is written for text-to-audio/music generation.
-Home-page: https://github.com/haoheliu/audioldm2
-Author: Haohe Liu
-Author-email: haoheliu@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 # AudioLDM 2
 
-[![arXiv](https://img.shields.io/badge/arXiv-2301.12503-brightgreen.svg?style=flat-square)](https://arxiv.org/abs/2301.12503)  [![githubio](https://img.shields.io/badge/GitHub.io-Audio_Samples-blue?logo=Github&style=flat-square)](https://audioldm.github.io/)  [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/haoheliu/audioldm-text-to-audio-generation)  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/olaviinha/NeuralTextToAudio/blob/main/AudioLDM_pub.ipynb?force_theme=dark)  [![Replicate](https://replicate.com/jagilley/audio-ldm/badge)](https://replicate.com/jagilley/audio-ldm)
+[![arXiv](https://img.shields.io/badge/arXiv-2301.12503-brightgreen.svg?style=flat-square)](https://arxiv.org/abs/2301.12503)  [![githubio](https://img.shields.io/badge/GitHub.io-Audio_Samples-blue?logo=Github&style=flat-square)](https://audioldm.github.io/audioldm2/)  [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/haoheliu/audioldm2-text2audio-text2music)  
 
 This repo currently support Text-to-Audio Generation (including Music)
 
 <hr>
 
 ## Web APP
 
@@ -81,14 +61,39 @@
 2. **audioldm2-music-665k**: This checkpoint is specialized on music generation. 
 3. **audioldm2-full-large-650k**: This checkpoint is the larger version of audioldm2-full. 
 
 Evaluation result on AudioCaps and MusicCaps evaluation set:
 
 Coming soon.
 
+## Other options
+```shell
+  usage: audioldm2 [-h] [-t TEXT] [-tl TEXT_LIST] [-s SAVE_PATH] [--model_name {audioldm2-full,audioldm2-music-665k,audioldm2-full-large-650k}] [-b BATCHSIZE] [--ddim_steps DDIM_STEPS] [-gs GUIDANCE_SCALE]
+                  [-n N_CANDIDATE_GEN_PER_TEXT] [--seed SEED]
+
+  optional arguments:
+    -h, --help            show this help message and exit
+    -t TEXT, --text TEXT  Text prompt to the model for audio generation
+    -tl TEXT_LIST, --text_list TEXT_LIST
+                          A file that contains text prompt to the model for audio generation
+    -s SAVE_PATH, --save_path SAVE_PATH
+                          The path to save model output
+    --model_name {audioldm2-full,audioldm2-music-665k,audioldm2-full-large-650k}
+                          The checkpoint you gonna use
+    -b BATCHSIZE, --batchsize BATCHSIZE
+                          Generate how many samples at the same time
+    --ddim_steps DDIM_STEPS
+                          The sampling step for DDIM
+    -gs GUIDANCE_SCALE, --guidance_scale GUIDANCE_SCALE
+                          Guidance scale (Large => better quality and relavancy to text; Small => better diversity)
+    -n N_CANDIDATE_GEN_PER_TEXT, --n_candidate_gen_per_text N_CANDIDATE_GEN_PER_TEXT
+                          Automatic quality control. This number control the number of candidates (e.g., generate three audios and choose the best to show you). A Larger value usually lead to better quality with
+                          heavier computation
+    --seed SEED           Change this value (any integer number) will lead to a different generation result.
+```
 
 ## Cite this work
 If you found this tool useful, please consider citing
 
 ```bibtex
     AudioLDM 2 paper coming soon
 ```
@@ -98,9 +103,7 @@
   title={AudioLDM: Text-to-Audio Generation with Latent Diffusion Models},
   author={Liu, Haohe and Chen, Zehua and Yuan, Yi and Mei, Xinhao and Liu, Xubo and Mandic, Danilo and Wang, Wenwu and Plumbley, Mark D},
   journal={arXiv preprint arXiv:2301.12503},
   year={2023}
 }
 ```
 
-
-
```

### Comparing `audioldm2-0.0.6/app.py` & `audioldm2-0.0.7/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 from huggingface_hub import hf_hub_download
 import torch
 import os
 
-os.environ["TOKENIZERS_PARALLELISM"] = "true"
-
 import gradio as gr
 from audioldm2 import text_to_audio, build_model
 from share_btn import community_icon_html, loading_icon_html, share_js
 
+os.environ["TOKENIZERS_PARALLELISM"] = "true"
+
+
+default_checkpoint="audioldm2-full"
 audioldm = None
 current_model_name = None
 
 def text2audio(
     text,
     guidance_scale,
     random_seed,
     n_candidates,
-    model_name="audioldm2-full",
+    model_name=default_checkpoint,
 ):
     global audioldm, current_model_name
     torch.set_float32_matmul_precision("high")
 
     if audioldm is None or model_name != current_model_name:
         audioldm = build_model(model_name=model_name)
         current_model_name = model_name
         audioldm = torch.compile(audioldm)
 
+    # print(text, length, guidance_scale)
     waveform = text_to_audio(
         latent_diffusion=audioldm,
         text=text,
         seed=random_seed,
         duration=10,
         guidance_scale=guidance_scale,
         n_candidate_gen_per_text=int(n_candidates),
@@ -290,43 +293,43 @@
         gr.Examples(
             [
                 [
                     "An excited crowd cheering at a sports game.",
                     3.5,
                     45,
                     3,
-                    "audioldm2-full",
+                    default_checkpoint,
                 ],
                 [
                     "A cat is meowing for attention.",
                     3.5,
                     45,
                     3,
-                    "audioldm2-full",
+                    default_checkpoint,
                 ],
                 [
                     "Birds singing sweetly in a blooming garden.",
                     3.5,
                     45,
                     3,
-                    "audioldm2-full",
+                    default_checkpoint,
                 ],
                 [
                     "A modern synthesizer creating futuristic soundscapes.",
                     3.5,
                     45,
                     3,
-                    "audioldm2-full",
+                    default_checkpoint,
                 ],
                 [
                     "The vibrant beat of Brazilian samba drums.",
                     3.5,
                     45,
                     3,
-                    "audioldm2-full",
+                    default_checkpoint,
                 ],
             ],
             fn=text2audio,
             # inputs=[textbox, duration, guidance_scale, seed, n_candidates, model_name],
             inputs=[textbox, guidance_scale, seed, n_candidates],
             outputs=[outputs],
             cache_examples=True,
```

### Comparing `audioldm2-0.0.6/audioldm2/audiomae_gen/sequence_input.py` & `audioldm2-0.0.7/audioldm2/audiomae_gen/sequence_input.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/audiomae_gen/utils.py` & `audioldm2-0.0.7/audioldm2/audiomae_gen/utils.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/clap/open_clip/__init__.py` & `audioldm2-0.0.7/audioldm2/clap/open_clip/__init__.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/clap/open_clip/bpe_simple_vocab_16e6.txt.gz` & `audioldm2-0.0.7/audioldm2/clap/open_clip/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/clap/open_clip/factory.py` & `audioldm2-0.0.7/audioldm2/clap/open_clip/factory.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/clap/open_clip/feature_fusion.py` & `audioldm2-0.0.7/audioldm2/clap/open_clip/feature_fusion.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/clap/open_clip/htsat.py` & `audioldm2-0.0.7/audioldm2/clap/open_clip/htsat.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/clap/open_clip/loss.py` & `audioldm2-0.0.7/audioldm2/clap/open_clip/loss.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/clap/open_clip/model.py` & `audioldm2-0.0.7/audioldm2/clap/open_clip/model.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/clap/open_clip/openai.py` & `audioldm2-0.0.7/audioldm2/clap/open_clip/openai.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/clap/open_clip/pann_model.py` & `audioldm2-0.0.7/audioldm2/clap/open_clip/pann_model.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/clap/open_clip/pretrained.py` & `audioldm2-0.0.7/audioldm2/clap/open_clip/pretrained.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/clap/open_clip/timm_model.py` & `audioldm2-0.0.7/audioldm2/clap/open_clip/timm_model.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/clap/open_clip/tokenizer.py` & `audioldm2-0.0.7/audioldm2/clap/open_clip/tokenizer.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/clap/open_clip/transform.py` & `audioldm2-0.0.7/audioldm2/clap/open_clip/transform.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/clap/open_clip/utils.py` & `audioldm2-0.0.7/audioldm2/clap/open_clip/utils.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/clap/training/audioset_textmap.npy` & `audioldm2-0.0.7/audioldm2/clap/training/audioset_textmap.npy`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/clap/training/bpe_simple_vocab_16e6.txt.gz` & `audioldm2-0.0.7/audioldm2/clap/training/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/clap/training/data.py` & `audioldm2-0.0.7/audioldm2/clap/training/data.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/clap/training/params.py` & `audioldm2-0.0.7/audioldm2/clap/training/params.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/hifigan/models.py` & `audioldm2-0.0.7/audioldm2/hifigan/models.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/hifigan/models_v2.py` & `audioldm2-0.0.7/audioldm2/hifigan/models_v2.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/models/ddim.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/models/ddim.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/models/ddpm.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/models/ddpm.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/models/plms.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/models/plms.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/modules/attention.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/attention.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/AudioMAE.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/AudioMAE.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/models_mae.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/models_mae.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/models_vit.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/models_vit.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/util/crop.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/crop.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/util/datasets.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/datasets.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/util/lars.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/lars.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/util/lr_decay.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/lr_decay.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/util/lr_sched.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/lr_sched.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/util/misc.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/misc.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/util/patch_embed.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/patch_embed.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/util/pos_embed.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/pos_embed.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/modules/audiomae/util/stat.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/audiomae/util/stat.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/modules/diffusionmodules/model.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/diffusionmodules/model.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/modules/diffusionmodules/openaimodel.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/diffusionmodules/openaimodel.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/modules/diffusionmodules/util.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/diffusionmodules/util.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/modules/distributions/distributions.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/modules/ema.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/ema.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/modules/encoders/modules.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/encoders/modules.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/modules/phoneme_encoder/attentions.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/phoneme_encoder/attentions.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/modules/phoneme_encoder/commons.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/phoneme_encoder/commons.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/modules/phoneme_encoder/encoder.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/modules/phoneme_encoder/encoder.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_diffusion/util.py` & `audioldm2-0.0.7/audioldm2/latent_diffusion/util.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/latent_encoder/autoencoder.py` & `audioldm2-0.0.7/audioldm2/latent_encoder/autoencoder.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/pipeline.py` & `audioldm2-0.0.7/audioldm2/pipeline.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/utilities/audio/audio_processing.py` & `audioldm2-0.0.7/audioldm2/utilities/audio/audio_processing.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/utilities/audio/stft.py` & `audioldm2-0.0.7/audioldm2/utilities/audio/stft.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/utilities/audio/tools.py` & `audioldm2-0.0.7/audioldm2/utilities/audio/tools.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/utilities/data/add_on.py` & `audioldm2-0.0.7/audioldm2/utilities/data/add_on.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/utilities/data/dataset.py` & `audioldm2-0.0.7/audioldm2/utilities/data/dataset.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/utilities/model.py` & `audioldm2-0.0.7/audioldm2/utilities/model.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/utilities/sampler.py` & `audioldm2-0.0.7/audioldm2/utilities/sampler.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/utilities/tools.py` & `audioldm2-0.0.7/audioldm2/utilities/tools.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2/utils.py` & `audioldm2-0.0.7/audioldm2/utils.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.6/audioldm2.egg-info/SOURCES.txt` & `audioldm2-0.0.7/audioldm2.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 app.py
 setup.py
 share_btn.py
-test.py
 audioldm2/__init__.py
 audioldm2/pipeline.py
 audioldm2/utils.py
 audioldm2.egg-info/PKG-INFO
 audioldm2.egg-info/SOURCES.txt
 audioldm2.egg-info/dependency_links.txt
 audioldm2.egg-info/requires.txt
```

### Comparing `audioldm2-0.0.6/bin/audioldm2` & `audioldm2-0.0.7/bin/audioldm2`

 * *Files 1% similar despite different names*

```diff
@@ -119,8 +119,8 @@
         duration=duration,
         guidance_scale=guidance_scale,
         ddim_steps=args.ddim_steps,
         n_candidate_gen_per_text=n_candidate_gen_per_text,
         batchsize=args.batchsize,
     )
      
-    save_wave(waveform, save_path, name=text)
+    save_wave(waveform, save_path, name=text[:256])
```

### Comparing `audioldm2-0.0.6/setup.py` & `audioldm2-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # Package meta-data.
 NAME = "audioldm2"
 DESCRIPTION = "This package is written for text-to-audio/music generation."
 URL = "https://github.com/haoheliu/audioldm2"
 EMAIL = "haoheliu@gmail.com"
 AUTHOR = "Haohe Liu"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "torch>=1.13.0",
     "torchaudio>=0.13.0",
     "torchvision>=0.14.0",
     "tqdm",
```

### Comparing `audioldm2-0.0.6/share_btn.py` & `audioldm2-0.0.7/share_btn.py`

 * *Files identical despite different names*

