# Comparing `tmp/hezar-0.20.0.tar.gz` & `tmp/hezar-0.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hezar-0.20.0.tar", max compression
+gzip compressed data, was "hezar-0.20.1.tar", max compression
```

## Comparing `hezar-0.20.0.tar` & `hezar-0.20.1.tar`

### file list

```diff
@@ -1,92 +1,93 @@
--rw-r--r--   0        0        0     1065 2023-08-04 08:49:04.037069 hezar-0.20.0/LICENSE
--rw-r--r--   0        0        0     4145 2023-08-04 08:49:04.037069 hezar-0.20.0/README.md
--rw-r--r--   0        0        0      260 2023-08-04 08:49:04.037069 hezar-0.20.0/hezar/__init__.py
--rw-r--r--   0        0        0     5336 2023-08-04 08:49:04.037069 hezar-0.20.0/hezar/builders.py
--rw-r--r--   0        0        0    11489 2023-08-04 08:49:04.037069 hezar-0.20.0/hezar/configs.py
--rw-r--r--   0        0        0     2072 2023-08-04 08:49:04.037069 hezar-0.20.0/hezar/constants.py
--rw-r--r--   0        0        0       75 2023-08-04 08:49:04.037069 hezar-0.20.0/hezar/data/__init__.py
--rw-r--r--   0        0        0     6365 2023-08-04 08:49:04.037069 hezar-0.20.0/hezar/data/data_collators.py
--rw-r--r--   0        0        0      320 2023-08-04 08:49:04.037069 hezar-0.20.0/hezar/data/datasets/__init__.py
--rw-r--r--   0        0        0     1758 2023-08-04 08:49:04.037069 hezar-0.20.0/hezar/data/datasets/dataset.py
--rw-r--r--   0        0        0     4545 2023-08-04 08:49:04.037069 hezar-0.20.0/hezar/data/datasets/sequence_labeling_dataset.py
--rw-r--r--   0        0        0     3653 2023-08-04 08:49:04.037069 hezar-0.20.0/hezar/data/datasets/text_classification_dataset.py
--rw-r--r--   0        0        0     3581 2023-08-04 08:49:04.037069 hezar-0.20.0/hezar/data/datasets/text_summarization_dataset.py
--rw-r--r--   0        0        0       26 2023-08-04 08:49:04.037069 hezar-0.20.0/hezar/data/utils/__init__.py
--rw-r--r--   0        0        0     1856 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/data/utils/data_utils.py
--rw-r--r--   0        0        0      127 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/embeddings/__init__.py
--rw-r--r--   0        0        0     4124 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/embeddings/embedding.py
--rw-r--r--   0        0        0     3122 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/embeddings/fasttext.py
--rw-r--r--   0        0        0     3081 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/embeddings/word2vec.py
--rw-r--r--   0        0        0      141 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/metrics/__init__.py
--rw-r--r--   0        0        0     1184 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/metrics/f1.py
--rw-r--r--   0        0        0      983 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/metrics/metric.py
--rw-r--r--   0        0        0     1295 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/metrics/recall.py
--rw-r--r--   0        0        0     2090 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/metrics/seqeval.py
--rw-r--r--   0        0        0      273 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/audio_classification/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/image2text/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/image2text/crnn/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/image2text/trocr/__init__.py
--rw-r--r--   0        0        0      144 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/language_modeling/__init__.py
--rw-r--r--   0        0        0       69 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/language_modeling/bert/__init__.py
--rw-r--r--   0        0        0     1614 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/language_modeling/bert/bert_lm.py
--rw-r--r--   0        0        0      762 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/language_modeling/bert/bert_lm_config.py
--rw-r--r--   0        0        0       93 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/language_modeling/distilbert/__init__.py
--rw-r--r--   0        0        0     1686 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/language_modeling/distilbert/distilbert_lm.py
--rw-r--r--   0        0        0      628 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
--rw-r--r--   0        0        0       81 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/language_modeling/roberta/__init__.py
--rw-r--r--   0        0        0     1644 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/language_modeling/roberta/roberta_lm.py
--rw-r--r--   0        0        0      822 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/language_modeling/roberta/roberta_lm_config.py
--rw-r--r--   0        0        0    11719 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/model.py
--rw-r--r--   0        0        0      152 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/sequence_labeling/__init__.py
--rw-r--r--   0        0        0      127 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/sequence_labeling/bert/__init__.py
--rw-r--r--   0        0        0     3981 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
--rw-r--r--   0        0        0      936 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
--rw-r--r--   0        0        0      151 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/sequence_labeling/distilbert/__init__.py
--rw-r--r--   0        0        0     4142 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
--rw-r--r--   0        0        0      877 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
--rw-r--r--   0        0        0        0 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/speech_recognition/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/speech_recognition/wav2vec/__init__.py
--rw-r--r--   0        0        0       47 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text2text/__init__.py
--rw-r--r--   0        0        0       89 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text2text/t5/__init__.py
--rw-r--r--   0        0        0     3848 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text2text/t5/t5_text2text.py
--rw-r--r--   0        0        0      764 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text2text/t5/t5_text2text_config.py
--rw-r--r--   0        0        0      240 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_classification/__init__.py
--rw-r--r--   0        0        0      135 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_classification/bert/__init__.py
--rw-r--r--   0        0        0     3540 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_classification/bert/bert_text_classification.py
--rw-r--r--   0        0        0      850 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_classification/bert/bert_text_classification_config.py
--rw-r--r--   0        0        0      159 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_classification/distilbert/__init__.py
--rw-r--r--   0        0        0     3676 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py
--rw-r--r--   0        0        0      753 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
--rw-r--r--   0        0        0      147 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_classification/roberta/__init__.py
--rw-r--r--   0        0        0     3819 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_classification/roberta/roberta_text_classification.py
--rw-r--r--   0        0        0      947 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py
--rw-r--r--   0        0        0        0 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_detection/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_detection/ctpn/__init__.py
--rw-r--r--   0        0        0        0 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/models/text_detection/dbnet/__init__.py
--rw-r--r--   0        0        0      155 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/preprocessors/__init__.py
--rw-r--r--   0        0        0     4119 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/preprocessors/preprocessor.py
--rw-r--r--   0        0        0     3633 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/preprocessors/text_normalizer.py
--rw-r--r--   0        0        0      324 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/preprocessors/tokenizers/__init__.py
--rw-r--r--   0        0        0     4556 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/preprocessors/tokenizers/bpe.py
--rw-r--r--   0        0        0     5045 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
--rw-r--r--   0        0        0     4965 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/preprocessors/tokenizers/sentencepiece_unigram.py
--rw-r--r--   0        0        0    19342 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/preprocessors/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     4132 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/preprocessors/tokenizers/wordpiece.py
--rw-r--r--   0        0        0     8828 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/registry.py
--rw-r--r--   0        0        0      143 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/trainers/__init__.py
--rw-r--r--   0        0        0       63 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/trainers/sequence_labeling/__init__.py
--rw-r--r--   0        0        0     2644 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
--rw-r--r--   0        0        0       67 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/trainers/text_classification/__init__.py
--rw-r--r--   0        0        0     2282 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/trainers/text_classification/text_classification_trainer.py
--rw-r--r--   0        0        0    17990 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/trainers/trainer.py
--rw-r--r--   0        0        0     1626 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/trainers/trainer_utils.py
--rw-r--r--   0        0        0      164 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/utils/__init__.py
--rw-r--r--   0        0        0      611 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/utils/common_utils.py
--rw-r--r--   0        0        0      482 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/utils/context_managers.py
--rw-r--r--   0        0        0     5614 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/utils/core_utils.py
--rw-r--r--   0        0        0     3660 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/utils/hub_utils.py
--rw-r--r--   0        0        0      374 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/utils/logging.py
--rw-r--r--   0        0        0      936 2023-08-04 08:49:04.041069 hezar-0.20.0/hezar/utils/registry_utils.py
--rw-r--r--   0        0        0     1648 2023-08-04 08:49:04.045070 hezar-0.20.0/pyproject.toml
--rw-r--r--   0        0        0     6627 1970-01-01 00:00:00.000000 hezar-0.20.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-05 10:51:49.803922 hezar-0.20.1/LICENSE
+-rw-r--r--   0        0        0     4750 2023-08-05 10:51:49.803922 hezar-0.20.1/README.md
+-rw-r--r--   0        0        0      260 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/__init__.py
+-rw-r--r--   0        0        0     5336 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/builders.py
+-rw-r--r--   0        0        0    11576 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/configs.py
+-rw-r--r--   0        0        0     2072 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/constants.py
+-rw-r--r--   0        0        0       75 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/data/__init__.py
+-rw-r--r--   0        0        0     6365 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/data/data_collators.py
+-rw-r--r--   0        0        0      320 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/data/datasets/__init__.py
+-rw-r--r--   0        0        0     1758 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/data/datasets/dataset.py
+-rw-r--r--   0        0        0     4545 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/data/datasets/sequence_labeling_dataset.py
+-rw-r--r--   0        0        0     3653 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/data/datasets/text_classification_dataset.py
+-rw-r--r--   0        0        0     3581 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/data/datasets/text_summarization_dataset.py
+-rw-r--r--   0        0        0       26 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/data/utils/__init__.py
+-rw-r--r--   0        0        0     1856 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/data/utils/data_utils.py
+-rw-r--r--   0        0        0      127 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/embeddings/__init__.py
+-rw-r--r--   0        0        0     4124 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/embeddings/embedding.py
+-rw-r--r--   0        0        0     3122 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/embeddings/fasttext.py
+-rw-r--r--   0        0        0     3081 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/embeddings/word2vec.py
+-rw-r--r--   0        0        0      141 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/metrics/__init__.py
+-rw-r--r--   0        0        0     1184 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/metrics/f1.py
+-rw-r--r--   0        0        0      983 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/metrics/metric.py
+-rw-r--r--   0        0        0     1295 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/metrics/recall.py
+-rw-r--r--   0        0        0     2090 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/metrics/seqeval.py
+-rw-r--r--   0        0        0      273 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/audio_classification/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/image2text/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/image2text/crnn/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/image2text/trocr/__init__.py
+-rw-r--r--   0        0        0      144 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/language_modeling/__init__.py
+-rw-r--r--   0        0        0       69 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/language_modeling/bert/__init__.py
+-rw-r--r--   0        0        0     1614 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/language_modeling/bert/bert_lm.py
+-rw-r--r--   0        0        0      762 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/language_modeling/bert/bert_lm_config.py
+-rw-r--r--   0        0        0       93 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/language_modeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     1686 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/language_modeling/distilbert/distilbert_lm.py
+-rw-r--r--   0        0        0      628 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
+-rw-r--r--   0        0        0       81 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/language_modeling/roberta/__init__.py
+-rw-r--r--   0        0        0     1644 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/language_modeling/roberta/roberta_lm.py
+-rw-r--r--   0        0        0      822 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/language_modeling/roberta/roberta_lm_config.py
+-rw-r--r--   0        0        0    11719 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/model.py
+-rw-r--r--   0        0        0     1434 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/model_outputs.py
+-rw-r--r--   0        0        0      152 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0      127 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/sequence_labeling/bert/__init__.py
+-rw-r--r--   0        0        0     3981 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
+-rw-r--r--   0        0        0      936 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
+-rw-r--r--   0        0        0      151 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/sequence_labeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     4142 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py
+-rw-r--r--   0        0        0      877 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py
+-rw-r--r--   0        0        0        0 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/speech_recognition/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/speech_recognition/wav2vec/__init__.py
+-rw-r--r--   0        0        0       47 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text2text/__init__.py
+-rw-r--r--   0        0        0       89 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text2text/t5/__init__.py
+-rw-r--r--   0        0        0     3848 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text2text/t5/t5_text2text.py
+-rw-r--r--   0        0        0      764 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text2text/t5/t5_text2text_config.py
+-rw-r--r--   0        0        0      240 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_classification/__init__.py
+-rw-r--r--   0        0        0      135 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_classification/bert/__init__.py
+-rw-r--r--   0        0        0     3540 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_classification/bert/bert_text_classification.py
+-rw-r--r--   0        0        0      850 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_classification/bert/bert_text_classification_config.py
+-rw-r--r--   0        0        0      159 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_classification/distilbert/__init__.py
+-rw-r--r--   0        0        0     3676 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_classification/distilbert/distilbert_text_classification.py
+-rw-r--r--   0        0        0      753 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
+-rw-r--r--   0        0        0      147 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_classification/roberta/__init__.py
+-rw-r--r--   0        0        0     3819 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_classification/roberta/roberta_text_classification.py
+-rw-r--r--   0        0        0      947 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_classification/roberta/roberta_text_classification_config.py
+-rw-r--r--   0        0        0        0 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_detection/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_detection/ctpn/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/models/text_detection/dbnet/__init__.py
+-rw-r--r--   0        0        0      155 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/preprocessors/__init__.py
+-rw-r--r--   0        0        0     4119 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/preprocessors/preprocessor.py
+-rw-r--r--   0        0        0     3633 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/preprocessors/text_normalizer.py
+-rw-r--r--   0        0        0      324 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/preprocessors/tokenizers/__init__.py
+-rw-r--r--   0        0        0     4556 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/preprocessors/tokenizers/bpe.py
+-rw-r--r--   0        0        0     5045 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
+-rw-r--r--   0        0        0     4965 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/preprocessors/tokenizers/sentencepiece_unigram.py
+-rw-r--r--   0        0        0    19472 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/preprocessors/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     4132 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/preprocessors/tokenizers/wordpiece.py
+-rw-r--r--   0        0        0     8828 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/registry.py
+-rw-r--r--   0        0        0      143 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/trainers/__init__.py
+-rw-r--r--   0        0        0       63 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/trainers/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0     2644 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
+-rw-r--r--   0        0        0       67 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/trainers/text_classification/__init__.py
+-rw-r--r--   0        0        0     2282 2023-08-05 10:51:49.807922 hezar-0.20.1/hezar/trainers/text_classification/text_classification_trainer.py
+-rw-r--r--   0        0        0    18229 2023-08-05 10:51:49.811922 hezar-0.20.1/hezar/trainers/trainer.py
+-rw-r--r--   0        0        0     1626 2023-08-05 10:51:49.811922 hezar-0.20.1/hezar/trainers/trainer_utils.py
+-rw-r--r--   0        0        0      164 2023-08-05 10:51:49.811922 hezar-0.20.1/hezar/utils/__init__.py
+-rw-r--r--   0        0        0      611 2023-08-05 10:51:49.811922 hezar-0.20.1/hezar/utils/common_utils.py
+-rw-r--r--   0        0        0      482 2023-08-05 10:51:49.811922 hezar-0.20.1/hezar/utils/context_managers.py
+-rw-r--r--   0        0        0     5615 2023-08-05 10:51:49.811922 hezar-0.20.1/hezar/utils/core_utils.py
+-rw-r--r--   0        0        0     3660 2023-08-05 10:51:49.811922 hezar-0.20.1/hezar/utils/hub_utils.py
+-rw-r--r--   0        0        0      374 2023-08-05 10:51:49.811922 hezar-0.20.1/hezar/utils/logging.py
+-rw-r--r--   0        0        0      936 2023-08-05 10:51:49.811922 hezar-0.20.1/hezar/utils/registry_utils.py
+-rw-r--r--   0        0        0     1648 2023-08-05 10:51:49.811922 hezar-0.20.1/pyproject.toml
+-rw-r--r--   0        0        0     7232 1970-01-01 00:00:00.000000 hezar-0.20.1/PKG-INFO
```

### Comparing `hezar-0.20.0/LICENSE` & `hezar-0.20.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/builders.py` & `hezar-0.20.1/hezar/builders.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/configs.py` & `hezar-0.20.1/hezar/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,16 @@
     "EmbeddingConfig": ConfigType.EMBEDDING,
     "CriterionConfig": ConfigType.CRITERION,
     "OptimizerConfig": ConfigType.OPTIMIZER,
     "LRSchedulerConfig": ConfigType.LR_SCHEDULER,
     "MetricConfig": ConfigType.METRIC,
 }
 
+CONFIG_CLASS_VARS = ["name", "config_type"]
+
 
 @dataclass
 class Config:
     """
     Base class for all configs in Hezar.
 
     All configs are simple dataclasses that have some customized functionalities to manage their attributes. There are
@@ -165,16 +167,16 @@
     @classmethod
     def from_dict(cls, dict_config: Union[Dict, DictConfig], **kwargs):
         """
         Load config from a dict-like object
         """
         # Update config parameters with kwargs
         dict_config.update(**kwargs)
-        dict_config.pop("name", None)
-        dict_config.pop("config_type", None)
+        # Remove class vars to avoid TypeError (unexpected argument)
+        [dict_config.pop(k) for k in CONFIG_CLASS_VARS]
 
         config = cls(**{k: v for k, v in dict_config.items() if hasattr(cls, k)})  # noqa
 
         return config
 
     def save(
         self,
```

### Comparing `hezar-0.20.0/hezar/constants.py` & `hezar-0.20.1/hezar/constants.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/data/data_collators.py` & `hezar-0.20.1/hezar/data/data_collators.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/data/datasets/dataset.py` & `hezar-0.20.1/hezar/data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/data/datasets/sequence_labeling_dataset.py` & `hezar-0.20.1/hezar/data/datasets/sequence_labeling_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/data/datasets/text_classification_dataset.py` & `hezar-0.20.1/hezar/data/datasets/text_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/data/datasets/text_summarization_dataset.py` & `hezar-0.20.1/hezar/data/datasets/text_summarization_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/data/utils/data_utils.py` & `hezar-0.20.1/hezar/data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/embeddings/embedding.py` & `hezar-0.20.1/hezar/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/embeddings/fasttext.py` & `hezar-0.20.1/hezar/embeddings/fasttext.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/embeddings/word2vec.py` & `hezar-0.20.1/hezar/embeddings/word2vec.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/metrics/f1.py` & `hezar-0.20.1/hezar/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/metrics/metric.py` & `hezar-0.20.1/hezar/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/metrics/recall.py` & `hezar-0.20.1/hezar/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/metrics/seqeval.py` & `hezar-0.20.1/hezar/metrics/seqeval.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/models/language_modeling/bert/bert_lm.py` & `hezar-0.20.1/hezar/models/language_modeling/bert/bert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/models/language_modeling/bert/bert_lm_config.py` & `hezar-0.20.1/hezar/models/language_modeling/bert/bert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/models/language_modeling/distilbert/distilbert_lm.py` & `hezar-0.20.1/hezar/models/language_modeling/distilbert/distilbert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py` & `hezar-0.20.1/hezar/models/language_modeling/distilbert/distilbert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/models/language_modeling/roberta/roberta_lm.py` & `hezar-0.20.1/hezar/models/language_modeling/roberta/roberta_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/models/language_modeling/roberta/roberta_lm_config.py` & `hezar-0.20.1/hezar/models/language_modeling/roberta/roberta_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/models/model.py` & `hezar-0.20.1/hezar/models/model.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py` & `hezar-0.20.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py` & `hezar-0.20.1/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py` & `hezar-0.20.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py` & `hezar-0.20.1/hezar/models/sequence_labeling/distilbert/distilbert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/models/text2text/t5/t5_text2text.py` & `hezar-0.20.1/hezar/models/text2text/t5/t5_text2text.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/models/text2text/t5/t5_text2text_config.py` & `hezar-0.20.1/hezar/models/text2text/t5/t5_text2text_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/models/text_classification/bert/bert_text_classification.py` & `hezar-0.20.1/hezar/models/text_classification/bert/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/models/text_classification/bert/bert_text_classification_config.py` & `hezar-0.20.1/hezar/models/text_classification/bert/bert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py` & `hezar-0.20.1/hezar/models/text_classification/distilbert/distilbert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py` & `hezar-0.20.1/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/models/text_classification/roberta/roberta_text_classification.py` & `hezar-0.20.1/hezar/models/text_classification/roberta/roberta_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py` & `hezar-0.20.1/hezar/models/text_classification/roberta/roberta_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/preprocessors/preprocessor.py` & `hezar-0.20.1/hezar/preprocessors/preprocessor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/preprocessors/text_normalizer.py` & `hezar-0.20.1/hezar/preprocessors/text_normalizer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/preprocessors/tokenizers/bpe.py` & `hezar-0.20.1/hezar/preprocessors/tokenizers/bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py` & `hezar-0.20.1/hezar/preprocessors/tokenizers/sentencepiece_bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/preprocessors/tokenizers/sentencepiece_unigram.py` & `hezar-0.20.1/hezar/preprocessors/tokenizers/sentencepiece_unigram.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/preprocessors/tokenizers/tokenizer.py` & `hezar-0.20.1/hezar/preprocessors/tokenizers/tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,14 +194,17 @@
             return_length: Whether to return input lengths
             **kwargs: Extra arguments reside here and therefore ignored
 
         Returns:
             A dictionary of encoded inputs like
                 {"token_ids": [batch_size x input_len], "attention_mask": [batch_size x input_len], ...}
         """
+        if isinstance(inputs, list) and not len(inputs):
+            raise ValueError("Tokenizer cannot process an empty list!")
+
         if isinstance(inputs, str):
             inputs = [inputs]
 
         padding_strategy = padding_strategy or self.config.padding_strategy
         truncation_strategy = truncation_strategy or self.config.truncation_strategy
         max_length = max_length or self.config.max_length
         pad_to_multiple_of = pad_to_multiple_of or self.config.pad_to_multiple_of
```

### Comparing `hezar-0.20.0/hezar/preprocessors/tokenizers/wordpiece.py` & `hezar-0.20.1/hezar/preprocessors/tokenizers/wordpiece.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/registry.py` & `hezar-0.20.1/hezar/registry.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py` & `hezar-0.20.1/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/trainers/text_classification/text_classification_trainer.py` & `hezar-0.20.1/hezar/trainers/text_classification/text_classification_trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/trainers/trainer.py` & `hezar-0.20.1/hezar/trainers/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     HEZAR_CACHE_DIR,
     TQDM_BAR_FORMAT,
 )
 from ..data.datasets import Dataset
 from ..models import Model
 from ..preprocessors import Preprocessor, PreprocessorsContainer
 from ..utils import get_logger
-from .trainer_utils import MetricsTracker
+from .trainer_utils import MetricsTracker, write_to_tensorboard
 
 
 logger = get_logger(__name__)
 
 optimizers = {
     "adam": torch.optim.Adam,
     "adamw": torch.optim.AdamW,
@@ -378,18 +378,22 @@
 
     def train(self):
         """
         The full training process like training, evaluation, logging and saving model checkpoints.
         """
         for epoch in range(1, self.config.num_epochs + 1):
             print()
-            self.inner_training_loop(epoch)
+            training_results = self.inner_training_loop(epoch)
             evaluation_results = self.evaluate()
             self.lr_scheduler.step(evaluation_results["loss"])
 
+            # tensorboard
+            write_to_tensorboard(self.tensorboard, training_results, "train", epoch)
+            write_to_tensorboard(self.tensorboard, evaluation_results, "eval", epoch)
+
             # maybe save checkpoint
             if epoch % self.config.save_freq == 0:
                 ckpt_save_path = os.path.join(self.config.checkpoints_dir, str(epoch))
                 self.save(ckpt_save_path)
 
     def save(
         self,
```

### Comparing `hezar-0.20.0/hezar/trainers/trainer_utils.py` & `hezar-0.20.1/hezar/trainers/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/utils/common_utils.py` & `hezar-0.20.1/hezar/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/utils/core_utils.py` & `hezar-0.20.1/hezar/utils/core_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     elif config_type == ConfigType.TRAINER:
         from ..registry import trainers_registry  # noqa
         registry = trainers_registry
 
     elif config_type is None:
         return None
     else:
-        raise ValueError(f"Invalid `config_type`: {config_type}!")
+        raise ValueError(f"Invalid `config_type`: `{config_type}`")
 
     config_cls = registry[name].config_class
     return config_cls
 
 
 def get_module_class(name: str, module_type: str):
     """
```

### Comparing `hezar-0.20.0/hezar/utils/hub_utils.py` & `hezar-0.20.1/hezar/utils/hub_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/hezar/utils/registry_utils.py` & `hezar-0.20.1/hezar/utils/registry_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.20.0/pyproject.toml` & `hezar-0.20.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hezar"
-version = "0.20.0"
+version = "0.20.1"
 packages = [{ include = "hezar" }]
 description = "Hezar: A seamless AI framework & library for Persian"
 license = "MIT"
 authors = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 maintainers = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 repository = "https://github.com/hezarai/hezar"
 homepage = "https://github.com/hezarai"
```

### Comparing `hezar-0.20.0/PKG-INFO` & `hezar-0.20.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hezar
-Version: 0.20.0
+Version: 0.20.1
 Summary: Hezar: A seamless AI framework & library for Persian
 Home-page: https://github.com/hezarai
 License: MIT
 Keywords: packaging,poetry
 Author: Aryan Shekarlaban
 Author-email: arxyzan@gmail.com
 Maintainer: Aryan Shekarlaban
@@ -81,23 +81,36 @@
 ```commandline
 {'labels': ['positive'], 'probs': [0.812910258769989]}
 ```
 #### Sequence labeling (part-of-speech tagging)
 ```python
 from hezar import Model
 
-hub_path = "hezarai/bert-fa-pos-lscp-500k"
+hub_path = "hezarai/distilbert-fa-pos-lscp-500k"
 model = Model.load(hub_path)
 inputs = ["سلام بر فارسی زبانان شریف"]
 outputs = model.predict(inputs)
 print(outputs)
 ```
 ```commandline
 [[{'token': 'سلام', 'tag': 'N'}, {'token': 'بر', 'tag': 'P'}, {'token': 'فارسی', 'tag': 'Ne'}, {'token': 'زبانان', 'tag': 'Ne'}, {'token': 'شریف', 'tag': 'AJ'}]]
 ```
+#### Sequence labeling (named entity recognition)
+```python
+from hezar import Model
+
+hub_path = "hezarai/bert-fa-ner-arman"
+model = Model.load(hub_path)
+inputs = ["شرکت هوش مصنوعی هزار برترین در نوع خود"]
+outputs = model.predict(inputs)
+print(outputs)
+```
+```commandline
+[[{'token': 'شرکت', 'tag': 'B-org'}, {'token': 'هوش', 'tag': 'I-org'}, {'token': 'مصنوعی', 'tag': 'I-org'}, {'token': 'هزار', 'tag': 'O'}, {'token': 'برترین', 'tag': 'O'}, {'token': 'در', 'tag': 'O'}, {'token': 'نوع', 'tag': 'O'}, {'token': 'خود', 'tag': 'O'}]]
+```
 ### Write your own model
 It's fairly easy to extend this library or add your own model. Hezar has its own `Model` base class that is simply a normal PyTorch `nn.Module` but with some extra features!
 
 Here's a simple example:
 ```python
 from dataclasses import dataclass
```

