# Comparing `tmp/audioldm2-0.0.2.tar.gz` & `tmp/audioldm2-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioldm2-0.0.2.tar", last modified: Fri Aug  4 17:03:36 2023, max compression
+gzip compressed data, was "audioldm2-0.0.3.tar", last modified: Sat Aug  5 10:51:16 2023, max compression
```

## Comparing `audioldm2-0.0.2.tar` & `audioldm2-0.0.3.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.948281 audioldm2-0.0.2/
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    20845 2023-08-04 16:01:51.000000 audioldm2-0.0.2/LICENSE
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       87 2023-08-04 16:01:51.000000 audioldm2-0.0.2/MANIFEST.in
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      828 2023-08-04 17:03:36.945016 audioldm2-0.0.2/PKG-INFO
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      151 2023-08-04 17:03:11.000000 audioldm2-0.0.2/README.md
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    14066 2023-08-04 16:59:32.000000 audioldm2-0.0.2/app.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:34.686800 audioldm2-0.0.2/audioldm2/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      105 2023-08-04 16:21:31.000000 audioldm2-0.0.2/audioldm2/__init__.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:34.702016 audioldm2-0.0.2/audioldm2/audiomae_gen/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       46 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/audiomae_gen/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    16876 2023-08-04 16:07:32.000000 audioldm2-0.0.2/audioldm2/audiomae_gen/sequence_input.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      730 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/audiomae_gen/utils.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:34.707540 audioldm2-0.0.2/audioldm2/clap/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/__init__.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:34.732854 audioldm2-0.0.2/audioldm2/clap/open_clip/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      639 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)  1356917 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/bpe_simple_vocab_16e6.txt.gz
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    10985 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/factory.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     7177 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/feature_fusion.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    48069 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/htsat.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    16096 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/loss.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    32924 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.827837 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/HTSAT-base.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      498 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/HTSAT-large.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/HTSAT-tiny.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/PANN-10.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/PANN-14-fmax-18k.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/PANN-14-tiny-transformer.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/PANN-14-win-1536.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/PANN-14.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      495 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/PANN-6.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      388 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/RN101-quickgelu.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      364 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/RN101.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      389 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/RN50-quickgelu.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      364 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/RN50.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      365 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/RN50x16.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      365 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/RN50x4.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      294 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/ViT-B-16.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      318 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/ViT-B-32-quickgelu.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      294 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/ViT-B-32.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      296 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/model_configs/ViT-L-14.json
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5023 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/openai.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    23369 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/pann_model.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6440 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/pretrained.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     4332 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/timm_model.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6400 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/tokenizer.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1051 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/transform.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    11952 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/open_clip/utils.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.845663 audioldm2-0.0.2/audioldm2/clap/training/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/training/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    84448 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/training/audioset_textmap.npy
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)  1356917 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/training/bpe_simple_vocab_16e6.txt.gz
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    29418 2023-08-04 16:06:43.000000 audioldm2-0.0.2/audioldm2/clap/training/data.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    17202 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/clap/training/params.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.850367 audioldm2-0.0.2/audioldm2/hifigan/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      230 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/hifigan/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5524 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/hifigan/models.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    12819 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/hifigan/models_v2.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.855969 audioldm2-0.0.2/audioldm2/latent_diffusion/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/__init__.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.859732 audioldm2-0.0.2/audioldm2/latent_diffusion/models/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/models/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    17259 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/models/ddim.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    65611 2023-08-04 16:47:57.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/models/ddpm.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    12849 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/models/plms.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.867241 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    15753 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/attention.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.873412 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5381 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/AudioMAE.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    21105 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/models_mae.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     7684 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/models_vit.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.894510 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1363 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/crop.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1924 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/datasets.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2026 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/lars.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2445 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/lr_decay.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      885 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/lr_sched.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    14517 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/misc.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     4381 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/patch_embed.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     8632 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/pos_embed.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2259 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/stat.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.896852 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/diffusionmodules/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/diffusionmodules/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    34452 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/diffusionmodules/model.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    40223 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/diffusionmodules/openaimodel.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     9870 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/diffusionmodules/util.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.904454 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/distributions/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/distributions/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3097 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/distributions/distributions.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3066 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/ema.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.908410 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/encoders/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/encoders/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    27449 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/encoders/modules.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.912846 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/phoneme_encoder/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/phoneme_encoder/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    14860 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/phoneme_encoder/attentions.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     4960 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/phoneme_encoder/commons.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1590 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/modules/phoneme_encoder/encoder.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6022 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_diffusion/util.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.921017 audioldm2-0.0.2/audioldm2/latent_encoder/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_encoder/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    11286 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/latent_encoder/autoencoder.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5805 2023-08-04 16:58:20.000000 audioldm2-0.0.2/audioldm2/pipeline.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.924642 audioldm2-0.0.2/audioldm2/utilities/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       62 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/utilities/__init__.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.933509 audioldm2-0.0.2/audioldm2/utilities/audio/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       73 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/utilities/audio/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2642 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/utilities/audio/audio_processing.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6312 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/utilities/audio/stft.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2528 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/utilities/audio/tools.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.941172 audioldm2-0.0.2/audioldm2/utilities/data/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       29 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/utilities/data/__init__.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    15063 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/utilities/data/add_on.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    20175 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/utilities/data/dataset.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3589 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/utilities/model.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    19538 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/utilities/sampler.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    18077 2023-08-04 16:01:51.000000 audioldm2-0.0.2/audioldm2/utilities/tools.py
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    12780 2023-08-04 16:13:23.000000 audioldm2-0.0.2/audioldm2/utils.py
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:34.699806 audioldm2-0.0.2/audioldm2.egg-info/
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      828 2023-08-04 17:03:34.000000 audioldm2-0.0.2/audioldm2.egg-info/PKG-INFO
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     4806 2023-08-04 17:03:34.000000 audioldm2-0.0.2/audioldm2.egg-info/SOURCES.txt
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)        1 2023-08-04 17:03:34.000000 audioldm2-0.0.2/audioldm2.egg-info/dependency_links.txt
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      189 2023-08-04 17:03:34.000000 audioldm2-0.0.2/audioldm2.egg-info/requires.txt
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       10 2023-08-04 17:03:34.000000 audioldm2-0.0.2/audioldm2.egg-info/top_level.txt
-drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 17:03:36.946898 audioldm2-0.0.2/bin/
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3065 2023-08-04 17:02:32.000000 audioldm2-0.0.2/bin/audioldm2
--rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       32 2023-08-04 16:01:51.000000 audioldm2-0.0.2/bin/audioldm2.cmd
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       38 2023-08-04 17:03:36.946471 audioldm2-0.0.2/setup.cfg
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     4403 2023-08-04 17:03:22.000000 audioldm2-0.0.2/setup.py
--rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     6448 2023-08-04 16:01:51.000000 audioldm2-0.0.2/share_btn.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 10:51:16.368326 audioldm2-0.0.3/
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    20845 2023-08-04 16:01:51.000000 audioldm2-0.0.3/LICENSE
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       87 2023-08-04 16:01:51.000000 audioldm2-0.0.3/MANIFEST.in
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     1139 2023-08-05 10:51:16.362758 audioldm2-0.0.3/PKG-INFO
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      462 2023-08-04 17:06:40.000000 audioldm2-0.0.3/README.md
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)    14066 2023-08-04 16:59:32.000000 audioldm2-0.0.3/app.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 10:51:11.072692 audioldm2-0.0.3/audioldm2/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      105 2023-08-04 16:21:31.000000 audioldm2-0.0.3/audioldm2/__init__.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 10:51:11.085145 audioldm2-0.0.3/audioldm2/audiomae_gen/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       46 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/audiomae_gen/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    16876 2023-08-04 16:07:32.000000 audioldm2-0.0.3/audioldm2/audiomae_gen/sequence_input.py
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      730 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/audiomae_gen/utils.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 10:51:11.089878 audioldm2-0.0.3/audioldm2/clap/
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/__init__.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 10:51:15.187224 audioldm2-0.0.3/audioldm2/clap/open_clip/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      639 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)  1356917 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/bpe_simple_vocab_16e6.txt.gz
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    10985 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/factory.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     7177 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/feature_fusion.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    48069 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/htsat.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    16096 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/loss.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    32924 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/model.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 10:51:16.242483 audioldm2-0.0.3/audioldm2/clap/open_clip/model_configs/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/model_configs/HTSAT-base.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      498 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/model_configs/HTSAT-large.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/model_configs/HTSAT-tiny.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/model_configs/PANN-10.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/model_configs/PANN-14-fmax-18k.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      496 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/model_configs/PANN-14-tiny-transformer.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/model_configs/PANN-14-win-1536.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      497 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/model_configs/PANN-14.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      495 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/model_configs/PANN-6.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      388 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/model_configs/RN101-quickgelu.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      364 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/model_configs/RN101.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      389 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/model_configs/RN50-quickgelu.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      364 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/model_configs/RN50.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      365 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/model_configs/RN50x16.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      365 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/model_configs/RN50x4.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      294 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/model_configs/ViT-B-16.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      318 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/model_configs/ViT-B-32-quickgelu.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      294 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/model_configs/ViT-B-32.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      296 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/model_configs/ViT-L-14.json
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5023 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/openai.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    23369 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/pann_model.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6440 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/pretrained.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     4332 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/timm_model.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6400 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/tokenizer.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1051 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/transform.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    11963 2023-08-05 10:50:27.000000 audioldm2-0.0.3/audioldm2/clap/open_clip/utils.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 10:51:16.259703 audioldm2-0.0.3/audioldm2/clap/training/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/training/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    84448 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/training/audioset_textmap.npy
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)  1356917 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/training/bpe_simple_vocab_16e6.txt.gz
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    29672 2023-08-04 17:59:22.000000 audioldm2-0.0.3/audioldm2/clap/training/data.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    17202 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/clap/training/params.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 10:51:16.264285 audioldm2-0.0.3/audioldm2/hifigan/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      230 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/hifigan/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5524 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/hifigan/models.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    12819 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/hifigan/models_v2.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 10:51:16.269548 audioldm2-0.0.3/audioldm2/latent_diffusion/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/__init__.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 10:51:16.273203 audioldm2-0.0.3/audioldm2/latent_diffusion/models/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/models/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    17259 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/models/ddim.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    65611 2023-08-04 16:47:57.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/models/ddpm.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    12849 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/models/plms.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 10:51:16.280557 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    15753 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/attention.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 10:51:16.286158 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5381 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/AudioMAE.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    21105 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/models_mae.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     7684 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/models_vit.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 10:51:16.308327 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/util/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1363 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/util/crop.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1924 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/util/datasets.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2026 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/util/lars.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2445 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/util/lr_decay.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)      885 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/util/lr_sched.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    14517 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/util/misc.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     4381 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/util/patch_embed.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     8632 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/util/pos_embed.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2259 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/util/stat.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 10:51:16.310770 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/diffusionmodules/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/diffusionmodules/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    34452 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/diffusionmodules/model.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    40223 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/diffusionmodules/openaimodel.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     9870 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/diffusionmodules/util.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 10:51:16.321614 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/distributions/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/distributions/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3097 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/distributions/distributions.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3066 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/ema.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 10:51:16.326449 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/encoders/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/encoders/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    27449 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/encoders/modules.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 10:51:16.330664 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/phoneme_encoder/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/phoneme_encoder/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    14860 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/phoneme_encoder/attentions.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     4960 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/phoneme_encoder/commons.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     1590 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/modules/phoneme_encoder/encoder.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6022 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_diffusion/util.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 10:51:16.337780 audioldm2-0.0.3/audioldm2/latent_encoder/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_encoder/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    11286 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/latent_encoder/autoencoder.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     5805 2023-08-04 16:58:20.000000 audioldm2-0.0.3/audioldm2/pipeline.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 10:51:16.341149 audioldm2-0.0.3/audioldm2/utilities/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       62 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/utilities/__init__.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 10:51:16.348935 audioldm2-0.0.3/audioldm2/utilities/audio/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       73 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/utilities/audio/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2642 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/utilities/audio/audio_processing.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     6312 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/utilities/audio/stft.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     2528 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/utilities/audio/tools.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 10:51:16.357767 audioldm2-0.0.3/audioldm2/utilities/data/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       29 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/utilities/data/__init__.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    15063 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/utilities/data/add_on.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    20175 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/utilities/data/dataset.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3589 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/utilities/model.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    19538 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/utilities/sampler.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    18077 2023-08-04 16:01:51.000000 audioldm2-0.0.3/audioldm2/utilities/tools.py
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)    13631 2023-08-05 09:55:26.000000 audioldm2-0.0.3/audioldm2/utils.py
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 10:51:15.161608 audioldm2-0.0.3/audioldm2.egg-info/
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     1139 2023-08-05 10:51:14.000000 audioldm2-0.0.3/audioldm2.egg-info/PKG-INFO
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     4806 2023-08-05 10:51:15.000000 audioldm2-0.0.3/audioldm2.egg-info/SOURCES.txt
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)        1 2023-08-05 10:51:14.000000 audioldm2-0.0.3/audioldm2.egg-info/dependency_links.txt
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)      189 2023-08-05 10:51:14.000000 audioldm2-0.0.3/audioldm2.egg-info/requires.txt
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       10 2023-08-05 10:51:14.000000 audioldm2-0.0.3/audioldm2.egg-info/top_level.txt
+drwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)        0 2023-08-05 10:51:16.364697 audioldm2-0.0.3/bin/
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)     3061 2023-08-05 10:51:15.000000 audioldm2-0.0.3/bin/audioldm2
+-rwxr-xr-x   0 hl01486  (314231) A-EE00-PGR (5000093)       32 2023-08-04 16:01:51.000000 audioldm2-0.0.3/bin/audioldm2.cmd
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)       38 2023-08-05 10:51:16.363903 audioldm2-0.0.3/setup.cfg
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     4403 2023-08-04 17:59:41.000000 audioldm2-0.0.3/setup.py
+-rw-r--r--   0 hl01486  (314231) A-EE00-PGR (5000093)     6448 2023-08-04 16:01:51.000000 audioldm2-0.0.3/share_btn.py
```

### Comparing `audioldm2-0.0.2/LICENSE` & `audioldm2-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/app.py` & `audioldm2-0.0.3/app.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/audiomae_gen/sequence_input.py` & `audioldm2-0.0.3/audioldm2/audiomae_gen/sequence_input.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/audiomae_gen/utils.py` & `audioldm2-0.0.3/audioldm2/audiomae_gen/utils.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/clap/open_clip/__init__.py` & `audioldm2-0.0.3/audioldm2/clap/open_clip/__init__.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/clap/open_clip/bpe_simple_vocab_16e6.txt.gz` & `audioldm2-0.0.3/audioldm2/clap/open_clip/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/clap/open_clip/factory.py` & `audioldm2-0.0.3/audioldm2/clap/open_clip/factory.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/clap/open_clip/feature_fusion.py` & `audioldm2-0.0.3/audioldm2/clap/open_clip/feature_fusion.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/clap/open_clip/htsat.py` & `audioldm2-0.0.3/audioldm2/clap/open_clip/htsat.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/clap/open_clip/loss.py` & `audioldm2-0.0.3/audioldm2/clap/open_clip/loss.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/clap/open_clip/model.py` & `audioldm2-0.0.3/audioldm2/clap/open_clip/model.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/clap/open_clip/openai.py` & `audioldm2-0.0.3/audioldm2/clap/open_clip/openai.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/clap/open_clip/pann_model.py` & `audioldm2-0.0.3/audioldm2/clap/open_clip/pann_model.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/clap/open_clip/pretrained.py` & `audioldm2-0.0.3/audioldm2/clap/open_clip/pretrained.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/clap/open_clip/timm_model.py` & `audioldm2-0.0.3/audioldm2/clap/open_clip/timm_model.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/clap/open_clip/tokenizer.py` & `audioldm2-0.0.3/audioldm2/clap/open_clip/tokenizer.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/clap/open_clip/transform.py` & `audioldm2-0.0.3/audioldm2/clap/open_clip/transform.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/clap/open_clip/utils.py` & `audioldm2-0.0.3/audioldm2/clap/open_clip/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 import torch
 from torch import nn as nn
 from torchvision.ops.misc import FrozenBatchNorm2d
 import logging
-import h5py
 from tqdm import tqdm
 import random
 import json
 import os
 import pathlib
 
 # TODO: (yusong) this not a good place to store those information and does not scale. Need to be fixed later.
@@ -213,27 +212,26 @@
     )
     """tensor for padding"""
 
     output = torch.cat((framewise_output, pad), dim=1)
     """(batch_size, frames_num, classes_num)"""
 
 
-def process_ipc(index_path, classes_num, filename):
-    # load data
-    logging.info("Load Data...............")
-    ipc = [[] for _ in range(classes_num)]
-    with h5py.File(index_path, "r") as f:
-        for i in tqdm(range(len(f["target"]))):
-            t_class = np.where(f["target"][i])[0]
-            for t in t_class:
-                ipc[t].append(i)
-    print(ipc)
-    np.save(filename, ipc)
-    logging.info("Load Data Succeed...............")
-
+# def process_ipc(index_path, classes_num, filename):
+#     # load data
+#     logging.info("Load Data...............")
+#     ipc = [[] for _ in range(classes_num)]
+#     with h5py.File(index_path, "r") as f:
+#         for i in tqdm(range(len(f["target"]))):
+#             t_class = np.where(f["target"][i])[0]
+#             for t in t_class:
+#                 ipc[t].append(i)
+#     print(ipc)
+#     np.save(filename, ipc)
+#     logging.info("Load Data Succeed...............")
 
 def save_to_dict(s, o_={}):
     sp = s.split(": ")
     o_.update({sp[0]: float(sp[1])})
     return o_
```

### Comparing `audioldm2-0.0.2/audioldm2/clap/training/audioset_textmap.npy` & `audioldm2-0.0.3/audioldm2/clap/training/audioset_textmap.npy`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/clap/training/bpe_simple_vocab_16e6.txt.gz` & `audioldm2-0.0.3/audioldm2/clap/training/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/clap/training/data.py` & `audioldm2-0.0.3/audioldm2/clap/training/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 import logging
 import os
 import random
-import h5py
 from dataclasses import dataclass
 import numpy as np
 import pandas as pd
 import torch
 import torchvision.datasets as datasets
 from PIL import Image
 from torch.utils.data import Dataset, DataLoader, SubsetRandomSampler
@@ -61,161 +60,160 @@
     return (x / 32767.0).astype(np.float32)
 
 
 def float32_to_int16(x):
     x = np.clip(x, a_min=-1.0, a_max=1.0)
     return (x * 32767.0).astype(np.int16)
 
-
 # For Toy Dataset
-class ToyDataset(Dataset):
-    def __init__(self, index_path, ipc, config, eval_mode=False):
-        """Toy Dataset for testing the audioset input with text labels
-        Parameters
-        ----------
-            index_path: str
-                the link to the h5 file of each audio
-            idc: str
-                the link to the npy file, the number of samples in each class
-            config: dict
-                the audio cfg file
-           eval_model (bool): to indicate if the dataset is a testing dataset
-        """
-        self.audio_cfg = config["audio_cfg"]
-        self.text_cfg = config["text_cfg"]
-        self.fp = h5py.File(index_path, "r")
-        self.ipc = np.load(ipc, allow_pickle=True)
-        self.total_size = len(self.fp["audio_name"])
-        self.classes_num = self.audio_cfg["class_num"]
-        self.eval_mode = eval_mode
-
-        if not eval_mode:
-            self.generate_queue()
-        else:
-            self.queue = []
-            for i in range(self.total_size):
-                target = self.fp["target"][i]
-                if np.sum(target) > 0:
-                    self.queue.append(i)
-            self.total_size = len(self.queue)
-        logging.info("total dataset size: %d" % (self.total_size))
-        logging.info("class num: %d" % (self.classes_num))
-
-    def time_shifting(self, x):
-        frame_num = len(x)
-        shift_len = random.randint(0, frame_num - 1)
-        new_sample = np.concatenate([x[shift_len:], x[:shift_len]], axis=0)
-        return new_sample
-
-    def generate_queue(self):
-        self.queue = []
-        while len(self.queue) < self.total_size:
-            class_set = [*range(self.classes_num)]
-            random.shuffle(class_set)
-            self.queue += [
-                self.ipc[d][random.randint(0, len(self.ipc[d]) - 1)] for d in class_set
-            ]
-        self.queue = self.queue[: self.total_size]
-
-        logging.info("queue regenerated:%s" % (self.queue[-5:]))
-
-    def crop_wav(self, x):
-        crop_size = self.audio_cfg["crop_size"]
-        crop_pos = random.randint(0, len(x) - crop_size - 1)
-        return x[crop_pos : crop_pos + crop_size]
-
-    def prompt_text(self, target):
-        events = _AUDIOSET_MAP[np.where(target > 0)]
-        event_text = "The sounds of " + ", ".join(events[:-1]) + " and " + events[-1]
-        text = tokenize(event_text)[0]
-        return text
-
-    def __getitem__(self, index):
-        """Load waveform, text, and target of an audio clip
-
-        Parameters
-        ----------
-            index: int
-                the index number
-        Return
-        ------
-            output: dict {
-                "hdf5_path": str,
-                "index_in_hdf5": int,
-                "audio_name": str,
-                "waveform": list (audio_length,),
-                "target": list (class_num, ),
-                "text": torch.tensor (context_length,)
-            }
-                the output dictionary
-        """
-        s_index = self.queue[index]
-
-        audio_name = self.fp["audio_name"][s_index].decode()
-        # Hardcode here CHANGE
-        hdf5_path = (
-            self.fp["hdf5_path"][s_index]
-            .decode()
-            .replace(
-                "../workspace",
-                "/home/la/kechen/Research/ke_zsasp/workspace",
-            )
-        )
-        r_idx = self.fp["index_in_hdf5"][s_index]
-        target = self.fp["target"][s_index].astype(np.float32)
-        text = self.prompt_text(target)
-        with h5py.File(hdf5_path, "r") as f:
-            waveform = int16_to_float32(f["waveform"][r_idx])[
-                : self.audio_cfg["clip_samples"]
-            ]
-        assert (
-            len(waveform) == self.audio_cfg["clip_samples"]
-        ), "The sample length is not match"
-        # Time shift
-        # if (self.config.enable_time_shift) and (not self.eval_mode):
-        #     waveform = self.time_shifting(waveform)
-        # # Label Enhance
-        # if (self.config.crop_size is not None) and (not self.eval_mode):
-        #     waveform = self.crop_wav(waveform)
-        # # the label enhance rate is fixed 0.5
-        # if (self.config.enable_label_enhance) and (not self.eval_mode) and random.random() < 0.5:
-        #     kidx = np.where(target)[0]
-        #     for k in kidx:
-        #         for add_key in self.class_map[k][1]:
-        #             target[add_key] = 1.0
-        #         if len(self.class_map[k][2]) > 0:
-        #             add_key = random.choice(self.class_map[k][2])
-        #             target[add_key] = 1.0
-
-        # missing the text input
-        mel_spec = get_mel(torch.from_numpy(waveform), self.audio_cfg)[None, :, :]
-        mel_spec = (
-            torch.cat(
-                [mel_spec, mel_spec.clone(), mel_spec.clone(), mel_spec.clone()], dim=0
-            )
-            .cpu()
-            .numpy()
-        )
-        longer = random.choice([True, False])
-        if longer == False:
-            mel_spec[1:, :, :] = 0.0
-        data_dict = {
-            "hdf5_path": hdf5_path,
-            "index_in_hdf5": r_idx,
-            "audio_name": audio_name,
-            "waveform": waveform,
-            "class_label": target,
-            "text": text,
-            "longer": longer,
-            "mel_fusion": mel_spec,
-        }
-        return data_dict
+# class ToyDataset(Dataset):
+#     def __init__(self, index_path, ipc, config, eval_mode=False):
+#         """Toy Dataset for testing the audioset input with text labels
+#         Parameters
+#         ----------
+#             index_path: str
+#                 the link to the h5 file of each audio
+#             idc: str
+#                 the link to the npy file, the number of samples in each class
+#             config: dict
+#                 the audio cfg file
+#            eval_model (bool): to indicate if the dataset is a testing dataset
+#         """
+#         self.audio_cfg = config["audio_cfg"]
+#         self.text_cfg = config["text_cfg"]
+#         self.fp = h5py.File(index_path, "r")
+#         self.ipc = np.load(ipc, allow_pickle=True)
+#         self.total_size = len(self.fp["audio_name"])
+#         self.classes_num = self.audio_cfg["class_num"]
+#         self.eval_mode = eval_mode
+
+#         if not eval_mode:
+#             self.generate_queue()
+#         else:
+#             self.queue = []
+#             for i in range(self.total_size):
+#                 target = self.fp["target"][i]
+#                 if np.sum(target) > 0:
+#                     self.queue.append(i)
+#             self.total_size = len(self.queue)
+#         logging.info("total dataset size: %d" % (self.total_size))
+#         logging.info("class num: %d" % (self.classes_num))
+
+#     def time_shifting(self, x):
+#         frame_num = len(x)
+#         shift_len = random.randint(0, frame_num - 1)
+#         new_sample = np.concatenate([x[shift_len:], x[:shift_len]], axis=0)
+#         return new_sample
+
+#     def generate_queue(self):
+#         self.queue = []
+#         while len(self.queue) < self.total_size:
+#             class_set = [*range(self.classes_num)]
+#             random.shuffle(class_set)
+#             self.queue += [
+#                 self.ipc[d][random.randint(0, len(self.ipc[d]) - 1)] for d in class_set
+#             ]
+#         self.queue = self.queue[: self.total_size]
+
+#         logging.info("queue regenerated:%s" % (self.queue[-5:]))
+
+#     def crop_wav(self, x):
+#         crop_size = self.audio_cfg["crop_size"]
+#         crop_pos = random.randint(0, len(x) - crop_size - 1)
+#         return x[crop_pos : crop_pos + crop_size]
+
+#     def prompt_text(self, target):
+#         events = _AUDIOSET_MAP[np.where(target > 0)]
+#         event_text = "The sounds of " + ", ".join(events[:-1]) + " and " + events[-1]
+#         text = tokenize(event_text)[0]
+#         return text
+
+#     def __getitem__(self, index):
+#         """Load waveform, text, and target of an audio clip
+
+#         Parameters
+#         ----------
+#             index: int
+#                 the index number
+#         Return
+#         ------
+#             output: dict {
+#                 "hdf5_path": str,
+#                 "index_in_hdf5": int,
+#                 "audio_name": str,
+#                 "waveform": list (audio_length,),
+#                 "target": list (class_num, ),
+#                 "text": torch.tensor (context_length,)
+#             }
+#                 the output dictionary
+#         """
+#         s_index = self.queue[index]
+
+#         audio_name = self.fp["audio_name"][s_index].decode()
+#         # Hardcode here CHANGE
+#         hdf5_path = (
+#             self.fp["hdf5_path"][s_index]
+#             .decode()
+#             .replace(
+#                 "../workspace",
+#                 "/home/la/kechen/Research/ke_zsasp/workspace",
+#             )
+#         )
+#         r_idx = self.fp["index_in_hdf5"][s_index]
+#         target = self.fp["target"][s_index].astype(np.float32)
+#         text = self.prompt_text(target)
+#         with h5py.File(hdf5_path, "r") as f:
+#             waveform = int16_to_float32(f["waveform"][r_idx])[
+#                 : self.audio_cfg["clip_samples"]
+#             ]
+#         assert (
+#             len(waveform) == self.audio_cfg["clip_samples"]
+#         ), "The sample length is not match"
+#         # Time shift
+#         # if (self.config.enable_time_shift) and (not self.eval_mode):
+#         #     waveform = self.time_shifting(waveform)
+#         # # Label Enhance
+#         # if (self.config.crop_size is not None) and (not self.eval_mode):
+#         #     waveform = self.crop_wav(waveform)
+#         # # the label enhance rate is fixed 0.5
+#         # if (self.config.enable_label_enhance) and (not self.eval_mode) and random.random() < 0.5:
+#         #     kidx = np.where(target)[0]
+#         #     for k in kidx:
+#         #         for add_key in self.class_map[k][1]:
+#         #             target[add_key] = 1.0
+#         #         if len(self.class_map[k][2]) > 0:
+#         #             add_key = random.choice(self.class_map[k][2])
+#         #             target[add_key] = 1.0
+
+#         # missing the text input
+#         mel_spec = get_mel(torch.from_numpy(waveform), self.audio_cfg)[None, :, :]
+#         mel_spec = (
+#             torch.cat(
+#                 [mel_spec, mel_spec.clone(), mel_spec.clone(), mel_spec.clone()], dim=0
+#             )
+#             .cpu()
+#             .numpy()
+#         )
+#         longer = random.choice([True, False])
+#         if longer == False:
+#             mel_spec[1:, :, :] = 0.0
+#         data_dict = {
+#             "hdf5_path": hdf5_path,
+#             "index_in_hdf5": r_idx,
+#             "audio_name": audio_name,
+#             "waveform": waveform,
+#             "class_label": target,
+#             "text": text,
+#             "longer": longer,
+#             "mel_fusion": mel_spec,
+#         }
+#         return data_dict
 
-    def __len__(self):
-        return self.total_size
+#     def __len__(self):
+#         return self.total_size
 
 
 class CsvDataset(Dataset):
     def __init__(self, input_filename, transforms, img_key, caption_key, sep="\t"):
         logging.debug(f"Loading csv data from {input_filename}.")
         df = pd.read_csv(input_filename, sep=sep)
 
@@ -228,15 +226,14 @@
         return len(self.captions)
 
     def __getitem__(self, idx):
         images = self.transforms(Image.open(str(self.images[idx])))
         texts = tokenize([str(self.captions[idx])])[0]
         return images, texts
 
-
 @dataclass
 class DataInfo:
     dataloader: DataLoader
     sampler: DistributedSampler
 
 
 def preprocess_txt(text):
```

### Comparing `audioldm2-0.0.2/audioldm2/clap/training/params.py` & `audioldm2-0.0.3/audioldm2/clap/training/params.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/hifigan/models.py` & `audioldm2-0.0.3/audioldm2/hifigan/models.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/hifigan/models_v2.py` & `audioldm2-0.0.3/audioldm2/hifigan/models_v2.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/models/ddim.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/models/ddim.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/models/ddpm.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/models/ddpm.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/models/plms.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/models/plms.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/attention.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/modules/attention.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/AudioMAE.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/AudioMAE.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/models_mae.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/models_mae.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/models_vit.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/models_vit.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/crop.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/util/crop.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/datasets.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/util/datasets.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/lars.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/util/lars.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/lr_decay.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/util/lr_decay.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/lr_sched.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/util/lr_sched.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/misc.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/util/misc.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/patch_embed.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/util/patch_embed.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/pos_embed.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/util/pos_embed.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/audiomae/util/stat.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/modules/audiomae/util/stat.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/diffusionmodules/model.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/modules/diffusionmodules/model.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/diffusionmodules/openaimodel.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/modules/diffusionmodules/openaimodel.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/diffusionmodules/util.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/modules/diffusionmodules/util.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/distributions/distributions.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/modules/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/ema.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/modules/ema.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/encoders/modules.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/modules/encoders/modules.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/phoneme_encoder/attentions.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/modules/phoneme_encoder/attentions.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/phoneme_encoder/commons.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/modules/phoneme_encoder/commons.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/modules/phoneme_encoder/encoder.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/modules/phoneme_encoder/encoder.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_diffusion/util.py` & `audioldm2-0.0.3/audioldm2/latent_diffusion/util.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/latent_encoder/autoencoder.py` & `audioldm2-0.0.3/audioldm2/latent_encoder/autoencoder.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/pipeline.py` & `audioldm2-0.0.3/audioldm2/pipeline.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/utilities/audio/audio_processing.py` & `audioldm2-0.0.3/audioldm2/utilities/audio/audio_processing.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/utilities/audio/stft.py` & `audioldm2-0.0.3/audioldm2/utilities/audio/stft.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/utilities/audio/tools.py` & `audioldm2-0.0.3/audioldm2/utilities/audio/tools.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/utilities/data/add_on.py` & `audioldm2-0.0.3/audioldm2/utilities/data/add_on.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/utilities/data/dataset.py` & `audioldm2-0.0.3/audioldm2/utilities/data/dataset.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/utilities/model.py` & `audioldm2-0.0.3/audioldm2/utilities/model.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/utilities/sampler.py` & `audioldm2-0.0.3/audioldm2/utilities/sampler.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/utilities/tools.py` & `audioldm2-0.0.3/audioldm2/utilities/tools.py`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/audioldm2/utils.py` & `audioldm2-0.0.3/audioldm2/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,20 +105,81 @@
         elif config == "__is_unconditional__":
             return None
         raise KeyError("Expected key `target` to instantiate.")
     try:
         return get_obj_from_str(config["target"])(**config.get("params", dict()))
     except:
         import ipdb
-
         ipdb.set_trace()
 
-
 def default_audioldm_config(model_name="audioldm2-full"):
-    basic_config = {
+    basic_config = get_basic_config()
+    if("-large-" in model_name):
+        basic_config["model"]["params"]["unet_config"]["params"]["context_dim"] = [768, 1024, None]
+        basic_config["model"]["params"]["unet_config"]["params"]["transformer_depth"] = 2
+    return basic_config
+
+def get_metadata():
+    return {
+        "audioldm2-full": {
+            "path": os.path.join(
+                CACHE_DIR,
+                "audioldm2-full.pth",
+            ),
+            "url": "https://huggingface.co/haoheliu/audioldm2-full/resolve/main/audioldm2-full.pth",
+        },
+        "audioldm2-music-665k": {
+            "path": os.path.join(
+                CACHE_DIR,
+                "audioldm2-music-665k",
+            ), 
+            "url": "https://huggingface.co/haoheliu/audioldm2-music-665k/resolve/main/audioldm2-music-665k.pth", 
+        },
+        "audioldm2-full-large-650k": {
+            "path": os.path.join(
+                CACHE_DIR,
+                "audioldm2-full-large-650k.pth",
+            ),
+            "url": "https://huggingface.co/haoheliu/audioldm2-full-large-650k/resolve/main/audioldm2-full-large-650k.pth", 
+        },
+    }
+
+class MyProgressBar:
+    def __init__(self):
+        self.pbar = None
+
+    def __call__(self, block_num, block_size, total_size):
+        if not self.pbar:
+            self.pbar = progressbar.ProgressBar(maxval=total_size)
+            self.pbar.start()
+
+        downloaded = block_num * block_size
+        if downloaded < total_size:
+            self.pbar.update(downloaded)
+        else:
+            self.pbar.finish()
+
+
+def download_checkpoint(checkpoint_name="audioldm2-full"):
+    meta = get_metadata()
+    if checkpoint_name not in meta.keys():
+        print(
+            "The model name you provided is not supported. Please use one of the following: ",
+            meta.keys(),
+        )
+
+    model_id = "haoheliu/%s" % checkpoint_name
+    hf_hub_download(
+        repo_id=model_id,
+        filename=os.path.basename(meta[checkpoint_name]["path"]),
+        local_dir=os.path.dirname(meta[checkpoint_name]["path"]),
+    )
+
+def get_basic_config():
+    return {
         "metadata_root": "/mnt/bn/lqhaoheliu/metadata/processed/dataset_root.json",
         "log_directory": "./log/audiomae_pred",
         "precision": "high",
         "data": {
             "train": [
                 "audiocaps",
                 "audioset",
@@ -161,15 +222,15 @@
                 "max_wav_value": 32768,
                 "duration": 10.24,
             },
             "stft": {"filter_length": 1024, "hop_length": 160, "win_length": 1024},
             "mel": {"n_mel_channels": 64, "mel_fmin": 0, "mel_fmax": 8000},
         },
         "augmentation": {"mixup": 0},
-        "model": {
+        "model": { # 
             "target": "audioldm2.latent_diffusion.models.ddpm.LatentDiffusion",
             "params": {
                 "first_stage_config": {
                     "base_learning_rate": 0.000008,
                     "target": "audioldm2.latent_encoder.autoencoder.AutoencoderKL",
                     "params": {
                         "sampling_rate": 16000,
@@ -300,53 +361,8 @@
                         "cond_stage_key": "text",
                         "conditioning_key": "crossattn",
                         "target": "audioldm2.latent_diffusion.modules.encoders.modules.FlanT5HiddenState",
                     },
                 },
             },
         },
-    }
-    return basic_config
-
-
-def get_metadata():
-    return {
-        "audioldm2-full": {
-            "path": os.path.join(
-                CACHE_DIR,
-                "audioldm2-full.pth",
-            ),
-            "url": "https://huggingface.co/haoheliu/audioldm2-full/resolve/main/audioldm2-full.pth",
-        },
-    }
-
-
-class MyProgressBar:
-    def __init__(self):
-        self.pbar = None
-
-    def __call__(self, block_num, block_size, total_size):
-        if not self.pbar:
-            self.pbar = progressbar.ProgressBar(maxval=total_size)
-            self.pbar.start()
-
-        downloaded = block_num * block_size
-        if downloaded < total_size:
-            self.pbar.update(downloaded)
-        else:
-            self.pbar.finish()
-
-
-def download_checkpoint(checkpoint_name="audioldm2-full"):
-    meta = get_metadata()
-    if checkpoint_name not in meta.keys():
-        print(
-            "The model name you provided is not supported. Please use one of the following: ",
-            meta.keys(),
-        )
-
-    model_id = "haoheliu/%s" % checkpoint_name
-    hf_hub_download(
-        repo_id=model_id,
-        filename=os.path.basename(meta[checkpoint_name]["path"]),
-        local_dir=os.path.dirname(meta[checkpoint_name]["path"]),
-    )
+    }
```

### Comparing `audioldm2-0.0.2/audioldm2.egg-info/SOURCES.txt` & `audioldm2-0.0.3/audioldm2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audioldm2-0.0.2/bin/audioldm2` & `audioldm2-0.0.3/bin/audioldm2`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from audioldm2 import text_to_audio, build_model, save_wave, get_time, read_list
 import argparse
 
 os.environ["TOKENIZERS_PARALLELISM"] = "true"
 matplotlib_logger = logging.getLogger('matplotlib')
 matplotlib_logger.setLevel(logging.WARNING)
 
-
 CACHE_DIR = os.getenv(
     "AUDIOLDM_CACHE_DIR",
     os.path.join(os.path.expanduser("~"), ".cache/audioldm2"))
 
 parser = argparse.ArgumentParser()
 
 parser.add_argument(
@@ -123,9 +122,9 @@
         seed=random_seed,
         duration=duration,
         guidance_scale=guidance_scale,
         ddim_steps=args.ddim_steps,
         n_candidate_gen_per_text=n_candidate_gen_per_text,
         batchsize=args.batchsize,
     )
-        
+     
     save_wave(waveform, save_path, name=text)
```

### Comparing `audioldm2-0.0.2/setup.py` & `audioldm2-0.0.3/setup.py`

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
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "torch>=1.13.0",
     "torchaudio>=0.13.0",
     "torchvision>=0.14.0",
     "tqdm",
```

### Comparing `audioldm2-0.0.2/share_btn.py` & `audioldm2-0.0.3/share_btn.py`

 * *Files identical despite different names*

