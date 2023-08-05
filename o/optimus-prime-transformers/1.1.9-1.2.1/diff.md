# Comparing `tmp/optimus-prime-transformers-1.1.9.tar.gz` & `tmp/optimus-prime-transformers-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimus-prime-transformers-1.1.9.tar", last modified: Wed Jul 26 17:12:35 2023, max compression
+gzip compressed data, was "optimus-prime-transformers-1.2.1.tar", last modified: Sat Aug  5 05:34:36 2023, max compression
```

## Comparing `optimus-prime-transformers-1.1.9.tar` & `optimus-prime-transformers-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:12:35.699484 optimus-prime-transformers-1.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-26 17:12:24.000000 optimus-prime-transformers-1.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-26 17:12:35.699484 optimus-prime-transformers-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    63670 2023-07-26 17:12:24.000000 optimus-prime-transformers-1.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:12:35.699484 optimus-prime-transformers-1.1.9/optimus_prime/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-26 17:12:24.000000 optimus-prime-transformers-1.1.9/optimus_prime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-07-26 17:12:24.000000 optimus-prime-transformers-1.1.9/optimus_prime/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-26 17:12:24.000000 optimus-prime-transformers-1.1.9/optimus_prime/autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-26 17:12:24.000000 optimus-prime-transformers-1.1.9/optimus_prime/continuous_autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-07-26 17:12:24.000000 optimus-prime-transformers-1.1.9/optimus_prime/flash.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-07-26 17:12:24.000000 optimus-prime-transformers-1.1.9/optimus_prime/nonautoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    55945 2023-07-26 17:12:24.000000 optimus-prime-transformers-1.1.9/optimus_prime/x_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-07-26 17:12:24.000000 optimus-prime-transformers-1.1.9/optimus_prime/xl_autoregressive_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:12:35.699484 optimus-prime-transformers-1.1.9/optimus_prime_transformers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-26 17:12:35.000000 optimus-prime-transformers-1.1.9/optimus_prime_transformers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-26 17:12:35.000000 optimus-prime-transformers-1.1.9/optimus_prime_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 17:12:35.000000 optimus-prime-transformers-1.1.9/optimus_prime_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-26 17:12:35.000000 optimus-prime-transformers-1.1.9/optimus_prime_transformers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 17:12:35.000000 optimus-prime-transformers-1.1.9/optimus_prime_transformers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 17:12:35.699484 optimus-prime-transformers-1.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-26 17:12:24.000000 optimus-prime-transformers-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 05:34:36.283532 optimus-prime-transformers-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-05 05:34:26.000000 optimus-prime-transformers-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-05 05:34:36.283532 optimus-prime-transformers-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    63651 2023-08-05 05:34:26.000000 optimus-prime-transformers-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 05:34:36.283532 optimus-prime-transformers-1.2.1/optimus_prime/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-08-05 05:34:26.000000 optimus-prime-transformers-1.2.1/optimus_prime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-08-05 05:34:26.000000 optimus-prime-transformers-1.2.1/optimus_prime/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-08-05 05:34:26.000000 optimus-prime-transformers-1.2.1/optimus_prime/autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-08-05 05:34:26.000000 optimus-prime-transformers-1.2.1/optimus_prime/continuous_autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-08-05 05:34:26.000000 optimus-prime-transformers-1.2.1/optimus_prime/flash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-08-05 05:34:26.000000 optimus-prime-transformers-1.2.1/optimus_prime/nonautoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55813 2023-08-05 05:34:26.000000 optimus-prime-transformers-1.2.1/optimus_prime/x_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-08-05 05:34:26.000000 optimus-prime-transformers-1.2.1/optimus_prime/xl_autoregressive_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 05:34:36.283532 optimus-prime-transformers-1.2.1/optimus_prime_transformers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-05 05:34:36.000000 optimus-prime-transformers-1.2.1/optimus_prime_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-05 05:34:36.000000 optimus-prime-transformers-1.2.1/optimus_prime_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 05:34:36.000000 optimus-prime-transformers-1.2.1/optimus_prime_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-05 05:34:36.000000 optimus-prime-transformers-1.2.1/optimus_prime_transformers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-05 05:34:36.000000 optimus-prime-transformers-1.2.1/optimus_prime_transformers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 05:34:36.283532 optimus-prime-transformers-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-05 05:34:26.000000 optimus-prime-transformers-1.2.1/setup.py
```

### Comparing `optimus-prime-transformers-1.1.9/LICENSE` & `optimus-prime-transformers-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.9/PKG-INFO` & `optimus-prime-transformers-1.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimus-prime-transformers
-Version: 1.1.9
+Version: 1.2.1
 Summary: optimus-prime - Pytorch
 Home-page: https://github.com/kyegomez/Optimus-Prime
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `optimus-prime-transformers-1.1.9/README.md` & `optimus-prime-transformers-1.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![PyPI version](https://badge.fury.io/py/x-transformers.svg)](https://badge.fury.io/py/x-transformers)
 
 A concise but fully-featured transformer, complete with a set of promising e**x**perimental features from various papers.
 
 ## Install
 
 ```bash
-$ pip install optimus-prime-transformers
+$ pip install primus
 ```
 
 ## Usage
 
 Full encoder / decoder
 
 ```python
@@ -1877,8 +1877,8 @@
 *solve intelligence... then use that to solve everything else.* - Demis Hassabis
 
 
 
 ## Todo
 * Integrate flash attention 2.0 cuda and make it optional so if set to true it'll download then compile
 * Integrate dynamic sparse attention in triton
-* Integrate Parallelization and distributed setup of The Attention
+* Integrate Parallelization and distributed setup of The Attention
```

#### html2text {}

```diff
@@ -1,163 +1,162 @@
 ## optimus-prime [![PyPI version](https://badge.fury.io/py/x-transformers.svg)]
 (https://badge.fury.io/py/x-transformers) A concise but fully-featured
 transformer, complete with a set of promising e**x**perimental features from
-various papers. ## Install ```bash $ pip install optimus-prime-transformers ```
-## Usage Full encoder / decoder ```python import torch from optimus_prime
-import XTransformer model = XTransformer( dim = 512, enc_num_tokens = 256,
-enc_depth = 6, enc_heads = 8, enc_max_seq_len = 1024, dec_num_tokens = 256,
-dec_depth = 6, dec_heads = 8, dec_max_seq_len = 1024, tie_token_emb = True #
-tie embeddings of encoder and decoder ) src = torch.randint(0, 256, (1, 1024))
-src_mask = torch.ones_like(src).bool() tgt = torch.randint(0, 256, (1, 1024))
-loss = model(src, tgt, mask = src_mask) # (1, 1024, 512) loss.backward() ```
-Decoder-only (GPT-like) ```python import torch from optimus_prime import
-TransformerWrapper, Decoder model = TransformerWrapper( num_tokens = 20000,
-max_seq_len = 1024, attn_layers = Decoder( dim = 512, depth = 12, heads = 8 )
-).cuda() x = torch.randint(0, 256, (1, 1024)).cuda() model(x) # (1, 1024,
-20000) ``` GPT3 would be approximately the following (but you wouldn't be able
-to run it anyways) ```python gpt3 = TransformerWrapper( num_tokens = 50000,
-max_seq_len = 2048, attn_layers = Decoder( dim = 12288, depth = 96, heads = 96,
-attn_dim_head = 128 ) ).cuda() ``` Encoder-only (BERT-like) ```python import
-torch from optimus_prime import TransformerWrapper, Encoder model =
-TransformerWrapper( num_tokens = 20000, max_seq_len = 1024, attn_layers =
-Encoder( dim = 512, depth = 12, heads = 8 ) ).cuda() x = torch.randint(0, 256,
-(1, 1024)).cuda() mask = torch.ones_like(x).bool() model(x, mask = mask) # (1,
-1024, 20000) ``` State of the art image classification ```python import torch
-from optimus_prime import ViTransformerWrapper, Encoder model =
-ViTransformerWrapper( image_size = 256, patch_size = 32, num_classes = 1000,
-attn_layers = Encoder( dim = 512, depth = 6, heads = 8, ) ) img = torch.randn
-(1, 3, 256, 256) model(img) # (1, 1000) ``` Image -> caption ```python import
-torch from optimus_prime import ViTransformerWrapper, TransformerWrapper,
-Encoder, Decoder encoder = ViTransformerWrapper( image_size = 256, patch_size =
-32, attn_layers = Encoder( dim = 512, depth = 6, heads = 8 ) ) decoder =
-TransformerWrapper( num_tokens = 20000, max_seq_len = 1024, attn_layers =
-Decoder( dim = 512, depth = 6, heads = 8, cross_attend = True ) ) img =
-torch.randn(1, 3, 256, 256) caption = torch.randint(0, 20000, (1, 1024))
-encoded = encoder(img, return_embeddings = True) decoder(caption, context =
-encoded) # (1, 1024, 20000) ``` PaLI, state of the art language-vision model
-```python import torch from optimus_prime import ViTransformerWrapper,
-XTransformer, Encoder # PaLI composes of # 1. vision transformer
-(ViTransformerWrapper) + # 2. encoder-decoder transformer (XTransformer) vit =
+various papers. ## Install ```bash $ pip install primus ``` ## Usage Full
+encoder / decoder ```python import torch from optimus_prime import XTransformer
+model = XTransformer( dim = 512, enc_num_tokens = 256, enc_depth = 6, enc_heads
+= 8, enc_max_seq_len = 1024, dec_num_tokens = 256, dec_depth = 6, dec_heads =
+8, dec_max_seq_len = 1024, tie_token_emb = True # tie embeddings of encoder and
+decoder ) src = torch.randint(0, 256, (1, 1024)) src_mask = torch.ones_like
+(src).bool() tgt = torch.randint(0, 256, (1, 1024)) loss = model(src, tgt, mask
+= src_mask) # (1, 1024, 512) loss.backward() ``` Decoder-only (GPT-like)
+```python import torch from optimus_prime import TransformerWrapper, Decoder
+model = TransformerWrapper( num_tokens = 20000, max_seq_len = 1024, attn_layers
+= Decoder( dim = 512, depth = 12, heads = 8 ) ).cuda() x = torch.randint(0,
+256, (1, 1024)).cuda() model(x) # (1, 1024, 20000) ``` GPT3 would be
+approximately the following (but you wouldn't be able to run it anyways)
+```python gpt3 = TransformerWrapper( num_tokens = 50000, max_seq_len = 2048,
+attn_layers = Decoder( dim = 12288, depth = 96, heads = 96, attn_dim_head = 128
+) ).cuda() ``` Encoder-only (BERT-like) ```python import torch from
+optimus_prime import TransformerWrapper, Encoder model = TransformerWrapper
+( num_tokens = 20000, max_seq_len = 1024, attn_layers = Encoder( dim = 512,
+depth = 12, heads = 8 ) ).cuda() x = torch.randint(0, 256, (1, 1024)).cuda()
+mask = torch.ones_like(x).bool() model(x, mask = mask) # (1, 1024, 20000) ```
+State of the art image classification ```python import torch from optimus_prime
+import ViTransformerWrapper, Encoder model = ViTransformerWrapper( image_size =
+256, patch_size = 32, num_classes = 1000, attn_layers = Encoder( dim = 512,
+depth = 6, heads = 8, ) ) img = torch.randn(1, 3, 256, 256) model(img) # (1,
+1000) ``` Image -> caption ```python import torch from optimus_prime import
+ViTransformerWrapper, TransformerWrapper, Encoder, Decoder encoder =
 ViTransformerWrapper( image_size = 256, patch_size = 32, attn_layers = Encoder
-( dim = 512, depth = 6, heads = 8 ) ) pali = XTransformer( dim = 512,
-enc_num_tokens = 256, enc_depth = 6, enc_heads = 8, enc_max_seq_len = 1024,
-dec_num_tokens = 256, dec_depth = 6, dec_heads = 8, dec_max_seq_len = 1024 ) #
-training data img = torch.randn(1, 3, 256, 256) # images prompt = torch.randint
-(0, 256, (1, 1024)) # prompt prompt_mask = torch.ones(1, 1024).bool() # prompt
-text mask output_text = torch.randint(0, 256, (1, 1024)) # target output text #
-train img_embeds = vit( img, return_embeddings = True ) loss = pali( prompt,
-output_text, mask = prompt_mask, src_prepend_embeds = img_embeds # will
-preprend image embeddings to encoder text embeddings before attention )
-loss.backward() # do the above for many steps on a 17B parameter model #
-attention is all you need ``` ## Dropouts ```python import torch from
-optimus_prime import TransformerWrapper, Decoder, Encoder model =
-TransformerWrapper( num_tokens = 20000, max_seq_len = 1024, emb_dropout = 0.1,
-# dropout after embedding attn_layers = Decoder( dim = 512, depth = 6, heads =
-8, layer_dropout = 0.1, # stochastic depth - dropout entire layer attn_dropout
-= 0.1, # dropout post-attention ff_dropout = 0.1 # feedforward dropout ) ) x =
-torch.randint(0, 20000, (1, 1024)) model(x) ``` ## Features ### Flash Attention
-[./images/flash-attention.png] What originally started off as a_short_paper
-from Markus Rabe culminated as a practical fused attention CUDA kernel, named
-Flash_Attention by Tri_Dao. The technique processes the attention matrix in
-tiles, only keeping track of the running softmax and exponentiated weighted
-sums. By recomputing on the backwards pass in a tiled fashion, one is able to
-keep the memory linear with respect to sequence length. This allows a lot of
-recent models to be able to reach for longer context lengths without worrying
-about the memory bottleneck. Other engineering decisions made by Tri Dao led to
-its enormous success, namely minimizing HBM accesses so that both the forwards
-and backwards outperform naive attention. In other words, flash attention is
-not only more memory efficient, but faster as well, making it a necessity for
-training transformers. MetaAI has recently added the ability to use Tri_Dao's
-CUDA_kernel through the scaled_dot_product_attention function in Pytorch 2.0.
-(They also have a `mem_efficient` attention, which is identical to flash
-attention design, just that the tiles are traversed differently) Llama was
-trained using Flash Attention. The only reason to avoid it is if you require
-operating on the attention matrix (dynamic positional bias, talking heads,
-residual attention). You can use it in this repository by setting `attn_flash`
-to `True` and enjoy the immediate memory savings and increase in speed. ex.
+( dim = 512, depth = 6, heads = 8 ) ) decoder = TransformerWrapper( num_tokens
+= 20000, max_seq_len = 1024, attn_layers = Decoder( dim = 512, depth = 6, heads
+= 8, cross_attend = True ) ) img = torch.randn(1, 3, 256, 256) caption =
+torch.randint(0, 20000, (1, 1024)) encoded = encoder(img, return_embeddings =
+True) decoder(caption, context = encoded) # (1, 1024, 20000) ``` PaLI, state of
+the art language-vision model ```python import torch from optimus_prime import
+ViTransformerWrapper, XTransformer, Encoder # PaLI composes of # 1. vision
+transformer (ViTransformerWrapper) + # 2. encoder-decoder transformer
+(XTransformer) vit = ViTransformerWrapper( image_size = 256, patch_size = 32,
+attn_layers = Encoder( dim = 512, depth = 6, heads = 8 ) ) pali = XTransformer
+( dim = 512, enc_num_tokens = 256, enc_depth = 6, enc_heads = 8,
+enc_max_seq_len = 1024, dec_num_tokens = 256, dec_depth = 6, dec_heads = 8,
+dec_max_seq_len = 1024 ) # training data img = torch.randn(1, 3, 256, 256) #
+images prompt = torch.randint(0, 256, (1, 1024)) # prompt prompt_mask =
+torch.ones(1, 1024).bool() # prompt text mask output_text = torch.randint(0,
+256, (1, 1024)) # target output text # train img_embeds = vit( img,
+return_embeddings = True ) loss = pali( prompt, output_text, mask =
+prompt_mask, src_prepend_embeds = img_embeds # will preprend image embeddings
+to encoder text embeddings before attention ) loss.backward() # do the above
+for many steps on a 17B parameter model # attention is all you need ``` ##
+Dropouts ```python import torch from optimus_prime import TransformerWrapper,
+Decoder, Encoder model = TransformerWrapper( num_tokens = 20000, max_seq_len =
+1024, emb_dropout = 0.1, # dropout after embedding attn_layers = Decoder( dim =
+512, depth = 6, heads = 8, layer_dropout = 0.1, # stochastic depth - dropout
+entire layer attn_dropout = 0.1, # dropout post-attention ff_dropout = 0.1 #
+feedforward dropout ) ) x = torch.randint(0, 20000, (1, 1024)) model(x) ``` ##
+Features ### Flash Attention [./images/flash-attention.png] What originally
+started off as a_short_paper from Markus Rabe culminated as a practical fused
+attention CUDA kernel, named Flash_Attention by Tri_Dao. The technique
+processes the attention matrix in tiles, only keeping track of the running
+softmax and exponentiated weighted sums. By recomputing on the backwards pass
+in a tiled fashion, one is able to keep the memory linear with respect to
+sequence length. This allows a lot of recent models to be able to reach for
+longer context lengths without worrying about the memory bottleneck. Other
+engineering decisions made by Tri Dao led to its enormous success, namely
+minimizing HBM accesses so that both the forwards and backwards outperform
+naive attention. In other words, flash attention is not only more memory
+efficient, but faster as well, making it a necessity for training transformers.
+MetaAI has recently added the ability to use Tri_Dao's_CUDA_kernel through the
+scaled_dot_product_attention function in Pytorch 2.0. (They also have a
+`mem_efficient` attention, which is identical to flash attention design, just
+that the tiles are traversed differently) Llama was trained using Flash
+Attention. The only reason to avoid it is if you require operating on the
+attention matrix (dynamic positional bias, talking heads, residual attention).
+You can use it in this repository by setting `attn_flash` to `True` and enjoy
+the immediate memory savings and increase in speed. ex. ```python import torch
+from optimus_prime import TransformerWrapper, Decoder, Encoder model =
+TransformerWrapper( num_tokens = 20000, max_seq_len = 1024, attn_layers =
+Decoder( dim = 512, depth = 6, heads = 8, attn_flash = True # just set this to
+True if you have pytorch 2.0 installed ) ) ``` ### Augmenting Self-attention
+with Persistent Memory [./images/all-attention.png] https://arxiv.org/abs/
+1907.01470 Proposes adding learned memory key / values prior to attention. They
+were able to remove feedforwards altogether and attain similar performance to
+the original transformers. I have found that keeping the feedforwards and
+adding the memory key / values leads to even better performance. ```python from
+optimus_prime import Decoder, Encoder enc = Encoder( dim = 512, depth = 6,
+heads = 8, attn_num_mem_kv = 16 # 16 memory key / values ) ``` ### Memory
+Transformers [./images/memory-transformer.png] https://arxiv.org/abs/2006.11527
+Proposes adding learned tokens, akin to CLS tokens, named memory tokens, that
+is passed through the attention layers alongside the input tokens. ```python
+import torch from optimus_prime import TransformerWrapper, Decoder, Encoder
+model = TransformerWrapper( num_tokens = 20000, max_seq_len = 1024,
+num_memory_tokens = 20, # 20 memory tokens attn_layers = Encoder( dim = 512,
+depth = 6, heads = 8 ) ) ``` ### Transformers Without Tears [./images/
+scalenorm.png] https://arxiv.org/abs/1910.05895 They experiment with
+alternatives to Layer normalization and found one that is both effective and
+simpler. Researchers have shared with me this leads to faster convergence.
 ```python import torch from optimus_prime import TransformerWrapper, Decoder,
 Encoder model = TransformerWrapper( num_tokens = 20000, max_seq_len = 1024,
-attn_layers = Decoder( dim = 512, depth = 6, heads = 8, attn_flash = True #
-just set this to True if you have pytorch 2.0 installed ) ) ``` ### Augmenting
-Self-attention with Persistent Memory [./images/all-attention.png] https://
-arxiv.org/abs/1907.01470 Proposes adding learned memory key / values prior to
-attention. They were able to remove feedforwards altogether and attain similar
-performance to the original transformers. I have found that keeping the
-feedforwards and adding the memory key / values leads to even better
-performance. ```python from optimus_prime import Decoder, Encoder enc = Encoder
-( dim = 512, depth = 6, heads = 8, attn_num_mem_kv = 16 # 16 memory key /
-values ) ``` ### Memory Transformers [./images/memory-transformer.png] https://
-arxiv.org/abs/2006.11527 Proposes adding learned tokens, akin to CLS tokens,
-named memory tokens, that is passed through the attention layers alongside the
-input tokens. ```python import torch from optimus_prime import
-TransformerWrapper, Decoder, Encoder model = TransformerWrapper( num_tokens =
-20000, max_seq_len = 1024, num_memory_tokens = 20, # 20 memory tokens
-attn_layers = Encoder( dim = 512, depth = 6, heads = 8 ) ) ``` ### Transformers
-Without Tears [./images/scalenorm.png] https://arxiv.org/abs/1910.05895 They
-experiment with alternatives to Layer normalization and found one that is both
-effective and simpler. Researchers have shared with me this leads to faster
-convergence. ```python import torch from optimus_prime import
+attn_layers = Decoder( dim = 512, depth = 6, heads = 8, use_scalenorm = True #
+set to True to use for all layers ) ) ``` You can also use the l2 normalized
+embeddings proposed as part of `fixnorm`. I have found it leads to improved
+convergence, when paired with small initialization (proposed by BlinkDL). The
+small initialization will be taken care of as long as `l2norm_embed` is set to
+`True` ```python import torch from optimus_prime import TransformerWrapper,
+Decoder, Encoder model = TransformerWrapper( num_tokens = 20000, max_seq_len =
+1024, l2norm_embed = True, # set this to True for l2 normalized embedding +
+small init attn_layers = Decoder( dim = 512, depth = 6, heads = 8 ) ) ``` Along
+the same lines of l2 normalized embeddings, Huggingface's 175B_parameter_BLOOM
+also places a layernorm right after the embeddings and just before the tokens
+enter the attention layers. This was corroborated by Yandex's 100B_parameter
+YaLM to stabilize training. It is recommended you either have either
+`l2norm_embed` or `post_emb_norm` set to `True` but not both, as they probably
+serve the same purpose. ```python import torch from optimus_prime import
 TransformerWrapper, Decoder, Encoder model = TransformerWrapper( num_tokens =
-20000, max_seq_len = 1024, attn_layers = Decoder( dim = 512, depth = 6, heads =
-8, use_scalenorm = True # set to True to use for all layers ) ) ``` You can
-also use the l2 normalized embeddings proposed as part of `fixnorm`. I have
-found it leads to improved convergence, when paired with small initialization
-(proposed by BlinkDL). The small initialization will be taken care of as long
-as `l2norm_embed` is set to `True` ```python import torch from optimus_prime
-import TransformerWrapper, Decoder, Encoder model = TransformerWrapper
-( num_tokens = 20000, max_seq_len = 1024, l2norm_embed = True, # set this to
-True for l2 normalized embedding + small init attn_layers = Decoder( dim = 512,
-depth = 6, heads = 8 ) ) ``` Along the same lines of l2 normalized embeddings,
-Huggingface's 175B_parameter_BLOOM also places a layernorm right after the
-embeddings and just before the tokens enter the attention layers. This was
-corroborated by Yandex's 100B_parameter_YaLM to stabilize training. It is
-recommended you either have either `l2norm_embed` or `post_emb_norm` set to
-`True` but not both, as they probably serve the same purpose. ```python import
-torch from optimus_prime import TransformerWrapper, Decoder, Encoder model =
-TransformerWrapper( num_tokens = 20000, max_seq_len = 1024, post_emb_norm =
-True, # set this to True to layernorm summed token + pos embeddings attn_layers
-= Decoder( dim = 512, depth = 6, heads = 8 ) ) ``` ### Root Mean Square Layer
-Normalization https://arxiv.org/abs/1910.07467 The authors propose to replace
-layer normalization with a simpler alternative, without mean centering and the
-learned bias. An investigative paper found this to be the best_performing
-normalization_variant. It was also used in Deepmind's latest large language
-models, Retro and Gopher. ```python import torch from optimus_prime import
+20000, max_seq_len = 1024, post_emb_norm = True, # set this to True to
+layernorm summed token + pos embeddings attn_layers = Decoder( dim = 512, depth
+= 6, heads = 8 ) ) ``` ### Root Mean Square Layer Normalization https://
+arxiv.org/abs/1910.07467 The authors propose to replace layer normalization
+with a simpler alternative, without mean centering and the learned bias. An
+investigative paper found this to be the best_performing_normalization_variant.
+It was also used in Deepmind's latest large language models, Retro and Gopher.
+```python import torch from optimus_prime import TransformerWrapper, Decoder,
+Encoder model = TransformerWrapper( num_tokens = 20000, max_seq_len = 1024,
+attn_layers = Decoder( dim = 512, depth = 6, heads = 8, use_rmsnorm = True #
+set to true to use for all layers ) ) ``` ### GLU Variants Improve Transformer
+[./images/ffglu.png] https://arxiv.org/abs/2002.05202 Noam Shazeer paper that
+explores gating in the feedforward, finding that simple gating with GELU leads
+to significant improvements. This variant also showed up in the latest mT5
+architecture. You should always turn this on (I may eventually turn it on by
+default). ```python import torch from optimus_prime import TransformerWrapper,
+Decoder, Encoder model = TransformerWrapper( num_tokens = 20000, max_seq_len =
+1024, attn_layers = Decoder( dim = 512, depth = 6, heads = 8, ff_glu = True #
+set to true to use for all feedforwards ) ) ``` The PaLM language model also
+chose to use the Swish GLU variant. You can turn this on by setting two flags
+```python import torch from optimus_prime import TransformerWrapper, Decoder,
+Encoder model = TransformerWrapper( num_tokens = 20000, max_seq_len = 1024,
+attn_layers = Decoder( dim = 512, depth = 6, heads = 8, ff_swish = True, # set
+this to True ff_glu = True # set to true to use for all feedforwards ) ) ``````
+### No Bias in Feedforward Starting with PaLM, there begun a trend to remove
+biases from the transformer all together. Boris_Dayma has run a number of
+experiments that showed removing biases from feedforwards led to increased
+throughput without any loss of accuracy. This was corroborated by yet_another
+paper investigating transformer architecture variants. You can turn off the
+feedforward bias as follows ```python import torch from optimus_prime import
 TransformerWrapper, Decoder, Encoder model = TransformerWrapper( num_tokens =
 20000, max_seq_len = 1024, attn_layers = Decoder( dim = 512, depth = 6, heads =
-8, use_rmsnorm = True # set to true to use for all layers ) ) ``` ### GLU
-Variants Improve Transformer [./images/ffglu.png] https://arxiv.org/abs/
-2002.05202 Noam Shazeer paper that explores gating in the feedforward, finding
-that simple gating with GELU leads to significant improvements. This variant
-also showed up in the latest mT5 architecture. You should always turn this on
-(I may eventually turn it on by default). ```python import torch from
-optimus_prime import TransformerWrapper, Decoder, Encoder model =
-TransformerWrapper( num_tokens = 20000, max_seq_len = 1024, attn_layers =
-Decoder( dim = 512, depth = 6, heads = 8, ff_glu = True # set to true to use
-for all feedforwards ) ) ``` The PaLM language model also chose to use the
-Swish GLU variant. You can turn this on by setting two flags ```python import
+8, ff_no_bias = True # set this to True ) ) ``` ### ReLUÂ² https://arxiv.org/
+abs/2109.08668 This paper used neural architecture search and found an
+activation, Relu Squared, that is both simpler and performs better than GELU,
+in the autoregressive language model setting. I have confirmed this in my
+independent experiments. However, if one were using the GLU variant from above,
+GELU still performs better. Pending further corroboration. ```python import
 torch from optimus_prime import TransformerWrapper, Decoder, Encoder model =
 TransformerWrapper( num_tokens = 20000, max_seq_len = 1024, attn_layers =
-Decoder( dim = 512, depth = 6, heads = 8, ff_swish = True, # set this to True
-ff_glu = True # set to true to use for all feedforwards ) ) `````` ### No Bias
-in Feedforward Starting with PaLM, there begun a trend to remove biases from
-the transformer all together. Boris_Dayma has run a number of experiments that
-showed removing biases from feedforwards led to increased throughput without
-any loss of accuracy. This was corroborated by yet_another_paper investigating
-transformer architecture variants. You can turn off the feedforward bias as
-follows ```python import torch from optimus_prime import TransformerWrapper,
-Decoder, Encoder model = TransformerWrapper( num_tokens = 20000, max_seq_len =
-1024, attn_layers = Decoder( dim = 512, depth = 6, heads = 8, ff_no_bias = True
-# set this to True ) ) ``` ### ReLUÂ² https://arxiv.org/abs/2109.08668 This
-paper used neural architecture search and found an activation, Relu Squared,
-that is both simpler and performs better than GELU, in the autoregressive
-language model setting. I have confirmed this in my independent experiments.
-However, if one were using the GLU variant from above, GELU still performs
-better. Pending further corroboration. ```python import torch from
-optimus_prime import TransformerWrapper, Decoder, Encoder model =
-TransformerWrapper( num_tokens = 20000, max_seq_len = 1024, attn_layers =
 Decoder( dim = 512, depth = 6, heads = 8, ff_relu_squared = True ) ) ``` ###
 Explicit Sparse Transformer: Concentrated Attention Through Explicit Selection
 [./images/topk-attention.png] https://arxiv.org/abs/1912.11637 This paper
 proposes an efficient way to sparsify attention by zeroing all dot-product
 query/key values not within the top k values. The show that this cheap method
 was as effective as other more expensive operations like sparsemax or entmax15.
 This technique comes with the cost of an extra hyperparameter (the top k values
```

### Comparing `optimus-prime-transformers-1.1.9/optimus_prime/__init__.py` & `optimus-prime-transformers-1.2.1/optimus_prime/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import torch
 from packaging import version
 
 if version.parse(torch.__version__) >= version.parse('2.0.0'):
     from einops._torch_specific import allow_ops_in_compiled_graph
     allow_ops_in_compiled_graph()
 
-from optimus_prime.x_transformers import XTransformer, Encoder, Decoder, CrossAttender, Attention, AttentionLayers, TransformerWrapper, ViTransformerWrapper, ContinuousTransformerWrapper
-from optimus_prime.x_transformers import AndromedaEmbedding #, AndromedaBnBEmbedding
 
-# d
-from optimus_prime.autoregressive_wrapper import AutoregressiveWrapper
-from optimus_prime.nonautoregressive_wrapper import NonAutoregressiveWrapper
-from optimus_prime.continuous_autoregressive_wrapper import ContinuousAutoregressiveWrapper
-from optimus_prime.xl_autoregressive_wrapper import XLAutoregressiveWrapper
+from x_transformers.x_transformers import XTransformer, Encoder, Decoder, CrossAttender, Attention, TransformerWrapper, ViTransformerWrapper, ContinuousTransformerWrapper
+
+from x_transformers.autoregressive_wrapper import AutoregressiveWrapper
+from x_transformers.nonautoregressive_wrapper import NonAutoregressiveWrapper
+from x_transformers.continuous_autoregressive_wrapper import ContinuousAutoregressiveWrapper
+from x_transformers.xl_autoregressive_wrapper import XLAutoregressiveWrapper
```

### Comparing `optimus-prime-transformers-1.1.9/optimus_prime/attend.py` & `optimus-prime-transformers-1.2.1/optimus_prime/attend.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,19 +6,17 @@
 
 from collections import namedtuple
 from functools import wraps
 from packaging import version
 from dataclasses import dataclass
 
 from einops import rearrange
-
-# from flash import FlashAttention
+from optimus_prime.flash import FlashAttention
 
 # constants
-
 EfficientAttentionConfig = namedtuple('EfficientAttentionConfig', ['enable_flash', 'enable_math', 'enable_mem_efficient'])
 
 @dataclass
 class Intermediates:
     qk_similarities: Tensor = None
     pre_softmax_attn: Tensor = None
     post_softmax_attn: Tensor = None
@@ -46,22 +44,29 @@
 
 # main class
 
 class Attend(nn.Module):
     def __init__(
         self,
         *,
+        dim,
+        dim_head,
+        q_bucket_size,
+        k_bucket_size,
+        parallel,
+        mixed_precision,
         dropout = 0.,
         causal = False,
         heads = None,
         talking_heads = False,
         scale = None,
         qk_norm = False,
         add_zero_kv=False,
         flash = False,
+        Flash2 = False
     ):
         super().__init__()
         self.scale = scale
         self.qk_norm = qk_norm
         self.causal = causal
         self.attn_fn = partial(F.softmax, dtype = torch.float32) if not qk_norm else F.softmax
 
@@ -75,14 +80,28 @@
         assert not (flash and talking_heads), 'talking heads not compatible with flash attention'
 
         self.talking_heads = talking_heads
         if talking_heads:
             self.pre_softmax_talking_heads = nn.Conv2d(heads, heads, 1, bias = False)
             self.post_softmax_talking_heads = nn.Conv2d(heads, heads, 1, bias = False)
 
+        self.Flash2 = Flash2
+        if Flash2:
+            self.flash_attention = FlashAttention(
+                dim = dim,
+                heads = heads,
+                dim_head = dim_head,
+                causal = causal,
+                q_bucket_size = q_bucket_size,
+                k_bucket_size = k_bucket_size,
+                parallel = parallel,
+                mixed_precision = mixed_precision
+            )
+
+
         # flash attention
 
         self.flash = flash
         assert not (flash and version.parse(torch.__version__) < version.parse('2.0.0')), 'in order to use flash attention, you must be using pytorch 2.0 or above'
 
         # determine efficient attention configs for cuda and cpu
 
@@ -207,14 +226,22 @@
             if exists(attn_bias):
                 attn_bias = F.pad(attn_bias, (1, 0), value=0.)
 
         if self.flash:
             assert not exists(prev_attn), 'residual attention not compatible with flash attention'
             return self.flash_attn(q, k, v, mask = mask, attn_bias = attn_bias)
             # return FlashAttention(q, k, v, mask=mask, attn_bias=attn_bias )
+        
+        if self.Flash2:
+            #reshape q, k, v before passing into flash attention
+            batch_size, sequence_length, dim=q.shape
+            q = q.view(batch_size, self.heads, sequence_length, self.dim_head)
+            k = k.view(batch_size, self.heads, sequence_length, self.dim_head)
+            v = v.view(batch_size, self.heads, self.dim_head)
+            return self.flash_attention(q, k, v)
 
         kv_einsum_eq = 'b j d' if k.ndim == 3 else 'b h j d'
 
         dots = einsum(f'b h i d, {kv_einsum_eq} -> b h i j', q, k) * scale
 
         if exists(prev_attn):
             dots = dots + prev_attn
```

### Comparing `optimus-prime-transformers-1.1.9/optimus_prime/autoregressive_wrapper.py` & `optimus-prime-transformers-1.2.1/optimus_prime/autoregressive_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,16 +79,14 @@
         temperature = 1.,
         filter_logits_fn = top_k,
         filter_thres = 0.9,
         min_p_pow = 2.0,
         min_p_ratio = 0.02,
         **kwargs
     ):
-        device = start_tokens.device
-        num_dims = start_tokens.ndim
 
         start_tokens, ps = pack([start_tokens], '* n')
 
         b, t = start_tokens.shape
 
         out = start_tokens
```

### Comparing `optimus-prime-transformers-1.1.9/optimus_prime/continuous_autoregressive_wrapper.py` & `optimus-prime-transformers-1.2.1/optimus_prime/continuous_autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.9/optimus_prime/flash.py` & `optimus-prime-transformers-1.2.1/optimus_prime/flash.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import math
 import torch
-from functools import partial
 from torch import nn, einsum
 from torch.autograd.function import Function
 
 from einops import rearrange
 
-from torch.jit import fork, wait
 
 from torch.cuda.amp import autocast, GradScaler
 from torch.nn import DataParallel
 # constants
 
 EPSILON = 1e-10
 
@@ -233,14 +231,17 @@
     ):
         q_bucket_size = default(q_bucket_size, self.q_bucket_size)
         k_bucket_size = default(k_bucket_size, self.k_bucket_size)
 
         h = self.heads
         context = default(context, x)
 
+        # batch_size = x.shape[0]
+        # x = x.view(batch_size, -1)
+
         q = self.to_q(x)
         k, v = self.to_kv(context).chunk(2, dim=-1)
 
         q, k, v = map(lambda t: rearrange(t, 'b n (h d) -> b h n d', h=h), (q, k, v))
 
         if self.parallel:
             # Split the input data into chunks and move each chunk to the correct GPU
```

### Comparing `optimus-prime-transformers-1.1.9/optimus_prime/nonautoregressive_wrapper.py` & `optimus-prime-transformers-1.2.1/optimus_prime/nonautoregressive_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from contextlib import nullcontext
 from collections import namedtuple
 
 import torch
 import torch.nn.functional as F
 from torch import nn
 
-from einops import rearrange, repeat, pack, unpack
+from einops import rearrange
 
 
 from optimus_prime.x_transformers import TransformerWrapper
 from typing import Optional
 
 # constants
 
@@ -215,15 +215,15 @@
 
             if exists(filter_thres):
                 logits = top_k(logits, filter_thres)
 
             annealing_scale = steps_until_x0 / self.steps
             temperature = start_temperature * annealing_scale
 
-            probs = (logits / max(temperature, 1e-3)).softmax(dim = -1)
+            (logits / max(temperature, 1e-3)).softmax(dim = -1)
 
             sampled_ids = gumbel_sample(logits, temperature = max(temperature, 1e-3))
 
             seq = torch.where(mask, sampled_ids, seq)
 
             if exists(self.token_critic):
                 scores = self.token_critic(seq)
```

### Comparing `optimus-prime-transformers-1.1.9/optimus_prime/x_transformers.py` & `optimus-prime-transformers-1.2.1/optimus_prime/x_transformers.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,18 @@
 
 import torch
 from torch import nn, einsum, Tensor
 import torch.nn.functional as F
 
 from functools import partial, wraps
 from inspect import isfunction
-from collections import namedtuple
 from dataclasses import dataclass
 from typing import List
 
-from einops import rearrange, repeat, reduce
-from einops.layers.torch import Rearrange
+from einops import rearrange, repeat
 
 from optimus_prime.attend import Attend, Intermediates
 from optimus_prime.autoregressive_wrapper import AutoregressiveWrapper
 
 from abc import ABC, abstractmethod
 # import bitsandbytes as bnb
 
@@ -501,15 +499,16 @@
     def __init__(self, value, fn):
         super().__init__()
         self.value = value
         self.fn = fn
 
     def forward(self, x, **kwargs):
         out = self.fn(x, **kwargs)
-        scale_fn = lambda t: t * self.value
+        def scale_fn(t):
+            return t * self.value
 
         if not isinstance(out, tuple):
             return scale_fn(out)
 
         return (scale_fn(out[0]), *out[1:])
 
 class ScaleNorm(nn.Module):
@@ -800,15 +799,14 @@
 
         if not self.one_kv_head:
             k, v, r = map(lambda t: maybe(rearrange)(t, 'b n (h d) -> b h n d', h = h), (k, v, r))
 
         if self.qk_norm:
             qk_l2norm = partial(l2norm, groups = self.qk_norm_groups)
             q, k = map(qk_l2norm, (q, k))
-            scale = self.qk_norm_scale
 
             q = q * self.qk_norm_q_scale
             k = k * self.qk_norm_k_scale
 
         if exists(rotary_pos_emb) and not has_context:
             freqs, xpos_scale = rotary_pos_emb
             l = freqs.shape[-1]
@@ -835,15 +833,15 @@
                 input_mask = pad_at_dim(input_mask, (self.num_mem_kv, 0), dim = -1, value = True)
 
 
         i, j = map(lambda t: t.shape[-2], (q, k))
 
         # determine masking
 
-        mask_value = max_neg_value(q)
+        max_neg_value(q)
         masks = []
         final_attn_mask = None
 
         if exists(input_mask):
             input_mask = rearrange(input_mask, 'b j -> b 1 1 j')
             masks.append(~input_mask)
 
@@ -1145,15 +1143,15 @@
         if exists(self.rotary_pos_emb):
             max_rotary_emb_length = max(list(map(lambda m: (m.shape[1] if exists(m) else 0) + x.shape[1], mems)))
             rotary_pos_emb = self.rotary_pos_emb(max_rotary_emb_length, x.device)
 
         outer_residual = x
 
         for ind, (layer_type, (norm, block, residual_fn), layer_dropout) in enumerate(zip(self.layer_types, self.layers, self.layer_dropouts)):
-            is_last = ind == (self.layers_length - 1)
+            ind == (self.layers_length - 1)
 
             if self.training and layer_dropout > 0. and random() < layer_dropout:
                 continue
 
             if layer_type == 'a':
                 if return_hiddens:
                     hiddens.append(x)
```

### Comparing `optimus-prime-transformers-1.1.9/optimus_prime/xl_autoregressive_wrapper.py` & `optimus-prime-transformers-1.2.1/optimus_prime/xl_autoregressive_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-from math import ceil
 
 import torch
 from torch import nn
 import torch.nn.functional as F
 
 from einops import rearrange, pack, unpack
-from optimus_prime.autoregressive_wrapper import top_p, top_k, eval_decorator
+from optimus_prime.autoregressive_wrapper import top_k, eval_decorator
 
 # helper functions
 
 def exists(val):
     return val is not None
 
 def divisible_by(numer, denom):
```

### Comparing `optimus-prime-transformers-1.1.9/optimus_prime_transformers.egg-info/PKG-INFO` & `optimus-prime-transformers-1.2.1/optimus_prime_transformers.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimus-prime-transformers
-Version: 1.1.9
+Version: 1.2.1
 Summary: optimus-prime - Pytorch
 Home-page: https://github.com/kyegomez/Optimus-Prime
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `optimus-prime-transformers-1.1.9/optimus_prime_transformers.egg-info/SOURCES.txt` & `optimus-prime-transformers-1.2.1/optimus_prime_transformers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.9/setup.py` & `optimus-prime-transformers-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'optimus-prime-transformers',
   packages = find_packages(exclude=['examples']),
-  version = '1.1.9',
+  version = '1.2.1',
   license='MIT',
   description = 'optimus-prime - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   url = 'https://github.com/kyegomez/Optimus-Prime',
   long_description_content_type = 'text/markdown',
   keywords = [
```

