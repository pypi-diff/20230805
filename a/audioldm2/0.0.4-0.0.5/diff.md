# Comparing `tmp/audioldm2-0.0.4.tar.gz` & `tmp/audioldm2-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioldm2-0.0.4.tar", last modified: Sat Aug  5 11:34:51 2023, max compression
+gzip compressed data, was "audioldm2-0.0.5.tar", last modified: Sat Aug  5 11:38:17 2023, max compression
```

## Comparing `audioldm2-0.0.4.tar` & `audioldm2-0.0.5.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:34:51.682171 audioldm2-0.0.4/
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    20845 2023-08-04 16:01:51.000000 audioldm2-0.0.4/LICENSE
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       87 2023-08-04 16:01:51.000000 audioldm2-0.0.4/MANIFEST.in
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     2672 2023-08-05 11:34:51.678338 audioldm2-0.0.4/PKG-INFO
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     1995 2023-08-05 11:33:01.000000 audioldm2-0.0.4/README.md
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    14066 2023-08-04 16:59:32.000000 audioldm2-0.0.4/app.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:34:51.503221 audioldm2-0.0.4/audioldm2/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      105 2023-08-04 16:21:31.000000 audioldm2-0.0.4/audioldm2/__init__.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:34:51.516626 audioldm2-0.0.4/audioldm2/audiomae_gen/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       46 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/audiomae_gen/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    16876 2023-08-04 16:07:32.000000 audioldm2-0.0.4/audioldm2/audiomae_gen/sequence_input.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      730 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/audiomae_gen/utils.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:34:51.522957 audioldm2-0.0.4/audioldm2/clap/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/__init__.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:34:51.547110 audioldm2-0.0.4/audioldm2/clap/open_clip/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      639 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)  1356917 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/bpe_simple_vocab_16e6.txt.gz
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    10985 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/factory.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     7177 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/feature_fusion.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    48069 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/htsat.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    16096 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/loss.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    32924 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/model.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:34:51.583912 audioldm2-0.0.4/audioldm2/clap/open_clip/model_configs/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/model_configs/HTSAT-base.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      498 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/model_configs/HTSAT-large.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/model_configs/HTSAT-tiny.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/model_configs/PANN-10.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/model_configs/PANN-14-fmax-18k.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/model_configs/PANN-14-tiny-transformer.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/model_configs/PANN-14-win-1536.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/model_configs/PANN-14.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      495 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/model_configs/PANN-6.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      388 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/model_configs/RN101-quickgelu.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      364 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/model_configs/RN101.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      389 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/model_configs/RN50-quickgelu.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      364 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/model_configs/RN50.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      365 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/model_configs/RN50x16.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      365 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/model_configs/RN50x4.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      294 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/model_configs/ViT-B-16.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      318 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/model_configs/ViT-B-32-quickgelu.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      294 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/model_configs/ViT-B-32.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      296 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/model_configs/ViT-L-14.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5023 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/openai.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    23369 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/pann_model.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6440 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/pretrained.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     4332 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/timm_model.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6400 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/tokenizer.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1051 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/transform.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    11963 2023-08-05 10:50:27.000000 audioldm2-0.0.4/audioldm2/clap/open_clip/utils.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:34:51.598434 audioldm2-0.0.4/audioldm2/clap/training/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/training/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    84448 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/training/audioset_textmap.npy
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)  1356917 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/training/bpe_simple_vocab_16e6.txt.gz
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    29672 2023-08-04 17:59:22.000000 audioldm2-0.0.4/audioldm2/clap/training/data.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    17202 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/clap/training/params.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:34:51.602031 audioldm2-0.0.4/audioldm2/hifigan/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      230 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/hifigan/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5524 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/hifigan/models.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    12819 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/hifigan/models_v2.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:34:51.606995 audioldm2-0.0.4/audioldm2/latent_diffusion/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/__init__.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:34:51.610318 audioldm2-0.0.4/audioldm2/latent_diffusion/models/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/models/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    17259 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/models/ddim.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    65611 2023-08-04 16:47:57.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/models/ddpm.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    12849 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/models/plms.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:34:51.616466 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    15753 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/attention.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:34:51.621268 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5381 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/AudioMAE.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    21105 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/models_mae.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     7684 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/models_vit.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:34:51.635220 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/util/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1363 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/util/crop.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1924 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/util/datasets.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2026 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/util/lars.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2445 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/util/lr_decay.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      885 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/util/lr_sched.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    14517 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/util/misc.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     4381 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/util/patch_embed.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     8632 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/util/pos_embed.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2259 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/util/stat.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:34:51.641680 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/diffusionmodules/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/diffusionmodules/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    34452 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/diffusionmodules/model.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    40223 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/diffusionmodules/openaimodel.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     9870 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/diffusionmodules/util.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:34:51.648408 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/distributions/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/distributions/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3097 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/distributions/distributions.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3066 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/ema.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:34:51.651767 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/encoders/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/encoders/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    27449 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/encoders/modules.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:34:51.654968 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/phoneme_encoder/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/phoneme_encoder/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    14860 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/phoneme_encoder/attentions.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     4960 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/phoneme_encoder/commons.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1590 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/modules/phoneme_encoder/encoder.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6022 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_diffusion/util.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:34:51.660889 audioldm2-0.0.4/audioldm2/latent_encoder/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_encoder/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    11286 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/latent_encoder/autoencoder.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5805 2023-08-04 16:58:20.000000 audioldm2-0.0.4/audioldm2/pipeline.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:34:51.663556 audioldm2-0.0.4/audioldm2/utilities/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       62 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/utilities/__init__.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:34:51.670045 audioldm2-0.0.4/audioldm2/utilities/audio/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       73 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/utilities/audio/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2642 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/utilities/audio/audio_processing.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6312 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/utilities/audio/stft.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2528 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/utilities/audio/tools.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:34:51.676250 audioldm2-0.0.4/audioldm2/utilities/data/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       29 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/utilities/data/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    15063 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/utilities/data/add_on.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    20175 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/utilities/data/dataset.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3589 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/utilities/model.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    19538 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/utilities/sampler.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    18077 2023-08-04 16:01:51.000000 audioldm2-0.0.4/audioldm2/utilities/tools.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    13631 2023-08-05 09:55:26.000000 audioldm2-0.0.4/audioldm2/utils.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:34:51.514691 audioldm2-0.0.4/audioldm2.egg-info/
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     2672 2023-08-05 11:34:51.000000 audioldm2-0.0.4/audioldm2.egg-info/PKG-INFO
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     4806 2023-08-05 11:34:51.000000 audioldm2-0.0.4/audioldm2.egg-info/SOURCES.txt
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)        1 2023-08-05 11:34:51.000000 audioldm2-0.0.4/audioldm2.egg-info/dependency_links.txt
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      194 2023-08-05 11:34:51.000000 audioldm2-0.0.4/audioldm2.egg-info/requires.txt
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       10 2023-08-05 11:34:51.000000 audioldm2-0.0.4/audioldm2.egg-info/top_level.txt
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:34:51.681285 audioldm2-0.0.4/bin/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3061 2023-08-05 10:51:15.000000 audioldm2-0.0.4/bin/audioldm2
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       32 2023-08-04 16:01:51.000000 audioldm2-0.0.4/bin/audioldm2.cmd
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       38 2023-08-05 11:34:51.679670 audioldm2-0.0.4/setup.cfg
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     4414 2023-08-05 11:34:26.000000 audioldm2-0.0.4/setup.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     6448 2023-08-04 16:01:51.000000 audioldm2-0.0.4/share_btn.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:38:17.202132 audioldm2-0.0.5/
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    20845 2023-08-04 16:01:51.000000 audioldm2-0.0.5/LICENSE
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       87 2023-08-04 16:01:51.000000 audioldm2-0.0.5/MANIFEST.in
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     2672 2023-08-05 11:38:17.198120 audioldm2-0.0.5/PKG-INFO
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     1995 2023-08-05 11:33:01.000000 audioldm2-0.0.5/README.md
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    14066 2023-08-04 16:59:32.000000 audioldm2-0.0.5/app.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:38:16.987037 audioldm2-0.0.5/audioldm2/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      105 2023-08-04 16:21:31.000000 audioldm2-0.0.5/audioldm2/__init__.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:38:17.001911 audioldm2-0.0.5/audioldm2/audiomae_gen/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       46 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/audiomae_gen/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    16876 2023-08-04 16:07:32.000000 audioldm2-0.0.5/audioldm2/audiomae_gen/sequence_input.py
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      730 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/audiomae_gen/utils.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:38:17.007322 audioldm2-0.0.5/audioldm2/clap/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/__init__.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:38:17.031738 audioldm2-0.0.5/audioldm2/clap/open_clip/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      639 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)  1356917 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/bpe_simple_vocab_16e6.txt.gz
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    10985 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/factory.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     7177 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/feature_fusion.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    48069 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/htsat.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    16096 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/loss.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    32924 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/model.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:38:17.065700 audioldm2-0.0.5/audioldm2/clap/open_clip/model_configs/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/model_configs/HTSAT-base.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      498 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/model_configs/HTSAT-large.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/model_configs/HTSAT-tiny.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/model_configs/PANN-10.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/model_configs/PANN-14-fmax-18k.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/model_configs/PANN-14-tiny-transformer.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/model_configs/PANN-14-win-1536.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/model_configs/PANN-14.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      495 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/model_configs/PANN-6.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      388 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/model_configs/RN101-quickgelu.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      364 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/model_configs/RN101.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      389 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/model_configs/RN50-quickgelu.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      364 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/model_configs/RN50.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      365 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/model_configs/RN50x16.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      365 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/model_configs/RN50x4.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      294 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/model_configs/ViT-B-16.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      318 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/model_configs/ViT-B-32-quickgelu.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      294 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/model_configs/ViT-B-32.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      296 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/model_configs/ViT-L-14.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5023 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/openai.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    23369 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/pann_model.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6440 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/pretrained.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     4332 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/timm_model.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6400 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/tokenizer.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1051 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/transform.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    11963 2023-08-05 10:50:27.000000 audioldm2-0.0.5/audioldm2/clap/open_clip/utils.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:38:17.082394 audioldm2-0.0.5/audioldm2/clap/training/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/training/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    84448 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/training/audioset_textmap.npy
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)  1356917 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/training/bpe_simple_vocab_16e6.txt.gz
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    29672 2023-08-04 17:59:22.000000 audioldm2-0.0.5/audioldm2/clap/training/data.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    17202 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/clap/training/params.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:38:17.086598 audioldm2-0.0.5/audioldm2/hifigan/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      230 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/hifigan/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5524 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/hifigan/models.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    12819 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/hifigan/models_v2.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:38:17.091391 audioldm2-0.0.5/audioldm2/latent_diffusion/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/__init__.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:38:17.095058 audioldm2-0.0.5/audioldm2/latent_diffusion/models/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/models/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    17259 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/models/ddim.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    65611 2023-08-04 16:47:57.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/models/ddpm.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    12849 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/models/plms.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:38:17.101982 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    15753 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/attention.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:38:17.109262 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5381 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/AudioMAE.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    21105 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/models_mae.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     7684 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/models_vit.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:38:17.135558 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/util/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1363 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/util/crop.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1924 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/util/datasets.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2026 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/util/lars.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2445 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/util/lr_decay.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      885 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/util/lr_sched.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    14517 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/util/misc.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     4381 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/util/patch_embed.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     8632 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/util/pos_embed.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2259 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/util/stat.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:38:17.150722 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/diffusionmodules/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/diffusionmodules/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    34452 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/diffusionmodules/model.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    40223 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/diffusionmodules/openaimodel.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     9870 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/diffusionmodules/util.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:38:17.158747 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/distributions/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/distributions/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3097 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/distributions/distributions.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3066 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/ema.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:38:17.163587 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/encoders/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/encoders/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    27449 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/encoders/modules.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:38:17.169418 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/phoneme_encoder/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/phoneme_encoder/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    14860 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/phoneme_encoder/attentions.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     4960 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/phoneme_encoder/commons.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1590 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/modules/phoneme_encoder/encoder.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6022 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_diffusion/util.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:38:17.179175 audioldm2-0.0.5/audioldm2/latent_encoder/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_encoder/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    11286 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/latent_encoder/autoencoder.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5805 2023-08-04 16:58:20.000000 audioldm2-0.0.5/audioldm2/pipeline.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:38:17.182463 audioldm2-0.0.5/audioldm2/utilities/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       62 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/utilities/__init__.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:38:17.188748 audioldm2-0.0.5/audioldm2/utilities/audio/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       73 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/utilities/audio/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2642 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/utilities/audio/audio_processing.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6312 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/utilities/audio/stft.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2528 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/utilities/audio/tools.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:38:17.196488 audioldm2-0.0.5/audioldm2/utilities/data/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       29 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/utilities/data/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    15063 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/utilities/data/add_on.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    20175 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/utilities/data/dataset.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3589 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/utilities/model.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    19538 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/utilities/sampler.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    18077 2023-08-04 16:01:51.000000 audioldm2-0.0.5/audioldm2/utilities/tools.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    13631 2023-08-05 09:55:26.000000 audioldm2-0.0.5/audioldm2/utils.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:38:16.999906 audioldm2-0.0.5/audioldm2.egg-info/
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     2672 2023-08-05 11:38:16.000000 audioldm2-0.0.5/audioldm2.egg-info/PKG-INFO
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     4806 2023-08-05 11:38:16.000000 audioldm2-0.0.5/audioldm2.egg-info/SOURCES.txt
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)        1 2023-08-05 11:38:16.000000 audioldm2-0.0.5/audioldm2.egg-info/dependency_links.txt
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      194 2023-08-05 11:38:16.000000 audioldm2-0.0.5/audioldm2.egg-info/requires.txt
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       10 2023-08-05 11:38:16.000000 audioldm2-0.0.5/audioldm2.egg-info/top_level.txt
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 11:38:17.201541 audioldm2-0.0.5/bin/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3114 2023-08-05 11:37:47.000000 audioldm2-0.0.5/bin/audioldm2
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       32 2023-08-04 16:01:51.000000 audioldm2-0.0.5/bin/audioldm2.cmd
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       38 2023-08-05 11:38:17.199376 audioldm2-0.0.5/setup.cfg
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     4414 2023-08-05 11:38:12.000000 audioldm2-0.0.5/setup.py
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     6448 2023-08-04 16:01:51.000000 audioldm2-0.0.5/share_btn.py
```

### Comparing `audioldm2-0.0.4/LICENSE` & `audioldm2-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/PKG-INFO` & `audioldm2-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioldm2
-Version: 0.0.4
+Version: 0.0.5
 Summary: This package is written for text-to-audio/music generation.
 Home-page: https://github.com/haoheliu/audioldm2
 Author: Haohe Liu
 Author-email: haoheliu@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `audioldm2-0.0.4/README.md` & `audioldm2-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/app.py` & `audioldm2-0.0.5/app.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/audiomae_gen/sequence_input.py` & `audioldm2-0.0.5/audioldm2/audiomae_gen/sequence_input.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/audiomae_gen/utils.py` & `audioldm2-0.0.5/audioldm2/audiomae_gen/utils.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/clap/open_clip/__init__.py` & `audioldm2-0.0.5/audioldm2/clap/open_clip/__init__.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/clap/open_clip/bpe_simple_vocab_16e6.txt.gz` & `audioldm2-0.0.5/audioldm2/clap/open_clip/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/clap/open_clip/factory.py` & `audioldm2-0.0.5/audioldm2/clap/open_clip/factory.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/clap/open_clip/feature_fusion.py` & `audioldm2-0.0.5/audioldm2/clap/open_clip/feature_fusion.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/clap/open_clip/htsat.py` & `audioldm2-0.0.5/audioldm2/clap/open_clip/htsat.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/clap/open_clip/loss.py` & `audioldm2-0.0.5/audioldm2/clap/open_clip/loss.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/clap/open_clip/model.py` & `audioldm2-0.0.5/audioldm2/clap/open_clip/model.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/clap/open_clip/openai.py` & `audioldm2-0.0.5/audioldm2/clap/open_clip/openai.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/clap/open_clip/pann_model.py` & `audioldm2-0.0.5/audioldm2/clap/open_clip/pann_model.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/clap/open_clip/pretrained.py` & `audioldm2-0.0.5/audioldm2/clap/open_clip/pretrained.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/clap/open_clip/timm_model.py` & `audioldm2-0.0.5/audioldm2/clap/open_clip/timm_model.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/clap/open_clip/tokenizer.py` & `audioldm2-0.0.5/audioldm2/clap/open_clip/tokenizer.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/clap/open_clip/transform.py` & `audioldm2-0.0.5/audioldm2/clap/open_clip/transform.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/clap/open_clip/utils.py` & `audioldm2-0.0.5/audioldm2/clap/open_clip/utils.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/clap/training/audioset_textmap.npy` & `audioldm2-0.0.5/audioldm2/clap/training/audioset_textmap.npy`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/clap/training/bpe_simple_vocab_16e6.txt.gz` & `audioldm2-0.0.5/audioldm2/clap/training/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/clap/training/data.py` & `audioldm2-0.0.5/audioldm2/clap/training/data.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/clap/training/params.py` & `audioldm2-0.0.5/audioldm2/clap/training/params.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/hifigan/models.py` & `audioldm2-0.0.5/audioldm2/hifigan/models.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/hifigan/models_v2.py` & `audioldm2-0.0.5/audioldm2/hifigan/models_v2.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/models/ddim.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/models/ddim.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/models/ddpm.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/models/ddpm.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/models/plms.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/models/plms.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/modules/attention.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/modules/attention.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/AudioMAE.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/AudioMAE.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/models_mae.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/models_mae.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/models_vit.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/models_vit.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/util/crop.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/util/crop.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/util/datasets.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/util/datasets.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/util/lars.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/util/lars.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/util/lr_decay.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/util/lr_decay.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/util/lr_sched.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/util/lr_sched.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/util/misc.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/util/misc.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/util/patch_embed.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/util/patch_embed.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/util/pos_embed.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/util/pos_embed.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/modules/audiomae/util/stat.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/modules/audiomae/util/stat.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/modules/diffusionmodules/model.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/modules/diffusionmodules/model.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/modules/diffusionmodules/openaimodel.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/modules/diffusionmodules/openaimodel.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/modules/diffusionmodules/util.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/modules/diffusionmodules/util.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/modules/distributions/distributions.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/modules/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/modules/ema.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/modules/ema.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/modules/encoders/modules.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/modules/encoders/modules.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/modules/phoneme_encoder/attentions.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/modules/phoneme_encoder/attentions.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/modules/phoneme_encoder/commons.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/modules/phoneme_encoder/commons.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/modules/phoneme_encoder/encoder.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/modules/phoneme_encoder/encoder.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_diffusion/util.py` & `audioldm2-0.0.5/audioldm2/latent_diffusion/util.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/latent_encoder/autoencoder.py` & `audioldm2-0.0.5/audioldm2/latent_encoder/autoencoder.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/pipeline.py` & `audioldm2-0.0.5/audioldm2/pipeline.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/utilities/audio/audio_processing.py` & `audioldm2-0.0.5/audioldm2/utilities/audio/audio_processing.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/utilities/audio/stft.py` & `audioldm2-0.0.5/audioldm2/utilities/audio/stft.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/utilities/audio/tools.py` & `audioldm2-0.0.5/audioldm2/utilities/audio/tools.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/utilities/data/add_on.py` & `audioldm2-0.0.5/audioldm2/utilities/data/add_on.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/utilities/data/dataset.py` & `audioldm2-0.0.5/audioldm2/utilities/data/dataset.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/utilities/model.py` & `audioldm2-0.0.5/audioldm2/utilities/model.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/utilities/sampler.py` & `audioldm2-0.0.5/audioldm2/utilities/sampler.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/utilities/tools.py` & `audioldm2-0.0.5/audioldm2/utilities/tools.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2/utils.py` & `audioldm2-0.0.5/audioldm2/utils.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/audioldm2.egg-info/PKG-INFO` & `audioldm2-0.0.5/audioldm2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioldm2
-Version: 0.0.4
+Version: 0.0.5
 Summary: This package is written for text-to-audio/music generation.
 Home-page: https://github.com/haoheliu/audioldm2
 Author: Haohe Liu
 Author-email: haoheliu@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `audioldm2-0.0.4/audioldm2.egg-info/SOURCES.txt` & `audioldm2-0.0.5/audioldm2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.4/bin/audioldm2` & `audioldm2-0.0.5/bin/audioldm2`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 parser.add_argument(
     "--model_name",
     type=str,
     required=False,
     help="The checkpoint you gonna use",
     default="audioldm2-full",
-    choices=["audioldm2-full"]
+    choices=["audioldm2-full", "audioldm2-music-665k", "audioldm2-full-large-650k"]
 )
 
 parser.add_argument(
     "-b",
     "--batchsize",
     type=int,
     required=False,
```

### Comparing `audioldm2-0.0.4/setup.py` & `audioldm2-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # Package meta-data.
 NAME = "audioldm2"
 DESCRIPTION = "This package is written for text-to-audio/music generation."
 URL = "https://github.com/haoheliu/audioldm2"
 EMAIL = "haoheliu@gmail.com"
 AUTHOR = "Haohe Liu"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "torch>=1.13.0",
     "torchaudio>=0.13.0",
     "torchvision>=0.14.0",
     "tqdm",
```

### Comparing `audioldm2-0.0.4/share_btn.py` & `audioldm2-0.0.5/share_btn.py`

 * *Files identical despite different names*

