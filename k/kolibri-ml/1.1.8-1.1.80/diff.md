# Comparing `tmp/kolibri_ml-1.1.8-py3-none-any.whl.zip` & `tmp/kolibri_ml-1.1.80-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,494 +1,701 @@
-Zip file size: 896369 bytes, number of entries: 492
--rw-r--r--  2.0 unx        6 b- defN 22-Dec-18 21:22 kolibri/VERSION
--rw-r--r--  2.0 unx     3871 b- defN 22-Nov-02 17:03 kolibri/__init__.py
--rw-r--r--  2.0 unx    16782 b- defN 22-Dec-05 22:19 kolibri/app.py
--rw-r--r--  2.0 unx     3190 b- defN 22-Sep-25 20:08 kolibri/config.py
--rw-r--r--  2.0 unx     1902 b- defN 22-Aug-28 22:03 kolibri/config_loader.py
--rw-r--r--  2.0 unx     3213 b- defN 22-Sep-08 11:52 kolibri/default_configs.py
--rw-r--r--  2.0 unx     3186 b- defN 22-Jan-21 10:53 kolibri/errors.py
--rw-r--r--  2.0 unx      795 b- defN 22-Aug-28 17:38 kolibri/logger.py
--rw-r--r--  2.0 unx     2219 b- defN 22-Jul-02 23:09 kolibri/metadata.py
--rw-r--r--  2.0 unx     9868 b- defN 22-Dec-18 21:13 kolibri/model_loader.py
--rw-r--r--  2.0 unx    23844 b- defN 22-Dec-18 16:22 kolibri/model_trainer.py
--rw-r--r--  2.0 unx      968 b- defN 22-Jun-30 13:31 kolibri/registry.py
--rw-r--r--  2.0 unx      153 b- defN 22-Dec-07 22:11 kolibri/requirements.txt
--rw-r--r--  2.0 unx      458 b- defN 22-Sep-08 17:35 kolibri/settings.yaml
--rw-r--r--  2.0 unx        0 b- defN 22-Sep-25 16:44 kolibri/api/__init__.py
--rw-r--r--  2.0 unx     2707 b- defN 22-Sep-25 19:43 kolibri/api/classification/__init__.py
--rw-r--r--  2.0 unx       66 b- defN 22-Oct-09 12:38 kolibri/autolearn/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 21-Sep-21 12:16 kolibri/autolearn/metalearn/__init__.py
--rw-r--r--  2.0 unx     3125 b- defN 22-Jul-05 22:48 kolibri/autolearn/metalearn/metafeature.py
--rw-r--r--  2.0 unx    46866 b- defN 21-Oct-19 09:44 kolibri/autolearn/metalearn/metafeatures.py
--rw-r--r--  2.0 unx        0 b- defN 21-Sep-21 12:16 kolibri/autolearn/model_zoo/__init__.py
--rw-r--r--  2.0 unx     4737 b- defN 22-Oct-09 13:05 kolibri/autolearn/model_zoo/zoo_classifier.py
--rw-r--r--  2.0 unx     4310 b- defN 22-Oct-09 12:38 kolibri/autolearn/model_zoo/zoo_regressor.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-02 09:22 kolibri/backend/__init__.py
--rw-r--r--  2.0 unx     6289 b- defN 22-Oct-08 14:57 kolibri/backend/models.py
--rw-r--r--  2.0 unx        0 b- defN 21-Sep-02 15:44 kolibri/backend/base/__init__.py
--rw-r--r--  2.0 unx    11843 b- defN 22-Dec-18 21:21 kolibri/backend/base/base_classifier.py
--rw-r--r--  2.0 unx     3916 b- defN 22-Nov-13 22:39 kolibri/backend/base/base_clustering.py
--rw-r--r--  2.0 unx    30343 b- defN 22-Dec-18 00:31 kolibri/backend/base/base_estimator.py
--rw-r--r--  2.0 unx     7481 b- defN 22-Dec-15 13:37 kolibri/backend/base/base_regressor.py
--rw-r--r--  2.0 unx        0 b- defN 21-Apr-13 11:37 kolibri/backend/sklearn/__init__.py
--rw-r--r--  2.0 unx       65 b- defN 21-Apr-15 22:05 kolibri/backend/sklearn/meta/__init__.py
--rw-r--r--  2.0 unx    13257 b- defN 22-Oct-31 12:46 kolibri/backend/sklearn/meta/chain_model.py
--rw-r--r--  2.0 unx    28314 b- defN 22-Oct-04 18:06 kolibri/backend/sklearn/meta/ecoc_model.py
--rw-r--r--  2.0 unx    28328 b- defN 22-Oct-31 12:46 kolibri/backend/sklearn/meta/ensemble_samplers.py
--rw-r--r--  2.0 unx     7646 b- defN 22-Oct-31 12:46 kolibri/backend/sklearn/meta/multi_output_estimator.py
--rw-r--r--  2.0 unx        0 b- defN 21-Apr-17 15:17 kolibri/backend/sklearn/meta/ecoc/__init__.py
--rw-r--r--  2.0 unx     8616 b- defN 21-Apr-21 12:22 kolibri/backend/sklearn/meta/ecoc/code_matrix.py
--rw-r--r--  2.0 unx     5551 b- defN 21-Apr-17 16:12 kolibri/backend/sklearn/meta/ecoc/criterion.py
--rw-r--r--  2.0 unx     9089 b- defN 21-Apr-17 17:44 kolibri/backend/sklearn/meta/ecoc/decoder.py
--rw-r--r--  2.0 unx     3869 b- defN 21-Oct-05 20:31 kolibri/backend/sklearn/meta/ecoc/sffs.py
--rw-r--r--  2.0 unx     2625 b- defN 22-Mar-25 17:19 kolibri/backend/tensorflow/__init__.py
--rw-r--r--  2.0 unx     2111 b- defN 22-Jan-20 18:54 kolibri/backend/tensorflow/callbacks.py
--rw-r--r--  2.0 unx     2959 b- defN 20-Aug-02 06:27 kolibri/backend/tensorflow/custom_loses.py
--rw-r--r--  2.0 unx     9632 b- defN 22-Jan-20 18:11 kolibri/backend/tensorflow/loader.py
--rw-r--r--  2.0 unx    14280 b- defN 22-Jan-20 18:11 kolibri/backend/tensorflow/loader_albert.py
--rw-r--r--  2.0 unx     9030 b- defN 22-May-11 08:30 kolibri/backend/tensorflow/utils.py
--rw-r--r--  2.0 unx      354 b- defN 22-May-12 08:51 kolibri/backend/tensorflow/autoencoder/__init__.py
--rw-r--r--  2.0 unx     6654 b- defN 22-Sep-12 12:27 kolibri/backend/tensorflow/autoencoder/base_autoencoder.py
--rw-r--r--  2.0 unx     3338 b- defN 22-May-12 08:51 kolibri/backend/tensorflow/autoencoder/conv_autoencoder.py
--rw-r--r--  2.0 unx     2601 b- defN 22-May-12 08:51 kolibri/backend/tensorflow/autoencoder/deep_autoencoder.py
--rw-r--r--  2.0 unx     3749 b- defN 22-May-12 08:52 kolibri/backend/tensorflow/autoencoder/variational_autoencoder.py
--rw-r--r--  2.0 unx      148 b- defN 20-Aug-03 09:50 kolibri/backend/tensorflow/autoencoder/decoders/__init__.py
--rw-r--r--  2.0 unx     2043 b- defN 22-Jan-20 18:22 kolibri/backend/tensorflow/autoencoder/decoders/att_gru_decoder.py
--rw-r--r--  2.0 unx     1265 b- defN 22-Jan-20 18:22 kolibri/backend/tensorflow/autoencoder/decoders/gru_decoder.py
--rw-r--r--  2.0 unx     1118 b- defN 22-May-12 10:29 kolibri/backend/tensorflow/autoencoder/decoders/lstm_decoder.py
--rw-r--r--  2.0 unx      199 b- defN 22-May-12 08:48 kolibri/backend/tensorflow/autoencoder/encoders/__init__.py
--rw-r--r--  2.0 unx     2159 b- defN 22-Sep-22 22:53 kolibri/backend/tensorflow/autoencoder/encoders/gru_encoder.py
--rw-r--r--  2.0 unx     1317 b- defN 22-May-12 10:22 kolibri/backend/tensorflow/autoencoder/encoders/lstm_encoder.py
--rw-r--r--  2.0 unx      113 b- defN 22-Jan-20 18:29 kolibri/backend/tensorflow/callbacks/__init__.py
--rw-r--r--  2.0 unx     2025 b- defN 22-Jan-21 00:43 kolibri/backend/tensorflow/callbacks/connl_callBack.py
--rw-r--r--  2.0 unx     2249 b- defN 22-Jan-20 18:54 kolibri/backend/tensorflow/callbacks/eval_callBack.py
--rw-r--r--  2.0 unx     1600 b- defN 22-Feb-18 16:28 kolibri/backend/tensorflow/cells/BayesianLSTM.py
--rw-r--r--  2.0 unx        0 b- defN 22-Feb-18 00:19 kolibri/backend/tensorflow/cells/__init__.py
--rw-r--r--  2.0 unx     2566 b- defN 22-Feb-18 00:43 kolibri/backend/tensorflow/cells/variational_posterior.py
--rw-r--r--  2.0 unx      425 b- defN 22-Jan-20 18:11 kolibri/backend/tensorflow/embeddings/__init__.py
--rw-r--r--  2.0 unx     8491 b- defN 22-Nov-06 17:59 kolibri/backend/tensorflow/embeddings/base_embedding.py
--rw-r--r--  2.0 unx     1448 b- defN 22-Sep-22 23:17 kolibri/backend/tensorflow/embeddings/bert_embedding.py
--rw-r--r--  2.0 unx     2326 b- defN 22-Nov-06 18:01 kolibri/backend/tensorflow/embeddings/default_embedding.py
--rw-r--r--  2.0 unx     8420 b- defN 22-Sep-25 11:09 kolibri/backend/tensorflow/embeddings/elmo_embedding.py
--rw-r--r--  2.0 unx     3196 b- defN 20-Jul-31 11:17 kolibri/backend/tensorflow/embeddings/embedding_trainer.py
--rw-r--r--  2.0 unx     1952 b- defN 22-Sep-25 11:09 kolibri/backend/tensorflow/embeddings/fasttext_embedding.py
--rw-r--r--  2.0 unx     2568 b- defN 22-Dec-13 09:19 kolibri/backend/tensorflow/embeddings/glove_embedding.py
--rw-r--r--  2.0 unx     4156 b- defN 22-Nov-04 19:07 kolibri/backend/tensorflow/embeddings/numeric_feature_embedding.py
--rw-r--r--  2.0 unx     4987 b- defN 22-Jan-21 13:32 kolibri/backend/tensorflow/embeddings/stacked_embedding.py
--rw-r--r--  2.0 unx     3801 b- defN 22-Sep-22 23:17 kolibri/backend/tensorflow/embeddings/transformer_embedding.py
--rw-r--r--  2.0 unx     3331 b- defN 22-Jan-21 09:29 kolibri/backend/tensorflow/embeddings/word_embedding.py
--rw-r--r--  2.0 unx      744 b- defN 22-Jan-21 13:14 kolibri/backend/tensorflow/layers/__init__.py
--rw-r--r--  2.0 unx     3258 b- defN 21-Mar-21 23:33 kolibri/backend/tensorflow/layers/att_wgt_avg_layer.py
--rw-r--r--  2.0 unx     1387 b- defN 22-Sep-24 08:45 kolibri/backend/tensorflow/layers/behdanau_attention.py
--rw-r--r--  2.0 unx    10697 b- defN 22-Jan-20 18:11 kolibri/backend/tensorflow/layers/bert_embeddings.py
--rw-r--r--  2.0 unx     4390 b- defN 22-Nov-06 13:43 kolibri/backend/tensorflow/layers/crf.py
--rw-r--r--  2.0 unx     1047 b- defN 20-Jul-24 10:40 kolibri/backend/tensorflow/layers/folding_layer.py
--rw-r--r--  2.0 unx     2033 b- defN 20-Jul-10 19:24 kolibri/backend/tensorflow/layers/highway_layer.py
--rw-r--r--  2.0 unx     3088 b- defN 22-Nov-06 23:40 kolibri/backend/tensorflow/layers/kmax_pool_layer.py
--rw-r--r--  2.0 unx      916 b- defN 21-Feb-23 16:21 kolibri/backend/tensorflow/layers/layer.py
--rw-r--r--  2.0 unx     5012 b- defN 21-Mar-21 22:58 kolibri/backend/tensorflow/layers/multi_head_attention.py
--rw-r--r--  2.0 unx      787 b- defN 20-Jul-23 20:51 kolibri/backend/tensorflow/layers/non_masking_layer.py
--rw-r--r--  2.0 unx       72 b- defN 22-Sep-24 21:26 kolibri/backend/tensorflow/tasks/__init__.py
--rw-r--r--  2.0 unx     5384 b- defN 22-Nov-06 18:12 kolibri/backend/tensorflow/tasks/base_model.py
--rw-r--r--  2.0 unx     7406 b- defN 22-Nov-06 21:50 kolibri/backend/tensorflow/tasks/dnn_estimator.py
--rw-r--r--  2.0 unx        0 b- defN 20-Sep-05 21:04 kolibri/backend/tensorflow/tasks/structured/__init__.py
--rw-r--r--  2.0 unx     7867 b- defN 22-Sep-08 17:33 kolibri/backend/tensorflow/tasks/structured/base_model.py
--rw-r--r--  2.0 unx        0 b- defN 22-May-23 13:21 kolibri/backend/tensorflow/tasks/structured/regression/__init__.py
--rw-r--r--  2.0 unx     4755 b- defN 22-Aug-20 14:01 kolibri/backend/tensorflow/tasks/structured/regression/base_model.py
--rw-r--r--  2.0 unx     1949 b- defN 22-Aug-20 14:01 kolibri/backend/tensorflow/tasks/structured/regression/dnn_regression_estimator.py
--rw-r--r--  2.0 unx     2750 b- defN 22-Aug-20 14:01 kolibri/backend/tensorflow/tasks/structured/regression/models.py
--rw-r--r--  2.0 unx        1 b- defN 22-Oct-23 23:43 kolibri/backend/tensorflow/tasks/text/__init__.py
--rw-r--r--  2.0 unx     6014 b- defN 22-Nov-06 18:12 kolibri/backend/tensorflow/tasks/text/base_model.py
--rw-r--r--  2.0 unx       22 b- defN 22-Oct-23 23:46 kolibri/backend/tensorflow/tasks/text/classification/__init__.py
--rw-r--r--  2.0 unx     9041 b- defN 22-Jan-21 13:15 kolibri/backend/tensorflow/tasks/text/classification/base_model.py
--rw-r--r--  2.0 unx     3394 b- defN 22-Jan-20 18:54 kolibri/backend/tensorflow/tasks/text/classification/cnn_attention_model.py
--rw-r--r--  2.0 unx     6180 b- defN 22-Jan-20 18:54 kolibri/backend/tensorflow/tasks/text/classification/dpcnn_model.py
--rw-r--r--  2.0 unx    28584 b- defN 22-Nov-06 22:11 kolibri/backend/tensorflow/tasks/text/classification/models.py
--rw-r--r--  2.0 unx     7451 b- defN 22-Jan-21 08:25 kolibri/backend/tensorflow/tasks/text/classification/multi_input_output_model.py
--rw-r--r--  2.0 unx        0 b- defN 21-Mar-29 15:23 kolibri/backend/tensorflow/tasks/text/classification/auto/__init__.py
--rw-r--r--  2.0 unx      253 b- defN 21-Mar-22 00:13 kolibri/backend/tensorflow/tasks/text/classification/auto/models.py
--rw-r--r--  2.0 unx      120 b- defN 22-Jan-20 18:54 kolibri/backend/tensorflow/tasks/text/labeling/__init__.py
--rw-r--r--  2.0 unx     8548 b- defN 22-Sep-23 19:17 kolibri/backend/tensorflow/tasks/text/labeling/base_model.py
--rw-r--r--  2.0 unx     3104 b- defN 22-Sep-23 19:32 kolibri/backend/tensorflow/tasks/text/labeling/experimental.py
--rw-r--r--  2.0 unx     9335 b- defN 22-Nov-06 16:57 kolibri/backend/tensorflow/tasks/text/labeling/models.py
--rw-r--r--  2.0 unx       64 b- defN 22-May-11 08:02 kolibri/backend/tensorflow/tasks/text/seq2seq/__init__.py
--rw-r--r--  2.0 unx    13778 b- defN 22-Sep-24 20:56 kolibri/backend/tensorflow/tasks/text/seq2seq/model.py
--rw-r--r--  2.0 unx     9322 b- defN 22-Jan-20 18:11 kolibri/backend/tensorflow/transformer/__init__.py
--rw-r--r--  2.0 unx     6388 b- defN 22-Jan-20 18:11 kolibri/backend/tensorflow/transformer/attention.py
--rw-r--r--  2.0 unx     2957 b- defN 22-Jan-20 18:11 kolibri/backend/tensorflow/transformer/model.py
--rw-r--r--  2.0 unx        0 b- defN 22-Nov-05 22:41 kolibri/backend/torch/__init__.py
--rw-r--r--  2.0 unx    12666 b- defN 22-Nov-06 00:21 kolibri/backend/torch/base_model.py
--rw-r--r--  2.0 unx      305 b- defN 22-Nov-06 00:02 kolibri/backend/torch/utils.py
--rw-r--r--  2.0 unx        0 b- defN 22-Nov-05 23:00 kolibri/backend/torch/layers/__init__.py
--rw-r--r--  2.0 unx     5973 b- defN 21-Mar-04 00:45 kolibri/backend/torch/layers/crf.py
--rw-r--r--  2.0 unx        0 b- defN 22-Nov-05 22:41 kolibri/backend/torch/tasks/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 22-Nov-05 22:41 kolibri/backend/torch/tasks/text/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 22-Nov-05 22:41 kolibri/backend/torch/tasks/text/labeling/__init__.py
--rw-r--r--  2.0 unx     1836 b- defN 22-Nov-05 22:36 kolibri/backend/torch/tasks/text/labeling/bi_lstm_crf.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jul-01 10:37 kolibri/core/__init__.py
--rw-r--r--  2.0 unx    18066 b- defN 22-Dec-04 22:57 kolibri/core/component.py
--rw-r--r--  2.0 unx     1111 b- defN 21-Dec-04 00:38 kolibri/core/entity.py
--rw-r--r--  2.0 unx     3987 b- defN 22-Jul-02 22:11 kolibri/core/modules.py
--rw-r--r--  2.0 unx    14623 b- defN 22-Dec-11 23:58 kolibri/core/pipeline.py
--rw-r--r--  2.0 unx     2429 b- defN 22-Sep-21 19:07 kolibri/core/serializable.py
--rw-r--r--  2.0 unx     5771 b- defN 22-Sep-25 11:32 kolibri/core/vocabulary.py
--rw-r--r--  2.0 unx      110 b- defN 22-Jul-01 10:02 kolibri/data/__init__.py
--rw-r--r--  2.0 unx    39086 b- defN 22-Sep-25 13:32 kolibri/data/downloader.py
--rw-r--r--  2.0 unx    42659 b- defN 22-Jul-01 09:18 kolibri/data/settings.py
--rw-r--r--  2.0 unx    43976 b- defN 22-Sep-25 13:22 kolibri/data/utils.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jan-21 08:45 kolibri/data/text/__init__.py
--rw-r--r--  2.0 unx     2246 b- defN 21-Apr-22 12:23 kolibri/data/text/base_stream.py
--rw-r--r--  2.0 unx     8152 b- defN 22-Sep-21 17:39 kolibri/data/text/corpus.py
--rw-r--r--  2.0 unx    29550 b- defN 22-Jan-21 08:46 kolibri/data/text/dataset.py
--rw-r--r--  2.0 unx    10385 b- defN 22-May-09 21:46 kolibri/data/text/file_stream.py
--rw-r--r--  2.0 unx     6806 b- defN 21-Mar-22 23:04 kolibri/data/text/generators.py
--rw-r--r--  2.0 unx      534 b- defN 21-Apr-22 12:04 kolibri/data/text/iterator.py
--rw-r--r--  2.0 unx    10130 b- defN 21-Apr-03 08:41 kolibri/data/text/schemes.py
--rw-r--r--  2.0 unx     5615 b- defN 22-Jan-21 08:46 kolibri/data/text/streams.py
--rw-r--r--  2.0 unx     7915 b- defN 22-Jan-21 08:46 kolibri/data/text/text.py
--rw-r--r--  2.0 unx      104 b- defN 22-Jan-21 08:57 kolibri/data/text/format/__init__.py
--rw-r--r--  2.0 unx      539 b- defN 20-Jul-31 11:17 kolibri/data/text/format/conll.py
--rw-r--r--  2.0 unx      385 b- defN 20-Jul-10 19:24 kolibri/data/text/format/csv.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jan-21 08:45 kolibri/data/text/quality/__init__.py
--rw-r--r--  2.0 unx     4891 b- defN 22-Oct-30 15:52 kolibri/data/text/quality/cosineSimilarity.py
--rw-r--r--  2.0 unx      983 b- defN 21-Oct-04 20:15 kolibri/data/text/quality/mismatch.py
--rw-r--r--  2.0 unx      166 b- defN 22-Oct-26 22:14 kolibri/data/text/quality/pairwise_cos_sim.py
--rw-r--r--  2.0 unx      837 b- defN 22-Oct-29 10:15 kolibri/data/text/quality/similar.py
--rw-r--r--  2.0 unx       47 b- defN 21-Oct-04 18:56 kolibri/datasets/__init__.py
--rw-r--r--  2.0 unx     1736 b- defN 22-Sep-25 14:51 kolibri/datasets/read_data.py
--rw-r--r--  2.0 unx       61 b- defN 22-Sep-21 09:26 kolibri/datasets/reader/__init__.py
--rw-r--r--  2.0 unx     3092 b- defN 22-Nov-05 17:57 kolibri/datasets/reader/base_reader.py
--rw-r--r--  2.0 unx     4055 b- defN 22-Sep-17 15:40 kolibri/datasets/reader/classification.py
--rw-r--r--  2.0 unx     2213 b- defN 22-Nov-05 21:50 kolibri/datasets/reader/conll.py
--rw-r--r--  2.0 unx    30779 b- defN 22-Sep-21 09:47 kolibri/datasets/reader/dialogs_reader.py
--rw-r--r--  2.0 unx     8005 b- defN 22-Sep-21 11:10 kolibri/datasets/reader/dstc2.py
--rw-r--r--  2.0 unx     4919 b- defN 22-Nov-04 20:27 kolibri/datasets/reader/snips.py
--rw-r--r--  2.0 unx        0 b- defN 21-Sep-02 15:44 kolibri/evaluation/__init__.py
--rw-r--r--  2.0 unx     7885 b- defN 22-Nov-02 17:01 kolibri/evaluation/classifier_evaluator.py
--rw-r--r--  2.0 unx     2489 b- defN 21-Oct-16 00:00 kolibri/evaluation/clustering_evaluator.py
--rw-r--r--  2.0 unx    41666 b- defN 22-Sep-27 16:09 kolibri/evaluation/model_plot.py
--rw-r--r--  2.0 unx      694 b- defN 22-Dec-17 12:46 kolibri/evaluation/metrics/__init__.py
--rw-r--r--  2.0 unx     5578 b- defN 22-Sep-26 15:32 kolibri/evaluation/metrics/anomaly.py
--rw-r--r--  2.0 unx     1792 b- defN 22-Sep-26 21:22 kolibri/evaluation/metrics/base_metric.py
--rw-r--r--  2.0 unx     9438 b- defN 22-Nov-03 18:01 kolibri/evaluation/metrics/classification.py
--rw-r--r--  2.0 unx     7198 b- defN 22-Sep-27 16:03 kolibri/evaluation/metrics/clustering.py
--rw-r--r--  2.0 unx     8757 b- defN 22-Sep-26 09:08 kolibri/evaluation/metrics/metric_utils.py
--rw-r--r--  2.0 unx     9345 b- defN 22-Oct-11 12:43 kolibri/evaluation/metrics/regression.py
--rw-r--r--  2.0 unx    10235 b- defN 22-Sep-26 14:25 kolibri/evaluation/metrics/time_series.py
--rw-r--r--  2.0 unx      224 b- defN 22-Nov-29 22:38 kolibri/experiment_tracking/__init__.py
--rw-r--r--  2.0 unx     8528 b- defN 22-Dec-17 08:43 kolibri/experiment_tracking/experiment_logger.py
--rw-r--r--  2.0 unx     5623 b- defN 22-Dec-16 00:23 kolibri/experiment_tracking/mlflow_logger.py
--rw-r--r--  2.0 unx        0 b- defN 21-Sep-02 15:44 kolibri/explainers/__init__.py
--rw-r--r--  2.0 unx    12089 b- defN 21-Oct-05 20:31 kolibri/explainers/shap_explainer.py
--rw-r--r--  2.0 unx      227 b- defN 22-Nov-15 18:51 kolibri/features/__init__.py
--rw-r--r--  2.0 unx     2781 b- defN 21-Sep-09 08:59 kolibri/features/base_feature.py
--rw-r--r--  2.0 unx     1431 b- defN 22-Dec-15 18:46 kolibri/features/basefeaturizer.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jan-05 23:16 kolibri/features/tabular/__init__.py
--rw-r--r--  2.0 unx     1763 b- defN 22-Jul-01 23:22 kolibri/features/tabular/time_serie_featurizer.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-15 14:23 kolibri/features/text/__init__.py
--rw-r--r--  2.0 unx     8352 b- defN 22-Aug-01 21:32 kolibri/features/text/feature_functions.py
--rw-r--r--  2.0 unx    10019 b- defN 22-Sep-16 15:26 kolibri/features/text/hashing_tfidf_vectorizer.py
--rw-r--r--  2.0 unx     5730 b- defN 22-Aug-01 23:21 kolibri/features/text/text_features.py
--rw-r--r--  2.0 unx     6275 b- defN 22-Dec-17 10:01 kolibri/features/text/tf_idf_featurizer.py
--rw-r--r--  2.0 unx     5782 b- defN 22-Dec-04 08:59 kolibri/features/text/tf_idf_topics_vectorizer.py
--rw-r--r--  2.0 unx     8331 b- defN 22-Sep-25 11:47 kolibri/features/text/tfidf_weighted_embedder.py
--rw-r--r--  2.0 unx      342 b- defN 22-Sep-18 15:10 kolibri/features/text/embedders/__init__.py
--rw-r--r--  2.0 unx     3700 b- defN 22-Nov-02 13:40 kolibri/features/text/embedders/abstract_embedder.py
--rw-r--r--  2.0 unx     1234 b- defN 22-Sep-17 23:04 kolibri/features/text/embedders/bow_embedder.py
--rw-r--r--  2.0 unx    13793 b- defN 22-Sep-16 15:26 kolibri/features/text/embedders/elmo_embedder.py
--rw-r--r--  2.0 unx     1581 b- defN 22-Dec-10 00:43 kolibri/features/text/embedders/fasttext_embedder.py
--rw-r--r--  2.0 unx     2040 b- defN 22-Dec-13 09:30 kolibri/features/text/embedders/glove_embedder.py
--rw-r--r--  2.0 unx     4920 b- defN 22-Sep-16 15:26 kolibri/features/text/embedders/transformers_embedder.py
--rw-r--r--  2.0 unx        0 b- defN 22-Jan-03 17:55 kolibri/features/timeseries/__init__.py
--rw-r--r--  2.0 unx    31971 b- defN 22-Jan-19 07:49 kolibri/features/timeseries/features_utils.py
--rw-r--r--  2.0 unx    10656 b- defN 22-Jul-02 20:23 kolibri/features/timeseries/ts_featurizer.py
--rw-r--r--  2.0 unx     7658 b- defN 22-Jan-06 22:49 kolibri/features/timeseries/utils.py
--rw-r--r--  2.0 unx      358 b- defN 22-Mar-06 10:38 kolibri/features/timeseries/feature_extraction/__init__.py
--rw-r--r--  2.0 unx    16661 b- defN 22-Jul-01 23:22 kolibri/features/timeseries/feature_extraction/data.py
--rw-r--r--  2.0 unx    13772 b- defN 22-Jul-01 23:22 kolibri/features/timeseries/feature_extraction/extraction.py
--rw-r--r--  2.0 unx    81555 b- defN 22-Mar-06 11:53 kolibri/features/timeseries/feature_extraction/feature_calculators.py
--rw-r--r--  2.0 unx    14105 b- defN 22-Mar-06 11:43 kolibri/features/timeseries/feature_extraction/settings.py
--rw-r--r--  2.0 unx      606 b- defN 22-Mar-06 13:17 kolibri/features/timeseries/feature_selection/__init__.py
--rw-r--r--  2.0 unx    15671 b- defN 22-Mar-06 13:20 kolibri/features/timeseries/feature_selection/relevance.py
--rw-r--r--  2.0 unx     7871 b- defN 22-Mar-06 13:25 kolibri/features/timeseries/feature_selection/selection.py
--rw-r--r--  2.0 unx     8691 b- defN 21-Dec-21 03:31 kolibri/features/timeseries/feature_selection/significance_tests.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-08 07:58 kolibri/formers/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-16 07:54 kolibri/formers/tabular/__init__.py
--rw-r--r--  2.0 unx     1043 b- defN 22-Sep-27 15:54 kolibri/formers/tabular/clustering.py
--rw-r--r--  2.0 unx        0 b- defN 21-Mar-18 16:07 kolibri/formers/text/__init__.py
--rw-r--r--  2.0 unx     4315 b- defN 22-Sep-25 19:46 kolibri/formers/text/classifier.py
--rw-r--r--  2.0 unx      230 b- defN 22-Jun-17 11:33 kolibri/formers/text/sentiment.py
--rw-r--r--  2.0 unx     4515 b- defN 22-Sep-27 17:27 kolibri/formers/text/similarity.py
--rw-r--r--  2.0 unx    40764 b- defN 22-Nov-13 23:17 kolibri/formers/text/topic_former.py
--rw-r--r--  2.0 unx      438 b- defN 22-Jan-20 21:51 kolibri/indexers/__init__.py
--rw-r--r--  2.0 unx     6836 b- defN 22-Jul-01 11:39 kolibri/indexers/base_indexer.py
--rw-r--r--  2.0 unx     3339 b- defN 22-Jul-06 14:24 kolibri/indexers/label_indexer.py
--rw-r--r--  2.0 unx     1248 b- defN 22-Jul-01 22:32 kolibri/indexers/multi_content_indexer.py
--rw-r--r--  2.0 unx     2394 b- defN 22-Jul-01 22:34 kolibri/indexers/multi_target_indexer.py
--rw-r--r--  2.0 unx     4944 b- defN 22-Jul-01 22:32 kolibri/indexers/sequence_char_indexer.py
--rw-r--r--  2.0 unx     4883 b- defN 22-Sep-22 22:51 kolibri/indexers/sequence_indexer.py
--rw-r--r--  2.0 unx     5940 b- defN 22-Nov-13 23:32 kolibri/indexers/text_indexer.py
--rw-r--r--  2.0 unx       43 b- defN 22-Sep-21 09:26 kolibri/knowledge/__init__.py
--rw-r--r--  2.0 unx     1173 b- defN 22-Sep-21 18:48 kolibri/knowledge/domain.py
--rw-r--r--  2.0 unx        0 b- defN 21-Sep-02 15:44 kolibri/optimizers/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 21-Sep-02 15:44 kolibri/optimizers/optuna/__init__.py
--rw-r--r--  2.0 unx    10410 b- defN 22-Dec-17 23:58 kolibri/optimizers/optuna/objective.py
--rw-r--r--  2.0 unx     2933 b- defN 22-Dec-18 10:03 kolibri/optimizers/optuna/tuner.py
--rw-r--r--  2.0 unx       49 b- defN 22-Sep-26 13:51 kolibri/output/__init__.py
--rw-r--r--  2.0 unx     3303 b- defN 22-Sep-27 13:39 kolibri/output/display.py
--rw-r--r--  2.0 unx     5694 b- defN 22-Sep-23 21:44 kolibri/output/display_backend.py
--rw-r--r--  2.0 unx     1637 b- defN 22-Sep-26 13:35 kolibri/output/display_component.py
--rw-r--r--  2.0 unx     4514 b- defN 22-Sep-26 13:35 kolibri/output/progress_bar.py
--rw-r--r--  2.0 unx       40 b- defN 22-Sep-27 15:59 kolibri/preprocess/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 22-Sep-16 15:26 kolibri/preprocess/preprocessors/__init__.py
--rw-r--r--  2.0 unx    14975 b- defN 22-Sep-16 15:26 kolibri/preprocess/preprocessors/bert_preprocessor.py
--rw-r--r--  2.0 unx     4942 b- defN 22-Sep-16 15:26 kolibri/preprocess/preprocessors/capitalization.py
--rw-r--r--  2.0 unx      596 b- defN 22-Sep-25 11:41 kolibri/preprocess/preprocessors/char_splitter.py
--rw-r--r--  2.0 unx     3356 b- defN 22-Sep-16 15:26 kolibri/preprocess/preprocessors/dirty_comments_preprocessor.py
--rw-r--r--  2.0 unx     1183 b- defN 22-Sep-25 11:49 kolibri/preprocess/preprocessors/mask.py
--rw-r--r--  2.0 unx     7324 b- defN 22-Sep-16 15:26 kolibri/preprocess/preprocessors/ner_preprocessor.py
--rw-r--r--  2.0 unx     6619 b- defN 22-Sep-16 15:26 kolibri/preprocess/preprocessors/odqa_preprocessors.py
--rw-r--r--  2.0 unx     1236 b- defN 22-Sep-16 15:26 kolibri/preprocess/preprocessors/random_embeddings_matrix.py
--rw-r--r--  2.0 unx    10390 b- defN 22-Sep-25 11:49 kolibri/preprocess/preprocessors/re_preprocessor.py
--rw-r--r--  2.0 unx     2501 b- defN 22-Sep-16 15:26 kolibri/preprocess/preprocessors/response_base_loader.py
--rw-r--r--  2.0 unx     2330 b- defN 22-Sep-25 11:55 kolibri/preprocess/preprocessors/sanitizer.py
--rw-r--r--  2.0 unx      574 b- defN 22-Sep-25 11:55 kolibri/preprocess/preprocessors/sentseg_preprocessor.py
--rw-r--r--  2.0 unx     5931 b- defN 22-Sep-25 11:55 kolibri/preprocess/preprocessors/siamese_preprocessor.py
--rw-r--r--  2.0 unx    20411 b- defN 22-Sep-16 15:26 kolibri/preprocess/preprocessors/squad_preprocessor.py
--rw-r--r--  2.0 unx     1883 b- defN 22-Sep-25 11:55 kolibri/preprocess/preprocessors/str_token_reverser.py
--rw-r--r--  2.0 unx     7566 b- defN 22-Sep-25 11:55 kolibri/preprocess/preprocessors/str_utf8_encoder.py
--rw-r--r--  2.0 unx     2657 b- defN 22-Sep-25 12:05 kolibri/preprocess/preprocessors/transformers_preprocessor.py
--rw-r--r--  2.0 unx     1624 b- defN 22-Dec-16 17:36 kolibri/preprocess/tabular/__init__.py
--rw-r--r--  2.0 unx     3030 b- defN 21-Nov-17 21:07 kolibri/preprocess/tabular/binning.py
--rw-r--r--  2.0 unx     8728 b- defN 21-Oct-01 14:04 kolibri/preprocess/tabular/boruta_py.py
--rw-r--r--  2.0 unx     5219 b- defN 21-Nov-17 21:50 kolibri/preprocess/tabular/cluster.py
--rw-r--r--  2.0 unx     1584 b- defN 22-Oct-11 15:18 kolibri/preprocess/tabular/columns_transfromer.py
--rw-r--r--  2.0 unx    11658 b- defN 22-Mar-20 01:26 kolibri/preprocess/tabular/data_imputer.py
--rw-r--r--  2.0 unx     2968 b- defN 21-Nov-22 18:01 kolibri/preprocess/tabular/dummy_converter.py
--rw-r--r--  2.0 unx    13109 b- defN 22-Oct-09 20:32 kolibri/preprocess/tabular/feature_interaction.py
--rw-r--r--  2.0 unx    10195 b- defN 22-Jan-10 22:17 kolibri/preprocess/tabular/feature_selection.py
--rw-r--r--  2.0 unx     3783 b- defN 21-Dec-04 21:57 kolibri/preprocess/tabular/infer_datatype.py
--rw-r--r--  2.0 unx    13298 b- defN 22-Mar-22 13:09 kolibri/preprocess/tabular/multicollinearity.py
--rw-r--r--  2.0 unx     4279 b- defN 22-Oct-05 07:21 kolibri/preprocess/tabular/normalize.py
--rw-r--r--  2.0 unx     2490 b- defN 22-Oct-19 13:50 kolibri/preprocess/tabular/one_hot_encoder_multi.py
--rw-r--r--  2.0 unx     1620 b- defN 21-Dec-30 19:38 kolibri/preprocess/tabular/ordinal_transformer.py
--rw-r--r--  2.0 unx     2616 b- defN 22-Mar-19 22:17 kolibri/preprocess/tabular/outlier_remover.py
--rw-r--r--  2.0 unx   149882 b- defN 22-Sep-26 13:47 kolibri/preprocess/tabular/preprocess.py
--rw-r--r--  2.0 unx    20154 b- defN 22-Mar-20 01:20 kolibri/preprocess/tabular/preprocessing_pipeline.py
--rw-r--r--  2.0 unx     3454 b- defN 22-Mar-22 13:09 kolibri/preprocess/tabular/rare_levels.py
--rw-r--r--  2.0 unx     8598 b- defN 21-Nov-17 22:13 kolibri/preprocess/tabular/reduce_cardinality.py
--rw-r--r--  2.0 unx     4848 b- defN 21-Dec-30 19:38 kolibri/preprocess/tabular/reduce_dimensionality.py
--rw-r--r--  2.0 unx     1801 b- defN 21-Nov-17 21:09 kolibri/preprocess/tabular/regression_target_transformer.py
--rw-r--r--  2.0 unx     2003 b- defN 21-Nov-17 21:04 kolibri/preprocess/tabular/similar_features.py
--rw-r--r--  2.0 unx     4003 b- defN 21-Dec-22 00:39 kolibri/preprocess/tabular/time_features_extractor.py
--rw-r--r--  2.0 unx     1808 b- defN 22-Mar-20 12:30 kolibri/preprocess/tabular/univar_outliers.py
--rw-r--r--  2.0 unx     3531 b- defN 22-Mar-22 13:09 kolibri/preprocess/tabular/zero_variance_remover.py
--rw-r--r--  2.0 unx       76 b- defN 22-Sep-25 16:02 kolibri/preprocess/text/__init__.py
--rw-r--r--  2.0 unx     4396 b- defN 22-Jun-17 10:45 kolibri/preprocess/text/collocation_analyzer.py
--rw-r--r--  2.0 unx     1412 b- defN 22-Jul-29 16:39 kolibri/preprocess/text/context_builder.py
--rw-r--r--  2.0 unx     1871 b- defN 22-Oct-16 09:08 kolibri/preprocess/text/email_cleaner.py
--rw-r--r--  2.0 unx     5288 b- defN 22-Oct-30 17:14 kolibri/preprocess/text/cleaning/__email_configs.py
--rw-r--r--  2.0 unx       67 b- defN 21-Oct-01 21:03 kolibri/preprocess/text/cleaning/__init__.py
--rw-r--r--  2.0 unx     4348 b- defN 22-Oct-30 19:42 kolibri/preprocess/text/cleaning/cleaning_scripts.py
--rw-r--r--  2.0 unx    23553 b- defN 22-Nov-04 15:05 kolibri/preprocess/text/cleaning/email2text.py
--rw-r--r--  2.0 unx     1425 b- defN 22-Oct-25 20:50 kolibri/preprocess/text/cleaning/email_parser.py
--rw-r--r--  2.0 unx     3279 b- defN 22-Nov-04 15:01 kolibri/preprocess/text/cleaning/header_parser.py
--rw-r--r--  2.0 unx       82 b- defN 21-Oct-01 21:03 kolibri/preprocess/text/language_detection/__init__.py
--rw-r--r--  2.0 unx     1420 b- defN 22-Oct-31 08:52 kolibri/preprocess/text/language_detection/lang_detect.py
--rw-r--r--  2.0 unx     7047 b- defN 21-Oct-01 21:03 kolibri/preprocess/text/translation/Translate_.py
--rw-r--r--  2.0 unx     1079 b- defN 21-Oct-01 21:03 kolibri/preprocess/text/translation/__init__.py
--rw-r--r--  2.0 unx     9890 b- defN 21-Oct-01 21:03 kolibri/preprocess/text/translation/client.py
--rw-r--r--  2.0 unx     9746 b- defN 21-Oct-01 21:03 kolibri/preprocess/text/translation/constants.py
--rw-r--r--  2.0 unx     1601 b- defN 21-Oct-01 21:03 kolibri/preprocess/text/translation/models.py
--rw-r--r--  2.0 unx     6090 b- defN 21-Oct-01 21:03 kolibri/preprocess/text/translation/translate.py
--rw-r--r--  2.0 unx     2640 b- defN 21-Oct-01 21:03 kolibri/preprocess/text/translation/utils.py
--rw-r--r--  2.0 unx       65 b- defN 22-Jan-01 21:19 kolibri/preprocess/timeseries/__init__.py
--rw-r--r--  2.0 unx    15014 b- defN 22-Aug-27 22:29 kolibri/preprocess/timeseries/multi_window_generator.py
--rw-r--r--  2.0 unx    10757 b- defN 22-Jul-21 10:02 kolibri/preprocess/timeseries/multi_window_generator_.py
--rw-r--r--  2.0 unx     7919 b- defN 22-Mar-04 17:08 kolibri/preprocess/timeseries/time_series_from_array.py
--rw-r--r--  2.0 unx     8504 b- defN 22-Mar-04 00:10 kolibri/preprocess/timeseries/window.py
--rw-r--r--  2.0 unx     7843 b- defN 22-Mar-06 17:26 kolibri/preprocess/timeseries/window_generator.py
--rw-r--r--  2.0 unx     2014 b- defN 22-Sep-25 13:38 kolibri/samplers/__init__.py
--rw-r--r--  2.0 unx     5095 b- defN 21-Oct-19 09:44 kolibri/samplers/auto_smpler.py
--rw-r--r--  2.0 unx       52 b- defN 21-Sep-02 15:44 kolibri/stopwords/__init__.py
--rw-r--r--  2.0 unx     2016 b- defN 22-Sep-13 05:39 kolibri/stopwords/stp_wrd.py
--rw-r--r--  2.0 unx       32 b- defN 22-Jul-02 22:37 kolibri/task/__init__.py
--rw-r--r--  2.0 unx      104 b- defN 22-Jan-20 18:52 kolibri/task/audio/__init__.py
--rw-r--r--  2.0 unx     9852 b- defN 22-Jan-21 09:01 kolibri/task/audio/base_model.py
--rw-r--r--  2.0 unx       75 b- defN 22-Jan-20 18:54 kolibri/task/audio/classification/__init__.py
--rw-r--r--  2.0 unx     3231 b- defN 22-Jul-07 12:42 kolibri/task/audio/classification/dnn_audio_estimator.py
--rw-r--r--  2.0 unx    10451 b- defN 22-Jan-20 18:54 kolibri/task/audio/classification/models.py
--rw-r--r--  2.0 unx        0 b- defN 22-Sep-16 15:26 kolibri/task/audio/nemo/__init__.py
--rw-r--r--  2.0 unx     7898 b- defN 22-Sep-16 15:26 kolibri/task/audio/nemo/asr.py
--rw-r--r--  2.0 unx     4329 b- defN 22-Sep-16 15:26 kolibri/task/audio/nemo/common.py
--rw-r--r--  2.0 unx     9128 b- defN 22-Sep-16 15:26 kolibri/task/audio/nemo/tts.py
--rw-r--r--  2.0 unx     5353 b- defN 22-Sep-16 15:26 kolibri/task/audio/nemo/vocoder.py
--rw-r--r--  2.0 unx       63 b- defN 22-Sep-27 16:01 kolibri/task/tabular/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 21-Dec-04 00:38 kolibri/task/tabular/anomaly/__init__.py
--rw-r--r--  2.0 unx     1437 b- defN 22-Jun-02 09:30 kolibri/task/tabular/anomaly/anomaly_estimator.py
--rw-r--r--  2.0 unx    18943 b- defN 22-Oct-31 12:46 kolibri/task/tabular/anomaly/half_space_trees.py
--rw-r--r--  2.0 unx      700 b- defN 22-Mar-26 18:39 kolibri/task/tabular/anomaly/models.py
--rw-r--r--  2.0 unx      742 b- defN 22-Jan-21 14:12 kolibri/task/tabular/anomaly/one_class_anomaly_dector.py
--rw-r--r--  2.0 unx     3274 b- defN 22-Jun-02 09:32 kolibri/task/tabular/anomaly/semi_supervised_anomaly_dector.py
--rw-r--r--  2.0 unx     4617 b- defN 22-Mar-25 10:42 kolibri/task/tabular/anomaly/unsupervised_anomaly_dector.py
--rw-r--r--  2.0 unx       74 b- defN 21-Oct-15 22:55 kolibri/task/tabular/clustering/__init__.py
--rw-r--r--  2.0 unx     4475 b- defN 22-Oct-08 10:01 kolibri/task/tabular/clustering/clustering.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-08 17:53 kolibri/task/tabular/regression/__init__.py
--rw-r--r--  2.0 unx     2094 b- defN 22-Dec-05 20:56 kolibri/task/tabular/regression/sklearn_regression_estimator.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-08 17:55 kolibri/task/tabular/rulemining/__init__.py
--rw-r--r--  2.0 unx     9912 b- defN 21-Oct-05 20:31 kolibri/task/tabular/rulemining/association_rules.py
--rw-r--r--  2.0 unx      140 b- defN 22-Oct-08 14:54 kolibri/task/text/__init__.py
--rw-r--r--  2.0 unx       94 b- defN 22-Oct-04 18:17 kolibri/task/text/classification/__init__.py
--rw-r--r--  2.0 unx     4243 b- defN 22-Sep-19 20:26 kolibri/task/text/classification/dnn_classification_estimator.py
--rw-r--r--  2.0 unx     3128 b- defN 22-Oct-08 23:58 kolibri/task/text/classification/sklearn_classification_estimator.py
--rw-r--r--  2.0 unx     3151 b- defN 22-Sep-24 21:28 kolibri/task/text/entities/__init__.py
--rw-r--r--  2.0 unx     1990 b- defN 22-Nov-04 18:50 kolibri/task/text/entities/common_reg_extractor.py
--rw-r--r--  2.0 unx    17418 b- defN 22-Nov-05 17:05 kolibri/task/text/entities/crf_entity_extractor.py
--rw-r--r--  2.0 unx      949 b- defN 22-Sep-24 21:28 kolibri/task/text/entities/dictionaryExtractor.py
--rw-r--r--  2.0 unx     4171 b- defN 22-Sep-24 21:26 kolibri/task/text/entities/entity_synonyms.py
--rw-r--r--  2.0 unx     6339 b- defN 22-Sep-24 21:26 kolibri/task/text/entities/lstm_entity_extractor.py
--rw-r--r--  2.0 unx     3633 b- defN 22-Sep-24 22:30 kolibri/task/text/entities/person_extractor.py
--rw-r--r--  2.0 unx     2279 b- defN 20-Feb-05 09:48 kolibri/task/text/entities/preprocessing.py
--rw-r--r--  2.0 unx     2668 b- defN 22-Sep-24 21:26 kolibri/task/text/entities/regex_extractor.py
--rw-r--r--  2.0 unx     6945 b- defN 22-Sep-24 21:33 kolibri/task/text/entities/templated_extractor.py
--rw-r--r--  2.0 unx     3498 b- defN 22-Nov-03 18:51 kolibri/task/text/entities/test.py
--rw-r--r--  2.0 unx        0 b- defN 21-Sep-20 22:05 kolibri/task/text/entities_back/__init__.py
--rw-r--r--  2.0 unx     6458 b- defN 22-Oct-16 09:08 kolibri/task/text/entities_back/common_reg_extractor.py
--rw-r--r--  2.0 unx    18309 b- defN 21-Oct-05 20:31 kolibri/task/text/entities_back/crf_entity_extractor.py
--rw-r--r--  2.0 unx     1011 b- defN 21-Dec-04 00:38 kolibri/task/text/entities_back/dictionaryExtractor.py
--rw-r--r--  2.0 unx     3003 b- defN 21-Sep-20 22:05 kolibri/task/text/entities_back/entity_extractor.py
--rw-r--r--  2.0 unx     4343 b- defN 21-May-13 22:26 kolibri/task/text/entities_back/entity_synonyms.py
--rw-r--r--  2.0 unx     3188 b- defN 22-Jun-11 23:47 kolibri/task/text/entities_back/person_extractor.py
--rw-r--r--  2.0 unx     2295 b- defN 21-Sep-23 23:05 kolibri/task/text/entities_back/preprocessing.py
--rw-r--r--  2.0 unx     2644 b- defN 21-Dec-04 00:38 kolibri/task/text/entities_back/regex_extractor.py
--rw-r--r--  2.0 unx     6419 b- defN 22-Jun-10 18:54 kolibri/task/text/entities_back/templated_extractor.py
--rw-r--r--  2.0 unx        5 b- defN 21-Oct-01 18:26 kolibri/task/text/intents/__init__.py
--rw-r--r--  2.0 unx    10307 b- defN 22-Sep-16 15:26 kolibri/task/text/intents/intent_catcher.py
--rw-r--r--  2.0 unx     3811 b- defN 22-Jun-02 09:06 kolibri/task/text/intents/intent_expressions.py
--rw-r--r--  2.0 unx     1437 b- defN 22-Jun-09 15:42 kolibri/task/text/intents/domains/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 22-Sep-16 15:26 kolibri/task/text/qa/__init__.py
--rw-r--r--  2.0 unx     8959 b- defN 22-Sep-16 15:26 kolibri/task/text/qa/entity_detection_parser.py
--rw-r--r--  2.0 unx    22335 b- defN 22-Sep-16 15:26 kolibri/task/text/qa/entity_linking.py
--rw-r--r--  2.0 unx    23543 b- defN 22-Sep-16 15:26 kolibri/task/text/qa/kbqa_entity_linking.py
--rw-r--r--  2.0 unx    12545 b- defN 22-Sep-16 15:26 kolibri/task/text/qa/query_generator.py
--rw-r--r--  2.0 unx    13495 b- defN 22-Sep-16 15:26 kolibri/task/text/qa/query_generator_base.py
--rw-r--r--  2.0 unx    10222 b- defN 22-Sep-16 15:26 kolibri/task/text/qa/query_generator_online.py
--rw-r--r--  2.0 unx     9552 b- defN 22-Sep-16 15:26 kolibri/task/text/qa/rel_ranking_bert_infer.py
--rw-r--r--  2.0 unx     3938 b- defN 22-Sep-16 15:26 kolibri/task/text/qa/rel_ranking_infer.py
--rw-r--r--  2.0 unx     7257 b- defN 22-Sep-16 15:26 kolibri/task/text/qa/sentence_answer.py
--rw-r--r--  2.0 unx     6657 b- defN 22-Sep-16 15:26 kolibri/task/text/qa/template_matcher.py
--rw-r--r--  2.0 unx    30317 b- defN 22-Sep-16 15:26 kolibri/task/text/qa/tree_to_sparql.py
--rw-r--r--  2.0 unx     6141 b- defN 22-Sep-16 15:26 kolibri/task/text/qa/utils.py
--rw-r--r--  2.0 unx    15627 b- defN 22-Sep-16 15:26 kolibri/task/text/qa/wiki_parser.py
--rw-r--r--  2.0 unx     4572 b- defN 22-Sep-16 15:26 kolibri/task/text/qa/wiki_parser_online.py
--rw-r--r--  2.0 unx        0 b- defN 22-Sep-16 15:26 kolibri/task/text/qa/squad/__init__.py
--rw-r--r--  2.0 unx    16890 b- defN 22-Sep-16 15:26 kolibri/task/text/qa/squad/squad.py
--rw-r--r--  2.0 unx    10294 b- defN 22-Sep-16 15:26 kolibri/task/text/qa/squad/utils.py
--rw-r--r--  2.0 unx        0 b- defN 22-Sep-16 15:26 kolibri/task/text/relations/__init__.py
--rw-r--r--  2.0 unx     2434 b- defN 22-Sep-16 15:26 kolibri/task/text/relations/losses.py
--rw-r--r--  2.0 unx     6541 b- defN 22-Sep-25 12:15 kolibri/task/text/relations/relation_extraction_bert.py
--rw-r--r--  2.0 unx        0 b- defN 22-Sep-16 15:26 kolibri/task/text/retrieval/__init__.py
--rw-r--r--  2.0 unx     6170 b- defN 22-Sep-25 12:15 kolibri/task/text/retrieval/logit_ranker.py
--rw-r--r--  2.0 unx     3537 b- defN 22-Oct-31 12:46 kolibri/task/text/retrieval/pop_ranker.py
--rw-r--r--  2.0 unx     2326 b- defN 22-Sep-25 12:15 kolibri/task/text/retrieval/tfidf_ranker.py
--rw-r--r--  2.0 unx      631 b- defN 22-Sep-25 12:09 kolibri/task/text/retrieval/utils.py
--rw-r--r--  2.0 unx        1 b- defN 22-Jun-11 23:14 kolibri/task/text/sentiment/__init__.py
--rw-r--r--  2.0 unx    12971 b- defN 22-Jun-13 12:29 kolibri/task/text/sentiment/lexicon_sentiment.py
--rw-r--r--  2.0 unx    32780 b- defN 22-Jun-13 21:11 kolibri/task/text/sentiment/util.py
--rw-r--r--  2.0 unx    22769 b- defN 22-Jun-18 22:58 kolibri/task/text/sentiment/vader.py
--rw-r--r--  2.0 unx        0 b- defN 22-Sep-16 15:26 kolibri/task/text/spelling/__init__.py
--rw-r--r--  2.0 unx       36 b- defN 22-Sep-16 15:26 kolibri/task/text/spelling/brillmoore/__init__.py
--rw-r--r--  2.0 unx    10846 b- defN 22-Sep-16 15:26 kolibri/task/text/spelling/brillmoore/error_model.py
--rw-r--r--  2.0 unx        0 b- defN 22-Sep-16 15:26 kolibri/task/text/spelling/electors/__init__.py
--rw-r--r--  2.0 unx     2861 b- defN 22-Sep-16 15:26 kolibri/task/text/spelling/electors/kenlm_elector.py
--rw-r--r--  2.0 unx     1446 b- defN 22-Sep-16 15:26 kolibri/task/text/spelling/electors/top1_elector.py
--rw-r--r--  2.0 unx       61 b- defN 22-Sep-16 15:26 kolibri/task/text/spelling/levenshtein/__init__.py
--rw-r--r--  2.0 unx    33386 b- defN 22-Sep-16 15:26 kolibri/task/text/spelling/levenshtein/levenshtein_searcher.py
--rw-r--r--  2.0 unx     3423 b- defN 22-Sep-16 15:26 kolibri/task/text/spelling/levenshtein/searcher_component.py
--rw-r--r--  2.0 unx    20586 b- defN 22-Sep-16 15:26 kolibri/task/text/spelling/levenshtein/tabled_trie.py
--rw-r--r--  2.0 unx      152 b- defN 22-Oct-08 14:57 kolibri/task/text/topics/__init__.py
--rw-r--r--  2.0 unx     3563 b- defN 22-Nov-13 22:39 kolibri/task/text/topics/baseTopic.py
--rw-r--r--  2.0 unx    24958 b- defN 22-Nov-13 22:41 kolibri/task/text/topics/mallet.py
--rw-r--r--  2.0 unx    14976 b- defN 22-Nov-13 22:53 kolibri/task/text/topics/topics_estimator.py
--rw-r--r--  2.0 unx       58 b- defN 22-Jan-01 21:20 kolibri/task/timeseries/__init__.py
--rw-r--r--  2.0 unx    23782 b- defN 22-Jan-17 00:01 kolibri/task/timeseries/dataset.py
--rw-r--r--  2.0 unx      962 b- defN 21-Sep-05 19:06 kolibri/task/timeseries/metrics.py
--rw-r--r--  2.0 unx     1953 b- defN 22-Jan-01 21:39 kolibri/task/timeseries/analysis/__init__.py
--rw-r--r--  2.0 unx     7234 b- defN 22-Jan-01 23:32 kolibri/task/timeseries/analysis/eda_utils.py
--rw-r--r--  2.0 unx    17003 b- defN 22-Jan-02 16:26 kolibri/task/timeseries/analysis/plotters.py
--rw-r--r--  2.0 unx      494 b- defN 22-Jan-01 22:01 kolibri/task/timeseries/analysis/feature_relevance/__init__.py
--rw-r--r--  2.0 unx     3066 b- defN 22-Jan-01 22:03 kolibri/task/timeseries/analysis/feature_relevance/relevance.py
--rw-r--r--  2.0 unx     2919 b- defN 22-Jan-01 22:02 kolibri/task/timeseries/analysis/feature_relevance/relevance_table.py
--rw-r--r--  2.0 unx      583 b- defN 22-Jan-01 21:39 kolibri/task/timeseries/analysis/outliers/__init__.py
--rw-r--r--  2.0 unx     5017 b- defN 22-Jan-02 16:39 kolibri/task/timeseries/analysis/outliers/density_outliers.py
--rw-r--r--  2.0 unx    13178 b- defN 22-Jan-01 21:47 kolibri/task/timeseries/analysis/outliers/hist_outliers.py
--rw-r--r--  2.0 unx     1878 b- defN 22-Jan-02 01:18 kolibri/task/timeseries/analysis/outliers/median_outliers.py
--rw-r--r--  2.0 unx     2998 b- defN 22-Jan-01 21:47 kolibri/task/timeseries/analysis/outliers/prediction_interval_outliers.py
--rw-r--r--  2.0 unx     3501 b- defN 22-Jan-02 17:47 kolibri/task/timeseries/analysis/outliers/sequence_outliers.py
--rw-r--r--  2.0 unx     1411 b- defN 22-Jul-25 21:34 kolibri/tokenizers/__init__.py
--rw-r--r--  2.0 unx     4709 b- defN 22-Sep-25 12:05 kolibri/tokenizers/bert_tokenizer.py
--rw-r--r--  2.0 unx     3999 b- defN 22-Dec-10 18:37 kolibri/tokenizers/char_tokenizer.py
--rw-r--r--  2.0 unx     7103 b- defN 22-Dec-10 18:37 kolibri/tokenizers/kolibri_tokenizer.py
--rw-r--r--  2.0 unx     2361 b- defN 22-Dec-10 18:37 kolibri/tokenizers/multi_word_tokenizer.py
--rw-r--r--  2.0 unx     2661 b- defN 22-Jul-01 23:11 kolibri/tokenizers/regex_tokenizer.py
--rw-r--r--  2.0 unx     1025 b- defN 22-Dec-10 18:37 kolibri/tokenizers/sentence_tokenizer.py
--rw-r--r--  2.0 unx     2708 b- defN 22-Dec-10 22:33 kolibri/tokenizers/tokenizer.py
--rw-r--r--  2.0 unx     6936 b- defN 22-Sep-13 05:47 kolibri/tokenizers/ugc_tokenizer.py
--rw-r--r--  2.0 unx     2340 b- defN 22-Dec-10 18:35 kolibri/tokenizers/word_tokenizer.py
--rw-r--r--  2.0 unx        0 b- defN 19-Sep-30 15:55 kolibri/tools/__init__.py
--rw-r--r--  2.0 unx      411 b- defN 21-Sep-29 21:43 kolibri/tools/_regex.py
--rw-r--r--  2.0 unx     2063 b- defN 21-Oct-24 15:26 kolibri/tools/gebbrisg_detector.py
--rw-r--r--  2.0 unx    25525 b- defN 21-Mar-12 11:04 kolibri/tools/keywords.py
--rw-r--r--  2.0 unx     1828 b- defN 22-Sep-13 05:47 kolibri/tools/regexes.py
--rw-r--r--  2.0 unx    17263 b- defN 22-Nov-04 00:23 kolibri/tools/scanner.py
--rw-r--r--  2.0 unx    13056 b- defN 22-Sep-25 10:47 kolibri/tools/word_frequencies.py
--rw-r--r--  2.0 unx     1754 b- defN 22-Dec-03 18:26 kolibri/utils/__init__.py
--rw-r--r--  2.0 unx    11174 b- defN 22-Sep-28 23:58 kolibri/utils/cm.py
--rw-r--r--  2.0 unx     6589 b- defN 22-Oct-04 09:50 kolibri/utils/common.py
--rw-r--r--  2.0 unx     3173 b- defN 22-Jul-01 10:58 kolibri/utils/config.py
--rw-r--r--  2.0 unx    11887 b- defN 22-Oct-05 20:55 kolibri/utils/cross_validation.py
--rw-r--r--  2.0 unx    14474 b- defN 22-Aug-27 18:17 kolibri/utils/distribution.py
--rw-r--r--  2.0 unx      544 b- defN 22-Mar-18 17:31 kolibri/utils/log_normalizer.py
--rw-r--r--  2.0 unx    28841 b- defN 22-Aug-09 13:07 kolibri/utils/timeseries_functions.py
--rw-r--r--  2.0 unx        0 b- defN 22-Sep-28 08:03 kolibri/visualizations/__init__.py
--rw-r--r--  2.0 unx    53405 b- defN 22-Oct-31 16:06 kolibri/visualizations/classification_plots.py
--rw-r--r--  2.0 unx    15746 b- defN 22-Sep-29 12:36 kolibri/visualizations/pipeline.py
--rw-r--r--  2.0 unx    34339 b- defN 22-Nov-03 14:46 kolibri/visualizations/regression_plots.py
--rw-r--r--  2.0 unx    15565 b- defN 22-Oct-06 14:17 kolibri/visualizations/utils.py
--rw-r--r--  2.0 unx        0 b- defN 22-Sep-27 15:51 test_backup/__init__.py
--rw-r--r--  2.0 unx     2623 b- defN 22-Jan-20 18:51 test_backup/dnn/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 22-Sep-27 15:51 test_backup/dnn/audio/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 22-Sep-27 15:51 test_backup/dnn/audio/test_classification/__init__.py
--rw-r--r--  2.0 unx     2435 b- defN 22-Jan-20 18:54 test_backup/dnn/audio/test_classification/test_pipeline_model.py
--rw-r--r--  2.0 unx        0 b- defN 20-Jul-28 11:13 test_backup/dnn/text/__init__.py
--rw-r--r--  2.0 unx      176 b- defN 20-Jul-05 12:31 test_backup/dnn/text/test_classification/__init__.py
--rw-r--r--  2.0 unx      575 b- defN 22-Jan-20 18:54 test_backup/dnn/text/test_classification/test_bi_gru_model.py
--rw-r--r--  2.0 unx     4129 b- defN 22-Jan-21 13:49 test_backup/dnn/text/test_classification/test_bi_lstm_model.py
--rw-r--r--  2.0 unx      718 b- defN 22-Jan-20 18:54 test_backup/dnn/text/test_classification/test_cnn_attention_model.py
--rw-r--r--  2.0 unx      581 b- defN 22-Jan-20 18:54 test_backup/dnn/text/test_classification/test_cnn_gru_model.py
--rw-r--r--  2.0 unx      584 b- defN 22-Jan-20 18:54 test_backup/dnn/text/test_classification/test_cnn_lstm_model.py
--rw-r--r--  2.0 unx      571 b- defN 22-Jan-20 18:54 test_backup/dnn/text/test_classification/test_cnn_model.py
--rw-r--r--  2.0 unx       36 b- defN 20-Aug-03 11:50 test_backup/dnn/text/test_embeddings/__init__.py
--rw-r--r--  2.0 unx     2235 b- defN 22-Jan-21 08:26 test_backup/dnn/text/test_embeddings/test_default_embedding.py
--rw-r--r--  2.0 unx      819 b- defN 22-Jul-07 12:43 test_backup/dnn/text/test_embeddings/test_word_embedding.py
--rw-r--r--  2.0 unx       36 b- defN 20-Aug-03 11:50 test_backup/dnn/text/test_indexer/__init__.py
--rw-r--r--  2.0 unx     1692 b- defN 22-Jan-20 21:42 test_backup/dnn/text/test_indexer/test_label_indexer.py
--rw-r--r--  2.0 unx     1149 b- defN 22-Jan-20 21:52 test_backup/dnn/text/test_indexer/test_multi_content_indexer.py
--rw-r--r--  2.0 unx     1618 b- defN 22-Jan-21 08:25 test_backup/dnn/text/test_indexer/test_multi_target_indexer.py
--rw-r--r--  2.0 unx     1040 b- defN 22-Jan-21 00:45 test_backup/dnn/text/test_indexer/test_sequence_char_indexer.py
--rw-r--r--  2.0 unx     2080 b- defN 22-Jan-21 08:25 test_backup/dnn/text/test_indexer/test_sequence_indexer.py
--rw-r--r--  2.0 unx       55 b- defN 20-Jul-28 11:54 test_backup/dnn/text/test_labeling/__init__.py
--rw-r--r--  2.0 unx     1642 b- defN 22-Jan-20 18:54 test_backup/dnn/text/test_labeling/test_bi_gru_model.py
--rw-r--r--  2.0 unx      375 b- defN 22-Jan-20 18:54 test_backup/dnn/text/test_labeling/test_bi_lstm_crf_model.py
--rw-r--r--  2.0 unx     2738 b- defN 22-Jan-20 18:54 test_backup/dnn/text/test_labeling/test_bi_lstm_model.py
--rw-r--r--  2.0 unx      371 b- defN 22-Jan-20 18:54 test_backup/dnn/text/test_labeling/test_cnn_lstm_model.py
--rw-r--r--  2.0 unx       36 b- defN 20-Aug-03 11:50 test_backup/dnn/text/test_seq2seq/__init__.py
--rw-r--r--  2.0 unx      889 b- defN 22-May-11 08:02 test_backup/dnn/text/test_seq2seq/test_seq2seq.py
--rw-r--r--  2.0 unx        0 b- defN 21-Sep-20 15:17 test_backup/entities/__init__.py
--rw-r--r--  2.0 unx     7837 b- defN 22-Jun-11 23:47 test_backup/entities/test.py
--rw-r--r--  2.0 unx        0 b- defN 20-Oct-01 22:47 test_backup/optuna/__init__.py
--rw-r--r--  2.0 unx        1 b- defN 21-Sep-29 12:49 test_backup/optuna/test_optuna.py
--rw-r--r--  2.0 unx     4594 b- defN 22-Dec-18 21:22 kolibri_ml-1.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Dec-18 21:22 kolibri_ml-1.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 22-Dec-18 21:22 kolibri_ml-1.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    49239 b- defN 22-Dec-18 21:22 kolibri_ml-1.1.8.dist-info/RECORD
-492 files, 3084358 bytes uncompressed, 816077 bytes compressed:  73.5%
+Zip file size: 1295974 bytes, number of entries: 699
+-rw-r--r--  2.0 unx       18 b- defN 23-Aug-03 22:02 kolibri/.env
+-rw-r--r--  2.0 unx        7 b- defN 23-Aug-05 18:43 kolibri/VERSION
+-rw-r--r--  2.0 unx     4358 b- defN 23-Aug-03 20:53 kolibri/__init__.py
+-rw-r--r--  2.0 unx    16782 b- defN 23-Jul-09 11:29 kolibri/app.py
+-rw-r--r--  2.0 unx     3190 b- defN 23-Jul-09 11:29 kolibri/config.py
+-rw-r--r--  2.0 unx     1902 b- defN 23-Jul-09 11:29 kolibri/config_loader.py
+-rw-r--r--  2.0 unx     3814 b- defN 23-Aug-03 22:27 kolibri/default_configs.py
+-rw-r--r--  2.0 unx     5968 b- defN 23-Aug-03 20:53 kolibri/errors.py
+-rw-r--r--  2.0 unx      795 b- defN 23-Jul-09 11:29 kolibri/logger.py
+-rw-r--r--  2.0 unx     2219 b- defN 23-Jul-09 11:29 kolibri/metadata.py
+-rw-r--r--  2.0 unx    10923 b- defN 23-Jul-09 11:29 kolibri/model_loader.py
+-rw-r--r--  2.0 unx    25966 b- defN 23-Jul-09 11:29 kolibri/model_trainer.py
+-rw-r--r--  2.0 unx     2763 b- defN 23-Jul-09 11:29 kolibri/registry.py
+-rw-r--r--  2.0 unx      153 b- defN 23-Jul-09 11:29 kolibri/requirements.txt
+-rw-r--r--  2.0 unx     2490 b- defN 23-Jul-09 11:29 kolibri/settings.py
+-rw-r--r--  2.0 unx      457 b- defN 23-Jul-09 11:29 kolibri/settings.yaml
+-rw-r--r--  2.0 unx      361 b- defN 23-Jul-09 11:29 kolibri/types.py
+-rw-r--r--  2.0 unx      166 b- defN 23-Jul-09 11:29 kolibri/version.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-03 20:53 kolibri/api/__init__.py
+-rw-r--r--  2.0 unx     2707 b- defN 23-Aug-03 20:53 kolibri/api/classification/__init__.py
+-rw-r--r--  2.0 unx       66 b- defN 23-Jul-09 11:29 kolibri/autolearn/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/autolearn/metalearn/__init__.py
+-rw-r--r--  2.0 unx     3125 b- defN 23-Jul-09 11:29 kolibri/autolearn/metalearn/metafeature.py
+-rw-r--r--  2.0 unx    46866 b- defN 23-Jul-09 11:29 kolibri/autolearn/metalearn/metafeatures.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/autolearn/model_zoo/__init__.py
+-rw-r--r--  2.0 unx     4737 b- defN 23-Aug-03 20:53 kolibri/autolearn/model_zoo/zoo_classifier.py
+-rw-r--r--  2.0 unx     5940 b- defN 23-Jul-09 11:29 kolibri/autolearn/model_zoo/zoo_estimator.py
+-rw-r--r--  2.0 unx     4246 b- defN 23-Jul-09 11:29 kolibri/autolearn/model_zoo/zoo_regressor.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/automl/__init__.py
+-rw-r--r--  2.0 unx    15341 b- defN 23-Jul-09 11:29 kolibri/automl/data_inspection.py
+-rw-r--r--  2.0 unx       50 b- defN 23-Jul-09 11:29 kolibri/backend/__init__.py
+-rw-r--r--  2.0 unx     6230 b- defN 23-Jul-09 11:29 kolibri/backend/models.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/backend/base/__init__.py
+-rw-r--r--  2.0 unx    11843 b- defN 23-Jul-09 11:29 kolibri/backend/base/base_classifier.py
+-rw-r--r--  2.0 unx     3916 b- defN 23-Jul-09 11:29 kolibri/backend/base/base_clustering.py
+-rw-r--r--  2.0 unx    30869 b- defN 23-Jul-09 11:29 kolibri/backend/base/base_estimator.py
+-rw-r--r--  2.0 unx     7677 b- defN 23-Jul-09 11:29 kolibri/backend/base/base_regressor.py
+-rw-r--r--  2.0 unx    14321 b- defN 23-Jul-09 11:29 kolibri/backend/base/estimator.py
+-rw-r--r--  2.0 unx      912 b- defN 23-Jul-09 11:29 kolibri/backend/base/nn_model.py
+-rw-r--r--  2.0 unx      449 b- defN 23-Jul-09 11:29 kolibri/backend/bn/BayesianModel.py
+-rw-r--r--  2.0 unx    44071 b- defN 23-Jul-09 11:29 kolibri/backend/bn/BayesianNetwork.py
+-rw-r--r--  2.0 unx    24029 b- defN 23-Jul-09 11:29 kolibri/backend/bn/CPD.py
+-rw-r--r--  2.0 unx     8931 b- defN 23-Jul-09 11:29 kolibri/backend/bn/ContinuousFactor.py
+-rw-r--r--  2.0 unx    40531 b- defN 23-Jul-09 11:29 kolibri/backend/bn/DAG.py
+-rw-r--r--  2.0 unx    28630 b- defN 23-Jul-09 11:29 kolibri/backend/bn/DiscreteFactor.py
+-rw-r--r--  2.0 unx    31370 b- defN 23-Jul-09 11:29 kolibri/backend/bn/DynamicBayesianNetwork.py
+-rw-r--r--  2.0 unx     4289 b- defN 23-Jul-09 11:29 kolibri/backend/bn/EliminationOrder.py
+-rw-r--r--  2.0 unx    39930 b- defN 23-Jul-09 11:29 kolibri/backend/bn/ExactInference.py
+-rw-r--r--  2.0 unx    10515 b- defN 23-Jul-09 11:29 kolibri/backend/bn/FactorGraph.py
+-rw-r--r--  2.0 unx    14252 b- defN 23-Jul-09 11:29 kolibri/backend/bn/Independencies.py
+-rw-r--r--  2.0 unx    11089 b- defN 23-Jul-09 11:29 kolibri/backend/bn/JointProbabilityDistribution.py
+-rw-r--r--  2.0 unx     3058 b- defN 23-Jul-09 11:29 kolibri/backend/bn/JunctionTree.py
+-rw-r--r--  2.0 unx     8219 b- defN 23-Jul-09 11:29 kolibri/backend/bn/LinearGaussianCPD.py
+-rw-r--r--  2.0 unx    13783 b- defN 23-Jul-09 11:29 kolibri/backend/bn/MarkovChain.py
+-rw-r--r--  2.0 unx    17804 b- defN 23-Jul-09 11:29 kolibri/backend/bn/MarkovNetwork.py
+-rw-r--r--  2.0 unx     5791 b- defN 23-Jul-09 11:29 kolibri/backend/bn/NaiveBayes.py
+-rw-r--r--  2.0 unx    24083 b- defN 23-Jul-09 11:29 kolibri/backend/bn/Sampling.py
+-rw-r--r--  2.0 unx     9237 b- defN 23-Jul-09 11:29 kolibri/backend/bn/UndirectedGraph.py
+-rw-r--r--  2.0 unx      723 b- defN 23-Jul-09 11:29 kolibri/backend/bn/__init__.py
+-rw-r--r--  2.0 unx    11145 b- defN 23-Jul-09 11:29 kolibri/backend/bn/base_estimator.py
+-rw-r--r--  2.0 unx     7604 b- defN 23-Jul-09 11:29 kolibri/backend/bn/base_inference.py
+-rw-r--r--  2.0 unx    48039 b- defN 23-Jul-09 11:29 kolibri/backend/bn/bnlearn.py
+-rw-r--r--  2.0 unx     3207 b- defN 23-Jul-09 11:29 kolibri/backend/bn/factors_base.py
+-rw-r--r--  2.0 unx     2348 b- defN 23-Jul-09 11:29 kolibri/backend/bn/metrics.py
+-rw-r--r--  2.0 unx    16476 b- defN 23-Jul-09 11:29 kolibri/backend/bn/network.py
+-rw-r--r--  2.0 unx     3178 b- defN 23-Jul-09 11:29 kolibri/backend/bn/state_name.py
+-rw-r--r--  2.0 unx    30222 b- defN 23-Jul-09 11:29 kolibri/backend/bn/tabulate.py
+-rw-r--r--  2.0 unx     5326 b- defN 23-Jul-09 11:29 kolibri/backend/bn/utils.py
+-rw-r--r--  2.0 unx    13476 b- defN 23-Jul-09 11:29 kolibri/backend/bn/distributions/CanonicalDistribution.py
+-rw-r--r--  2.0 unx    11847 b- defN 23-Jul-09 11:29 kolibri/backend/bn/distributions/CustomDistribution.py
+-rw-r--r--  2.0 unx    19195 b- defN 23-Jul-09 11:29 kolibri/backend/bn/distributions/GaussianDistribution.py
+-rw-r--r--  2.0 unx      220 b- defN 23-Jul-09 11:29 kolibri/backend/bn/distributions/__init__.py
+-rw-r--r--  2.0 unx      841 b- defN 23-Jul-09 11:29 kolibri/backend/bn/distributions/base.py
+-rw-r--r--  2.0 unx    12715 b- defN 23-Jul-09 11:29 kolibri/backend/bn/estimators/HillClimbSearch.py
+-rw-r--r--  2.0 unx     4805 b- defN 23-Jul-09 11:29 kolibri/backend/bn/estimators/MLE.py
+-rw-r--r--  2.0 unx     4221 b- defN 23-Jul-09 11:29 kolibri/backend/bn/estimators/ScoreCache.py
+-rw-r--r--  2.0 unx    18012 b- defN 23-Jul-09 11:29 kolibri/backend/bn/estimators/StructureScore.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/backend/bn/estimators/__init__.py
+-rw-r--r--  2.0 unx     7985 b- defN 23-Jul-09 11:29 kolibri/backend/bn/estimators/bayesianEstimator.py
+-rw-r--r--  2.0 unx       57 b- defN 23-Jul-09 11:29 kolibri/backend/bn/inference/__init__.py
+-rw-r--r--  2.0 unx     3044 b- defN 23-Jul-09 11:29 kolibri/backend/bn/inference/inference.py
+-rw-r--r--  2.0 unx      194 b- defN 23-Jul-09 11:29 kolibri/backend/bn/inference/predict.py
+-rw-r--r--  2.0 unx      130 b- defN 23-Jul-09 11:29 kolibri/backend/bn/parameters/__init__.py
+-rw-r--r--  2.0 unx      490 b- defN 23-Jul-09 11:29 kolibri/backend/bn/parameters/learn.py
+-rw-r--r--  2.0 unx    12213 b- defN 23-Jul-09 11:29 kolibri/backend/bn/parameters/parameter_learning.py
+-rw-r--r--  2.0 unx    18288 b- defN 23-Jul-09 11:29 kolibri/backend/bn/readwrite/BIF.py
+-rw-r--r--  2.0 unx    14034 b- defN 23-Jul-09 11:29 kolibri/backend/bn/readwrite/UAI.py
+-rw-r--r--  2.0 unx    16390 b- defN 23-Jul-09 11:29 kolibri/backend/bn/readwrite/XMLBIF.py
+-rw-r--r--  2.0 unx      491 b- defN 23-Jul-09 11:29 kolibri/backend/bn/readwrite/__init__.py
+-rw-r--r--  2.0 unx      311 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/__init__.py
+-rw-r--r--  2.0 unx     7020 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/base.py
+-rw-r--r--  2.0 unx     8354 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/evaluation.py
+-rw-r--r--  2.0 unx     1989 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/learn.py
+-rw-r--r--  2.0 unx     7267 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/linear.py
+-rw-r--r--  2.0 unx     7902 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/low_rank.py
+-rw-r--r--  2.0 unx    22607 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/no_tears.py
+-rw-r--r--  2.0 unx     2961 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/no_tears_tf.py
+-rw-r--r--  2.0 unx     1898 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/no_tears_tf2.py
+-rw-r--r--  2.0 unx     2961 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/no_tears_tf_bak.py
+-rw-r--r--  2.0 unx     8816 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/nonlinear.py
+-rw-r--r--  2.0 unx     4376 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/notears_tf2.py
+-rw-r--r--  2.0 unx     4208 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/plot_dag.py
+-rw-r--r--  2.0 unx    13671 b- defN 23-Jul-09 11:29 kolibri/backend/bn/structure/structure_model.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/backend/generators/__init__.py
+-rw-r--r--  2.0 unx      157 b- defN 23-Jul-09 11:29 kolibri/backend/sklearn/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/backend/sklearn/extensions/__init__.py
+-rw-r--r--  2.0 unx    18744 b- defN 23-Jul-09 11:29 kolibri/backend/sklearn/extensions/decision_tree_log_reg.py
+-rw-r--r--  2.0 unx     1100 b- defN 23-Jul-09 11:29 kolibri/backend/sklearn/extensions/distributed_nn.py
+-rw-r--r--  2.0 unx    15651 b- defN 23-Jul-09 11:29 kolibri/backend/sklearn/extensions/lazy_learner.py
+-rw-r--r--  2.0 unx    14524 b- defN 23-Jul-09 11:29 kolibri/backend/sklearn/extensions/lookup_learner.py
+-rw-r--r--  2.0 unx       65 b- defN 23-Jul-09 11:29 kolibri/backend/sklearn/meta/__init__.py
+-rw-r--r--  2.0 unx    13257 b- defN 23-Jul-09 11:29 kolibri/backend/sklearn/meta/chain_model.py
+-rw-r--r--  2.0 unx    28317 b- defN 23-Jul-09 11:29 kolibri/backend/sklearn/meta/ecoc_model.py
+-rw-r--r--  2.0 unx    28328 b- defN 23-Jul-09 11:29 kolibri/backend/sklearn/meta/ensemble_samplers.py
+-rw-r--r--  2.0 unx     7646 b- defN 23-Jul-09 11:29 kolibri/backend/sklearn/meta/multi_output_estimator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/backend/sklearn/meta/ecoc/__init__.py
+-rw-r--r--  2.0 unx     8616 b- defN 23-Jul-09 11:29 kolibri/backend/sklearn/meta/ecoc/code_matrix.py
+-rw-r--r--  2.0 unx     5551 b- defN 23-Jul-09 11:29 kolibri/backend/sklearn/meta/ecoc/criterion.py
+-rw-r--r--  2.0 unx     9095 b- defN 23-Jul-09 11:29 kolibri/backend/sklearn/meta/ecoc/decoder.py
+-rw-r--r--  2.0 unx     3869 b- defN 23-Jul-09 11:29 kolibri/backend/sklearn/meta/ecoc/sffs.py
+-rw-r--r--  2.0 unx     2953 b- defN 23-Aug-03 20:53 kolibri/backend/tensorflow/__init__.py
+-rw-r--r--  2.0 unx      519 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/logger.py
+-rw-r--r--  2.0 unx      308 b- defN 23-Aug-03 20:53 kolibri/backend/tensorflow/macros.py
+-rw-r--r--  2.0 unx      457 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/autoencoder/__init__.py
+-rw-r--r--  2.0 unx     6848 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/autoencoder/base_autoencoder.py
+-rw-r--r--  2.0 unx     3339 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/autoencoder/conv_autoencoder.py
+-rw-r--r--  2.0 unx     2611 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/autoencoder/deep_autoencoder.py
+-rw-r--r--  2.0 unx     3757 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/autoencoder/variational_autoencoder.py
+-rw-r--r--  2.0 unx      204 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/autoencoder/decoders/__init__.py
+-rw-r--r--  2.0 unx     2091 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/autoencoder/decoders/att_gru_decoder.py
+-rw-r--r--  2.0 unx     1294 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/autoencoder/decoders/gru_decoder.py
+-rw-r--r--  2.0 unx     1213 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/autoencoder/decoders/lstm_decoder.py
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/autoencoder/encoders/__init__.py
+-rw-r--r--  2.0 unx     1257 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/autoencoder/encoders/gru_encoder.py
+-rw-r--r--  2.0 unx     1383 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/autoencoder/encoders/lstm_encoder.py
+-rw-r--r--  2.0 unx      134 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/callbacks/__init__.py
+-rw-r--r--  2.0 unx     2025 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/callbacks/conll_call_back.py
+-rw-r--r--  2.0 unx     2241 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/callbacks/eval_callBack.py
+-rw-r--r--  2.0 unx     4874 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/callbacks/save_callback.py
+-rw-r--r--  2.0 unx      320 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/__init__.py
+-rw-r--r--  2.0 unx     1709 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/bare_embedding.py
+-rw-r--r--  2.0 unx     4676 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/base_embedding.py
+-rw-r--r--  2.0 unx     1322 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/bert_embedding.py
+-rw-r--r--  2.0 unx     8420 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/elmo_embedding.py
+-rw-r--r--  2.0 unx     3196 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/embedding_trainer.py
+-rw-r--r--  2.0 unx     1952 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/fasttext_embedding.py
+-rw-r--r--  2.0 unx     2568 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/glove_embedding.py
+-rw-r--r--  2.0 unx     9637 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/loader.py
+-rw-r--r--  2.0 unx    14296 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/loader_albert.py
+-rw-r--r--  2.0 unx     4114 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/numeric_feature_embedding.py
+-rw-r--r--  2.0 unx     4911 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/stacked_embedding.py
+-rw-r--r--  2.0 unx     3830 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/transformer_embedding.py
+-rw-r--r--  2.0 unx     3346 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/embeddings/word_embedding.py
+-rw-r--r--  2.0 unx      679 b- defN 23-Aug-03 20:53 kolibri/backend/tensorflow/gan/__init__.py
+-rw-r--r--  2.0 unx    15332 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/gan/_transformer.py
+-rw-r--r--  2.0 unx      462 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/gan/bgm.py
+-rw-r--r--  2.0 unx     3406 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/gan/discriminator.py
+-rw-r--r--  2.0 unx     2727 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/gan/generator.py
+-rw-r--r--  2.0 unx      412 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/gan/ohe.py
+-rw-r--r--  2.0 unx     1015 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/layers/__init__.py
+-rw-r--r--  2.0 unx     3258 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/layers/att_wgt_avg_layer.py
+-rw-r--r--  2.0 unx     1528 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/layers/behdanau_attention.py
+-rw-r--r--  2.0 unx     4389 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/layers/conditional_random_field.py
+-rw-r--r--  2.0 unx     1047 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/layers/folding_layer.py
+-rw-r--r--  2.0 unx     4173 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/layers/gen_activation.py
+-rw-r--r--  2.0 unx     2033 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/layers/highway_layer.py
+-rw-r--r--  2.0 unx     3088 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/layers/kmax_pool_layer.py
+-rw-r--r--  2.0 unx     1129 b- defN 23-Aug-03 20:53 kolibri/backend/tensorflow/layers/layer_utils.py
+-rw-r--r--  2.0 unx     5012 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/layers/multi_head_attention.py
+-rw-r--r--  2.0 unx      787 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/layers/non_masking_layer.py
+-rw-r--r--  2.0 unx     1892 b- defN 23-Aug-03 20:53 kolibri/backend/tensorflow/layers/residual.py
+-rw-r--r--  2.0 unx      372 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/losses/__init__.py
+-rw-r--r--  2.0 unx     1416 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/losses/conditional_loss.py
+-rw-r--r--  2.0 unx     2959 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/losses/custom_loses.py
+-rw-r--r--  2.0 unx     2299 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/losses/gradient_penalty.py
+-rw-r--r--  2.0 unx      292 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/metrics/__init__.py
+-rw-r--r--  2.0 unx     2525 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/metrics/multi_label_classification.py
+-rw-r--r--  2.0 unx    14331 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/metrics/sequence_labeling.py
+-rw-r--r--  2.0 unx      158 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/__init__.py
+-rw-r--r--  2.0 unx     5384 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/base_model.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/structured/__init__.py
+-rw-r--r--  2.0 unx     7871 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/structured/base_model.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/structured/regression/__init__.py
+-rw-r--r--  2.0 unx     4756 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/structured/regression/base_model.py
+-rw-r--r--  2.0 unx     1929 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/structured/regression/dnn_regression_estimator.py
+-rw-r--r--  2.0 unx     2744 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/structured/regression/models.py
+-rw-r--r--  2.0 unx      517 b- defN 23-Aug-03 20:53 kolibri/backend/tensorflow/tasks/structured/synthetic/__init__.py
+-rw-r--r--  2.0 unx    20393 b- defN 23-Aug-03 20:53 kolibri/backend/tensorflow/tasks/structured/synthetic/_synthesizer.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/text/__init__.py
+-rw-r--r--  2.0 unx      417 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/text/classification/__init__.py
+-rw-r--r--  2.0 unx    15208 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/text/classification/base_model.py
+-rw-r--r--  2.0 unx     3381 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/text/classification/cnn_attention_model.py
+-rw-r--r--  2.0 unx     6196 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/text/classification/dpcnn_model.py
+-rw-r--r--  2.0 unx    28815 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/text/classification/models.py
+-rw-r--r--  2.0 unx      429 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/text/labeling/__init__.py
+-rw-r--r--  2.0 unx    17329 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/text/labeling/base_model.py
+-rw-r--r--  2.0 unx     2846 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/text/labeling/bi_gru_crf_model.py
+-rw-r--r--  2.0 unx     2249 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/text/labeling/bi_gru_model.py
+-rw-r--r--  2.0 unx     2991 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/text/labeling/bi_lstm_crf_model.py
+-rw-r--r--  2.0 unx     2295 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/text/labeling/bi_lstm_model.py
+-rw-r--r--  2.0 unx     1440 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/text/labeling/cnn_lstm_model.py
+-rw-r--r--  2.0 unx       84 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/text/seq2seq/__init__.py
+-rw-r--r--  2.0 unx     2443 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/text/seq2seq/generator.py
+-rw-r--r--  2.0 unx    13913 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/tasks/text/seq2seq/model.py
+-rw-r--r--  2.0 unx     1203 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/utils/__init__.py
+-rw-r--r--  2.0 unx      740 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/utils/_load_demo.py
+-rw-r--r--  2.0 unx      919 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/utils/data.py
+-rw-r--r--  2.0 unx     1629 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/utils/model.py
+-rw-r--r--  2.0 unx     1131 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/utils/multi_label.py
+-rw-r--r--  2.0 unx      862 b- defN 23-Jul-09 11:29 kolibri/backend/tensorflow/utils/serialize.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/backend/torch/__init__.py
+-rw-r--r--  2.0 unx    12666 b- defN 23-Jul-09 11:29 kolibri/backend/torch/base_model.py
+-rw-r--r--  2.0 unx     8161 b- defN 23-Jul-09 11:29 kolibri/backend/torch/models.py
+-rw-r--r--  2.0 unx      305 b- defN 23-Jul-09 11:29 kolibri/backend/torch/utils.py
+-rw-r--r--  2.0 unx      671 b- defN 23-Jul-09 11:29 kolibri/backend/torch/golem_utils/__init__.py
+-rw-r--r--  2.0 unx     4438 b- defN 23-Jul-09 11:29 kolibri/backend/torch/golem_utils/golem_model.py
+-rw-r--r--  2.0 unx     2545 b- defN 23-Jul-09 11:29 kolibri/backend/torch/golem_utils/train.py
+-rw-r--r--  2.0 unx     1636 b- defN 23-Jul-09 11:29 kolibri/backend/torch/golem_utils/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/backend/torch/layers/__init__.py
+-rw-r--r--  2.0 unx     5973 b- defN 23-Jul-09 11:29 kolibri/backend/torch/layers/crf.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/backend/torch/tasks/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/backend/torch/tasks/text/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/backend/torch/tasks/text/labeling/__init__.py
+-rw-r--r--  2.0 unx     1836 b- defN 23-Jul-09 11:29 kolibri/backend/torch/tasks/text/labeling/bi_lstm_crf.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/backend/torch/utils/__init__.py
+-rw-r--r--  2.0 unx     4009 b- defN 23-Jul-09 11:29 kolibri/backend/torch/utils/lbfgsb_scipy.py
+-rw-r--r--  2.0 unx     2864 b- defN 23-Jul-09 11:29 kolibri/backend/torch/utils/locally_connected.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/bin/__init__.py
+-rw-r--r--  2.0 unx      471 b- defN 23-Jul-09 11:29 kolibri/bin/datasets_configs.json
+-rw-r--r--  2.0 unx     2731 b- defN 23-Jul-09 11:29 kolibri/bin/kolibri-download.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/core/__init__.py
+-rw-r--r--  2.0 unx    18812 b- defN 23-Aug-03 20:53 kolibri/core/component.py
+-rw-r--r--  2.0 unx      223 b- defN 23-Aug-03 20:53 kolibri/core/document.py
+-rw-r--r--  2.0 unx     1111 b- defN 23-Jul-09 11:29 kolibri/core/entity.py
+-rw-r--r--  2.0 unx     4052 b- defN 23-Jul-09 11:29 kolibri/core/modules.py
+-rw-r--r--  2.0 unx    17570 b- defN 23-Jul-09 11:29 kolibri/core/pipeline.py
+-rw-r--r--  2.0 unx     2289 b- defN 23-Jul-09 11:29 kolibri/core/serializable.py
+-rw-r--r--  2.0 unx     5771 b- defN 23-Jul-09 11:29 kolibri/core/vocabulary.py
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-09 11:29 kolibri/data/__init__.py
+-rw-r--r--  2.0 unx     4452 b- defN 23-Jul-09 11:29 kolibri/data/auto_downloader.py
+-rw-r--r--  2.0 unx     2246 b- defN 23-Jul-09 11:29 kolibri/data/base_stream.py
+-rw-r--r--  2.0 unx     5113 b- defN 23-Jul-09 11:29 kolibri/data/blob.py
+-rw-r--r--  2.0 unx    29540 b- defN 23-Jul-09 11:29 kolibri/data/dataset.py
+-rw-r--r--  2.0 unx      234 b- defN 23-Jul-09 11:29 kolibri/data/document.py
+-rw-r--r--  2.0 unx    39086 b- defN 23-Jul-09 11:29 kolibri/data/downloader.py
+-rw-r--r--  2.0 unx    10372 b- defN 23-Jul-09 11:29 kolibri/data/file_stream.py
+-rw-r--r--  2.0 unx      534 b- defN 23-Jul-09 11:29 kolibri/data/iterator.py
+-rw-r--r--  2.0 unx      743 b- defN 23-Jul-09 11:29 kolibri/data/resources.py
+-rw-r--r--  2.0 unx    10130 b- defN 23-Jul-09 11:29 kolibri/data/schemes.py
+-rw-r--r--  2.0 unx    42659 b- defN 23-Jul-09 11:29 kolibri/data/settings.py
+-rw-r--r--  2.0 unx     5610 b- defN 23-Jul-09 11:29 kolibri/data/streams.py
+-rw-r--r--  2.0 unx     7910 b- defN 23-Jul-09 11:29 kolibri/data/text.py
+-rw-r--r--  2.0 unx    43976 b- defN 23-Jul-09 11:29 kolibri/data/utils.py
+-rw-r--r--  2.0 unx       94 b- defN 23-Jul-09 11:29 kolibri/data/format/__init__.py
+-rw-r--r--  2.0 unx      539 b- defN 23-Jul-09 11:29 kolibri/data/format/conll.py
+-rw-r--r--  2.0 unx      385 b- defN 23-Jul-09 11:29 kolibri/data/format/csv.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/data/loaders/__init__.py
+-rw-r--r--  2.0 unx      960 b- defN 23-Jul-09 11:29 kolibri/data/loaders/arxiv.py
+-rw-r--r--  2.0 unx     2516 b- defN 23-Jul-09 11:29 kolibri/data/loaders/base.py
+-rw-r--r--  2.0 unx     2238 b- defN 23-Jul-09 11:29 kolibri/data/loaders/csv_loader.py
+-rw-r--r--  2.0 unx     4577 b- defN 23-Jul-09 11:29 kolibri/data/loaders/pdf.py
+-rw-r--r--  2.0 unx     1973 b- defN 23-Jul-09 11:29 kolibri/data/loaders/text.py
+-rw-r--r--  2.0 unx     7710 b- defN 23-Jul-09 11:29 kolibri/data/loaders/web_base.py
+-rw-r--r--  2.0 unx      242 b- defN 23-Jul-09 11:29 kolibri/data/parsers/__init__.py
+-rw-r--r--  2.0 unx     1929 b- defN 23-Jul-09 11:29 kolibri/data/parsers/audio.py
+-rw-r--r--  2.0 unx     1090 b- defN 23-Jul-09 11:29 kolibri/data/parsers/base.py
+-rw-r--r--  2.0 unx     2429 b- defN 23-Jul-09 11:29 kolibri/data/parsers/generic.py
+-rw-r--r--  2.0 unx      813 b- defN 23-Jul-09 11:29 kolibri/data/parsers/pdf.py
+-rw-r--r--  2.0 unx      906 b- defN 23-Jul-09 11:29 kolibri/data/parsers/registry.py
+-rw-r--r--  2.0 unx      453 b- defN 23-Jul-09 11:29 kolibri/data/parsers/txt.py
+-rw-r--r--  2.0 unx       85 b- defN 23-Jul-09 11:29 kolibri/data/parsers/html/__init__.py
+-rw-r--r--  2.0 unx     1567 b- defN 23-Jul-09 11:29 kolibri/data/parsers/html/bs4.py
+-rw-r--r--  2.0 unx      929 b- defN 23-Jul-09 11:29 kolibri/data/parsers/html/hyperlinks.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/data/text/__init__.py
+-rw-r--r--  2.0 unx     2246 b- defN 23-Jul-09 11:29 kolibri/data/text/base_stream.py
+-rw-r--r--  2.0 unx     1236 b- defN 23-Jul-09 11:29 kolibri/data/text/corpus.py
+-rw-r--r--  2.0 unx    29550 b- defN 23-Jul-09 11:29 kolibri/data/text/dataset.py
+-rw-r--r--  2.0 unx    10385 b- defN 23-Jul-09 11:29 kolibri/data/text/file_stream.py
+-rw-r--r--  2.0 unx     5145 b- defN 23-Jul-09 11:29 kolibri/data/text/generators.py
+-rw-r--r--  2.0 unx      534 b- defN 23-Jul-09 11:29 kolibri/data/text/iterator.py
+-rw-r--r--  2.0 unx    10130 b- defN 23-Jul-09 11:29 kolibri/data/text/schemes.py
+-rw-r--r--  2.0 unx     5615 b- defN 23-Jul-09 11:29 kolibri/data/text/streams.py
+-rw-r--r--  2.0 unx     7915 b- defN 23-Jul-09 11:29 kolibri/data/text/text.py
+-rw-r--r--  2.0 unx      104 b- defN 23-Jul-09 11:29 kolibri/data/text/format/__init__.py
+-rw-r--r--  2.0 unx      539 b- defN 23-Jul-09 11:29 kolibri/data/text/format/conll.py
+-rw-r--r--  2.0 unx      385 b- defN 23-Jul-09 11:29 kolibri/data/text/format/csv.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/data/text/quality/__init__.py
+-rw-r--r--  2.0 unx     4796 b- defN 23-Jul-09 11:29 kolibri/data/text/quality/cosineSimilarity.py
+-rw-r--r--  2.0 unx      983 b- defN 23-Jul-09 11:29 kolibri/data/text/quality/mismatch.py
+-rw-r--r--  2.0 unx      166 b- defN 23-Jul-09 11:29 kolibri/data/text/quality/pairwise_cos_sim.py
+-rw-r--r--  2.0 unx      837 b- defN 23-Jul-09 11:29 kolibri/data/text/quality/similar.py
+-rw-r--r--  2.0 unx       47 b- defN 23-Jul-09 11:29 kolibri/datasets/__init__.py
+-rw-r--r--  2.0 unx     1800 b- defN 23-Aug-03 21:57 kolibri/datasets/read_data.py
+-rw-r--r--  2.0 unx       61 b- defN 23-Jul-09 11:29 kolibri/datasets/reader/__init__.py
+-rw-r--r--  2.0 unx     3092 b- defN 23-Jul-09 11:29 kolibri/datasets/reader/base_reader.py
+-rw-r--r--  2.0 unx     4055 b- defN 23-Jul-09 11:29 kolibri/datasets/reader/classification.py
+-rw-r--r--  2.0 unx     2213 b- defN 23-Jul-09 11:29 kolibri/datasets/reader/conll.py
+-rw-r--r--  2.0 unx    30779 b- defN 23-Jul-09 11:29 kolibri/datasets/reader/dialogs_reader.py
+-rw-r--r--  2.0 unx     8005 b- defN 23-Jul-09 11:29 kolibri/datasets/reader/dstc2.py
+-rw-r--r--  2.0 unx     4919 b- defN 23-Jul-09 11:29 kolibri/datasets/reader/snips.py
+-rw-r--r--  2.0 unx     3531 b- defN 23-Jul-09 11:29 kolibri/distances/__init__.py
+-rw-r--r--  2.0 unx     4899 b- defN 23-Jul-09 11:29 kolibri/distances/base_categorical.py
+-rw-r--r--  2.0 unx     2551 b- defN 23-Jul-09 11:29 kolibri/distances/eskin.py
+-rw-r--r--  2.0 unx     3907 b- defN 23-Jul-09 11:29 kolibri/distances/goodall.py
+-rw-r--r--  2.0 unx     6368 b- defN 23-Jul-09 11:29 kolibri/distances/heom.py
+-rw-r--r--  2.0 unx     5015 b- defN 23-Jul-09 11:29 kolibri/distances/hvdm.py
+-rw-r--r--  2.0 unx     1226 b- defN 23-Jul-09 11:29 kolibri/distances/lin.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/evaluation/__init__.py
+-rw-r--r--  2.0 unx     7885 b- defN 23-Jul-09 11:29 kolibri/evaluation/classifier_evaluator.py
+-rw-r--r--  2.0 unx     2489 b- defN 23-Jul-09 11:29 kolibri/evaluation/clustering_evaluator.py
+-rw-r--r--  2.0 unx    41666 b- defN 23-Jul-09 11:29 kolibri/evaluation/model_plot.py
+-rw-r--r--  2.0 unx      809 b- defN 23-Jul-09 11:29 kolibri/evaluation/metrics/__init__.py
+-rw-r--r--  2.0 unx     5578 b- defN 23-Jul-09 11:29 kolibri/evaluation/metrics/anomaly.py
+-rw-r--r--  2.0 unx     1792 b- defN 23-Jul-09 11:29 kolibri/evaluation/metrics/base_metric.py
+-rw-r--r--  2.0 unx     9438 b- defN 23-Jul-09 11:29 kolibri/evaluation/metrics/classification.py
+-rw-r--r--  2.0 unx     7198 b- defN 23-Jul-09 11:29 kolibri/evaluation/metrics/clustering.py
+-rw-r--r--  2.0 unx     8757 b- defN 23-Jul-09 11:29 kolibri/evaluation/metrics/metric_utils.py
+-rw-r--r--  2.0 unx     9491 b- defN 23-Jul-09 11:29 kolibri/evaluation/metrics/regression.py
+-rw-r--r--  2.0 unx    10235 b- defN 23-Jul-09 11:29 kolibri/evaluation/metrics/time_series.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/evaluators/__init__.py
+-rw-r--r--  2.0 unx     8796 b- defN 23-Jul-09 11:29 kolibri/evaluators/classifier_evaluator.py
+-rw-r--r--  2.0 unx     2489 b- defN 23-Jul-09 11:29 kolibri/evaluators/clustering_evaluator.py
+-rw-r--r--  2.0 unx    41682 b- defN 23-Jul-09 11:29 kolibri/evaluators/model_plot.py
+-rw-r--r--  2.0 unx     3215 b- defN 23-Jul-28 21:31 kolibri/evaluators/synthetic_data.py
+-rw-r--r--  2.0 unx      224 b- defN 23-Jul-09 11:29 kolibri/experiment_tracking/__init__.py
+-rw-r--r--  2.0 unx     6170 b- defN 23-Jul-09 11:29 kolibri/experiment_tracking/experiment_logger.py
+-rw-r--r--  2.0 unx     4971 b- defN 23-Jul-09 11:29 kolibri/experiment_tracking/mlflow_logger.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/explainers/__init__.py
+-rw-r--r--  2.0 unx    12089 b- defN 23-Jul-09 11:29 kolibri/explainers/shap_explainer.py
+-rw-r--r--  2.0 unx      227 b- defN 23-Jul-09 11:29 kolibri/features/__init__.py
+-rw-r--r--  2.0 unx     2781 b- defN 23-Jul-09 11:29 kolibri/features/base_feature.py
+-rw-r--r--  2.0 unx     1431 b- defN 23-Jul-09 11:29 kolibri/features/basefeaturizer.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/features/tabular/__init__.py
+-rw-r--r--  2.0 unx     1763 b- defN 23-Jul-09 11:29 kolibri/features/tabular/time_serie_featurizer.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/features/text/__init__.py
+-rw-r--r--  2.0 unx     8352 b- defN 23-Jul-09 11:29 kolibri/features/text/feature_functions.py
+-rw-r--r--  2.0 unx    10000 b- defN 23-Jul-09 11:29 kolibri/features/text/hashing_tfidf_vectorizer.py
+-rw-r--r--  2.0 unx     5801 b- defN 23-Jul-09 11:29 kolibri/features/text/text_features.py
+-rw-r--r--  2.0 unx     6336 b- defN 23-Jul-09 11:29 kolibri/features/text/tf_idf_featurizer.py
+-rw-r--r--  2.0 unx     5853 b- defN 23-Jul-09 11:29 kolibri/features/text/tf_idf_topics_vectorizer.py
+-rw-r--r--  2.0 unx     8121 b- defN 23-Jul-09 11:29 kolibri/features/text/tfidf_weighted_embedder.py
+-rw-r--r--  2.0 unx      346 b- defN 23-Aug-03 20:53 kolibri/features/text/embedders/__init__.py
+-rw-r--r--  2.0 unx     3709 b- defN 23-Jul-09 11:29 kolibri/features/text/embedders/base.py
+-rw-r--r--  2.0 unx     1347 b- defN 23-Jul-09 11:29 kolibri/features/text/embedders/bow_embedder.py
+-rw-r--r--  2.0 unx     9928 b- defN 23-Jul-09 11:29 kolibri/features/text/embedders/elmo_embedder.py
+-rw-r--r--  2.0 unx     1568 b- defN 23-Jul-09 11:29 kolibri/features/text/embedders/fasttext_embedder.py
+-rw-r--r--  2.0 unx     2027 b- defN 23-Jul-09 11:29 kolibri/features/text/embedders/glove_embedder.py
+-rw-r--r--  2.0 unx     4096 b- defN 23-Jul-09 11:29 kolibri/features/text/embedders/llamacpp.py
+-rw-r--r--  2.0 unx    17705 b- defN 23-Aug-03 20:53 kolibri/features/text/embedders/openai.py
+-rw-r--r--  2.0 unx     2466 b- defN 23-Jul-09 11:29 kolibri/features/text/embedders/tensorflow_hub.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/__init__.py
+-rw-r--r--  2.0 unx    31971 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/features_utils.py
+-rw-r--r--  2.0 unx    10656 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/ts_featurizer.py
+-rw-r--r--  2.0 unx     7659 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/utils.py
+-rw-r--r--  2.0 unx      358 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/feature_extraction/__init__.py
+-rw-r--r--  2.0 unx    16661 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/feature_extraction/data.py
+-rw-r--r--  2.0 unx    13772 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/feature_extraction/extraction.py
+-rw-r--r--  2.0 unx    81555 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/feature_extraction/feature_calculators.py
+-rw-r--r--  2.0 unx    14105 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/feature_extraction/settings.py
+-rw-r--r--  2.0 unx      606 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/feature_selection/__init__.py
+-rw-r--r--  2.0 unx    15671 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/feature_selection/relevance.py
+-rw-r--r--  2.0 unx     7871 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/feature_selection/selection.py
+-rw-r--r--  2.0 unx     8691 b- defN 23-Jul-09 11:29 kolibri/features/timeseries/feature_selection/significance_tests.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/formers/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/formers/tabular/__init__.py
+-rw-r--r--  2.0 unx     1043 b- defN 23-Jul-09 11:29 kolibri/formers/tabular/clustering.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/formers/text/__init__.py
+-rw-r--r--  2.0 unx     4315 b- defN 23-Jul-09 11:29 kolibri/formers/text/classifier.py
+-rw-r--r--  2.0 unx      230 b- defN 23-Jul-09 11:29 kolibri/formers/text/sentiment.py
+-rw-r--r--  2.0 unx     4515 b- defN 23-Jul-09 11:29 kolibri/formers/text/similarity.py
+-rw-r--r--  2.0 unx    40754 b- defN 23-Jul-09 11:29 kolibri/formers/text/topic_former.py
+-rw-r--r--  2.0 unx      219 b- defN 23-Jul-09 11:29 kolibri/indexers/__init__.py
+-rw-r--r--  2.0 unx     2680 b- defN 23-Jul-09 11:29 kolibri/indexers/base_indexer.py
+-rw-r--r--  2.0 unx     1239 b- defN 23-Jul-09 11:29 kolibri/indexers/kolibri_label_encoder.py
+-rw-r--r--  2.0 unx     3570 b- defN 23-Jul-09 11:29 kolibri/indexers/label_indexer.py
+-rw-r--r--  2.0 unx     1248 b- defN 23-Jul-09 11:29 kolibri/indexers/multi_content_indexer.py
+-rw-r--r--  2.0 unx     2394 b- defN 23-Jul-09 11:29 kolibri/indexers/multi_target_indexer.py
+-rw-r--r--  2.0 unx     4944 b- defN 23-Jul-09 11:29 kolibri/indexers/sequence_char_indexer.py
+-rw-r--r--  2.0 unx     6012 b- defN 23-Jul-25 15:43 kolibri/indexers/sequence_indexer.py
+-rw-r--r--  2.0 unx     5940 b- defN 23-Jul-09 11:29 kolibri/indexers/text_indexer.py
+-rw-r--r--  2.0 unx       43 b- defN 23-Jul-09 11:29 kolibri/knowledge/__init__.py
+-rw-r--r--  2.0 unx     1173 b- defN 23-Jul-09 11:29 kolibri/knowledge/domain.py
+-rw-r--r--  2.0 unx    11163 b- defN 23-Jul-09 11:29 kolibri/mlflow/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/optimizers/__init__.py
+-rw-r--r--  2.0 unx     9226 b- defN 23-Jul-09 11:29 kolibri/optimizers/metric.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/optimizers/optuna/__init__.py
+-rw-r--r--  2.0 unx    10868 b- defN 23-Jul-09 11:29 kolibri/optimizers/optuna/objective.py
+-rw-r--r--  2.0 unx     2889 b- defN 23-Jul-09 11:29 kolibri/optimizers/optuna/tuner.py
+-rw-r--r--  2.0 unx       49 b- defN 23-Jul-09 11:29 kolibri/output/__init__.py
+-rw-r--r--  2.0 unx     3303 b- defN 23-Jul-09 11:29 kolibri/output/display.py
+-rw-r--r--  2.0 unx     5694 b- defN 23-Jul-09 11:29 kolibri/output/display_backend.py
+-rw-r--r--  2.0 unx     1637 b- defN 23-Jul-09 11:29 kolibri/output/display_component.py
+-rw-r--r--  2.0 unx     4514 b- defN 23-Jul-09 11:29 kolibri/output/progress_bar.py
+-rw-r--r--  2.0 unx       40 b- defN 23-Jul-09 11:29 kolibri/preprocess/__init__.py
+-rw-r--r--  2.0 unx    13211 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/DataFrameVectorizer.py
+-rw-r--r--  2.0 unx     1780 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/__init__.py
+-rw-r--r--  2.0 unx     3030 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/binning.py
+-rw-r--r--  2.0 unx     8728 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/boruta_py.py
+-rw-r--r--  2.0 unx     1907 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/category_transformer.py
+-rw-r--r--  2.0 unx     5219 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/cluster.py
+-rw-r--r--  2.0 unx     1062 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/columns_remover.py
+-rw-r--r--  2.0 unx     1521 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/columns_transfromer.py
+-rw-r--r--  2.0 unx    11658 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/data_imputer.py
+-rw-r--r--  2.0 unx     2970 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/dummy_converter.py
+-rw-r--r--  2.0 unx    13500 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/feature_interaction.py
+-rw-r--r--  2.0 unx    10314 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/feature_selection.py
+-rw-r--r--  2.0 unx     4365 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/infer_datatype.py
+-rw-r--r--  2.0 unx    13584 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/multicollinearity.py
+-rw-r--r--  2.0 unx     4341 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/normalize.py
+-rw-r--r--  2.0 unx     2494 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/one_hot_encoder_multi.py
+-rw-r--r--  2.0 unx     1620 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/ordinal_transformer.py
+-rw-r--r--  2.0 unx     2616 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/outlier_remover.py
+-rw-r--r--  2.0 unx   149882 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/preprocess.py
+-rw-r--r--  2.0 unx    20056 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/preprocessing_pipeline.py
+-rw-r--r--  2.0 unx     3454 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/rare_levels.py
+-rw-r--r--  2.0 unx     8598 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/reduce_cardinality.py
+-rw-r--r--  2.0 unx     4848 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/reduce_dimensionality.py
+-rw-r--r--  2.0 unx     1801 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/regression_target_transformer.py
+-rw-r--r--  2.0 unx     2003 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/similar_features.py
+-rw-r--r--  2.0 unx     4003 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/time_features_extractor.py
+-rw-r--r--  2.0 unx     1808 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/univar_outliers.py
+-rw-r--r--  2.0 unx     3531 b- defN 23-Jul-09 11:29 kolibri/preprocess/tabular/zero_variance_remover.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/__init__.py
+-rw-r--r--  2.0 unx     4058 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/capitalization.py
+-rw-r--r--  2.0 unx      596 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/char_splitter.py
+-rw-r--r--  2.0 unx     4297 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/collocation_analyzer.py
+-rw-r--r--  2.0 unx     1412 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/context_builder.py
+-rw-r--r--  2.0 unx     3356 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/dirty_comments_preprocessor.py
+-rw-r--r--  2.0 unx     5305 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/doc_chuncker.py
+-rw-r--r--  2.0 unx     1183 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/mask.py
+-rw-r--r--  2.0 unx     7307 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/ner_preprocessor.py
+-rw-r--r--  2.0 unx     1229 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/random_embeddings_matrix.py
+-rw-r--r--  2.0 unx    10274 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/re_preprocessor.py
+-rw-r--r--  2.0 unx     5800 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/siamese_preprocessor.py
+-rw-r--r--  2.0 unx     1883 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/str_token_reverser.py
+-rw-r--r--  2.0 unx     7566 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/str_utf8_encoder.py
+-rw-r--r--  2.0 unx     6299 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/text_splitter.py
+-rw-r--r--  2.0 unx     2657 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/transformers_preprocessor.py
+-rw-r--r--  2.0 unx     5288 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/cleaning/__email_configs.py
+-rw-r--r--  2.0 unx       67 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/cleaning/__init__.py
+-rw-r--r--  2.0 unx     4348 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/cleaning/cleaning_scripts.py
+-rw-r--r--  2.0 unx    23554 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/cleaning/email2text.py
+-rw-r--r--  2.0 unx     1871 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/cleaning/email_cleaner.py
+-rw-r--r--  2.0 unx     1425 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/cleaning/email_parser.py
+-rw-r--r--  2.0 unx     3279 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/cleaning/header_parser.py
+-rw-r--r--  2.0 unx       82 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/language_detection/__init__.py
+-rw-r--r--  2.0 unx     1420 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/language_detection/lang_detect.py
+-rw-r--r--  2.0 unx     7047 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/translation/Translate_.py
+-rw-r--r--  2.0 unx     1079 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/translation/__init__.py
+-rw-r--r--  2.0 unx     9890 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/translation/client.py
+-rw-r--r--  2.0 unx     9746 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/translation/constants.py
+-rw-r--r--  2.0 unx     1601 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/translation/models.py
+-rw-r--r--  2.0 unx     6090 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/translation/translate.py
+-rw-r--r--  2.0 unx     2640 b- defN 23-Jul-09 11:29 kolibri/preprocess/text/translation/utils.py
+-rw-r--r--  2.0 unx       65 b- defN 23-Jul-09 11:29 kolibri/preprocess/timeseries/__init__.py
+-rw-r--r--  2.0 unx    16072 b- defN 23-Jul-09 11:29 kolibri/preprocess/timeseries/multi_window_generator.py
+-rw-r--r--  2.0 unx    15304 b- defN 23-Jul-09 11:29 kolibri/preprocess/timeseries/multi_window_generator_back.py
+-rw-r--r--  2.0 unx     7919 b- defN 23-Jul-09 11:29 kolibri/preprocess/timeseries/time_series_from_array.py
+-rw-r--r--  2.0 unx     8504 b- defN 23-Jul-09 11:29 kolibri/preprocess/timeseries/window.py
+-rw-r--r--  2.0 unx     7843 b- defN 23-Jul-09 11:29 kolibri/preprocess/timeseries/window_generator.py
+-rw-r--r--  2.0 unx     2131 b- defN 23-Jul-09 11:29 kolibri/samplers/__init__.py
+-rw-r--r--  2.0 unx     5095 b- defN 23-Jul-09 11:29 kolibri/samplers/auto_smpler.py
+-rw-r--r--  2.0 unx     5952 b- defN 23-Jul-09 11:29 kolibri/samplers/conditional.py
+-rw-r--r--  2.0 unx     2651 b- defN 23-Jul-09 11:29 kolibri/samplers/data_sampler.py
+-rw-r--r--  2.0 unx     7780 b- defN 23-Jul-09 11:29 kolibri/samplers/smoteR.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/scripts/__init__.py
+-rw-r--r--  2.0 unx      988 b- defN 23-Jul-09 11:29 kolibri/scripts/check_requirements.py
+-rw-r--r--  2.0 unx     1284 b- defN 23-Jul-09 11:29 kolibri/scripts/install_plugin_deps.py
+-rw-r--r--  2.0 unx       52 b- defN 23-Jul-09 11:29 kolibri/stopwords/__init__.py
+-rw-r--r--  2.0 unx     2016 b- defN 23-Jul-09 11:29 kolibri/stopwords/stp_wrd.py
+-rw-r--r--  2.0 unx      495 b- defN 23-Aug-05 11:31 kolibri/synthetic_data/__init__.py
+-rw-r--r--  2.0 unx     3060 b- defN 23-Aug-03 20:53 kolibri/synthetic_data/anonymization.py
+-rw-r--r--  2.0 unx    45818 b- defN 23-Aug-05 14:21 kolibri/synthetic_data/base.py
+-rw-r--r--  2.0 unx    18063 b- defN 23-Aug-03 20:53 kolibri/synthetic_data/base_contraint.py
+-rw-r--r--  2.0 unx    11071 b- defN 23-Aug-05 15:57 kolibri/synthetic_data/copulagan.py
+-rw-r--r--  2.0 unx    14946 b- defN 23-Aug-05 14:21 kolibri/synthetic_data/copulas.py
+-rw-r--r--  2.0 unx     9468 b- defN 23-Aug-03 20:53 kolibri/synthetic_data/ctgan_synthesizer.py
+-rw-r--r--  2.0 unx    35479 b- defN 23-Aug-05 14:47 kolibri/synthetic_data/data_processor.py
+-rw-r--r--  2.0 unx    21080 b- defN 23-Aug-05 14:30 kolibri/synthetic_data/metadata.py
+-rw-r--r--  2.0 unx     7180 b- defN 23-Aug-03 20:53 kolibri/synthetic_data/single_table.py
+-rw-r--r--  2.0 unx     3227 b- defN 23-Aug-05 16:08 kolibri/synthetic_data/synthpop.py
+-rw-r--r--  2.0 unx    10163 b- defN 23-Aug-05 06:42 kolibri/synthetic_data/utils.py
+-rw-r--r--  2.0 unx     1186 b- defN 23-Aug-05 11:04 kolibri/synthetic_data/benchmark/__init__.py
+-rw-r--r--  2.0 unx    15188 b- defN 23-Aug-05 06:42 kolibri/synthetic_data/benchmark/benchmark.py
+-rw-r--r--  2.0 unx     6232 b- defN 23-Aug-05 16:16 kolibri/synthetic_data/benchmark/data.py
+-rw-r--r--  2.0 unx     3309 b- defN 23-Aug-03 20:53 kolibri/synthetic_data/benchmark/metrics.py
+-rw-r--r--  2.0 unx     2241 b- defN 23-Aug-05 18:27 kolibri/synthetic_data/benchmark/ml.py
+-rw-r--r--  2.0 unx     2051 b- defN 23-Aug-05 11:00 kolibri/synthetic_data/benchmark/privacy.py
+-rw-r--r--  2.0 unx     4985 b- defN 23-Aug-03 20:53 kolibri/synthetic_data/benchmark/reporting.py
+-rw-r--r--  2.0 unx     2239 b- defN 23-Aug-05 08:41 kolibri/synthetic_data/benchmark/utility.py
+-rw-r--r--  2.0 unx     4880 b- defN 23-Aug-05 07:10 kolibri/synthetic_data/benchmark/utils.py
+-rw-r--r--  2.0 unx     1063 b- defN 23-Aug-05 15:35 kolibri/synthetic_data/benchmark/synthesizers/__init__.py
+-rw-r--r--  2.0 unx     1992 b- defN 23-Aug-05 06:42 kolibri/synthetic_data/benchmark/synthesizers/base.py
+-rw-r--r--  2.0 unx     7232 b- defN 23-Aug-03 20:53 kolibri/synthetic_data/benchmark/synthesizers/generate.py
+-rw-r--r--  2.0 unx     1337 b- defN 23-Aug-03 20:53 kolibri/synthetic_data/benchmark/synthesizers/identity.py
+-rw-r--r--  2.0 unx     2114 b- defN 23-Aug-03 20:53 kolibri/synthetic_data/benchmark/synthesizers/independent.py
+-rw-r--r--  2.0 unx     3491 b- defN 23-Aug-05 15:35 kolibri/synthetic_data/benchmark/synthesizers/sd.py
+-rw-r--r--  2.0 unx     1665 b- defN 23-Aug-03 20:53 kolibri/synthetic_data/benchmark/synthesizers/uniform.py
+-rw-r--r--  2.0 unx       66 b- defN 23-Jul-09 11:29 kolibri/task/__init__.py
+-rw-r--r--  2.0 unx     7685 b- defN 23-Jul-09 11:29 kolibri/task/dnn_estimator.py
+-rw-r--r--  2.0 unx      104 b- defN 23-Jul-09 11:29 kolibri/task/audio/__init__.py
+-rw-r--r--  2.0 unx     9853 b- defN 23-Jul-09 11:29 kolibri/task/audio/base_model.py
+-rw-r--r--  2.0 unx       75 b- defN 23-Jul-09 11:29 kolibri/task/audio/classification/__init__.py
+-rw-r--r--  2.0 unx     3231 b- defN 23-Jul-09 11:29 kolibri/task/audio/classification/dnn_audio_estimator.py
+-rw-r--r--  2.0 unx    10451 b- defN 23-Jul-09 11:29 kolibri/task/audio/classification/models.py
+-rw-r--r--  2.0 unx      156 b- defN 23-Jul-09 11:29 kolibri/task/tabular/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/task/tabular/anomaly/__init__.py
+-rw-r--r--  2.0 unx     1437 b- defN 23-Jul-09 11:29 kolibri/task/tabular/anomaly/anomaly_estimator.py
+-rw-r--r--  2.0 unx    18943 b- defN 23-Jul-09 11:29 kolibri/task/tabular/anomaly/half_space_trees.py
+-rw-r--r--  2.0 unx      700 b- defN 23-Jul-09 11:29 kolibri/task/tabular/anomaly/models.py
+-rw-r--r--  2.0 unx      742 b- defN 23-Jul-09 11:29 kolibri/task/tabular/anomaly/one_class_anomaly_dector.py
+-rw-r--r--  2.0 unx     3274 b- defN 23-Jul-09 11:29 kolibri/task/tabular/anomaly/semi_supervised_anomaly_dector.py
+-rw-r--r--  2.0 unx     4617 b- defN 23-Jul-09 11:29 kolibri/task/tabular/anomaly/unsupervised_anomaly_dector.py
+-rw-r--r--  2.0 unx       74 b- defN 23-Jul-09 11:29 kolibri/task/tabular/clustering/__init__.py
+-rw-r--r--  2.0 unx     4518 b- defN 23-Jul-09 11:29 kolibri/task/tabular/clustering/clustering.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/task/tabular/regression/__init__.py
+-rw-r--r--  2.0 unx     1874 b- defN 23-Jul-09 11:29 kolibri/task/tabular/regression/dnn_regression_estimator.py
+-rw-r--r--  2.0 unx     2170 b- defN 23-Jul-09 11:29 kolibri/task/tabular/regression/sklearn_regression_estimator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/task/tabular/rulemining/__init__.py
+-rw-r--r--  2.0 unx     9912 b- defN 23-Jul-09 11:29 kolibri/task/tabular/rulemining/association_rules.py
+-rw-r--r--  2.0 unx      140 b- defN 23-Jul-09 11:29 kolibri/task/text/__init__.py
+-rw-r--r--  2.0 unx      190 b- defN 23-Jul-09 11:29 kolibri/task/text/classification/__init__.py
+-rw-r--r--  2.0 unx     4316 b- defN 23-Jul-09 11:29 kolibri/task/text/classification/dnn_classification_estimator.py
+-rw-r--r--  2.0 unx     3199 b- defN 23-Jul-09 11:29 kolibri/task/text/classification/sklearn_classification_estimator.py
+-rw-r--r--  2.0 unx     3407 b- defN 23-Jul-09 11:29 kolibri/task/text/classification/sklearn_estimator.py
+-rw-r--r--  2.0 unx     3145 b- defN 23-Jul-09 11:29 kolibri/task/text/entities/__init__.py
+-rw-r--r--  2.0 unx     1990 b- defN 23-Jul-09 11:29 kolibri/task/text/entities/common_reg_extractor.py
+-rw-r--r--  2.0 unx    17418 b- defN 23-Jul-09 11:29 kolibri/task/text/entities/crf_entity_extractor.py
+-rw-r--r--  2.0 unx      949 b- defN 23-Jul-09 11:29 kolibri/task/text/entities/dictionaryExtractor.py
+-rw-r--r--  2.0 unx     1111 b- defN 23-Jul-09 11:29 kolibri/task/text/entities/entity.py
+-rw-r--r--  2.0 unx     3007 b- defN 23-Jul-09 11:29 kolibri/task/text/entities/entity_extractor.py
+-rw-r--r--  2.0 unx     4171 b- defN 23-Jul-09 11:29 kolibri/task/text/entities/entity_synonyms.py
+-rw-r--r--  2.0 unx     6339 b- defN 23-Jul-09 11:29 kolibri/task/text/entities/lstm_entity_extractor.py
+-rw-r--r--  2.0 unx     3633 b- defN 23-Jul-09 11:29 kolibri/task/text/entities/person_extractor.py
+-rw-r--r--  2.0 unx     2279 b- defN 23-Jul-09 11:29 kolibri/task/text/entities/preprocessing.py
+-rw-r--r--  2.0 unx     2668 b- defN 23-Jul-09 11:29 kolibri/task/text/entities/regex_extractor.py
+-rw-r--r--  2.0 unx     6945 b- defN 23-Jul-09 11:29 kolibri/task/text/entities/templated_extractor.py
+-rw-r--r--  2.0 unx     3498 b- defN 23-Jul-09 11:29 kolibri/task/text/entities/test.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/task/text/entities_back/__init__.py
+-rw-r--r--  2.0 unx     6458 b- defN 23-Jul-09 11:29 kolibri/task/text/entities_back/common_reg_extractor.py
+-rw-r--r--  2.0 unx    18309 b- defN 23-Jul-09 11:29 kolibri/task/text/entities_back/crf_entity_extractor.py
+-rw-r--r--  2.0 unx     1011 b- defN 23-Jul-09 11:29 kolibri/task/text/entities_back/dictionaryExtractor.py
+-rw-r--r--  2.0 unx     2997 b- defN 23-Jul-09 11:29 kolibri/task/text/entities_back/entity_extractor.py
+-rw-r--r--  2.0 unx     4343 b- defN 23-Jul-09 11:29 kolibri/task/text/entities_back/entity_synonyms.py
+-rw-r--r--  2.0 unx     3188 b- defN 23-Jul-09 11:29 kolibri/task/text/entities_back/person_extractor.py
+-rw-r--r--  2.0 unx     2295 b- defN 23-Jul-09 11:29 kolibri/task/text/entities_back/preprocessing.py
+-rw-r--r--  2.0 unx     2644 b- defN 23-Jul-09 11:29 kolibri/task/text/entities_back/regex_extractor.py
+-rw-r--r--  2.0 unx     6419 b- defN 23-Jul-09 11:29 kolibri/task/text/entities_back/templated_extractor.py
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-09 11:29 kolibri/task/text/intents/__init__.py
+-rw-r--r--  2.0 unx    10289 b- defN 23-Jul-09 11:29 kolibri/task/text/intents/intent_catcher.py
+-rw-r--r--  2.0 unx     3811 b- defN 23-Jul-09 11:29 kolibri/task/text/intents/intent_expressions.py
+-rw-r--r--  2.0 unx     1437 b- defN 23-Jul-09 11:29 kolibri/task/text/intents/domains/__init__.py
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-09 11:29 kolibri/task/text/sentiment/__init__.py
+-rw-r--r--  2.0 unx    12971 b- defN 23-Jul-09 11:29 kolibri/task/text/sentiment/lexicon_sentiment.py
+-rw-r--r--  2.0 unx    32780 b- defN 23-Jul-09 11:29 kolibri/task/text/sentiment/util.py
+-rw-r--r--  2.0 unx    22769 b- defN 23-Jul-09 11:29 kolibri/task/text/sentiment/vader.py
+-rw-r--r--  2.0 unx     2587 b- defN 23-Jul-09 11:29 kolibri/task/text/similarity/__init__.py
+-rw-r--r--  2.0 unx      559 b- defN 23-Jul-09 11:29 kolibri/task/text/similarity/arxiv.py
+-rw-r--r--  2.0 unx     6717 b- defN 23-Jul-09 11:29 kolibri/task/text/similarity/docarray.py
+-rw-r--r--  2.0 unx     2361 b- defN 23-Jul-09 11:29 kolibri/task/text/similarity/knn.py
+-rw-r--r--  2.0 unx     2907 b- defN 23-Jul-09 11:29 kolibri/task/text/similarity/llama_index.py
+-rw-r--r--  2.0 unx     2907 b- defN 23-Jul-09 11:29 kolibri/task/text/similarity/merger_retriever.py
+-rw-r--r--  2.0 unx      569 b- defN 23-Jul-09 11:29 kolibri/task/text/similarity/pupmed.py
+-rw-r--r--  2.0 unx     2953 b- defN 23-Jul-09 11:29 kolibri/task/text/similarity/svm.py
+-rw-r--r--  2.0 unx     2470 b- defN 23-Jul-09 11:29 kolibri/task/text/similarity/tfidf.py
+-rw-r--r--  2.0 unx      579 b- defN 23-Jul-09 11:29 kolibri/task/text/similarity/wikipedia.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/task/text/spelling/__init__.py
+-rw-r--r--  2.0 unx       36 b- defN 23-Jul-09 11:29 kolibri/task/text/spelling/brillmoore/__init__.py
+-rw-r--r--  2.0 unx    10769 b- defN 23-Jul-09 11:29 kolibri/task/text/spelling/brillmoore/error_model.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/task/text/spelling/electors/__init__.py
+-rw-r--r--  2.0 unx     2815 b- defN 23-Jul-09 11:29 kolibri/task/text/spelling/electors/kenlm_elector.py
+-rw-r--r--  2.0 unx     1421 b- defN 23-Jul-09 11:29 kolibri/task/text/spelling/electors/top1_elector.py
+-rw-r--r--  2.0 unx       61 b- defN 23-Jul-09 11:29 kolibri/task/text/spelling/levenshtein/__init__.py
+-rw-r--r--  2.0 unx    33386 b- defN 23-Jul-09 11:29 kolibri/task/text/spelling/levenshtein/levenshtein_searcher.py
+-rw-r--r--  2.0 unx     3406 b- defN 23-Jul-09 11:29 kolibri/task/text/spelling/levenshtein/searcher_component.py
+-rw-r--r--  2.0 unx    20586 b- defN 23-Jul-09 11:29 kolibri/task/text/spelling/levenshtein/tabled_trie.py
+-rw-r--r--  2.0 unx      152 b- defN 23-Jul-09 11:29 kolibri/task/text/topics/__init__.py
+-rw-r--r--  2.0 unx     3563 b- defN 23-Jul-09 11:29 kolibri/task/text/topics/baseTopic.py
+-rw-r--r--  2.0 unx    24958 b- defN 23-Jul-09 11:29 kolibri/task/text/topics/mallet.py
+-rw-r--r--  2.0 unx    14976 b- defN 23-Jul-09 11:29 kolibri/task/text/topics/topics_estimator.py
+-rw-r--r--  2.0 unx       58 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/__init__.py
+-rw-r--r--  2.0 unx    23782 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/dataset.py
+-rw-r--r--  2.0 unx      962 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/metrics.py
+-rw-r--r--  2.0 unx     1953 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/analysis/__init__.py
+-rw-r--r--  2.0 unx     7234 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/analysis/eda_utils.py
+-rw-r--r--  2.0 unx    17003 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/analysis/plotters.py
+-rw-r--r--  2.0 unx      494 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/analysis/feature_relevance/__init__.py
+-rw-r--r--  2.0 unx     3066 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/analysis/feature_relevance/relevance.py
+-rw-r--r--  2.0 unx     2919 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/analysis/feature_relevance/relevance_table.py
+-rw-r--r--  2.0 unx      583 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/analysis/outliers/__init__.py
+-rw-r--r--  2.0 unx     5017 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/analysis/outliers/density_outliers.py
+-rw-r--r--  2.0 unx    13178 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/analysis/outliers/hist_outliers.py
+-rw-r--r--  2.0 unx     1878 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/analysis/outliers/median_outliers.py
+-rw-r--r--  2.0 unx     2998 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/analysis/outliers/prediction_interval_outliers.py
+-rw-r--r--  2.0 unx     3501 b- defN 23-Jul-09 11:29 kolibri/task/timeseries/analysis/outliers/sequence_outliers.py
+-rw-r--r--  2.0 unx     1470 b- defN 23-Jul-09 11:29 kolibri/tokenizers/__init__.py
+-rw-r--r--  2.0 unx     4690 b- defN 23-Jul-09 11:29 kolibri/tokenizers/bert_tokenizer.py
+-rw-r--r--  2.0 unx     3999 b- defN 23-Jul-09 11:29 kolibri/tokenizers/char_tokenizer.py
+-rw-r--r--  2.0 unx     7103 b- defN 23-Jul-09 11:29 kolibri/tokenizers/kolibri_tokenizer.py
+-rw-r--r--  2.0 unx     2361 b- defN 23-Jul-09 11:29 kolibri/tokenizers/multi_word_tokenizer.py
+-rw-r--r--  2.0 unx     2661 b- defN 23-Jul-09 11:29 kolibri/tokenizers/regex_tokenizer.py
+-rw-r--r--  2.0 unx     1025 b- defN 23-Jul-09 11:29 kolibri/tokenizers/sentence_tokenizer.py
+-rw-r--r--  2.0 unx     2708 b- defN 23-Jul-09 11:29 kolibri/tokenizers/tokenizer.py
+-rw-r--r--  2.0 unx     6936 b- defN 23-Jul-09 11:29 kolibri/tokenizers/ugc_tokenizer.py
+-rw-r--r--  2.0 unx     2404 b- defN 23-Jul-09 11:29 kolibri/tokenizers/word_tokenizer.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/tools/__init__.py
+-rw-r--r--  2.0 unx      411 b- defN 23-Jul-09 11:29 kolibri/tools/_regex.py
+-rw-r--r--  2.0 unx      841 b- defN 23-Jul-09 11:29 kolibri/tools/arxiv.py
+-rw-r--r--  2.0 unx     1208 b- defN 23-Jul-09 11:29 kolibri/tools/bing_search.py
+-rw-r--r--  2.0 unx     1441 b- defN 23-Jul-09 11:29 kolibri/tools/ddg_search.py
+-rw-r--r--  2.0 unx     2063 b- defN 23-Jul-09 11:29 kolibri/tools/gebbrisg_detector.py
+-rw-r--r--  2.0 unx     1231 b- defN 23-Jul-09 11:29 kolibri/tools/google_search.py
+-rw-r--r--  2.0 unx    25525 b- defN 23-Jul-09 11:29 kolibri/tools/keywords.py
+-rw-r--r--  2.0 unx      777 b- defN 23-Jul-09 11:29 kolibri/tools/openweathermap.py
+-rw-r--r--  2.0 unx      853 b- defN 23-Jul-09 11:29 kolibri/tools/pubmed.py
+-rw-r--r--  2.0 unx     1828 b- defN 23-Jul-09 11:29 kolibri/tools/regexes.py
+-rw-r--r--  2.0 unx    17263 b- defN 23-Jul-09 11:29 kolibri/tools/scanner.py
+-rw-r--r--  2.0 unx      690 b- defN 23-Jul-09 11:29 kolibri/tools/wikipedia.py
+-rw-r--r--  2.0 unx      699 b- defN 23-Jul-09 11:29 kolibri/tools/wolfram_alpha.py
+-rw-r--r--  2.0 unx    13056 b- defN 23-Jul-09 11:29 kolibri/tools/word_frequencies.py
+-rw-r--r--  2.0 unx     1447 b- defN 23-Jul-09 11:29 kolibri/tools/youtube_search.py
+-rw-r--r--  2.0 unx     4826 b- defN 23-Aug-03 20:53 kolibri/utils/__init__.py
+-rw-r--r--  2.0 unx    11174 b- defN 23-Jul-09 11:29 kolibri/utils/cm.py
+-rw-r--r--  2.0 unx     6904 b- defN 23-Jul-09 11:29 kolibri/utils/common.py
+-rw-r--r--  2.0 unx     3173 b- defN 23-Jul-09 11:29 kolibri/utils/config.py
+-rw-r--r--  2.0 unx    12009 b- defN 23-Jul-09 11:29 kolibri/utils/cross_validation.py
+-rw-r--r--  2.0 unx    14474 b- defN 23-Jul-09 11:29 kolibri/utils/distribution.py
+-rw-r--r--  2.0 unx      873 b- defN 23-Jul-09 11:29 kolibri/utils/environement.py
+-rw-r--r--  2.0 unx     3259 b- defN 23-Jul-09 11:29 kolibri/utils/language_info.py
+-rw-r--r--  2.0 unx      544 b- defN 23-Jul-09 11:29 kolibri/utils/log_normalizer.py
+-rw-r--r--  2.0 unx     5686 b- defN 23-Jul-09 11:29 kolibri/utils/mathext.py
+-rw-r--r--  2.0 unx     2904 b- defN 23-Jul-09 11:29 kolibri/utils/matrix.py
+-rw-r--r--  2.0 unx     3158 b- defN 23-Jul-09 11:29 kolibri/utils/nb_clusters.py
+-rw-r--r--  2.0 unx      631 b- defN 23-Jul-09 11:29 kolibri/utils/parallel.py
+-rw-r--r--  2.0 unx     2361 b- defN 23-Jul-09 11:29 kolibri/utils/progress_bar.py
+-rw-r--r--  2.0 unx     4618 b- defN 23-Aug-03 20:53 kolibri/utils/serializable.py
+-rw-r--r--  2.0 unx     2280 b- defN 23-Jul-09 11:29 kolibri/utils/spinner.py
+-rw-r--r--  2.0 unx     1252 b- defN 23-Jul-09 11:29 kolibri/utils/text_encoding.py
+-rw-r--r--  2.0 unx    28893 b- defN 23-Jul-09 11:29 kolibri/utils/timeseries_functions.py
+-rw-r--r--  2.0 unx    28840 b- defN 23-Jul-09 11:29 kolibri/utils/timeseries_functions_back.py
+-rw-r--r--  2.0 unx      547 b- defN 23-Jul-09 11:29 kolibri/utils/wrappers/__init__.py
+-rw-r--r--  2.0 unx     5589 b- defN 23-Jul-09 11:29 kolibri/utils/wrappers/arxiv.py
+-rw-r--r--  2.0 unx     3344 b- defN 23-Jul-09 11:29 kolibri/utils/wrappers/bing_search.py
+-rw-r--r--  2.0 unx     3330 b- defN 23-Jul-09 11:29 kolibri/utils/wrappers/duckduckgo_search.py
+-rw-r--r--  2.0 unx     4910 b- defN 23-Jul-09 11:29 kolibri/utils/wrappers/google_search.py
+-rw-r--r--  2.0 unx     2431 b- defN 23-Jul-09 11:29 kolibri/utils/wrappers/openweathermap.py
+-rw-r--r--  2.0 unx     5742 b- defN 23-Jul-09 11:29 kolibri/utils/wrappers/pupmed.py
+-rw-r--r--  2.0 unx     4035 b- defN 23-Jul-09 11:29 kolibri/utils/wrappers/wikipedia.py
+-rw-r--r--  2.0 unx     2000 b- defN 23-Jul-09 11:29 kolibri/utils/wrappers/wolfram_alpha.py
+-rw-r--r--  2.0 unx      347 b- defN 23-Jul-09 11:29 kolibri/vectordb/__init__.py
+-rw-r--r--  2.0 unx    16298 b- defN 23-Aug-03 20:53 kolibri/vectordb/base.py
+-rw-r--r--  2.0 unx    23410 b- defN 23-Jul-09 11:29 kolibri/vectordb/faiss.py
+-rw-r--r--  2.0 unx    21803 b- defN 23-Aug-03 20:53 kolibri/vectordb/redis.py
+-rw-r--r--  2.0 unx    12276 b- defN 23-Jul-09 11:29 kolibri/vectordb/sklearn.py
+-rw-r--r--  2.0 unx     1462 b- defN 23-Jul-09 11:29 kolibri/vectordb/utils.py
+-rw-r--r--  2.0 unx      204 b- defN 23-Jul-09 11:29 kolibri/vectordb/docarray/__init__.py
+-rw-r--r--  2.0 unx     6872 b- defN 23-Aug-03 20:53 kolibri/vectordb/docarray/base.py
+-rw-r--r--  2.0 unx     4062 b- defN 23-Jul-09 11:29 kolibri/vectordb/docarray/hnsw.py
+-rw-r--r--  2.0 unx     2416 b- defN 23-Jul-09 11:29 kolibri/vectordb/docarray/in_memory.py
+-rw-r--r--  2.0 unx      280 b- defN 23-Jul-09 11:29 kolibri/vectordb/docstore/__init__.py
+-rw-r--r--  2.0 unx      924 b- defN 23-Jul-09 11:29 kolibri/vectordb/docstore/arbitrary_fn.py
+-rw-r--r--  2.0 unx      694 b- defN 23-Jul-09 11:29 kolibri/vectordb/docstore/base.py
+-rw-r--r--  2.0 unx      973 b- defN 23-Jul-09 11:29 kolibri/vectordb/docstore/in_memory.py
+-rw-r--r--  2.0 unx     1376 b- defN 23-Jul-09 11:29 kolibri/vectordb/docstore/wikipedia.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 kolibri/visualizations/__init__.py
+-rw-r--r--  2.0 unx    53405 b- defN 23-Jul-09 11:29 kolibri/visualizations/classification_plots.py
+-rw-r--r--  2.0 unx    15746 b- defN 23-Jul-09 11:29 kolibri/visualizations/pipeline.py
+-rw-r--r--  2.0 unx    34339 b- defN 23-Jul-09 11:29 kolibri/visualizations/regression_plots.py
+-rw-r--r--  2.0 unx    15565 b- defN 23-Jul-09 11:29 kolibri/visualizations/utils.py
+-rw-r--r--  2.0 unx       52 b- defN 23-Jul-09 11:29 tests/__init__.py
+-rw-r--r--  2.0 unx    20075 b- defN 23-Jul-09 11:29 tests/test_data_transformer.py
+-rw-r--r--  2.0 unx      960 b- defN 23-Jul-09 11:29 tests/test_pipeline.py
+-rw-r--r--  2.0 unx      557 b- defN 23-Jul-09 11:29 tests/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 tests/entities/__init__.py
+-rw-r--r--  2.0 unx     7812 b- defN 23-Jul-09 11:29 tests/entities/test.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 tests/optuna/__init__.py
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-09 11:29 tests/optuna/test_optuna.py
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-09 11:29 tests/synthesizer/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 tests/synthesizer/data_modules/__init__.py
+-rw-r--r--  2.0 unx     2865 b- defN 23-Jul-09 11:29 tests/synthesizer/data_modules/test_conditional.py
+-rw-r--r--  2.0 unx     1131 b- defN 23-Jul-09 11:29 tests/synthesizer/data_modules/test_sampler.py
+-rw-r--r--  2.0 unx     2949 b- defN 23-Jul-09 11:29 tests/synthesizer/data_modules/test_transformer.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 tests/synthesizer/layers/__init__.py
+-rw-r--r--  2.0 unx     7960 b- defN 23-Jul-09 11:29 tests/synthesizer/layers/test_gen_activation.py
+-rw-r--r--  2.0 unx     1429 b- defN 23-Jul-09 11:29 tests/synthesizer/layers/test_layer_utils.py
+-rw-r--r--  2.0 unx     4793 b- defN 23-Jul-09 11:29 tests/synthesizer/layers/test_residual.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 tests/synthesizer/losses/__init__.py
+-rw-r--r--  2.0 unx     1128 b- defN 23-Jul-09 11:29 tests/synthesizer/losses/test_conditional_loss.py
+-rw-r--r--  2.0 unx      812 b- defN 23-Jul-09 11:29 tests/synthesizer/losses/test_gradient_penalty.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 tests/synthesizer/models/__init__.py
+-rw-r--r--  2.0 unx     1214 b- defN 23-Jul-09 11:29 tests/synthesizer/models/test_critic.py
+-rw-r--r--  2.0 unx     4972 b- defN 23-Jul-09 11:29 tests/synthesizer/models/test_generator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-09 11:29 tests/synthesizer/synthesizer/__init__.py
+-rw-r--r--  2.0 unx     4090 b- defN 23-Jul-09 11:29 tests/synthesizer/synthesizer/test_synthesizer.py
+-rw-r--r--  2.0 unx    34572 b- defN 23-Aug-05 18:44 kolibri_ml-1.1.80.dist-info/LICENCE.txt
+-rw-r--r--  2.0 unx     4885 b- defN 23-Aug-05 18:44 kolibri_ml-1.1.80.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-05 18:44 kolibri_ml-1.1.80.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Aug-05 18:44 kolibri_ml-1.1.80.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    67912 b- defN 23-Aug-05 18:44 kolibri_ml-1.1.80.dist-info/RECORD
+699 files, 4493698 bytes uncompressed, 1186200 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -1,7 +1,10 @@
+Filename: kolibri/.env
+Comment: 
+
 Filename: kolibri/VERSION
 Comment: 
 
 Filename: kolibri/__init__.py
 Comment: 
 
 Filename: kolibri/app.py
@@ -33,17 +36,26 @@
 
 Filename: kolibri/registry.py
 Comment: 
 
 Filename: kolibri/requirements.txt
 Comment: 
 
+Filename: kolibri/settings.py
+Comment: 
+
 Filename: kolibri/settings.yaml
 Comment: 
 
+Filename: kolibri/types.py
+Comment: 
+
+Filename: kolibri/version.py
+Comment: 
+
 Filename: kolibri/api/__init__.py
 Comment: 
 
 Filename: kolibri/api/classification/__init__.py
 Comment: 
 
 Filename: kolibri/autolearn/__init__.py
@@ -60,17 +72,26 @@
 
 Filename: kolibri/autolearn/model_zoo/__init__.py
 Comment: 
 
 Filename: kolibri/autolearn/model_zoo/zoo_classifier.py
 Comment: 
 
+Filename: kolibri/autolearn/model_zoo/zoo_estimator.py
+Comment: 
+
 Filename: kolibri/autolearn/model_zoo/zoo_regressor.py
 Comment: 
 
+Filename: kolibri/automl/__init__.py
+Comment: 
+
+Filename: kolibri/automl/data_inspection.py
+Comment: 
+
 Filename: kolibri/backend/__init__.py
 Comment: 
 
 Filename: kolibri/backend/models.py
 Comment: 
 
 Filename: kolibri/backend/base/__init__.py
@@ -84,17 +105,233 @@
 
 Filename: kolibri/backend/base/base_estimator.py
 Comment: 
 
 Filename: kolibri/backend/base/base_regressor.py
 Comment: 
 
+Filename: kolibri/backend/base/estimator.py
+Comment: 
+
+Filename: kolibri/backend/base/nn_model.py
+Comment: 
+
+Filename: kolibri/backend/bn/BayesianModel.py
+Comment: 
+
+Filename: kolibri/backend/bn/BayesianNetwork.py
+Comment: 
+
+Filename: kolibri/backend/bn/CPD.py
+Comment: 
+
+Filename: kolibri/backend/bn/ContinuousFactor.py
+Comment: 
+
+Filename: kolibri/backend/bn/DAG.py
+Comment: 
+
+Filename: kolibri/backend/bn/DiscreteFactor.py
+Comment: 
+
+Filename: kolibri/backend/bn/DynamicBayesianNetwork.py
+Comment: 
+
+Filename: kolibri/backend/bn/EliminationOrder.py
+Comment: 
+
+Filename: kolibri/backend/bn/ExactInference.py
+Comment: 
+
+Filename: kolibri/backend/bn/FactorGraph.py
+Comment: 
+
+Filename: kolibri/backend/bn/Independencies.py
+Comment: 
+
+Filename: kolibri/backend/bn/JointProbabilityDistribution.py
+Comment: 
+
+Filename: kolibri/backend/bn/JunctionTree.py
+Comment: 
+
+Filename: kolibri/backend/bn/LinearGaussianCPD.py
+Comment: 
+
+Filename: kolibri/backend/bn/MarkovChain.py
+Comment: 
+
+Filename: kolibri/backend/bn/MarkovNetwork.py
+Comment: 
+
+Filename: kolibri/backend/bn/NaiveBayes.py
+Comment: 
+
+Filename: kolibri/backend/bn/Sampling.py
+Comment: 
+
+Filename: kolibri/backend/bn/UndirectedGraph.py
+Comment: 
+
+Filename: kolibri/backend/bn/__init__.py
+Comment: 
+
+Filename: kolibri/backend/bn/base_estimator.py
+Comment: 
+
+Filename: kolibri/backend/bn/base_inference.py
+Comment: 
+
+Filename: kolibri/backend/bn/bnlearn.py
+Comment: 
+
+Filename: kolibri/backend/bn/factors_base.py
+Comment: 
+
+Filename: kolibri/backend/bn/metrics.py
+Comment: 
+
+Filename: kolibri/backend/bn/network.py
+Comment: 
+
+Filename: kolibri/backend/bn/state_name.py
+Comment: 
+
+Filename: kolibri/backend/bn/tabulate.py
+Comment: 
+
+Filename: kolibri/backend/bn/utils.py
+Comment: 
+
+Filename: kolibri/backend/bn/distributions/CanonicalDistribution.py
+Comment: 
+
+Filename: kolibri/backend/bn/distributions/CustomDistribution.py
+Comment: 
+
+Filename: kolibri/backend/bn/distributions/GaussianDistribution.py
+Comment: 
+
+Filename: kolibri/backend/bn/distributions/__init__.py
+Comment: 
+
+Filename: kolibri/backend/bn/distributions/base.py
+Comment: 
+
+Filename: kolibri/backend/bn/estimators/HillClimbSearch.py
+Comment: 
+
+Filename: kolibri/backend/bn/estimators/MLE.py
+Comment: 
+
+Filename: kolibri/backend/bn/estimators/ScoreCache.py
+Comment: 
+
+Filename: kolibri/backend/bn/estimators/StructureScore.py
+Comment: 
+
+Filename: kolibri/backend/bn/estimators/__init__.py
+Comment: 
+
+Filename: kolibri/backend/bn/estimators/bayesianEstimator.py
+Comment: 
+
+Filename: kolibri/backend/bn/inference/__init__.py
+Comment: 
+
+Filename: kolibri/backend/bn/inference/inference.py
+Comment: 
+
+Filename: kolibri/backend/bn/inference/predict.py
+Comment: 
+
+Filename: kolibri/backend/bn/parameters/__init__.py
+Comment: 
+
+Filename: kolibri/backend/bn/parameters/learn.py
+Comment: 
+
+Filename: kolibri/backend/bn/parameters/parameter_learning.py
+Comment: 
+
+Filename: kolibri/backend/bn/readwrite/BIF.py
+Comment: 
+
+Filename: kolibri/backend/bn/readwrite/UAI.py
+Comment: 
+
+Filename: kolibri/backend/bn/readwrite/XMLBIF.py
+Comment: 
+
+Filename: kolibri/backend/bn/readwrite/__init__.py
+Comment: 
+
+Filename: kolibri/backend/bn/structure/__init__.py
+Comment: 
+
+Filename: kolibri/backend/bn/structure/base.py
+Comment: 
+
+Filename: kolibri/backend/bn/structure/evaluation.py
+Comment: 
+
+Filename: kolibri/backend/bn/structure/learn.py
+Comment: 
+
+Filename: kolibri/backend/bn/structure/linear.py
+Comment: 
+
+Filename: kolibri/backend/bn/structure/low_rank.py
+Comment: 
+
+Filename: kolibri/backend/bn/structure/no_tears.py
+Comment: 
+
+Filename: kolibri/backend/bn/structure/no_tears_tf.py
+Comment: 
+
+Filename: kolibri/backend/bn/structure/no_tears_tf2.py
+Comment: 
+
+Filename: kolibri/backend/bn/structure/no_tears_tf_bak.py
+Comment: 
+
+Filename: kolibri/backend/bn/structure/nonlinear.py
+Comment: 
+
+Filename: kolibri/backend/bn/structure/notears_tf2.py
+Comment: 
+
+Filename: kolibri/backend/bn/structure/plot_dag.py
+Comment: 
+
+Filename: kolibri/backend/bn/structure/structure_model.py
+Comment: 
+
+Filename: kolibri/backend/generators/__init__.py
+Comment: 
+
 Filename: kolibri/backend/sklearn/__init__.py
 Comment: 
 
+Filename: kolibri/backend/sklearn/extensions/__init__.py
+Comment: 
+
+Filename: kolibri/backend/sklearn/extensions/decision_tree_log_reg.py
+Comment: 
+
+Filename: kolibri/backend/sklearn/extensions/distributed_nn.py
+Comment: 
+
+Filename: kolibri/backend/sklearn/extensions/lazy_learner.py
+Comment: 
+
+Filename: kolibri/backend/sklearn/extensions/lookup_learner.py
+Comment: 
+
 Filename: kolibri/backend/sklearn/meta/__init__.py
 Comment: 
 
 Filename: kolibri/backend/sklearn/meta/chain_model.py
 Comment: 
 
 Filename: kolibri/backend/sklearn/meta/ecoc_model.py
@@ -120,27 +357,18 @@
 
 Filename: kolibri/backend/sklearn/meta/ecoc/sffs.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/__init__.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/callbacks.py
+Filename: kolibri/backend/tensorflow/logger.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/custom_loses.py
-Comment: 
-
-Filename: kolibri/backend/tensorflow/loader.py
-Comment: 
-
-Filename: kolibri/backend/tensorflow/loader_albert.py
-Comment: 
-
-Filename: kolibri/backend/tensorflow/utils.py
+Filename: kolibri/backend/tensorflow/macros.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/autoencoder/__init__.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/autoencoder/base_autoencoder.py
 Comment: 
@@ -174,105 +402,144 @@
 
 Filename: kolibri/backend/tensorflow/autoencoder/encoders/lstm_encoder.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/callbacks/__init__.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/callbacks/connl_callBack.py
+Filename: kolibri/backend/tensorflow/callbacks/conll_call_back.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/callbacks/eval_callBack.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/cells/BayesianLSTM.py
-Comment: 
-
-Filename: kolibri/backend/tensorflow/cells/__init__.py
+Filename: kolibri/backend/tensorflow/callbacks/save_callback.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/cells/variational_posterior.py
+Filename: kolibri/backend/tensorflow/embeddings/__init__.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/embeddings/__init__.py
+Filename: kolibri/backend/tensorflow/embeddings/bare_embedding.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/embeddings/base_embedding.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/embeddings/bert_embedding.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/embeddings/default_embedding.py
-Comment: 
-
 Filename: kolibri/backend/tensorflow/embeddings/elmo_embedding.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/embeddings/embedding_trainer.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/embeddings/fasttext_embedding.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/embeddings/glove_embedding.py
 Comment: 
 
+Filename: kolibri/backend/tensorflow/embeddings/loader.py
+Comment: 
+
+Filename: kolibri/backend/tensorflow/embeddings/loader_albert.py
+Comment: 
+
 Filename: kolibri/backend/tensorflow/embeddings/numeric_feature_embedding.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/embeddings/stacked_embedding.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/embeddings/transformer_embedding.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/embeddings/word_embedding.py
 Comment: 
 
+Filename: kolibri/backend/tensorflow/gan/__init__.py
+Comment: 
+
+Filename: kolibri/backend/tensorflow/gan/_transformer.py
+Comment: 
+
+Filename: kolibri/backend/tensorflow/gan/bgm.py
+Comment: 
+
+Filename: kolibri/backend/tensorflow/gan/discriminator.py
+Comment: 
+
+Filename: kolibri/backend/tensorflow/gan/generator.py
+Comment: 
+
+Filename: kolibri/backend/tensorflow/gan/ohe.py
+Comment: 
+
 Filename: kolibri/backend/tensorflow/layers/__init__.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/layers/att_wgt_avg_layer.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/layers/behdanau_attention.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/layers/bert_embeddings.py
+Filename: kolibri/backend/tensorflow/layers/conditional_random_field.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/layers/crf.py
+Filename: kolibri/backend/tensorflow/layers/folding_layer.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/layers/folding_layer.py
+Filename: kolibri/backend/tensorflow/layers/gen_activation.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/layers/highway_layer.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/layers/kmax_pool_layer.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/layers/layer.py
+Filename: kolibri/backend/tensorflow/layers/layer_utils.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/layers/multi_head_attention.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/layers/non_masking_layer.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/tasks/__init__.py
+Filename: kolibri/backend/tensorflow/layers/residual.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/tasks/base_model.py
+Filename: kolibri/backend/tensorflow/losses/__init__.py
+Comment: 
+
+Filename: kolibri/backend/tensorflow/losses/conditional_loss.py
+Comment: 
+
+Filename: kolibri/backend/tensorflow/losses/custom_loses.py
+Comment: 
+
+Filename: kolibri/backend/tensorflow/losses/gradient_penalty.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/tasks/dnn_estimator.py
+Filename: kolibri/backend/tensorflow/metrics/__init__.py
+Comment: 
+
+Filename: kolibri/backend/tensorflow/metrics/multi_label_classification.py
+Comment: 
+
+Filename: kolibri/backend/tensorflow/metrics/sequence_labeling.py
+Comment: 
+
+Filename: kolibri/backend/tensorflow/tasks/__init__.py
+Comment: 
+
+Filename: kolibri/backend/tensorflow/tasks/base_model.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/tasks/structured/__init__.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/tasks/structured/base_model.py
 Comment: 
@@ -285,18 +552,21 @@
 
 Filename: kolibri/backend/tensorflow/tasks/structured/regression/dnn_regression_estimator.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/tasks/structured/regression/models.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/tasks/text/__init__.py
+Filename: kolibri/backend/tensorflow/tasks/structured/synthetic/__init__.py
+Comment: 
+
+Filename: kolibri/backend/tensorflow/tasks/structured/synthetic/_synthesizer.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/tasks/text/base_model.py
+Filename: kolibri/backend/tensorflow/tasks/text/__init__.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/tasks/text/classification/__init__.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/tasks/text/classification/base_model.py
 Comment: 
@@ -306,59 +576,86 @@
 
 Filename: kolibri/backend/tensorflow/tasks/text/classification/dpcnn_model.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/tasks/text/classification/models.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/tasks/text/classification/multi_input_output_model.py
+Filename: kolibri/backend/tensorflow/tasks/text/labeling/__init__.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/tasks/text/classification/auto/__init__.py
+Filename: kolibri/backend/tensorflow/tasks/text/labeling/base_model.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/tasks/text/classification/auto/models.py
+Filename: kolibri/backend/tensorflow/tasks/text/labeling/bi_gru_crf_model.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/tasks/text/labeling/__init__.py
+Filename: kolibri/backend/tensorflow/tasks/text/labeling/bi_gru_model.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/tasks/text/labeling/base_model.py
+Filename: kolibri/backend/tensorflow/tasks/text/labeling/bi_lstm_crf_model.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/tasks/text/labeling/experimental.py
+Filename: kolibri/backend/tensorflow/tasks/text/labeling/bi_lstm_model.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/tasks/text/labeling/models.py
+Filename: kolibri/backend/tensorflow/tasks/text/labeling/cnn_lstm_model.py
 Comment: 
 
 Filename: kolibri/backend/tensorflow/tasks/text/seq2seq/__init__.py
 Comment: 
 
+Filename: kolibri/backend/tensorflow/tasks/text/seq2seq/generator.py
+Comment: 
+
 Filename: kolibri/backend/tensorflow/tasks/text/seq2seq/model.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/transformer/__init__.py
+Filename: kolibri/backend/tensorflow/utils/__init__.py
+Comment: 
+
+Filename: kolibri/backend/tensorflow/utils/_load_demo.py
+Comment: 
+
+Filename: kolibri/backend/tensorflow/utils/data.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/transformer/attention.py
+Filename: kolibri/backend/tensorflow/utils/model.py
 Comment: 
 
-Filename: kolibri/backend/tensorflow/transformer/model.py
+Filename: kolibri/backend/tensorflow/utils/multi_label.py
+Comment: 
+
+Filename: kolibri/backend/tensorflow/utils/serialize.py
 Comment: 
 
 Filename: kolibri/backend/torch/__init__.py
 Comment: 
 
 Filename: kolibri/backend/torch/base_model.py
 Comment: 
 
+Filename: kolibri/backend/torch/models.py
+Comment: 
+
 Filename: kolibri/backend/torch/utils.py
 Comment: 
 
+Filename: kolibri/backend/torch/golem_utils/__init__.py
+Comment: 
+
+Filename: kolibri/backend/torch/golem_utils/golem_model.py
+Comment: 
+
+Filename: kolibri/backend/torch/golem_utils/train.py
+Comment: 
+
+Filename: kolibri/backend/torch/golem_utils/utils.py
+Comment: 
+
 Filename: kolibri/backend/torch/layers/__init__.py
 Comment: 
 
 Filename: kolibri/backend/torch/layers/crf.py
 Comment: 
 
 Filename: kolibri/backend/torch/tasks/__init__.py
@@ -369,20 +666,41 @@
 
 Filename: kolibri/backend/torch/tasks/text/labeling/__init__.py
 Comment: 
 
 Filename: kolibri/backend/torch/tasks/text/labeling/bi_lstm_crf.py
 Comment: 
 
+Filename: kolibri/backend/torch/utils/__init__.py
+Comment: 
+
+Filename: kolibri/backend/torch/utils/lbfgsb_scipy.py
+Comment: 
+
+Filename: kolibri/backend/torch/utils/locally_connected.py
+Comment: 
+
+Filename: kolibri/bin/__init__.py
+Comment: 
+
+Filename: kolibri/bin/datasets_configs.json
+Comment: 
+
+Filename: kolibri/bin/kolibri-download.py
+Comment: 
+
 Filename: kolibri/core/__init__.py
 Comment: 
 
 Filename: kolibri/core/component.py
 Comment: 
 
+Filename: kolibri/core/document.py
+Comment: 
+
 Filename: kolibri/core/entity.py
 Comment: 
 
 Filename: kolibri/core/modules.py
 Comment: 
 
 Filename: kolibri/core/pipeline.py
@@ -393,23 +711,116 @@
 
 Filename: kolibri/core/vocabulary.py
 Comment: 
 
 Filename: kolibri/data/__init__.py
 Comment: 
 
+Filename: kolibri/data/auto_downloader.py
+Comment: 
+
+Filename: kolibri/data/base_stream.py
+Comment: 
+
+Filename: kolibri/data/blob.py
+Comment: 
+
+Filename: kolibri/data/dataset.py
+Comment: 
+
+Filename: kolibri/data/document.py
+Comment: 
+
 Filename: kolibri/data/downloader.py
 Comment: 
 
+Filename: kolibri/data/file_stream.py
+Comment: 
+
+Filename: kolibri/data/iterator.py
+Comment: 
+
+Filename: kolibri/data/resources.py
+Comment: 
+
+Filename: kolibri/data/schemes.py
+Comment: 
+
 Filename: kolibri/data/settings.py
 Comment: 
 
+Filename: kolibri/data/streams.py
+Comment: 
+
+Filename: kolibri/data/text.py
+Comment: 
+
 Filename: kolibri/data/utils.py
 Comment: 
 
+Filename: kolibri/data/format/__init__.py
+Comment: 
+
+Filename: kolibri/data/format/conll.py
+Comment: 
+
+Filename: kolibri/data/format/csv.py
+Comment: 
+
+Filename: kolibri/data/loaders/__init__.py
+Comment: 
+
+Filename: kolibri/data/loaders/arxiv.py
+Comment: 
+
+Filename: kolibri/data/loaders/base.py
+Comment: 
+
+Filename: kolibri/data/loaders/csv_loader.py
+Comment: 
+
+Filename: kolibri/data/loaders/pdf.py
+Comment: 
+
+Filename: kolibri/data/loaders/text.py
+Comment: 
+
+Filename: kolibri/data/loaders/web_base.py
+Comment: 
+
+Filename: kolibri/data/parsers/__init__.py
+Comment: 
+
+Filename: kolibri/data/parsers/audio.py
+Comment: 
+
+Filename: kolibri/data/parsers/base.py
+Comment: 
+
+Filename: kolibri/data/parsers/generic.py
+Comment: 
+
+Filename: kolibri/data/parsers/pdf.py
+Comment: 
+
+Filename: kolibri/data/parsers/registry.py
+Comment: 
+
+Filename: kolibri/data/parsers/txt.py
+Comment: 
+
+Filename: kolibri/data/parsers/html/__init__.py
+Comment: 
+
+Filename: kolibri/data/parsers/html/bs4.py
+Comment: 
+
+Filename: kolibri/data/parsers/html/hyperlinks.py
+Comment: 
+
 Filename: kolibri/data/text/__init__.py
 Comment: 
 
 Filename: kolibri/data/text/base_stream.py
 Comment: 
 
 Filename: kolibri/data/text/corpus.py
@@ -483,14 +894,35 @@
 
 Filename: kolibri/datasets/reader/dstc2.py
 Comment: 
 
 Filename: kolibri/datasets/reader/snips.py
 Comment: 
 
+Filename: kolibri/distances/__init__.py
+Comment: 
+
+Filename: kolibri/distances/base_categorical.py
+Comment: 
+
+Filename: kolibri/distances/eskin.py
+Comment: 
+
+Filename: kolibri/distances/goodall.py
+Comment: 
+
+Filename: kolibri/distances/heom.py
+Comment: 
+
+Filename: kolibri/distances/hvdm.py
+Comment: 
+
+Filename: kolibri/distances/lin.py
+Comment: 
+
 Filename: kolibri/evaluation/__init__.py
 Comment: 
 
 Filename: kolibri/evaluation/classifier_evaluator.py
 Comment: 
 
 Filename: kolibri/evaluation/clustering_evaluator.py
@@ -519,14 +951,29 @@
 
 Filename: kolibri/evaluation/metrics/regression.py
 Comment: 
 
 Filename: kolibri/evaluation/metrics/time_series.py
 Comment: 
 
+Filename: kolibri/evaluators/__init__.py
+Comment: 
+
+Filename: kolibri/evaluators/classifier_evaluator.py
+Comment: 
+
+Filename: kolibri/evaluators/clustering_evaluator.py
+Comment: 
+
+Filename: kolibri/evaluators/model_plot.py
+Comment: 
+
+Filename: kolibri/evaluators/synthetic_data.py
+Comment: 
+
 Filename: kolibri/experiment_tracking/__init__.py
 Comment: 
 
 Filename: kolibri/experiment_tracking/experiment_logger.py
 Comment: 
 
 Filename: kolibri/experiment_tracking/mlflow_logger.py
@@ -573,30 +1020,36 @@
 
 Filename: kolibri/features/text/tfidf_weighted_embedder.py
 Comment: 
 
 Filename: kolibri/features/text/embedders/__init__.py
 Comment: 
 
-Filename: kolibri/features/text/embedders/abstract_embedder.py
+Filename: kolibri/features/text/embedders/base.py
 Comment: 
 
 Filename: kolibri/features/text/embedders/bow_embedder.py
 Comment: 
 
 Filename: kolibri/features/text/embedders/elmo_embedder.py
 Comment: 
 
 Filename: kolibri/features/text/embedders/fasttext_embedder.py
 Comment: 
 
 Filename: kolibri/features/text/embedders/glove_embedder.py
 Comment: 
 
-Filename: kolibri/features/text/embedders/transformers_embedder.py
+Filename: kolibri/features/text/embedders/llamacpp.py
+Comment: 
+
+Filename: kolibri/features/text/embedders/openai.py
+Comment: 
+
+Filename: kolibri/features/text/embedders/tensorflow_hub.py
 Comment: 
 
 Filename: kolibri/features/timeseries/__init__.py
 Comment: 
 
 Filename: kolibri/features/timeseries/features_utils.py
 Comment: 
@@ -660,14 +1113,17 @@
 
 Filename: kolibri/indexers/__init__.py
 Comment: 
 
 Filename: kolibri/indexers/base_indexer.py
 Comment: 
 
+Filename: kolibri/indexers/kolibri_label_encoder.py
+Comment: 
+
 Filename: kolibri/indexers/label_indexer.py
 Comment: 
 
 Filename: kolibri/indexers/multi_content_indexer.py
 Comment: 
 
 Filename: kolibri/indexers/multi_target_indexer.py
@@ -684,17 +1140,23 @@
 
 Filename: kolibri/knowledge/__init__.py
 Comment: 
 
 Filename: kolibri/knowledge/domain.py
 Comment: 
 
+Filename: kolibri/mlflow/__init__.py
+Comment: 
+
 Filename: kolibri/optimizers/__init__.py
 Comment: 
 
+Filename: kolibri/optimizers/metric.py
+Comment: 
+
 Filename: kolibri/optimizers/optuna/__init__.py
 Comment: 
 
 Filename: kolibri/optimizers/optuna/objective.py
 Comment: 
 
 Filename: kolibri/optimizers/optuna/tuner.py
@@ -714,80 +1176,35 @@
 
 Filename: kolibri/output/progress_bar.py
 Comment: 
 
 Filename: kolibri/preprocess/__init__.py
 Comment: 
 
-Filename: kolibri/preprocess/preprocessors/__init__.py
-Comment: 
-
-Filename: kolibri/preprocess/preprocessors/bert_preprocessor.py
-Comment: 
-
-Filename: kolibri/preprocess/preprocessors/capitalization.py
-Comment: 
-
-Filename: kolibri/preprocess/preprocessors/char_splitter.py
-Comment: 
-
-Filename: kolibri/preprocess/preprocessors/dirty_comments_preprocessor.py
-Comment: 
-
-Filename: kolibri/preprocess/preprocessors/mask.py
-Comment: 
-
-Filename: kolibri/preprocess/preprocessors/ner_preprocessor.py
-Comment: 
-
-Filename: kolibri/preprocess/preprocessors/odqa_preprocessors.py
-Comment: 
-
-Filename: kolibri/preprocess/preprocessors/random_embeddings_matrix.py
-Comment: 
-
-Filename: kolibri/preprocess/preprocessors/re_preprocessor.py
-Comment: 
-
-Filename: kolibri/preprocess/preprocessors/response_base_loader.py
-Comment: 
-
-Filename: kolibri/preprocess/preprocessors/sanitizer.py
-Comment: 
-
-Filename: kolibri/preprocess/preprocessors/sentseg_preprocessor.py
-Comment: 
-
-Filename: kolibri/preprocess/preprocessors/siamese_preprocessor.py
-Comment: 
-
-Filename: kolibri/preprocess/preprocessors/squad_preprocessor.py
-Comment: 
-
-Filename: kolibri/preprocess/preprocessors/str_token_reverser.py
-Comment: 
-
-Filename: kolibri/preprocess/preprocessors/str_utf8_encoder.py
-Comment: 
-
-Filename: kolibri/preprocess/preprocessors/transformers_preprocessor.py
+Filename: kolibri/preprocess/tabular/DataFrameVectorizer.py
 Comment: 
 
 Filename: kolibri/preprocess/tabular/__init__.py
 Comment: 
 
 Filename: kolibri/preprocess/tabular/binning.py
 Comment: 
 
 Filename: kolibri/preprocess/tabular/boruta_py.py
 Comment: 
 
+Filename: kolibri/preprocess/tabular/category_transformer.py
+Comment: 
+
 Filename: kolibri/preprocess/tabular/cluster.py
 Comment: 
 
+Filename: kolibri/preprocess/tabular/columns_remover.py
+Comment: 
+
 Filename: kolibri/preprocess/tabular/columns_transfromer.py
 Comment: 
 
 Filename: kolibri/preprocess/tabular/data_imputer.py
 Comment: 
 
 Filename: kolibri/preprocess/tabular/dummy_converter.py
@@ -846,35 +1263,74 @@
 
 Filename: kolibri/preprocess/tabular/zero_variance_remover.py
 Comment: 
 
 Filename: kolibri/preprocess/text/__init__.py
 Comment: 
 
+Filename: kolibri/preprocess/text/capitalization.py
+Comment: 
+
+Filename: kolibri/preprocess/text/char_splitter.py
+Comment: 
+
 Filename: kolibri/preprocess/text/collocation_analyzer.py
 Comment: 
 
 Filename: kolibri/preprocess/text/context_builder.py
 Comment: 
 
-Filename: kolibri/preprocess/text/email_cleaner.py
+Filename: kolibri/preprocess/text/dirty_comments_preprocessor.py
+Comment: 
+
+Filename: kolibri/preprocess/text/doc_chuncker.py
+Comment: 
+
+Filename: kolibri/preprocess/text/mask.py
+Comment: 
+
+Filename: kolibri/preprocess/text/ner_preprocessor.py
+Comment: 
+
+Filename: kolibri/preprocess/text/random_embeddings_matrix.py
+Comment: 
+
+Filename: kolibri/preprocess/text/re_preprocessor.py
+Comment: 
+
+Filename: kolibri/preprocess/text/siamese_preprocessor.py
+Comment: 
+
+Filename: kolibri/preprocess/text/str_token_reverser.py
+Comment: 
+
+Filename: kolibri/preprocess/text/str_utf8_encoder.py
+Comment: 
+
+Filename: kolibri/preprocess/text/text_splitter.py
+Comment: 
+
+Filename: kolibri/preprocess/text/transformers_preprocessor.py
 Comment: 
 
 Filename: kolibri/preprocess/text/cleaning/__email_configs.py
 Comment: 
 
 Filename: kolibri/preprocess/text/cleaning/__init__.py
 Comment: 
 
 Filename: kolibri/preprocess/text/cleaning/cleaning_scripts.py
 Comment: 
 
 Filename: kolibri/preprocess/text/cleaning/email2text.py
 Comment: 
 
+Filename: kolibri/preprocess/text/cleaning/email_cleaner.py
+Comment: 
+
 Filename: kolibri/preprocess/text/cleaning/email_parser.py
 Comment: 
 
 Filename: kolibri/preprocess/text/cleaning/header_parser.py
 Comment: 
 
 Filename: kolibri/preprocess/text/language_detection/__init__.py
@@ -906,15 +1362,15 @@
 
 Filename: kolibri/preprocess/timeseries/__init__.py
 Comment: 
 
 Filename: kolibri/preprocess/timeseries/multi_window_generator.py
 Comment: 
 
-Filename: kolibri/preprocess/timeseries/multi_window_generator_.py
+Filename: kolibri/preprocess/timeseries/multi_window_generator_back.py
 Comment: 
 
 Filename: kolibri/preprocess/timeseries/time_series_from_array.py
 Comment: 
 
 Filename: kolibri/preprocess/timeseries/window.py
 Comment: 
@@ -924,51 +1380,141 @@
 
 Filename: kolibri/samplers/__init__.py
 Comment: 
 
 Filename: kolibri/samplers/auto_smpler.py
 Comment: 
 
+Filename: kolibri/samplers/conditional.py
+Comment: 
+
+Filename: kolibri/samplers/data_sampler.py
+Comment: 
+
+Filename: kolibri/samplers/smoteR.py
+Comment: 
+
+Filename: kolibri/scripts/__init__.py
+Comment: 
+
+Filename: kolibri/scripts/check_requirements.py
+Comment: 
+
+Filename: kolibri/scripts/install_plugin_deps.py
+Comment: 
+
 Filename: kolibri/stopwords/__init__.py
 Comment: 
 
 Filename: kolibri/stopwords/stp_wrd.py
 Comment: 
 
-Filename: kolibri/task/__init__.py
+Filename: kolibri/synthetic_data/__init__.py
 Comment: 
 
-Filename: kolibri/task/audio/__init__.py
+Filename: kolibri/synthetic_data/anonymization.py
 Comment: 
 
-Filename: kolibri/task/audio/base_model.py
+Filename: kolibri/synthetic_data/base.py
 Comment: 
 
-Filename: kolibri/task/audio/classification/__init__.py
+Filename: kolibri/synthetic_data/base_contraint.py
 Comment: 
 
-Filename: kolibri/task/audio/classification/dnn_audio_estimator.py
+Filename: kolibri/synthetic_data/copulagan.py
 Comment: 
 
-Filename: kolibri/task/audio/classification/models.py
+Filename: kolibri/synthetic_data/copulas.py
+Comment: 
+
+Filename: kolibri/synthetic_data/ctgan_synthesizer.py
+Comment: 
+
+Filename: kolibri/synthetic_data/data_processor.py
+Comment: 
+
+Filename: kolibri/synthetic_data/metadata.py
+Comment: 
+
+Filename: kolibri/synthetic_data/single_table.py
+Comment: 
+
+Filename: kolibri/synthetic_data/synthpop.py
+Comment: 
+
+Filename: kolibri/synthetic_data/utils.py
+Comment: 
+
+Filename: kolibri/synthetic_data/benchmark/__init__.py
+Comment: 
+
+Filename: kolibri/synthetic_data/benchmark/benchmark.py
+Comment: 
+
+Filename: kolibri/synthetic_data/benchmark/data.py
+Comment: 
+
+Filename: kolibri/synthetic_data/benchmark/metrics.py
+Comment: 
+
+Filename: kolibri/synthetic_data/benchmark/ml.py
+Comment: 
+
+Filename: kolibri/synthetic_data/benchmark/privacy.py
+Comment: 
+
+Filename: kolibri/synthetic_data/benchmark/reporting.py
+Comment: 
+
+Filename: kolibri/synthetic_data/benchmark/utility.py
+Comment: 
+
+Filename: kolibri/synthetic_data/benchmark/utils.py
+Comment: 
+
+Filename: kolibri/synthetic_data/benchmark/synthesizers/__init__.py
+Comment: 
+
+Filename: kolibri/synthetic_data/benchmark/synthesizers/base.py
 Comment: 
 
-Filename: kolibri/task/audio/nemo/__init__.py
+Filename: kolibri/synthetic_data/benchmark/synthesizers/generate.py
 Comment: 
 
-Filename: kolibri/task/audio/nemo/asr.py
+Filename: kolibri/synthetic_data/benchmark/synthesizers/identity.py
 Comment: 
 
-Filename: kolibri/task/audio/nemo/common.py
+Filename: kolibri/synthetic_data/benchmark/synthesizers/independent.py
 Comment: 
 
-Filename: kolibri/task/audio/nemo/tts.py
+Filename: kolibri/synthetic_data/benchmark/synthesizers/sd.py
 Comment: 
 
-Filename: kolibri/task/audio/nemo/vocoder.py
+Filename: kolibri/synthetic_data/benchmark/synthesizers/uniform.py
+Comment: 
+
+Filename: kolibri/task/__init__.py
+Comment: 
+
+Filename: kolibri/task/dnn_estimator.py
+Comment: 
+
+Filename: kolibri/task/audio/__init__.py
+Comment: 
+
+Filename: kolibri/task/audio/base_model.py
+Comment: 
+
+Filename: kolibri/task/audio/classification/__init__.py
+Comment: 
+
+Filename: kolibri/task/audio/classification/dnn_audio_estimator.py
+Comment: 
+
+Filename: kolibri/task/audio/classification/models.py
 Comment: 
 
 Filename: kolibri/task/tabular/__init__.py
 Comment: 
 
 Filename: kolibri/task/tabular/anomaly/__init__.py
 Comment: 
@@ -996,14 +1542,17 @@
 
 Filename: kolibri/task/tabular/clustering/clustering.py
 Comment: 
 
 Filename: kolibri/task/tabular/regression/__init__.py
 Comment: 
 
+Filename: kolibri/task/tabular/regression/dnn_regression_estimator.py
+Comment: 
+
 Filename: kolibri/task/tabular/regression/sklearn_regression_estimator.py
 Comment: 
 
 Filename: kolibri/task/tabular/rulemining/__init__.py
 Comment: 
 
 Filename: kolibri/task/tabular/rulemining/association_rules.py
@@ -1017,26 +1566,35 @@
 
 Filename: kolibri/task/text/classification/dnn_classification_estimator.py
 Comment: 
 
 Filename: kolibri/task/text/classification/sklearn_classification_estimator.py
 Comment: 
 
+Filename: kolibri/task/text/classification/sklearn_estimator.py
+Comment: 
+
 Filename: kolibri/task/text/entities/__init__.py
 Comment: 
 
 Filename: kolibri/task/text/entities/common_reg_extractor.py
 Comment: 
 
 Filename: kolibri/task/text/entities/crf_entity_extractor.py
 Comment: 
 
 Filename: kolibri/task/text/entities/dictionaryExtractor.py
 Comment: 
 
+Filename: kolibri/task/text/entities/entity.py
+Comment: 
+
+Filename: kolibri/task/text/entities/entity_extractor.py
+Comment: 
+
 Filename: kolibri/task/text/entities/entity_synonyms.py
 Comment: 
 
 Filename: kolibri/task/text/entities/lstm_entity_extractor.py
 Comment: 
 
 Filename: kolibri/task/text/entities/person_extractor.py
@@ -1092,102 +1650,54 @@
 
 Filename: kolibri/task/text/intents/intent_expressions.py
 Comment: 
 
 Filename: kolibri/task/text/intents/domains/__init__.py
 Comment: 
 
-Filename: kolibri/task/text/qa/__init__.py
-Comment: 
-
-Filename: kolibri/task/text/qa/entity_detection_parser.py
-Comment: 
-
-Filename: kolibri/task/text/qa/entity_linking.py
-Comment: 
-
-Filename: kolibri/task/text/qa/kbqa_entity_linking.py
-Comment: 
-
-Filename: kolibri/task/text/qa/query_generator.py
-Comment: 
-
-Filename: kolibri/task/text/qa/query_generator_base.py
-Comment: 
-
-Filename: kolibri/task/text/qa/query_generator_online.py
-Comment: 
-
-Filename: kolibri/task/text/qa/rel_ranking_bert_infer.py
-Comment: 
-
-Filename: kolibri/task/text/qa/rel_ranking_infer.py
-Comment: 
-
-Filename: kolibri/task/text/qa/sentence_answer.py
-Comment: 
-
-Filename: kolibri/task/text/qa/template_matcher.py
-Comment: 
-
-Filename: kolibri/task/text/qa/tree_to_sparql.py
-Comment: 
-
-Filename: kolibri/task/text/qa/utils.py
-Comment: 
-
-Filename: kolibri/task/text/qa/wiki_parser.py
-Comment: 
-
-Filename: kolibri/task/text/qa/wiki_parser_online.py
-Comment: 
-
-Filename: kolibri/task/text/qa/squad/__init__.py
+Filename: kolibri/task/text/sentiment/__init__.py
 Comment: 
 
-Filename: kolibri/task/text/qa/squad/squad.py
+Filename: kolibri/task/text/sentiment/lexicon_sentiment.py
 Comment: 
 
-Filename: kolibri/task/text/qa/squad/utils.py
+Filename: kolibri/task/text/sentiment/util.py
 Comment: 
 
-Filename: kolibri/task/text/relations/__init__.py
+Filename: kolibri/task/text/sentiment/vader.py
 Comment: 
 
-Filename: kolibri/task/text/relations/losses.py
+Filename: kolibri/task/text/similarity/__init__.py
 Comment: 
 
-Filename: kolibri/task/text/relations/relation_extraction_bert.py
+Filename: kolibri/task/text/similarity/arxiv.py
 Comment: 
 
-Filename: kolibri/task/text/retrieval/__init__.py
+Filename: kolibri/task/text/similarity/docarray.py
 Comment: 
 
-Filename: kolibri/task/text/retrieval/logit_ranker.py
+Filename: kolibri/task/text/similarity/knn.py
 Comment: 
 
-Filename: kolibri/task/text/retrieval/pop_ranker.py
+Filename: kolibri/task/text/similarity/llama_index.py
 Comment: 
 
-Filename: kolibri/task/text/retrieval/tfidf_ranker.py
+Filename: kolibri/task/text/similarity/merger_retriever.py
 Comment: 
 
-Filename: kolibri/task/text/retrieval/utils.py
+Filename: kolibri/task/text/similarity/pupmed.py
 Comment: 
 
-Filename: kolibri/task/text/sentiment/__init__.py
+Filename: kolibri/task/text/similarity/svm.py
 Comment: 
 
-Filename: kolibri/task/text/sentiment/lexicon_sentiment.py
+Filename: kolibri/task/text/similarity/tfidf.py
 Comment: 
 
-Filename: kolibri/task/text/sentiment/util.py
-Comment: 
-
-Filename: kolibri/task/text/sentiment/vader.py
+Filename: kolibri/task/text/similarity/wikipedia.py
 Comment: 
 
 Filename: kolibri/task/text/spelling/__init__.py
 Comment: 
 
 Filename: kolibri/task/text/spelling/brillmoore/__init__.py
 Comment: 
@@ -1305,29 +1815,56 @@
 
 Filename: kolibri/tools/__init__.py
 Comment: 
 
 Filename: kolibri/tools/_regex.py
 Comment: 
 
+Filename: kolibri/tools/arxiv.py
+Comment: 
+
+Filename: kolibri/tools/bing_search.py
+Comment: 
+
+Filename: kolibri/tools/ddg_search.py
+Comment: 
+
 Filename: kolibri/tools/gebbrisg_detector.py
 Comment: 
 
+Filename: kolibri/tools/google_search.py
+Comment: 
+
 Filename: kolibri/tools/keywords.py
 Comment: 
 
+Filename: kolibri/tools/openweathermap.py
+Comment: 
+
+Filename: kolibri/tools/pubmed.py
+Comment: 
+
 Filename: kolibri/tools/regexes.py
 Comment: 
 
 Filename: kolibri/tools/scanner.py
 Comment: 
 
+Filename: kolibri/tools/wikipedia.py
+Comment: 
+
+Filename: kolibri/tools/wolfram_alpha.py
+Comment: 
+
 Filename: kolibri/tools/word_frequencies.py
 Comment: 
 
+Filename: kolibri/tools/youtube_search.py
+Comment: 
+
 Filename: kolibri/utils/__init__.py
 Comment: 
 
 Filename: kolibri/utils/cm.py
 Comment: 
 
 Filename: kolibri/utils/common.py
@@ -1338,140 +1875,224 @@
 
 Filename: kolibri/utils/cross_validation.py
 Comment: 
 
 Filename: kolibri/utils/distribution.py
 Comment: 
 
+Filename: kolibri/utils/environement.py
+Comment: 
+
+Filename: kolibri/utils/language_info.py
+Comment: 
+
 Filename: kolibri/utils/log_normalizer.py
 Comment: 
 
+Filename: kolibri/utils/mathext.py
+Comment: 
+
+Filename: kolibri/utils/matrix.py
+Comment: 
+
+Filename: kolibri/utils/nb_clusters.py
+Comment: 
+
+Filename: kolibri/utils/parallel.py
+Comment: 
+
+Filename: kolibri/utils/progress_bar.py
+Comment: 
+
+Filename: kolibri/utils/serializable.py
+Comment: 
+
+Filename: kolibri/utils/spinner.py
+Comment: 
+
+Filename: kolibri/utils/text_encoding.py
+Comment: 
+
 Filename: kolibri/utils/timeseries_functions.py
 Comment: 
 
-Filename: kolibri/visualizations/__init__.py
+Filename: kolibri/utils/timeseries_functions_back.py
 Comment: 
 
-Filename: kolibri/visualizations/classification_plots.py
+Filename: kolibri/utils/wrappers/__init__.py
 Comment: 
 
-Filename: kolibri/visualizations/pipeline.py
+Filename: kolibri/utils/wrappers/arxiv.py
 Comment: 
 
-Filename: kolibri/visualizations/regression_plots.py
+Filename: kolibri/utils/wrappers/bing_search.py
 Comment: 
 
-Filename: kolibri/visualizations/utils.py
+Filename: kolibri/utils/wrappers/duckduckgo_search.py
+Comment: 
+
+Filename: kolibri/utils/wrappers/google_search.py
+Comment: 
+
+Filename: kolibri/utils/wrappers/openweathermap.py
+Comment: 
+
+Filename: kolibri/utils/wrappers/pupmed.py
+Comment: 
+
+Filename: kolibri/utils/wrappers/wikipedia.py
+Comment: 
+
+Filename: kolibri/utils/wrappers/wolfram_alpha.py
+Comment: 
+
+Filename: kolibri/vectordb/__init__.py
+Comment: 
+
+Filename: kolibri/vectordb/base.py
+Comment: 
+
+Filename: kolibri/vectordb/faiss.py
+Comment: 
+
+Filename: kolibri/vectordb/redis.py
+Comment: 
+
+Filename: kolibri/vectordb/sklearn.py
+Comment: 
+
+Filename: kolibri/vectordb/utils.py
 Comment: 
 
-Filename: test_backup/__init__.py
+Filename: kolibri/vectordb/docarray/__init__.py
 Comment: 
 
-Filename: test_backup/dnn/__init__.py
+Filename: kolibri/vectordb/docarray/base.py
 Comment: 
 
-Filename: test_backup/dnn/audio/__init__.py
+Filename: kolibri/vectordb/docarray/hnsw.py
 Comment: 
 
-Filename: test_backup/dnn/audio/test_classification/__init__.py
+Filename: kolibri/vectordb/docarray/in_memory.py
 Comment: 
 
-Filename: test_backup/dnn/audio/test_classification/test_pipeline_model.py
+Filename: kolibri/vectordb/docstore/__init__.py
 Comment: 
 
-Filename: test_backup/dnn/text/__init__.py
+Filename: kolibri/vectordb/docstore/arbitrary_fn.py
 Comment: 
 
-Filename: test_backup/dnn/text/test_classification/__init__.py
+Filename: kolibri/vectordb/docstore/base.py
+Comment: 
+
+Filename: kolibri/vectordb/docstore/in_memory.py
+Comment: 
+
+Filename: kolibri/vectordb/docstore/wikipedia.py
+Comment: 
+
+Filename: kolibri/visualizations/__init__.py
+Comment: 
+
+Filename: kolibri/visualizations/classification_plots.py
+Comment: 
+
+Filename: kolibri/visualizations/pipeline.py
+Comment: 
+
+Filename: kolibri/visualizations/regression_plots.py
+Comment: 
+
+Filename: kolibri/visualizations/utils.py
 Comment: 
 
-Filename: test_backup/dnn/text/test_classification/test_bi_gru_model.py
+Filename: tests/__init__.py
 Comment: 
 
-Filename: test_backup/dnn/text/test_classification/test_bi_lstm_model.py
+Filename: tests/test_data_transformer.py
 Comment: 
 
-Filename: test_backup/dnn/text/test_classification/test_cnn_attention_model.py
+Filename: tests/test_pipeline.py
 Comment: 
 
-Filename: test_backup/dnn/text/test_classification/test_cnn_gru_model.py
+Filename: tests/utils.py
 Comment: 
 
-Filename: test_backup/dnn/text/test_classification/test_cnn_lstm_model.py
+Filename: tests/entities/__init__.py
 Comment: 
 
-Filename: test_backup/dnn/text/test_classification/test_cnn_model.py
+Filename: tests/entities/test.py
 Comment: 
 
-Filename: test_backup/dnn/text/test_embeddings/__init__.py
+Filename: tests/optuna/__init__.py
 Comment: 
 
-Filename: test_backup/dnn/text/test_embeddings/test_default_embedding.py
+Filename: tests/optuna/test_optuna.py
 Comment: 
 
-Filename: test_backup/dnn/text/test_embeddings/test_word_embedding.py
+Filename: tests/synthesizer/__init__.py
 Comment: 
 
-Filename: test_backup/dnn/text/test_indexer/__init__.py
+Filename: tests/synthesizer/data_modules/__init__.py
 Comment: 
 
-Filename: test_backup/dnn/text/test_indexer/test_label_indexer.py
+Filename: tests/synthesizer/data_modules/test_conditional.py
 Comment: 
 
-Filename: test_backup/dnn/text/test_indexer/test_multi_content_indexer.py
+Filename: tests/synthesizer/data_modules/test_sampler.py
 Comment: 
 
-Filename: test_backup/dnn/text/test_indexer/test_multi_target_indexer.py
+Filename: tests/synthesizer/data_modules/test_transformer.py
 Comment: 
 
-Filename: test_backup/dnn/text/test_indexer/test_sequence_char_indexer.py
+Filename: tests/synthesizer/layers/__init__.py
 Comment: 
 
-Filename: test_backup/dnn/text/test_indexer/test_sequence_indexer.py
+Filename: tests/synthesizer/layers/test_gen_activation.py
 Comment: 
 
-Filename: test_backup/dnn/text/test_labeling/__init__.py
+Filename: tests/synthesizer/layers/test_layer_utils.py
 Comment: 
 
-Filename: test_backup/dnn/text/test_labeling/test_bi_gru_model.py
+Filename: tests/synthesizer/layers/test_residual.py
 Comment: 
 
-Filename: test_backup/dnn/text/test_labeling/test_bi_lstm_crf_model.py
+Filename: tests/synthesizer/losses/__init__.py
 Comment: 
 
-Filename: test_backup/dnn/text/test_labeling/test_bi_lstm_model.py
+Filename: tests/synthesizer/losses/test_conditional_loss.py
 Comment: 
 
-Filename: test_backup/dnn/text/test_labeling/test_cnn_lstm_model.py
+Filename: tests/synthesizer/losses/test_gradient_penalty.py
 Comment: 
 
-Filename: test_backup/dnn/text/test_seq2seq/__init__.py
+Filename: tests/synthesizer/models/__init__.py
 Comment: 
 
-Filename: test_backup/dnn/text/test_seq2seq/test_seq2seq.py
+Filename: tests/synthesizer/models/test_critic.py
 Comment: 
 
-Filename: test_backup/entities/__init__.py
+Filename: tests/synthesizer/models/test_generator.py
 Comment: 
 
-Filename: test_backup/entities/test.py
+Filename: tests/synthesizer/synthesizer/__init__.py
 Comment: 
 
-Filename: test_backup/optuna/__init__.py
+Filename: tests/synthesizer/synthesizer/test_synthesizer.py
 Comment: 
 
-Filename: test_backup/optuna/test_optuna.py
+Filename: kolibri_ml-1.1.80.dist-info/LICENCE.txt
 Comment: 
 
-Filename: kolibri_ml-1.1.8.dist-info/METADATA
+Filename: kolibri_ml-1.1.80.dist-info/METADATA
 Comment: 
 
-Filename: kolibri_ml-1.1.8.dist-info/WHEEL
+Filename: kolibri_ml-1.1.80.dist-info/WHEEL
 Comment: 
 
-Filename: kolibri_ml-1.1.8.dist-info/top_level.txt
+Filename: kolibri_ml-1.1.80.dist-info/top_level.txt
 Comment: 
 
-Filename: kolibri_ml-1.1.8.dist-info/RECORD
+Filename: kolibri_ml-1.1.80.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kolibri/VERSION

```diff
@@ -1 +1 @@
-1.1.8
+1.1.80
```

## kolibri/__init__.py

```diff
@@ -9,15 +9,38 @@
 The Kolibri toolkit is an open source Python library
 for Artificial Intelligence including Natural Language Processing and general purpose Machine learning with Scikit learn and Deep learning.  
 
 Mohamed Ben Hadou (2017).
 isort:skip_file
 """
 
+
+
+
 import os
+import random
+from dotenv import load_dotenv
+
+if "pytest" in sys.argv or "pytest" in sys.modules or os.getenv("CI"):
+    print("Setting random seed to 42")
+    random.seed(42)
+
+# Load the users .env file into environment variables
+load_dotenv(verbose=True, override=True)
+
+del load_dotenv
+verbose=1
+
+from dotenv import load_dotenv
+
+# Load the users .env file into environment variables
+load_dotenv(verbose=True, override=True)
+
+del load_dotenv
+verbose=1
 
 # //////////////////////////////////////////////////////
 # Metadata
 # //////////////////////////////////////////////////////
 
 # Version.  For each new release, the version number should be updated
 # in the file VERSION.
@@ -130,14 +153,15 @@
 
 
 
 from kolibri.data.downloader import download, download_shell
 from kolibri.config import ModelConfig
 from kolibri.model_loader import ModelLoader
 from kolibri.model_trainer import ModelTrainer
+from kolibri.backend import *
 try:
     from kolibri.backend.tensorflow import tasks
 except:
     pass
 
 
 ####################
```

## kolibri/app.py

```diff
@@ -149,15 +149,15 @@
     a step size defined in ``grid_interval`` parameter. This function will display
     a plot of the performance metrics at each probability threshold and returns the
     best model based on the metric defined under ``optimize`` parameter.
 
 
     Example
     -------
-    >>> from pycaret.datasets import get_data
+    >>> from kolibri.datasets import get_data
     >>> juice = get_data('juice')
     >>> experiment_name = setup(data = juice,  target = 'Purchase')
     >>> lr = create_model('lr')
     >>> best_lr_threshold = optimize_threshold(lr)
 
 
     Parameters
@@ -211,17 +211,17 @@
 ):
     """
     This function deploys the transformation pipeline and trained model on cloud.
 
 
     Example
     -------
-    >>> from pycaret.datasets import get_data
+    >>> from kolibri.datasets import get_data
     >>> juice = get_data('juice')
-    >>> from pycaret.classification import *
+    >>> from kolibri.classification import *
     >>> exp_name = setup(data = juice,  target = 'Purchase')
     >>> lr = create_model('lr')
     >>> # sets appropriate credentials for the platform as environment variables
     >>> import os
     >>> os.environ["AWS_ACCESS_KEY_ID"] = str("foo")
     >>> os.environ["AWS_SECRET_ACCESS_KEY"] = str("bar")
     >>> deploy_model(model = lr, model_name = 'lr-for-deployment', platform = 'aws', authentication = {'bucket' : 'S3-bucket-name'})
@@ -306,17 +306,17 @@
     Ruby, F#). This functionality is very useful if you want to deploy models
     into environments where you can't install your normal Python stack to
     support model inference.
 
 
     Example
     -------
-    >>> from pycaret.datasets import get_data
+    >>> from kolibri.datasets import get_data
     >>> juice = get_data('juice')
-    >>> from pycaret.classification import *
+    >>> from kolibri.classification import *
     >>> exp_name = setup(data = juice,  target = 'Purchase')
     >>> lr = create_model('lr')
     >>> lr_java = convert_model(lr, 'java')
 
 
     estimator: scikit-learn compatible object
         Trained model object
@@ -356,17 +356,17 @@
     This function generates AutoEDA using AutoVIZ library. You must
     install Autoviz separately ``pip install autoviz`` to use this
     function.
 
 
     Example
     -------
-    >>> from pycaret.datasets import get_data
+    >>> from kolibri.datasets import get_data
     >>> juice = get_data('juice')
-    >>> from pycaret.classification import *
+    >>> from kolibri.classification import *
     >>> exp_name = setup(data = juice,  target = 'Purchase')
     >>> eda(display_format = 'bokeh')
 
     display_format: str, default = 'bokeh'
         When set to 'bokeh' the plots are interactive. Other option is ``svg`` for static
         plots that are generated using matplotlib and seaborn.
 
@@ -389,17 +389,17 @@
     the approach known as group fairness, which asks: Which groups of individuals
     are at risk for experiencing harms. This function provides fairness-related
     metrics between different groups (also called subpopulation).
 
 
     Example
     -------
-    >>> from pycaret.datasets import get_data
+    >>> from kolibri.datasets import get_data
     >>> income = get_data('income')
-    >>> from pycaret.classification import *
+    >>> from kolibri.classification import *
     >>> exp_name = setup(data = income,  target = 'income >50K')
     >>> lr = create_model('lr')
     >>> lr_fairness = check_fairness(lr, sensitive_features = ['sex', 'race'])
 
 
     estimator: scikit-learn compatible object
         Trained model object
@@ -434,17 +434,17 @@
     This function takes an input ``estimator`` and creates a POST API for
     inference. It only creates the API and doesn't run it automatically.
     To run the API, you must run the Python file using ``!python``.
 
 
     Example
     -------
-    >>> from pycaret.datasets import get_data
+    >>> from kolibri.datasets import get_data
     >>> juice = get_data('juice')
-    >>> from pycaret.classification import *
+    >>> from kolibri.classification import *
     >>> exp_name = setup(data = juice,  target = 'Purchase')
     >>> lr = create_model('lr')
     >>> create_api(lr, 'lr_api'
     >>> !python lr_api.py
 
 
     estimator: scikit-learn compatible object
@@ -479,17 +479,17 @@
     """
     This function creates a ``Dockerfile`` and ``requirements.txt`` for
     productionalizing API end-point.
 
 
     Example
     -------
-    >>> from pycaret.datasets import get_data
+    >>> from kolibri.datasets import get_data
     >>> juice = get_data('juice')
-    >>> from pycaret.classification import *
+    >>> from kolibri.classification import *
     >>> exp_name = setup(data = juice,  target = 'Purchase')
     >>> lr = create_model('lr')
     >>> create_api(lr, 'lr_api')
     >>> create_docker('lr_api')
 
 
     api_name: str
@@ -519,17 +519,17 @@
     This function creates a basic gradio app for inference.
     It will later be expanded for other app types such as
     Streamlit.
 
 
     Example
     -------
-    >>> from pycaret.datasets import get_data
+    >>> from kolibri.datasets import get_data
     >>> juice = get_data('juice')
-    >>> from pycaret.classification import *
+    >>> from kolibri.classification import *
     >>> exp_name = setup(data = juice,  target = 'Purchase')
     >>> lr = create_model('lr')
     >>> create_app(lr)
 
 
     estimator: scikit-learn compatible object
         Trained model object
@@ -550,17 +550,17 @@
     """
     This function runs a full suite check over a trained model
     using deepchecks library.
 
 
     Example
     -------
-    >>> from pycaret.datasets import get_data
+    >>> from kolibri.datasets import get_data
     >>> juice = get_data('juice')
-    >>> from pycaret.classification import *
+    >>> from kolibri.classification import *
     >>> exp_name = setup(data = juice,  target = 'Purchase')
     >>> lr = create_model('lr')
     >>> deep_check(lr)
 
 
     estimator: scikit-learn compatible object
         Trained model object
```

## kolibri/default_configs.py

```diff
@@ -1,96 +1,104 @@
+import pathlib
+
 from kdmt.path import is_writable
 import os
 import sys
 from kolibri.config_loader import parse_config
 
 __location__ = os.path.realpath(
     os.path.join(os.getcwd(), os.path.dirname(__file__)))
-
 _settings=parse_config(os.path.join(__location__,"settings.yaml"))
-KOLIBRI_DATA_FOLDER = _settings['data']['KOLIBRI_DATA_FOLDER']
 
-RESOURCES_AUTO_DOWNLOAD = _settings['data']['RESOURCES_AUTO_DOWNLOAD']
+#kolibri_data_folder_defined
+KOLIBRI_DATA_FOLDER=os.getenv('KOLIBRI_DATA_PATH', "")
+if KOLIBRI_DATA_FOLDER != "":
+    if os.path.exists(pathlib.Path(KOLIBRI_DATA_FOLDER).parent) and is_writable(pathlib.Path(KOLIBRI_DATA_FOLDER).parent):
+        if not os.path.exists(KOLIBRI_DATA_FOLDER):
+            os.mkdir(KOLIBRI_DATA_FOLDER)
+else:
+    #kolibri dataforlder not defined
 
+    DATA_PATH = []
+    """A list of directories where packages from the Kolibri data are downloaded."""
 
-if RESOURCES_AUTO_DOWNLOAD is None:
-    RESOURCES_AUTO_DOWNLOAD = "true"
-    os.environ['RESOURCES_AUTO_DOWNLOAD'] = RESOURCES_AUTO_DOWNLOAD
-
-
-######################################################################
-# data Path
-######################################################################
-
-DATA_PATH = []
-"""A list of directories where packages from the Kolibri data are downloaded."""
-
-# User-specified locations:
-_paths_from_env = os.environ.get("KOLIBRI_DATA_PATH", "").split(os.pathsep)
-DATA_PATH += [d for d in _paths_from_env if d]
-if "APPENGINE_RUNTIME" not in os.environ and os.path.expanduser("~/") != "~/":
-    DATA_PATH.append(os.path.expanduser("~/.kolibri"))
-
-if sys.platform.startswith("win"):
-    # Common locations on Windows:
-    DATA_PATH += [
-        os.path.join(sys.prefix, ".kolibri"),
-        os.path.join(sys.prefix, "share", ".kolibri"),
-        os.path.join(sys.prefix, "lib", ".kolibri"),
-        os.path.join(os.environ.get("APPDATA", "C:\\"), ".kolibri"),
-        r"C:\.kolibri",
-        r"D:\.kolibri",
-        r"E:\.kolibri",
-    ]
-else:
-    # Common locations on UNIX & OS X:
-    DATA_PATH += [
-        os.path.join(sys.prefix, ".kolibri"),
-        os.path.join(sys.prefix, "share", ".kolibri"),
-        os.path.join(sys.prefix, "lib", ".kolibri"),
-        "/usr/share/.kolibri",
-        "/usr/local/share/.kolibri",
-        "/usr/lib/.kolibri",
-        "/usr/local/lib/.kolibri",
-    ]
+    #User-specified locations:
+
+    if "APPENGINE_RUNTIME" not in os.environ and os.path.expanduser("~/") != "~/":
 
-if KOLIBRI_DATA_FOLDER is None:
+        # On Windows, use %APPDATA%
+        if sys.platform == "win32" and "APPDATA" in os.environ:
+            homedir = os.environ["APPDATA"]
+
+        # Otherwise, install in the user's home directory.
+        else:
+            homedir = os.path.expanduser("~/")
+            if homedir == "~/":
+                raise ValueError("Could not find a default download directory")
+
+            DATA_PATH.append(os.path.join(homedir,".kolibri"))
+
+    if sys.platform.startswith("win"):
+        # Common locations on Windows:
+        DATA_PATH += [
+            os.path.join(sys.prefix, ".kolibri"),
+            os.path.join(sys.prefix, "share", ".kolibri"),
+            os.path.join(sys.prefix, "lib", ".kolibri"),
+            os.path.join(os.environ.get("APPDATA", "C:\\"), ".kolibri"),
+            r"C:\.kolibri",
+            r"D:\.kolibri",
+            r"E:\.kolibri",
+        ]
+    else:
+        # Common locations on UNIX & OS X:
+        DATA_PATH += [
+            os.path.join(sys.prefix, ".kolibri"),
+            os.path.join(sys.prefix, "share", ".kolibri"),
+            os.path.join(sys.prefix, "lib", ".kolibri"),
+            "/usr/share/.kolibri",
+            "/usr/local/share/.kolibri",
+            "/usr/lib/.kolibri",
+            "/usr/local/lib/.kolibri",
+        ]
 
     for kolibridir in DATA_PATH:
         if os.path.exists(kolibridir) and is_writable(kolibridir):
-                KOLIBRI_DATA_FOLDER= kolibridir
+            KOLIBRI_DATA_FOLDER = kolibridir
+            break
 
-    # On Windows, use %APPDATA%
-    if sys.platform == "win32" and "APPDATA" in os.environ:
-        homedir = os.environ["APPDATA"]
 
-    # Otherwise, install in the user's home directory.
-    else:
-        homedir = os.path.expanduser("~/")
-        if homedir == "~/":
-            raise ValueError("Could not find a default download directory")
+        if os.path.exists(pathlib.Path(kolibridir).parent) and is_writable(pathlib.Path(kolibridir).parent):
+            if not os.path.exists(kolibridir):
+                os.mkdir(kolibridir)
+            KOLIBRI_DATA_FOLDER= kolibridir
+            break
+
+RESOURCES_AUTO_DOWNLOAD = os.getenv('RESOURCES_AUTO_DOWNLOAD') or str(_settings['data']['RESOURCES_AUTO_DOWNLOAD'])
+RESOURCES_AUTO_DOWNLOAD=RESOURCES_AUTO_DOWNLOAD.lower()=="true"
 
-        # append ".kolibri" to the home directory
-        KOLIBRI_DATA_FOLDER= os.path.join(homedir, ".kolibri")
 
-    os.environ['KOLIBRI_DATA_PATH'] = KOLIBRI_DATA_FOLDER
+os.environ['KOLIBRI_DATA_PATH'] = KOLIBRI_DATA_FOLDER
 
+LOG_NAME = os.getenv('LOG_NAME') or _settings['logs']['LOG_NAME']
+LOG_LEVEL = os.getenv('LOG_LEVEL') or _settings['logs']['LOG_LEVEL']
+LOG_TO_FILE=os.getenv('LOG_TO_FILE') or str(_settings['logs']['LOG_TO_FILE'])
+LOG_TO_FILE=LOG_TO_FILE.lower()=="true"
 
-LOG_NAME = _settings['logs']['LOG_NAME']
-LOG_LEVEL = _settings['logs']['LOG_LEVEL']
-LOG_TO_FILE=_settings['logs']['LOG_TO_FILE']
 LOGS_DIR = os.path.join(KOLIBRI_DATA_FOLDER, 'logs')
 if LOG_TO_FILE:
     if not os.path.exists(LOGS_DIR):
         try:
             os.mkdir(LOGS_DIR)
         except:
             LOG_TO_FILE=False
             pass
 
-DEFAULT_NN_MODEL_FILENAME=_settings['neural_networks']['DEFAULT_NN_MODEL_FILENAME']
-EMBEDDING_SIZE = _settings['neural_networks']['EMBEDDING_SIZE']
+DEFAULT_NN_MODEL_FILENAME=os.getenv('DEFAULT_NN_MODEL_FILENAME') or _settings['neural_networks']['DEFAULT_NN_MODEL_FILENAME']
+EMBEDDING_SIZE = os.getenv('EMBEDDING_SIZE') or _settings['neural_networks']['EMBEDDING_SIZE']
+
+
+if os.getenv('Kolibri_DOWNLOAD_URL') is not None:
+    os.environ['Kolibri_DOWNLOAD_URL']=_settings['data']['Kolibri_DOWNLOAD_URL']
 
-os.environ['Kolibri_DOWNLOAD_URL']=_settings['data']['Kolibri_DOWNLOAD_URL']
-DEFAULT_SEED=_settings['misc']['DEFAULT_SEED']
-TARGET_RANKING_LENGTH = _settings['misc']['TARGET_RANKING_LENGTH']
+DEFAULT_SEED=os.getenv('DEFAULT_SEED') or _settings['misc']['DEFAULT_SEED']
+TARGET_RANKING_LENGTH = os.getenv('TARGET_RANKING_LENGTH') or _settings['misc']['TARGET_RANKING_LENGTH']
```

## kolibri/errors.py

```diff
@@ -14,14 +14,24 @@
     def __init__(self, document, message):
         self.document = document
         logger.error(message)
 
     def __str__(self):
         return self.document
 
+class ConfigError(Exception):
+    """Any configuration error."""
+
+    def __init__(self, message):
+        super(ConfigError, self).__init__()
+        self.message = message
+
+    def __str__(self):
+        return repr(self.message)
+
 
 class UnsupportedLanguageError(Exception):
     """Raised when a component is created but the language is not supported.
 
     Attributes:
         component -- component name
         language -- language that component doesn't support
@@ -110,8 +120,109 @@
     def __init__(self, message):
         Exception.__init__(self, message)
         logger.error(message)
 
 class MetricException(Exception):
     def __init__(self, message):
         Exception.__init__(self, message)
-        logger.error(message)
+
+        logger.error(message)
+
+
+class InvalidDataError(Exception):
+    """Error to raise when data is not valid."""
+
+    def __init__(self, errors):
+        self.errors = errors
+
+    def __str__(self):
+        return (
+            'The provided data does not match the metadata:\n' +
+            '\n\n'.join(map(str, self.errors))
+        )
+
+
+class NotFittedError(Exception):
+    """Error to raise when sample is called and the model is not fitted."""
+
+
+class ConstraintsNotMetError(ValueError):
+    """Exception raised when the given data is not valid for the constraints."""
+
+    def __init__(self, message=''):
+        self.message = message
+        super().__init__(self.message)
+
+
+class SynthesizerInputError(Exception):
+    """Error to raise when a bad input is provided to a ``Synthesizer``."""
+
+
+class SamplingError(Exception):
+    """Error to raise when sampling gets a bad input or can't be used."""
+
+
+class NonParametricError(Exception):
+    """Exception to indicate that a model is not parametric."""
+
+"""Data processing exceptions."""
+
+
+class NotFittedError(Exception):
+    """Error to raise when ``DataProcessor`` is used before fitting."""
+
+
+class InvalidConstraintsError(Exception):
+    """Error to raise when constraints are not valid."""
+
+    def __init__(self, errors):
+        errors = errors if isinstance(errors, list) else [errors]
+        self.errors = errors
+
+    def __str__(self):
+        return (
+            'The provided constraint is invalid:\n' +
+            '\n\n'.join(map(str, self.errors))
+        )
+
+
+"""Constraint Exceptions."""
+
+
+class MissingConstraintColumnError(Exception):
+    """Error used when constraint is provided a table with missing columns."""
+
+    def __init__(self, missing_columns):
+        self.missing_columns = missing_columns
+
+
+class AggregateConstraintsError(Exception):
+    """Error used to represent a list of constraint errors."""
+
+    def __init__(self, errors):
+        self.errors = errors
+
+    def __str__(self):
+        return '\n' + '\n\n'.join(map(str, self.errors))
+
+
+class InvalidFunctionError(Exception):
+    """Error used when an invalid function is utilized."""
+
+
+class FunctionError(Exception):
+    """Error used when an a function produces an unexpected error."""
+
+
+class ConstraintMetadataError(Exception):
+    """Error to raise when Metadata is not valid."""
+
+
+"""Metadata Exceptions."""
+
+
+class InvalidMetadataError(Exception):
+    """Error to raise when Metadata is not valid."""
+
+
+class MetadataNotFittedError(InvalidMetadataError):
+    """Error to raise when Metadata is used before fitting."""
```

## kolibri/model_loader.py

```diff
@@ -1,25 +1,20 @@
-from typing import Optional
-
-import pandas as pd
 import numpy as np
+import pandas as pd
+from kdmt.lib import check_dependencies
+
+from kolibri import __version__ as ver
 from kolibri.config import TaskType
+from kolibri.features import *
 from kolibri.core.component import ComponentBuilder
-from kolibri import __version__ as ver
 from kolibri.core.modules import validate_requirements
-from kolibri.metadata import Metadata
 from kolibri.core.pipeline import Pipeline
+from kolibri.metadata import Metadata
 from .errors import *
-from pathlib import Path
-from kolibri.tokenizers import *
-from kolibri.features import *
-from kolibri.task import *
-from kolibri.autolearn.model_zoo.zoo_regressor import ZooRegressor
-from  kolibri.task.tabular.regression.sklearn_regression_estimator import RegSklearnEstimator
-from kdmt.lib import check_dependencies
+
 logger = get_logger(__name__)
 
 MINIMUM_COMPATIBLE_VERSION = "0.0.1"
 
 
 class ModelLoader(object):
     """Use a trained pipeline of components to parse text documents."""
@@ -44,33 +39,68 @@
                 "loaded by this nlp instance. "
                 "Either retrain the model_type, or run with"
                 "an older version. "
                 "Model version: {} Instance version: {}"
                 "".format(model_version, ver.__version__))
 
     @staticmethod
+    def load_component(component_meta, model_dir, component_builder=None):
+        component = component_builder.load_component(
+            component_meta, model_dir)
+        return component
+
+    @staticmethod
+    def load_pipeline(pipeline_meta, model_dir, component_builder=None):
+        pipeline = []
+        for component_meta in pipeline_meta:
+            if "pipeline" in component_meta:
+                pipeline.append(ModelLoader.load_pipeline(component_meta["pipeline"], model_dir, component_builder))
+            else:
+                pipeline.append(
+                    (component_meta['name'], ModelLoader.load_component(component_meta, model_dir, component_builder)))
+
+        return pipeline
+
+    @staticmethod
     def load(model_dir, component_builder=None, skip_validation=False):
+        """Create a pipeline based on a persisted model.
+
+        Args:
+            model_dir (str): The path of the model to load
+            component_builder (ComponentBuilder): The
+                :class:`ComponentBuilder` to use.
+
+        Returns:
+            ModelLoader: A pipeline that uses the loaded model.
+        """
+        model_metadata = Metadata.load(model_dir)
+        ModelLoader.ensure_model_compatibility(model_metadata)
+
+        if component_builder is None:
+            # If no builder is passed, every interpreter creation will result
+            # in a new builder. hence, no components are reused.
+            component_builder = ComponentBuilder()
+
+        steps = ModelLoader.load_pipeline(model_metadata.metadata["pipeline"], model_dir, component_builder)
+
+        return ModelLoader(Pipeline(steps), {}, model_metadata)
+
+    @staticmethod
+    def load2(model_dir, component_builder=None, skip_validation=False):
         """Create an interpreter based on a persisted model_type.
 
         Args:
             model_dir (str): The path of the model_type to load
             component_builder (ComponentBuilder): The
                 :class:`ComponentBuilder` to use.
 
         Returns:
             ModelLoader: An interpreter that uses the loaded model_type.
         """
 
-        from shutil import unpack_archive
-        # model_dir_to_load = model_dir if model_dir[:-4] == '.tgz' else model_dir + ".tgz"
-        # if os.path.exists(model_dir_to_load):
-        #     import tarfile
-        #     tar = tarfile.open(model_dir_to_load)
-        #     tar.extractall(path=Path(model_dir).parent)
-        #     tar.close()
 
         model_metadata = Metadata.load(model_dir)
 
         ModelLoader.ensure_model_compatibility(model_metadata)
         return ModelLoader.create(model_metadata,
                                   component_builder,
                                   skip_validation)
@@ -126,14 +156,15 @@
             # should pass an empty string in the first place.
             output = self.default_output_attributes()
             output["text"] = ""
             return output
 
         output = self.pipeline.predict(data)
 
+
         if isinstance(data, pd.DataFrame):
             data_out = data.copy()
             if self.pipeline.estimator.task_type == TaskType.ANOMALY_DETECTION:
                 data_out["Anomaly"] = [list(c.keys())[0] for c in output]
                 data_out["score"] = [list(c.values())[0] for c in output]
             elif hasattr(output, "dtype") and np.issubdtype(output.dtype, np.number):
                 data_out["Prediction"] = output
@@ -260,15 +291,15 @@
 
 
             Returns:
                 None
             """
 
             requirements = """
-        pycaret
+        kolibri-ml
         fastapi
         uvicorn
         """
             print("Writing requirements.txt")
             f = open("requirements.txt", "w")
             f.write(requirements)
             f.close()
```

## kolibri/model_trainer.py

```diff
@@ -27,15 +27,15 @@
 except Exception as e:
     print(str(e))
     logger.warning(str(e))
     pass
 
 import os
 import pandas as pd
-import psutil, shutil
+from kolibri.task import *
 import uuid
 import time
 from kolibri.config import ModelConfig, is_unsupervised
 from kolibri.utils.common import get_target_type
 from kolibri.utils.config import get_parameter_from_config
 from kolibri.config import TaskType
 
@@ -59,27 +59,28 @@
         'register-model': False,
         'max-time-for-optimization': 3600,
         'random-state': 42,
         'track-experiments':False,
         'archive-exiting-versions': True,
         'model-stage': "Staging", #"Archived", "Prouction"
         'experiment-name': 'experiment_1',
-        'model-name': None,
+        'model-name': "current",
         'experiment-uri': None,
         'ml-task': None,
         'explain-level': 2,
         'opt-metric-name': None,
         'optimize-pipeline': False,
         'optimizer': 'optuna',
         'output-folder': '.',
         'n-jobs': -1,
+        'optimization-n-jobs': -1,
         'log-data':True,
         'log-data-profile':True,
         'log-model':True,
-        'model-path': "current",
+        'artefacts-path': "kolibri-model",
         'combine-rare-classes': False,
         'rare-classes-name': 'Other',
         'rare-classes-threshold': 10,
         'log-experiment':False,
         'log-experiment-location': None,
         'log-cross-validated-data':True,
         "experiment_custom_tags":None,
@@ -99,15 +100,15 @@
         except Exception as e:
             print(str(e))
             pass
         self.experiment_name=self.config["experiment-name"]
         self.logger=logger
         if self.config['evaluate-performance']==False:
             self.config['save-evaluation-output']=False
-
+            self.config['track-experiments']=False
         if self.config['save-evaluation-output']==True:
             try:
                 import openpyxl
             except:
                 raise Exception("The library 'openpyxl' in not installed. To save evaluation result, You must install 'openpyxl' or chaange 'save-evaluation-output' to False")
         logger.debug("ModelTrainer.__init__")
         self.uid = str(uuid.uuid4())
@@ -143,27 +144,38 @@
         # build pipeline
 
         self.pipeline = self._build_pipeline(params)
 
         self.all_params=self.pipeline.parameters
 
         self.original_data=pd.DataFrame()
+
     @staticmethod
-    def _build_pipeline(params):
-        """Transform the passed names of the pipeline components into classes"""
+    def _build_pipeline(config):
+        pipeline = config['pipeline']
+        steps= ModelTrainer._process_steps(pipeline, config)
+        return Pipeline(steps)
 
-        steps = []
-        # Transform the passed names of the pipeline components into classes
-        for component_name in params['pipeline']:
-            component = modules.create_component_by_name(
-                component_name, params)
-            steps.append((component_name, component))
+    @staticmethod
+    def _process_steps(steps, params):
+        builded_steps = []
 
-        return Pipeline(steps)
+        for step in steps:
+            if isinstance(step, tuple):
+                # Import the module and get the class
+                module_name, class_name = step
+                instance = modules.create_component_by_name(class_name, params)
+
+                builded_steps.append((module_name, instance))
+            elif isinstance(step, list):
+                # Process nested pipeline
+                nested_pipeline = ModelTrainer._process_steps(step, params)
+                builded_steps.append(nested_pipeline)
 
+        return builded_steps
 
     def fit_transformers(self, X, y, X_val=None, y_val=None):
         return self.pipeline.fit_transformers(X, y, X_val, y_val)
 
     def fit_estimator(self, X, y, X_val=None, y_val=None):
         self.pipeline.fit_estimator(X, y, X_val, y_val)
 
@@ -185,53 +197,50 @@
 
         start_time = time.time()
         if self.config.get('optimize-pipeline'):
             logger.debug(f"ModelTrainer.fit - optimizing pipeline")
             self.pipeline.estimator.hyperparameters['fixed']["evaluate-performance"] = True
             self.optimize(X, y)
             self.pipeline=Pipeline.from_configs(self.hyperparameters)
-            self.pipeline.estimator.hyperparameters['fixed']["evaluate-performance"]=False
 
         try:
             model_results, runtime, model_fit_time, predictions=self.pipeline.fit(X, y, X_val, y_val)
         except Exception as e:
             print(e)
             model_results, runtime, model_fit_time, predictions=self.pipeline.fit(X, y)
 
         os.makedirs(os.path.join(self.config["output-folder"], "plots"), exist_ok=True)
 
         if not isinstance(self.pipeline.estimator,ZooRegressor) and not isinstance(self.pipeline.estimator,ZooClassifier) :
             if self.config['evaluate-performance'] and not self.config['optimize-pipeline']:
                 self.plot_model()
             if self.config['track-experiments']:
-
                 performance_data=None
-    #            self.y_true = y
-    #            self.y_pred=list(predictions[:,0])
                 if predictions is not None and len(predictions.shape)>1 and predictions.shape[1]>2:
                     performance_data=pd.DataFrame(X)
                     performance_data['class']=y
                     performance_data['prediction']=predictions[:,0]
                     probabilities=predictions[:,1:,]
                     new_columns=probabilities.shape[1]
                     columns=performance_data.columns.values.tolist()
                     for i in range(0,new_columns):
                         columns.append(f"probability_{i}")
                     performance_data=pd.concat([performance_data, pd.DataFrame(probabilities)], axis=1)
 
                     performance_data.columns=columns
-                elif predictions.size >0 and (len(predictions.shape)==1 or predictions.shape[1]==1):
+                elif predictions is not None and predictions.size >0 and (len(predictions.shape)==1 or predictions.shape[1]==1):
                     performance_data=pd.DataFrame(X)
                     performance_data['class']=y
                     performance_data['prediction']=predictions.reshape(-1, 1)[:,0]
                 if model_results is not None:
                     avgs_dict_log = {k: v for k, v in model_results.loc["Mean"].items()}
                     log_plots=self.config["log-plots"]
                     data_frames=[performance_data]
                     if self.experiment_logger is not None:
+                        print("Logging experiment...")
                         self.experiment_logger.log_model(
                             experiment=self,
                             model=self.pipeline,
                             model_results=model_results,
                             pipeline=None,
                             score_dict=avgs_dict_log,
                             source="KolibriEstimator.fit",
@@ -243,15 +252,15 @@
                             tune_cv_results=None,
                             URI=None
                         )
             if self.config["register-model"]:
                 model_name=self.config["model-name"]
                 if model_name is None:
                     model_name=self.pipeline.estimator.name
-                self.experiment_logger.register_model(model_name,artifact=self.config['model-path'], registered_model_version_stage=self.config["model-stage"], archive_existing_versions=self.config["archive-exiting-versions"])
+                self.experiment_logger.register_model(model_name,artifact=self.config['artefacts-path'], registered_model_version_stage=self.config["model-stage"], archive_existing_versions=self.config["archive-exiting-versions"])
         self.train_time=time.time()-start_time,
 
         gc.collect()
         return self.pipeline
 
     def objective(self, X, y):
 
@@ -274,15 +283,15 @@
         try:
             optimizer = OptunaTuner(
                     self.config['output-folder'],
                     eval_metric=self._get_optimize_metric(),
                     time_budget=self.config["max-time-for-optimization"],
                     init_params={},
                     verbose=True,
-                    n_jobs=-1,
+                    n_jobs=self.config["optimization-n-jobs"],
                     random_state=self.config['random-state']
                 )
 
             start_time = time.time()
             self.hyperparameters = optimizer.optimize(
                 objective=self.objective(X, y),
                 learner_params=self.pipeline.parameters
@@ -362,15 +371,15 @@
                         ["PCA Components", get_parameter_from_config(self.all_params, "pca-components", 0)],
                         ["Ignore Low Variance", 'NearZeroVariance' in list(self.all_params.keys())],
                         ["Combine Rare Levels", 'Catagorical_variables_With_Rare_levels'  in list(self.all_params.keys())],
                         ["Rare Level Threshold", get_parameter_from_config(self.all_params, "rare-level-threshold", None)],
                         ["Numeric Binning", 'Binning' in list(self.all_params.keys())],
                         ["Remove Outliers", 'Outlier' in list(self.all_params.keys())],
     #                    ["Outliers Threshold", outliers_threshold_grid],
-                        ["Remove Multicollinearity", 'Fix_multicollinearity' in list(self.all_params.keys())],
+                        ["Remove Multicollinearity", 'Multicollinearity' in list(self.all_params.keys())],
                         ["Multicollinearity Threshold",  get_parameter_from_config(self.all_params, "colinearity-threshold", None)],
                         ["Remove Perfect Collinearity", get_parameter_from_config(self.all_params, "correlation-with-target-threshold", 0)==1],
                         ["Clustering", 'ClusterDataset' in list(self.all_params.keys())],
                         ["Group Features", "Reduce_Cardinality_with_Clustering"  in list(self.all_params.keys())],
                         ["Feature Selection", "Advanced_Feature_Selection_Classic"  in list(self.all_params.keys())],
                         ["Top Features Selected", get_parameter_from_config(self.all_params,"top-features-to-pick", None)],
                     ]
@@ -492,26 +501,80 @@
                     plt.save(os.path.join(save_dir, plot+".svg"))
                 else:
                     print("not saved")
 
             if plt is not None and hasattr(plt, "close"):
                 plt.close()
 
+    def persist_pipeline(self, pipeline, dir_name, metadata):
+        for component in pipeline:
+            if isinstance(component, tuple):
+                update = component[1].persist(dir_name)
+                component_meta = component[1].hyperparameters
+                if update:
+                    component_meta.update(update)
+                component_meta["label"] = module_path_from_object(component[1])
+                component_meta["name"] = component[0]
+
+                metadata["pipeline"].append(component_meta)
+            elif isinstance(component, list):
+                sub_pipeline_metadata = {"pipeline": []}
+                self.persist_pipeline(component, dir_name, sub_pipeline_metadata)
+                metadata["pipeline"].append(sub_pipeline_metadata)
+
+        return metadata
+
     def persist(self, path, fixed_model_name=None):
         """Persist all components of the pipeline to the passed path.
+        Returns the directory of the persisted model."""
+
+        timestamp = datetime.datetime.now().strftime('%Y%m%d-%H%M%S')
+        metadata = {
+            "pipeline": [],
+        }
+
+        if fixed_model_name is not None:
+            model_name = fixed_model_name
+        else:
+            model_name = "model_" + timestamp
+
+        path = Path(path).resolve()
+        dir_name = os.path.join(path, model_name)
+
+        create_dir(dir_name)
+
+        metadata = self.persist_pipeline(self.pipeline.steps, dir_name, metadata)
+
+        if hasattr(self, "x_schema"):
+            metadata["X_schema"] = self.x_schema
+
+        Metadata(metadata, dir_name).persist(dir_name)
+
+        if self.performance_data is not None:
+            try:
+                self.performance_data.to_excel(os.path.join(path, 'validatation_data_.xlsx'), engine='xlsxwriter')
+            except:
+                pass
+
+        logger.info("Successfully saved model into "
+                    "'{}'".format(os.path.abspath(dir_name)))
+        return dir_name
+
+    def persist2(self, path, fixed_model_name=None):
+        """Persist all components of the pipeline to the passed path.
 
         Returns the directory of the persisted model."""
 
 
         timestamp = datetime.datetime.now().strftime('%Y%m%d-%H%M%S')
         metadata = {
             "pipeline": [],
         }
 
-        if fixed_model_name:
+        if fixed_model_name is not None:
             model_name = fixed_model_name
         else:
             model_name = "model_" + timestamp
 
         path = Path(path).resolve()
         dir_name = os.path.join(path, model_name)
 
@@ -537,20 +600,14 @@
 
         if self.performance_data is not None:
             try:
                 self.performance_data.to_excel(os.path.join(path, 'validatation_data_.xlsx'), engine='xlsxwriter')
             except:
                 pass
 
-        # import tarfile
-        # tar = tarfile.open(dir_name+".tgz", "w:gz")
-        # tar.add(dir_name, arcname=fixed_model_name)
-        # tar.close()
-        # if os.path.exists(dir_name) and os.path.isdir(dir_name):
-        #     shutil.rmtree(dir_name)
         logger.info("Successfully saved model into "
                     "'{}'".format(os.path.abspath(dir_name)))
         return dir_name
 
     def explain(self, **kwargs):
```

## kolibri/registry.py

```diff
@@ -1,40 +1,79 @@
-from kolibri.config import TaskType
-
-class ModulesRegistry:
-
-    registry = {
-        'Estimators':{
-        },
-        'kolibri':{}
-    }
-
-    for task_type in TaskType:
-        registry['Estimators'][task_type.name]={}
-
-
-    @staticmethod
-    def add_algorithm(
-        task_name,
-        model_class,
-        model_params,
-        required_preprocessing,
-        additional,
-        default_params,
-    ):
-        model_information = {
-            "class": model_class,
-            "params": model_params,
-            "required_preprocessing": required_preprocessing,
-            "additional": additional,
-            "default_params": default_params,
-        }
-        ModulesRegistry.registry['Estimator'][task_name][
-            model_class.algorithm_short_name
-        ] = model_information
-
-    @staticmethod
-    def add_module(
-        module_name,
-        module_class,
-    ):
-        ModulesRegistry.registry['kolibri'][module_name] = {'class':module_class}
+# Copyright 2017 Neural Networks and Deep Learning lab, MIPT
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import importlib
+import json
+from logging import getLogger
+from pathlib import Path
+
+from kolibri.errors import ConfigError
+
+logger = getLogger(__name__)
+
+_registry_path = Path(__file__).parent / 'registry.json'
+if _registry_path.exists():
+    with _registry_path.open(encoding='utf-8') as f:
+        _REGISTRY = json.load(f)
+else:
+    _REGISTRY = {}
+
+inverted_registry = {val: key for key, val in _REGISTRY.items()}
+
+
+def cls_from_str(name: str) -> type:
+    """Returns a class object with the name given as a string."""
+    try:
+        module_name, cls_name = name.split(':')
+    except ValueError:
+        raise ConfigError('Expected class description in a `module.submodules:ClassName` form, but got `{}`'
+                          .format(name))
+
+    return getattr(importlib.import_module(module_name), cls_name)
+
+
+def register(name: str = None) -> type:
+    """
+    Register classes that could be initialized from JSON configuration file.
+    If name is not passed, the class name is converted to snake-case.
+    """
+
+    def decorate(model_cls: type, reg_name: str = None) -> type:
+        model_name = reg_name or short_name(model_cls)
+        global _REGISTRY
+        cls_name = model_cls.__module__ + ':' + model_cls.__name__
+        if model_name in _REGISTRY and _REGISTRY[model_name] != cls_name:
+            logger.warning('Registry name "{}" has been already registered and will be overwritten.'.format(model_name))
+        _REGISTRY[model_name] = cls_name
+        return model_cls
+
+    return lambda model_cls_name: decorate(model_cls_name, name)
+
+
+def short_name(cls: type) -> str:
+    """Returns just a class name (without package and module specification)."""
+    return cls.__name__.split('.')[-1]
+
+
+def get_model(name: str) -> type:
+    """Returns a registered class object with the name given in the string."""
+    if name not in _REGISTRY:
+        if ':' not in name:
+            raise ConfigError("Model {} is not registered.".format(name))
+        return cls_from_str(name)
+    return cls_from_str(_REGISTRY[name])
+
+
+def list_models() -> list:
+    """Returns a list of names of registered classes."""
+    return list(_REGISTRY)
```

## kolibri/settings.yaml

```diff
@@ -3,15 +3,15 @@
  KOLIBRI_DATA_FOLDER:  !ENV ${KOLIBRI_DATA_PATH}
  RESOURCES_AUTO_DOWNLOAD: True
  Kolibri_DOWNLOAD_URL: "https://raw.githubusercontent.com/mbenhaddou/kolibri-data/main/index.json"
  AZURE_STORAGE_CONNECTION_STRING: !ENV ${AZURE_STORAGE_CONNECTION_STRING}
 logs:
  LOG_NAME: 'kolibri'
  LOG_LEVEL: DEBUG
- LOG_TO_FILE: False
+ LOG_TO_FILE: True
 
 neural_networks:
  DEFAULT_NN_MODEL_FILENAME: "_model_.h5"
  EMBEDDING_SIZE: 100
 
 misc:
  DEFAULT_SEED: 4231
```

## kolibri/autolearn/model_zoo/zoo_regressor.py

```diff
@@ -1,12 +1,11 @@
 import copy
 import joblib
 from tqdm import tqdm
 from kdmt.jupyter import isnotebook
-from kolibri.backend.base.base_classifier import BaseClassifier
 from kolibri.backend.base.base_regressor import BaseRegressor
 from kdmt.dict import update
 from kolibri.optimizers.optuna.objective import EstimatorObjective
 from copy import deepcopy
 from kolibri.logger import get_logger
 from kolibri.config import TaskType
 from kdmt.objects import class_from_module_path
```

## kolibri/backend/__init__.py

```diff
@@ -0,0 +1,4 @@
+00000000: 6672 6f6d 206b 6f6c 6962 7269 2e62 6163  from kolibri.bac
+00000010: 6b65 6e64 2e73 6b6c 6561 726e 2069 6d70  kend.sklearn imp
+00000020: 6f72 7420 4c61 7a79 5265 6772 6573 7369  ort LazyRegressi
+00000030: 6f6e                                     on
```

## kolibri/backend/models.py

```diff
@@ -1,15 +1,12 @@
+import pandas as pd
 
-
-from kdmt.file import read_json_file
-from pathlib import Path
-from kolibri.task.text.topics import get_available_models as get_topics_available_models
-import kolibri.task.text.topics.topics_estimator
+# from kolibri.task.text.topics import get_available_models as get_topics_available_models
+# import kolibri.task.text.topics.topics_estimator
 from kolibri.config import TaskType
-import pandas as pd
 from kolibri.data import load
 
 try:
 
     sklearn_classification_models=load('packages/models/sklearn/classifiers.json')
     sklearn_classification_models_names=list(sklearn_classification_models.keys())
```

## kolibri/backend/base/base_estimator.py

```diff
@@ -1,34 +1,31 @@
 import gc
 import os
 import uuid
 from typing import Tuple
+
 import numpy as np
-from kdmt.ml.common import sklearn_numpy_warning_fix
-from kolibri.utils.cross_validation import cross_val_predict_score
 from kdmt.jupyter import isnotebook
-from kolibri.core.component import Component
+from kdmt.ml.common import sklearn_numpy_warning_fix
 
+from kolibri.core.component import Component
+from kolibri.utils.cross_validation import cross_val_predict_score
 
 try:
     from kolibri.explainers.shap_explainer import PlotSHAP
 except:
     pass
 from kdmt.cloud import google
 from kdmt.cloud import azure
-
-from kolibri.config import TaskType
-from kolibri.config import ParamType
+from sklearn.model_selection import cross_validate
 from kdmt.dict import update
-from sklearn.utils.multiclass import type_of_target
 from sklearn.calibration import CalibratedClassifierCV
 from copy import deepcopy
 from kdmt.objects import class_from_module_path
 from kolibri.logger import get_logger
-from kolibri import default_configs as settings
 import pandas as pd
 import time
 import datetime
 
 
 logger = get_logger(__name__)
 from kolibri.output import DefaultDisplay
@@ -94,14 +91,15 @@
             'imputer': 'none',
             'fold-shuffle': True,
             'cross-validate': True,
             'groups': None,
             "n-folds": 5,
             "round": 4,
             "display": "default",
+            "return-predictions": True
         },
 
         "tunable": {
             'model':{
                 "value":{
 
                 }
@@ -187,14 +185,19 @@
         if "fixed" in self.hyperparameters:
             for c in self.hyperparameters["fixed"]:
 
                 if c in self.hyperparameters["tunable"]["model"]["value"]["parameters"]:
                     self.hyperparameters["tunable"]["model"]["value"]["parameters"][c]["value"] = self.hyperparameters["fixed"][
                         c]
 
+        model_params={k[6:]:p for k, p in self.params.items() if 'model.' in k[:6]}
+        for k, p in model_params.items():
+            if k in self.hyperparameters["tunable"]["model"]["value"]["parameters"]:
+                self.hyperparameters["tunable"]["model"]["value"]["parameters"][k]["value"] = p
+
     def fit(self, data_X=None, data_y=None, X_val=None, y_val=None):
 
         """
         Internal version of ``create_model`` with private arguments.
         """
         raise NotImplementedError
 
@@ -294,15 +297,14 @@
                 row_idx=1,
                 message=f"Fitting {cv} Folds"
             )
             """
             MONITOR UPDATE ENDS
             """
 
-            from sklearn.model_selection import cross_validate
             metrics = self._get_metrics()
             metrics_dict = dict([(k, v.scorer) for k, v in metrics.items()])
 
             logger.info("Starting cross validation")
 
             n_jobs = self.get_parameter("n_jobs")
             from sklearn.gaussian_process import (
@@ -311,26 +313,35 @@
             )
 
             # special case to prevent running out of memory
             if isinstance(self.model, (GaussianProcessClassifier, GaussianProcessRegressor)):
                 n_jobs = 1
 
             logger.info(f"Cross validating with {cv}, n_jobs={n_jobs}")
-
-            predictions, scores = cross_val_predict_score(
+            predictions=None
+            if self.get_parameter("return-predictions"):
+                predictions, scores = cross_val_predict_score(
+                    self.model,
+                    data_X,
+                    data_y,
+                    method='predict_proba',
+                    cv=cv,
+                    scoring=metrics_dict,
+                    n_jobs=n_jobs,
+                    error_score=0,
+                )
+            else:
+                scores=cross_validate(
                 self.model,
-                data_X,
-                data_y,
-                method='predict_proba',
-                cv=cv,
-                scoring=metrics_dict,
-                n_jobs=n_jobs,
-                error_score=0,
-            )
-
+                    data_X,
+                    data_y,
+                    cv=cv,
+                    scoring=metrics_dict,
+                    n_jobs=n_jobs,
+                    error_score=0)
             score_dict = {}
             for k, v in metrics.items():
                 score_dict[v.display_name] = []
                 test_score = scores[f"test_{k}"] * (1 if v.greater_is_better else -1)
                 test_score = test_score.tolist()
                 score_dict[v.display_name] += test_score
 
@@ -560,15 +571,15 @@
             _download_blob_azure(container_name, filename, filename)
 
             model = cls.load_model(filename, verbose=False)
 
             logger.info("Transformation Pipeline and Model Successfully Loaded")
             return model
         else:
-            print(f"Platform {platform} is not supported by pycaret or illegal option")
+            print(f"Platform {platform} is not supported by Kolibri or illegal option")
         gc.collect()
 
     def persist(self, model_dir):
         """Persist this model_type into the passed directory."""
 
         classifier_file = os.path.join(model_dir, KOLIBRI_MODEL_FILE_NAME)
         joblib.dump(self, classifier_file)
@@ -666,15 +677,14 @@
         if isnotebook():
             display = DefaultDisplay(verbose=verbose, html_param=True)
 
         plot_kwargs = {}
 
         logger.info("Preloading libraries")
         # pre-load libraries
-        import matplotlib.pyplot as plt
 
         np.random.seed(self.get_parameter("seed"))
 
         estimator = deepcopy(self.model)
         model = estimator
 
         # plots used for logging (controlled through plots_log_param)
@@ -712,18 +722,18 @@
         logger.info("Initializing deploy_model()")
         logger.info(f"deploy_model({function_params_str})")
 
         allowed_platforms = ["aws", "gcp", "azure"]
 
         if platform not in allowed_platforms:
             logger.error(
-                f"(Value Error): Platform {platform} is not supported by pycaret or illegal option"
+                f"(Value Error): Platform {platform} is not supported by Kolibri or illegal option"
             )
             raise ValueError(
-                f"Platform {platform} is not supported by pycaret or illegal option"
+                f"Platform {platform} is not supported by Kolibri or illegal option"
             )
 
         if platform:
             if not authentication:
                 raise ValueError("Authentication is missing.")
 
         # general dependencies
```

## kolibri/backend/base/base_regressor.py

```diff
@@ -205,27 +205,30 @@
         logger.info(
             "create_model() successfully completed......................................"
         )
         gc.collect()
 #        self.display.close()
 #        self.display=None
 
-        self.y_true=data_y
-        self.X=data_X
-        if predictions!=[] and len(predictions.shape)==1:
-            self.y_pred=predictions
-        else:
-            self.y_pred= [] if predictions==[] else predictions[:,1:,].astype(np.float16)
-
-        self.plotter =  RegressionPlots(y_true=self.y_true, y_pred=self.y_pred, model_name=str(self.model), X=self.X,
-                                    y=self.y_true, estimator=self.model,
-                                    features_names=self.feature_names)
+        if predictions is not None:
+            self.y_true=data_y
+            self.X=data_X
+            if predictions!=[]  and len(predictions.shape)==1:
+                self.y_pred=predictions
+            else:
+                self.y_pred= [] if predictions==[]  else predictions[:,1:,].astype(np.float16)
+
+            self.plotter =  RegressionPlots(y_true=self.y_true, y_pred=self.y_pred, model_name=str(self.model), X=self.X,
+                                        y=self.y_true, estimator=self.model,
+                                        features_names=self.feature_names)
 
-
-        self.performace_scores=performace_scores.loc[['Mean', 'Std']].to_dict()
+        if performace_scores is not None:
+            self.performace_scores=performace_scores.loc[['Mean', 'Std']].to_dict()
+        else:
+            self.performace_scores="Performance not evaluated"
         return performace_scores, runtime, model_fit_time, predictions
 
     def predict(self, X_test):
 
         preds=self.model.predict(X_test)
 
         return preds
```

## kolibri/backend/sklearn/__init__.py

```diff
@@ -0,0 +1,10 @@
+00000000: 6672 6f6d 206b 6f6c 6962 7269 2e62 6163  from kolibri.bac
+00000010: 6b65 6e64 2e73 6b6c 6561 726e 2e65 7874  kend.sklearn.ext
+00000020: 656e 7369 6f6e 732e 6c61 7a79 5f6c 6561  ensions.lazy_lea
+00000030: 726e 6572 2069 6d70 6f72 7420 4c61 7a79  rner import Lazy
+00000040: 5265 6772 6573 7369 6f6e 0a66 726f 6d20  Regression.from 
+00000050: 6b6f 6c69 6272 692e 6261 636b 656e 642e  kolibri.backend.
+00000060: 736b 6c65 6172 6e2e 6578 7465 6e73 696f  sklearn.extensio
+00000070: 6e73 2e6c 6f6f 6b75 705f 6c65 6172 6e65  ns.lookup_learne
+00000080: 7220 696d 706f 7274 204c 617a 794c 6f6f  r import LazyLoo
+00000090: 6b75 7052 6567 7265 7373 696f 6e         kupRegression
```

## kolibri/backend/sklearn/meta/ecoc_model.py

```diff
@@ -45,16 +45,16 @@
     ECOC meta classifier
     ref: http://www.cs.cmu.edu/~aberger/pdf/ecoc.pdf
 
     Parameters:
         base_estimator: string
             classfier name. This classfier name comes from kolibri model_type database. These are mainly sklearn models
         code_size:  specifies the code size. ie the number of base classifiers that will be created.
-        decoder: str
-            indicates the type of decoder, get a decoder object immediately when initialization.
+        decoders: str
+            indicates the type of decoders, get a decoders object immediately when initialization.
             For more details, check Decoding.Decoder.get_decoder.
 
     Attributes:
         estimator_type: str, {'decision_function','predict_proba'}
             which type the estimator belongs to.
             'decision_function' - predict value range (-∞,+∞)
             'predict_proba' - predict value range [0,1]
```

## kolibri/backend/sklearn/meta/ecoc/decoder.py

```diff
@@ -8,18 +8,18 @@
 Code by Tycho Zhong, Dec 6, 2017.
 """
 
 import numpy as np
 
 
 def get_decoder(dec):
-    """ Get a decoder object.
+    """ Get a decoders object.
     Parameters:
         dec: str
-            Indicates a kind of decoder. Cognitive dec list below.
+            Indicates a kind of decoders. Cognitive dec list below.
             'HD' - Hamming Decoder.
             'IHD' - Inverse Hamming Decoder.
             'LD' - Laplacian Decoder.
             'ED' - Euclidean Decoder.
             'AED' - Attenuated Euclidean Decoder.
             'RED' - Ratio Euclidean Decoder.
             'EuD' - Euler Decoder.
@@ -27,15 +27,15 @@
             'ELB' - Exponential Loss Based Decoder.
             'LLW' - Linear Loss Weighted Decoder.
             'ELW' - Exponential Loss Weighted Decoder.
             'PD' - Probabilistic Decoder (Coming soon).
 
     Returns:
         o: object
-            A decoder object.
+            A decoders object.
     """
     if dec == 'HD':
         return HammingDecoder()
     elif dec == 'IHD':
         return InverseHammingDecoder()
     elif dec == 'LD':
         return LaplacianDecoder()
@@ -180,15 +180,15 @@
         if W.shape[1] != M.shape[1]:
             raise ValueError('Length of W must be the same with column number of Matrix.')
         return W
 
 
 class HammingDecoder(HardDecoder):
     """Hamming Decoder (HD)
-    Hamming decoder must check if Y contains only -1, 0 or 1.
+    Hamming decoders must check if Y contains only -1, 0 or 1.
     """
     @staticmethod
     def _distance(y, m):
         return sum(abs(y-m))
 
 
 
@@ -213,30 +213,30 @@
     @staticmethod
     def _distance(y, m):
         c, e, k = sum(y == m), sum(y != m) - sum(y == 0), 2
         return (c + e + k) / (c + 1)
 
 
 class EulerDecoder(OrdinaryDecoder):
-    """Scikit-learn default decoder."""
+    """Scikit-learn default decoders."""
     def decode(self, Y, M):
         Y, M = self._check_param(Y, M)
         return -1 * np.dot(Y, M.T) / np.einsum('ij,ij->i', M, M)
 
 
 class EuclideanDecoder(OrdinaryDecoder):
     """Euclidean Decoder (ED)."""
     @staticmethod
     def _distance(y, m):
         return np.sqrt(sum((y-m)**2))
 
 
 class AttenuatedEuclideanDecoder(OrdinaryDecoder):
     """Attenuated Euclidean Decoder (AED).
-    Note that this decoder is originally designed for tenary code matrix.
+    Note that this decoders is originally designed for tenary code matrix.
     """
     @staticmethod
     def _distance(y, m):
         return np.sqrt(sum(((y-m)**2)*abs(m)*abs(y)))       #按道理这里应该还有乘以一个abs(xj),其实好像并不需要
         #return np.sqrt(sum(((y-m)**2)*abs(m)))
 
 class RatioEuclideanDecoder(OrdinaryDecoder):
```

## kolibri/backend/tensorflow/__init__.py

```diff
@@ -1,25 +1,35 @@
 import importlib
 
 from packaging import version
-import tensorflow as tf
+#from . import data_modules
+from . import layers
+from . import losses
+#from . import models
+#from . import synthesizer_name
+#from . import utils
 #from kolibri.backend.tensorflow.tasks.audio import *
 #from kolibri.backend.tensorflow.tasks.text import *
 import sys
 from kolibri.logger import get_logger
 logger = get_logger(__name__)
 
 
 if sys.version_info < (3, 8):
     import importlib_metadata
 else:
     import importlib.metadata as importlib_metadata
 
-tf.compat.v1.logging.set_verbosity(tf.compat.v1.logging.ERROR)
-custom_objects = tf.keras.utils.get_custom_objects()
+try:
+    import tensorflow as tf
+    tf.compat.v1.logging.set_verbosity(tf.compat.v1.logging.ERROR)
+    custom_objects = tf.keras.utils.get_custom_objects()
+except:
+    pass
+
 
 
 def custom_object_scope():
     return tf.keras.utils.custom_object_scope(custom_objects)
 
 
 
@@ -66,8 +76,22 @@
     if version.parse(_tf_version) < version.parse("2"):
         logger.info(f"TensorFlow found but with version {_tf_version}. Transformers requires version 2 minimum.")
         is_tf_available = False
     else:
         logger.info(f"TensorFlow version {_tf_version} available.")
 else:
     logger.info("Disabling Tensorflow because USE_TORCH is set")
-    is_tf_available = False
+    is_tf_available = False
+
+
+
+
+
+__all__ = [
+    'custom_object_scope',
+#    'data_modules',
+    'layers',
+    'losses',
+#    'models',
+#    'synthesizer_name',
+    'utils'
+]
```

## kolibri/backend/tensorflow/autoencoder/__init__.py

```diff
@@ -1,5 +1,6 @@
-__all__ = ['Conv1DAutoencoder', 'VariationalAutoencoder', 'SequenceAutoencoder']
+__all__ = ['Conv1DAutoencoder', 'VariationalAutoencoder', 'SequenceAutoencoder', 'BaseAutoEncoder']
 
 from kolibri.backend.tensorflow.autoencoder.conv_autoencoder import Conv1DAutoencoder
 from kolibri.backend.tensorflow.autoencoder.deep_autoencoder import SequenceAutoencoder
 from kolibri.backend.tensorflow.autoencoder.variational_autoencoder import VariationalAutoencoder
+from kolibri.backend.tensorflow.autoencoder.base_autoencoder import BaseAutoEncoder
```

## kolibri/backend/tensorflow/autoencoder/base_autoencoder.py

```diff
@@ -4,15 +4,15 @@
 from typing import Any, Dict
 
 import numpy as np
 import tensorflow as tf
 import tqdm
 
 import kolibri
-from kdmt.azure import upload_file, get_file_object
+from kdmt.cloud.azure import upload_file, get_file_object
 from kolibri.backend.tensorflow.autoencoder.decoders.lstm_decoder import Decoder
 from kolibri.backend.tensorflow.autoencoder.encoders.lstm_encoder import Encoder
 from tensorflow import keras
 from kolibri.logger import get_logger
 
 logger = get_logger(__name__)
 
@@ -26,17 +26,17 @@
             '__class_name__': self.__class__.__name__,
             '__module__': self.__class__.__module__,
             'config': {
                 "configs":self.configs,
                 'input_shape': self.input_shape,
                 'output_shape': self.output_shape
             },
-
-            'encoder': self.encoder.to_dict(),  # type: ignore
-            'decoder': self.decoder.to_dict(),
+            '_features_names': self._features_names,
+            'encoders': self.encoder.to_dict(),  # type: ignore
+            'decoders': self.decoder.to_dict(),
 
         }
 
     def __init__(self, configs, input_shape, output_shape):
         super(BaseAutoEncoder, self).__init__()
         self.ae_model = None
         self.configs=configs
@@ -49,20 +49,20 @@
             self.model_chekpoint_path = os.path.join(td.name, 'Checkpoints', self.model_name)
         self.input_shape=input_shape
         self.output_shape=output_shape
         self.title = "AutoEncoder training History"
         self.encoder = Encoder(self.input_shape, dropout=configs["dropout"])
         self.decoder = Decoder(self.output_shape, self.encoder.encoder_states, dropout=configs["dropout"])
         self.loss=configs["ae-loss"]
-        # encoder decoder model
+        # encoders decoders model
         self.ae_model = tf.keras.Model([self.encoder.encoder_input, self.decoder.decoder_input], self.decoder.decoder_output)
         self.ae_model.compile(loss=self.loss, optimizer='adam')
         self.history=None
         self.title=""
-
+        self._features_names=self.configs["features"]
     def summary(self):
         if self.ae_model is not None:
             return self.ae_model.summary()
 
     def fit(self, encoder_train, decoder_train, label_train, encoder_val=None, decoder_val=None, label_val=None,
                 epochs=500, patience=10):
             if self.ae_model is None:
@@ -75,15 +75,17 @@
                                                                                                   label_val), verbose=1,
                 callbacks=[
                     tf.keras.callbacks.EarlyStopping(monitor='val_loss', min_delta=0, patience=patience, verbose=1,
                                                      mode='min'),
                     tf.keras.callbacks.ModelCheckpoint(self.model_chekpoint_path, monitor='val_loss', save_best_only=True,
                                                        mode='min',
                                                        verbose=0)])
-
+    @property
+    def features_names(self):
+        return self._features_names
 
     def save(self, model_path: str) -> str:
         """
         Save model
         Args:
             model_path:
         """
```

## kolibri/backend/tensorflow/autoencoder/conv_autoencoder.py

```diff
@@ -81,14 +81,14 @@
 
     def predict(self,
                x_data,
                batch_size=32,
                debug_info=False,
                predict_kwargs= None):
         """
-        Generates output predictions for the encoder.
+        Generates output predictions for the encoders.
         """
         if predict_kwargs is None:
             predict_kwargs = {}
         pred = self.autoencoder.predict(np.expand_dims(x_data,axis=2), batch_size=batch_size, **predict_kwargs)
 
         return pred
```

## kolibri/backend/tensorflow/autoencoder/deep_autoencoder.py

```diff
@@ -32,23 +32,23 @@
         #dim_out=self.hyper_parameters['latent']['units']
         dims_encoder = self.hyper_parameters['nb-layers']
         dims_decoding = dims_encoder
         input_img: object = Input(shape=(dim_in,), name='EncoderIn')
 
         encoded = input_img
 
-        # Construct encoder layers
+        # Construct encoders layers
         out_dim = self.input_dim
         for i in range(dims_encoder):
             name = 'Encoder{0}'.format(i)
             out_dim = int(out_dim / 2)
             encoded = Dense(out_dim, activation='relu', name=name, activity_regularizer=regularizers.l2(self.hyper_parameters['sparsity']))(encoded)
 
-        # Construct decoder layers
-        # The decoded is connected to the encoders, whereas the decoder is not
+        # Construct decoders layers
+        # The decoded is connected to the encoders, whereas the decoders is not
         decoded = encoded
         decoder_input = Input(shape=(out_dim,), name='DecoderIn')
 
         decoder = decoder_input
         for i in range(dims_decoding):
             name = 'Decoder{0}'.format(i)
 
@@ -56,21 +56,21 @@
             out_dim = out_dim * 2
             decoder = Dense(out_dim, activation=activation, name=name, activity_regularizer=regularizers.l2(self.hyper_parameters['sparsity']))(decoder)
 
         decoder = Dense(self.input_dim, activation=activation, name='output')(decoder)
 
         self.encoder = Model(inputs=input_img, outputs=encoded)
 
-        # instantiate decoder model
+        # instantiate decoders model
 
-        self.decoder = Model(decoder_input, decoder, name='decoder')
+        self.decoder = Model(decoder_input, decoder, name='decoders')
 
-        # autoencoder = encoder + decoder
+        # autoencoder = encoders + decoders
         # instantiate autoencoder model
         self.autoencoder = Model(input_img,
                                  self.decoder(self.encoder(input_img)),
                                  name='autoencoder')
 
-#		self.encoder = Model(input=input_img, output=encoded)
-#		self.decoder = Model(input=decoder_input, output=decoder)
+#		self.encoders = Model(input=input_img, output=encoded)
+#		self.decoders = Model(input=decoder_input, output=decoders)
 
 #		self.autoencoder.compile(optimizer='adadelta', loss='binary_crossentropy')
```

## kolibri/backend/tensorflow/autoencoder/variational_autoencoder.py

```diff
@@ -46,39 +46,39 @@
                 }
 
     def build_model_arc(self):
         # network parameters
         input_shape = (self.input_dim,)
         latent_dim = self.hyper_parameters['latent']['units']
 
-        # VAE model = encoder + decoder
-        # build encoder model
+        # VAE model = encoders + decoders
+        # build encoders model
         inputs = Input(shape=input_shape, name='encoder_input')
         x = Dense(**self.hyper_parameters['hidden'])(inputs)
         z_mean = Dense(**self.hyper_parameters['latent'], name='z_mean')(x)
         z_log_var = Dense(**self.hyper_parameters['latent'], name='z_log_var')(x)
 
         # use reparameterization trick to push the sampling out as input
         # note that "output_shape" isn't necessary
         # with the TensorFlow backend
         z = Lambda(self.sampling,
                    output_shape=(latent_dim,),
                    name='z')([z_mean, z_log_var])
 
-        # instantiate encoder model
-        self.encoder = Model(inputs, [z_mean, z_log_var, z], name='encoder')
+        # instantiate encoders model
+        self.encoder = Model(inputs, [z_mean, z_log_var, z], name='encoders')
 
 
-        # decoder model
+        # decoders model
         latent_inputs = Input(shape=(latent_dim,), name='z_sampling')
         x = Dense(**self.hyper_parameters['hidden'])(latent_inputs)
         outputs = Dense(self.input_dim, activation='sigmoid')(x)
 
-        # instantiate decoder model
-        self.decoder = Model(latent_inputs, outputs, name='decoder')
+        # instantiate decoders model
+        self.decoder = Model(latent_inputs, outputs, name='decoders')
 
         # instantiate VAE model
         outputs = self.decoder(self.encoder(inputs)[2])
         self.autoencoder = Model(inputs, outputs, name='vae_mlp')
 
         # VAE loss = mse_loss or xent_loss + kl_loss
         if self.hyper_parameters['input_distribution']=='bernoulli':
```

## kolibri/backend/tensorflow/autoencoder/decoders/__init__.py

```diff
@@ -1,5 +1,12 @@
+# encoding: utf-8
+
+
+
+# file: __init__.py
+# time: 2:33 
+
 from .att_gru_decoder import AttGRUDecoder  # type: ignore
 from .gru_decoder import GRUDecoder  # type: ignore
 
 if __name__ == "__main__":
     pass
```

## kolibri/backend/tensorflow/autoencoder/decoders/att_gru_decoder.py

```diff
@@ -1,35 +1,39 @@
+# encoding: utf-8
+
 import tensorflow as tf
-from tensorflow.keras.layers import Input
 
-from kolibri.backend.tensorflow.embeddings import Embedding
-from kolibri.backend.tensorflow.layers.behdanau_attention import BahdanauAttention
+from kolibri.backend.tensorflow.embeddings.base_embedding import BaseEmbedding
+from kolibri.backend.tensorflow.layers import L
 
 
 class AttGRUDecoder(tf.keras.Model):
     def __init__(self,
-                 embedding: Embedding,
+                 embedding: BaseEmbedding,
                  vocab_size: int,
                  hidden_size: int = 1024):
         super(AttGRUDecoder, self).__init__()
         self.embedding = embedding
         self.hidden_size = hidden_size
         self.gru = tf.keras.layers.GRU(hidden_size,
                                        return_sequences=True,
                                        return_state=True,
                                        recurrent_initializer='glorot_uniform')
         self.fc = tf.keras.layers.Dense(vocab_size)
 
-        # For attention
-        self.attention = BahdanauAttention(hidden_size)
+        # 用于注意力
+        self.attention = L.BahdanauAttention(hidden_size)
 
     def call(self, x, hidden, enc_output):
         # enc_output shape == (batch_size, max_length, hidden_size)
         context_vector, attention_weights = self.attention(hidden, enc_output)
 
+        if self.embedding.segment:
+            x = x, tf.zeros(x.shape)
+
         # x shape after passing through embedding == (batch_size, 1, embedding_dim)
         x = self.embedding.embed_model(x)
 
         # x shape after concatenation == (batch_size, 1, embedding_dim + hidden_size)
         x = tf.concat([tf.expand_dims(context_vector, 1), x], axis=-1)
 
         # passing the concatenated vector to the GRU
@@ -40,17 +44,17 @@
 
         # output shape == (batch_size, vocab)
         x = self.fc(output)
 
         return x, state, attention_weights
 
     def model(self):
-        x1 = Input(shape=(None,))
-        x2 = Input(shape=(self.hidden_size,))
-        x3 = Input(shape=(self.hidden_size,))
+        x1 = L.Input(shape=(None,))
+        x2 = L.Input(shape=(self.hidden_size,))
+        x3 = L.Input(shape=(self.hidden_size,))
         return tf.keras.Model(inputs=[x1, x2, x3],
                               outputs=self.call(x1, x2, x3),
                               name='AttGRUDecoder')
 
 
 if __name__ == "__main__":
     pass
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## kolibri/backend/tensorflow/autoencoder/decoders/gru_decoder.py

```diff
@@ -1,36 +1,39 @@
+# encoding: utf-8
+
+
 import tensorflow as tf
 
-from kolibri.backend.tensorflow.embeddings import Embedding
+from kolibri.backend.tensorflow.embeddings.base_embedding import BaseEmbedding
 
 
 class GRUDecoder(tf.keras.Model):
     def __init__(self,
-                 embedding: Embedding,
+                 embedding: BaseEmbedding,
                  hidden_size: int,
                  vocab_size: int):
         super(GRUDecoder, self).__init__()
         self.embedding = embedding
 
         self.gru = tf.keras.layers.GRU(hidden_size,
                                        return_sequences=True,
                                        return_state=True,
                                        recurrent_initializer='glorot_uniform')
         self.fc = tf.keras.layers.Dense(vocab_size)
 
     def call(self, dec_input, dec_hidden, enc_output):
-        # The shape of x after passing through the embedding layer == (batch size, 1, embedding dimension)
+        # x 在通过嵌入层后的形状 == （批大小，1，嵌入维度）
         decoder_embedding = self.embedding.embed_model(dec_input)
 
         s = self.gru(decoder_embedding, initial_state=dec_hidden)
         decoder_outputs, decoder_state = s
 
-        # Output shape == (batch size * 1, hidden layer size)
+        # 输出的形状 == （批大小 * 1，隐藏层大小）
         output = tf.reshape(decoder_outputs, (-1, decoder_outputs.shape[2]))
 
-        # Output shape == (batch size, vocab)
+        # 输出的形状 == （批大小，vocab）
         x = self.fc(output)
         return x, decoder_state, None
 
 
 if __name__ == "__main__":
     pass
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## kolibri/backend/tensorflow/autoencoder/decoders/lstm_decoder.py

```diff
@@ -1,29 +1,29 @@
 import tensorflow as tf
 
-class Decoder():
+class Decoder(tf.keras.Model):
 
     def to_dict(self):
         return {
             '__class_name__': self.__class__.__name__,
             '__module__': self.__class__.__module__,
-            'input_shape': self.input_shape,  # type: ignore
+            'decoder_input_shape': self.decoder_input_shape,  # type: ignore
             'dropout': self.dropout,
 
         }
 
-    def __init__(self, input_shape, encoder_states, dropout=0.3):
+    def __init__(self, input_shape, encoder_states,layer1_size=64, layer2_size=200, dropout=0.3):
         super(Decoder, self).__init__()
 
-        self.input_shape=input_shape
+        self.decoder_input_shape=input_shape
         self.dropout=dropout
-        self.decoder_input = tf.keras.Input(shape=self.input_shape)
+        self.decoder_input = tf.keras.Input(shape=self.decoder_input_shape)
         # gaussian_decoder_input = GaussianNoise(0.01)(decoder_input)
 
-        decoder_lstm1 = tf.keras.layers.LSTM(64, return_sequences=True, return_state=True, dropout=self.dropout)
+        decoder_lstm1 = tf.keras.layers.LSTM(layer1_size, return_sequences=True, return_state=True, dropout=self.dropout)
         decoder_output1, _, _ = decoder_lstm1(self.decoder_input, initial_state=encoder_states, training=True)
 
-        decoder_lstm2 = tf.keras.layers.LSTM(200, return_state=True, dropout=self.dropout)
+        decoder_lstm2 = tf.keras.layers.LSTM(layer2_size, return_state=True, dropout=self.dropout)
         decoder_output2, _, _ = decoder_lstm2(decoder_output1, training=True)
 
         decoder_dense = tf.keras.layers.Dense(4)
         self.decoder_output = decoder_dense(decoder_output2)
```

## kolibri/backend/tensorflow/autoencoder/encoders/__init__.py

```diff
@@ -1,5 +1,6 @@
-from kolibri.backend.tensorflow.autoencoder.encoders.lstm_encoder import Encoder
-from kolibri.backend.tensorflow.autoencoder.decoders.lstm_decoder import Decoder
+# encoding: utf-8
+
+from .gru_encoder import GRUEncoder
 
 if __name__ == "__main__":
     pass
```

## kolibri/backend/tensorflow/autoencoder/encoders/gru_encoder.py

```diff
@@ -1,57 +1,36 @@
+# encoding: utf-8
+
 import numpy as np
 import tensorflow as tf
 
-from kolibri.backend.tensorflow.embeddings import Embedding
+from kolibri.backend.tensorflow.embeddings.base_embedding import BaseEmbedding
 from kolibri.backend.tensorflow.layers import L
 
 
 class GRUEncoder(tf.keras.Model):
-    def __init__(self, embedding: Embedding, hidden_size: int = 1024):
+    def __init__(self, embedding: BaseEmbedding, hidden_size: int = 1024):
         super(GRUEncoder, self).__init__()
         self.embedding = embedding
         self.hidden_size = hidden_size
         self.gru = tf.keras.layers.GRU(hidden_size,
                                        return_sequences=True,
                                        return_state=True,
                                        recurrent_initializer='glorot_uniform')
 
     def call(self, x: np.ndarray, hidden: np.ndarray) -> np.ndarray:
+        if self.embedding.segment:
+            x = (x, tf.zeros(x.shape))
         x = self.embedding.embed_model(x)
         output, state = self.gru(x, initial_state=hidden)
         return output, state
 
     def model(self) -> tf.keras.Model:
         x1 = L.Input(shape=(None,))
         x2 = L.Input(shape=(self.hidden_size,))
         return tf.keras.Model(inputs=[x1, x2],
                               outputs=self.call(x1, x2),
                               name='GRUEncoder')
 
 
-
-class LSTMEncoder(tf.keras.Model):
-    def __init__(self, embedding=None, hidden_size: int = 1024, dropout=0.3):
-        super(LSTMEncoder, self).__init__()
-        self.embedding = embedding
-        self.hidden_size = hidden_size
-        self.lstm = tf.keras.layers.LSTM(hidden_size,
-                                       return_sequences=True,
-                                       return_state=True,
-                                        dropout=dropout,
-                                       recurrent_initializer='glorot_uniform')
-
-    def call(self, x: np.ndarray, hidden: np.ndarray, **kwargs):
-        x = self.embedding.embed_model(x)
-        output, state = self.lstm(x, initial_state=hidden)
-        return output, state
-
-    def model(self) -> tf.keras.Model:
-        x1 = L.Input(shape=(None,))
-        x2 = L.Input(shape=(self.hidden_size,))
-        return tf.keras.Model(inputs=[x1, x2],
-                              outputs=self.call(x1, x2),
-                              name='LSTMEncoder')
-
-
 if __name__ == "__main__":
     pass
```

## kolibri/backend/tensorflow/autoencoder/encoders/lstm_encoder.py

```diff
@@ -1,34 +1,34 @@
 import tensorflow as tf
 
 
-class Encoder():
+class Encoder(tf.keras.Model):
     def to_dict(self):
         return {
             '__class_name__': self.__class__.__name__,
             '__module__': self.__class__.__module__,
             'input_shape': self.inout_shape,  # type: ignore
             'dropout': self.dropout,
 
         }
 
-    def __init__(self, input_shape, dropout=0.3):
+    def __init__(self, input_shape, layer1_size=200, layer2_size=64, dropout=0.3):
         super(Encoder, self).__init__( )
-        # encoder
+        # encoders
         self.inout_shape=input_shape
         self.dropout=dropout
         self.encoder_input = tf.keras.Input(shape=self.inout_shape)
         #gaussian_encoder_input = GaussianNoise(0.01)(encoder_input)
 
-        encoder_lstm1 = tf.keras.layers.LSTM(200, return_state = True, return_sequences=True, dropout = self.dropout)
+        encoder_lstm1 = tf.keras.layers.LSTM(layer1_size, return_state = True, return_sequences=True, dropout = self.dropout)
         encoder_output1,state_h1, state_c1 = encoder_lstm1(self.encoder_input, training = True)
 
-        encoder_lstm2 = tf.keras.layers.LSTM(64, return_state = True, dropout = self.dropout)
+        encoder_lstm2 = tf.keras.layers.LSTM(layer2_size, return_state = True, dropout = self.dropout)
         encoder_output2,state_h2, state_c2 = encoder_lstm2(encoder_output1, training = True)
 
         self.encoder_states = [state_h2, state_c2]
 
-        # The encoder model outputs the cell state to provide features for the inference part
+        # The encoders model outputs the cell state to provide features for the inference part
         self.encoder_model = tf.keras.Model(self.encoder_input, state_c2)
 
     def predict(self, input):
         return self.encoder_model.predict(input)
```

## kolibri/backend/tensorflow/callbacks/__init__.py

```diff
@@ -1,4 +1,8 @@
+# encoding: utf-8
+
+
+
 from kolibri.backend.tensorflow.callbacks.eval_callBack import EvalCallBack
 
 if __name__ == "__main__":
     pass
```

## kolibri/backend/tensorflow/callbacks/eval_callBack.py

```diff
@@ -1,50 +1,52 @@
+# encoding: utf-8
+
 from typing import List, Any, Dict
 
 import tensorflow as tf
 from tensorflow import keras
 
-from kolibri.backend.tensorflow.tasks.text.base_model import TextBaseModel
+from kolibri.backend.tensorflow.tasks.base_model import TaskBaseModel
 
 
 class EvalCallBack(keras.callbacks.Callback):
 
     def __init__(self,
-                 kolibri_model: TextBaseModel,
+                 kash_model: TaskBaseModel,
                  x_data: List[Any],
                  y_data: List[Any],
                  *,
                  step: int = 5,
                  truncating: bool = False,
                  batch_size: int = 256) -> None:
         """
         Evaluate callback, calculate precision, recall and f1
         Args:
-            kolibri_model: the dnn task model to evaluate
-            x_data: feature texts for evaluation
-            y_data: label texts for evaluation
+            kash_model: the kolibri task model to evaluate
+            x_data: feature data for evaluation
+            y_data: label data for evaluation
             step: step, default 5
             truncating: truncating: remove values from sequences larger than `model.embedding.sequence_length`
             batch_size: batch size, default 256
         """
         super(EvalCallBack, self).__init__()
-        self.kolibri_model: TextBaseModel = kolibri_model
+        self.kash_model: TaskBaseModel = kash_model
         self.x_data = x_data
         self.y_data = y_data
         self.step = step
         self.truncating = truncating
         self.batch_size = batch_size
         self.logs: List[Dict] = []
 
     def on_epoch_end(self, epoch: int, logs: Any = None) -> None:
         if (epoch + 1) % self.step == 0:
-            report = self.kolibri_model.evaluate(self.x_data,  # type: ignore
-                                                 self.y_data,
-                                                 truncating=self.truncating,
-                                                 batch_size=self.batch_size)
+            report = self.kash_model.evaluate(self.x_data,  # type: ignore
+                                              self.y_data,
+                                              truncating=self.truncating,
+                                              batch_size=self.batch_size)
 
             self.logs.append({
                 'precision': report['precision'],
                 'recall': report['recall'],
                 'f1-score': report['f1-score']
             })
```

## kolibri/backend/tensorflow/embeddings/__init__.py

```diff
@@ -1,5 +1,15 @@
-from kolibri.backend.tensorflow.embeddings.base_embedding import Embedding
-from kolibri.backend.tensorflow.embeddings.default_embedding import DefaultEmbedding
-from kolibri.backend.tensorflow.embeddings.numeric_feature_embedding import NumericFeaturesEmbedding
-from kolibri.backend.tensorflow.embeddings.stacked_embedding import StackedEmbedding
-from kolibri.backend.tensorflow.embeddings.word_embedding import WordEmbedding
+# encoding: utf-8
+
+
+
+# file: __init__.py
+# time: 3:06 
+
+from .base_embedding import BaseEmbedding
+from .bare_embedding import DefaultEmbedding
+from .bert_embedding import BertEmbedding
+from .transformer_embedding import TransformerEmbedding
+from .word_embedding import WordEmbedding
+
+if __name__ == "__main__":
+    pass
```

## kolibri/backend/tensorflow/embeddings/base_embedding.py

```diff
@@ -10,136 +10,23 @@
 import json
 from typing import Dict, List, Any, Optional
 
 import numpy as np
 import tensorflow as tf
 import tqdm
 
-import kolibri.backend
-from kolibri.indexers.base_indexer import BaseIndexer
-from kolibri.logger import get_logger
-
-logger = get_logger(__name__)
+import kolibri
+from kolibri.data.text.generators import CorpusGenerator
+from kolibri.backend.tensorflow.logger import logger
+from kolibri.indexers import BaseIndexer
 
 L = tf.keras.layers
 
 
-class Embedding:
-    def to_dict(self) -> Dict[str, Any]:
-        config: Dict[str, Any] = {
-            'embedding_size': self.embedding_size,
-            'max_position': self.max_position,
-            **self.kwargs
-        }
-        return {
-            '__class_name__': self.__class__.__name__,
-            '__module__': self.__class__.__module__,
-            'config': config,
-            'embed_model': json.loads(self.embed_model.to_json())
-        }
-
-    def __init__(self,
-                 embedding_size: int = 100,
-                 max_position: int = None,
-                 **kwargs: Any):
-
-        self.embed_model: tf.keras.Model = None
-
-        self.kwargs = kwargs
-
-        self.embedding_size: int = embedding_size  # type: ignore
-        self.max_position: int = max_position  # type: ignore
-        self.token2idx = self.load_embed_vocab()
-        self.indexer: Optional[BaseIndexer] = None
-
-    def _override_load_model(self, config: Dict) -> None:
-        embed_model_json_str = json.dumps(config['embed_model'])
-        self.embed_model = tf.keras.models.model_from_json(embed_model_json_str,
-                                                           custom_objects=kolibri.backend.tensorflow.custom_objects)
-
-    def setup_text_processor(self, indexer):
-        self.indexer = indexer
-        self.build_embedding_model(vocab_size=indexer.vocab_size)
-        if self.token2idx:
-            self.indexer.token2idx = self.token2idx
-            self.indexer.idx2token = dict([(v, k) for k, v in self.token2idx.items()])
-
-    def get_seq_length_from_corpus(self,
-                                   generators,
-                                   *,
-                                   use_label: bool = False,
-                                   cover_rate: float = 0.95) -> int:
-        """
-        Calculate proper sequence length_train according to the corpus
-
-        Args:
-            generators:
-            use_label:
-            cover_rate:
-
-        Returns:
-
-        """
-        seq_lens = []
-        for gen in generators:
-            for sentence, label in tqdm.tqdm(gen, desc="Calculating sequence length_train"):
-                if use_label:
-                    seq_lens.append(len(label))
-                else:
-                    seq_lens.append(len(sentence))
-        if cover_rate == 1.0:
-            target_index = -1
-        else:
-            target_index = int(cover_rate * len(seq_lens))
-        sequence_length = sorted(seq_lens)[target_index]
-        logger.debug(f'Calculated sequence length_train = {sequence_length}')
-        print('Calculated sequence length_train = {}'.format(sequence_length))
-        return sequence_length
-
-    def load_embed_vocab(self) -> Optional[Dict[str, int]]:
-        """
-        Load vocab dict from embedding layer
-
-        Returns:
-            vocab dict or None
-        """
-        raise NotImplementedError
-
-    def build_embedding_model(self,
-                              *,
-                              vocab_size: int = None,
-                              force: bool = False,
-                              **kwargs: Dict) -> None:
-        raise NotImplementedError
-
-    def embed(self,
-              sentences: List[List[str]],
-              *,
-              debug: bool = False) -> np.ndarray:
-        """
-        batch embed sentences
-
-        Args:
-            sentences: Sentence list to embed
-            debug: show debug info
-        Returns:
-            vectorized sentence list
-        """
-        if self.indexer is None:
-            raise ValueError('Need to setup the `embedding.setup_text_processor` before calling the embed function.')
-
-        tensor_x = self.indexer.transform(sentences)
-        if debug:
-            logger.debug(f'sentence tensor: {tensor_x}')
-        embed_results = self.embed_model.predict(tensor_x)
-        return embed_results
-
-
-
-class ABCEmbedding:
+class BaseEmbedding:
     def to_dict(self) -> Dict[str, Any]:
         config: Dict[str, Any] = {
             'segment': self.segment,
             'embedding_size': self.embedding_size,
             'max_position': self.max_position,
             **self.kwargs
         }
@@ -159,32 +46,32 @@
         self.embed_model: tf.keras.Model = None
 
         self.segment: bool = segment  # type: ignore
         self.kwargs = kwargs
 
         self.embedding_size: int = embedding_size  # type: ignore
         self.max_position: int = max_position  # type: ignore
-        self.vocab2idx = self.load_embed_vocab()
+        self.token2idx = self.load_embed_vocab()
         self._text_processor: Optional[BaseIndexer] = None
 
     def _override_load_model(self, config: Dict) -> None:
         embed_model_json_str = json.dumps(config['embed_model'])
         self.embed_model = tf.keras.models.model_from_json(embed_model_json_str,
                                                            custom_objects=kolibri.backend.tensorflow.custom_objects)
 
     def setup_text_processor(self, processor: BaseIndexer) -> None:
         self._text_processor = processor
         self.build_embedding_model(vocab_size=processor.vocab_size)
         self._text_processor.segment = self.segment
-        if self.vocab2idx:
-            self._text_processor.vocab2idx = self.vocab2idx
-            self._text_processor.idx2vocab = dict([(v, k) for k, v in self.vocab2idx.items()])
+        if self.token2idx:
+            self._text_processor.token2idx = self.token2idx
+            self._text_processor.idx2token = dict([(v, k) for k, v in self.token2idx.items()])
 
     def get_seq_length_from_corpus(self,
-                                   generators: List,
+                                   generators: List[CorpusGenerator],
                                    *,
                                    use_label: bool = False,
                                    cover_rate: float = 0.95) -> int:
         """
         Calculate proper sequence length according to the corpus
 
         Args:
@@ -246,9 +133,10 @@
                                                   segment=self.segment,
                                                   seq_length=self.max_position)
         if debug:
             logger.debug(f'sentence tensor: {tensor_x}')
         embed_results = self.embed_model.predict(tensor_x)
         return embed_results
 
+
 if __name__ == "__main__":
     pass
```

## kolibri/backend/tensorflow/embeddings/bert_embedding.py

```diff
@@ -1,16 +1,9 @@
 # encoding: utf-8
 
-# author: BrikerMan
-# contact: eliyar917@gmail.com
-# blog: https://eliyar.biz
-
-# file: bert_embedding.py
-# time: 2:49 下午
-
 import os
 from typing import Dict, Any
 
 from kolibri.backend.tensorflow.embeddings.transformer_embedding import TransformerEmbedding
 
 
 class BertEmbedding(TransformerEmbedding):
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## kolibri/backend/tensorflow/embeddings/numeric_feature_embedding.py

```diff
@@ -1,34 +1,36 @@
 # encoding: utf-8
 
-# author: BrikerMan
-# contact: eliyar917@gmail.com
-# blog: https://eliyar.biz
+
 
 # file: numeric_feature_embedding.py
 # time: 2019-05-23 09:04
 
 
 from typing import Union, Optional, Tuple, List
 
 import numpy as np
-from tensorflow import keras
+try:
+    from tensorflow import keras
+    L = keras.layers
+except:
+    pass
+
 from keras.utils import pad_sequences
 
 import kolibri.backend
 from kolibri.backend.tensorflow.embeddings.base_embedding import Embedding
 
 # from kolibri.indexers import BaseIndexer
 
-L = keras.layers
 
 
 # Todo: A better name for this class
 class NumericFeaturesEmbedding(Embedding):
-    """Embedding layer without pre-training, train embedding layer while training model"""
+    """Embeddings layer without pre-training, train embedding layer while training model"""
 
     def info(self):
         info = super(NumericFeaturesEmbedding, self).info()
         info['config'] = {
             'feature_count': self.feature_count,
             'feature_name': self.feature_name,
             'sequence_length': self.sequence_length,
@@ -66,17 +68,17 @@
         self.feature_name = feature_name
         if not from_saved_model:
             self._build_model()
 
     def _build_model(self, **kwargs):
         input_tensor = L.Input(shape=(self.sequence_length,),
                                name=f'input_{self.feature_name}')
-        layer_embedding = L.Embedding(self.feature_count + 1,
-                                      self.embedding_size,
-                                      name=f'layer_embedding_{self.feature_name}')
+        layer_embedding = L.Embeddings(self.feature_count + 1,
+                                       self.embedding_size,
+                                       name=f'layer_embedding_{self.feature_name}')
 
         embedded_tensor = layer_embedding(input_tensor)
         self.embed_model = keras.Model(input_tensor, embedded_tensor)
 
     def analyze_corpus(self,
                        x: Union[Tuple[List[List[str]], ...], List[List[str]]],
                        y: Union[List[List[str]], List[str]]):
```

## kolibri/backend/tensorflow/embeddings/stacked_embedding.py

```diff
@@ -1,12 +1,10 @@
 # encoding: utf-8
 
-# author: BrikerMan
-# contact: eliyar917@gmail.com
-# blog: https://eliyar.biz
+
 
 # file: stacked_embedding.py
 # time: 2019-05-23 09:18
 
 import json
 import pydoc
 from typing import Union, Optional, Tuple, List, Dict
@@ -20,15 +18,15 @@
 from kolibri.backend.tensorflow.layers import L
 
 
 # from kolibri.indexers import BaseIndexer
 
 
 class StackedEmbedding(Embedding):
-    """Embedding layer without pre-training, train embedding layer while training model"""
+    """Embeddings layer without pre-training, train embedding layer while training model"""
 
     @classmethod
     def _load_saved_instance(cls,
                              config_dict: Dict,
                              model_path: str,
                              tf_model: keras.Model):
         embeddings = []
```

## kolibri/backend/tensorflow/embeddings/transformer_embedding.py

```diff
@@ -1,22 +1,21 @@
+# encoding: utf-8
 
 
 import codecs
 import json
 from typing import Dict, List, Any, Optional
 
-from bert4keras.models import build_transformer_model
+#from bert4keras.models import build_transformer_model
 
-from kolibri.backend.tensorflow.embeddings import Embedding
-from kolibri.logger import get_logger
+from kolibri.backend.tensorflow.embeddings.base_embedding import BaseEmbedding
+from kolibri.backend.tensorflow.logger import logger
 
-logger=get_logger(__name__)
 
-
-class TransformerEmbedding(Embedding):
+class TransformerEmbedding(BaseEmbedding):
     """
     TransformerEmbedding is based on bert4keras.
     The embeddings itself are wrapped into our simple embedding interface so that they can be used like any other embedding.
     """
     def to_dict(self) -> Dict[str, Any]:
         info_dic = super(TransformerEmbedding, self).to_dict()
         info_dic['config']['vocab_path'] = self.vocab_path
@@ -79,15 +78,15 @@
                 self.max_position = config['max_position']
             else:
                 self.max_position = config.get('max_position_embeddings')
 
             bert_model = build_transformer_model(config_path=self.config_path,
                                                  checkpoint_path=self.checkpoint_path,
                                                  model=self.model_type,
-                                                 application='encoder',
+                                                 application='encoders',
                                                  return_keras_model=True)
             for layer in bert_model.layers:
                 layer.trainable = False
             self.embed_model = bert_model
             self.embedding_size = bert_model.output.shape[-1]
```

## kolibri/backend/tensorflow/embeddings/word_embedding.py

```diff
@@ -1,22 +1,22 @@
+# encoding: utf-8
+
 from typing import Dict, Any, Optional
 
 import numpy as np
 from gensim.models import KeyedVectors
 from tensorflow import keras
 
-from kolibri.backend.tensorflow.embeddings.base_embedding import Embedding
-from kolibri.logger import get_logger
-
-logger = get_logger(__name__)
+from kolibri.backend.tensorflow.embeddings.base_embedding import BaseEmbedding
+from kolibri.backend.tensorflow.logger import logger
 
 L = keras.layers
 
 
-class WordEmbedding(Embedding):
+class WordEmbedding(BaseEmbedding):
     def to_dict(self) -> Dict[str, Any]:
         info_dic = super(WordEmbedding, self).to_dict()
         info_dic['config']['w2v_path'] = self.w2v_path
         info_dic['config']['w2v_kwargs'] = self.w2v_kwargs
         return info_dic
 
     def __init__(self,
@@ -48,24 +48,24 @@
         token2idx = {
             '[PAD]': 0,
             '[UNK]': 1,
             '[BOS]': 2,
             '[EOS]': 3
         }
 
-        for token in w2v.index_to_key:
+        for token in w2v.index2word:
             token2idx[token] = len(token2idx)
 
         vector_matrix = np.zeros((len(token2idx), w2v.vector_size))
         vector_matrix[1] = np.random.rand(w2v.vector_size)
         vector_matrix[4:] = w2v.vectors
 
         self.embedding_size = w2v.vector_size
         self.w2v_matrix = vector_matrix
-        w2v_top_words = w2v.index_to_key[:50]
+        w2v_top_words = w2v.index2entity[:50]
 
         logger.debug('------------------------------------------------')
         logger.debug("Loaded gensim word2vec model's vocab")
         logger.debug('model        : {}'.format(self.w2v_path))
         logger.debug('word count   : {}'.format(len(self.w2v_matrix)))
         logger.debug('Top 50 words : {}'.format(w2v_top_words))
         logger.debug('------------------------------------------------')
@@ -76,20 +76,20 @@
                               *,
                               vocab_size: int = None,
                               force: bool = False,
                               **kwargs: Dict) -> None:
         if self.embed_model is None:
             input_tensor = L.Input(shape=(None,),
                                    name=f'input')
-            layer_embedding = L.Embedding(len(self.token2idx),
-                                          self.embedding_size,
-                                          weights=[self.w2v_matrix],
-                                          trainable=False,
-                                          mask_zero=True,
-                                          name=f'layer_embedding')
+            layer_embedding = L.Embeddings(len(self.token2idx),
+                                           self.embedding_size,
+                                           weights=[self.w2v_matrix],
+                                           trainable=False,
+                                           mask_zero=True,
+                                           name=f'layer_embedding')
 
             embedded_tensor = layer_embedding(input_tensor)
             self.embed_model = keras.Model(input_tensor, embedded_tensor)
 
 
 if __name__ == "__main__":
     pass
```

## kolibri/backend/tensorflow/layers/__init__.py

```diff
@@ -1,15 +1,39 @@
-#from kapre.composed import get_melspectrogram_layer
-import tensorflow as tf
+"""
+The :mod:`ctgan.layers` module contains the definition of custom neural
+networks layers, and helper methods to initialize their weights and bias.
 
-from kolibri.backend.tensorflow.layers.att_wgt_avg_layer import AttentionWeightedAverage, AttWgtAvgLayer
-from kolibri.backend.tensorflow.layers.att_wgt_avg_layer import AttentionWeightedAverageLayer
-from kolibri.backend.tensorflow.layers.folding_layer import FoldingLayer
-from kolibri.backend.tensorflow.layers.kmax_pool_layer import KMaxPoolingLayer, KMaxPoolLayer, KMaxPooling
-from kolibri.backend.tensorflow.layers.non_masking_layer import NonMaskingLayer
-from kolibri.backend.tensorflow.layers.multi_head_attention import MultiHeadSelfAttention
-#Melspectrogram = get_melspectrogram_layer
+For further details, please consult sections 4.4 of :cite:`xu2019modeling`.
+"""
 
-L = tf.keras.layers
+from .layer_utils import init_bounded
+from .residual import ResidualLayer
+from .gen_activation import GenActivation
 
-if __name__ == "__main__":
-    print("Hello world")
+# encoding: utf-8
+
+
+
+# file: __init__.py
+# time: 7:39
+
+from typing import Dict, Any
+from tensorflow import keras
+
+from .conditional_random_field import KConditionalRandomField
+from .behdanau_attention import BahdanauAttention  # type: ignore
+
+L = keras.layers
+L.BahdanauAttention = BahdanauAttention
+L.KConditionalRandomField = KConditionalRandomField
+
+
+def resigter_custom_layers(custom_objects: Dict[str, Any]) -> Dict[str, Any]:
+    custom_objects['KConditionalRandomField'] = KConditionalRandomField
+    custom_objects['BahdanauAttention'] = BahdanauAttention
+    return custom_objects
+
+__all__ = [
+    'init_bounded',
+    'ResidualLayer',
+    'GenActivation'
+]
```

## kolibri/backend/tensorflow/layers/behdanau_attention.py

```diff
@@ -1,11 +1,17 @@
-import tensorflow as tf
+# encoding: utf-8
+
 
+# type: ignore
+
+import tensorflow as tf
+from tensorflow.python.util.tf_export import keras_export
 
 
+@keras_export('keras.layers.BahdanauAttention')
 class BahdanauAttention(tf.keras.layers.Layer):
     def __init__(self, units):
         super(BahdanauAttention, self).__init__()
         self.W1 = tf.keras.layers.Dense(units)
         self.W2 = tf.keras.layers.Dense(units)
         self.V = tf.keras.layers.Dense(1)
```

## kolibri/backend/tensorflow/tasks/__init__.py

```diff
@@ -1 +1,11 @@
-from kolibri.backend.tensorflow.tasks.dnn_estimator import DnnEstimator
+# encoding: utf-8
+
+
+
+# file: __init__.py
+# time: 4:04 
+
+from kolibri.backend.tensorflow.tasks.text import classification
+
+if __name__ == "__main__":
+    pass
```

## kolibri/backend/tensorflow/tasks/structured/base_model.py

```diff
@@ -5,15 +5,15 @@
 from typing import Dict, Any
 
 import numpy as np
 import tempfile, time
 from sklearn import metrics as sklearn_metrics
 
 import h5py
-from kolibri.data.text.generators import DataGenerator
+from kolibri.data.text.generators import CorpusGenerator
 from kolibri.backend.tensorflow.tasks.base_model import TaskBaseModel
 from kolibri.default_configs import DEFAULT_NN_MODEL_FILENAME
 from kolibri.backend.tensorflow.utils import load_data_object
 from kolibri.logger import get_logger
 import tensorflow as tf
 logger = get_logger(__name__)
 
@@ -60,15 +60,15 @@
             x_train:
             y_train:
 
         Returns:
 
         """
 
-        train_gen = DataGenerator(x_train, y_train)
+        train_gen = CorpusGenerator(x_train, y_train)
         self.build_model_generator(train_gen)
 
     def build_model_generator(self, generators):
 
         if self.tf_model is None:
             self.build_model_arc(generators)
         self.compile_model()
```

## kolibri/backend/tensorflow/tasks/structured/regression/base_model.py

```diff
@@ -1,15 +1,15 @@
 import operator
 from typing import List, Dict, Any
 import tempfile
 import numpy as np
 from sklearn import metrics as sklearn_metrics
 
 import kolibri
-from kolibri.data.text.generators import DataGenerator
+from kolibri.data.text.generators_ import DataGenerator
 from kolibri.backend.tensorflow.tasks.structured.base_model import BaseStructuredModel
 from kolibri.backend.tensorflow.embeddings import DefaultEmbedding
 from kolibri.default_configs import DEFAULT_NN_MODEL_FILENAME
 from kolibri.logger import get_logger
 
 logger = get_logger(__name__)
```

## kolibri/backend/tensorflow/tasks/structured/regression/dnn_regression_estimator.py

```diff
@@ -2,15 +2,15 @@
 from kolibri.core.component import Component
 import pathlib, os, json
 from kolibri.backend.tensorflow.tasks.structured.regression.models import get_model
 import tensorflow as tf
 import kolibri
 from kolibri.config import override_defaults
 from kolibri.logger import get_logger
-from kolibri.backend.tensorflow.tasks.dnn_estimator import DnnEstimator
+from kolibri.task.dnn_estimator import DnnEstimator
 logger = get_logger(__name__)
 
 KOLIBRI_MODEL_FILE_NAME = "regressor_lstm.pkl"
 DNN_MODEL_FILE_NAME = "regressor_dnn"
 
 
 class DnnRegressionEstimator(DnnEstimator):
```

## kolibri/backend/tensorflow/tasks/structured/regression/models.py

```diff
@@ -37,17 +37,17 @@
                 'rate': 0.02
             }
         }
 
     def build_model_arc(self, generators):
         config = self.hyper_parameters
 
-        embeding_size=generators.x_values[0].shape[1]
-        time_steps=generators.x_values[1].shape[1]
-        n_features=generators.x_values[1].shape[2]
+        embeding_size=generators.x_data[0].shape[1]
+        time_steps=generators.x_data[1].shape[1]
+        n_features=generators.x_data[1].shape[2]
         X = tf.keras.Input(shape=(embeding_size,))
 
         F = tf.keras.Input(shape=(time_steps, n_features,))
 
         lstm = tf.keras.layers.LSTM( **config['lstm1'], input_shape=(time_steps, n_features,))
 
         out_lstm = lstm(F)
```

## kolibri/backend/tensorflow/tasks/text/__init__.py

```diff
@@ -1 +0,0 @@
-00000000: 0a                                       .
```

## kolibri/backend/tensorflow/tasks/text/classification/__init__.py

```diff
@@ -1 +1,23 @@
-from .models import *
+# encoding: utf-8
+
+
+
+# file: __init__.py
+# time: 4:05 
+
+from .base_model import BaseTextClassificationModel
+from .models import BiGRU_Model, BiLSTM_Model,CNN_GRU_Model, CNN_LSTM_Model, CNN_Model
+from .cnn_attention_model import CNN_Attention_Model
+
+
+ALL_MODELS = [
+    BiGRU_Model,
+    BiLSTM_Model,
+    CNN_Attention_Model,
+    CNN_GRU_Model,
+    CNN_LSTM_Model,
+    CNN_Model
+]
+
+if __name__ == "__main__":
+    pass
```

## kolibri/backend/tensorflow/tasks/text/classification/base_model.py

```diff
@@ -1,105 +1,154 @@
-import operator
-from typing import List, Dict, Any
+# encoding: utf-8
 
+# author: BrikerMan
+# contact: eliyar917@gmail.com
+# blog: https://eliyar.biz
+
+# file: abs_model.py
+# time: 4:05 下午
+
+import random
+from abc import ABC
 import numpy as np
+from typing import List, Dict, Any, Union
+
 from sklearn import metrics as sklearn_metrics
+from tensorflow import keras
 
 import kolibri
-from kolibri.data.text.generators import DataGenerator
-from kolibri.backend.tensorflow.tasks.text.base_model import TextBaseModel
-from kolibri.backend.tensorflow.embeddings import DefaultEmbedding
+from kolibri.backend.tensorflow.embeddings import BaseEmbedding, DefaultEmbedding
+from kolibri.data.text.generators import BatchDataSet, CorpusGenerator
 from kolibri.backend.tensorflow.layers import L
-from kolibri.logger import get_logger
-
-logger = get_logger(__name__)
+from kolibri.backend.tensorflow.logger import logger
+from kolibri.backend.tensorflow.metrics.multi_label_classification import multi_label_classification_report
+from kolibri.indexers import BaseIndexer
+from kolibri.indexers import LabelIndexer
+from kolibri.indexers import SequenceIndexer
+from kolibri.backend.tensorflow.tasks.base_model import TaskBaseModel
+from kolibri.types import TextSamplesVar, ClassificationLabelVar, MultiLabelClassificationLabelVar
 
-from kdmt.ml.metrics.multi_label_classification import multi_label_classification_report
 
-
-class BaseTextClassificationModel(TextBaseModel):
+class BaseTextClassificationModel(TaskBaseModel, ABC):
     """
     Abstract Classification Model
     """
 
     __task__ = 'classification'
 
     def to_dict(self) -> Dict:
         info = super(BaseTextClassificationModel, self).to_dict()
         info['config']['multi_label'] = self.multi_label
         return info
 
-    def __init__(self, embedding=None, *, sequence_length=None, hyper_parameters=None, multi_label: bool = False,
-                 content_indexer=None, label_indexer=None):
+    def __init__(self,
+                 embedding: BaseEmbedding = None,
+                 *,
+                 sequence_length: int = None,
+                 hyper_parameters: Dict[str, Dict[str, Any]] = None,
+                 multi_label: bool = False,
+                 text_processor: BaseIndexer = None,
+                 label_processor: BaseIndexer = None):
         """
 
         Args:
             embedding: embedding object
-            sequence_length: target sequence length_train
+            sequence_length: target sequence length
             hyper_parameters: hyper_parameters to overwrite
             multi_label: is multi-label classification
-            content_indexer: text processor
-            label_indexer: label processor
+            text_processor: text processor
+            label_processor: label processor
         """
-        super().__init__(embedding, sequence_length, hyper_parameters, multi_label, content_indexer, label_indexer)
+        super(BaseTextClassificationModel, self).__init__()
+        if embedding is None:
+            embedding = DefaultEmbedding()  # type: ignore
+
+        if hyper_parameters is None:
+            hyper_parameters = self.get_default_hyper_parameters()
+
+        if text_processor is None:
+            text_processor = SequenceIndexer()
+
+        if label_processor is None:
+            label_processor = LabelIndexer(multi_label=multi_label)
+
+        self.tf_model: keras.Model = None
+        self.embedding = embedding
+        self.hyper_parameters = hyper_parameters
+        self.sequence_length = sequence_length
+        self.multi_label = multi_label
+
+        self.text_processor = text_processor
+        self.label_indexer = label_processor
 
     def _activation_layer(self) -> L.Layer:
         if self.multi_label:
             return L.Activation('sigmoid')
         else:
             return L.Activation('softmax')
 
     def build_model(self,
-                    x_train,
-                    y_train):
+                    x_train: TextSamplesVar,
+                    y_train: Union[ClassificationLabelVar, MultiLabelClassificationLabelVar]) -> None:
         """
         Build Model with x_data and y_data
 
         This function will setup a :class:`CorpusGenerator`,
          then call py:meth:`BaseTextClassificationModel.build_model_gen` for preparing processor and model
 
         Args:
             x_train:
             y_train:
 
         Returns:
 
         """
 
-        train_gen = DataGenerator(x_train, y_train)
+        train_gen = CorpusGenerator(x_train, y_train)
         self.build_model_generator([train_gen])
 
-    def build_model_generator(self, generators):
-        if not self.content_indexer.token2idx:
-            self.content_indexer.build_vocab_generator(generators)
-
+    def build_model_generator(self,
+                              generators: List[CorpusGenerator]) -> None:
+        if not self.text_processor.token2idx:
+            self.text_processor.build_vocab_generator(generators)
         self.label_indexer.build_vocab_generator(generators)
-        self.embedding.setup_text_processor(self.content_indexer)
+        self.embedding.setup_text_processor(self.text_processor)
 
         if self.sequence_length is None:
             self.sequence_length = self.embedding.get_seq_length_from_corpus(generators)
 
         if self.tf_model is None:
             self.build_model_arc()
             self.compile_model()
 
-    @classmethod
-    def get_default_hyper_parameters(cls) -> Dict[str, Dict[str, Any]]:
-        raise NotImplementedError
-
-    def build_model_arc(self):
+    def build_model_arc(self) -> None:
         raise NotImplementedError
 
     def compile_model(self,
                       loss: Any = None,
                       optimizer: Any = None,
                       metrics: Any = None,
                       **kwargs: Any) -> None:
         """
         Configures the model for training.
+        call :meth:`tf.keras.Model.predict` to compile model with custom loss, optimizer and metrics
+
+        Examples:
+
+            >>> model = BiLSTM_Model()
+            # Build model with corpus
+            >>> model.build_model(train_x, train_y)
+            # Compile model with custom loss, optimizer and metrics
+            >>> model.compile(loss='categorical_crossentropy', optimizer='rsm', metrics = ['accuracy'])
+
+        Args:
+            loss: name of objective function, objective function or ``tf.keras.losses.Loss`` instance.
+            optimizer: name of optimizer or optimizer instance.
+            metrics (object): List of metrics to be evaluated by the model during training and testing.
+            **kwargs: additional params passed to :meth:`tf.keras.Model.predict``.
         """
         if loss is None:
             if self.multi_label:
                 loss = 'binary_crossentropy'
             else:
                 loss = 'sparse_categorical_crossentropy'
         if optimizer is None:
@@ -108,128 +157,196 @@
             metrics = ['accuracy']
 
         self.tf_model.compile(loss=loss,
                               optimizer=optimizer,
                               metrics=metrics,
                               **kwargs)
 
-    def predict(self, x_data, *,
-                top_k=5,
+    def fit(self,
+            x_train: TextSamplesVar,
+            y_train: Union[ClassificationLabelVar, MultiLabelClassificationLabelVar],
+            x_validate: TextSamplesVar = None,
+            y_validate: Union[ClassificationLabelVar, MultiLabelClassificationLabelVar] = None,
+            *,
+            batch_size: int = 64,
+            epochs: int = 5,
+            callbacks: List['keras.callbacks.Callback'] = None,
+            fit_kwargs: Dict = None) -> 'keras.callbacks.History':
+        """
+        Trains the model for a given number of epochs with given data set list.
+
+        Args:
+            x_train: Array of train feature data (if the model has a single input),
+                or tuple of train feature data array (if the model has multiple inputs)
+            y_train: Array of train label data
+            x_validate: Array of validation feature data (if the model has a single input),
+                or tuple of validation feature data array (if the model has multiple inputs)
+            y_validate: Array of validation label data
+            batch_size: Number of samples per gradient update, default to 64.
+            epochs: Number of epochs to train the model.
+                An epoch is an iteration over the entire `x` and `y` data provided.
+            callbacks: List of `tf.keras.callbacks.Callback` instances.
+                List of callbacks to apply during training.
+                See :class:`tf.keras.callbacks`.
+            fit_kwargs: fit_kwargs: additional arguments passed to :meth:`tf.keras.Model.fit`
+
+        Returns:
+            A :class:`tf.keras.callback.History`  object. Its `History.history` attribute is
+            a record of training loss values and metrics values
+            at successive epochs, as well as validation loss values
+            and validation metrics values (if applicable).
+        """
+        train_gen = CorpusGenerator(x_train, y_train)
+        if x_validate is not None:
+            valid_gen = CorpusGenerator(x_validate, y_validate)
+        else:
+            valid_gen = None
+        return self.fit_generator(train_sample_gen=train_gen,
+                                  valid_sample_gen=valid_gen,
+                                  batch_size=batch_size,
+                                  epochs=epochs,
+                                  callbacks=callbacks,
+                                  fit_kwargs=fit_kwargs)
+
+    def fit_generator(self,
+                      train_sample_gen: CorpusGenerator,
+                      valid_sample_gen: CorpusGenerator = None,
+                      *,
+                      batch_size: int = 64,
+                      epochs: int = 5,
+                      callbacks: List['keras.callbacks.Callback'] = None,
+                      fit_kwargs: Dict = None) -> 'keras.callbacks.History':
+        """
+        Trains the model for a given number of epochs with given data generator.
+
+        Data generator must be the subclass of `CorpusGenerator`
+
+        Args:
+            train_sample_gen: train data generator.
+            valid_sample_gen: valid data generator.
+            batch_size: Number of samples per gradient update, default to 64.
+            epochs: Number of epochs to train the model.
+                An epoch is an iteration over the entire `x` and `y` data provided.
+            callbacks: List of `tf.keras.callbacks.Callback` instances.
+                List of callbacks to apply during training.
+                See `tf.keras.callbacks`.
+            fit_kwargs: fit_kwargs: additional arguments passed to :meth:`tf.keras.Model.fit`
+
+        Returns:
+            A :py:class:`tf.keras.callback.History`  object. Its `History.history` attribute is
+            a record of training loss values and metrics values
+            at successive epochs, as well as validation loss values
+            and validation metrics values (if applicable).
+        """
+        self.build_model_generator([g for g in [train_sample_gen, valid_sample_gen] if g])
+
+        model_summary = []
+        self.tf_model.summary(print_fn=lambda x: model_summary.append(x))
+        logger.debug('\n'.join(model_summary))
+
+        train_set = BatchDataSet(train_sample_gen,
+                                 text_processor=self.text_processor,
+                                 label_processor=self.label_indexer,
+                                 segment=self.embedding.segment,
+                                 seq_length=self.sequence_length,
+                                 batch_size=batch_size)
+
+        if fit_kwargs is None:
+            fit_kwargs = {}
+
+        if valid_sample_gen:
+            valid_gen = BatchDataSet(valid_sample_gen,
+                                     text_processor=self.text_processor,
+                                     label_processor=self.label_indexer,
+                                     segment=self.embedding.segment,
+                                     seq_length=self.sequence_length,
+                                     batch_size=batch_size)
+            fit_kwargs['validation_data'] = valid_gen.take()
+            fit_kwargs['validation_steps'] = len(valid_gen)
+
+        return self.tf_model.fit(train_set.take(),
+                                 steps_per_epoch=len(train_set),
+                                 epochs=epochs,
+                                 callbacks=callbacks,
+                                 **fit_kwargs)
+
+    def predict(self,
+                x_data: TextSamplesVar,
+                *,
                 batch_size: int = 32,
                 truncating: bool = False,
                 multi_label_threshold: float = 0.5,
-                predict_kwargs: Dict = None):
+                predict_kwargs: Dict = None) -> Union[ClassificationLabelVar, MultiLabelClassificationLabelVar]:
         """
         Generates output predictions for the input samples.
 
         Computation is done in batches.
 
         Args:
-            x_data: The input texts, as a Numpy array (or list of Numpy arrays if the model has multiple inputs).
+            x_data: The input data, as a Numpy array (or list of Numpy arrays if the model has multiple inputs).
             batch_size: Integer. If unspecified, it will default to 32.
             truncating: remove values from sequences larger than `model.embedding.sequence_length`
             multi_label_threshold:
             predict_kwargs: arguments passed to ``predict()`` function of ``tf.keras.Model``
 
         Returns:
             array(s) of predictions.
         """
         if predict_kwargs is None:
             predict_kwargs = {}
-        with kolibri.backend.tensorflow.custom_object_scope():
-            tensor = self.content_indexer.transform(x_data, )
-            logger.debug(f'predict input shape {np.array(tensor).shape}')
+        with kolibri.backend.tensorflow.utils.custom_object_scope():
+            if truncating:
+                seq_length = self.sequence_length
+            else:
+                seq_length = None
+            tensor = self.text_processor.transform(x_data,
+                                                   segment=self.embedding.segment,
+                                                   seq_length=seq_length,
+                                                   max_position=self.embedding.max_position)
+            logger.debug(f'predict input shape {np.array(tensor).shape} x: \n{tensor}')
             pred = self.tf_model.predict(tensor, batch_size=batch_size, **predict_kwargs)
             logger.debug(f'predict output shape {pred.shape}')
-            sorted_indices = np.fliplr(np.argsort(pred, axis=1))
             if self.multi_label:
                 multi_label_binarizer = self.label_indexer.multi_label_binarizer  # type: ignore
-                labels = multi_label_binarizer.inverse_transform(pred,
+                res = multi_label_binarizer.inverse_transform(pred,
                                                               threshold=multi_label_threshold)
             else:
-                labels=np.array([self.label_indexer.inverse_transform(p) for p in sorted_indices])
-
-#                logger.debug(f'predict output: {res}')
-
-
-
-
-        return labels, pred[np.arange(pred.shape[0])[:, None], sorted_indices]
-
-    def predict_top_k_class(self,
-                            x_data,
-                            top_k=5,
-                            batch_size=32,
-                            debug_info=False,
-                            truncating: bool = False,
-                            predict_kwargs: Dict = None) -> List[Dict]:
-        """
-        Generates output predictions with confidence for the input samples.
-        """
-        if predict_kwargs is None:
-            predict_kwargs = {}
-        with kolibri.backend.custom_object_scope():
-            if truncating:
-                seq_length = self.sequence_length
-            else:
-                seq_length = None
-            tensor = self.content_indexer.transform(x_data, )
-
-            pred = self.tf_model.predict(tensor, batch_size=batch_size, **predict_kwargs)
-            new_results = []
-
-            for sample_prob in pred:
-                sample_res = zip(self.label_indexer.idx2token.keys(), sample_prob)
-                sample_res = sorted(sample_res, key=lambda k: k[1], reverse=True)
-                data = {}
-                for label, confidence in sample_res[:top_k]:
-                    if 'candidates' not in data:
-                        if self.embedding.indexer.multi_label:
-                            data['candidates'] = []
-                        else:
-                            data['label'] = label
-                            data['confidence'] = confidence
-                            data['candidates'] = []
-                            continue
-                    data['candidates'].append({
-                        'label': label,
-                        'confidence': confidence
-                    })
-
-                new_results.append(data)
-
-            if debug_info:
-                logger.info('input: {}'.format(tensor))
-                logger.info('output: {}'.format(pred))
-                logger.info('output argmax: {}'.format(pred.argmax(-1)))
-        return new_results
-
-    def evaluate(self, x_data, y_data, *,
+                pred_argmax = pred.argmax(-1)
+                lengths = [len(sen) for sen in x_data]
+                res = self.label_indexer.inverse_transform(pred_argmax,
+                                                           lengths=lengths)
+                logger.debug(f'predict output argmax: {pred_argmax}')
+
+        return res
+
+    def evaluate(self,  # type: ignore[override]
+                 x_data: TextSamplesVar,
+                 y_data: Union[ClassificationLabelVar, MultiLabelClassificationLabelVar],
+                 *,
                  batch_size: int = 32,
                  digits: int = 4,
                  multi_label_threshold: float = 0.5,
-                 truncating: bool = False, ):
+                 truncating: bool = False,) -> Dict:
         y_pred = self.predict(x_data,
                               batch_size=batch_size,
                               truncating=truncating,
                               multi_label_threshold=multi_label_threshold)
 
-
         if self.multi_label:
             report = multi_label_classification_report(y_data,  # type: ignore
                                                        y_pred,  # type: ignore
                                                        binarizer=self.label_indexer.multi_label_binarizer)  # type: ignore
 
         else:
             original_report = sklearn_metrics.classification_report(y_data,
-                                                                    y_pred[0][:,0],
+                                                                    y_pred,
                                                                     output_dict=True,
                                                                     digits=digits)
             print(sklearn_metrics.classification_report(y_data,
-                                                        y_pred[0][:,0],
+                                                        y_pred,
                                                         output_dict=False,
                                                         digits=digits))
             report = {
                 'detail': original_report,
                 **original_report['weighted avg']
             }
         return report
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## kolibri/backend/tensorflow/tasks/text/classification/cnn_attention_model.py

```diff
@@ -1,38 +1,39 @@
-from typing import Dict, Any
+# encoding: utf-8
+
 
+from abc import ABC
+from typing import Dict, Any
 import tensorflow as tf
 import tensorflow.keras.layers as L
 from tensorflow import keras
+from kolibri.backend.tensorflow.logger import logger
 
 from kolibri.backend.tensorflow.tasks.text.classification.base_model import BaseTextClassificationModel
-from kolibri.logger import get_logger
 
-logger = get_logger(__name__)
 
-
-class CNN_Attention_Model(BaseTextClassificationModel):
+class CNN_Attention_Model(BaseTextClassificationModel, ABC):
 
     @classmethod
-    def get_default_hyper_parameters(cls) -> Dict[str, Dict[str, Any]]:
+    def default_hyper_parameters(cls) -> Dict[str, Dict[str, Any]]:
         return {
             'conv_layer1': {
-                'filters': 128,
+                'filters': 264,
                 'kernel_size': 3,
                 'padding': 'same',
                 'activation': 'relu'
             },
             'conv_layer2': {
-                'filters': 64,
+                'filters': 128,
                 'kernel_size': 3,
                 'padding': 'same',
                 'activation': 'relu'
             },
             'conv_layer3': {
-                'filters': 32,
+                'filters': 64,
                 'kernel_size': 3,
                 'padding': 'same',
                 'activation': 'relu'
             },
             'layer_output': {
             },
         }
@@ -79,11 +80,11 @@
         # Concatenate query and document encodings to produce a DNN input layer.
         input_layer = L.Concatenate(axis=-1)([query_encoding, query_value_attention])
 
         output = L.Dense(output_dim, **config['layer_output'])(input_layer)
         output = self._activation_layer()(output)
 
         self.tf_model = keras.Model(embed_model.input, output)
-        print(self.tf_model.summary())
+
 
 if __name__ == "__main__":
     pass
```

## kolibri/backend/tensorflow/tasks/text/classification/dpcnn_model.py

```diff
@@ -14,15 +14,15 @@
 
 from math import log2, floor
 from typing import Dict, Any
 
 import tensorflow as tf
 
 from kolibri.backend.tensorflow.tasks.text.classification.base_model import BaseTextClassificationModel
-from kolibri.backend.tensorflow.layers import L, KMaxPoolingLayer
+from kolibri.backend.tensorflow.layers.kmax_pool_layer import L, KMaxPoolingLayer
 
 
 class DPCNN_Model(BaseTextClassificationModel):
     '''
     This implementation of DPCNN requires a clear declared sequence length_train.
     So sequences input in should be padded or cut to a given length_train in advance.
     '''
```

## kolibri/backend/tensorflow/tasks/text/classification/models.py

```diff
@@ -1,15 +1,19 @@
 from typing import Dict, Any
 
 import tensorflow as tf
+from tensorflow import keras
 
 from kolibri.backend.tensorflow.tasks.text.classification.base_model import BaseTextClassificationModel
 from kolibri.backend.tensorflow.tasks.text.classification.cnn_attention_model import CNN_Attention_Model
 from kolibri.backend.tensorflow.tasks.text.classification.dpcnn_model import DPCNN_Model
-from kolibri.backend.tensorflow.layers import L, AttentionWeightedAverageLayer, KMaxPoolingLayer, MultiHeadSelfAttention
+from kolibri.backend.tensorflow.layers import L
+from kolibri.backend.tensorflow.layers.att_wgt_avg_layer import AttentionWeightedAverageLayer
+from kolibri.backend.tensorflow.layers.kmax_pool_layer import KMaxPoolingLayer
+from kolibri.backend.tensorflow.layers.multi_head_attention import MultiHeadSelfAttention
 
 #tf.compat.v1.disable_eager_execution()
 
 class FastText(BaseTextClassificationModel):
 
     @classmethod
     def get_default_hyper_parameters(cls):
@@ -43,27 +47,27 @@
 
         self.tf_model = tf.keras.Model(embed_model.inputs, tensor)
 
         print(self.tf_model.summary())
 
 
 class BiLSTM_Model(BaseTextClassificationModel):
-
     @classmethod
-    def get_default_hyper_parameters(cls):
+    def get_default_hyper_parameters(cls) -> Dict[str, Dict[str, Any]]:
         return {
             'layer_bi_lstm': {
                 'units': 128,
                 'return_sequences': False
             },
             'layer_output': {
+
             }
         }
 
-    def build_model_arc(self):
+    def build_model_arc(self) -> None:
         output_dim = self.label_indexer.vocab_size
 
         config = self.hyper_parameters
         embed_model = self.embedding.embed_model
 
         # build model structure in sequent way
         layer_stack = [
@@ -72,16 +76,15 @@
             self._activation_layer()
         ]
 
         tensor = embed_model.output
         for layer in layer_stack:
             tensor = layer(tensor)
 
-        self.tf_model = tf.keras.Model(embed_model.inputs, tensor)
-        print(self.tf_model.summary())
+        self.tf_model: keras.Model = keras.Model(embed_model.inputs, tensor)
 
 class BiGRU_Model(BaseTextClassificationModel):
 
     @classmethod
     def get_default_hyper_parameters(cls):
         return {
             'layer_bi_gru': {
@@ -819,15 +822,15 @@
 #    corpus=corpus.sample(n=2000)
 #    corpus=corpus.groupby("target").filter(lambda x: len(x) > 100)
 #    corpus["content"]=corpus['translated_title_fr']+"\n"+corpus['translated_clean_body_fr']
 #    corpus.dropna(subset=["content"], inplace=True)
 
     x_train = corpus['f_body'].values.tolist()
     y_train = corpus['target'].values.tolist()
-    m = FastText()
+    m = BiLSTM_Model()
 
     x_train = [x.split() for x in x_train]
     # m.build_model(x, y)
     m.fit(x_train, y_train, epochs=1)
 
     print(m.predict(x_train[:10]))
     # m.evaluate(x, y)
```

## kolibri/backend/tensorflow/tasks/text/labeling/__init__.py

```diff
@@ -1,3 +1,19 @@
-from kolibri.backend.tensorflow.tasks.text.labeling.models import *
+# encoding: utf-8
+
+from .base_model import BaseLabelingModel
+from .bi_gru_model import BiGRU_Model
+from .bi_gru_crf_model import BiGRU_CRF_Model
+from .bi_lstm_model import BiLSTM_Model
+from .bi_lstm_crf_model import BiLSTM_CRF_Model
+from .cnn_lstm_model import CNN_LSTM_Model
+
+ALL_MODELS = [
+    BiGRU_Model,
+    BiGRU_CRF_Model,
+    BiLSTM_Model,
+    BiLSTM_CRF_Model,
+    CNN_LSTM_Model,
+]
+
 if __name__ == "__main__":
-    print("Hello world")
+    pass
```

## kolibri/backend/tensorflow/tasks/text/labeling/base_model.py

```diff
@@ -1,75 +1,94 @@
-import logging
-from typing import Dict, Any
+# encoding: utf-8
+
+# author: BrikerMan
+# contact: eliyar917@gmail.com
+# blog: https://eliyar.biz
+
+# file: base_model.py
+# time: 4:30 下午
+
+from abc import ABC
+from typing import List, Dict, Any, Union, Optional
 
 import numpy as np
-from seqeval.metrics.sequence_labeling import get_entities
+import tensorflow as tf
 
 import kolibri
-from kolibri.data.text.generators import DataGenerator
-from kolibri.backend.tensorflow.tasks.text.base_model import TextBaseModel
-from kolibri.backend.tensorflow.embeddings import DefaultEmbedding
+from kolibri.backend.tensorflow.embeddings import BaseEmbedding, DefaultEmbedding
+from kolibri.data.text.generators import CorpusGenerator, BatchDataSet
+from kolibri.backend.tensorflow.layers import KConditionalRandomField
+from kolibri.backend.tensorflow.logger import logger
+from kolibri.backend.tensorflow.metrics.sequence_labeling import get_entities
+from kolibri.backend.tensorflow.metrics.sequence_labeling import sequence_labeling_report
 from kolibri.indexers import SequenceIndexer
-from kolibri.logger import get_logger
+from kolibri.backend.tensorflow.tasks.base_model import TaskBaseModel
+from kolibri.types import TextSamplesVar
 
-logger = get_logger(__name__)
 
-from kdmt.ml.metrics.sequences import labeling_report
-
-
-class BaseLabelingModel(TextBaseModel):
+class BaseLabelingModel(TaskBaseModel, ABC):
     """
     Abstract Labeling Model
     """
 
-    def __init__(self, embedding=None, sequence_length: int = None, hyper_parameters: Dict[str, Dict[str, Any]] = None):
+    def __init__(self,
+                 embedding: BaseEmbedding = None,
+                 sequence_length: int = None,
+                 hyper_parameters: Dict[str, Dict[str, Any]] = None):
         """
 
         Args:
             embedding: embedding object
-            sequence_length: target sequence length_train
+            sequence_length: target sequence length
             hyper_parameters: hyper_parameters to overwrite
         """
-        #       super(BaseLabelingModel, self).__init__()
-        super(BaseLabelingModel, self).__init__(embedding, sequence_length, hyper_parameters)
-        if self.embedding is None:
-            self.embedding = DefaultEmbedding()  # type: ignore
-
-        if self.hyper_parameters is None:
-            self.hyper_parameters = self.get_default_hyper_parameters()
-
+        super(BaseLabelingModel, self).__init__()
+        if embedding is None:
+            embedding = DefaultEmbedding()  # type: ignore
+
+        if hyper_parameters is None:
+            hyper_parameters = self.default_hyper_parameters()
+
+        self.tf_model: Optional[tf.keras.Model] = None
+        self.embedding = embedding
+        self.hyper_parameters = hyper_parameters
         self.sequence_length = sequence_length
-        self.content_indexer = SequenceIndexer()
-        self.label_indexer = SequenceIndexer(build_in_vocab='labeling',
-                                             min_count=1,
-                                             build_vocab_from_labels=True)
-
-    def build_model(self, x_data, y_data):
+        self.text_processor: SequenceIndexer = SequenceIndexer()
+        self.label_processor: SequenceIndexer = SequenceIndexer(build_in_vocab='labeling',
+                                                                    min_count=1,
+                                                                    build_vocab_from_labels=True)
+
+        self.crf_layer: Optional[KConditionalRandomField] = None
+
+    def build_model(self,
+                    x_data: TextSamplesVar,
+                    y_data: TextSamplesVar) -> None:
         """
         Build Model with x_data and y_data
 
         This function will setup a :class:`CorpusGenerator`,
          then call :meth:`BaseTextClassificationModel.build_model_gen` for preparing processor and model
 
         Args:
             x_data:
             y_data:
 
         Returns:
 
         """
 
-        train_gen = DataGenerator(x_data, y_data)
+        train_gen = CorpusGenerator(x_data, y_data)
         self.build_model_generator([train_gen])
 
-    def build_model_generator(self, generators):
-        if not self.content_indexer.token2idx:
-            self.content_indexer.build_vocab_generator(generators)
-        self.label_indexer.build_vocab_generator(generators)
-        self.embedding.setup_text_processor(self.content_indexer)
+    def build_model_generator(self,
+                              generators: List[CorpusGenerator]) -> None:
+        if not self.text_processor.token2idx:
+            self.text_processor.build_vocab_generator(generators)
+        self.label_processor.build_vocab_generator(generators)
+        self.embedding.setup_text_processor(self.text_processor)
 
         if self.sequence_length is None:
             self.sequence_length = self.embedding.get_seq_length_from_corpus(generators)
 
         if self.tf_model is None:
             self.build_model_arc()
             self.compile_model()
@@ -81,76 +100,201 @@
                       loss: Any = None,
                       optimizer: Any = None,
                       metrics: Any = None,
                       **kwargs: Any) -> None:
         """
         Configures the model for training.
         call :meth:`tf.keras.Model.predict` to compile model with custom loss, optimizer and metrics
+
+        Examples:
+
+            >>> model = BiLSTM_Model()
+            # Build model with corpus
+            >>> model.build_model(train_x, train_y)
+            # Compile model with custom loss, optimizer and metrics
+            >>> model.compile(loss='categorical_crossentropy', optimizer='rsm', metrics = ['accuracy'])
+
+        Args:
+            loss: name of objective function, objective function or ``tf.keras.losses.Loss`` instance.
+            optimizer: name of optimizer or optimizer instance.
+            metrics (object): List of metrics to be evaluated by the model during training and testing.
+            kwargs: additional params passed to :meth:`tf.keras.Model.predict``.
         """
         if loss is None:
             loss = 'sparse_categorical_crossentropy'
         if optimizer is None:
             optimizer = 'adam'
         if metrics is None:
             metrics = ['accuracy']
 
         self.tf_model.compile(loss=loss,
                               optimizer=optimizer,
                               metrics=metrics,
                               **kwargs)
 
+    def fit(self,
+            x_train: TextSamplesVar,
+            y_train: TextSamplesVar,
+            x_validate: TextSamplesVar = None,
+            y_validate: TextSamplesVar = None,
+            batch_size: int = 64,
+            epochs: int = 5,
+            callbacks: List[tf.keras.callbacks.Callback] = None,
+            fit_kwargs: Dict = None) -> 'tf.keras.callbacks.History':
+        """
+        Trains the model for a given number of epochs with given data set list.
+
+        Args:
+            x_train: Array of train feature data (if the model has a single input),
+                or tuple of train feature data array (if the model has multiple inputs)
+            y_train: Array of train label data
+            x_validate: Array of validation feature data (if the model has a single input),
+                or tuple of validation feature data array (if the model has multiple inputs)
+            y_validate: Array of validation label data
+            batch_size: Number of samples per gradient update, default to 64.
+            epochs: Number of epochs to train the model.
+                An epoch is an iteration over the entire `x` and `y` data provided.
+            callbacks: List of `tf.keras.callbacks.Callback` instances.
+                List of callbacks to apply during training.
+                See :py:class:`tf.keras.callbacks`.
+            fit_kwargs: fit_kwargs: additional arguments passed to :meth:`tf.keras.Model.fit`
+
+        Returns:
+            A :py:class:`tf.keras.callback.History`  object. Its `History.history` attribute is
+            a record of training loss values and metrics values
+            at successive epochs, as well as validation loss values
+            and validation metrics values (if applicable).
+        """
+        train_gen = CorpusGenerator(x_train, y_train)
+        if x_validate is not None:
+            valid_gen = CorpusGenerator(x_validate, y_validate)
+        else:
+            valid_gen = None
+        return self.fit_generator(train_sample_gen=train_gen,
+                                  valid_sample_gen=valid_gen,
+                                  batch_size=batch_size,
+                                  epochs=epochs,
+                                  callbacks=callbacks,
+                                  fit_kwargs=fit_kwargs)
+
+    def fit_generator(self,
+                      train_sample_gen: CorpusGenerator,
+                      valid_sample_gen: CorpusGenerator = None,
+                      batch_size: int = 64,
+                      epochs: int = 5,
+                      callbacks: List['tf.keras.callbacks.Callback'] = None,
+                      fit_kwargs: Dict = None) -> 'tf.keras.callbacks.History':
+        """
+        Trains the model for a given number of epochs with given data generator.
+
+        Data generator must be the subclass of `CorpusGenerator`
+
+        Args:
+            train_sample_gen: train data generator.
+            valid_sample_gen: valid data generator.
+            batch_size: Number of samples per gradient update, default to 64.
+            epochs: Number of epochs to train the model.
+                An epoch is an iteration over the entire `x` and `y` data provided.
+            callbacks: List of `tf.keras.callbacks.Callback` instances.
+                List of callbacks to apply during training.
+                See `tf.keras.callbacks`.
+            fit_kwargs: fit_kwargs: additional arguments passed to :meth:`tf.keras.Model.fit`
+
+        Returns:
+            A :py:class:`tf.keras.callback.History`  object. Its `History.history` attribute is
+            a record of training loss values and metrics values
+            at successive epochs, as well as validation loss values
+            and validation metrics values (if applicable).
+        """
+        self.build_model_generator([g for g in [train_sample_gen, valid_sample_gen] if g])
+
+        train_set = BatchDataSet(train_sample_gen,
+                                 text_processor=self.text_processor,
+                                 label_processor=self.label_processor,
+                                 segment=self.embedding.segment,
+                                 seq_length=self.sequence_length,
+                                 max_position=self.embedding.max_position,
+                                 batch_size=batch_size)
+
+        if fit_kwargs is None:
+            fit_kwargs = {}
+        if valid_sample_gen:
+            valid_set = BatchDataSet(valid_sample_gen,
+                                     text_processor=self.text_processor,
+                                     label_processor=self.label_processor,
+                                     segment=self.embedding.segment,
+                                     seq_length=self.sequence_length,
+                                     max_position=self.embedding.max_position,
+                                     batch_size=batch_size)
+            fit_kwargs['validation_data'] = valid_set.take()
+            fit_kwargs['validation_steps'] = len(valid_set)
+
+        for x, y in train_set.take(1):
+            logger.debug('fit input shape: {}'.format(np.array(x).shape))
+            logger.debug('fit input shape: {}'.format(np.array(y).shape))
+        return self.tf_model.fit(train_set.take(),
+                                 steps_per_epoch=len(train_set),
+                                 epochs=epochs,
+                                 callbacks=callbacks,
+                                 **fit_kwargs)
+
     def predict(self,
-                x_data,
+                x_data: TextSamplesVar,
                 *,
                 batch_size: int = 32,
                 truncating: bool = False,
-                predict_kwargs: Dict = None):
+                predict_kwargs: Dict = None) -> List[List[str]]:
         """
         Generates output predictions for the input samples.
 
         Computation is done in batches.
 
         Args:
-            x_data: The input texts, as a Numpy array (or list of Numpy arrays if the model has multiple inputs).
+            x_data: The input data, as a Numpy array (or list of Numpy arrays if the model has multiple inputs).
             batch_size: Integer. If unspecified, it will default to 32.
             truncating: remove values from sequences larger than `model.embedding.sequence_length`
             predict_kwargs: arguments passed to :meth:`tf.keras.Model.predict`
 
         Returns:
             array(s) of predictions.
         """
         if predict_kwargs is None:
             predict_kwargs = {}
-        with kolibri.backend.tensorflow.custom_object_scope():
+        with kolibri.backend.tensorflow.utils.custom_object_scope():
             if truncating:
                 seq_length = self.sequence_length
             else:
                 seq_length = None
-            tensor = self.content_indexer.transform(x_data)
+
+            tensor = self.text_processor.transform(x_data,
+                                                   segment=self.embedding.segment,
+                                                   seq_length=seq_length,
+                                                   max_position=self.embedding.max_position)
             logger.debug('predict seq_length: {}, input: {}'.format(seq_length, np.array(tensor).shape))
-            pred = self.tf_model.predict(tensor, batch_size=batch_size, **predict_kwargs)
+            pred = self.tf_model.predict(tensor, batch_size=batch_size, verbose=1, **predict_kwargs)
             pred = pred.argmax(-1)
+
             lengths = [len(sen) for sen in x_data]
 
-            res = self.label_indexer.inverse_transform(pred,  # type: ignore
-                                                       lengths=lengths)
+            res: List[List[str]] = self.label_processor.inverse_transform(pred,  # type: ignore
+                                                                          lengths=lengths)
             logger.debug('predict output: {}'.format(np.array(pred).shape))
-            logger.debug('predict output argmax: {}'.format(pred.argmax(-1)))
+            logger.debug('predict output argmax: {}'.format(pred))
         return res
 
     def predict_entities(self,
-                         x_data,
+                         x_data: TextSamplesVar,
                          batch_size: int = 32,
                          join_chunk: str = ' ',
                          truncating: bool = False,
-                         predict_kwargs: Dict = None):
+                         predict_kwargs: Dict = None) -> List[Dict]:
         """Gets entities from sequence.
 
         Args:
-            x_data: The input texts, as a Numpy array (or list of Numpy arrays if the model has multiple inputs).
+            x_data: The input data, as a Numpy array (or list of Numpy arrays if the model has multiple inputs).
             batch_size: Integer. If unspecified, it will default to 32.
             truncating: remove values from sequences larger than `model.embedding.sequence_length`
             join_chunk: str or False,
             predict_kwargs: arguments passed to :meth:`tf.keras.Model.predict`
 
         Returns:
             list: list of entity.
@@ -164,74 +308,106 @@
                            truncating=truncating,
                            predict_kwargs=predict_kwargs)
         new_res = [get_entities(seq) for seq in res]
         final_res = []
         for index, seq in enumerate(new_res):
             seq_data = []
             for entity in seq:
-                res_entities = []
+                res_entities: List[str] = []
                 for i, e in enumerate(text_seq[index][entity[1]:entity[2] + 1]):
                     # Handle bert tokenizer
                     if e.startswith('##') and len(res_entities) > 0:
                         res_entities[-1] += e.replace('##', '')
                     else:
                         res_entities.append(e)
-                value = None
+                value: Union[str, List[str]]
                 if join_chunk is False:
                     value = res_entities
                 else:
                     value = join_chunk.join(res_entities)
 
                 seq_data.append({
                     "entity": entity[0],
                     "start": entity[1],
                     "end": entity[2],
                     "value": value,
                 })
 
             final_res.append({
                 'tokenized': x_data[index],
-                'y_values': seq_data
+                'labels': seq_data
             })
         return final_res
 
     def evaluate(self,
-                 x_data, y_data,
+                 x_data: TextSamplesVar,
+                 y_data: TextSamplesVar,
                  batch_size: int = 32,
                  digits: int = 4,
                  truncating: bool = False) -> Dict:
         """
         Build a text report showing the main labeling metrics.
+
+        Args:
+            x_data:
+            y_data:
+            batch_size:
+            digits:
+            truncating:
+
+        Returns:
+            A report dict
+
+        Example:
+
+            >>> from kolibri.backend.tensorflow.tasks.labeling import BiGRU_Model
+            >>> model = BiGRU_Model()
+            >>> model.fit(train_x, train_y, valid_x, valid_y)
+            >>> report = model.evaluate(test_x, test_y)
+                       precision    recall  f1-score   support
+                <BLANKLINE>
+                      ORG     0.0665    0.1108    0.0831       984
+                      LOC     0.1870    0.2086    0.1972      1951
+                      PER     0.1685    0.0882    0.1158       884
+                <BLANKLINE>
+                micro avg     0.1384    0.1555    0.1465      3819
+                macro avg     0.1516    0.1555    0.1490      3819
+                <BLANKLINE>
+            >>> print(report)
+                {
+                 'f1-score': 0.14895159934887792,
+                 'precision': 0.1516294012813676,
+                 'recall': 0.15553809897879026,
+                 'support': 3819,
+                 'detail': {'LOC': {'f1-score': 0.19718992248062014,
+                                    'precision': 0.18695452457510336,
+                                    'recall': 0.20861096873398258,
+                                    'support': 1951},
+                            'ORG': {'f1-score': 0.08307926829268293,
+                                    'precision': 0.06646341463414634,
+                                    'recall': 0.11077235772357724,
+                                    'support': 984},
+                            'PER': {'f1-score': 0.11581291759465479,
+                                    'precision': 0.16846652267818574,
+                                    'recall': 0.08823529411764706,
+                                    'support': 884}},
+                }
+
         """
         y_pred = self.predict(x_data,
                               batch_size=batch_size,
                               truncating=truncating)
         y_true = [seq[:len(y_pred[index])] for index, seq in enumerate(y_data)]
 
         new_y_pred = []
         for x in y_pred:
             new_y_pred.append([str(i) for i in x])
         new_y_true = []
         for x in y_true:
             new_y_true.append([str(i) for i in x])
 
-        report = labeling_report(y_true, y_pred, digits=digits)
+        report = sequence_labeling_report(y_true, y_pred, digits=digits)
         return report
 
 
 if __name__ == "__main__":
-    logging.basicConfig(level=logging.DEBUG)
-    from kolibri.data.text.corpus import CONLL2003ENCorpus
-
-    corpus = CONLL2003ENCorpus('train')
-    train_x, train_y = corpus.get_data()
-    valid_x, valid_y = CONLL2003ENCorpus('valid')
-
-    train_x, train_y = train_x[:5120], train_y[:5120]
-
-    model = None
-    model.build_model(train_x[:100], train_y[:100])
-
-    model.fit(train_x[:1000], train_y[:1000], epochs=10)
-
-    model.evaluate(train_x[:20], train_y[:20])
-    print("Hello world")
+    pass
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## kolibri/backend/tensorflow/tasks/text/seq2seq/__init__.py

```diff
@@ -1,4 +1,7 @@
+# encoding: utf-8
+
+
 from .model import Seq2Seq
 
 if __name__ == "__main__":
     pass
```

## kolibri/backend/tensorflow/tasks/text/seq2seq/model.py

```diff
@@ -1,59 +1,60 @@
+# encoding: utf-8
+
 import json
 import os
 import pathlib
-from typing import Any, Dict
+from typing import Any, Tuple, List, Dict
 
 import numpy as np
 import tensorflow as tf
 import tqdm
 
 import kolibri
-from kolibri.data.text.generators import DataGenerator, Seq2SeqDataSet
-from kolibri.backend.tensorflow.autoencoder.decoders.att_gru_decoder import AttGRUDecoder
-from kolibri.backend.tensorflow.autoencoder.encoders.gru_encoder import GRUEncoder
 from kolibri.backend.tensorflow.embeddings import DefaultEmbedding
-from kolibri.backend.tensorflow.embeddings import Embedding
+from kolibri.backend.tensorflow.embeddings.base_embedding import BaseEmbedding
+from kolibri.data.text.generators import CorpusGenerator, Seq2SeqDataSet
+from kolibri.backend.tensorflow.logger import logger
 from kolibri.indexers import SequenceIndexer
-from kolibri.logger import get_logger
-
-logger = get_logger(__name__)
+from kolibri.backend.tensorflow.autoencoder.decoders import AttGRUDecoder
+from kolibri.backend.tensorflow.autoencoder.encoders import GRUEncoder
+from kolibri.types import TextSamplesVar
 
 
 class Seq2Seq:
     def to_dict(self) -> Dict[str, Any]:
         return {
             'tf_version': tf.__version__,  # type: ignore
-            'kolibri_version': kolibri.__version__,
+            'kolibri_version': kolibri.backend.tensorflow.__version__,
             '__class_name__': self.__class__.__name__,
             '__module__': self.__class__.__module__,
             'config': {
                 'encoder_seq_length': self.encoder_seq_length,  # type: ignore
                 'decoder_seq_length': self.decoder_seq_length,  # type: ignore
                 'hidden_size': self.hidden_size
             },
             'encoder_embedding': self.encoder_embedding.to_dict(),  # type: ignore
             'decoder_embedding': self.decoder_embedding.to_dict(),
             'encoder_processor': self.encoder_processor.to_dict(),
             'decoder_processor': self.decoder_processor.to_dict(),
         }
 
     def __init__(self,
-                 encoder_embedding: Embedding = None,
-                 decoder_embedding: Embedding = None,
+                 encoder_embedding: BaseEmbedding = None,
+                 decoder_embedding: BaseEmbedding = None,
                  encoder_seq_length: int = None,
                  decoder_seq_length: int = None,
                  hidden_size: int = 1024,
                  **kwargs: Any):
         """
         Init Labeling Model
 
         Args:
             embedding: embedding object
-            sequence_length: target sequence length_train
+            sequence_length: target sequence length
             hyper_parameters: hyper_parameters to overwrite
             **kwargs:
         """
         logger.warning("Seq2Seq API is experimental. It may be changed in the future without notice.")
         if encoder_embedding is None:
             encoder_embedding = DefaultEmbedding(embedding_size=256)  # type: ignore
 
@@ -75,75 +76,70 @@
         self.encoder_seq_length = encoder_seq_length
         self.decoder_seq_length = decoder_seq_length
 
         self.optimizer = tf.keras.optimizers.Adam()
         self.loss_object = tf.keras.losses.SparseCategoricalCrossentropy(from_logits=True, reduction='none')
 
     # @tf.function
-    # def loss_function(self, real: tf.Tensor, pred: tf.Tensor) -> tf.Tensor:
-    #     mask = tf.math.logical_not(tf.math.equal(real, 0))
-    #     loss_ = self.loss_object(real, pred)
-    #
-    #     mask = tf.cast(mask, dtype=loss_.dtype)
-    #     loss_ *= mask
-    #
-    #     return tf.reduce_mean(loss_)
+    def loss_function(self, real: tf.Tensor, pred: tf.Tensor) -> tf.Tensor:
+        mask = tf.math.logical_not(tf.math.equal(real, 0))
+        loss_ = self.loss_object(real, pred)
 
-    def loss_function2(self, target, pred):
-        """
-        Returns the total loss over all batch, using categorical crossentropy
-        """
-        return tf.math.reduce_sum(tf.keras.losses.sparse_categorical_crossentropy(target, pred))
+        mask = tf.cast(mask, dtype=loss_.dtype)
+        loss_ *= mask
+
+        return tf.reduce_mean(loss_)
 
     def build_model(self,
-                    x_train, y_train):
-        train_gen = DataGenerator(x_train, y_train)
+                    x_train: TextSamplesVar,
+                    y_train: TextSamplesVar) -> None:
+        train_gen = CorpusGenerator(x_train, y_train)
         self.build_model_generator(train_gen)
 
     def _build_encoder_decoder(self) -> None:
         self.encoder = GRUEncoder(self.encoder_embedding, hidden_size=self.hidden_size)
         self.decoder = AttGRUDecoder(self.decoder_embedding,
                                      hidden_size=self.hidden_size,
                                      vocab_size=self.decoder_processor.vocab_size)
         try:
             self.encoder.model().summary()
             self.decoder.model().summary()
         except:
             pass
 
     def build_model_generator(self,
-                              train_gen) -> None:
+                              train_gen: CorpusGenerator) -> None:
         """
         Build model with a generator, This function will do:
 
         1. setup processor's vocab if the vocab is empty.
-        2. calculate the sequence length_train if `sequence_length` is None.
+        2. calculate the sequence length if `sequence_length` is None.
         3. build up model architect.
         4. compile the ``tf_model`` with default loss, optimizer and metrics.
 
         Args:
-            train_gen: train texts generator
+            train_gen: train data generator
 
         """
         if self.encoder is None:
             self.encoder_processor.build_vocab_generator([train_gen])
             self.decoder_processor.build_vocab_generator([train_gen])
             self.encoder_embedding.setup_text_processor(self.encoder_processor)
             self.decoder_embedding.setup_text_processor(self.decoder_processor)
 
             if self.encoder_seq_length is None:
                 self.encoder_seq_length = self.encoder_embedding.get_seq_length_from_corpus([train_gen],
                                                                                             cover_rate=1.0)
-                logger.info(f"calculated encoder sequence length_train: {self.encoder_seq_length}")
+                logger.info(f"calculated encoder sequence length: {self.encoder_seq_length}")
 
             if self.decoder_seq_length is None:
                 self.decoder_seq_length = self.decoder_embedding.get_seq_length_from_corpus([train_gen],
                                                                                             use_label=True,
                                                                                             cover_rate=1.0)
-                logger.info(f"calculated decoder sequence length_train: {self.decoder_seq_length}")
+                logger.info(f"calculated decoder sequence length: {self.decoder_seq_length}")
 
             self._build_encoder_decoder()
 
     # @tf.function
     def train_step(self,  # type: ignore
                    input_seq,
                    target_seq,
@@ -156,34 +152,35 @@
             dec_hidden = enc_hidden
 
             bos_token_id = self.encoder_processor.token2idx[self.encoder_processor.token_bos]
             dec_input = tf.expand_dims([bos_token_id] * target_seq.shape[0], 1)
 
             # Teacher forcing - feeding the target as the next input
             for t in range(1, target_seq.shape[1]):
-                # pass enc_output to the decoder
+                # pass enc_output to the decoders
                 predictions, dec_hidden, _ = self.decoder(dec_input, dec_hidden, enc_output)
-                loss += self.loss_function2(target_seq[:, t], predictions)
+                loss += self.loss_function(target_seq[:, t], predictions)
                 # using teacher forcing
                 dec_input = tf.expand_dims(target_seq[:, t], 1)
 
         batch_loss = (loss / int(target_seq.shape[1]))
         variables = self.encoder.trainable_variables + self.decoder.trainable_variables
         gradients = tape.gradient(loss, variables)
         self.optimizer.apply_gradients(zip(gradients, variables))
 
         return batch_loss
 
     def fit(self,
-            x_train, y_train,
+            x_train: TextSamplesVar,
+            y_train: TextSamplesVar,
             *,
             batch_size: int = 64,
             epochs: int = 5,
-            callbacks=None):
-        train_gen = DataGenerator(x_train, y_train)
+            callbacks: List[tf.keras.callbacks.Callback] = None) -> tf.keras.callbacks.History:
+        train_gen = CorpusGenerator(x_train, y_train)
         self.build_model_generator(train_gen)
 
         train_dataset = Seq2SeqDataSet(train_gen,
                                        batch_size=batch_size,
                                        encoder_processor=self.encoder_processor,
                                        encoder_seq_length=self.encoder_seq_length,
                                        decoder_processor=self.decoder_processor,
@@ -201,15 +198,15 @@
         for epoch in range(epochs):
             for c in callbacks:
                 c.on_epoch_begin(epoch=epoch)
             enc_hidden = tf.zeros((batch_size, self.hidden_size))
             total_loss = []
 
             with tqdm.tqdm(total=len(train_dataset)) as p_bar:
-                for (inputs, targets) in train_dataset:
+                for (inputs, targets) in train_dataset.take():
                     p_bar.update(1)
                     batch_loss = self.train_step(inputs, targets, enc_hidden)
                     total_loss.append(batch_loss.numpy())
                     info = f"Epoch {epoch + 1}/{epochs} | Epoch Loss: {np.mean(total_loss):.4f} " \
                            f"Batch Loss: {batch_loss.numpy():.4f}"
                     p_bar.set_description_str(info)
             logs = {'loss': np.mean(total_loss)}
@@ -251,31 +248,43 @@
         model.encoder_embedding = load_data_object(model_config['encoder_embedding'])
         model.decoder_embedding = load_data_object(model_config['decoder_embedding'])
 
         model._build_encoder_decoder()
         # Load Model Weights
         model.encoder_embedding.embed_model.load_weights(os.path.join(model_path, 'encoder_embed_weights.h5'))
         model.decoder_embedding.embed_model.load_weights(os.path.join(model_path, 'decoder_embed_weights.h5'))
-        model.encoder.built = True
+
+        # ------ Fix Start -------
+        # load model issue on TF 2.3
+        # Unable to load weights saved in HDF5 format into a subclassed Model which has not created its variables yet.
+        # Call the Model first, then load the weights.
+        input_seq = model.encoder_processor.transform([['hello']],
+                                                      seq_length=model.encoder_seq_length)
+        dec_input = tf.expand_dims([3], 0)
+        enc_hidden = tf.zeros((1, model.hidden_size))
+        dec_hidden = enc_hidden
+        enc_output, enc_hidden = model.encoder(input_seq, enc_hidden)
+        _ = model.decoder(dec_input, dec_hidden, enc_output)
+        # ------ Fix End -------
+
         model.encoder.load_weights(os.path.join(model_path, 'encoder_weights.h5'))
-        model.decoder.built=True
         model.decoder.load_weights(os.path.join(model_path, 'decoder_weights.h5'))
 
         return model
 
-    def predict(self, x_data):
+    def predict(self,
+                x_data: TextSamplesVar) -> Tuple[List, np.ndarray]:
         results = []
         attentions = []
 
         bos_token_id = self.decoder_processor.token2idx[self.decoder_processor.token_bos]
-
         eos_token_id = self.decoder_processor.token2idx[self.decoder_processor.token_eos]
 
         for sample in x_data:
-            input_seq = self.encoder_processor.transform([sample])
+            input_seq = self.encoder_processor.transform([sample], seq_length=self.encoder_seq_length)
             enc_hidden = tf.zeros((1, self.hidden_size))
             enc_output, enc_hidden = self.encoder(input_seq, enc_hidden)
             dec_hidden = enc_hidden
 
             attention_plot = np.zeros((self.decoder_seq_length, self.encoder_seq_length))
             token_out = []
 
@@ -295,42 +304,24 @@
             r = self.decoder_processor.inverse_transform([token_out])[0]
             results.append(r)
             attentions.append(attention_plot)
         return results, np.array(attentions)
 
 
 if __name__ == "__main__":
-    from kolibri.datasets.reader.snips import SnipsIntentCorpus
+    from kolibri.data.text.corpus import ChineseDailyNerCorpus
     import logging
 
     logging.basicConfig(level='INFO', format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
-    import json
-    import pandas as pd
-
 
-    # Setup data path
-    DATA_PATH = '/Users/mohamedmentis/Dropbox/Mac (2)/Documents/Mentis/Development/Python/kolibri-ml/examples/conversations.json'
+    x, y = ChineseDailyNerCorpus.load_data('test')
+    x, y = x[:100], y[:100]
 
-    data = json.load(open(DATA_PATH, "r"))
-    processed_data = []
-    for d in data:
-        processed_data.append([list(d[0].values())[0].split(' '), list(d[1].values())[0].split(' ')])
-
-    df = pd.DataFrame(processed_data)
-    x=df[0].values.tolist()
-    y=df[1].values.tolist()
     seq2seq = Seq2Seq(hidden_size=256)
     seq2seq.build_model(x, y)
-    seq2seq.fit(x[:100], y[:100])
-
-
-    model_path=seq2seq.save('./seq2seq_model')
-
-    s = Seq2Seq.load_model(model_path)
-    y_pred, att = seq2seq.predict(x[:50])
-
-    from seqeval.metrics import accuracy_score
-    from seqeval.metrics import classification_report
-    from seqeval.metrics import f1_score
-    y_true =y[:50]
-    classification_report(y_true, y_pred)
+#    seq2seq.save('./seq2seq_model')
 
+#    s = Seq2Seq.load_model('./seq2seq_model')
+    res, att = seq2seq.predict(x[:10])
+#    res2, att2 = s.predict(x[:10])
+    print(res)
+    print(y[:10])
```

## kolibri/core/component.py

```diff
@@ -9,49 +9,45 @@
 import regex as re
 
 
 try:
     from kolibri.optimizers.optuna.tuner import OptunaTuner
 except:
     pass
-
+from abc import ABC
 from kolibri.errors import *
 from kdmt.dict import update
 import joblib
 from kolibri.utils.config import get_parameter
 from kdmt.dict import nested_dict_set_key_value, nested_dict_get_key_path
+from kdmt.path import expand_path
 from kolibri.config import ModelConfig
 
 logger = get_logger(__name__)
 from pathlib import Path
 
-def register(new_class):
-    from kolibri.registry import ModulesRegistry
-    ModulesRegistry.add_module(new_class.name, new_class)
-
-
-class ComponentMetaclass(type):
-    """Metaclass with `name` class property"""
-
-    @property
-    def name(cls):
-        """The name property is a function of the class - its __name__."""
+# def register(new_class):
+#     from kolibri.registry import ModulesRegistry
+#     ModulesRegistry.add_module(new_class.name, new_class)
+
+# class ComponentMetaclass(type):
+#     """Metaclass with `name` class property"""
+#
+#     @property
+#     def name(cls):
+#         """The name property is a function of the class - its __name__."""
+#
+#         return cls.__name__
+#
+#     def __new__(cls, clsname, bases, attrs):
+#         newclass = super(ComponentMetaclass, cls).__new__(cls, clsname, bases, attrs)
+#         register(newclass)  # here is your register function
+#         return newclass
 
-        return cls.__name__
-
-    def __new__(cls, clsname, bases, attrs):
-        newclass = super(ComponentMetaclass, cls).__new__(cls, clsname, bases, attrs)
-        register(newclass)  # here is your register function
-        return newclass
-
-def expand_path(path):
-    """Convert relative paths to absolute with resolving user directory."""
-    return Path(path).expanduser().resolve()
-
-class Component(metaclass=ComponentMetaclass):
+class Component(ABC):
     """A component is a document processing unit in a pipeline.
     Components are the base class for most of kolibri classes. it define some of the basic functionalities and properties.
     In Kolibri all components are responsible for updating thier parameters.
     Component define basic functionalities for loading and saving and creating components.
     It also create the necessary interfaces that need to be implemented by children: fit and transform
     Components are collected sequentially in a pipeline. Each component
     is called one after another. This holds for
@@ -60,15 +56,15 @@
     methods will be called first.
 """
 
     @property
     def name(self):
         """Access the class's property name from an instance."""
 
-        return type(self).name
+        return self.__class__.__name__
 
     component_type = ""
     # Name of the component to be used when integrating it in a
     # pipeline. E.g. ``[ComponentA, ComponentB]``
     # will be a proper pipeline definition where ``ComponentA``
     # is the name of the first component of the pipeline.
     component_name = ""
@@ -118,15 +114,16 @@
             "random-state": 41,
             "output-folder": None,
             "n_jobs": 1,
             "save-base-model": False,
             "target": None,
             "load-path":None,
             "save-patg": None,
-            "verbose": False
+            "verbose": False,
+            "required-libs":{}
         },
 
         "tunable": {
             # "example": {
             #     "description": "This is just an example of a tuneable variable",
             #     "value": 1,
             #     "type": "int",
@@ -138,28 +135,30 @@
 
     def __init__(self, parameters=None):
 
         self.update_default_hyper_parameters()
         self.hyperparameters = {}
         self.hyperparameters = deepcopy(self.defaults)
         self.override_default_parameters(parameters)
+
         self.model = self
         # add component name to the config
         self.hyperparameters["fixed"]["name"] = self.name
 
         self.language = self.get_parameter("language")
         self.target = self.get_parameter("target")
         self._tunable = self._get_tunable(self.hyperparameters)
 
         if self.get_parameter("save-path"):
-            self.save_path = expand_path(save_path)
+            self.save_path = expand_path(self.get_parameter("save-path"))
             self.save_path.parent.mkdir(parents=True, exist_ok=True)
         else:
             self.save_path = None
 
+
         # if self.get_parameter("load-path") is not None:
         #     self.load_path = expand_path(self.get_parameter("load-path"))
         #     if mode != 'train' and self.save_path and self.load_path != self.save_path:
         #         log.warning("Load path '{}' differs from save path '{}' in '{}' mode for {}."
         #                     .format(self.load_path, self.save_path, mode, self.__class__.__name__))
         # elif mode != 'train' and self.save_path:
         #     self.load_path = self.save_path
@@ -306,20 +305,37 @@
     def persist(self, model_dir):
         """Persist this model_type into the passed directory.
         Returns the metadata necessary to load the model_type again."""
 
         model_file = os.path.join(model_dir, self.name + ".pkl")
         joblib.dump(self, model_file)
 
-        return {"model_file": self.name + ".pkl", 'folder': model_dir}
+        return {"model_file": self.name + ".pkl", 'folder': None}
+
+    @classmethod
+    def get_subclasses(cls, include_parents=False):
+        """Recursively find subclasses of this Baseline.
+
+        Args:
+            include_parents (bool):
+                Whether to include subclasses which are parents to
+                other classes. Defaults to ``False``.
+        """
+        subclasses = {}
+        for child in cls.__subclasses__():
+            grandchildren = child.get_subclasses(include_parents)
+            subclasses.update(grandchildren)
+            if include_parents or not grandchildren:
+                subclasses[child.__name__] = child
 
+        return subclasses
 
     @classmethod
     def load_from_azure(cls, container_name=None):
-        from kdmt.azure import get_file_object
+        from kdmt.cloud.azure import get_file_object
         connect_str=os.environ.get("STORAGE_CONTAINER_STRING")
 
         blob_model_file=cls.__name__+'.model.pkl'
 
         model_file=get_file_object(connect_str, container_name, blob_model_file)
 
         model = joblib.load(model_file)
@@ -327,27 +343,31 @@
         return model
 
     def _default_ouptut_file_name(self):
         file_name=self.__class__.__name__+'.model.pkl'
 
         return re.sub('[^A-Za-z0-9-\.]+', '', file_name)
 
+    def __repr__(self):
+
+        return self.__class__.__name__
+
     def save_to_azure(self, container_name):
         """
         Save model
         Args:
             model_path:
         """
 
         connect_str=os.environ.get("STORAGE_CONTAINER_STRING")
-        from kdmt.azure import  upload_file
+        from kdmt.cloud.azure import  upload_file
         import tempfile
         td=tempfile.TemporaryDirectory()
         model_dir=td.name
-        local_model_file = os.path.join(model_dir, self._default_ouptut_file_name())
+        local_model_file = tempfile.NamedTemporaryFile(dir=model_dir, delete=True).name
         joblib.dump(self, local_model_file)
         blob_model_file=self._default_ouptut_file_name()
         upload_file(connect_str, container_name, local_model_file, blob_model_file, overwrite=True)
 
         return container_name
 
 
@@ -378,14 +398,16 @@
         Otherwise, an instantiation of the
         component will be reused for all models where the
         metadata creates the same key."""
 
         return None
 
     def __eq__(self, other):
+        if isinstance(other, str):
+            return self.__repr__()==other
         return self.__dict__ == other.__dict__
 
     @classmethod
     def _get_tunable(cls, hyperparameters):
         tunable = dict()
         for name, param in hyperparameters.get('tunable', dict()).items():
             tunable[name] = param
```

## kolibri/core/modules.py

```diff
@@ -1,13 +1,12 @@
 from typing import Any
 from typing import Optional
 from typing import Text
-from typing import Type
-
-from kolibri.registry import ModulesRegistry
+from kolibri.registry import get_model, list_models
+#from kolibri.registry import ModulesRegistry
 
 def find_unavailable_packages(package_names):
     """Tries to import all the package names and returns
     the packages where it failed."""
     import importlib
 
     failed_imports = set()
@@ -15,25 +14,28 @@
         try:
             importlib.import_module(package)
         except ImportError:
             failed_imports.add(package)
     return failed_imports
 
 
-def validate_requirements(component_names):
+def validate_requirements(components):
     """Ensures that all required python packages are installed to
     instantiate and used the passed components."""
     from kolibri.core import modules
 
     # Validate that all required packages are installed
     failed_imports = set()
-    for component_name in component_names:
-        component_class = modules.get_component_class_from_name(component_name)
-        failed_imports.update(find_unavailable_packages(
-            component_class.required_packages()))
+    for component in components:
+        if isinstance(component, list):
+            validate_requirements(component)
+        else:
+            component_class = modules.get_component_class_from_name(component[1])
+            failed_imports.update(find_unavailable_packages(
+                component_class.required_packages()))
     if failed_imports:  # pragma: no cover
         # if available, use the development file to figure out the correct
         # version numbers for each requirement
         raise Exception("Not all required packages are installed. " +
                         "To use this pipeline, you need to install the "
                         "missing dependencies. " +
                         "Please install {}".format(", ".join(failed_imports)))
@@ -55,27 +57,27 @@
         return getattr(m, class_name)
     else:
         return globals()[module_path]
 
 
 def get_component_class_from_name(component_name):
     """Resolve component name to a registered components class."""
-    if component_name not in ModulesRegistry.registry['kolibri']:
+    if component_name not in list_models():
         try:
             return class_from_module_path(component_name)
         except Exception:
             raise Exception(
                 "Failed to find component class for '{}'. Unknown "
                 "component name. Check your configured pipeline and make "
                 "sure the mentioned component is not misspelled. If you "
                 "are creating your own component, make sure it is either "
                 "listed as part of the `component_classes` in "
                 "`kolibti.modules.py` or is a proper name of a class "
                 "in a module.".format(component_name))
-    return ModulesRegistry.registry['kolibri'][component_name]['class']
+    return get_model(component_name)
 
 def load_component_by_name(component_name, model_dir, metadata, cached_component, **kwargs):
     """Resolves a component and calls its load method to init it based on a
     previously persisted model."""
 
     component_clz = get_component_class_from_name(component_name)
     return component_clz.load(model_dir, metadata, cached_component, **kwargs)
```

## kolibri/core/pipeline.py

```diff
@@ -1,15 +1,16 @@
 import logging
 import time
 from collections import defaultdict
-
+from scipy.sparse import issparse, hstack, vstack, csr_matrix
+from abc import ABC
 import pandas
 
 from kolibri.core import modules
-from kolibri.core.component import ComponentMetaclass
+#from kolibri.core.component import ComponentMetaclass
 import numpy as np
 
 LOGGER = logging.getLogger(__name__)
 
 
 def validate_arguments(pipeline, context, allow_empty_pipeline=False):
     """Validates a pipeline before it is run. Ensures, that all
@@ -29,15 +30,15 @@
         for r in component.requires:
             if r not in provided_properties:
                 raise Exception("Failed to validate at component "
                                 "'{}'. Missing property: '{}'"
                                 "".format(component.my_name, r))
         provided_properties.update(component.provides)
 
-class Pipeline(object, metaclass=ComponentMetaclass):
+class Pipeline(ABC):
     """Pipeline Class.
 
     The **Pipeline** class represents a Machine Learning Pipeline, which
     is an ordered collection of Machine Learning tools or Primitives,
     represented by **Component instances**, that will be executed
     sequentially in order to produce results.
 
@@ -60,77 +61,64 @@
         """Get the tunable hyperperparameters from all the blocks in this pipelines."""
         tunable = {}
         for step_name, step in self.steps.items():
             tunable[step_name] = step.get_tunable_hyperparameters()
 
         return tunable
 
-    def _validate_components(self):
-        if self.steps is None:
+    def _validate_components(self, steps=None):
+        if steps is None:
+            steps = self.steps
+        if not steps:
             return
 
-        names, components = self.steps.keys(), self.steps.values()
-
-        self.transformers=[]
-        self.estimator=None
-        for component in components:
-            if component.component_type=="estimator":
-                self.estimator=component
-            else:
-                self.transformers.append(component)
-
         self.active = True
 
-        for t in self.transformers:
-            if t is None:
-                continue
-            else:
-                if not (hasattr(t, "fit") or hasattr(t, "fit_transform")) or not hasattr(t, "transform"):
+        for step in steps:
+            if isinstance(step, tuple):
+                if step[1].component_type == "estimator":
+                    if hasattr(self, 'estimator') and self.estimator is not None:
+                        raise ValueError("Only one estimator allowed")
+                    self.estimator=step[1]
+                if not (hasattr(step[1], "fit") or hasattr(step[1], "fit_transform")) or not hasattr(step[1],
+                                                                                                     "transform"):
                     self.active = False
-                    raise TypeError("All intermediate steps, including an evaluator, "
-                                    "should implement fit and transform.")
+                    raise TypeError(f"Component {step[1]} should implement fit and transform.")
+            elif isinstance(step, list):
+                # If the step is a list, recursively validate its components
+                self._validate_components(step)
 
     def __init__(self, steps=None, parameters={}):
-
-        self.steps= {}
+        self.steps = []
         if steps is not None:
             for step in steps:
-                self.steps[step[0]]=step[1]
-
+                self.steps.append(step)
 
+        self.estimator=None
         self._validate_components()
 
-
-        self.verbose =  parameters["verbose"] if "verbose" in parameters else False
+        self.verbose = parameters.get("verbose", False)
 
         super(Pipeline, self).__init__()
 
-    def add_steps(self, steps):
-        if self.steps is None:
-            self.steps={}
-        for name, component in steps:
-            if name not in self.steps:
-                self.steps[name]=component
-            else:
-                raise ValueError("duplicate Compoenent name in the pipeline")
-
-        self._validate_components()
-
     @staticmethod
     def from_configs(params):
         """Transform the passed names of the pipeline components into classes"""
 
-        steps = []
+        branches = []
         # Transform the passed names of the pipeline components into classes
-        for component_name, param_val in params.items():
-            component = modules.create_component_by_name(
-                component_name, param_val)
-            steps.append((component_name, component))
+        for branch_name, branch_params in params.items():
+            branch = []
+            for component_name, param_val in branch_params.items():
+                component = modules.create_component_by_name(
+                    component_name, param_val)
+                branch.append((component_name, component))
+            branches.append(branch)
 
-        return Pipeline(steps)
+        return Pipeline(branches)
 
     @staticmethod
     def _flatten_dict(hyperparameters):
         return {
             (block, name): value
             for block, block_hyperparameters in hyperparameters.items()
             for name, value in block_hyperparameters.items()
@@ -233,14 +221,26 @@
                 block, hyperparameter = key
                 params_tree[block][hyperparameter] = value
             else:
                 params_tree[key] = value
 
         return params_tree
 
+    def flatten_config(self, config):
+        flat_config = []
+
+        for item in config:
+            if isinstance(item, list):
+                flat_config.extend(self. flatten_config(item))
+            else:
+                flat_config.append(item)
+
+        return flat_config
+
+
     @property
     def parameters(self):
         """Get the current hyperparamters of each block.
 
         Args:
             flat (bool): If True, return a flattened dictionary where each key
                 is a two elements tuple containing the name of the block as the first
@@ -251,15 +251,15 @@
 
         Returns:
             dict:
                 A dictionary containing the block names as keys and
                 the current block configs dictionary as values.
         """
         hyperparameters = dict()
-        for block_name, block in self.steps.items():
+        for block_name, block in self.flatten_config(self.steps):
             hyperparameters[block_name] = block.get_hyperparameters()
 
         return hyperparameters
 
     def set_hyperparameters(self, hyperparameters):
         """Set new hyperparameter values for some blocks.
 
@@ -286,46 +286,82 @@
             Contains the true class y_values for all the samples in data.
         Returns
         -------
         Pipeline
             self
         """
 
-        Xt, y, Xt_val, y_val=self.fit_transformers(X, y, X_val,y_val)
+        Xt, y, Xt_val, y_val=self.fit_transformers(self.steps, X, y, X_val,y_val)
 
         return self.fit_estimator(Xt, y, Xt_val, y_val)
 
 
 
-    def fit_transformers(self, X, y, X_val=None, y_val=None):
+    def _is_transformer(self, component):
+        return (hasattr(component, 'component_type') and component.component_type == "transformer") and (hasattr(component, 'transform') or hasattr(component, 'fit_transform'))
+
+
+
+    def _is_estimator(self, component):
+        return  (hasattr(component, 'component_type') and component.component_type == "estimator") or hasattr(component, 'fit') and (hasattr(component, 'predict') or hasattr(component, 'predict_proba'))
 
-        Xt = X
-        Xt_val = X_val
 
-        for transformer in self.transformers:
-            start=time.time()
-            if transformer is None:
-                pass
-            if hasattr(transformer, "fit_transform"):
-                Xt = transformer.fit_transform(Xt, y)
-                if Xt_val is not None:
-                    Xt_val = transformer.fit_transform(Xt_val, y_val)
+    def fit_transformers(self, steps, X, y, X_val=None, y_val=None, fitted_config=[], fitted_config_transformed=[]):
+        for step in steps:
+            if isinstance(step, list):
+                # A branch is a list of stages
+                X_transformed, y, X_val_transformed, y_val = self.fit_transformers(step, X, y, X_val, y_val, fitted_config, fitted_config_transformed)
+                fitted_config.append(X_transformed)
+                if X_val_transformed is not None:
+                    fitted_config_transformed.append(X_val_transformed)
+            elif step[0] == 'join':
+                # A join operation
+                X= self.concatenate_matrices([branch_transformed for branch_transformed in fitted_config], axis=1)
+                if fitted_config_transformed:
+                    X_val = self.concatenate_matrices([branch_transformed for branch_transformed in fitted_config], axis=1)
+
+                if self._is_transformer(step[1]):
+                    X, y, X_val, y_val=self.fit_transformer(step[1], X, y, X_val, y_val)
             else:
-                Xt = transformer.fit(Xt, y).transform(Xt)
-                if Xt_val is not None:
-                    Xt_val = transformer.transform(Xt_val)
-            print('fitted component ' + transformer.name + '. Elapsed time ' + str(time.time() - start))
+                if self._is_transformer(step[1]):
+                    X, y, X_val, y_val=self.fit_transformer(step[1], X, y, X_val, y_val)
+
+        return X, y, X_val, y_val
+
+    def concatenate_matrices(self, mat_array, axis=1):
+        # Convert all matrices in array to csr format if they're not already
+        mat_array = [mat if issparse(mat) else csr_matrix(mat) for mat in mat_array]
+
+        if axis == 0:
+            return vstack(mat_array)
+        else:
+            return hstack(mat_array)
+
+    def fit_transformer(self, transformer, Xt, y, Xt_val=None, y_val=None):
+
+        start=time.time()
+        if transformer is None:
+            pass
+        if hasattr(transformer, "fit_transform"):
+            Xt = transformer.fit_transform(Xt, y)
+            if Xt_val is not None:
+                Xt_val = transformer.fit_transform(Xt_val, y_val)
+        else:
+            Xt = transformer.fit(Xt, y).transform(Xt)
+            if Xt_val is not None:
+                Xt_val = transformer.transform(Xt_val)
+        print('fitted component ' + transformer.name + '. Elapsed time ' + str(time.time() - start))
 
         return Xt, y, Xt_val, y_val
 
     def fit_estimator(self, Xt, y, Xt_val=None, y_val=None):
         if self.estimator is not None:
-            print('fitting estimator '+self.estimator.name)
+            print('fitting estimator '+ self.estimator.name)
             try:
-                return  self.estimator.fit(Xt, y, Xt_val, y_val)
+                return self.estimator.fit(Xt, y, Xt_val, y_val)
             except Exception as e:
                 return self.estimator.fit(Xt, y)
 
     def predict(self, X):
         """ predict
         Sequentially applies all transforms and then predict with last step.
         Parameters
@@ -341,22 +377,39 @@
         if isinstance(X, np.ndarray):
             X=X.tolist()
         if isinstance(X, list) or isinstance(X, pandas.DataFrame):
             Xt = X
         else:
             Xt=[X]
 
-        for transform in self.transformers:
-            if transform is not None:
-                Xt = transform.transform(Xt)
+        Xt= self._predict_transform(self.steps, Xt, [])
         if self.estimator is not None:
             return self.estimator.predict(Xt)
         else:
             return Xt
 
+
+    def _predict_transform(self, stages, X, fitted_config=[]):
+        for stage in stages:
+            if isinstance(stage, list):
+                # A branch is a list of stages
+                X_transformed = self._predict_transform(stage, X, fitted_config)
+                fitted_config.append(X_transformed)
+            elif stage[0] == 'join':
+                # A join operation
+                # A join operation
+                X= self.concatenate_matrices([branch_transformed for branch_transformed in fitted_config], axis=1)
+
+                if self._is_transformer(stage[1]):
+                    X =stage[1].transform(stage[1], X)
+            else:
+                if self._is_transformer(stage[1]):
+                    X= stage[1].transform(X)
+        return X
+
     def predict_proba(self, X):
         if isinstance(X, np.ndarray):
             X=X.tolist()
         if isinstance(X, list) or isinstance(X, pandas.DataFrame):
             Xt = X
         else:
             Xt=[X]
```

## kolibri/core/serializable.py

```diff
@@ -12,25 +12,22 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from abc import ABCMeta, abstractmethod
 from logging import getLogger
 from pathlib import Path
 from typing import Union, Optional
-
-def expand_path(path: Union[str, Path]) -> Path:
-    """Convert relative paths to absolute with resolving user directory."""
-    return Path(path).expanduser().resolve()
+from kdmt.path import expand_path
 
 log = getLogger(__name__)
 
 
 class Serializable(metaclass=ABCMeta):
     """
-    :class:`deeppavlov.models.model.serializable.Serializable` is an abstract base class that expresses the interface
+    :class:`kolibri.models.model.serializable.Serializable` is an abstract base class that expresses the interface
     for all models that can serialize data to a path.
     """
 
     def __init__(self, save_path: Optional[Union[str, Path]], load_path: Optional[Union[str, Path]] = None,
                  mode: str = 'infer',
                  *args, **kwargs) -> None:
```

## kolibri/data/text/corpus.py

```diff
@@ -1,237 +1,45 @@
 # encoding: utf-8
 
-import json
+
 import os
-from operator import itemgetter
-from pathlib import Path
+from typing import List
+from typing import Tuple
 
-import pandas as pd
-from tensorflow.keras.utils import get_file
+from kolibri.backend.tensorflow import macros as K
 
-from kolibri import default_configs as k
-from kolibri.data.text.streams import DataStream
-from kolibri.data.text.file_stream import FileStream
-from kolibri.tokenizers import WordTokenizer
-
-CORPUS_PATH = os.path.join(k.DATA_PATH, 'corpus')
-
-Path(CORPUS_PATH).mkdir(exist_ok=True, parents=True)
-
-
-class CONLL2003ENCorpus(FileStream):
-    __corpus_name__ = 'conll2003_en'
-    __zip_file__name = 'https://www.dropbox.com/s/73jma78ywqzvjyq/conll2003.tar?dl=1'
-
-    def __init__(self, subset_name: str = 'train', task_name: str = 'ner'):
-
-        corpus_path = get_file(self.__corpus_name__,
-                               self.__zip_file__name,
-                               cache_dir=CORPUS_PATH,
-                               untar=True)
-
-        if subset_name not in {'train', 'test', 'valid'}:
-            raise ValueError()
-        self.task_name = task_name
-        self.filepath = os.path.join(corpus_path, f'{subset_name}.txt')
-        self.data_index = ['pos', 'chunking', 'ner'].index(self.task_name) + 1
-        super().__init__(self.filepath, content_col=0, target_cols=self.data_index, filetype='conll')
-        if self.task_name not in {'pos', 'chunking', 'ner'}:
-            raise ValueError()
-        self.prepare()
-
-    def _load_data(self):
-        try:
-            raw_data = self.read_function(self.filepath)
-            self.n_samples = 0
-            for line in raw_data:
-                self.n_samples += 1
-                for token in line:
-                    self.target_values.append(itemgetter(*self.target_columns)(token))
-
-            self.target_values = list(self.target_values)
-
-            self.raw_data = self.read_function(self.filepath)
-
-        except FileNotFoundError:
-            raise FileNotFoundError("File {} does not exist.".format(self.filepath))
-        pass
-
-    def __iter__(self):
-
-        for token in self.raw_data:
-            yield [d[self.content_column] for d in token], [d[self.target_columns[0]] for d in token]
-
-
-class Sentiment140Corpus(FileStream):
-    """
-
-    """
-
-    __corpus_name__ = 'Sentiments140'
-    __zip_file__name = "https://www.dropbox.com/s/egk8cwupfs05g00/Sentiments140.tar.gz?dl=1"
-
-    def __init__(self, subset_name='sentiment140_sample'):
-        self.corpus_path = get_file(self.__corpus_name__,
-                                    self.__zip_file__name,
-                                    cache_dir=k.DATA_PATH,
-                                    untar=True)
-
-        if subset_name not in {'sentiment140_sample', 'all'}:
-            raise ValueError()
-
-        self.file_path = os.path.join(self.corpus_path, f'{subset_name}.csv')
-
-        super().__init__(filepath=self.file_path, content_col=' text', target_cols='label')
-        self.prepare()
-
-class CreditCardFraud(DataStream):
-    """
-
-    """
-
-    __corpus_name__ = 'creditcard_fraud'
-    __zip_file__name = "https://www.dropbox.com/s/7v4tm6lsjkxnvfk/creditcard_fraud.tgz?dl=1"
-
-    def __init__(self, subset_name='creditcard'):
-        self.corpus_path = get_file(self.__corpus_name__,
-                                    self.__zip_file__name,
-                                    cache_dir=k.DATA_PATH,
-                                    untar=True)
-
-        if subset_name not in {'creditcard'}:
-            raise ValueError()
-
-        self.file_path = os.path.join(self.corpus_path, f'{subset_name}.csv')
-        data=pd.read_csv(self.file_path)
-        columns=[ c for c in data.columns if c not in ['Class', 'Time']]
-
-        super().__init__(data=data[columns], y=data['Class'].values)
-        self.prepare()
-
-
-class ConsumerComplaintsCorpus(FileStream):
-    """
-
-    """
-
-    __corpus_name__ = 'consumer_complaints'
-    __zip_file__name = "https://www.dropbox.com/s/8a1pm3gg9e5szso/consumer_complaints.tar.gz?dl=1"
-
-    def __init__(self, subset_name='sample'):
-        self.corpus_path = get_file(self.__corpus_name__,
-                                    self.__zip_file__name,
-                                    cache_dir=k.DATA_PATH,
-                                    untar=True)
-
-        if subset_name not in {'sample', 'validate', 'train', 'test'}:
-            raise ValueError()
-
-        self.file_path = os.path.join(self.corpus_path, f'{subset_name}.csv')
-
-        super().__init__(filepath=self.file_path, content_col='Consumer_complaint', target_cols=['Product'])
-        self.prepare()
-
-
-class SnipsIntentCorpus(DataStream):
-    """
-    SNIPS dataset_train class
-
-    Args:
-            path (str): dataset_train path
-            sentence_length (int, optional): max sentence length
-            word_length (int, optional): max word length
-    """
-
-    __corpus_name__ = 'snips_intents'
-    __zip_file__name = "https://www.dropbox.com/s/somo7vz6p23e2aq/snips_intent.tgz?dl=1"
-
-    train_files = [
-        "AddToPlaylist/train_AddToPlaylist_full.json",
-        "BookRestaurant/train_BookRestaurant_full.json",
-        "GetWeather/train_GetWeather_full.json",
-        "PlayMusic/train_PlayMusic_full.json",
-        "RateBook/train_RateBook_full.json",
-        "SearchCreativeWork/train_SearchCreativeWork_full.json",
-        "SearchScreeningEvent/train_SearchScreeningEvent_full.json",
-    ]
-    test_files = [
-        "AddToPlaylist/validate_AddToPlaylist.json",
-        "BookRestaurant/validate_BookRestaurant.json",
-        "GetWeather/validate_GetWeather.json",
-        "PlayMusic/validate_PlayMusic.json",
-        "RateBook/validate_RateBook.json",
-        "SearchCreativeWork/validate_SearchCreativeWork.json",
-        "SearchScreeningEvent/validate_SearchScreeningEvent.json",
-    ]
-    files = ["train", "test"]
-
-    def __init__(self, subset_name: str = 'train', task_name: str = 'ner'):
-
-        corpus_path = get_file(self.__corpus_name__,
-                               self.__zip_file__name,
-                               cache_dir=CORPUS_PATH,
-                               untar=True)
-
-        if subset_name not in {'train', 'test'}:
-            raise ValueError()
-        self.task_name = task_name
-
-        self.dataset_root = corpus_path
-        data_set_raw = self._load_dataset(subset_name)
-        data_set_raw = pd.DataFrame(data_set_raw, columns=['Content', 'Entities', 'Intent'])
-        super().__init__(data=data_set_raw[['Content']], y=data_set_raw[['Entities', 'Intent']])
-        self.prepare()
-
-    def _load_dataset(self, dataset):
-        """returns a tuple of train/test with 3-tuple of tokens, tags, intent_type"""
-        if dataset == 'train':
-            _data = self._load_intents(self.train_files)
-        else:
-            _data = self._load_intents(self.test_files)
-
-        data = [(t, l, i) for i in sorted(_data) for t, l in _data[i]]
-
-        return data
-
-    def _load_intents(self, files):
-        data = {}
-        for f in sorted(files):
-            fname = os.path.join(self.dataset_root, f)
-            intent = f.split(os.sep)[0]
-            with open(fname, encoding="utf-8", errors="ignore") as fp:
-                fdata = json.load(fp)
-            entries = self._parse_json([d["data"] for d in fdata[intent]])
-            data[intent] = entries
-        return data
-
-    def _parse_json(self, data):
-        tokenizer = WordTokenizer()
-        sentences = []
-        for s in data:
-            tokens = []
-            tags = []
-            for t in s:
-                new_tokens = tokenizer.tokenize(t["text"].strip())
-                tokens += new_tokens
-                ent = t.get("entity", None)
-                if ent is not None:
-                    tags += self._create_tags(ent, len(new_tokens))
-                else:
-                    tags += ["O"] * len(new_tokens)
-            sentences.append((tokens, tags))
-        return sentences
+CORPUS_PATH = os.path.join(K.DATA_PATH, 'corpus')
 
-    @staticmethod
-    def _create_tags(tag, length):
-        labels = ["B-" + tag]
-        if length > 1:
-            for _ in range(length - 1):
-                labels.append("I-" + tag)
-        return labels
 
+class DataReader:
 
-if __name__ == "__main__":
-    corpus = SnipsIntentCorpus()
+    @staticmethod
+    def read_conll_format_file(file_path: str,
+                               text_index: int = 0,
+                               label_index: int = 1) -> Tuple[List[List[str]], List[List[str]]]:
+        """
+        Read conll format data_file
+        Args:
+            file_path: path of target file
+            text_index: index of text data, default 0
+            label_index: index of label data, default 1
+
+        Returns:
+
+        """
+        x_data, y_data = [], []
+        with open(file_path, 'r', encoding='utf-8') as f:
+            lines = f.read().splitlines()
+            x: List[str] = []
+            y: List[str] = []
+            for line in lines:
+                rows = line.split(' ')
+                if len(rows) == 1:
+                    x_data.append(x)
+                    y_data.append(y)
+                    x = []
+                    y = []
+                else:
+                    x.append(rows[text_index])
+                    y.append(rows[label_index])
+        return x_data, y_data
 
-    for d in corpus.X:
-        print(list(d))
```

## kolibri/data/text/generators.py

```diff
@@ -1,181 +1,141 @@
-import os
-from glob import glob
-from typing import Any
-from typing import Iterable, Iterator
+# encoding: utf-8
+
+
+
+from abc import ABC
+from typing import Iterable, Iterator, TYPE_CHECKING
+from typing import List, Any, Tuple
 
 import numpy as np
-import tensorflow as tf
-from tensorflow import keras
 
-from kolibri.indexers.multi_content_indexer import MultiContentIndexer
-from kolibri.indexers.multi_target_indexer import MultiTargetIndexer
 
 
-class DataGenerator(keras.utils.Sequence):
+class BaseGenerator(Iterable, ABC):
+    def __init__(self, buffer_size: int = 2000) -> None:
+        self.buffer_size = buffer_size
 
-    def __init__(self, x_values, y_values, content_indexer=None, label_indexer=None, x_augmentor=None, batch_size=1,
-                 shuffle=False):
-        self.y_values = y_values  # array of y_values
-        self.x_values = x_values  # array of image paths
-        self.batch_size = batch_size  # batch size
-        self.shuffle = shuffle  # shuffle bool
-        self.on_epoch_end()
-        self.content_indexer = content_indexer
-        self.label_indexer = label_indexer
-        self.augmentor = x_augmentor
-
-    def __len__(self):
-        'Denotes the number of batches per epoch'
-
-        if self.x_values is not None:
-            return max(1, int(np.ceil(len(self.x_values) / self.batch_size)))
-        else:
-            return max(1, int(np.ceil(len(self.y_values) / self.batch_size)))
-
-    def set_batch_size(self, new_batch_size):
-        self.batch_size = new_batch_size
-
-    def on_epoch_end(self):
-        'Updates indexes after each epoch'
-        if self.x_values is not None:
-            self.indexes = np.arange(len(self.x_values))
-        else:
-            self.indexes = np.arange(len(self.y_values))
-
-        if self.shuffle:
-            np.random.shuffle(self.indexes)
-
-    def __getitem__(self, index):
-        'Generate one batch of texts'
-        # selects indices of texts for next batch
-        indexes = self.indexes[index * self.batch_size: (index + 1) * self.batch_size]
-
-        # select texts and load images
-        labels = None
-        content = None
-
-        if self.y_values is not None:
-            labels = np.array([self.y_values[k] for k in indexes])
-            if self.label_indexer:
-                labels = self.label_indexer.transform(labels)
-            if self.batch_size == 1:
-                if isinstance(self.label_indexer, MultiTargetIndexer):
-                    labels = [l[0] for l in labels]
-                else:
-                    labels = labels[0]
-        if self.x_values is not None:
-            # preprocess and augment texts
-
-            content = [self.x_values[k] for k in indexes]
-            if self.augmentor:
-                content = self.augmentor(content)
-
-            if self.content_indexer:
-                content = self.content_indexer.transform(content)
-
-            if self.batch_size == 1:
-                if isinstance(self.content_indexer, MultiContentIndexer):
-                    content = [c[0] for c in content]
-                else:
-                    content = content[0]
-        #           content = np.array(content)
-        return content, labels
-
-    def get_data(self):
-        X = []
-        Y = []
-        batchsize = self.batch_size
-        self.batch_size = 1
-        if isinstance(self.content_indexer, MultiContentIndexer):
-            for i in self.content_indexer.content_indexers:
-                X.append([])
-        if isinstance(self.label_indexer, MultiTargetIndexer):
-            for i in self.label_indexer.label_indexers:
-                Y.append([])
-
-        for i in range(0, len(self.x_values)):
-            if isinstance(self.content_indexer, MultiContentIndexer):
-                for j in range(len(self.content_indexer.content_indexers)):
-                    X[j].append(self[i][0][j])
-            else:
-                X.append(self[i][0])
-            if isinstance(self.content_indexer, MultiContentIndexer):
-                for j in range(len(self.label_indexer.label_indexers)):
-                    Y[j].append(self[i][1][j])
-            else:
-                Y.append(self[i][1])
-
-        self.batch_size = batchsize
-
-        if isinstance(self.content_indexer, MultiContentIndexer):
-            for i in range(len(self.content_indexer.content_indexers)):
-                X[i] = np.array(X[i])
-        else:
-            X = np.array(X)
-        if isinstance(self.label_indexer, MultiTargetIndexer):
-            for i in range(len(self.label_indexer.label_indexers)):
-                Y[i] = np.array(Y[i])
-        else:
-            Y = np.array(Y)
-
-        return X, Y
-
-
-class FolderDataGenerator(DataGenerator):
-
-    def __init__(self, folder_path, content_indexer=None, label_indexer=None, x_augmentor=None,
-                 batch_size=1, shuffle=False):
-        if not os.path.exists(folder_path):
-            raise Exception('(' + folder_path + ') Folder not found')
-        file_paths = glob('{}/**'.format(folder_path), recursive=True)
-        file_paths = [x.replace(os.sep, '/') for x in file_paths if os.path.isfile(x)]
-        labels = [os.path.basename(os.path.dirname(x)) for x in file_paths]
+    def __iter__(self) -> Iterator[Tuple[Any, Any]]:
+        raise NotImplementedError
 
-        super().__init__(x_values=file_paths, y_values=labels, content_indexer=content_indexer,
-                         label_indexer=label_indexer, x_augmentor=x_augmentor, batch_size=batch_size, shuffle=shuffle)
+    def __len__(self) -> int:
+        raise NotImplementedError
 
+    def sample(self) -> Iterator[Tuple[Any, Any]]:
+        buffer, is_full = [], False
+        for sample in self:
+            buffer.append(sample)
+            if is_full:
+                i = np.random.randint(len(buffer))
+                yield buffer.pop(i)
+            elif len(buffer) == self.buffer_size:
+                is_full = True
+        while buffer:
+            i = np.random.randint(len(buffer))
+            yield buffer.pop(i)
+
+
+class CorpusGenerator(BaseGenerator):
 
-class Seq2SeqDataSet(Iterable):
     def __init__(self,
-                 corpus,
+                 x_data: List,
+                 y_data: List,
                  *,
-                 batch_size: int = 64,
-                 encoder_processor,
-                 decoder_processor,
-                 encoder_seq_length: int = None,
-                 decoder_seq_length: int = None):
-        self.corpus = corpus
+                 buffer_size: int = 2000) -> None:
+        super(CorpusGenerator, self).__init__(buffer_size=buffer_size)
+        self.x_data = x_data
+        self.y_data = y_data
+        self.buffer_size = buffer_size
+
+    def __iter__(self) -> Iterator[Tuple[Any, Any]]:
+
+        data_length=len(self.x_data) if self.x_data is not None else len(self.y_data)
+        for i in range(data_length):
+            y_value=None
+            x_value=None
+            if self.y_data is not None:
+                y_value=self.y_data[i]
+            if self.x_data is not None:
+                x_value=self.x_data[i]
+            yield x_value,y_value
 
-        self.encoder_processor = encoder_processor
-        self.decoder_processor = decoder_processor
+    def __len__(self) -> int:
+        return len(self.x_data)
+
+
+class BatchDataSet(Iterable):
+    def __init__(self,
+                 corpus: CorpusGenerator,
+                 *,
+                 text_processor: 'BaseIndexer',
+                 label_processor: 'BaseIndexer',
+                 seq_length: int = None,
+                 max_position: int = None,
+                 segment: bool = False,
+                 batch_size: int = 64) -> None:
+        self.corpus = corpus
+        self.text_processor = text_processor
+        self.label_processor = label_processor
 
-        self.encoder_seq_length = encoder_seq_length
-        self.decoder_seq_length = decoder_seq_length
+        self.seq_length = seq_length
+        self.max_position = max_position
+        self.segment = segment
 
         self.batch_size = batch_size
 
     def __len__(self) -> int:
         return max(len(self.corpus) // self.batch_size, 1)
 
     def __iter__(self) -> Iterator:
         batch_x, batch_y = [], []
-        for x, y in self.corpus:
+        for x, y in self.corpus.sample():
             batch_x.append(x)
             batch_y.append(y)
             if len(batch_x) == self.batch_size:
-                x_tensor = self.encoder_processor.transform(batch_x, )
-                y_tensor = self.decoder_processor.transform(batch_y, )
+                x_tensor = self.text_processor.transform(batch_x,
+                                                         seq_length=self.seq_length,
+                                                         max_position=self.max_position,
+                                                         segment=self.segment)
+                y_tensor = self.label_processor.transform(batch_y,
+                                                          seq_length=self.seq_length,
+                                                          max_position=self.max_position)
                 yield x_tensor, y_tensor
                 batch_x, batch_y = [], []
+        if batch_x:
+            x_tensor = self.text_processor.transform(batch_x,
+                                                     seq_length=self.seq_length,
+                                                     max_position=self.max_position,
+                                                     segment=self.segment)
+            y_tensor = self.label_processor.transform(batch_y,
+                                                      seq_length=self.seq_length,
+                                                      max_position=self.max_position)
+            yield x_tensor, y_tensor
+
+    def take(self, batch_count: int = None) -> Any:
+        """
+        take batches from the dataset
+
+        Args:
+            batch_count: number of batch count, iterate forever when batch_count is None.
+        """
+        i = 0
+        should_continue = True
+        while should_continue:
+            for batch_x, batch_y in self.__iter__():
+                if batch_count is None or i < batch_count:
+                    i += 1
+                    yield batch_x, batch_y
+                if batch_count and i >= batch_count:
+                    should_continue = False
+                    break
+
+        # x_shape = self.text_processor.get_tensor_shape(self.batch_size, self.seq_length)
+        # y_shape = self.label_indexer.get_tensor_shape(self.batch_size, self.seq_length)
+        # dataset = tf.data.Dataset.from_generator(self.__iter__,
+        #                                          output_types=(tf.int64, tf.int64),
+        #                                          output_shapes=(x_shape, y_shape))
+        # dataset = dataset.repeat()
+        # dataset = dataset.prefetch(50)
+        # if batch_count is None:
+        #     batch_count = len(self)
+        # return dataset.take(batch_count)
 
-    def items(self, batch_count: int = None) -> Any:
-        x_shape = [self.batch_size, self.encoder_seq_length]
-        y_shape = [self.batch_size, self.decoder_seq_length]
-        dataset = tf.data.Dataset.from_generator(self.__iter__,
-                                                 output_types=(tf.int64, tf.int64),
-                                                 output_shapes=(x_shape, y_shape))
-        dataset = dataset.repeat()
-        dataset = dataset.prefetch(50)
-        if batch_count is None:
-            batch_count = len(self)
-        return dataset.take(batch_count)
```

## kolibri/data/text/quality/cosineSimilarity.py

 * *Ordering differences only*

```diff
@@ -1,96 +1,96 @@
-import numpy as np
-import pandas as pd
-import gc
-import networkx as nx
-
-from sklearn.feature_extraction.text import TfidfVectorizer
-from sklearn.metrics.pairwise import linear_kernel
-#from sklearn.metrics.pairwise import cosine_similarity
-from kolibri.data.text.quality.pairwise_cos_sim import cosine_similarity
-from kdmt.sequences import chunk_generator
-import datetime
-
-
-def find_similar(tfidf_matrix, index, top_n=5):
-    cosine_similarities = linear_kernel(tfidf_matrix[index:index + 1], tfidf_matrix).flatten()
-    related_docs_indices = [i for i in cosine_similarities.argsort()[::-1] if i != index]
-    # related_docs_indices = [i for i in cosine_similarities.argsort()[::-1] ]
-    return [(index, cosine_similarities[index]) for index in related_docs_indices][0:top_n]
-
-
-def findMisclassification(df, content_field, classField, id_col):
-    start_time = datetime.datetime.now()
-    # newCol ='Desp_NoSign_ShortDescription'
-    newCol = content_field
-    tfidf = TfidfVectorizer().fit_transform(df[newCol].values.astype('U'))
-    similarList = []
-    n = len(df[newCol])
-    threshold = 0.95 #config.qualityControl['simiScore']
-    count = 0
-    for searchIndex in range(n):
-        simiIndex = set()
-        for index, score in find_similar(tfidf, searchIndex):
-            if (score > threshold):
-                if df.iloc[searchIndex][classField] != df.iloc[index][classField]:
-                    simiIndex.add(df.iloc[index][id_col])
-        if simiIndex:
-            simiIndex.add(df.iloc[searchIndex][id_col])
-            if simiIndex not in similarList:
-                if similarList:
-                    newSet = True
-                    for itemSimi in simiIndex:
-                        # for itemList in similarList:
-                        for i in range(len(similarList)):
-                            if itemSimi in similarList[i]:
-                                similarList[i] = set(list(similarList[i]) + list(simiIndex))
-                                newSet = False
-                                break
-                    # that mean simiIndex is new set
-                    if newSet:
-                        if not set(simiIndex) < set(similarListSet):
-                            similarList.append((set(simiIndex)))
-                else:
-                    similarListSet = (tuple(x) for x in similarList)
-                    if not set(simiIndex) < set(similarListSet):  # check subset of list
-                        similarList.append(set(simiIndex))
-        if (searchIndex % 1000 == 0 and searchIndex != 0):
-            #logger.info('Compared %s data', (str)(searchIndex))
-            print("Compared %s data", str(searchIndex))
-
-        count = count + 1
-    end_time = datetime.datetime.now()
-
-    #logger.info('----Time to find miss classification {}----'.format(end_time - start_time))
-    print('Time to find miss classiication {}----'.format(end_time - start_time))
-    return similarList
-
-
-
-def findMisclassification2(df, content_field, classField, id_field, threshold = 0.95,chunk_size=1000):
-    start_time = datetime.datetime.now()
-    tfidf = TfidfVectorizer().fit_transform(df[content_field].values.astype('U'))
-    similarList = []
-    n = len(df[content_field])
-     #config.qualityControl['simiScore']
-    count = 0
-    G = nx.Graph()
-    for chunk in chunk_generator(list(range(0, n)), chunk_size):
-
-        if count==6:
-            print(count)
-        cosines=linear_kernel(tfidf[chunk], tfidf)
-        similar_sub_list_=np.where(cosines>threshold)
-#        similar_sub_list=[(df.iloc[s[0]+(count*chunk_size)]['source'], df.iloc[s[0]+(count*chunk_size)][id_field], df.iloc[s[0]+(count*chunk_size)][classField],df.iloc[s[0]+(count*chunk_size)][content_field], df.iloc[s[1]]['source'], df.iloc[s[1]][id_field], df.iloc[s[1]][classField], df.iloc[s[1]][content_field], df.iloc[s[1]]['lib1']) for s in zip(*similar_sub_list_) if s[0] != s[1] and df.iloc[s[0]+(count*chunk_size)][classField] !=df.iloc[s[1]][classField]]
-        similar_sub_list=[(df.index[s[0]+(count*chunk_size)], df.index[s[1]]) for s in zip(*similar_sub_list_) if s[0] != s[1] and df.iloc[s[0]+(count*chunk_size)][classField] !=df.iloc[s[1]][classField]]
-        count+=1
-        similarList.extend(similar_sub_list)
-        gc.collect()
-#    similarList=np.where(cosines>threshold)
-#    similarList=[(s[0], df.iloc[s[0]][classField], s[1], df.iloc[s[1]][classField]) for s in zip(*similarList) if s[0] != s[1] and df.iloc[s[0]][classField] !=df.iloc[s[1]][classField]]
-
-    end_time = datetime.datetime.now()
-
-    #logger.info('----Time to find miss classification {}----'.format(end_time - start_time))
-    print('Time to find miss classiication {}----'.format(end_time - start_time))
-    G.add_edges_from(similarList)
+import numpy as np
+import pandas as pd
+import gc
+import networkx as nx
+
+from sklearn.feature_extraction.text import TfidfVectorizer
+from sklearn.metrics.pairwise import linear_kernel
+#from sklearn.metrics.pairwise import cosine_similarity
+from kolibri.data.text.quality.pairwise_cos_sim import cosine_similarity
+from kdmt.sequences import chunk_generator
+import datetime
+
+
+def find_similar(tfidf_matrix, index, top_n=5):
+    cosine_similarities = linear_kernel(tfidf_matrix[index:index + 1], tfidf_matrix).flatten()
+    related_docs_indices = [i for i in cosine_similarities.argsort()[::-1] if i != index]
+    # related_docs_indices = [i for i in cosine_similarities.argsort()[::-1] ]
+    return [(index, cosine_similarities[index]) for index in related_docs_indices][0:top_n]
+
+
+def findMisclassification(df, content_field, classField, id_col):
+    start_time = datetime.datetime.now()
+    # newCol ='Desp_NoSign_ShortDescription'
+    newCol = content_field
+    tfidf = TfidfVectorizer().fit_transform(df[newCol].values.astype('U'))
+    similarList = []
+    n = len(df[newCol])
+    threshold = 0.95 #config.qualityControl['simiScore']
+    count = 0
+    for searchIndex in range(n):
+        simiIndex = set()
+        for index, score in find_similar(tfidf, searchIndex):
+            if (score > threshold):
+                if df.iloc[searchIndex][classField] != df.iloc[index][classField]:
+                    simiIndex.add(df.iloc[index][id_col])
+        if simiIndex:
+            simiIndex.add(df.iloc[searchIndex][id_col])
+            if simiIndex not in similarList:
+                if similarList:
+                    newSet = True
+                    for itemSimi in simiIndex:
+                        # for itemList in similarList:
+                        for i in range(len(similarList)):
+                            if itemSimi in similarList[i]:
+                                similarList[i] = set(list(similarList[i]) + list(simiIndex))
+                                newSet = False
+                                break
+                    # that mean simiIndex is new set
+                    if newSet:
+                        if not set(simiIndex) < set(similarListSet):
+                            similarList.append((set(simiIndex)))
+                else:
+                    similarListSet = (tuple(x) for x in similarList)
+                    if not set(simiIndex) < set(similarListSet):  # check subset of list
+                        similarList.append(set(simiIndex))
+        if (searchIndex % 1000 == 0 and searchIndex != 0):
+            #logger.info('Compared %s data', (str)(searchIndex))
+            print("Compared %s data", str(searchIndex))
+
+        count = count + 1
+    end_time = datetime.datetime.now()
+
+    #logger.info('----Time to find miss classification {}----'.format(end_time - start_time))
+    print('Time to find miss classiication {}----'.format(end_time - start_time))
+    return similarList
+
+
+
+def findMisclassification2(df, content_field, classField, id_field, threshold = 0.95,chunk_size=1000):
+    start_time = datetime.datetime.now()
+    tfidf = TfidfVectorizer().fit_transform(df[content_field].values.astype('U'))
+    similarList = []
+    n = len(df[content_field])
+     #config.qualityControl['simiScore']
+    count = 0
+    G = nx.Graph()
+    for chunk in chunk_generator(list(range(0, n)), chunk_size):
+
+        if count==6:
+            print(count)
+        cosines=linear_kernel(tfidf[chunk], tfidf)
+        similar_sub_list_=np.where(cosines>threshold)
+#        similar_sub_list=[(df.iloc[s[0]+(count*chunk_size)]['source'], df.iloc[s[0]+(count*chunk_size)][id_field], df.iloc[s[0]+(count*chunk_size)][classField],df.iloc[s[0]+(count*chunk_size)][content_field], df.iloc[s[1]]['source'], df.iloc[s[1]][id_field], df.iloc[s[1]][classField], df.iloc[s[1]][content_field], df.iloc[s[1]]['lib1']) for s in zip(*similar_sub_list_) if s[0] != s[1] and df.iloc[s[0]+(count*chunk_size)][classField] !=df.iloc[s[1]][classField]]
+        similar_sub_list=[(df.index[s[0]+(count*chunk_size)], df.index[s[1]]) for s in zip(*similar_sub_list_) if s[0] != s[1] and df.iloc[s[0]+(count*chunk_size)][classField] !=df.iloc[s[1]][classField]]
+        count+=1
+        similarList.extend(similar_sub_list)
+        gc.collect()
+#    similarList=np.where(cosines>threshold)
+#    similarList=[(s[0], df.iloc[s[0]][classField], s[1], df.iloc[s[1]][classField]) for s in zip(*similarList) if s[0] != s[1] and df.iloc[s[0]][classField] !=df.iloc[s[1]][classField]]
+
+    end_time = datetime.datetime.now()
+
+    #logger.info('----Time to find miss classification {}----'.format(end_time - start_time))
+    print('Time to find miss classiication {}----'.format(end_time - start_time))
+    G.add_edges_from(similarList)
     return [g for g in nx.connected_components(G)]
```

## kolibri/datasets/read_data.py

```diff
@@ -46,14 +46,15 @@
         filename = find('datasets/' + dataset + '.csv')
     except:
         try:
             filename=find('datasets/' + dataset)
         except:
             if download is not None:
                 download('datasets/'+dataset)
+                filename = find('datasets/' + dataset + '.csv')
             else:
                 pass
 
     data =None
     if filename is not None:
         if os.path.isfile(filename):
             try:
```

## kolibri/evaluation/metrics/__init__.py

```diff
@@ -4,8 +4,10 @@
 from kolibri.evaluation.metrics.classification import get_all_metrics as get_all_classification_metrics
 from kolibri.evaluation.metrics.regression import get_all_metrics as get_all_regression_metrics
 from kolibri.config import TaskType
 
 
 def get_metric(task_type, metric):
     if task_type in [TaskType.CLASSIFICATION, TaskType.MULTI_TARGET_CLASSIFICATION, TaskType.BINARY_CLASSIFICATION]:
-        return get_all_classification_metrics()[metric]
+        return get_all_classification_metrics()[metric]
+    elif task_type in [TaskType.REGRESSION, TaskType.SCORING]:
+        return get_all_regression_metrics()[metric]
```

## kolibri/evaluation/metrics/regression.py

```diff
@@ -279,8 +279,16 @@
             instance = obj()
             if instance.active:
                 metrics_containers.append(instance)
         except Exception as e:
             print(e)
             pass
 
-    return {metric.id: metric for metric in metrics_containers}
+    return {metric.id: metric for metric in metrics_containers}
+
+
+
+if __name__ == "__main__":
+    mae=MAEMetric()
+    true_y=[1.2, 1.3, 1.4]
+    pred_y=[0.9, 1.1, 1.0]
+    print(mae.score_func(true_y, pred_y))
```

## kolibri/experiment_tracking/experiment_logger.py

```diff
@@ -128,15 +128,16 @@
                     console.info(
                         "SubProcess plot_model() called =================================="
                     )
 
                     def _log_plot(plot):
                         try:
                             plot_name = os.path.join(experiment.config["output-folder"], "plots", plot+".png")
-                            logger.log_plot(plot_name, Path(plot_name).stem)
+                            if os.path.exists(plot_name):
+                                logger.log_plot(plot_name, Path(plot_name).stem)
 
                         except Exception:
                             console.warning(
                                 f"Couldn't create plot {plot} for model, exception below:\n"
                                 f"{traceback.format_exc()}"
                             )
                     for plot in log_plots:
@@ -169,83 +170,14 @@
 
     def register_model(self, registered_model_name, artifact, registered_model_version_stage="Staging", archive_existing_versions=True):
         for logger in self.loggers:
             logger.register_model(registered_model_name, artifact, registered_model_version_stage=registered_model_version_stage, archive_existing_versions=archive_existing_versions)
     def log_pandas(self, df):
         for logger in self.loggers:
             logger.log_pandas(df)
-    def log_experiment(
-        self,
-        experiment: "ML_Experiment",
-        log_profile,
-        log_data,
-        experiment_custom_tags,
-        runtime,
-    ):
-        console = experiment.logger
-        console.info("Logging experiment in loggers")
-
-        k = experiment.display_container[0].copy()
-        k.set_index("Description", drop=True, inplace=True)
-        kdict = k.to_dict()
-        params = kdict.get("Value")
-        for logger in self.loggers:
-            logger.init_experiment(
-                experiment.exp_name_log, f"{SETUP_TAG} {experiment.USI}"
-            )
-            logger.log_params(params, "setup")
-            logger.set_tags("setup", experiment_custom_tags, runtime)
-
-        with tempfile.TemporaryDirectory() as tmpdir:
-            # Log the transformation pipeline
-            console.info(
-                "SubProcess save_model() called =================================="
-            )
-            experiment.save_model(
-                experiment.pipeline,
-                os.path.join(tmpdir, "Transformation Pipeline"),
-                verbose=False,
-            )
-            console.info(
-                "SubProcess save_model() end =================================="
-            )
-            [
-                logger.log_artifact(
-                    os.path.join(tmpdir, "Transformation Pipeline.pkl"),
-                    "transformation_pipe",
-                )
-                for logger in self.loggers
-            ]
-
-            # Log pandas profile
-            if log_profile:
-                profile_path = os.path.join(tmpdir, "Data Profile.html")
-                experiment.report.to_file(profile_path)
-                [
-                    logger.log_artifact(profile_path, "data_profile")
-                    for logger in self.loggers
-                ]
-
-            # Log training and testing set
-            if log_data:
-
-                train_path = os.path.join(tmpdir, "Train.csv")
-                test_path = os.path.join(tmpdir, "Test.csv")
-
-                experiment.train.to_csv(train_path)
-                experiment.test.to_csv(test_path)
-                [
-                    logger.log_artifact(train_path, "train_data")
-                    for logger in self.loggers
-                ]
-                [
-                    logger.log_artifact(test_path, "test_data")
-                    for logger in self.loggers
-                ]
-
 
     def log_model_comparison(self, results, source):
         for logger in self.loggers:
             logger.log_model_comparison(results, source)
 
     def finish(self):
         for logger in self.loggers:
```

## kolibri/experiment_tracking/mlflow_logger.py

```diff
@@ -1,37 +1,44 @@
 import secrets
 import os
 import tempfile
 import sklearn
 import platform
+try:
+    from kolibri import mlflow as kolibri_flavor
+except:
+    pass
 from kolibri import __version__
 try:
     import mlflow
     import mlflow.sklearn
 except ImportError:
     mlflow = None
-from kdmt.mlflow import is_model_registered
 
 def mlflow_remove_bad_chars(string: str) -> str:
     """Leaves only alphanumeric, spaces _, -, ., / in a string"""
     return "".join(c for c in string if c.isalpha() or c in ("_", "-", ".", " ", "/"))
 
 SETUP_TAG = "Session Initialized"
 
 class MlflowLogger():
     def __init__(self, config={}):
         if mlflow is None:
             raise ImportError(
                 "MlflowLogger requires mlflow. Install using `pip install mlflow`"
             )
+        if "MLFLOW_TRACKING_URI" in os.environ:
+            self.traking_uri= os.environ["MLFLOW_TRACKING_URI"]
+        if config["experiment-uri"] not in [None, ""]:
+            self.traking_uri=config["experiment-uri"]
 
-        self.traking_uri=config["experiment-uri"]
         self.experiment_name=config['experiment-name']
         if self.traking_uri is not None:
             mlflow.set_tracking_uri(self.traking_uri)
+
         self.run = None
 
     def init_experiment(self, exp_name_log):
         # get USI from nlp or tabular
         USI = secrets.token_hex(nbytes=2)
 
         experiment = mlflow.set_experiment(experiment_name=exp_name_log)
@@ -107,35 +114,20 @@
         default_conda_env["name"] = f"{experiment.experiment_name}-env"
         default_conda_env.get("dependencies").pop(-3)
         dependencies = default_conda_env.get("dependencies")[-1]
 
         dep = f"kolibri-ml=={__version__}"
         dependencies["pip"] = [dep]
 
+        try:
+            kolibri_flavor.log_model(experiment, artifact_path=experiment.config["artefacts-path"])
+        except Exception as e:
+            print(e)
 
-        library=experiment.pipeline.estimator.model_library
-        model=experiment.pipeline.estimator.model
-
-        if library == "sklearn":
-            mlflow.sklearn.log_model(model, "sklearn-model", registered_model_name=experiment.config['model-name'])
-        elif library == "xgboost":
-            mlflow.xgboost.log_model(model, "xgboost-model", registered_model_name=experiment.config['model-name'])
-        elif library == "catboost":
-            mlflow.catboost.log_model(model, "catboost-model", registered_model_name=experiment.config['model-name'])
-        else:
-            pass
-        directory=experiment.config["output-folder"]
-        for root, dirs, files in os.walk(directory):
-            for filename in files:
-                filre_path=os.path.join(root, filename)
-                dir_relative= os.path.relpath(root, start=directory)
-                if dir_relative=='.':
-                    dir_relative=None
 
-                mlflow.tracking.fluent.log_artifact(filre_path, dir_relative)
 
     def register_model(self, registered_model_name, artifact_path, registered_model_version_stage="Staging", archive_existing_versions=True):
         if self.run is None:
             raise Exception("Cannot register model if experiment is not tracked.")
         client=None
 
         model_uri = "runs:/{run_id}/{artifact_path}".format(run_id=self.run.info.run_id, artifact_path=artifact_path)
```

## kolibri/features/text/hashing_tfidf_vectorizer.py

```diff
@@ -17,18 +17,17 @@
 from typing import List, Any, Generator, Tuple, KeysView, ValuesView, Dict, Optional
 
 import numpy as np
 import scipy as sp
 from scipy import sparse
 from sklearn.utils import murmurhash3_32
 
-from deeppavlov.core.common.registry import register
-from deeppavlov.core.models.component import Component
-from deeppavlov.core.models.estimator import Estimator
-
+from kolibri.registry import register
+from kolibri.core.component import Component
+from kolibri.features.basefeaturizer import BaseFeaturizer
 logger = getLogger(__name__)
 
 Sparse = sp.sparse.csr_matrix
 
 
 def hash_(token: str, hash_size: int) -> int:
     """Convert a token to a hash of given size.
@@ -39,16 +38,16 @@
     Returns:
         int, hashed token
 
     """
     return murmurhash3_32(token, positive=True) % hash_size
 
 
-@register('hashing_tfidf_vectorizer')
-class HashingTfIdfVectorizer(Estimator):
+@register('HashingTfIdfVectorizer')
+class HashingTfIdfVectorizer(BaseFeaturizer):
     """Create a tfidf matrix from collection of documents of size [n_documents X n_features(hash_size)].
 
     Args:
         tokenizer: a tokenizer class
         hash_size: a hash size, power of two
         doc_index: a dictionary of document ids and their titles
         save_path: a path to **.npz** file where tfidf matrix is saved
```

## kolibri/features/text/text_features.py

```diff
@@ -1,17 +1,18 @@
 from kolibri.features.basefeaturizer import BaseFeaturizer
 from kolibri.logger import get_logger
 import numpy as np
 import inspect
 import kolibri.features.text.feature_functions as ffunctions
-
+from kolibri.registry import register
 logger = get_logger(__name__)
 
 
 
+@register('TextFeatureExtractor')
 class TextFeatureExtractor(BaseFeaturizer):
 
     provides = ["text_features"]
 
     requires = []
 
     defaults = {
```

## kolibri/features/text/tf_idf_featurizer.py

```diff
@@ -4,17 +4,18 @@
 
 import joblib
 import pickle
 from sklearn.feature_extraction.text import TfidfVectorizer
 from kdmt.dict import update
 from kolibri.features.basefeaturizer import BaseFeaturizer
 from kolibri.logger import get_logger
-
+from kolibri.registry import register
 logger = get_logger(__name__)
 
+@register('TFIDFFeaturizer')
 class TFIDFFeaturizer(BaseFeaturizer):
     """Bag of words featurizer
 
     Creates bag-of-words representation of intent features
     using sklearn's `CountVectorizer`.
     All tokens which consist only of digits (e.g. 123 and 99
     but not ab12d) will be represented by a single feature."""
@@ -146,15 +147,15 @@
         featurizer_file = os.path.join(model_dir, self.name + ".pkl")
         joblib.dump(self, featurizer_file)
 
         if self.get_parameter("save-base-model")==True:
             pickle.dump(self.vectorizer.vocabulary_, open(os.path.join(model_dir, "_base_tfidf_.pkl"), "wb"))
 
 
-        return {"featurizer_file": self.name + ".pkl", 'folder': model_dir}
+        return {"featurizer_file": self.name + ".pkl", 'folder': None}
 
     @classmethod
     def load(cls,
              model_dir=None, model_metadata=None, cached_component=None, **kwargs):
 
 
         if model_metadata.get("folder") is not None:
```

## kolibri/features/text/tf_idf_topics_vectorizer.py

```diff
@@ -5,17 +5,18 @@
 
 import joblib
 import pickle
 from sklearn.decomposition import TruncatedSVD
 from sklearn.pipeline import Pipeline as SKPipeline
 from kolibri.features.text.tf_idf_featurizer import TFIDFFeaturizer
 from kolibri.logger import get_logger
-
+from kolibri.registry import register
 logger = get_logger(__name__)
 
+@register('TFIDFTopicFeaturizer')
 class TFIDFTopicFeaturizer(TFIDFFeaturizer):
     """Bag of words featurizer
 
     Creates bag-of-words representation of intent features
     using sklearn's `CountVectorizer`.
     All tokens which consist only of digits (e.g. 123 and 99
     but not ab12d) will be represented by a single feature."""
```

## kolibri/features/text/tfidf_weighted_embedder.py

```diff
@@ -1,31 +1,21 @@
 
 from logging import getLogger
-from typing import List, Union, Optional, Tuple
+from typing import List, Union
 
 import numpy as np
+from kdmt.sequences import pad
 from overrides import overrides
-from pathlib import Path
-from kdmt.dict import update
-from kolibri.features.text.tf_idf_featurizer import TFIDFFeaturizer
-from kolibri.logger import get_logger
-
-
+from kolibri.registry import register
 from kolibri.features.text.embedders import get_embedder
-
-def expand_path(path: Union[str, Path]) -> Path:
-    """Convert relative paths to absolute with resolving user directory."""
-    return Path(path).expanduser().resolve()
-
-from kdmt.sequences import pad
-
+from kolibri.features.text.tf_idf_featurizer import TFIDFFeaturizer
 
 logger = getLogger(__name__)
 
-
+@register('TfidfWeightedEmbedder')
 class TfidfWeightedEmbedder(TFIDFFeaturizer):
     """
     The class implements the functionality of embedding the sentence \
         as a weighted average by special coefficients of tokens embeddings. \
         Coefficients can be taken from the given TFIDF-vectorizer in ``vectorizer`` or \
         calculated as TFIDF from counter vocabulary given in ``counter_vocab_path``.
         Also one can give ``tags_vocab_path`` to the vocabulary with weights of tags. \
@@ -55,16 +45,16 @@
         counter_vocab: counter vocabulary
         idf_base_count: minimal idf value (less time occured are not counted)
         log_base: logarithm base for TFIDF-coefficient calculation froom counter vocabulary
         min_idf_weight: minimal idf weight
 
     Examples:
         >>> from kolibri.features.text.embedders.tfidf_weighted_embedder import TfidfWeightedEmbedder
-        >>> from kolibri.features.text.embedders.fasttext_embedder import FasttextEmbedder
-        >>> fasttext_embedder = FasttextEmbedder('/data/embeddings/wiki.ru.bin')
+        >>> from kolibri.features.text.embedders.fasttext_embedder import FasttextEmbedding
+        >>> fasttext_embedder = FasttextEmbedding('/data/embeddings/wiki.ru.bin')
         >>> fastTextTfidf = TfidfWeightedEmbedder(embedder=fasttext_embedder,
                 counter_vocab_path='/data/vocabs/counts_wiki_lenta.txt')
         >>> fastTextTfidf([['большой', 'и', 'розовый', 'бегемот']])
         [array([ 1.99135890e-01, -7.14746421e-02,  8.01428872e-02, -5.32840924e-02,
                  5.05212297e-02,  2.76053832e-01, -2.53270134e-01, -9.34443950e-02,
                  ...
                  1.18385439e-02,  1.05643446e-01, -1.21904516e-03,  7.70555378e-02])]
```

## kolibri/features/text/embedders/__init__.py

```diff
@@ -1,10 +1,10 @@
-from kolibri.features.text.embedders.glove_embedder import GloVeEmbedder
-from kolibri.features.text.embedders.fasttext_embedder import FasttextEmbedder
+from kolibri.features.text.embedders.glove_embedder import GloVeEmbedding
+from kolibri.features.text.embedders.fasttext_embedder import FasttextEmbedding
 
 def get_embedder(embedder, configs):
     if embedder=="glove":
-        return GloVeEmbedder(configs)
+        return GloVeEmbedding(configs)
     elif embedder=="fasttext":
-        return FasttextEmbedder(configs)
+        return FasttextEmbedding(configs)
 
     return None
```

## kolibri/features/text/embedders/bow_embedder.py

```diff
@@ -1,16 +1,17 @@
 
 from typing import List
 
 import numpy as np
+from kolibri.registry import register
+from kolibri.features.text.embedders.base import Embeddings
 
-from kolibri.core.component import Component
 
-
-class BoWEmbedder(Component):
+@register('BoWEmbedder')
+class BoWEmbedder(Embeddings):
     """
     Performs one-hot encoding of tokens based on a pre-built vocabulary of tokens.
 
     Parameters:
         depth: size of output numpy vector.
         with_counts: flag denotes whether to use binary encoding (with zeros and ones),
             or to use counts as token representation.
@@ -23,18 +24,19 @@
             >>> bow([[0, 1], [1], [])
             [array([1, 1, 0], dtype=int32),
              array([0, 1, 0], dtype=int32),
              array([0, 0, 0], dtype=int32)]
     """
 
     def __init__(self, depth: int, with_counts: bool = False, **kwargs) -> None:
+        super().__init__()
         self.depth = depth
         self.with_counts = with_counts
 
-    def _encode(self, token_indices: List[int]) -> np.ndarray:
+    def embed_documents(self, token_indices: List[int]) -> np.ndarray:
         bow = np.zeros([self.depth], dtype=np.int32)
         for idx in token_indices:
             if self.with_counts:
                 bow[idx] += 1
             else:
                 bow[idx] = 1
         return bow
```

## kolibri/features/text/embedders/elmo_embedder.py

```diff
@@ -1,41 +1,28 @@
-# Copyright 2017 Neural Networks and Deep Learning lab, MIPT
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
 
 import sys
 from logging import getLogger
 from typing import Iterator, List, Union, Optional
 
 import numpy as np
 import tensorflow as tf
 import tensorflow_hub as hub
 from overrides import overrides
 
-from deeppavlov.core.commands.utils import expand_path
-from deeppavlov.core.common.registry import register
-from deeppavlov.core.data.utils import zero_pad, chunk_generator
-from deeppavlov.core.models.component import Component
-from deeppavlov.core.models.tf_backend import TfModelMeta
+from kdmt.path import expand_path
+from kolibri.registry import register
+from kdmt.lists import chunk_generator
+from kolibri.core.component import Component
+#from kolibri.core.models.tf_backend import TfModelMeta
 
 log = getLogger(__name__)
 
 
-@register('elmo_embedder')
-class ELMoEmbedder(Component, metaclass=TfModelMeta):
+@register('ELMoEmbedder')
+class ELMoEmbedder(Component):
     """
     ``ELMo`` (Embeddings from Language Models) representations are pre-trained contextual representations from
     large-scale bidirectional language models. See a paper `Deep contextualized word representations
     <https://arxiv.org/abs/1802.05365>`__ for more information about the algorithm and a detailed analysis.
 
     Parameters:
         spec: A ``ModuleSpec`` defining the Module to instantiate or a path where to load a ``ModuleSpec`` from via
@@ -59,79 +46,24 @@
         mini_batch_size: It is used to reduce the memory requirements of the device.
 
 
     If some required packages are missing, install all the requirements by running in command line:
 
     .. code:: bash
 
-        python -m deeppavlov install <path_to_config>
+        python -m kolibri install <path_to_config>
 
     where ``<path_to_config>`` is a path to one of the :config:`provided config files <elmo_embedder>`
     or its name without an extension, for example :
 
     .. code:: bash
 
-        python -m deeppavlov install elmo_ru-news
+        python -m kolibri install elmo_ru-news
         
     Examples:
-        >>> from deeppavlov.models.embedders.elmo_embedder import ELMoEmbedder
-        >>> elmo = ELMoEmbedder("http://files.deeppavlov.ai/deeppavlov_data/elmo_ru-news_wmt11-16_1.5M_steps.tar.gz")
-        >>> elmo([['вопрос', 'жизни', 'Вселенной', 'и', 'вообще', 'всего'], ['42']])
-        array([[ 0.00719104,  0.08544601, -0.07179783, ...,  0.10879009,
-                -0.18630421, -0.2189409 ],
-               [ 0.16325025, -0.04736076,  0.12354863, ..., -0.1889013 ,
-                 0.04972512,  0.83029324]], dtype=float32)
-
-        You can use ELMo models from DeepPavlov as usual `TensorFlow Hub Module
-        <https://www.tensorflow.org/hub/modules/google/elmo/2>`_.
-
-        >>> import tensorflow as tf
-        >>> import tensorflow_hub as hub
-        >>> elmo = hub.Module("http://files.deeppavlov.ai/deeppavlov_data/elmo_ru-news_wmt11-16_1.5M_steps.tar.gz",
-        trainable=True)
-        >>> sess = tf.Session()
-        >>> sess.run(tf.global_variables_initializer())
-        >>> embeddings = elmo(["это предложение", "word"], signature="default", as_dict=True)["elmo"]
-        >>> sess.run(embeddings)
-        array([[[ 0.05817392,  0.22493343, -0.19202903, ..., -0.14448944,
-                 -0.12425567,  1.0148407 ],
-                [ 0.53596294,  0.2868537 ,  0.28028542, ..., -0.08028372,
-                  0.49089077,  0.75939953]],
-               [[ 0.3433637 ,  1.0031182 , -0.1597258 , ...,  1.2442509 ,
-                  0.61029315,  0.43388373],
-                [ 0.05370751,  0.02260921,  0.01074906, ...,  0.08748816,
-                 -0.0066415 , -0.01344293]]], dtype=float32)
-
-        TensorFlow Hub module also supports tokenized sentences in the following format.
-
-        >>> tokens_input = [["мама", "мыла", "раму"], ["рама", "", ""]]
-        >>> tokens_length = [3, 1]
-        >>> embeddings = elmo(
-                inputs={
-                        "tokens": tokens_input,
-                        "sequence_len": tokens_length
-                        },
-                signature="tokens",
-                as_dict=True)["elmo"]
-        >>> sess.run(embeddings)
-        array([[[ 0.6040001 , -0.16130011,  0.56478846, ..., -0.00376141,
-                 -0.03820051,  0.26321286],
-                [ 0.01834148,  0.17055789,  0.5311495 , ..., -0.5675535 ,
-                  0.62669843, -0.05939034],
-                [ 0.3242596 ,  0.17909613,  0.01657108, ...,  0.1866098 ,
-                  0.7392496 ,  0.08285746]],
-               [[ 1.1322289 ,  0.19077688, -0.17811403, ...,  0.42973226,
-                  0.23391506, -0.01294377],
-                [ 0.05370751,  0.02260921,  0.01074906, ...,  0.08748816,
-                 -0.0066415 , -0.01344293],
-                [ 0.05370751,  0.02260921,  0.01074906, ...,  0.08748816,
-                 -0.0066415 , -0.01344293]]], dtype=float32)
-
-        You can also get ``hub.text_embedding_column`` like described `here
-        <https://www.tensorflow.org/hub/tutorials/text_classification_with_tf_hub#feature_columns>`_.
 
 
     """
 
     def __init__(self, spec: str, elmo_output_names: Optional[List] = None,
                  dim: Optional[int] = None, pad_zero: bool = False,
                  concat_last_axis: bool = True, max_token: Optional[int] = None,
@@ -287,17 +219,14 @@
             elmo_output_values = []
             for mini_batch in batch_gen:
                 mini_batch_out = self._mini_batch_fit(mini_batch, *args, **kwargs)
                 elmo_output_values.extend(mini_batch_out)
         else:
             elmo_output_values = self._mini_batch_fit(batch, *args, **kwargs)
 
-        if self.pad_zero:
-            elmo_output_values = zero_pad(elmo_output_values)
-
         return elmo_output_values
 
     def __iter__(self) -> Iterator:
         """
         Iterate over all words from a ELMo model vocabulary.
         The ELMo model vocabulary consists of ``['<S>', '</S>', '<UNK>']``.
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## kolibri/features/text/embedders/fasttext_embedder.py

```diff
@@ -9,19 +9,19 @@
     fast_text_loaded = True
 except:
     fast_text_not_loaded=True
 
 import numpy as np
 from overrides import overrides
 
-from kolibri.features.text.embedders.abstract_embedder import Embedder
+from kolibri.features.text.embedders.base import Embeddings
 
 log = getLogger(__name__)
 
-class FasttextEmbedder(Embedder):
+class FasttextEmbedding(Embeddings):
     """
     Class implements fastText embedding model
 
     Args:
         load_path: path where to load pre-trained embedding model from
         pad_zero: whether to pad samples or not
 
@@ -29,15 +29,15 @@
         model: fastText model instance
         tok2emb: dictionary with already embedded tokens
         dim: dimension of embeddings
         pad_zero: whether to pad sequence of tokens with zeros or not
         load_path: path with pre-trained fastText binary model
     """
 
-    def _get_word_vector(self, w: str) -> np.ndarray:
+    def embed_query(self, w: str) -> np.ndarray:
         return self.model.get_word_vector(w)
 
     def load(self) -> None:
         """
         Load fastText binary model from self.load_path
         """
         log.info(f"[loading fastText embeddings from `{self.load_path}`]")
```

## kolibri/features/text/embedders/glove_embedder.py

```diff
@@ -8,21 +8,21 @@
 try:
     from gensim.models import KeyedVectors
     gensim_imported=True
 except:
     pass
 from overrides import overrides
 
-from kolibri.features.text.embedders.abstract_embedder import Embedder
+from kolibri.features.text.embedders.base import Embeddings
 
 log = getLogger(__name__)
 
 
 #Todo: soleve duplicate declaration of this class in tensorflow backend
-class GloVeEmbedder(Embedder):
+class GloVeEmbedding(Embeddings):
     """
     Class implements GloVe embedding model
 
     Args:
         load_path: path where to load pre-trained embedding model from
         pad_zero: whether to pad samples or not
 
@@ -30,15 +30,15 @@
         model: GloVe model instance
         tok2emb: dictionary with already embedded tokens
         dim: dimension of embeddings
         pad_zero: whether to pad sequence of tokens with zeros or not
         load_path: path with pre-trained GloVe model
     """
 
-    def _get_word_vector(self, w: str) -> np.ndarray:
+    def embed_query(self, w: str) -> np.ndarray:
         return self.model[w]
 
     def load(self):
         """
         Load dict of embeddings from given file
         """
         log.info(f"[loading GloVe embeddings from `{self.load_path}`]")
```

## kolibri/features/timeseries/utils.py

```diff
@@ -41,15 +41,15 @@
 def embed(x: np.array, p: int) -> np.array:
     """Embeds the time series x into a low-dimensional Euclidean space.
     Parameters
     ----------
     x: numpy array
         Time series.
     p: int
-        Embedding dimension.
+        Embeddings dimension.
     References
     ----------
     https://www.rdocumentation.org/packages/stats/versions/3.6.2/topics/embed
     """
     x = np.transpose(np.vstack(list((np.roll(x, k) for k in range(p)))))
     x = x[p - 1:]
```

## kolibri/formers/text/topic_former.py

```diff
@@ -24,15 +24,15 @@
 
     """
 
     defaults={
         "model": "lda",
         "algorithm": "gibbs",
         "model_name":"topics",
-        "num_topics": 20,
+        "": 20,
         "language":"en",
         "remove-stopwords": True
 
     }
     def __init__(self,output_folder, data, target, configs={}):
 
         for key in configs:
```

## kolibri/indexers/__init__.py

```diff
@@ -1,7 +1,10 @@
-from kolibri.indexers.label_indexer import LabelIndexer
-from kolibri.indexers.text_indexer import TextIndexer
-from kolibri.indexers.label_indexer import LabelIndexer
-from kolibri.indexers.multi_content_indexer import MultiContentIndexer
-from kolibri.indexers.sequence_char_indexer import SequenceCharIndexer
-from kolibri.indexers.multi_target_indexer import MultiTargetIndexer
-from kolibri.indexers.sequence_indexer import SequenceIndexer
+# encoding: utf-8
+
+
+from .base_indexer import BaseIndexer
+from .label_indexer import LabelIndexer
+from .sequence_indexer import SequenceIndexer
+from .text_indexer import TextIndexer
+
+if __name__ == "__main__":
+    pass
```

## kolibri/indexers/base_indexer.py

```diff
@@ -1,198 +1,83 @@
-from typing import Dict, Any, Tuple
-from collections import Counter
-import sys, warnings, os
-import tqdm
-from multiprocessing import Pool
-import tempfile, operator, collections
+# encoding: utf-8
 
+from abc import ABC
+from typing import Dict, List, Optional, Any, Tuple
+from kolibri.types import TextSamplesVar
+
+import numpy as np
+try:
+    from kolibri.data.text.generators import CorpusGenerator
+except:
+    pass
 
-class BaseIndexer():
+class BaseIndexer(ABC):
     def to_dict(self) -> Dict[str, Any]:
         return {
             'config': {
                 'token_pad': self.token_pad,
                 'token_unk': self.token_unk,
                 'token_bos': self.token_bos,
                 'token_eos': self.token_eos,
-                'token2idx': self.token2idx
+                'token2idx': self.token2idx,
+                'segment': self.segment
             },
             '__class_name__': self.__class__.__name__,
             '__module__': self.__class__.__module__,
         }
 
-    def __init__(self,multi_label=False,index=None, **kwargs: Any) -> None:
-        from sklearn.preprocessing import MultiLabelBinarizer
-
+    def __init__(self, **kwargs: Any) -> None:
         self.token2idx = kwargs.get('token2idx', {})
         self.idx2token = dict([(v, k) for k, v in self.token2idx.items()])
 
+        self.segment = False
+
         self.token_pad: str = kwargs.get('token_pad', '[PAD]')  # type: ignore
         self.token_unk: str = kwargs.get('token_unk', '[UNK]')  # type: ignore
         self.token_bos: str = kwargs.get('token_bos', '[CLS]')  # type: ignore
         self.token_eos: str = kwargs.get('token_eos', '[SEP]')  # type: ignore
 
-        self.multi_label = multi_label
-        self.index = index
-        self.multi_label_binarizer = MultiLabelBinarizer(classes=self.token2idx)
+        self._sequence_length_from_saved_model: Optional[int] = None
 
     @property
     def vocab_size(self) -> int:
         return len(self.token2idx)
 
-    def __getitem__(self, tokenid):
-        """Get the string token that corresponds to `tokenid`.
-        Parameters
-        ----------
-        tokenid : int
-            Id of token.
-        Returns
-        -------
-        str
-            Token corresponding to `tokenid`.
-        Raises
-        ------
-        KeyError
-            If this Dictionary doesn't contain such `tokenid`.
-        """
-
-        return self.idx2token[tokenid]  # will throw for non-existent ids
-
-    def __iter__(self):
-        """Iterate over all tokens."""
-        return iter(self.keys())
-
-    # restore Py2-style dict API
-    iterkeys = __iter__
-
-    def keys(self):
-        """Get all stored ids.
-        Returns
-        -------
-        list of int
-            List of all token ids.
-        """
-        return list(self.token2idx.values())
-
-    def __len__(self):
-        """Get number of stored tokens.
-        Returns
-        -------
-        int
-            Number of stored tokens.
-        """
-        return len(self.token2idx)
-
-
     @property
     def is_vocab_build(self) -> bool:
         return self.vocab_size != 0
 
-    def build_vocab(self, x_data, y_data=None):
-        raise NotImplementedError
+    def build_vocab(self,
+                    x_data: TextSamplesVar,
+                    y_data: TextSamplesVar) -> None:
+        corpus_gen = CorpusGenerator(x_data, y_data)
+        self.build_vocab_generator([corpus_gen])
 
-    def build_vocab_generator(self, generators):
-        try:
-            from sklearn.preprocessing import MultiLabelBinarizer
-        except:
-            pass
-
-
-        if self.token2idx:
-            return
-
-        vocab2idx: Dict[str, int] = {}
-        token2count: Dict[str, int] = {}
-        for generator in generators:
-            if self.multi_label:
-                for _, label in tqdm.tqdm(generator, desc="Preparing classification label vocab dict"):
-                    if self.index is not None:
-                        label = label[self.index]
-                    for token in label:
-                        count = token2count.get(token, 0)
-                        token2count[token] = count + 1
-            else:
-                for _, label in tqdm.tqdm(generator, desc="Preparing classification label vocab dict"):
-                    if self.index is not None:
-                        label = label[self.index]
-
-                    count = token2count.get(label, 0)
-                    token2count[label] = count + 1
-
-        sorted_token2count = sorted(token2count.items(),
-                                    key=operator.itemgetter(1),
-                                    reverse=True)
-        token2count = collections.OrderedDict(sorted_token2count)
-
-        for token, token_count in token2count.items():
-            if token not in vocab2idx:
-                vocab2idx[token] = len(vocab2idx)
-        self.token2idx = vocab2idx
-        self.idx2token = dict([(v, k) for k, v in self.token2idx.items()])
-        self.multi_label_binarizer = MultiLabelBinarizer(classes=self.token2idx)
+    def build_vocab_generator(self,
+                              generators: List[CorpusGenerator]) -> None:
+        raise NotImplementedError
 
     def get_tensor_shape(self, batch_size: int, seq_length: int) -> Tuple:
-        return batch_size, seq_length
+        if self.segment:
+            return 2, batch_size, seq_length
+        else:
+            return batch_size, seq_length
 
-    def transform(self, samples):
+    def transform(self,
+                  samples: TextSamplesVar,
+                  *,
+                  seq_length: int = None,
+                  max_position: int = None,
+                  segment: bool = False) -> np.ndarray:
         raise NotImplementedError
 
-    def inverse_transform(self, labels, lengths=None, threshold: float = 0.5, **kwargs):
+    def inverse_transform(self,
+                          labels: List[int],
+                          *,
+                          lengths: List[int] = None,
+                          threshold: float = 0.5,
+                          **kwargs: Any) -> List[str]:
         raise NotImplementedError
 
-    def get_vocabulary(self, data, is_dict=False, num_workers=1):
-        """Read text and return dictionary that encodes vocabulary
-        """
-        vocab = Counter()
-        if is_dict:
-
-            for i, line in enumerate( tqdm.tqdm(data)):
-                try:
-                    word, count = line.strip('\r\n ').split(' ')
-                except:
-                    print('Failed reading vocabulary file at line {0}: {1}'.format(i, line))
-                    sys.exit(1)
-                vocab[word] += int(count)
-        elif num_workers == 1:
-            if num_workers > 1:
-                warnings.warn("In parallel mode, the input cannot be STDIN. Using 1 processor instead.")
-            for i, line in enumerate( tqdm.tqdm(data)):
-                for word in line.strip('\r\n ').split(' '):
-                    if word:
-                        vocab[word] += 1
-
-        elif num_workers > 1:
-            size = len(data)
-            chunk_size = int(size / num_workers)
-            offsets = [i*chunk_size for i in range(num_workers + 1)]
-            offsets[-1]=size
-
-            vocab_files = []
-            pool = Pool(processes=num_workers)
-            for i in range(num_workers):
-                tmp = tempfile.NamedTemporaryFile(delete=False)
-                tmp.close()
-                vocab_files.append(tmp)
-                pool.apply_async(self._get_vocabulary, (data, tmp.name, offsets[i], offsets[i + 1]))
-            pool.close()
-            pool.join()
-            import pickle
-            for i in range(num_workers):
-                with open(vocab_files[i].name, 'rb', encoding='utf-8') as f:
-                    vocab += pickle.load(f)
-                os.remove(vocab_files[i].name)
-        else:
-            raise ValueError('`num_workers` is expected to be a positive number, but got {}.'.format(num_workers))
-        return vocab
-    def _get_vocabulary(self, data, outfile, begin, end):
-        import pickle
-        vocab = Counter()
-        for line in  tqdm.tqdm(data[begin:end]):
-            for word in line.strip('\r\n ').split(' '):
-                if word:
-                    vocab[word] += 1
-        with open(outfile, 'wb') as f:
-            pickle.dump(vocab, f)
-
 
 if __name__ == "__main__":
-    print("Hello world")
+    pass
```

## kolibri/indexers/label_indexer.py

```diff
@@ -1,93 +1,95 @@
+# encoding: utf-8
+
+
 import collections
 import operator
-from typing import Dict, Any, Tuple
+from typing import List, Union, Dict, Any, Tuple
 
 import numpy as np
 import tqdm
 
+from kolibri.data.text.generators import CorpusGenerator
 from kolibri.indexers.base_indexer import BaseIndexer
+from kolibri.types import TextSamplesVar
 
 
 class LabelIndexer(BaseIndexer):
 
     def to_dict(self) -> Dict[str, Any]:
         data = super(LabelIndexer, self).to_dict()
         data['config']['multi_label'] = self.multi_label
-        data['config']['index'] = self.index
         return data
 
-    def __init__(self, multi_label=False, index=None, **kwargs):
-        from sklearn.preprocessing import MultiLabelBinarizer
+    def __init__(self,
+                 multi_label: bool = False,
+                 **kwargs: Any) -> None:
+        from kolibri.backend.tensorflow.utils import MultiLabelBinarizer
         super(LabelIndexer, self).__init__(**kwargs)
         self.multi_label = multi_label
-        self.multi_label_binarizer = MultiLabelBinarizer()
-        self.multi_label_binarizer.fit_transform(self.token2idx)
-        self.index = index
+        self.multi_label_binarizer = MultiLabelBinarizer(self.token2idx)
 
-    def build_vocab(self, x_data, y_data):
-        from sklearn.preprocessing import MultiLabelBinarizer
+    def build_vocab_generator(self,
+                              generators: List[CorpusGenerator]) -> None:
+        from kolibri.backend.tensorflow.utils import MultiLabelBinarizer
         if self.token2idx:
             return
 
-        if y_data is None:
-            raise ValueError
-
         token2idx: Dict[str, int] = {}
         token2count: Dict[str, int] = {}
-        if self.multi_label:
-            for label in tqdm.tqdm(y_data, desc="Preparing classification label vocab dict"):
-                if self.index is not None:
-                    label = label[self.index]
-                for token in label:
-                    count = token2count.get(token, 0)
-                    token2count[token] = count + 1
-        else:
-            for label in tqdm.tqdm(y_data, desc="Preparing classification label vocab dict"):
-                if self.index is not None:
-                    label = label[self.index]
-
-                count = token2count.get(label, 0)
-                token2count[label] = count + 1
+        for generator in generators:
+            if self.multi_label:
+                for _, label in tqdm.tqdm(generator, desc="Preparing classification label vocab dict"):
+                    for token in label:
+                        count = token2count.get(token, 0)
+                        token2count[token] = count + 1
+            else:
+                for _, label in tqdm.tqdm(generator, desc="Preparing classification label vocab dict"):
+                    count = token2count.get(label, 0)
+                    token2count[label] = count + 1
 
         sorted_token2count = sorted(token2count.items(),
                                     key=operator.itemgetter(1),
                                     reverse=True)
         token2count = collections.OrderedDict(sorted_token2count)
 
         for token, token_count in token2count.items():
             if token not in token2idx:
                 token2idx[token] = len(token2idx)
         self.token2idx = token2idx
         self.idx2token = dict([(v, k) for k, v in self.token2idx.items()])
-        self.multi_label_binarizer = MultiLabelBinarizer()
-        self.multi_label_binarizer.fit(self.token2idx)
+        self.multi_label_binarizer = MultiLabelBinarizer(self.token2idx)
 
     def get_tensor_shape(self, batch_size: int, seq_length: int) -> Tuple:
         if self.multi_label:
             return batch_size, len(self.token2idx)
         else:
             return (batch_size,)
 
-    def transform(self, samples, **kwargs):
+    def transform(self,
+                  samples: TextSamplesVar,
+                  *,
+                  seq_length: int = None,
+                  max_position: int = None,
+                  segment: bool = False) -> np.ndarray:
         if self.multi_label:
             sample_tensor = self.multi_label_binarizer.transform(samples)
             return sample_tensor
-        if self.index is not None:
-            sample_tensor = [self.token2idx[sample[self.index]] for sample in samples]
-        else:
-            sample_tensor = [self.token2idx[sample] for sample in samples]
+
+        sample_tensor = [self.token2idx[i] for i in samples]
         return np.array(sample_tensor)
 
-    def inverse_transform(self,
-                          labels,
+    def inverse_transform(self,  # type: ignore[override]
+                          labels: Union[List[int], np.ndarray],
                           *,
-                          lengths=None,
-                          **kwargs):
+                          lengths: List[int] = None,
+                          threshold: float = 0.5,
+                          **kwargs: Any) -> Union[List[List[str]], List[str]]:
         if self.multi_label:
-            return self.multi_label_binarizer.inverse_transform(labels)
+            return self.multi_label_binarizer.inverse_transform(labels,
+                                                                threshold=threshold)
         else:
             return [self.idx2token[i] for i in labels]
 
 
 if __name__ == "__main__":
     pass
```

## kolibri/indexers/sequence_char_indexer.py

```diff
@@ -55,15 +55,15 @@
         self._showed_seq_len_warning = False
 
     def build_vocab(self, x_data, y_data=None):
         self.build_vocab_generator(zip(x_data, y_data))
 
     def build_vocab_generator(self, generators):
         if not self.token2idx:
-            vocab2idx = self._initial_vocab_dic
+            token2idx = self._initial_vocab_dic
             v_count = 2
             char_seq_length = 0
             for sentence, label in tqdm.tqdm(generators, desc="Preparing text vocab dict"):
                     if self.build_vocab_from_labels:
                         if self.index is not None:
                             target = label[self.index]
                         else:
@@ -74,28 +74,28 @@
                         target = target[self.index]
 
                     for token in target:
                         if isinstance(token, list):
                             for word in token:
                                 char_seq_length = max(char_seq_length, len(word))
                                 for ch in word:
-                                    if ch not in vocab2idx:
-                                        vocab2idx[ch] = v_count
+                                    if ch not in token2idx:
+                                        token2idx[ch] = v_count
                                         v_count += 1
                         else:
                             char_seq_length = max(char_seq_length, len(token))
                             for ch in token:
-                                if ch not in vocab2idx:
-                                    vocab2idx[ch] = v_count
+                                if ch not in token2idx:
+                                    token2idx[ch] = v_count
                                     v_count += 1
                     self.seq_length = max(self.seq_length, len(target))
             #            self.seq_length += 2
             if self.char_seq_length is None:
                 self.char_seq_length = char_seq_length
-            self.token2idx = vocab2idx
+            self.token2idx = token2idx
             self.idx2token = dict([(v, k) for k, v in self.token2idx.items()])
 
     def transform(self,
                   samples,
                   *,
                   char_seq_length: int = None,
                   max_position: int = None):
```

## kolibri/indexers/sequence_indexer.py

```diff
@@ -1,59 +1,63 @@
+# encoding: utf-8
+
+# author: BrikerMan
+# contact: eliyar917@gmail.com
+# blog: https://eliyar.biz
+
+# file: text_processor.py
+# time: 12:27 下午
+
 import collections
 import operator
-from typing import Dict, Any
+from typing import Dict, List, Any, Union
 
+import numpy as np
 import tqdm
 try:
     from tensorflow.keras.preprocessing.sequence import pad_sequences
+    from kolibri.backend.tensorflow.logger import logger
 except:
     pass
 
-from kolibri.indexers.base_indexer import BaseIndexer
-from kolibri.logger import get_logger
+from kolibri.data.text.generators import CorpusGenerator
 
-logger = get_logger(__name__)
+from kolibri.indexers.base_indexer import BaseIndexer
+from kolibri.types import TextSamplesVar
 
 
 class SequenceIndexer(BaseIndexer):
     """
     Generic indexers for the sequence samples.
     """
 
     def to_dict(self) -> Dict[str, Any]:
         data = super(SequenceIndexer, self).to_dict()
         data['config'].update({
             'build_in_vocab': self.build_in_vocab,
-            'min_count': self.min_count,
-            'seq_length': self.seq_length,
-            'index': self.index
+            'min_count': self.min_count
         })
         return data
 
     def __init__(self,
                  build_in_vocab: str = 'text',
-                 min_count: int = 0,
+                 min_count: int = 3,
                  build_vocab_from_labels: bool = False,
-                 index=None,
-                 **kwargs: Any):
+                 **kwargs: Any) -> None:
         """
 
         Args:
             vocab_dict_type: initial vocab dict type, one of `text` `labeling`.
             **kwargs:
         """
         super(SequenceIndexer, self).__init__(**kwargs)
 
         self.build_in_vocab = build_in_vocab
         self.min_count = min_count
         self.build_vocab_from_labels = build_vocab_from_labels
-        self.index = index
-        self.seq_length = 0
-        if 'seq_length' in kwargs:
-            self.seq_length = kwargs['seq_length']
 
         if build_in_vocab == 'text':
             self._initial_vocab_dic = {
                 self.token_pad: 0,
                 self.token_unk: 1,
                 self.token_bos: 2,
                 self.token_eos: 3
@@ -63,79 +67,105 @@
                 self.token_pad: 0
             }
         else:
             self._initial_vocab_dic = {}
 
         self._showed_seq_len_warning = False
 
-    def build_vocab_generator(self, generators):
+    def build_vocab_generator(self,
+                              generators: List[CorpusGenerator]) -> None:
         if not self.token2idx:
-            vocab2idx = self._initial_vocab_dic
-            max_len = 0
+            token2idx = self._initial_vocab_dic
+
             token2count: Dict[str, int] = {}
 
             for gen in generators:
                 for sentence, label in tqdm.tqdm(gen, desc="Preparing text vocab dict"):
                     if self.build_vocab_from_labels:
                         target = label
                     else:
                         target = sentence
-                    if self.index is not None:
-                        target = target[self.index]
-                    max_len = max(max_len, len(target))
-
-                    self.seq_length = max(self.seq_length, len(target))
                     for token in target:
                         count = token2count.get(token, 0)
                         token2count[token] = count + 1
-            #            self.seq_length += 2
+
             sorted_token2count = sorted(token2count.items(),
                                         key=operator.itemgetter(1),
                                         reverse=True)
             token2count = collections.OrderedDict(sorted_token2count)
 
             for token, token_count in token2count.items():
-                if token not in vocab2idx and token_count >= self.min_count:
-                    vocab2idx[token] = len(vocab2idx)
-            self.token2idx = vocab2idx
+                if token not in token2idx and token_count >= self.min_count:
+                    token2idx[token] = len(token2idx)
+            self.token2idx = token2idx
             self.idx2token = dict([(v, k) for k, v in self.token2idx.items()])
 
             top_k_vocab = [k for (k, v) in list(self.token2idx.items())[:10]]
             logger.debug(f"--- Build vocab dict finished, Total: {len(self.token2idx)} ---")
             logger.debug(f"Top-10: {top_k_vocab}")
-    def transform(self, samples):
+
+    def transform(self,
+                  samples: TextSamplesVar,
+                  *,
+                  seq_length: int = None,
+                  max_position: int = None,
+                  segment: bool = False) -> np.ndarray:
+        seq_length_from = ""
+
+        # An ugly patch for tf-serving use case.
+        if seq_length is None and self._sequence_length_from_saved_model is not None:
+            seq_length = self._sequence_length_from_saved_model
+
+        if seq_length is None:
+            seq_length_from = "max length of the samples"
+            seq_length = max([len(i) for i in samples]) + 2
+        if max_position is not None and max_position < seq_length:
+            seq_length_from = "max embedding seq length"
+            seq_length = max_position
+
+        if seq_length_from and not self._showed_seq_len_warning:
+            logger.warning(
+                f'Sequence length is None, will use the {seq_length_from}, which is {seq_length}')
+            self._showed_seq_len_warning = True
+
         numerized_samples = []
         for seq in samples:
-            if self.index is not None:
-                seq = seq[self.index]
-
-                if self.token_bos in self.token2idx:
-                    seq = [self.token_bos] + seq + [self.token_eos]
-                else:
-                    seq = [self.token_pad] + seq + [self.token_pad]
+            if self.token_bos in self.token2idx:
+                seq = [self.token_bos] + seq + [self.token_eos]
+            else:
+                seq = [self.token_pad] + seq + [self.token_pad]
             if self.token_unk in self.token2idx:
                 unk_index = self.token2idx[self.token_unk]
                 numerized_samples.append([self.token2idx.get(token, unk_index) for token in seq])
             else:
                 numerized_samples.append([self.token2idx[token] for token in seq])
 
-        sample_index = pad_sequences(numerized_samples, self.seq_length, padding='post', truncating='post')
-        token_ids = sample_index
+        sample_index = pad_sequences(numerized_samples, seq_length, padding='post', truncating='post')
+        token_ids = np.array(sample_index)
 
-        return token_ids
+        if segment:
+            segment_ids = np.zeros(token_ids.shape, dtype=np.int32)
+            return token_ids, segment_ids
+        else:
+            return token_ids
 
-    def inverse_transform(self, labels, *, lengths=None, threshold=0.5, **kwargs):
+    def inverse_transform(self,  # type: ignore[override]
+                          labels: Union[List[List[int]], np.ndarray],
+                          *,
+                          lengths: List[int] = None,
+                          threshold: float = 0.5,
+                          **kwargs: Any) -> List[List[str]]:
         result = []
         for index, seq in enumerate(labels):
             labels_ = []
-
             for idx in seq:
                 labels_.append(self.idx2token[idx])
             if lengths is not None:
-                labels_ = labels_[0:lengths[index]]
-
+                labels_ = labels_[1:lengths[index] + 1]
+            else:
+                labels_ = labels_[1:-1]
             result.append(labels_)
         return result
 
 
 if __name__ == "__main__":
     pass
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## kolibri/optimizers/optuna/objective.py

```diff
@@ -188,29 +188,33 @@
             if self.sampling_ratio is not None:
                 X_train, X_test, y_train, y_test = train_test_split(self.X, self.y, test_size = 0.3)
 
             else:
                 X_train, y_train=self.X, self.y
 
             results= pipeline.fit(X_train, y_train)
-            # pred=pipeline.predict(X_test)
-            # if self.estimator.estimator.task_type==TaskType.CLASSIFICATION:
-            #     pred=[p['name'] for p in pred['label']]
+            if self.eval_metric.display_name in results[0].to_dict():
+                score = results[0].to_dict()[self.eval_metric.display_name]['Mean']
+            else:
+                pred=pipeline.predict(X_test)
+                if self.estimator.estimator.task_type==TaskType.CLASSIFICATION:
+                    pred=[p['name'] for p in pred['label']]
+
 
 
+                score = self.eval_metric(y_test, pred)
 
-            score = results[0].to_dict()['F1']['Mean']#self.eval_metric(y_test, pred)
             if not self.eval_metric.greater_is_better:
                 score *= -1.0
 
         except optuna.exceptions.TrialPruned as e:
             raise e
         except Exception as e:
             print("Exception in EstimatorObjective", str(e))
-            if self.eval_metric.greater_is_better:
+            if not self.eval_metric.greater_is_better:
                 return -100000
             else:
                 return 100000
 
 
         return score
 
@@ -220,10 +224,16 @@
                 keys=key.split(".")
                 if len(keys)>1 and keys[0]=='model':
                     for name, component in self.parameters.items():
                         if 'model' in component["tunable"]:
                             for param_name, param in component["tunable"]["model"]["value"]["parameters"].items():
                                 if param_name==keys[1]:
                                     component["tunable"]["model"]["value"]["parameters"][param_name]["value"]=best[key]
+                else:
+                    for name, component in self.parameters.items():
+                        for param_name, param in component["tunable"].items():
+                            if param_name==keys[0]:
+                                component["tunable"][param_name]["value"]=best[key]
+
 
 
         return self.parameters
```

## kolibri/optimizers/optuna/tuner.py

```diff
@@ -10,15 +10,15 @@
 except:
     has_optuna=False
     pass
 
 from kdmt.file import create_dir
 from kolibri.evaluation.metrics import get_metric
 from kolibri.config import TaskType
-from optuna.integration.mlflow import MLflowCallback
+
 class OptunaTuner:
     def __init__(
         self,
         results_path,
         eval_metric,
         time_budget=3600,
         init_params={},
@@ -70,23 +70,23 @@
                 pruner=SuccessiveHalvingPruner()
             )
         study.enqueue_trial(objective.get_optuna_parameters(defaults))
 #        study.enqueue_trial(defaults)
 
         callbacks=[]
 
-        study.optimize(objective, timeout=self.time_budget, n_jobs=-1, callbacks=callbacks)
+        study.optimize(objective, timeout=self.time_budget, n_jobs=self.n_jobs, callbacks=callbacks)
 
         joblib.dump(study, os.path.join(self.study_dir, str(algorithm) + ".joblib"))
 
         best = study.best_params
 
         self.save()
 
-        return objective.update_parameters( best)
+        return objective.update_parameters(best)
 
 
     def save(self):
         with open(self.tuning_fname, "w", encoding='utf-8') as fout:
             fout.write(json.dumps(self.tuning, indent=4))
 
     def load(self):
```

## kolibri/preprocess/tabular/__init__.py

```diff
@@ -1,20 +1,22 @@
 from kolibri.preprocess.tabular.dummy_converter import DummyConverter
 from kolibri.preprocess.tabular.normalize import Normalizer
 from kolibri.preprocess.tabular.infer_datatype import AutoInferDatatype
 from kolibri.preprocess.tabular.preprocessing_pipeline import DataPreprocessingPipeline
 from kolibri.preprocess.tabular.reduce_dimensionality import DimensionalityReduction
-from kolibri.preprocess.tabular.multicollinearity import Fix_multicollinearity
+from kolibri.preprocess.tabular.multicollinearity import Multicollinearity
 from kolibri.preprocess.tabular.outlier_remover import Outlier
 from kolibri.preprocess.tabular.cluster import ClusterDataset
 from kolibri.preprocess.tabular.feature_selection import Boruta_Feature_Selection, Advanced_Feature_Selection_Classic
 from kolibri.preprocess.tabular.time_features_extractor import TimeFeatures
 from kolibri.preprocess.tabular.ordinal_transformer import Ordinal
 from kolibri.preprocess.tabular.binning import Binning
 from kolibri.preprocess.tabular.reduce_cardinality import Reduce_Cardinality_with_Counts, Reduce_Cardinality_with_Clustering
 from kolibri.preprocess.tabular.rare_levels import Catagorical_variables_With_Rare_levels
 from kolibri.preprocess.tabular.zero_variance_remover import NearZeroVariance
 from kolibri.preprocess.tabular.data_imputer import IterativeImputer, DataImputer
-from kolibri.preprocess.tabular.feature_interaction import Advanced_Feature_Selection_Classic, DFS_Classic
+from kolibri.preprocess.tabular.feature_interaction import Advanced_Feature_Selection_Classic, FeaturesInteractions
 from kolibri.preprocess.tabular.one_hot_encoder_multi import MultiColomnOneHotEncoder
 from kolibri.preprocess.tabular.similar_features import Group_Similar_Features
-from kolibri.preprocess.tabular.columns_transfromer import PandasColumnTransformer
+from kolibri.preprocess.tabular.columns_transfromer import PandasColumnTransformer
+from kolibri.preprocess.tabular.category_transformer import CategoryEncoder
+from kolibri.preprocess.tabular.columns_remover import PandasColumnRemover
```

## kolibri/preprocess/tabular/columns_transfromer.py

```diff
@@ -1,24 +1,27 @@
 from kolibri.core.component import Component
-from sklearn.impute._base import _BaseImputer, SimpleImputer
-import numpy as np
-import pandas as pd
-from copy import deepcopy
-from kolibri.utils.common import prepare_names_for_json
-from kolibri.preprocess.tabular.dummy_converter import DummyConverter
-from kolibri.preprocess.tabular.time_features_extractor import TimeFeatures
-from sklearn.preprocessing import LabelEncoder
-import gc
+from kolibri.registry import register
 
+@register('PandasColumnTransformer')
 class PandasColumnTransformer(Component):
 
     defaults = {
         "fixed":{
             "formulas": None,
             "new-column-names": None
+        },
+        "tuneable":{
+            "drop-source-columns":{
+                "value": False,
+                "type": "boolean",
+                "values": [
+                    True,
+                    False
+                ]
+            }
         }
 
     }
 
 
     def __init__(self, params={}):
         super().__init__(params)
```

## kolibri/preprocess/tabular/dummy_converter.py

```diff
@@ -64,9 +64,9 @@
         else:
             return data
 
     def fit_transform(self, data, y=None):
         return self.fit(data, y).transform(data, y)
 
 
-from kolibri.registry import ModulesRegistry
-ModulesRegistry.add_module(DummyConverter.name, DummyConverter)
+#from kolibri.registry import ModulesRegistry
+#ModulesRegistry.add_module(DummyConverter.name, DummyConverter)
```

## kolibri/preprocess/tabular/feature_interaction.py

```diff
@@ -2,15 +2,15 @@
 from kolibri.config import TaskType
 import numpy as np
 import pandas as pd
 from kolibri.preprocess.tabular.feature_selection import Advanced_Feature_Selection_Classic
 
 # _______________________________________________________________________________________________________________________________________________________________________________________________
 # custome DFS
-class DFS_Classic(Component):
+class FeaturesInteractions(Component):
     """
     - Automated feature interactions using multiplication, division , addition & substraction
     - Only accepts numeric / One Hot Encoded features
     - Takes DF, return same DF
     - for Multiclass classification problem , set subclass arg as 'multi'
   """
 
@@ -138,30 +138,35 @@
             dummy_all[self.target] = dataset[self.target]
         return dummy_all
 
     def fit_transform(self, dataset, y=None):
 
         data = dataset
 
-        data_without_target = data.drop(self.target, axis=1, errors="ignore")
-
+        if self.target is not None:
+            data_without_target = data.drop(self.target, axis=1, errors="ignore")
+        else:
+            data_without_target=dataset
         # we need to seperate numerical and ont hot encoded columns
         # self.ohe_columns = [i if ((len(data[i].unique())==2) & (data[i].unique()[0] in [0,1]) & (data[i].unique()[1] in [0,1]) ) else None for i in data.drop(self.target,axis=1).columns]
         self.ohe_columns = [
             i
             for i in data.columns
             if data[i].nunique() == 2
             and data[i].unique()[0] in [0, 1]
             and data[i].unique()[1] in [0, 1]
         ]
         # self.ohe_columns = [i for i in self.ohe_columns if i is not None]
         self.numeric_columns = [
             i for i in data_without_target.columns if i not in self.ohe_columns
         ]
-        target_variable = data[[self.target]]
+        if y is not None:
+            target_variable=y
+        else:
+            target_variable = data[[self.target]]
 
         # for multiplication:
         # we need bot catagorical and numerical columns
 
         if "multiply" in self.interactions:
             data_multiply = pd.concat(
                 [
@@ -289,35 +294,42 @@
             (data_multiply, data_divide, data_add, data_substract), axis=1
         )
         del data_multiply
         del data_divide
         del data_add
         del data_substract
 
+        if self.target is None:
+            self.target="__target__"
         dummy_all[self.target] = target_variable
         self.dummy_all = dummy_all
 
         # apply advanced feature selection
-        afs = Advanced_Feature_Selection_Classic(
-            target=self.target,
-            ml_usecase=self.ml_usecase,
-            top_features_to_pick=self.top_n_correlated,
-            random_state=self.random_state,
-            subclass=self.subclass,
-            n_jobs=self.n_jobs,
+        afs = Advanced_Feature_Selection_Classic(configs={
+            "target":self.target,
+            "task-type":self.ml_usecase,
+            "top_features_to_pick":self.top_n_correlated,
+            "random_state":self.random_state,
+            "subclass":self.subclass,
+            "n_jobs":self.n_jobs,}
         )
         dummy_all_t = afs.fit_transform(dummy_all)
 
         data_fe_final = pd.concat(
             (data, dummy_all_t), axis=1
         )  # self.data_fe[self.corr]
         # # making sure no duplicated columns are there
         data_fe_final = data_fe_final.loc[
             :, ~data_fe_final.columns.duplicated()
         ]  # new added
         # # remove thetarget column
         # # this is the final data we want that includes original , fe data plus impact of top n correlated
+
         self.columns_to_keep = data_fe_final.drop(self.target, axis=1).columns
         del dummy_all
         del dummy_all_t
 
+
+        if y is not None and self.target=='__target__':
+            data_fe_final=data_fe_final.drop(self.target, axis=1)
+
         return data_fe_final
```

## kolibri/preprocess/tabular/feature_selection.py

```diff
@@ -1,21 +1,20 @@
 from kolibri.core.component import Component
 from kolibri.config import TaskType
 from sklearn.ensemble import RandomForestClassifier as rfc
 from sklearn.ensemble import RandomForestRegressor as rfr
 try:
-    from lightgbm import LGBMClassifier as lgbmc
-    from lightgbm import LGBMRegressor as lgbmr
+    import lightgbm
 except:
     pass
 
 
 import numpy as np
 import pandas as pd
-
+from kdmt.lib import install_and_import, is_module_installed
 # ______________________________________________________________________________________________________________________________________________________
 # Feature Selection
 class Advanced_Feature_Selection_Classic(Component):
     """
     - Selects important features and reduces the feature space. Feature selection is based on Random Forest , Light GBM and Correlation
     - to run on multiclass classification , set the subclass argument to 'multi'
   """
@@ -34,14 +33,17 @@
 
         self.target = self.get_parameter("target")
         self.ml_usecase = self.get_parameter("task-type")
         self.top_features_to_pick = 1 - self.get_parameter("top-features-to-pick")
         self.random_state = self.get_parameter("random-state")
         self.subclass = self.get_parameter("subclass")
         self.n_jobs = self.get_parameter("n_jobs")
+        if not is_module_installed("lightgbm"):
+            lightgbm=install_and_import("lightgbm")
+
 
     def fit(self, dataset, y=None):
         self.fit_transform(dataset, y=y)
         return self
 
     def transform(self, dataset, y=None):
         # return the data with onlys specific columns
@@ -98,23 +100,23 @@
         max_fe = min(70, int(np.sqrt(len(dummy_all.columns))))
         max_sa = min(
             float(1000 / len(dummy_all)),
             float(np.sqrt(len(dummy_all) / len(dummy_all))),
         )
 
         if self.ml_usecase == "classification":
-            m = lgbmc(
+            m = lightgbm.LGBMClassifier(
                 n_estimators=100,
                 max_depth=5,
                 n_jobs=self.n_jobs,
                 subsample=max_sa,
                 random_state=self.random_state,
             )
         else:
-            m = lgbmr(
+            m = lightgbm.LGBMRegressor(
                 n_estimators=100,
                 max_depth=5,
                 n_jobs=self.n_jobs,
                 subsample=max_sa,
                 random_state=self.random_state,
             )
         m.fit(dummy_all.drop(self.target, axis=1), dummy_all[self.target])
```

## kolibri/preprocess/tabular/infer_datatype.py

```diff
@@ -1,25 +1,29 @@
 from kolibri.core.component import Component
 import numpy as np
 import pandas as pd
 from ast import literal_eval
+from kolibri.registry import register
 
-
+@register('AutoInferDatatype')
 class AutoInferDatatype(Component):
     """
     - This will try to automatically infer data types .
     - also clean target varioables and remove columns where all the values are null
   """
 
     defaults = {
         "fixed":{
             "target": None,
             "task": "classification",
             "categorical-features":[],
             "eval-literal":True,
+            "drop-na":False,
+            "drop-id-column": True,
+            "guess-id-columns":False,
             "numerical-features": [],
             "date-features": [],
             "features-to-drop":[]
         },
         "tunable":
             {
             }
@@ -45,14 +49,31 @@
         """
     Args:
       data: accepts a pandas data frame
     Returns:
       Panda Data Frame
     """
 
+        if self.id_columns ==[] and self.get_parameter("guess-id-columns"):
+            for col in data.columns:
+                if self.is_id_column(data[col]):
+                    self.id_columns.append(col)
+        return self
+
+
+    def is_id_column(self, col_values: pd.Series):
+        return len(col_values.unique())==len(col_values)
+    def transform(self, data, y=None):
+        """
+      Args:
+        data: accepts a pandas data frame
+      Returns:
+        Panda Data Frame
+    """
+
         # drop any columns that were asked to drop
         if self.features_todrop:
             data.drop(columns=self.features_todrop, errors="ignore", inplace=True)
 
         # if there are inf or -inf then replace them with NaN
         data.replace([np.inf, -np.inf], np.NaN, inplace=True)
 
@@ -84,35 +105,31 @@
 
         # table of learned types
         self.learned_dtypes = data.dtypes
         # self.training_columns = data.drop(self.target,axis=1).columns
 
         # remove columns with duplicate name
         data = data.loc[:, ~data.columns.duplicated()]
-        # Remove NAs
-        data.dropna(axis=0, how="all", inplace=True)
-        data.dropna(axis=1, how="all", inplace=True)
-        # remove the row if target column has NA
-        try:
-            data.dropna(subset=[self.target], inplace=True)
-        except KeyError:
-            pass
+
 
         # drop id columns
         data.drop(self.id_columns, axis=1, errors="ignore", inplace=True)
 
         return data
 
-    def transform(self, dataset, y=None):
-        """
-      Args:
-        data: accepts a pandas data frame
-      Returns:
-        Panda Data Frame
-    """
-
-        return self.fit(dataset, y)
 
     # fit_transform
-    def fit_transform(self, dataset, y=None):
+    def fit_transform(self, data, y=None):
+
+        self.fit(data, y)
+        self.transform(data, y)
+        # Remove NAs
+        if self.get_parameter("drop-na"):
+            data.dropna(axis=0, how="all", inplace=True)
+            data.dropna(axis=1, how="all", inplace=True)
+            # remove the row if target column has NA
+            try:
+                data.dropna(subset=[self.target], inplace=True)
+            except KeyError:
+                pass
 
-        return self.fit(dataset, y)
+        return data
```

## kolibri/preprocess/tabular/multicollinearity.py

```diff
@@ -1,13 +1,14 @@
 from kolibri.core.component import Component
 import numpy as np
 import pandas as pd
+from copy import copy
 
 # _________________________________________________________________________________________________________________________________________
-class Fix_multicollinearity(Component):
+class Multicollinearity(Component):
     """
           Fixes multicollinearity between predictor variables , also considering the correlation between target variable.
           Only applies to regression or two class classification ML use case
           Takes numerical and one hot encoded variables only
             Args:
               threshold (float): The utmost absolute pearson correlation tolerated beyween featres from 0.0 to 1.0
               target_variable (str): The target variable/column name
@@ -32,35 +33,41 @@
         self.target_variable = self.get_parameter("target")
         self.correlation_with_target_threshold = self.get_parameter("correlation-with-target-threshold")
         self.target_corr_weight = self.get_parameter("correlation_with_target_preference")
         self.multicol_weight = 1 - self.get_parameter("correlation_with_target_preference")
 
     # Make fit method
 
-    def fit(self, data, y=None):
+    def fit(self, data_, y=None):
         """
         Args:
             data = takes preprocessed data frame
         Returns:
             None
         """
 
-        if data[self.target_variable].dtype not in ["int32", "int64", "float32", "float64"]:
+        data=copy(data_)
+        if self.target_variable==None:
+            self.target_variable='target'
+        data[self.target_variable]=y
+        data[self.target_variable]=data[self.target_variable].convert_dtypes()
+
+        if data[self.target_variable].dtype.name.lower() not in ["int32", "int64", "float32", "float64"]:
             raise ValueError('dtype for the target variable should be int32, int64, float32, or float64 only')
 
         # global data1
         data1 = data.select_dtypes(include=["int32", "int64", "float32", "float64"])
         # try:
         #   self.data1 = self.data1.astype('float16')
         # except:
         #   None
         # make an correlation db with abs correlation db
         # self.data_c = self.data1.T.drop_duplicates()
         # self.data1 = self.data_c.T
-        corr = pd.DataFrame(np.corrcoef(data1.T))
+        corr = pd.DataFrame(np.corrcoef(data1.T.astype(float)))
         corr.columns = data1.columns
         corr.index = data1.columns
         # corr_matrix = abs(data1.corr())
         corr_matrix = abs(corr)
 
         # for every diagonal value, make it Nan
         corr_matrix.values[
@@ -199,15 +206,15 @@
         except:
             pass
 
         # now we want to keep only the columns that have more correlation with traget by a threshold
         self.to_drop_taret_correlation = []
         if self.correlation_with_target_threshold != 0.0:
             corr = pd.DataFrame(
-                np.corrcoef(data.drop(self.to_drop, axis=1).T),
+                np.corrcoef(data.drop(self.to_drop, axis=1).T.astype(float)),
                 columns=data.drop(self.to_drop, axis=1).columns,
                 index=data.drop(self.to_drop, axis=1).columns,
             )
             self.to_drop_taret_correlation = corr[self.target_variable].abs()
             # to_drop_taret_correlation = data.drop(self.to_drop,axis=1).corr()[target_variable].abs()
             self.to_drop_taret_correlation = self.to_drop_taret_correlation[
                 self.to_drop_taret_correlation < self.correlation_with_target_threshold
@@ -239,15 +246,15 @@
 
         """
         Args:
             data = takes preprocessed data frame
         Returns:
             data frame
     """
-        self.fit(data)
+        self.fit(data, y)
         return self.transform(data)
 
 class Fix_Perfect_collinearity(Component):
     """
     - Takes DF, return data frame while removing features that are perfectly correlated (droping one)
   """
```

## kolibri/preprocess/tabular/normalize.py

```diff
@@ -3,18 +3,18 @@
 from sklearn.preprocessing import MinMaxScaler
 from sklearn.preprocessing import MaxAbsScaler
 from sklearn.preprocessing import QuantileTransformer
 from sklearn.preprocessing import RobustScaler
 from kolibri.utils.log_normalizer import LogNormaliser
 import pandas as pd
 import numpy as np
+from kolibri.registry import register
 
 
-
-
+@register('Normalizer')
 class Normalizer(Component):
     defaults = {
         "fixed":{
             "normalization-method": "zscore",
             "random-state-quantile":42,
             "ignore-columns":[],
             "include-columns":"all",
@@ -111,9 +111,9 @@
 
     def inverse_transform_col(self, data, colName):
         dummy = pd.DataFrame(np.zeros((len(data), len(self.numeric_features))), columns=self.numeric_features)
         dummy[colName] = data
         dummy = pd.DataFrame(self.inverse_transform(dummy), columns=self.numeric_features)
         return dummy[colName].values
 
-from kolibri.registry import ModulesRegistry
-ModulesRegistry.add_module(Normalizer.name, Normalizer)
+#from kolibri.registry import ModulesRegistry
+#ModulesRegistry.add_module(Normalizer.name, Normalizer)
```

## kolibri/preprocess/tabular/one_hot_encoder_multi.py

```diff
@@ -32,15 +32,15 @@
             OneHotEncoder.fit(np.array(data.loc[:, col]).reshape(-1, 1))
             self.__MultiOHE[col] = OneHotEncoder
             self.encoded_dict[col]=self.grt_new_col_names(col, OneHotEncoder)
         return self
 
 
     def grt_new_col_names(self, col,  ohe):
-        return [str(col) + '_' + str(c) for c in ohe.get_feature_names()]
+        return [str(col) + '_' + str(c) for c in ohe.get_feature_names_out()]
     def transform(self, data):
 
         ##
 
         if self.__catColumns==[]:
             return data
         catData = data[self.__catColumns]
```

## kolibri/preprocess/tabular/preprocessing_pipeline.py

```diff
@@ -1,49 +1,44 @@
-import datetime
-import gc
-import os
-import sys
 import time
-import traceback
+import time
 import warnings
-from copy import deepcopy
-from kolibri.utils.common import infer_task_type
-from kolibri.core.pipeline import Pipeline
-from kolibri.core.component import Component
+
 import numpy as np
 import pandas as pd
-from kolibri.preprocess.tabular.infer_datatype import AutoInferDatatype
-from kolibri.preprocess.tabular.data_imputer import DataImputer, IterativeImputer
-from kolibri.preprocess.tabular.zero_variance_remover import NearZeroVariance
-from kolibri.preprocess.tabular.rare_levels import Catagorical_variables_With_Rare_levels
-from kolibri.preprocess.tabular.reduce_cardinality import Reduce_Cardinality_with_Counts, Reduce_Cardinality_with_Clustering
-from kolibri.preprocess.tabular.ordinal_transformer import Ordinal
+from kdmt.dict import update
+from kolibri.registry import register
+from kolibri.config import TaskType
+from kolibri.core.component import Component
+from kolibri.core.pipeline import Pipeline
+from kolibri.logger import get_logger
 from kolibri.preprocess.tabular.binning import Binning
-from kolibri.preprocess.tabular.normalize import Normalizer
-from kolibri.preprocess.tabular.time_features_extractor import TimeFeatures
-from kolibri.preprocess.tabular.dummy_converter import DummyConverter
-from kolibri.preprocess.tabular.outlier_remover import Outlier
 from kolibri.preprocess.tabular.cluster import ClusterDataset
+from kolibri.preprocess.tabular.data_imputer import DataImputer, IterativeImputer
+from kolibri.preprocess.tabular.dummy_converter import DummyConverter
 from kolibri.preprocess.tabular.feature_selection import Boruta_Feature_Selection, Advanced_Feature_Selection_Classic
-from kolibri.preprocess.tabular.multicollinearity import Fix_multicollinearity, Fix_Perfect_collinearity
+from kolibri.preprocess.tabular.infer_datatype import AutoInferDatatype
+from kolibri.preprocess.tabular.multicollinearity import Multicollinearity, Fix_Perfect_collinearity
+from kolibri.preprocess.tabular.normalize import Normalizer
+from kolibri.preprocess.tabular.ordinal_transformer import Ordinal
+from kolibri.preprocess.tabular.outlier_remover import Outlier
+from kolibri.preprocess.tabular.rare_levels import Catagorical_variables_With_Rare_levels
+from kolibri.preprocess.tabular.reduce_cardinality import Reduce_Cardinality_with_Counts, \
+    Reduce_Cardinality_with_Clustering
 from kolibri.preprocess.tabular.reduce_dimensionality import DimensionalityReduction
-from kolibri.config import TaskType
-from kolibri.logger import get_logger
-from kolibri.core.pipeline import Pipeline
-from kdmt.dict import update
+from kolibri.preprocess.tabular.time_features_extractor import TimeFeatures
+from kolibri.preprocess.tabular.zero_variance_remover import NearZeroVariance
 
 warnings.filterwarnings("ignore")
 
 _available_plots = {}
 
 
 logger=get_logger(__name__)
 
-
-
+@register('DataPreprocessingPipeline')
 class DataPreprocessingPipeline(Pipeline, Component):
     defaults = {
         "fixed":{
             "categorical-features":[],
             "categorical-iterative-imputer": "lightgbm",
             "numerical-features" : [],
             "ordinal-features": [],
@@ -257,17 +252,17 @@
                 feature_select = Advanced_Feature_Selection_Classic(self.hyperparameters)
 
 
         # removing multicollinearity
         fix_multi=None
         if self.get_parameter("remove-multicollinearity") == True:
             if self.ml_task !=TaskType.MULTI_TARGET_CLASSIFICATION and self.ml_task !=TaskType.MULTI_TARGET_REGRESSION:
-                fix_multi = Fix_multicollinearity(self.hyperparameters)
+                fix_multi = Multicollinearity(self.hyperparameters)
             else:
-                fix_multi = Fix_multicollinearity(self.hyperparameters)
+                fix_multi = Multicollinearity(self.hyperparameters)
 
 
         # remove 100% collinearity
         fix_perfect=None
         if self.get_parameter("remove-perfect-collinearity") == True:
             fix_perfect = Fix_Perfect_collinearity(self.hyperparameters)
 
@@ -501,9 +496,9 @@
         experiment__.append(("Transformation Pipeline", prep_pipe))
 
         # end runtime
         runtime_end = time.time()
         runtime = np.array(runtime_end - runtime_start).round(2)
 
 
-from kolibri.registry import ModulesRegistry
-ModulesRegistry.add_module(DataPreprocessingPipeline.name, DataPreprocessingPipeline)
+#from kolibri.registry import ModulesRegistry
+#ModulesRegistry.add_module(DataPreprocessingPipeline.name, DataPreprocessingPipeline)
```

## kolibri/preprocess/text/collocation_analyzer.py

```diff
@@ -1,23 +1,22 @@
 import os
-from typing import List
-from typing import Text
+
 
 import joblib
 from gensim.models import Phrases
-
+from kolibri.registry import register
 from kolibri.core.component import Component
 from kolibri.logger import get_logger
 from kdmt.file import save_to_disk, load_from_disk
 
 logger = get_logger(__name__)
 
 BIGRAM_FILENAME = "kolibri-bigram.model"
 
-
+@register('CollocationAnalyzer')
 class CollocationAnalyzer(Component):
 
     _estimator_type = 'estimator'
 
     provides = ["ngram"]
 
     requires = ["text_features"]
@@ -134,11 +133,7 @@
         return {
             "bigram_file": BIGRAM_FILENAME
         }
 
     def get_info(self):
         return "brigram analyzer"
 
-
-
-from kolibri.registry import ModulesRegistry
-ModulesRegistry.add_module(CollocationAnalyzer.name, CollocationAnalyzer)
```

## kolibri/preprocess/text/cleaning/email2text.py

```diff
@@ -174,14 +174,15 @@
 class Fragment(object):
     """ A Fragment is a part of
         an Email Message, labeling each part.
     """
 
     def __init__(self, email_text, salutations, regex_header, collated_text=False, parse_dates=False):
         self.collated_text=collated_text
+        self.parse_dates=parse_dates
         self.salutations = salutations
         self.body = email_text.strip()
         self.regex_header = regex_header
         self.is_forwarded_message = self._get_forwarded()
         self.is_out_of_office=False
         self.is_rejected=False
         self.subject = None
@@ -192,15 +193,15 @@
         if self.subject is None and not self.collated_text:
             self.subject = self._get_title()
         self.attachement = self._get_attachement()
         self.salutation = self._get_salutation()
         self.disclaimer = self._get_disclaimer()
         self.signature = self._get_signature()
         self._content = email_text
-        self.parse_dates=parse_dates
+
 
     def _get_title(self):
         patterns = [
             "(R[Ee]|Antw\.:|F[Ww])\s?:\s?.+",
             ".*\s+(?=(Hi|Hello|Dear))"
         ]
```

## kolibri/preprocess/timeseries/multi_window_generator.py

```diff
@@ -2,15 +2,15 @@
 import pandas as pd
 import numpy as np
 import datetime
 import matplotlib.pyplot as plt
 from kolibri.core.component import Component
 import tensorflow as tf
 from kolibri.utils.timeseries_functions import roll_time_series
-from tensorflow.keras.preprocessing.sequence import pad_sequences
+#from tensorflow.keras.preprocessing.sequence import pad_sequences
 
 
 class MultiWindowGenerator(Component):
     """Base class for sliding and expanding window splitter."""
 
     defaults = {
         "fixed": {
@@ -28,18 +28,18 @@
             "horizon": 1,
             "n_jobs": 4,
             "sets": ["val", "test"],  # or "predict"
             "main-period": -1
         },
         "tunable": {
             "min-window-history": {
-                "value": 4
+                "value": 1
             },
             "max-window-history": {
-                "value": 8
+                "value": 4
             }
         }
 
     }
 
     def __init__(self, data, configs={}):
         super(MultiWindowGenerator, self).__init__(configs)
@@ -83,16 +83,16 @@
         self.labels_slice = slice(self.label_start, None)
         self.label_indices = np.arange(self.total_window_size)[self.labels_slice]
         self._roll_data()
         if set(self._split_sets) <= set(["val", "test"]):
             self.split_train_test_val()
         elif self._split_sets ==["predict"]:
             self.get_main_set()
-        if self.column_indices is None:
-            columns = [col for col in self._train_df.columns if col not in self._extra_columns]
+        if self.column_indices is None and len(self._train_df)>0:
+            columns = [col for col in self._train_df[0].columns if col not in self._extra_columns]
             if self._train_df is not None:
                 self.column_indices = {name: i for i, name in
                                        enumerate(columns)}
 
     def __repr__(self):
         return '\n'.join([
             f'Total window size: {self.total_window_size}',
@@ -149,37 +149,41 @@
             self.data = self.data.fillna(0)
 
         self.df_rolled = roll_time_series(self.data, column_id=self.get_parameter("group"),
                                           column_sort=self.get_parameter("timestamp"),
                                           n_jobs=self.get_parameter("n_jobs"),
                                           max_timeshift=self.get_parameter("max-window-history") + self.horizon - 1,
                                           min_timeshift=self.get_parameter(
-                                              "min-window-history") + self.horizon - 1).drop(
-            columns=[self.get_parameter("group"), self.get_parameter("timestamp")])
+                                              "min-window-history") + self.horizon - 1)
+#        df_rolled=[df.drop(
+#            columns=[self.get_parameter("group"), self.get_parameter("timestamp")]) for df in df_rolled]
 
-        self.df_rolled[['id_group', 'id_sort']] = pd.DataFrame(self.df_rolled['id'].tolist(),
-                                                               index=self.df_rolled.index)
 
+        for df in self.df_rolled:
+            df.drop(columns=[self.get_parameter("group"), self.get_parameter("timestamp")], inplace=True)
+            df[['id_group', 'id_sort']]=pd.DataFrame(df['id'].tolist(),index=df.index)
+
+        return
     def split_train_test_val(self):
         timestamps = sorted(self.data[self.get_parameter("timestamp")].unique())
         valid_timestamp=None
         test_timestamp=None
 
 
         if "val" in self._split_sets:
             valid_timestamp = timestamps[-(self._split_sets.index("val")+2)]
-            self._valid_df = self.df_rolled[self.df_rolled["id_sort"] == valid_timestamp]
+            self._valid_df = [df[df["id_sort"] == valid_timestamp] for df in self.df_rolled if len(df[df["id_sort"] == valid_timestamp])>0]
 
         if "test" in self._split_sets:
             test_timestamp = timestamps[-(self._split_sets.index("test"))]
-            self._test_df = self.df_rolled[self.df_rolled["id_sort"] == test_timestamp]
+            self._test_df =[df[df["id_sort"] == test_timestamp] for df in self.df_rolled if len(df[df["id_sort"] == test_timestamp])>0]
 
         if valid_timestamp or test_timestamp:
             train_timestamp=min(value for value in [valid_timestamp, test_timestamp] if value is not None)
-            self._train_df = self.df_rolled[self.df_rolled["id_sort"] < train_timestamp]
+            self._train_df = [df[df["id_sort"] < train_timestamp] for df in self.df_rolled if len(df[df["id_sort"] < train_timestamp])>0]
         else:
             self._train_df = self.df_rolled
 
     def get_main_set(self):
         main_period=self.get_parameter("main-period")
         timestamps = sorted(self.data[self.get_parameter("timestamp")].unique())
 
@@ -189,38 +193,40 @@
                 if abs(main_period)>=len(timestamps):
                     raise Exception("The Index of the target period, " + str(main_period) + " is greater the number of periods of the dataset, (" + str(len(timestamps)) + "periods)")
                 main_timestamp=timestamps[main_period]
             elif isinstance(main_period, datetime.datetime):
                 main_timestamp=main_period
             else:
                 raise Exception("Wrong 'main-period' format. Should be either an integer or a datatime.")
-        self._train_df = self.df_rolled[self.df_rolled["id_sort"] == main_timestamp]
+        self._train_df = [df[df["id_sort"] == main_timestamp] for df in self.df_rolled]
 
      #   self._train_df = self.df_rolled[main_timestamp]
 
     def _get_array_values(self, ds, drop_ids=None):
 
-        values = ds.groupby(["id", "id_sort"])
+#        values = ds.groupby(["id", "id_sort"])
         colums_to_drop = ["id", "id_sort", "id_group"]
         dtypes = 'float32'
         if drop_ids is not None:
             colums_to_drop = drop_ids
             dtypes = 'object'
         if self.get_parameter('max-window-history') == self.get_parameter('min-window-history'):
-            values = np.array(
-                [values.get_group(group).drop(columns=colums_to_drop) for group in values.groups])
+            values = [d[1].drop(columns=colums_to_drop).values for df in ds for d in df.groupby(["id_group"])]
+
         else:
-            values = pad_sequences(np.array(
-                [values.get_group(group).drop(columns=colums_to_drop).values for group in values.groups]), dtype=dtypes)
+            values = [tf.keras.preprocessing.sequence.pad_sequences(
+                d[1].drop(columns=colums_to_drop).values.T, dtype=dtypes, padding='pre',
+                maxlen=self.get_parameter('max-window-history')+self.get_parameter('horizon'), value=0.0).T for df in ds for d in df.groupby(["id_group"])]
+
+            # values = [tf.keras.preprocessing.sequence.pad_sequences(
+            #     df.drop(columns=colums_to_drop).values.T, dtype=dtypes, padding='pre',
+            #     maxlen=self.get_parameter('max-window-history')+self.get_parameter('horizon'), value=0.0).T  for df in ds]
 
-        #            tf.keras.preprocessing.sequence.pad_sequences(
-        #                sequences, maxlen=None, dtype='int32', padding='pre',
-        #                truncating='pre', value=0.0
-        #            )
-        return values
+
+        return np.rollaxis(np.dstack(values), -1)
 
     @property
     def train(self):
 
         if not hasattr(self, "train_values"):
             self.train_values = self.split_window(self._get_array_values(self._train_df))
 
@@ -294,15 +300,15 @@
             # And cache it for next time
             self._example = result
 
         return result
 
     @property
     def train_df(self):
-        return self._train_df.drop(columns=["id", "id_sort", "id_group"])
+        return pd.concat([df.drop(columns=["id", "id_sort", "id_group"]) for df in self._train_df])
 
     @property
     def main_df(self):
         if hasattr(self, "main_df_"):
             return self.main_df_
         else:
             main_values = self._get_array_values(self._train_df, drop_ids=["id"])
@@ -364,7 +370,18 @@
             columns=[self.get_parameter("group"), self.get_parameter("timestamp")])
 
         self.df_predict[['id_group', 'id_sort']] = pd.DataFrame(self.df_rolled['id'].tolist(),
                                                                 index=self.df_rolled.index)
         predict_values = self.split_window(self._get_array_values(self.df_predict))
 
         return predict_values
+
+
+if __name__=="__main__":
+    data=pd.read_csv("/Users/mohamedmentis/Dropbox/Mac (2)/Documents/Mentis/Development/Projects/Alight/Eloise/us_data/20000_employees.csv")
+#    data=data.drop(columns=['Company_Id', 'Pay_Period', 'Pay_Group', 'Code_Status'])
+    data['Employee_Status'] = data['Employee_Status'].astype('category').cat.codes
+
+    configs={"timestamp": "Original_Start_Date", "target": ['Value'], "sets": ["predict"],  "group":'Employee_Id'}
+    mwg=MultiWindowGenerator(data, configs=configs)
+
+    print(mwg.train)
```

## kolibri/samplers/__init__.py

```diff
@@ -1,7 +1,10 @@
+from kolibri.samplers.conditional import ConditionalGenerator
+from kolibri.samplers.data_sampler import DataSampler
+
 from imblearn.combine import (
     SMOTEENN, SMOTETomek,
 )
 from imblearn.over_sampling import (
     SMOTE, ADASYN, BorderlineSMOTE,
 )
 from imblearn.under_sampling import (
```

## kolibri/task/__init__.py

```diff
@@ -1 +1,2 @@
 from kolibri.task.text import *
+from kolibri.task.tabular import *
```

## kolibri/task/audio/base_model.py

```diff
@@ -4,15 +4,15 @@
 from typing import Dict, Any
 
 import numpy as np
 # import tensorflow as tf
 from sklearn import metrics as sklearn_metrics
 
 import kolibri
-from kolibri.data.text.generators import DataGenerator
+from kolibri.data.text.generators_ import DataGenerator
 from kolibri.backend.tensorflow.tasks.base_model import TaskBaseModel
 from kolibri.backend.tensorflow.layers import L
 from kolibri.backend.tensorflow.utils import load_data_object
 from kolibri.logger import get_logger
 import tensorflow as tf
 logger = get_logger(__name__)
```

## kolibri/task/tabular/__init__.py

```diff
@@ -1 +1,2 @@
-from kolibri.task.tabular.clustering import ClusteringEstimator
+from kolibri.task.tabular.clustering import ClusteringEstimator
+from kolibri.task.tabular.regression.sklearn_regression_estimator import RegSklearnEstimator
```

## kolibri/task/tabular/clustering/clustering.py

```diff
@@ -2,21 +2,21 @@
 import numpy as np
 import warnings
 from kolibri.backend.base.base_classifier import BaseClassifier
 from kolibri.evaluation.clustering_evaluator import ClusteringEvaluator
 from kolibri.logger import get_logger
 import pandas as pd
 from kolibri.config import TaskType
-from kdmt.dict import update
+from kolibri.registry import register
 
 
 logger = get_logger(__name__)
 warnings.filterwarnings("ignore")
 MODEL_FILE_NAME="clustering_model.pkl"
-
+@register('ClusteringEstimator')
 class ClusteringEstimator(BaseClassifier):
 
     defaults={
         "fixed":{
             "log_plot": False,
             "n_clusters": 4,
             "round": 4,
@@ -131,9 +131,9 @@
         if os.path.exists(classifier_file):
             model = joblib.load(classifier_file)
 
             return model
         else:
             return cls(model_metadata)
 
-from kolibri.registry import ModulesRegistry
-ModulesRegistry.add_module(ClusteringEstimator.name, ClusteringEstimator)
+#from kolibri.registry import ModulesRegistry
+#ModulesRegistry.add_module(ClusteringEstimator.name, ClusteringEstimator)
```

## kolibri/task/tabular/regression/sklearn_regression_estimator.py

```diff
@@ -1,25 +1,26 @@
 import copy
 
 import joblib
 import pandas as pd
-
+from kolibri.registry import register
 from kolibri.backend.base.base_regressor import BaseRegressor
 from kdmt.dict import update
 
 try:
     from kolibri.optimizers.optuna.objective import EstimatorObjective
 except:
     pass
 
 from kolibri.logger import get_logger
 
 logger = get_logger(__name__)
 from kolibri.config import TaskType
 
+@register('RegSklearnEstimator')
 class RegSklearnEstimator(BaseRegressor):
     defaults = {"fixed": {
         "default-params": None,
         "task-type": TaskType.REGRESSION
     },
 
         "tunable": {
@@ -42,15 +43,15 @@
 
         if isinstance(X,pd.DataFrame):
             if self.get_parameter("target") in X.columns:
                 X=X.drop(self.get_parameter("target"), axis=1)
 
             self.feature_names=X.columns
 
-            X=X.to_numpy()
+#            X=X.to_numpy()
 
         model_results = super(RegSklearnEstimator, self).fit(X, y)
 
         return model_results
 
     def copy(self):
         return copy.deepcopy(self)
@@ -65,10 +66,10 @@
 
     def objective(self, X, y):
         objective = EstimatorObjective(X, y, self, None, eval_metric=self.get_parameter('opt-metric-name'), n_jobs=-1,
                                        random_state=42, direction='minimize')
         return objective
 
 
-from kolibri.registry import ModulesRegistry
-
-ModulesRegistry.add_module(RegSklearnEstimator.name, RegSklearnEstimator)
+# from kolibri.registry import ModulesRegistry
+#
+# ModulesRegistry.add_module(RegSklearnEstimator.name, RegSklearnEstimator)
```

## kolibri/task/text/classification/__init__.py

```diff
@@ -1 +1,2 @@
-from kolibri.task.text.classification.sklearn_classification_estimator import SklearnEstimator
+from kolibri.task.text.classification.sklearn_classification_estimator import SklearnEstimator
+from kolibri.task.text.classification.dnn_classification_estimator import DnnTextClassEstimator
```

## kolibri/task/text/classification/dnn_classification_estimator.py

```diff
@@ -1,13 +1,18 @@
 from kolibri import default_configs as settings
 from kolibri.config import TaskType
 from kolibri.config import override_defaults
-from kolibri.backend.tensorflow.tasks.dnn_estimator import DnnEstimator
-from kolibri.backend.tensorflow.tasks.text.classification.models import get_model
-from kolibri.backend.tensorflow.embeddings import DefaultEmbedding, WordEmbedding
+from kolibri.task.dnn_estimator import DnnEstimator
+
+try:
+    from kolibri.backend.tensorflow.tasks.text.classification.models import get_model
+    from kolibri.backend.tensorflow.embeddings import DefaultEmbedding, WordEmbedding
+except Exception as e:
+    pass
+
 from kolibri.logger import get_logger
 from kolibri.indexers.label_indexer import LabelIndexer
 
 logger = get_logger(__name__)
 
 KOLIBRI_MODEL_FILE_NAME = "classifier_kolibri.pkl"
 DNN_MODEL_FILE_NAME = "classifier_dnn"
@@ -30,14 +35,15 @@
             "model": "bilstm",
             "embeddings": "default",
             "multi-label": False,
             "sequence_length": 'auto',
             "epochs": 1,
             "loss": 'categorical_crossentropy',
             "class-weight": False,
+            "architecture":None
 
         },
         "tunable":{
 
         }
         # the models used in the classifier if several models are given they will be combined
 
@@ -60,15 +66,15 @@
             self.embeddings = WordEmbedding(w2v_path=self.get_parameter("embedding_path"),
                                             task=TaskType.CLASSIFICATION,
                                             sequence_length=self.get_parameter("sequence_length"),
                                             indexer=self.indexer)
         elif self.get_parameter('embeddings') == None:
             self.embeddings = None
 
-        self.clf = get_model(self.get_parameter('model'), embedding=self.embeddings, hyper_parameters=self.hyperparameters)
+        self.clf = get_model(self.get_parameter('model'), embedding=self.embeddings, hyper_parameters=self.get_parameter("architecture"))
         self.classifier_type = type(self.clf)
 
     @classmethod
     def required_packages(cls):
         return ["tensorflow"]
 
     def process(self, document, **kwargs):
```

## kolibri/task/text/classification/sklearn_classification_estimator.py

```diff
@@ -7,18 +7,18 @@
 
 try:
     from kolibri.optimizers.optuna.objective import EstimatorObjective
 except:
     pass
 from kolibri.config import TaskType
 from kolibri.logger import get_logger
-
+from kolibri.registry import register
 logger = get_logger(__name__)
 
-
+@register('SklearnEstimator')
 class SklearnEstimator(BaseClassifier):
     defaults = {"fixed": {
         "default-params": None,
         "task-type": TaskType.CLASSIFICATION
     },
 
         "tunable": {
@@ -86,10 +86,10 @@
 
     def objective(self, X, y):
         objective = EstimatorObjective(X, y, self, None, eval_metric=self.get_parameter('opt-metric-name'), n_jobs=-1,
                                        random_state=42)
         return objective
 
 
-from kolibri.registry import ModulesRegistry
-
-ModulesRegistry.add_module(SklearnEstimator.name, SklearnEstimator)
+# from kolibri.registry import ModulesRegistry
+#
+# ModulesRegistry.add_module(SklearnEstimator.name, SklearnEstimator)
```

## kolibri/task/text/entities/__init__.py

```diff
@@ -17,18 +17,18 @@
     def add_extractor_name(self, entities):
         for entity in entities:
             entity["extractor"] = self.name
         return entities
 
     def add_processor_name(self, entity):
         # type: (Dict[Text, Any]) -> Dict[Text, Any]
-        if "processors" in entity:
-            entity["processors"].append(self.name)
+        if "indexers" in entity:
+            entity["indexers"].append(self.name)
         else:
-            entity["processors"] = [self.name]
+            entity["indexers"] = [self.name]
 
         return entity
 
     @staticmethod
     def find_entity(ent, text, tokens):
         offsets = [token.offset for token in tokens]
         ends = [token.end for token in tokens]
```

## kolibri/task/text/entities_back/entity_extractor.py

```diff
@@ -15,18 +15,18 @@
 class EntityExtractor(Component):
     def add_extractor_name(self, entities):
         for entity in entities:
             entity["extractor"] = self.name
         return entities
 
     def add_processor_name(self, entity):
-        if "processors" in entity:
-            entity["processors"].append(self.name)
+        if "indexers" in entity:
+            entity["indexers"].append(self.name)
         else:
-            entity["processors"] = [self.name]
+            entity["indexers"] = [self.name]
 
         return entity
 
     @staticmethod
     def find_entity(ent, text, tokens):
         offsets = [token.offset for token in tokens]
         ends = [token.end for token in tokens]
```

## kolibri/task/text/intents/intent_catcher.py

```diff
@@ -21,21 +21,21 @@
 
 import numpy as np
 import tensorflow as tf
 import tensorflow_hub as tfhub
 from overrides import overrides
 from xeger import Xeger
 
-from deeppavlov.core.common.registry import register
-from deeppavlov.core.models.nn_model import NNModel
+from kolibri.registry import register
+from kolibri.backend.base.nn_model import NNModel
 
 log = getLogger(__name__)
 
 
-@register("intent_catcher")
+@register("IntentCatcher")
 class IntentCatcher(NNModel):
     """Class for IntentCatcher Chainer's pipeline components."""
 
     def __init__(self, save_path: Union[str, Path], load_path: Union[str, Path],
         embeddings : str = 'use', limit : int = 10, multilabel : bool = False,
         number_of_layers : int = 0, number_of_intents : int = 1,
         hidden_dim : int = 256, mode : str = 'train', **kwargs) -> None:
```

## kolibri/task/text/spelling/brillmoore/error_model.py

```diff
@@ -18,35 +18,35 @@
 from heapq import heappop, heappushpop, heappush
 from logging import getLogger
 from math import log, exp
 from typing import List, Iterable, Tuple
 
 from tqdm import tqdm
 
-from deeppavlov.core.common.errors import ConfigError
-from deeppavlov.core.common.registry import register
-from deeppavlov.core.models.estimator import Estimator
-from deeppavlov.vocabs.typos import StaticDictionary
+from kolibri.errors import ConfigError
+from kolibri.registry import register
+from kolibri.backend.base.base_estimator import BaseEstimator
+
 
 logger = getLogger(__name__)
 
 
 @register('spelling_error_model')
-class ErrorModel(Estimator):
+class ErrorModel(BaseEstimator):
     """Component that uses statistics based error model to find best candidates in a static dictionary.
     Based on An Improved Error Model for Noisy Channel Spelling Correction by Eric Brill and Robert C. Moore
 
     Args:
-        dictionary: a :class:`~deeppavlov.vocabs.typos.StaticDictionary` object
+        dictionary: a :class:`~kolibri.vocabs.typos.StaticDictionary` object
         window: maximum context window size
         candidates_count: maximum number of replacement candidates to return for every token in the input
 
     Attributes:
         costs: logarithmic probabilities of character sequences replacements
-        dictionary: a :class:`~deeppavlov.vocabs.typos.StaticDictionary` object
+        dictionary: a :class:`~kolibri.vocabs.typos.StaticDictionary` object
         window: maximum context window size
         candidates_count: maximum number of replacement candidates to return for every token in the input
     """
 
     def __init__(self, dictionary: StaticDictionary, window: int = 1, candidates_count: int = 1, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.costs = defaultdict(itertools.repeat(float('-inf')).__next__)
```

## kolibri/task/text/spelling/electors/kenlm_elector.py

```diff
@@ -14,17 +14,17 @@
 
 from logging import getLogger
 from pathlib import Path
 from typing import List, Tuple
 
 import kenlm
 
-from deeppavlov.core.commands.utils import expand_path
-from deeppavlov.core.common.registry import register
-from deeppavlov.core.models.component import Component
+from kdmt.path import expand_path
+from kolibri.registry import register
+from kolibri.core.component import Component
 
 logger = getLogger(__name__)
 
 
 @register('kenlm_elector')
 class KenlmElector(Component):
     """Component that chooses a candidate with the highest product of base and language model probabilities
```

## kolibri/task/text/spelling/electors/top1_elector.py

```diff
@@ -11,16 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from logging import getLogger
 from typing import List, Tuple
 
-from deeppavlov.core.common.registry import register
-from deeppavlov.core.models.component import Component
+from kolibri.registry import register
+from kolibri.core.component import Component
 
 logger = getLogger(__name__)
 
 
 @register('top1_elector')
 class TopOneElector(Component):
     """Component that chooses a candidate with highest base probability for every token
```

## kolibri/task/text/spelling/levenshtein/searcher_component.py

```diff
@@ -12,22 +12,22 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import string
 from logging import getLogger
 from math import log10
 from typing import Iterable, List, Tuple, Optional
 
-from deeppavlov.core.common.registry import register
-from deeppavlov.core.models.component import Component
+from kolibri.registry import register
+from kolibri.core.component import Component
 from .levenshtein_searcher import LevenshteinSearcher
 
 logger = getLogger(__name__)
 
 
-@register('spelling_levenshtein')
+@register('LevenshteinSearcherComponent')
 class LevenshteinSearcherComponent(Component):
     """Component that finds replacement candidates for tokens at a set Damerau-Levenshtein distance
 
     Args:
         words: list of every correct word
         max_distance: maximum allowed Damerau-Levenshtein distance between source words and candidates
         error_probability: assigned probability for every edit
```

## kolibri/tokenizers/__init__.py

```diff
@@ -1,14 +1,14 @@
 from kolibri.tokenizers.kolibri_tokenizer import KolibriTokenizer
 from kolibri.tokenizers.char_tokenizer import CharTokenizer
 from kolibri.tokenizers.regex_tokenizer import RegexpTokenizer
 from kolibri.tokenizers.word_tokenizer import WordTokenizer
 from kolibri.tokenizers.sentence_tokenizer import SentenceTokenizer
 from kolibri.tokenizers.ugc_tokenizer import UGCTokenizer
-
+from kolibri.tokenizers.bert_tokenizer import BertTokenizer
 
 # Standard sentence tokenizer.
 def tokenize_sentences(text):
     """
     Return a sentence-tokenized copy of *text*,
     using NLTK's recommended sentence tokenizer
     (currently :class:`.PunktSentenceTokenizer`
```

## kolibri/tokenizers/bert_tokenizer.py

```diff
@@ -43,15 +43,15 @@
         self._token_cls: str = token_cls
         self._token_sep: str = token_sep
         self._token_unk: str = token_unk
         self._pad_index: int = pad_index
         self._cased: bool = cased
 
     @classmethod
-    def load_from_vocab_file(cls, vocab_path: str) -> 'BertTokenizer':
+    def load_from_vocab_file(cls, vocab_path: str):
         token2idx: Dict[str, int] = {}
         with codecs.open(vocab_path, 'r', 'utf8') as reader:
             for line in reader:
                 token = line.strip()
                 token2idx[token] = len(token2idx)
         return BertTokenizer(token_dict=token2idx)
```

## kolibri/tokenizers/word_tokenizer.py

```diff
@@ -1,11 +1,12 @@
 from kolibri.tokenizers.regex_tokenizer import RegexpTokenizer
 from kolibri.tokenizers.tokenizer import Tokenizer
 from kdmt.dict import update
-
+from kolibri.registry import register
+@register('WordTokenizer')
 class WordTokenizer(Tokenizer):
     defaults = {
         "fixed": {
             'whitespace': False,
             'regex': None,
             'split': " "
         },
```

## kolibri/utils/__init__.py

```diff
@@ -1,26 +1,21 @@
-import io
+
 import json
 import logging
 import six
-from typing import Text, Any
-import functools
+from typing import  Optional, Sequence, Union, Collection
+import numpy as np
+
 logger = logging.getLogger(__name__)
 
 
 def overlap(start1, end1, start2, end2):
     return not (end1 <= start2 or start1 >= end2)
 
 
-def alnum_or_num(text):
-    return any(char.isdigit() for char in text)
-
-
-
-
 def lazyproperty(fn):
     """Allows to avoid recomputing a property over and over.
 
     The result gets stored in a local var. Computation of the property
     will happen once, on the first call of the property. All
     succeeding calls will use the text stored in the private property."""
 
@@ -45,31 +40,112 @@
 
 def json_to_string(obj, **kwargs):
     indent = kwargs.pop("indent", 2)
     ensure_ascii = kwargs.pop("ensure_ascii", False)
     return json.dumps(obj, indent=indent, ensure_ascii=ensure_ascii, **kwargs)
 
 
-def write_json_to_file(filename, obj, **kwargs):
-    # type: (Text, Any) -> None
-    """Write an object as a json string to a file."""
-
-    write_to_file(filename, json_to_string(obj, **kwargs))
-
 
+def zero_pad_truncate(batch: Sequence[Sequence[Union[int, float, np.integer, np.floating,
+                                                     Sequence[Union[int, float, np.integer, np.floating]]]]],
+                      max_len: int, pad: str = 'post', trunc: str = 'post',
+                      dtype: Optional[Union[type, str]] = None) -> np.ndarray:
+    """
+
+    Args:
+        batch: assumes a batch of lists of word indexes or their vector representations
+        max_len: resulting length of every batch item
+        pad: how to pad shorter batch items: can be ``'post'`` or ``'pre'``
+        trunc: how to truncate a batch item: can be ``'post'`` or ``'pre'``
+        dtype: overrides dtype for the resulting ``ndarray`` if specified,
+         otherwise ``np.int32`` is used for 2-d arrays and ``np.float32`` — for 3-d arrays
+
+    Returns:
+        a 2-d array of size ``(len(batch), max_len)`` or a 3-d array of size ``(len(batch), max_len, len(batch[0][0]))``
+    """
+    if isinstance(batch[0][0], Collection):  # ndarray behaves like a Sequence without actually being one
+        size = (len(batch), max_len, len(batch[0][0]))
+        dtype = dtype or np.float32
+    else:
+        size = (len(batch), max_len)
+        dtype = dtype or np.int32
 
+    padded_batch = np.zeros(size, dtype=dtype)
+    for i, batch_item in enumerate(batch):
+        if len(batch_item) > max_len:  # trunc
+            padded_batch[i] = batch_item[slice(max_len) if trunc == 'post' else slice(-max_len, None)]
+        else:  # pad
+            padded_batch[i, slice(len(batch_item)) if pad == 'post' else slice(-len(batch_item), None)] = batch_item
 
-def write_to_file(filename, text):
-    # type: (Text, Text) -> None
-    """Write a text to a file."""
-
-    with io.open(filename, 'w', encoding="utf-8") as f:
-        f.write(str(text))
-
-
+    return np.asarray(padded_batch)
 def ordered(obj):
     if isinstance(obj, dict):
         return sorted((k, ordered(v)) for k, v in obj.items())
     if isinstance(obj, list):
         return sorted(ordered(x) for x in obj)
     else:
         return obj
+
+import re
+from typing import List
+
+
+def enforce_stop_tokens(text: str, stop: List[str]) -> str:
+    """Cut off the text as soon as any stop words occur."""
+    return re.split("|".join(stop), text)[0]
+
+
+def write_file(data_contents, path):
+    """Write a file to the given path with the given contents.
+
+    If the path is an s3 directory, we will use the given aws credentials
+    to write to s3.
+
+    Args:
+        data_contents (bytes):
+            The contents that will be written to the file.
+        path (str):
+            The path to write the file to, which can be either local
+            or an s3 path.
+    Returns:
+        none
+    """
+    content_encoding = ''
+    write_mode = 'w'
+    if path.endswith('gz') or path.endswith('gzip'):
+        content_encoding = 'gzip'
+        write_mode = 'wb'
+    elif isinstance(data_contents, bytes):
+        write_mode = 'wb'
+
+
+    with open(path, write_mode) as f:
+        if write_mode == 'w':
+            f.write(data_contents.decode('utf-8'))
+        else:
+            f.write(data_contents)
+
+
+def write_csv(data, path):
+    """Write a csv file to the given path with the given contents.
+
+    If the path is an s3 directory, we will use the given aws credentials
+    to write to s3.
+
+    Args:
+        data (pandas.DataFrame):
+            The data that will be written to the csv file.
+        path (str):
+            The path to write the file to, which can be either local
+            or an s3 path.
+        aws_key (str):
+            The access key id that will be used to communicate with s3,
+            if provided.
+        aws_secret (str):
+            The secret access key that will be used to communicate
+            with s3, if provided.
+
+    Returns:
+        none
+    """
+    data_contents = data.to_csv(index=False).encode('utf-8')
+    write_file(data_contents, path)
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## kolibri/utils/common.py

```diff
@@ -1,15 +1,15 @@
 import os
 import numpy as np
 import pandas as pd
-
 from kolibri.config import TaskType
-
+from kdmt.numerical import is_int
 from copy import deepcopy
 
+
 def construct_learner_name(fold, repeat, repeats):
     repeat_str = f"_repeat_{repeat}" if repeats > 1 else ""
     return f"learner_fold_{fold}{repeat_str}"
 
 
 def intersect(d):
     result = set(d[0]).intersection(*d[1:])
@@ -107,24 +107,14 @@
     Method to check if the problem is multiclass.
     """
     try:
         return ml_task == TaskType.CLASSIFICATION and y.value_counts().count() > 2
     except:
         return False
 
-def is_int(x):
-    """Check if x is of integer type, but not boolean"""
-    # boolean are subclasses of integers in Python, so explicitly exclude them
-    return isinstance(x, (int, np.integer)) and not isinstance(x, bool)
-
-
-def is_float(x):
-    """Check if x is of float type"""
-    return isinstance(x, (float, np.floating))
-
 
 def check_n_jobs(n_jobs):
     """Check `n_jobs` parameter according to the scikit-learn convention.
 
     Parameters
     ----------
     n_jobs : int, positive or -1
@@ -208,7 +198,31 @@
     if error < 0.0000001:
         error = 0.0000001
     if error == 1:
         error = 0.9999999
     return 0.5*np.log((1-error)/error)
 
 
+def cast_to_iterable(value):
+    """Return a ``list`` if the input object is not a ``list`` or ``tuple``."""
+    if isinstance(value, (list, tuple)):
+        return value
+
+    return [value]
+
+
+
+def groupby_list(list_to_check):
+    """Return the first element of the list if the length is 1 else the entire list."""
+    return list_to_check[0] if len(list_to_check) == 1 else list_to_check
+
+
+def create_unique_name(name, list_names):
+    """Modify the ``name`` parameter if it already exists in the list of names."""
+    result = name
+    while result in list_names:
+        result += '_'
+
+    return result
+
+
+
```

## kolibri/utils/cross_validation.py

```diff
@@ -7,15 +7,15 @@
 from sklearn.base import is_classifier, clone
 from sklearn.utils import indexable
 from sklearn.utils.validation import _check_fit_params
 from sklearn.utils.validation import _num_samples
 from sklearn.utils.fixes import delayed
 from sklearn.utils.metaestimators import _safe_split
 from sklearn.metrics import check_scoring
-from sklearn.metrics._scorer import _check_multimetric_scoring
+from sklearn.metrics._scorer import _check_multimetric_scoring, _MultimetricScorer
 from sklearn.model_selection._split import check_cv
 from sklearn.preprocessing import LabelEncoder
 
 
 def cross_val_predict_score(
     estimator,
     X,
@@ -86,15 +86,15 @@
         .. versionchanged:: 0.22
             ``cv`` default value if None changed from 3-fold to 5-fold.
 
     n_jobs : int, default=None
         Number of jobs to run in parallel. Training the estimator and
         predicting are parallelized over the cross-validation splits.
         ``None`` means 1 unless in a :obj:`joblib.parallel_backend` context.
-        ``-1`` means using all processors. See :term:`Glossary <n_jobs>`
+        ``-1`` means using all indexers. See :term:`Glossary <n_jobs>`
         for more details.
 
     verbose : int, default=0
         The verbosity level.
 
     fit_params : dict, default=None
         Parameters to pass to the fit method of the estimator.
@@ -283,14 +283,18 @@
 
     if y_train is None:
         estimator.fit(X_train, **fit_params)
     else:
         estimator.fit(X_train, y_train, **fit_params)
     func = getattr(estimator, method)
     predictions = func(X_test)
+    sum_val=0
+    for i in range(len(predictions)):
+        sum_val += abs(predictions[i] - y_test[i])
+
     test_scores = _score(estimator, X_test, y_test, scorer, error_score)
 
     encode = (
         method in ["decision_function", "predict_proba", "predict_log_proba"]
         and y is not None
     )
```

## kolibri/utils/timeseries_functions.py

```diff
@@ -329,14 +329,15 @@
             shift_until = shift_from + max_timeshift + 1
 
             df_temp = x.iloc[shift_from:shift_until]
 
         if df_temp is None or len(df_temp) < min_timeshift + 1:
             return
 
+
         df_temp = df_temp.copy()
 
         # and set the shift correctly
         if column_sort and rolling_direction > 0:
             timeshift_value = df_temp[column_sort].iloc[-1]
         elif column_sort and rolling_direction < 0:
             timeshift_value = df_temp[column_sort].iloc[0]
@@ -508,15 +509,15 @@
     if column_sort is not None:
         # Require no Nans in column
         if df[column_sort].isnull().any():
             raise ValueError("You have NaN values in your sort column.")
 
         df = df.sort_values(column_sort)
 
-        if df[column_sort].dtype != np.object:
+        if df[column_sort].dtype != object:
             # if rolling is enabled, the data should be uniformly sampled in this column
             # Build the differences between consecutive time sort values
 
             differences = df.groupby(grouper)[column_sort].apply(
                 lambda x: x.values[:-1] - x.values[1:]
             )
             # Write all of them into one big list
@@ -576,17 +577,19 @@
         data=range_of_shifts,
         chunk_size=chunksize,
         function_kwargs=kwargs,
     )
 
     distributor.close()
 
-    df_shift = pd.concat(shifted_chunks, ignore_index=True)
 
-    return df_shift.sort_values(by=["id", column_sort or "sort"])
+    return [c for c in shifted_chunks if len(c)>0]
+#    df_shift = pd.concat(shifted_chunks, ignore_index=True)
+
+#    return df_shift.sort_values(by=["id", column_sort or "sort"])
 
 
 def make_forecasting_frame(x, kind, max_timeshift, rolling_direction):
     """
     Takes a singular time series x and constructs a DataFrame df and target vector y that can be used for a time series
     forecasting task.
```

## Comparing `kolibri/backend/tensorflow/custom_loses.py` & `kolibri/backend/tensorflow/losses/custom_loses.py`

 * *Files identical despite different names*

## Comparing `kolibri/backend/tensorflow/loader.py` & `kolibri/backend/tensorflow/embeddings/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,22 +49,22 @@
     pns  = prefix.split("/")
 
     # assert ns[0] == "bert"
 
     name = "/".join(pns + ns[1:])
     ns = name.split("/")
 
-    if ns[1] not in ["encoder", "embeddings"]:
+    if ns[1] not in ["encoders", "embeddings"]:
         return None
     if ns[1] == "embeddings":
         if ns[2] == "LayerNorm":
             return name
         else:
             return name + "/embeddings"
-    if ns[1] == "encoder":
+    if ns[1] == "encoders":
         if ns[3] == "intermediate":
             return "/".join(ns[:4] + ns[5:])
         else:
             return name
     return None
 
 
@@ -75,28 +75,28 @@
 
     if ns[:len(pns)] != pns:
         return None
 
     name = "/".join(["bert"] + ns[len(pns):])
     ns   = name.split("/")
 
-    if ns[1] not in ["encoder", "embeddings"]:
+    if ns[1] not in ["encoders", "embeddings"]:
         return None
     if ns[1] == "embeddings":
         if ns[2] == "LayerNorm":
             return name
         elif ns[2] == "word_embeddings_projector":
             ns[2] = "word_embeddings_2"
             if ns[3] == "projector":
                 ns[3] = "embeddings"
                 return "/".join(ns[:-1])
             return "/".join(ns)
         else:
             return "/".join(ns[:-1])
-    if ns[1] == "encoder":
+    if ns[1] == "encoders":
         if ns[3] == "intermediate":
             return "/".join(ns[:4] + ["dense"] + ns[4:])
         else:
             return name
     return None
 
 
@@ -175,15 +175,15 @@
 
 def _checkpoint_exists(ckpt_path):
     cktp_files = tf.io.gfile.glob(ckpt_path + "*")
     return len(cktp_files) > 0
 
 
 def bert_prefix(bert: BertModelLayer):
-    re_bert = re.compile(r'(.*)/(embeddings|encoder)/(.+):0')
+    re_bert = re.compile(r'(.*)/(embeddings|encoders)/(.+):0')
     match = re_bert.match(bert.weights[0].name)
     assert match, "Unexpected bert layer: {} weight:{}".format(bert, bert.weights[0].name)
     prefix = match.group(1)
     return prefix
 
 
 def load_stock_weights(bert: BertModelLayer, ckpt_path, map_to_stock_fn=map_to_stock_variable_name):
```

## Comparing `kolibri/backend/tensorflow/loader_albert.py` & `kolibri/backend/tensorflow/embeddings/loader_albert.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,47 +216,47 @@
     fetched_dir = pf.utils.unpack_archive(fetched_file)
 
     return fetched_dir
 
 
 def map_to_tfhub_albert_variable_name(name, prefix="bert"):
 
-    name = re.compile("encoder/layer_shared/intermediate/(?=kernel|bias)").sub(
-        "encoder/transformer/group_0/inner_group_0/ffn_1/intermediate/dense/", name)
-    name = re.compile("encoder/layer_shared/output/dense/(?=kernel|bias)").sub(
-        "encoder/transformer/group_0/inner_group_0/ffn_1/intermediate/output/dense/", name)
-
-    name = name.replace("encoder/layer_shared/output/dense",               "encoder/transformer/group_0/inner_group_0/ffn_1/intermediate/output/dense")
-    name = name.replace("encoder/layer_shared/attention/output/LayerNorm", "encoder/transformer/group_0/inner_group_0/LayerNorm")
-    name = name.replace("encoder/layer_shared/output/LayerNorm", "encoder/transformer/group_0/inner_group_0/LayerNorm_1")
-    name = name.replace("encoder/layer_shared/attention",        "encoder/transformer/group_0/inner_group_0/attention_1")
+    name = re.compile("encoders/layer_shared/intermediate/(?=kernel|bias)").sub(
+        "encoders/transformer/group_0/inner_group_0/ffn_1/intermediate/dense/", name)
+    name = re.compile("encoders/layer_shared/output/dense/(?=kernel|bias)").sub(
+        "encoders/transformer/group_0/inner_group_0/ffn_1/intermediate/output/dense/", name)
+
+    name = name.replace("encoders/layer_shared/output/dense",               "encoders/transformer/group_0/inner_group_0/ffn_1/intermediate/output/dense")
+    name = name.replace("encoders/layer_shared/attention/output/LayerNorm", "encoders/transformer/group_0/inner_group_0/LayerNorm")
+    name = name.replace("encoders/layer_shared/output/LayerNorm", "encoders/transformer/group_0/inner_group_0/LayerNorm_1")
+    name = name.replace("encoders/layer_shared/attention",        "encoders/transformer/group_0/inner_group_0/attention_1")
 
     name = name.replace("embeddings/word_embeddings_projector/projector",
-                        "encoder/embedding_hidden_mapping_in/kernel")
+                        "encoders/embedding_hidden_mapping_in/kernel")
     name = name.replace("embeddings/word_embeddings_projector/bias",
-                        "encoder/embedding_hidden_mapping_in/bias")
+                        "encoders/embedding_hidden_mapping_in/bias")
 
     name = name.split(":")[0]
     ns   = name.split("/")
     pns  = prefix.split("/")
 
     if ns[:len(pns)] != pns:
         return None
 
     name = "/".join(["bert"] + ns[len(pns):])
     ns   = name.split("/")
 
-    if ns[1] not in ["encoder", "embeddings"]:
+    if ns[1] not in ["encoders", "embeddings"]:
         return None
     if ns[1] == "embeddings":
         if ns[2] == "LayerNorm":
             return name
         else:
             return "/".join(ns[:-1])
-    if ns[1] == "encoder":
+    if ns[1] == "encoders":
         if ns[3] == "intermediate":
             return "/".join(ns[:4] + ["dense"] + ns[4:])
         else:
             return name
     return None
```

## Comparing `kolibri/backend/tensorflow/callbacks/connl_callBack.py` & `kolibri/backend/tensorflow/callbacks/conll_call_back.py`

 * *Files identical despite different names*

## Comparing `kolibri/backend/tensorflow/embeddings/default_embedding.py` & `kolibri/backend/tensorflow/embeddings/bare_embedding.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,54 @@
+# encoding: utf-8
 
-from typing import Any
+
+
+from typing import Dict, Any, Optional
 
 from tensorflow import keras
-from typing import Dict
-from kolibri.backend.tensorflow.embeddings.base_embedding import ABCEmbedding
+
+from kolibri.backend.tensorflow.embeddings.base_embedding import BaseEmbedding
 
 L = keras.layers
 
 
-class DefaultEmbedding(ABCEmbedding):
+class DefaultEmbedding(BaseEmbedding):
     """
-    DefaultEmbedding is a random init `tf.keras.layers.Embedding` layer for text sequence embedding,
-    which is the defualt embedding class for dnn models.
+    DefaultEmbedding is a random init `tf.keras.layers.Embeddings` layer for text sequence embedding,
+    which is the defualt embedding class for kolibri models.
     """
 
     def __init__(self,
                  embedding_size: int = 100,
                  **kwargs: Any):
         """
 
         Args:
             embedding_size: Dimension of the dense embedding.
             kwargs: additional params
         """
         self.embedding_size: int = embedding_size
         super(DefaultEmbedding, self).__init__(embedding_size=embedding_size,
                                                **kwargs)
-    def load_embed_vocab(self):
+
+    def load_embed_vocab(self) -> Optional[Dict[str, int]]:
         return None
 
-    # def build_embedding_model(self, *, vocab_size=None, force=False, **kwargs):
-    #     if self.embed_model is None or force:
-    #         self.input_tensor = L.Input(shape=(None,),
-    #                                         name=f'input')
-    #
-    #         layer_embedding = L.Embedding(vocab_size,
-    #                                       self.embedding_size,
-    #                                       mask_zero=True,
-    #                                       name= f'_layer_embedding')
-    #
-    #         self.embedded_tensor = layer_embedding(self.input_tensor)
-    #         self.embed_model = keras.Model(self.input_tensor, self.embedded_tensor)
     def build_embedding_model(self,
                               *,
                               vocab_size: int = None,
                               force: bool = False,
                               **kwargs: Dict) -> None:
         if self.embed_model is None or force:
             input_tensor = L.Input(shape=(None,),
                                    name=f'input')
-            layer_embedding = L.Embedding(vocab_size,
-                                          self.embedding_size,
-                                          mask_zero=True,
-                                          name=f'layer_embedding')
+            layer_embedding = L.Embeddings(vocab_size,
+                                           self.embedding_size,
+                                           mask_zero=True,
+                                           name=f'layer_embedding')
 
             embedded_tensor = layer_embedding(input_tensor)
             self.embed_model = keras.Model(input_tensor, embedded_tensor)
 
 
 if __name__ == "__main__":
     pass
```

## Comparing `kolibri/backend/tensorflow/layers/crf.py` & `kolibri/backend/tensorflow/layers/conditional_random_field.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
 from distutils.version import LooseVersion
 
 import tensorflow as tf
 import tensorflow.keras.backend as K
 import tensorflow_addons as tfa
 
 
-class ConditionalRandomField(tf.keras.layers.Layer):
+class KConditionalRandomField(tf.keras.layers.Layer):
     """
-    K is to mark Kashgari version of CRF
+    K is to mark Kolibri version of CRF
     Conditional Random Field layer (tf.keras)
     `CRF` can be used as the last layer in a network (as a classifier). Input shape (features)
     must be equal to the number of classes the CRF can predict (a linear layer is recommended).
 
     Args:
         num_labels (int): the number of labels to tag each temporal input.
 
@@ -107,15 +109,15 @@
     # Use argmax to estimate accuracy
     def fast_accuracy(self, y_true, y_pred):
         mask = self.mask
         if len(K.int_shape(y_true)) == 3:
             y_true = K.argmax(y_true, axis=-1)
         y_pred = K.argmax(y_pred, -1)
         y_true = K.cast(y_true, y_pred.dtype)
-        # Take the maximum label by label to roughly evaluate the training effect
+        # 逐标签取最大来粗略评测训练效果
         isequal = K.equal(y_true, y_pred)
         isequal = K.cast(isequal, y_pred.dtype)
         if mask is None:
             return K.mean(isequal)
         else:
             mask = K.cast(mask, y_pred.dtype)
             return K.sum(isequal * mask) / K.sum(mask)
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `kolibri/backend/tensorflow/tasks/dnn_estimator.py` & `kolibri/task/dnn_estimator.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from sklearn.utils import class_weight
 import h5py
 from kolibri.config import override_defaults
 from kolibri.core.component import Component
 from kolibri.logger import get_logger
 from sklearn.model_selection import train_test_split
 from kdmt.cloud.azure import upload_file, get_file_object
-from kolibri.evaluation.classifier_evaluator import ClassifierEvaluator
-from tensorflow import keras
+from kolibri.evaluators.classifier_evaluator import ClassifierEvaluator
+
 
 logger = get_logger(__name__)
 from kolibri.default_configs import DEFAULT_NN_MODEL_FILENAME
 KOLIBRI_MODEL_FILE_NAME = "classifier-kolibri.pkl"
 DNN_MODEL_FOLDER_NAME = "classifier-dnn"
 
 
@@ -41,51 +41,60 @@
             "sequence_length": 'auto',
             "epochs": 1,
             "loss": 'categorical_crossentropy',
             "class-weight": False,
             "test_size": 0.3,
             "remote-storage": "azure-blob",
             "container-name": None,
-            "model-name": DEFAULT_NN_MODEL_FILENAME
+            "model-name": DEFAULT_NN_MODEL_FILENAME,
+            "features":[]
         },
         'tunable':{}
 
     }
 
     def __init__(self, component_config=None):
 
         """Construct a new class classifier using the sklearn framework."""
 
         self.defaults = override_defaults(
             super(DnnEstimator, self).defaults, self.defaults)
         self.clf=None
         super().__init__(parameters=component_config)
+        self._features_names = self.get_parameter("features")
 
 
     @classmethod
     def required_packages(cls):
         return ["tensorflow"]
 
+    @property
+    def features_names(self):
+        return self._features_names
+
+
     def fit(self, X, y, X_val=None, y_val=None):
         fit_kwargs = {}
         if self.get_parameter('class-weight'):
-            class_weights = class_weight.compute_class_weight('balanced',classes=np.unique(y), y=y)
+            class_weights = class_weight.compute_class_weight('balanced',
+                                                              np.unique(y),
+                                                              y)
             fit_kwargs = {"class_weight": class_weights}
 
         if X_val ==None or y_val==None:
             X, X_val, y,y_val = train_test_split(X, y, test_size=self.get_parameter("test_size"))
 
 
         self.clf.fit(X, y, x_validate=X_val, y_validate=y_val, epochs=self.get_parameter("epochs"),
                      fit_kwargs=fit_kwargs)
 
-#        print(self.clf.evaluate(X_val, y_val))
-        predictions=self.clf.predict(X_val)
-#        self.performance_report=ClassifierEvaluator.get_performance_report(y_val, y_pred[0][:,0], None)
-        return None, None, None, predictions
+        print(self.clf.evaluate(X_val, y_val))
+        y_pred=self.clf.predict(X_val)
+        self.performance_report=ClassifierEvaluator.get_performance_report(y_val, y_pred, None)
+
     def transform(self, document):
 
         return self.clf.transform(document, )
 
     def predict(self, X):
         """Given a bow vector of an input text, predict most probable label.
 
@@ -104,19 +113,19 @@
         self.fit(X, y)
 
     def process(self, document, **kwargs):
         raise NotImplementedError
 
     def __getstate__(self):
         """Return state values to be pickled."""
-        return (self.hyperparameters, self.classifier_type)
+        return (self.hyperparameters, self.classifier_type, self._features_names)
 
     def __setstate__(self, state):
         """Restore state from the unpickled state values."""
-        self.hyperparameters, self.classifier_type = state
+        self.hyperparameters, self.classifier_type, self._features_names= state
 
 
     @classmethod
     def load(cls, model_dir=None, model_metadata=None, cached_component=None, **kwargs):
 
 
 #        model_file=cls.__name__+'.model-weights.h5'
@@ -153,14 +162,15 @@
             return model
         else:
             return None
 
 
     @classmethod
     def load_from_azure(cls, container_name=None):
+        from tensorflow import keras
 
         connect_str=os.environ.get("STORAGE_CONTAINER_STRING")
 
 
         blob_classifier_file=cls.__name__+'.'+KOLIBRI_MODEL_FILE_NAME
 
         classfier_file=get_file_object(connect_str, container_name, blob_classifier_file)
```

## Comparing `kolibri/backend/tensorflow/tasks/text/labeling/experimental.py` & `kolibri/backend/tensorflow/tasks/text/labeling/bi_gru_crf_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,86 @@
-# encoding: utf-8
-
-# author: BrikerMan
-# contact: eliyar917@gmail.com
-# blog: https://eliyar.biz
-
-# file: experimental.py
-# time: 2019-05-22 19:35
+#!/usr/bin/env python
 
 from typing import Dict, Any
 
 from tensorflow import keras
-from keras_self_attention import SeqSelfAttention
 
-import kolibri.backend
-from kolibri.backend.tensorflow.tasks.text.labeling import BaseLabelingModel
-from kolibri.backend.tensorflow.layers import L
+from kolibri.backend.tensorflow.layers import L, KConditionalRandomField
+from kolibri.backend.tensorflow.tasks.text.labeling.base_model import BaseLabelingModel
 
 
-class BLSTMAttentionModel(BaseLabelingModel):
-    """Bidirectional LSTM Self Attention Sequence Labeling Model"""
+class BiGRU_CRF_Model(BaseLabelingModel):
 
     @classmethod
-    def get_default_hyper_parameters(cls) -> Dict[str, Dict[str, Any]]:
-        """
-        Get hyper parameters of model
-        Returns:
-            hyper parameters dict
-        """
+    def default_hyper_parameters(cls) -> Dict[str, Dict[str, Any]]:
         return {
-            'layer_blstm': {
-                'units': 64,
+            'layer_bgru': {
+                'units': 128,
                 'return_sequences': True
             },
-            'layer_self_attention': {
-                'attention_activation': 'sigmoid'
-            },
             'layer_dropout': {
-                'rate': 0.5
+                'rate': 0.4
             },
             'layer_time_distributed': {},
             'layer_activation': {
                 'activation': 'softmax'
             }
         }
 
-    def build_model_arc(self):
-        """
-        build model architectural
-        """
-        output_dim = len(self.label_indexer.token2idx)
+    def build_model_arc(self) -> None:
+        output_dim = self.label_processor.vocab_size
+
         config = self.hyper_parameters
         embed_model = self.embedding.embed_model
 
-        layer_blstm = L.Bidirectional(L.LSTM(**config['layer_blstm']),
-                                      name='layer_blstm')
-        layer_self_attention = SeqSelfAttention(**config['layer_self_attention'],
-                                                name='layer_self_attention')
-        layer_dropout = L.Dropout(**config['layer_dropout'],
-                                  name='layer_dropout')
-
-        layer_time_distributed = L.TimeDistributed(L.Dense(output_dim,
-                                                           **config['layer_time_distributed']),
-                                                   name='layer_time_distributed')
-        layer_activation = L.Activation(**config['layer_activation'])
-
-        tensor = layer_blstm(embed_model.output)
-        tensor = layer_self_attention(tensor)
-        tensor = layer_dropout(tensor)
-        tensor = layer_time_distributed(tensor)
-        output_tensor = layer_activation(tensor)
+        crf = KConditionalRandomField()
 
-        self.tf_model = keras.Model(embed_model.inputs, output_tensor)
+        layer_stack = [
+            L.Bidirectional(L.GRU(**config['layer_bgru']), name='layer_bgru'),
+            L.Dropout(**config['layer_dropout'], name='layer_dropout'),
+            L.Dense(output_dim, **config['layer_time_distributed']),
+            crf
+        ]
+
+        tensor = embed_model.output
+        for layer in layer_stack:
+            tensor = layer(tensor)
+
+        self.tf_model = keras.Model(embed_model.inputs, tensor)
+        self.crf_layer = crf
+
+    def compile_model(self,
+                      loss: Any = None,
+                      optimizer: Any = None,
+                      metrics: Any = None,
+                      **kwargs: Any) -> None:
+        if loss is None:
+            loss = self.crf_layer.loss
+        if metrics is None:
+            metrics = [self.crf_layer.accuracy]
+        super(BiGRU_CRF_Model, self).compile_model(loss=loss,
+                                                   optimizer=optimizer,
+                                                   metrics=metrics,
+                                                   **kwargs)
 
 
-# Register custom layer
-kolibri.backend.tensorflow.custom_objects['SeqSelfAttention'] = SeqSelfAttention
-
 if __name__ == "__main__":
+    from kolibri.data.text.corpus import ChineseDailyNerCorpus
+    from kolibri.backend.tensorflow.callbacks import EvalCallBack
 
-    from kolibri.datasets.reader.snips import SnipsIntentCorpus
-
-    train_corpus = SnipsIntentCorpus()
-    train_corpus.read(task_name='ner')
-
-
-    train_x, train_y = train_corpus.get_instances(sub_set='train')
-    valid_x, valid_y = train_corpus.get_instances(sub_set='test')
-    model = BLSTMAttentionModel()
-    model.fit(train_x, train_y, valid_x, valid_y, epochs=2, batch_size=64)
-    model.evaluate(valid_x, valid_y)
-    model.save("/Users/mohamedmentis/Documents/Mentis/Development/Python/Deep_kolibri/demos/classifier_dnn")
+    train_x, train_y = ChineseDailyNerCorpus.load_data('train')
+    valid_x, valid_y = ChineseDailyNerCorpus.load_data('valid')
+    test_x, test_y = ChineseDailyNerCorpus.load_data('test')
+
+    model = BiGRU_CRF_Model(sequence_length=10)
+
+    eval_callback = EvalCallBack(kash_model=model,
+                                 x_data=valid_x,
+                                 y_data=valid_y,
+                                 truncating=True,
+                                 step=1)
+
+    model.fit(train_x, train_y, valid_x, valid_y, epochs=1,
+              callbacks=[])
+    y = model.predict(test_x[:200])
+    model.tf_model.summary()
+    model.evaluate(test_x, test_y)
```

## Comparing `kolibri/features/text/embedders/abstract_embedder.py` & `kolibri/features/text/embedders/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from overrides import overrides
 from kolibri.core.component import Component
 from kdmt.sequences import pad
 
 log = getLogger(__name__)
 
 
-class Embedder(Component):
+class Embeddings(Component):
     """
     Class implements fastText embedding model
 
     Args:
         load_path: path where to load pre-trained embedding model from
         pad_zero: whether to pad samples or not
 
@@ -71,41 +71,41 @@
         Args:
             batch: list of tokenized text samples
             mean: whether to return mean embedding of tokens per sample
 
         Returns:
             embedded batch
         """
-        batch = [self._encode(sample, mean) for sample in batch]
+        batch = [self.embed_documents(sample, mean) for sample in batch]
         if self.pad_zero:
             batch = pad(batch)
         return batch
 
     @abstractmethod
     def __iter__(self) -> Iterator[str]:
         """
         Iterate over all words from the model vocabulary
 
         Returns:
             iterator
         """
 
     @abstractmethod
-    def _get_word_vector(self, w: str) -> np.ndarray:
+    def embed_query(self, w: str) -> np.ndarray:
         """
         Embed a word using ``self.model``
 
         Args:
-            w: a word
+            w: a word, or documnet
 
         Returns:
             embedding vector
         """
 
-    def _encode(self, tokens: List[str], mean: bool) -> Union[List[np.ndarray], np.ndarray]:
+    def embed_documents(self, tokens: List[str], mean: bool=False) -> List[List[float]]:
         """
         Embed one text sample
 
         Args:
             tokens: tokenized text sample
             mean: whether to return mean embedding of tokens per sample
 
@@ -114,15 +114,15 @@
         """
         embedded_tokens = []
         for t in tokens:
             try:
                 emb = self.tok2emb[t]
             except KeyError:
                 try:
-                    emb = self._get_word_vector(t)
+                    emb = self.embed_query(t)
                 except KeyError:
                     emb = np.zeros(self.dim, dtype=np.float32)
                 self.tok2emb[t] = emb
             embedded_tokens.append(emb)
 
         if mean is None:
             mean = self.mean
```

## Comparing `kolibri/preprocess/preprocessors/char_splitter.py` & `kolibri/preprocess/text/char_splitter.py`

 * *Files identical despite different names*

## Comparing `kolibri/preprocess/preprocessors/dirty_comments_preprocessor.py` & `kolibri/preprocess/text/dirty_comments_preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,26 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import re
 import string
 from typing import List
 
-from deeppavlov.core.common.registry import register
-from deeppavlov.core.models.component import Component
+from kolibri.registry import register
+from kolibri.core.component import Component
 
 
-@register('dirty_comments_preprocessor')
+@register('DirtyCommentsPreprocessor')
 class DirtyCommentsPreprocessor(Component):
     """
     Class implements preprocessing of english texts with low level of literacy such as comments
     """
 
     def __init__(self, remove_punctuation: bool = True, *args, **kwargs):
+        super().__init__()
         self.remove_punctuation = remove_punctuation
 
     def __call__(self, batch: List[str], **kwargs) -> List[str]:
         """
         Preprocess given batch
 
         Args:
```

## Comparing `kolibri/preprocess/preprocessors/mask.py` & `kolibri/preprocess/text/mask.py`

 * *Files identical despite different names*

## Comparing `kolibri/preprocess/preprocessors/ner_preprocessor.py` & `kolibri/preprocess/text/ner_preprocessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import errno
 import os
 from logging import getLogger
 from typing import List
 
 import numpy as np
 
-from deeppavlov.core.common.registry import register
-from deeppavlov.core.models.estimator import Estimator
+from kolibri.registry import register
+from kolibri.core.component import Component
 
 log = getLogger(__name__)
 
 
-@register("ner_preprocessor")
-class NerPreprocessor():
+@register("NerPreprocessor")
+class NerPreprocessor(Component):
     """ Preprocess the batch of list of tokens
 
     Params:
         get_x_padded_for_elmo: whether the padded batch used for ELMo is returned
         get_x_cap_padded: whether the padded batch used for capitalization feature extraction is returned
     """
```

## Comparing `kolibri/preprocess/preprocessors/odqa_preprocessors.py` & `kolibri/preprocess/text/doc_chuncker.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,19 @@
-# Copyright 2017 Neural Networks and Deep Learning lab, MIPT
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
 
 from itertools import chain
 from logging import getLogger
 from typing import List, Callable, Union, Tuple, Optional
-
-from nltk import sent_tokenize
-
-from deeppavlov.core.common.registry import register
-from deeppavlov.core.models.component import Component
+from kolibri.tokenizers.sentence_tokenizer import split_text_to_sentences
+from kolibri.registry import register
+from kolibri.core.component import Component
 
 logger = getLogger(__name__)
 
 
-@register('document_chunker')
+@register('DocumentChunker')
 class DocumentChunker(Component):
     """Make chunks from a document or a list of documents. Don't tear up sentences if needed.
 
     Args:
         sentencize_fn: a function for sentence segmentation
         keep_sentences: whether to tear up sentences between chunks or not
         tokens_limit: a number of tokens in a single chunk (usually this number corresponds to the squad model limit)
@@ -39,24 +24,28 @@
         keep_sentences: whether to tear up sentences between chunks or not
         tokens_limit: a number of tokens in a single chunk
         flatten_result: whether to flatten the resulting list of lists of chunks
         paragraphs: whether to split document by paragrahs; if set to True, tokens_limit is ignored
 
     """
 
-    def __init__(self, sentencize_fn: Callable = sent_tokenize, keep_sentences: bool = True,
-                 tokens_limit: int = 400, flatten_result: bool = False,
-                 paragraphs: bool = False, number_of_paragraphs: int = -1, *args, **kwargs) -> None:
-        self._sentencize_fn = sentencize_fn
+    def __init__(self,  keep_sentences: bool = True, tokens_limit: int = 400,
+                 flatten_result: bool = False, paragraphs: bool = False, number_of_paragraphs: int = -1, *args,
+                 **kwargs) -> None:
+        super().__init__()
         self.keep_sentences = keep_sentences
         self.tokens_limit = tokens_limit
         self.flatten_result = flatten_result
         self.paragraphs = paragraphs
         self.number_of_paragraphs = number_of_paragraphs
 
+
+    def fit(self, X, y=None):
+        return self(X)
+
     def __call__(self, batch_docs: List[Union[str, List[str]]],
                  batch_docs_ids: Optional[List[Union[str, List[str]]]] = None) -> \
             Union[Tuple[Union[List[str], List[List[str]]], Union[List[str], List[List[str]]]],
                   Union[List[str], List[List[str]]]]:
         """Make chunks from a batch of documents. There can be several documents in each batch.
         Args:
             batch_docs: a batch of documents / a batch of lists of documents
@@ -92,15 +81,15 @@
                     if self.number_of_paragraphs != -1:
                         split_doc = split_doc[:self.number_of_paragraphs]
                     batch_chunks.append(split_doc)
                     batch_chunks_ids.append([id] * len(split_doc))
                 else:
                     doc_chunks = []
                     if self.keep_sentences:
-                        sentences = sent_tokenize(doc)
+                        sentences = split_text_to_sentences(doc)
                         n_tokens = 0
                         keep = []
                         for s in sentences:
                             n_tokens += len(s.split())
                             if n_tokens > self.tokens_limit:
                                 if keep:
                                     doc_chunks.append(' '.join(keep))
@@ -128,35 +117,7 @@
                     result[i] = flattened
                     result_ids[i] = flattened_ids
 
         if empty_docs_ids_flag:
             return result
 
         return result, result_ids
-
-
-@register('string_multiplier')
-class StringMultiplier(Component):
-    """Make a list of strings from a provided string. A length of the resulting list equals a length
-    of a provided reference argument.
-
-    """
-
-    def __init__(self, **kwargs):
-        pass
-
-    def __call__(self, batch_s: List[str], ref: List[str]) -> List[List[str]]:
-        """ Multiply each string in a provided batch of strings.
-
-        Args:
-            batch_s: a batch of strings to be multiplied
-            ref: a reference to obtain a length of the resulting list
-
-        Returns:
-            a multiplied s as list
-
-        """
-        res = []
-        for s, r in zip(batch_s, ref):
-            res.append([s] * len(r))
-
-        return res
```

## Comparing `kolibri/preprocess/preprocessors/random_embeddings_matrix.py` & `kolibri/preprocess/text/random_embeddings_matrix.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import numpy as np
 
-from deeppavlov.core.common.registry import register
+from kolibri.registry import register
 
 
-@register('random_emb_mat')
+@register('RandomEmbeddingsMatrix')
 class RandomEmbeddingsMatrix:
     """Assembles matrix of random embeddings.
 
     Args:
         vocab_len: length of the vocabulary (number of tokens in it)
         emb_dim: dimensionality of the embeddings
```

## Comparing `kolibri/preprocess/preprocessors/re_preprocessor.py` & `kolibri/preprocess/text/re_preprocessor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,38 @@
 
 from logging import getLogger
 from pathlib import Path
 from typing import Tuple, List, Union
 
 import numpy as np
-from transformers import BertTokenizer
+from kolibri.tokenizers import BertTokenizer
 
-from deeppavlov.core.commands.utils import expand_path
-from deeppavlov.core.common.file import read_json
-from deeppavlov.core.common.registry import register
-from deeppavlov.core.models.component import Component
+from kdmt.path import expand_path
+from kdmt.file import read_json
+from kolibri.registry import register
+from kolibri.core.component import Component
 
 log = getLogger(__name__)
 
 
 @register('re_preprocessor')
 class REPreprocessor(Component):
-    def __init__(
-            self,
-            vocab_file: str,
-            special_token: str = '<ENT>',
-            ner_tags=None,
-            max_seq_length: int = 512,
-            do_lower_case: bool = False,
-            default_tag: str = None,
-            **kwargs
-    ):
+    def __init__(self, vocab_file: str, special_token: str = '<ENT>', ner_tags=None, max_seq_length: int = 512,
+                 do_lower_case: bool = False, default_tag: str = None, **kwargs):
         """
         Args:
             vocab_file: path to vocabulary / name of vocabulary for tokenizer initialization
             special_token: an additional token that will be used for marking the entities in the document
             do_lower_case: set True if lowercasing is needed
             default_tag: used for test purposes to create a valid input
         Return:
             list of feature batches with input_ids, attention_mask, entity_pos, ner_tags
         """
 
+        super().__init__()
         self.special_token = special_token
         self.special_tokens_dict = {'additional_special_tokens': [self.special_token]}
         self.default_tag = default_tag
 
         if ner_tags is None:
             ner_tags = ['ORG', 'TIME', 'MISC', 'LOC', 'PER', 'NUM']
         self.ner2id = {tag: tag_id for tag_id, tag in enumerate(ner_tags)}
```

## Comparing `kolibri/preprocess/preprocessors/siamese_preprocessor.py` & `kolibri/preprocess/text/siamese_preprocessor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 
 from logging import getLogger
 from typing import List, Union, Iterable, Optional
 
 import numpy as np
 
-from deeppavlov.core.commands.utils import expand_path
-from deeppavlov.core.common.registry import register
-from deeppavlov.core.data.utils import zero_pad_truncate
-from deeppavlov.core.models.component import Component
-from deeppavlov.core.models.estimator import Estimator
+from kdmt.path import expand_path
+from kolibri.registry import register
+from kolibri.utils import zero_pad_truncate
+from kolibri.core.component import Component
+ 
 
 log = getLogger(__name__)
 
 
-@register('siamese_preprocessor')
-class SiamesePreprocessor(Estimator):
+@register('SiamesePreprocessor')
+class SiamesePreprocessor(Component):
     """ Preprocessing of data samples containing text strings to feed them in a siamese network.
 
     First ``num_context_turns`` strings in each data sample corresponds to the dialogue ``context``
     and the rest string(s) in the sample is (are) ``response(s)``.
 
     Args:
         save_path: The parameter is only needed to initialize the base class
-            :class:`~deeppavlov.core.models.serializable.Serializable`.
+            :class:`~kolibri.core.models.serializable.Serializable`.
         load_path: The parameter is only needed to initialize the base class
-            :class:`~deeppavlov.core.models.serializable.Serializable`.
+            :class:`~kolibri.core.models.serializable.Serializable`.
         max_sequence_length: A maximum length of text sequences in tokens.
             Longer sequences will be truncated and shorter ones will be padded.
         dynamic_batch:  Whether to use dynamic batching. If ``True``, the maximum length of a sequence for a batch
             will be equal to the maximum of all sequences lengths from this batch,
             but not higher than ``max_sequence_length``.
         padding: Padding. Possible values are ``pre`` and ``post``.
             If set to ``pre`` a sequence will be padded at the beginning.
@@ -37,18 +37,18 @@
             If set to ``pre`` a sequence will be truncated at the beginning.
             If set to ``post`` it will truncated at the end.
         use_matrix: Whether to use a trainable matrix with token (word) embeddings.
         num_context_turns: A number of ``context`` turns in data samples.
         num_ranking_samples: A number of condidates for ranking including positive one.
         add_raw_text: whether add raw text sentences to output data list or not.
             Use with conjunction of models using sentence encoders
-        tokenizer: An instance of one of the :class:`deeppavlov.models.tokenizers`.
-        vocab: An instance of :class:`deeppavlov.core.data.simple_vocab.SimpleVocabulary`.
-        embedder: an instance of one of the :class:`deeppavlov.models.embedders`.
-        sent_vocab: An instance of of :class:`deeppavlov.core.data.simple_vocab.SimpleVocabulary`.
+        tokenizer: An instance of one of the :class:`kolibri.models.tokenizers`.
+        vocab: An instance of :class:`kolibri.core.data.simple_vocab.SimpleVocabulary`.
+        embedder: an instance of one of the :class:`kolibri.models.embedders`.
+        sent_vocab: An instance of of :class:`kolibri.core.data.simple_vocab.SimpleVocabulary`.
             It is used to store all ``responces`` and to find the best ``response``
             to the user ``context`` in the ``interact`` mode.
     """
 
     def __init__(self,
                  save_path: str = './tok.dict',
                  load_path: str = './tok.dict',
@@ -57,17 +57,17 @@
                  padding: str = 'post',
                  truncating: str = 'post',
                  use_matrix: bool = True,
                  num_context_turns: int = 1,
                  num_ranking_samples: int = 1,
                  add_raw_text: bool = False,
                  tokenizer: Component = None,
-                 vocab: Optional[Estimator] = None,
+                 vocab: Optional[Component] = None,
                  embedder: Optional[Component] = None,
-                 sent_vocab: Optional[Estimator] = None,
+                 sent_vocab: Optional[Component] = None,
                  **kwargs):
 
         self.max_sequence_length = max_sequence_length
         self.padding = padding
         self.truncating = truncating
         self.dynamic_batch = dynamic_batch
         self.use_matrix = use_matrix
```

## Comparing `kolibri/preprocess/preprocessors/str_token_reverser.py` & `kolibri/preprocess/text/str_token_reverser.py`

 * *Files identical despite different names*

## Comparing `kolibri/preprocess/preprocessors/str_utf8_encoder.py` & `kolibri/preprocess/text/str_utf8_encoder.py`

 * *Files identical despite different names*

## Comparing `kolibri/preprocess/preprocessors/transformers_preprocessor.py` & `kolibri/preprocess/text/transformers_preprocessor.py`

 * *Files identical despite different names*

## Comparing `kolibri/preprocess/text/email_cleaner.py` & `kolibri/preprocess/text/cleaning/email_cleaner.py`

 * *Files identical despite different names*

## Comparing `test_backup/dnn/text/test_labeling/test_bi_gru_model.py` & `kolibri/backend/tensorflow/tasks/text/labeling/bi_gru_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,70 @@
 # encoding: utf-8
 
-import tests.dnn.text.test_labeling.test_bi_lstm_model as base
-from kolibri.backend.tensorflow.tasks.text.labeling import BiGRU_Model
-from kolibri.tokenizer import WordTokenizer
 
-tokenizer = WordTokenizer()
+from typing import Dict, Any
 
+from tensorflow import keras
 
-class TestBiGRU_Model(base.TestBiLSTM_Model):
+from kolibri.backend.tensorflow.layers import L
+from kolibri.backend.tensorflow.tasks.text.labeling.base_model import BaseLabelingModel
+
+
+class BiGRU_Model(BaseLabelingModel):
 
     @classmethod
-    def setUpClass(cls):
-        cls.EPOCH_COUNT = 1
-        cls.TASK_MODEL_CLASS = BiGRU_Model
-
-    def test_basic_use(self):
-        super(TestBiGRU_Model, self).test_basic_use()
-
-    def test_predict_and_callback(self):
-        from kolibri.data.text.corpus import CONLL2003ENCorpus
-        from kolibri.backend.tensorflow.callbacks import EvalCallBack
-        corpus = CONLL2003ENCorpus()
-        train_x, train_y = corpus.get_data(nb_samples=500)
-        valid_x, valid_y = corpus.get_data(nb_samples=100)
-
-        model = BiGRU_Model(sequence_length=10)
-
-        eval_callback = EvalCallBack(kolibri_model=model,
-                                     x_data=valid_x[:200],
-                                     y_data=valid_y[:200],
-                                     truncating=True,
-                                     step=1)
-
-        model.fit(train_x[:300], train_y[:300],
-                  valid_x[:200], valid_y[:200],
-                  epochs=1,
-                  callbacks=[eval_callback])
-        response = model.predict(train_x[:200], truncating=True)
-        lengths = [len(i) for i in response]
-        assert all([(i <= 10) for i in lengths])
-
-        response = model.predict(train_x[:200])
-        lengths = [len(i) for i in response]
-        assert not all([(i <= 10) for i in lengths])
+    def default_hyper_parameters(cls) -> Dict[str, Dict[str, Any]]:
+        return {
+            'layer_bgru': {
+                'units': 128,
+                'return_sequences': True
+            },
+            'layer_dropout': {
+                'rate': 0.4
+            },
+            'layer_time_distributed': {},
+            'layer_activation': {
+                'activation': 'softmax'
+            }
+        }
+
+    def build_model_arc(self) -> None:
+        output_dim = self.label_processor.vocab_size
+
+        config = self.hyper_parameters
+        embed_model = self.embedding.embed_model
+
+        layer_stack = [
+            L.Bidirectional(L.GRU(**config['layer_bgru']), name='layer_bgru'),
+            L.Dropout(**config['layer_dropout'], name='layer_dropout'),
+            L.TimeDistributed(L.Dense(output_dim, **config['layer_time_distributed']), name='layer_time_distributed'),
+            L.Activation(**config['layer_activation'])
+        ]
+
+        tensor = embed_model.output
+        for layer in layer_stack:
+            tensor = layer(tensor)
+
+        self.tf_model = keras.Model(embed_model.inputs, tensor)
 
 
 if __name__ == "__main__":
-    pass
+    from kolibri.data.text.corpus import ChineseDailyNerCorpus
+    from kolibri.backend.tensorflow.callbacks import EvalCallBack
+
+    train_x, train_y = ChineseDailyNerCorpus.load_data('train')
+    valid_x, valid_y = ChineseDailyNerCorpus.load_data('valid')
+    test_x, test_y = ChineseDailyNerCorpus.load_data('test')
+
+    model = BiGRU_Model(sequence_length=10)
+
+    eval_callback = EvalCallBack(kash_model=model,
+                                 x_data=valid_x,
+                                 y_data=valid_y,
+                                 truncating=True,
+                                 step=1)
+
+    model.fit(train_x[:300], train_y[:300], valid_x, valid_y, epochs=1,
+              callbacks=[eval_callback])
+    y = model.predict(train_x[:200])
+    model.tf_model.summary()
+    model.evaluate(test_x, test_y)
```

## Comparing `test_backup/entities/test.py` & `tests/entities/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
-from kolibri.task.text.entities_back.templated_extractor import TemplatedEntityExtractor
-from kolibri.task.text.entities_back import PersonExtractor
-from kolibri.task.text.entities_back.regex_extractor import RegexExtractor
-from kolibri.task.text.entities_back.dictionaryExtractor import DictionaryExtractor
-from kolibri.task.text.entities_back import CommonRegexExtractor
+from kolibri.task.text.entities.templated_extractor import TemplatedEntityExtractor
+from kolibri.task.text.entities import PersonExtractor
+from kolibri.task.text.entities.regex_extractor import RegexExtractor
+from kolibri.task.text.entities.dictionaryExtractor import DictionaryExtractor
+from kolibri.task.text.entities import CommonRegexExtractor
 import csv, operator
 
 template_extractor = TemplatedEntityExtractor('../../data/nga/ressources/entities_Descriptions.csv')
 person_extractor = PersonExtractor()
 # leave_types = DictionaryExtractor('leaveType', 'LeaveType')
 # company_name = DictionaryExtractor('companyNames.csv', 'Company')
```

## Comparing `kolibri_ml-1.1.8.dist-info/METADATA` & `kolibri_ml-1.1.80.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,51 +1,60 @@
 Metadata-Version: 2.1
 Name: kolibri-ml
-Version: 1.1.8
+Version: 1.1.80
 Summary: Deep Learning and more NLP toolkit
 Home-page: 
 Author: Mohamed Ben Haddou
 Author-email: mbenhaddou@mentis.io
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: kdmt (>=1.0.38)
+License-File: LICENCE.txt
+Requires-Dist: kdmt (>=1.0.68)
 Requires-Dist: scikit-learn (==1.1.3)
 Requires-Dist: py-dateinfer
 Requires-Dist: overrides
 Requires-Dist: Pyaml
 Requires-Dist: joblib
 Requires-Dist: tabulate
 Requires-Dist: psutil
 Requires-Dist: imblearn
 Requires-Dist: seaborn
 Requires-Dist: packaging
+Requires-Dist: ipython
+Requires-Dist: pypickle
+Requires-Dist: python-louvain
+Requires-Dist: category-encoders
+Requires-Dist: networkx
+Requires-Dist: dtreeviz
 Requires-Dist: httpcore
 Requires-Dist: httpx
 Requires-Dist: httpx[http2]
 Requires-Dist: xlsxwriter
 Provides-Extra: all
-Requires-Dist: tensorflow ; extra == 'all'
-Requires-Dist: fasttext ; extra == 'all'
 Requires-Dist: gensim ; extra == 'all'
-Requires-Dist: dateparser ; extra == 'all'
-Requires-Dist: ipywidgets ; extra == 'all'
-Requires-Dist: pyLDAvis ; extra == 'all'
 Requires-Dist: sonopy ; extra == 'all'
+Requires-Dist: dateparser ; extra == 'all'
 Requires-Dist: wordcloud ; extra == 'all'
+Requires-Dist: pyLDAvis ; extra == 'all'
+Requires-Dist: ipywidgets ; extra == 'all'
+Requires-Dist: eml-parser ; extra == 'all'
+Requires-Dist: fasttext ; extra == 'all'
+Requires-Dist: tensorflow (==2.8.0) ; extra == 'all'
 Provides-Extra: audio
 Requires-Dist: sonopy ; extra == 'audio'
 Provides-Extra: dnn
-Requires-Dist: tensorflow ; extra == 'dnn'
+Requires-Dist: tensorflow (==2.8.0) ; extra == 'dnn'
 Provides-Extra: nlp
 Requires-Dist: gensim ; extra == 'nlp'
 Requires-Dist: fasttext ; extra == 'nlp'
 Requires-Dist: dateparser ; extra == 'nlp'
+Requires-Dist: eml-parser ; extra == 'nlp'
 Provides-Extra: notebook
 Requires-Dist: ipywidgets ; extra == 'notebook'
 Requires-Dist: pyLDAvis ; extra == 'notebook'
 Requires-Dist: wordcloud ; extra == 'notebook'
 
 # Kolibri
```

## Comparing `kolibri_ml-1.1.8.dist-info/RECORD` & `kolibri_ml-1.1.80.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,210 +1,361 @@
-kolibri/VERSION,sha256=Mz2JqgaMernrf-e6VTh-ArJvr9z6BrYtLkXj0KQ8O5o,6
-kolibri/__init__.py,sha256=-2X2HPVIFeSaVPJ1ja3O8WRLv1D9eQEZcd3BxcSh7uo,3871
-kolibri/app.py,sha256=3wRL1O4N0Nu0C7tW_yA9NYdT14HddQHy-GAC_A5x5uE,16782
+kolibri/.env,sha256=aTGCLQU1hQapds_lZrqczNPt3lbKv_aYKYE2Dl6iso0,18
+kolibri/VERSION,sha256=y_tbezMtYeB6yOtm73HFO7mHkUVJBhU1qxCVghcUg8s,7
+kolibri/__init__.py,sha256=mwGSkniI5XxmXMotgoe9P-jbkM35WtVsyO1uck-TDFg,4358
+kolibri/app.py,sha256=b_vLL8hIcbXgW_F-zOQfllebEiN-VdHsN7nEivYkZBA,16782
 kolibri/config.py,sha256=L1xrnHExgtg3gjE-pl67-BsOTJCtd9a-Gk8cG9FOo6M,3190
 kolibri/config_loader.py,sha256=gsdbv6fd6DU0HHd8aSOOMnOJL5dZJy8_pP2fqBWH_os,1902
-kolibri/default_configs.py,sha256=cI8pL54tDF2DRAawcyeX592uB2EcVgzRMY6Y2wurs7o,3213
-kolibri/errors.py,sha256=-vtNIze-fifEIqjUyEso7Pqc4poHxmMATuAa7-tZveo,3186
+kolibri/default_configs.py,sha256=dGMN3ps9j_GD5C2KVWN5kFhVsIRHY8j5m4LsM3d4Gto,3814
+kolibri/errors.py,sha256=w4CWaoHWprc4NwaG9OmG0QKy8TsjzW40wx6x_p24dT8,5968
 kolibri/logger.py,sha256=bfFKEoKSshW41L2TCOTRDM03uP0RKJJ6ksyjToYaoYc,795
 kolibri/metadata.py,sha256=N-y50guFW7JojwgP0A_sZh-PidHnDk6ih1a3f2qw3TI,2219
-kolibri/model_loader.py,sha256=wY6RRx-u2Og-C-1mMDZsvNv-lwZES0jkCtVcvuwtPLI,9868
-kolibri/model_trainer.py,sha256=GONJV5s0imhy7Cjj8bIw8zNS8BI3Wp5pHNjl_UlnH9g,23844
-kolibri/registry.py,sha256=MJhdN5OZBxj6TCj7cIpwrGjLXJ55nK2mhi323CPFFxI,968
+kolibri/model_loader.py,sha256=8XgjKM-oJ0xqcg3qiZ8uxXIO8-oL3PiRAR47cpEnbiI,10923
+kolibri/model_trainer.py,sha256=4TNiqz2UEl8fNk-hsxHJ_vEeVE5STrT26pfVwHXJiPI,25966
+kolibri/registry.py,sha256=24l7CETeYLPnUjqVFHfiB1sU6T0GAgs7RtZSwwglBPk,2763
 kolibri/requirements.txt,sha256=wl9k0zC_6wMrj1aajNJUdT6mLw9Ow7c-aiS4s_tDVzU,153
-kolibri/settings.yaml,sha256=SlgxRaaWue2Uk0rLQH4-qDr4J_81jGB6xRBJkQ8CdeU,458
+kolibri/settings.py,sha256=3-sXHEqp36xsV7y0U5GNrc5vjaLGJY23IyYJc3xIgFw,2490
+kolibri/settings.yaml,sha256=SbFpPQw3EeZc0W7GF9oyzIPIbVXMBSn7OyFnTT-ndwM,457
+kolibri/types.py,sha256=owjp0xUWDyV6yN3zuAZ8zdouU6LUS47yH5N3vLhi8TQ,361
+kolibri/version.py,sha256=O9Da2-eXuC6viLld4Vv9fFKJbZiQtCyH3j5t_xQNx3g,166
 kolibri/api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/api/classification/__init__.py,sha256=_a-0VMXP0GdHBVKAj29d7aip0jfl2j7_HU-C17YMHvQ,2707
 kolibri/autolearn/__init__.py,sha256=Rv8ku1zDQlJFmPGGJgFGuy2odOmhXqlCNLoLH_fOWxc,66
 kolibri/autolearn/metalearn/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/autolearn/metalearn/metafeature.py,sha256=wXK9VbJ0msW8V_Bwdq0Po4dNQ1GnH2Ix3jaTeBTjqKw,3125
 kolibri/autolearn/metalearn/metafeatures.py,sha256=d43ZAEYIvrdRLPu4tPNYh1A6PD9YAAUySLUommeyiwU,46866
 kolibri/autolearn/model_zoo/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/autolearn/model_zoo/zoo_classifier.py,sha256=2RxezAcf3vbW3qwP4qKca_5ghh8HBVb813WFvAOTmPY,4737
-kolibri/autolearn/model_zoo/zoo_regressor.py,sha256=MVQ6UwcPnnhwesSF_Mz8CdArS1ZZsJ_0TQrRLyDqBqU,4310
-kolibri/backend/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolibri/backend/models.py,sha256=N5hffNAnXkDThhEAQqiIAhEDqVp450z4wg7Bf2jEtVs,6289
+kolibri/autolearn/model_zoo/zoo_estimator.py,sha256=RI9CZ_GwtkqyXkc7HeZCPCTpdiSG6lNbgP6WVatCeCo,5940
+kolibri/autolearn/model_zoo/zoo_regressor.py,sha256=qw-NLhgR12JO7aKuqtisU7pItiJ1WFeUOMKiT80d62o,4246
+kolibri/automl/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+kolibri/automl/data_inspection.py,sha256=vV2ShQbbCTzYfNuaTT86dxRHPxkgIREJuJ5szV3ecK0,15341
+kolibri/backend/__init__.py,sha256=vrTpplaj6Gj_ZxqkcGYU3dV1FLhTc5yiSH4VUlmZ8VY,50
+kolibri/backend/models.py,sha256=X_olXosRAjLWgMIjR5blSzvy-HK-UJTT2RlJr5PiYA0,6230
 kolibri/backend/base/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/backend/base/base_classifier.py,sha256=LJol6p3yRqPgiUtAIFnRLgNInepIKLTvzUhokhcod18,11843
 kolibri/backend/base/base_clustering.py,sha256=-qOmW2V1nZga_xmNYf66MSy20KjMRadc8JGpPujTHE0,3916
-kolibri/backend/base/base_estimator.py,sha256=7x1G3E5aKeH4DcAI6SdoXCwsikLQpHBhjWNiUIV9paI,30343
-kolibri/backend/base/base_regressor.py,sha256=N7OopZB33zNgSGUA0Z5ZB5pV5Xdp6meZ-CVMWprror0,7481
-kolibri/backend/sklearn/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+kolibri/backend/base/base_estimator.py,sha256=PMhttjNiutM6f3CpGZEVyVVuqISq4ssJ-9FpgVdYCEU,30869
+kolibri/backend/base/base_regressor.py,sha256=OjIqHPSouzLV3Q4lbK1qTJ-vntDQ-Zn1MDipP-JVXW8,7677
+kolibri/backend/base/estimator.py,sha256=jqCjFFH3TvZspLJ1uzo2hDO_meLBNWCL4r59QCyNv0o,14321
+kolibri/backend/base/nn_model.py,sha256=Azfnt31dNnV7cpS1RvV3XGLNhRUGvqHSIkbaEKjKqYc,912
+kolibri/backend/bn/BayesianModel.py,sha256=2MsqjQ-T-c2yucpATa5qQJFGvkmDD4o-nSII6GhhRhs,449
+kolibri/backend/bn/BayesianNetwork.py,sha256=o9io0ndF2_MAX-ka8SPMIkqtMgazwl4NOGBJc3Vprls,44071
+kolibri/backend/bn/CPD.py,sha256=NgnqTgX-Mff2DWs5-xHdiK00wNz6QPvJiZSrj3tzAd8,24029
+kolibri/backend/bn/ContinuousFactor.py,sha256=oYzPEf5Q2SwnPMakyrk92WJQindhP-YCKp-9BiNJOn0,8931
+kolibri/backend/bn/DAG.py,sha256=0Sm6db1YnPZjd5pqF882_nBzUFENlcvV02ap4CuEK34,40531
+kolibri/backend/bn/DiscreteFactor.py,sha256=U3dYFwSC_5l3gjLnVB41w93jtZrOcfk-3wMDb_tn-rE,28630
+kolibri/backend/bn/DynamicBayesianNetwork.py,sha256=AEOnPTAklDg_1TEN5dKbx3SFURED6u_qocTSgod3T0I,31370
+kolibri/backend/bn/EliminationOrder.py,sha256=2X6jAe36fNhD_9Iby4saCt93EZeau6ljrHNLdHxatwc,4289
+kolibri/backend/bn/ExactInference.py,sha256=yuQ1-Dy4iaICDAi__O6TJoiNWPsj0moQ6OJDSPDrGb8,39930
+kolibri/backend/bn/FactorGraph.py,sha256=EIFgOsLi9sizmd0QI4e16lLRBSHHY1VjscTEtlbvA4s,10515
+kolibri/backend/bn/Independencies.py,sha256=5vy2hq4G5pKTomxlft8cBEbltX6--RvJMSEDWUyIhys,14252
+kolibri/backend/bn/JointProbabilityDistribution.py,sha256=DRh6-IwKqeXQbtnhmUUXE0O7OJteGvrplMXHvMTZWTI,11089
+kolibri/backend/bn/JunctionTree.py,sha256=mej5cnKF98aBzH-2WGZyutxIN4pORhd2MjcJeipnueI,3058
+kolibri/backend/bn/LinearGaussianCPD.py,sha256=7j3SeUW9EwWj_-JYFtE2GL9p_gqIqihibGRwB7FbLzU,8219
+kolibri/backend/bn/MarkovChain.py,sha256=nsheozassHYfDmLyTfb4rnv1xDZu2BzRaHcV9uv60cM,13783
+kolibri/backend/bn/MarkovNetwork.py,sha256=-QuZCL9fQfAqI0GkfdAOmAssXL32l2VeXf48GPLxE18,17804
+kolibri/backend/bn/NaiveBayes.py,sha256=5uq4O5XTbzE4fvaOFnVcE-G-6EyUx9rSzXlQ3wkLeSM,5791
+kolibri/backend/bn/Sampling.py,sha256=5zBg4faFCuh58lmC3UjORvy8Cc3B3MAx_5fL-IVkAIk,24083
+kolibri/backend/bn/UndirectedGraph.py,sha256=QLHsIGiHhUUN4gtKhyzmaSNP3iTlYrqmifpi34iMwoA,9237
+kolibri/backend/bn/__init__.py,sha256=hO8OUTdSX5KFWbJLgnVJSzNp1ZmvksjK7EudQ7QNAf0,723
+kolibri/backend/bn/base_estimator.py,sha256=m84EGYF9sbkSyDuT8iLqG6nvAH8TWYPBqeaKAp8DVd4,11145
+kolibri/backend/bn/base_inference.py,sha256=K7dJ6kTWem0RU5KBIBm-y6oP92uXKQLyDtqaup7H-U8,7604
+kolibri/backend/bn/bnlearn.py,sha256=Q2RYcNWOEPRhE465JWZlVQO79rntcOZfhugsifRDyT0,48039
+kolibri/backend/bn/factors_base.py,sha256=PcCTyEM_ZDN-N0G3rI2dd6vVSxPQH-j7xXLevrSmuTQ,3207
+kolibri/backend/bn/metrics.py,sha256=ArPv8rfBW2BQ0BH6ZnwEZZu9W5_nfTPYORgV_3TCkoE,2348
+kolibri/backend/bn/network.py,sha256=1VxiK5oknn5cBbfCdHI12BndnSx5d0JtzKi3pD7Z1M4,16476
+kolibri/backend/bn/state_name.py,sha256=aCjVrWKWCCiqAzM7Q7Vfct2p2CML6p1O0mXapEI1G04,3178
+kolibri/backend/bn/tabulate.py,sha256=k_Ou99XJNH2it6hZ4Nzt3YvzLgz3XKG1D9-qKzn4DLg,30222
+kolibri/backend/bn/utils.py,sha256=cP5uGJfZdyCP1SQPRyyTvq4M6seB0z3uTPMKNY0UGUw,5326
+kolibri/backend/bn/distributions/CanonicalDistribution.py,sha256=qGT9ii7-GGZ3zcS4O8ZBDiXZuULPWr_fbvgutFmcbCg,13476
+kolibri/backend/bn/distributions/CustomDistribution.py,sha256=f6xEJw63T4WHoHrDt9ZWlMuCC3LQ4a43_I7IE8bBy64,11847
+kolibri/backend/bn/distributions/GaussianDistribution.py,sha256=Pj50Posi4vzjJLFIpMSExxrrsvvLY3haqkrEX2tPWYY,19195
+kolibri/backend/bn/distributions/__init__.py,sha256=ihRaaLuyWXf2qwNwqftZJCwvXA_MXlPAVvT3hAYU-pk,220
+kolibri/backend/bn/distributions/base.py,sha256=CXf_67u3WHYgKLNbhGNEx7-tpVAWMkPDGrTEcvhAehg,841
+kolibri/backend/bn/estimators/HillClimbSearch.py,sha256=OxPQ9hu0lxaylrnZyQ5HlOEd3v6kG3DlI3RitVGmHlk,12715
+kolibri/backend/bn/estimators/MLE.py,sha256=_0Uf-rWZjUasKG6vt-XcFkaHIz5RizbgqBjEfJl8AiY,4805
+kolibri/backend/bn/estimators/ScoreCache.py,sha256=bu4TyYobeHOejQBDO0fnZmXXSf5uaCiO4eYxQhAqEhU,4221
+kolibri/backend/bn/estimators/StructureScore.py,sha256=dwoSCsRCe06Tbh-4sO2EHFQ7AUImgT_e3axwG9dHQL0,18012
+kolibri/backend/bn/estimators/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+kolibri/backend/bn/estimators/bayesianEstimator.py,sha256=foLuPdAXpnWj8MRbUAsHb1XabmL5Xj5GIhS-2x7IzJQ,7985
+kolibri/backend/bn/inference/__init__.py,sha256=wJHbKVRcGDRG5C8-G0IJ0_PtReqY7cC6opbetliJc3Q,57
+kolibri/backend/bn/inference/inference.py,sha256=IKyJdEpc-S_zI2aKGUMLdhjAXJdxmMUHXaHIxYXr3fg,3044
+kolibri/backend/bn/inference/predict.py,sha256=XIhSX0vWxB7I5UKvURes4Ej9XINzBlvZTPNhxFHVf3c,194
+kolibri/backend/bn/parameters/__init__.py,sha256=unCZOHhHIFHVeUor8gF6XOLgkkjgBG2vJqylCXes9AI,130
+kolibri/backend/bn/parameters/learn.py,sha256=c8tICnYX82YDe8p7oY2jZ1d67rHWtU5wZMQQr57YBXw,490
+kolibri/backend/bn/parameters/parameter_learning.py,sha256=Cps86a2K94Ut6NE7mZ7HRaaJEZRWVrf9gF9x4Og0RJ0,12213
+kolibri/backend/bn/readwrite/BIF.py,sha256=Q5VD6URTCNTQNsjeZ6HB7WAxZDmcLnX4x-z4Rrs0YiA,18288
+kolibri/backend/bn/readwrite/UAI.py,sha256=KaGm2IsE6DMVwUZRUVDHyzJJHT-piaI8gW35XJRJTQk,14034
+kolibri/backend/bn/readwrite/XMLBIF.py,sha256=DObvwK5o-up5a6YL-GDhT31tmKXjXpBO8C0jk-hVGF0,16390
+kolibri/backend/bn/readwrite/__init__.py,sha256=U4aRmO-WAXL4bp-MsNpzh_N1bTDKH86lw-tqyepW__U,491
+kolibri/backend/bn/structure/__init__.py,sha256=Mh_6WEKPgDBeg0vjCkTDg1dFaxudnKIu0bS7xcbE8jI,311
+kolibri/backend/bn/structure/base.py,sha256=EMm4nD8W9rpj3Q0DYs0Vaoq6DnuAh61B0P-HPLJmy1E,7020
+kolibri/backend/bn/structure/evaluation.py,sha256=LrP8zqLPDb5QrDgxN3ffBPH1vGuJ80D88FKN-yD0QCE,8354
+kolibri/backend/bn/structure/learn.py,sha256=CjM-CTEDmnYnT9faPPI3xsaY27VJyyKqdLtJxi52lhM,1989
+kolibri/backend/bn/structure/linear.py,sha256=hQZKQ0ZjbEs17z_5pdSKJ_v-_sdrjNYzyUpfcMIS0mI,7267
+kolibri/backend/bn/structure/low_rank.py,sha256=9sWiZCiiyrkP6Pq0kEVvCoYeJSFdIEWE34VlOlo0Sxg,7902
+kolibri/backend/bn/structure/no_tears.py,sha256=TywuREMPmoZMzNmo76VQ4nDX9dAoaIUWjFdc0TGFobs,22607
+kolibri/backend/bn/structure/no_tears_tf.py,sha256=_gSzC9gALIqnufrlgFloQdTVAoVBpno8rA5XIutVse4,2961
+kolibri/backend/bn/structure/no_tears_tf2.py,sha256=vHegAFKIhm-gzPanlSjdZNADSzESbengWQ9m5j8CGUE,1898
+kolibri/backend/bn/structure/no_tears_tf_bak.py,sha256=_gSzC9gALIqnufrlgFloQdTVAoVBpno8rA5XIutVse4,2961
+kolibri/backend/bn/structure/nonlinear.py,sha256=wsdBgGZEzzVYR63tbE2gq62zCWzh8u2-QRaNty6KyNY,8816
+kolibri/backend/bn/structure/notears_tf2.py,sha256=arZKt0xa4rOHtheMaIe-1RgwtAH7WUR5N5LRsg7azWU,4376
+kolibri/backend/bn/structure/plot_dag.py,sha256=JyFCcgnR53yzAuxr8jJ3RHEw-KxKSA6C85Gp0n5ierc,4208
+kolibri/backend/bn/structure/structure_model.py,sha256=0IDc08xa5o-TygQ0iySFRPjXHFnpisMBRR0XUjsV1ls,13671
+kolibri/backend/generators/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+kolibri/backend/sklearn/__init__.py,sha256=7aIw8aWCxKcGFPNfJHiqNxdIkDlO3f_FNOr4TVyX9-g,157
+kolibri/backend/sklearn/extensions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+kolibri/backend/sklearn/extensions/decision_tree_log_reg.py,sha256=s-JImpaPsxEfe5ywRXpeGXDrstVY_irVlXiRARBuB9c,18744
+kolibri/backend/sklearn/extensions/distributed_nn.py,sha256=iWW_5haFKBzCKqbirwi9306c0cW18JF9w0wJu9rPNyI,1100
+kolibri/backend/sklearn/extensions/lazy_learner.py,sha256=fmG4FGZAdajTpX8kzZda1CmZ2qfLWzdILv91btJbI-A,15651
+kolibri/backend/sklearn/extensions/lookup_learner.py,sha256=Q-_DVoStwFZz-PHjzuY7E7fmMBBOP2UbMbmQ1WjrVqU,14524
 kolibri/backend/sklearn/meta/__init__.py,sha256=YvrffJMeN_MHWddQAwtasEzhYfOp372p-9s1YLG_kxI,65
 kolibri/backend/sklearn/meta/chain_model.py,sha256=nslunEUGQm5DArP8SrmS24xsENZyyaqniIu90pAIEvc,13257
-kolibri/backend/sklearn/meta/ecoc_model.py,sha256=b9gQeXL_vN17i3n4_xQfnxmmVH1wRQBAGd2ryI7wUi4,28314
+kolibri/backend/sklearn/meta/ecoc_model.py,sha256=WOK53WGKHU9LfGPzLgSM-v79LnBslQrFkdZEEGbS4ZI,28317
 kolibri/backend/sklearn/meta/ensemble_samplers.py,sha256=5uowHV8wkHha5D25VgCjclxdMfaFYwhLW4SjTDgxgDw,28328
 kolibri/backend/sklearn/meta/multi_output_estimator.py,sha256=uWFw6Jyg_jl8lQbnHj6lcNL2aH6sqG6BBOn1UbsCt0c,7646
 kolibri/backend/sklearn/meta/ecoc/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/backend/sklearn/meta/ecoc/code_matrix.py,sha256=Ls1UyCt3zI5WMKDSsSJYhwlNmxy7flbNBXX6ExOvDwk,8616
 kolibri/backend/sklearn/meta/ecoc/criterion.py,sha256=7HFXDTufc5poIo0F-PnEFxK-tc3wDGvTMYJ09RXrDsA,5551
-kolibri/backend/sklearn/meta/ecoc/decoder.py,sha256=tbyglJ-WzNFHCDKRrFS5IDnji8rKsKUqRSyCxs3_iz0,9089
+kolibri/backend/sklearn/meta/ecoc/decoder.py,sha256=5fRtGc5NDt1TCqJc2btq-izLS4OsQxI_tv9zz7JLYDg,9095
 kolibri/backend/sklearn/meta/ecoc/sffs.py,sha256=G9Z2RvEYLTx9zl6EZUfPhfHiB7fgGZRKgxspjzOGULk,3869
-kolibri/backend/tensorflow/__init__.py,sha256=ItIrJ1Xu1U1nguuxdas0BS5_p3RRBP5BdJzwgj0BWXw,2625
-kolibri/backend/tensorflow/callbacks.py,sha256=0PFypWkZ2Ip-5U6RnVXTnb1yx4iguKOJXtlJNmKeVQ4,2111
-kolibri/backend/tensorflow/custom_loses.py,sha256=w2Qgt8z7Wz2T5Tk6x9kDzwgfhK4Y2sv2iuijpXgL-A4,2959
-kolibri/backend/tensorflow/loader.py,sha256=PbWK-UwVU26Ci-oBf1DetPabf633n6QRwUW7YhCqDv4,9632
-kolibri/backend/tensorflow/loader_albert.py,sha256=c0aID0CwZlW1XB8Sgwxbp_KpiMRuk_Wpgv65sNew1Z4,14280
-kolibri/backend/tensorflow/utils.py,sha256=pG3EVrEYOQH-FbEYWp6ELupbRl9zjDsphbqMIpEFWEo,9030
-kolibri/backend/tensorflow/autoencoder/__init__.py,sha256=kRfUV3aE0pmpUuq2oUlJaHl4zAcJNI3v2oGfVylbcHs,354
-kolibri/backend/tensorflow/autoencoder/base_autoencoder.py,sha256=EdYbfiW3snQJnx6VKDIZ8AxlTkK8w6ydX3DSmPHWweI,6654
-kolibri/backend/tensorflow/autoencoder/conv_autoencoder.py,sha256=_LnMWdxF-b8vGzkV2gcEfvfdF1C1ZVvzWY4DQfYIOfQ,3338
-kolibri/backend/tensorflow/autoencoder/deep_autoencoder.py,sha256=M4HjbHUoVaqFZLwmT4NYf4qeJX6S_cAnxwenvad5C9w,2601
-kolibri/backend/tensorflow/autoencoder/variational_autoencoder.py,sha256=KfUe8gmYwLzoOuztxxjmnklwnFK9TMDTFV8zgzJauZY,3749
-kolibri/backend/tensorflow/autoencoder/decoders/__init__.py,sha256=CSv3-1ObAJX439tFdSyXrlMiBdDKGRzQHOO980--huo,148
-kolibri/backend/tensorflow/autoencoder/decoders/att_gru_decoder.py,sha256=xMrpuZqo6NGpJg43_H_V782WIvuUkgeNSnlGOvJi6nI,2043
-kolibri/backend/tensorflow/autoencoder/decoders/gru_decoder.py,sha256=giAdnPRXA08A45LHOCjNBdLcNoFjZsQ1oUyWN678GUI,1265
-kolibri/backend/tensorflow/autoencoder/decoders/lstm_decoder.py,sha256=3cCE0fXkMts6tcGUqJAyfXGaPBSZxwJcu9ewbcQicE4,1118
-kolibri/backend/tensorflow/autoencoder/encoders/__init__.py,sha256=-cwNaSoKW3UOUUF3MkACsvBEP_HOioFet7VJ4gz0CWc,199
-kolibri/backend/tensorflow/autoencoder/encoders/gru_encoder.py,sha256=oZeAOKu_dI-vOReoBda8Me9_BhzGoTGZWiMn62vROLc,2159
-kolibri/backend/tensorflow/autoencoder/encoders/lstm_encoder.py,sha256=8WNqVWOKAfrXT1DSHExJaQj-VS8Y0TLaeDOKNOllOwc,1317
-kolibri/backend/tensorflow/callbacks/__init__.py,sha256=Sp9G9M068a8WY0YaQIKI5T1mEF-yE_gwDmDyQTTQzMs,113
-kolibri/backend/tensorflow/callbacks/connl_callBack.py,sha256=KSZJukRn2nUv_y5odhmFAXa9FR9xFADsI5X_ZmYlMGc,2025
-kolibri/backend/tensorflow/callbacks/eval_callBack.py,sha256=np38gh7oLLDn8WucdQwrTV7q2GiIS9mVvHIQfUErk20,2249
-kolibri/backend/tensorflow/cells/BayesianLSTM.py,sha256=rm-bsTIre4T6CJ9Pt4fOa7zjQ_72LV7TYzu-8tmKh_4,1600
-kolibri/backend/tensorflow/cells/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolibri/backend/tensorflow/cells/variational_posterior.py,sha256=7Glp5gcBnZJMTJeKI3ERXrNc2BD_CGGW2V-HQLDPIvc,2566
-kolibri/backend/tensorflow/embeddings/__init__.py,sha256=N6h3A8foPkIVSHSyge7Uh5cjdsd5nik5P5N9qieswII,425
-kolibri/backend/tensorflow/embeddings/base_embedding.py,sha256=xEOa1uO6YUlVi1j_7CdIxbXyRjRlQ8q51F3ahM0NHWc,8491
-kolibri/backend/tensorflow/embeddings/bert_embedding.py,sha256=If-3cGxM4WD8NEaRMXmVBLwukz02ysI7NyQHnm4SO_A,1448
-kolibri/backend/tensorflow/embeddings/default_embedding.py,sha256=iru8KmlUyS6-iHTKQUWlFGXckfjh3eLKi5HF7hgHVb0,2326
+kolibri/backend/tensorflow/__init__.py,sha256=vCRlW9nQhyP18aVGwa0KQi52kEm-EVSiTho0NCachFU,2953
+kolibri/backend/tensorflow/logger.py,sha256=mIDKhGDgVbLYClY1MeHYBytnsbimixhWIfd8MZkLjjY,519
+kolibri/backend/tensorflow/macros.py,sha256=3iYF50U3XQhILEwYABrBbm5j8468jMEhsu3sR-5tU8A,308
+kolibri/backend/tensorflow/autoencoder/__init__.py,sha256=ljG8rr0kd8lzv2UvHiOxe-9ZdxfhVLZAkAaMR5RCT6Y,457
+kolibri/backend/tensorflow/autoencoder/base_autoencoder.py,sha256=5-jDr1Uj2QpOJWdiNG6vjx47txDs2moBvi8OZihHwiU,6848
+kolibri/backend/tensorflow/autoencoder/conv_autoencoder.py,sha256=uCZDD1oeIJeNrIS4NgV1EVCbJQZ2LdqJK7h0bmO7F4E,3339
+kolibri/backend/tensorflow/autoencoder/deep_autoencoder.py,sha256=DZMSVTSk1Xjk7PzK2BeTVEJW2WplLuX_KDcqwnEjuWw,2611
+kolibri/backend/tensorflow/autoencoder/variational_autoencoder.py,sha256=FSBGKiAS307TIH_I85WBjn3SBxjp3A9AytQIqFt2_ac,3757
+kolibri/backend/tensorflow/autoencoder/decoders/__init__.py,sha256=2BWM88rhuedNX22STALJxJ3LleHAjybO8ru5Ol0d_aw,204
+kolibri/backend/tensorflow/autoencoder/decoders/att_gru_decoder.py,sha256=8E5qZrw4YLaKFBse9FBDTUD5l5MkNVxr7KxEQpP0CxY,2091
+kolibri/backend/tensorflow/autoencoder/decoders/gru_decoder.py,sha256=xpnZnoAkuPchs89m4ThhgEZj0rYF7kn96hw2xHQ_IbY,1294
+kolibri/backend/tensorflow/autoencoder/decoders/lstm_decoder.py,sha256=TAYOeWEhIPwWcbIRZlo_GM3fSekm8nJYEpg8GFfk-p0,1213
+kolibri/backend/tensorflow/autoencoder/encoders/__init__.py,sha256=XDh6fCzRjMrTQuZ0qb2ChTi8KA9YEY5VXaOTxVoRZGE,92
+kolibri/backend/tensorflow/autoencoder/encoders/gru_encoder.py,sha256=rdHSzFgsY7cwTSxQd35vjLwCTxmk_l5PgoBmKORx4P0,1257
+kolibri/backend/tensorflow/autoencoder/encoders/lstm_encoder.py,sha256=kJxhlOvDEcxgjoMtZPkO9sDuBp8EUI-q0THi16apY9U,1383
+kolibri/backend/tensorflow/callbacks/__init__.py,sha256=qzKWL5aDS7BsxqREC5JgnLvj2djS-mUnPDuPsdZNwAM,134
+kolibri/backend/tensorflow/callbacks/conll_call_back.py,sha256=KSZJukRn2nUv_y5odhmFAXa9FR9xFADsI5X_ZmYlMGc,2025
+kolibri/backend/tensorflow/callbacks/eval_callBack.py,sha256=-kuX4V2pStjrOWVKfd-NlFasLrYRGNXjQOAzchFcPC8,2241
+kolibri/backend/tensorflow/callbacks/save_callback.py,sha256=-E2B1pPCCY_jdEbm3ReKrCUlZ13pd7l5m_fZe4a67MA,4874
+kolibri/backend/tensorflow/embeddings/__init__.py,sha256=pun_hnzPUhD3zUQktHBJRMvXsGpl9n29qySsSsNmiQA,320
+kolibri/backend/tensorflow/embeddings/bare_embedding.py,sha256=ht4TnnkkyOmPB-3Jdf2B4giY5tDMIvEy4HiAzthjWHA,1709
+kolibri/backend/tensorflow/embeddings/base_embedding.py,sha256=YVcEMgaEeo_TntJnioVfl_OOdtYE1O18aJbRD-gZ0Tc,4676
+kolibri/backend/tensorflow/embeddings/bert_embedding.py,sha256=GdKNLhq47N7Lxr9m-CvixN3Q4Ct1M_WqKNAWKNUraoY,1322
 kolibri/backend/tensorflow/embeddings/elmo_embedding.py,sha256=Fsq2TWjBwk287L9mO_I-Uxsy7oWB3Dcd-r2Yu3olUYA,8420
 kolibri/backend/tensorflow/embeddings/embedding_trainer.py,sha256=t-Xredb4fGiNC9jqcoJW7C7ohCl92xAK77MDe1V55WI,3196
 kolibri/backend/tensorflow/embeddings/fasttext_embedding.py,sha256=VExjnMkrBll06Pmu1o1HETmUs-41TCn0rmQe3azltm4,1952
 kolibri/backend/tensorflow/embeddings/glove_embedding.py,sha256=a_bMbd5019rbD7wsAfmOZXdEXmbtHA-ShxmnuDISTco,2568
-kolibri/backend/tensorflow/embeddings/numeric_feature_embedding.py,sha256=dZvVHHSD0V4Gx6nf5PBv1Mt7xFqIDc2V5guZJ_yoj5g,4156
-kolibri/backend/tensorflow/embeddings/stacked_embedding.py,sha256=oSh-hJJpNEfVs8K-dvNzmREsOxOFFAqaJfYG_1tNcQk,4987
-kolibri/backend/tensorflow/embeddings/transformer_embedding.py,sha256=aSU7nVBlWJN5xCWfDjTEjxgRBXfkBc2qI6dDvhXhULo,3801
-kolibri/backend/tensorflow/embeddings/word_embedding.py,sha256=C1Xop1oFjrYF5Sa_3Q1y6aJhpdsc7qQ34L_5iKwiLfk,3331
-kolibri/backend/tensorflow/layers/__init__.py,sha256=-r9D7L9wioKLWW1RcAQQYkViILyDyZPnaAUhoRjkq6o,744
+kolibri/backend/tensorflow/embeddings/loader.py,sha256=e_niAWXtWglCagG7ms_CzoawzgS9pzLx-EX4wJWlu3U,9637
+kolibri/backend/tensorflow/embeddings/loader_albert.py,sha256=KbPbjRBo28brEyq9_p5MFxX_hsbdj2IG5J-C7TbHKjE,14296
+kolibri/backend/tensorflow/embeddings/numeric_feature_embedding.py,sha256=sjWFqABEMEITRSRxwOU4WVRjzlBvGq1i6mX7TVmfQag,4114
+kolibri/backend/tensorflow/embeddings/stacked_embedding.py,sha256=JkSfsT9IMhoeOEjR58V8BdlcpHyhj2B84N_2TkDvWOg,4911
+kolibri/backend/tensorflow/embeddings/transformer_embedding.py,sha256=QRjIe9Iq9e8sPswKUKBRckUJxttqlB4tKQZEX-LwuIE,3830
+kolibri/backend/tensorflow/embeddings/word_embedding.py,sha256=6VSWXsGEIb8HYfXiHXOMUSi6MFOzyg6XgMcCk3i1c3c,3346
+kolibri/backend/tensorflow/gan/__init__.py,sha256=4d0YebKdS_hClZLer85CixOugbxLNYQl-73-EfSr5ss,679
+kolibri/backend/tensorflow/gan/_transformer.py,sha256=fTCMaEDGJxa9wy7S2LkBRPRuQ3VFu5cAKhcjQr5vsKo,15332
+kolibri/backend/tensorflow/gan/bgm.py,sha256=OhuQcT0FWRGXxBko2THxrRR9fT8fk8YomunhV7OAmXk,462
+kolibri/backend/tensorflow/gan/discriminator.py,sha256=jb3HtwUIvIugdFb0jwN4I4VATZWWzCxQZKjXS54syCQ,3406
+kolibri/backend/tensorflow/gan/generator.py,sha256=Yn99viZYOyLnBhw4uKUW4yl7agem5jrjEMGIFkpFM7A,2727
+kolibri/backend/tensorflow/gan/ohe.py,sha256=kaYE19uoM41X6PXTo9KB-JVwhxxHKpPiw5HFQmoSn5o,412
+kolibri/backend/tensorflow/layers/__init__.py,sha256=lTfOthWKGGZsRTHNbtsaguyR_JNPuJ35BNfHlm8cRuc,1015
 kolibri/backend/tensorflow/layers/att_wgt_avg_layer.py,sha256=HN4m_U7LvruBjgY1XMbEoP2Lz4JjFSW3eh_Dn89od88,3258
-kolibri/backend/tensorflow/layers/behdanau_attention.py,sha256=OEDvvOYk_MlKDzrQYSTW_6vaPOyFnp0PWtW2D7en8YU,1387
-kolibri/backend/tensorflow/layers/bert_embeddings.py,sha256=rWFylL3vxzjqPbv-KvrfzfOUcsvrSDadKxRJXaoUa34,10697
-kolibri/backend/tensorflow/layers/crf.py,sha256=ciM5cItJietiKXdV_T8pFyKJ6HTyiO5ny5OcnQ0jTMs,4390
+kolibri/backend/tensorflow/layers/behdanau_attention.py,sha256=LqynH1Nf0SlDLwynvxgP4lw68qfGABeVGbtHPZzYgBA,1528
+kolibri/backend/tensorflow/layers/conditional_random_field.py,sha256=ZeBvFDvHxhwlPbU80DjwYd5j7OB6h0nX093ZIxNnKjs,4389
 kolibri/backend/tensorflow/layers/folding_layer.py,sha256=wAvNGVNKAXfn-ps-TLfV6EP9dbDIr8UaoA9F9mZTe0c,1047
+kolibri/backend/tensorflow/layers/gen_activation.py,sha256=IJ6JCRyngZjp6n1cBlv7JsvcJjNJw7N4Or_b_6WuHxI,4173
 kolibri/backend/tensorflow/layers/highway_layer.py,sha256=RxlUg9r01S65G1pgyeK6aVNMrWlTjW6rPAjAZQTpIKw,2033
 kolibri/backend/tensorflow/layers/kmax_pool_layer.py,sha256=XAXVMMLFZJa5K2ntVq5XlOy-60e908wv03CRMDxz4tc,3088
-kolibri/backend/tensorflow/layers/layer.py,sha256=f-GAhehhePDjf5IyZhvYnrlJtPDPKzgRuXQaK-SFoCs,916
+kolibri/backend/tensorflow/layers/layer_utils.py,sha256=T4TnqlBg18uLYegBLmfdJCYWexig5sf_pxxH87KbJcA,1129
 kolibri/backend/tensorflow/layers/multi_head_attention.py,sha256=EPaIQIzM7aCjsftfiQizaxVxSqwtDOYH2FQkCXsMIVA,5012
 kolibri/backend/tensorflow/layers/non_masking_layer.py,sha256=gb9TKmq-QFi_EqlkkK7gX-n298dW0sodz7PrODY8zrU,787
-kolibri/backend/tensorflow/tasks/__init__.py,sha256=Rs0UuxeHt9Wp9Dp2RLMyPVuMrVLDEcfTDi0ARwrU3dY,72
+kolibri/backend/tensorflow/layers/residual.py,sha256=-KG22aSP1tJxl7bntdLeTkaLxwOpr2HjuLSK0zvA-yI,1892
+kolibri/backend/tensorflow/losses/__init__.py,sha256=RSw7UHep1cmPMVLZlkAWUUdL1CGHpkpZeFCbmWZJx1s,372
+kolibri/backend/tensorflow/losses/conditional_loss.py,sha256=I0LkaFhF9K-22IDsY3csdOAEdJUz99sQ0GmP-3hDuNk,1416
+kolibri/backend/tensorflow/losses/custom_loses.py,sha256=w2Qgt8z7Wz2T5Tk6x9kDzwgfhK4Y2sv2iuijpXgL-A4,2959
+kolibri/backend/tensorflow/losses/gradient_penalty.py,sha256=oI5V8lxXB723HlIQpM0Jpoa5vGvk0O4dJU8Qwg6_K-s,2299
+kolibri/backend/tensorflow/metrics/__init__.py,sha256=dJ1A79LgJcaV_QhWb3XtBG5Nhd8ziHrgxt0zvHh9HSQ,292
+kolibri/backend/tensorflow/metrics/multi_label_classification.py,sha256=Lfl1SGBvwaNlCcwYAypwTLiWRpvDP3h00e63pWKv3N0,2525
+kolibri/backend/tensorflow/metrics/sequence_labeling.py,sha256=YxPVi5VVk8uHgz58ZG6YO7Ym3Djt2fReOsuDfpdrDV8,14331
+kolibri/backend/tensorflow/tasks/__init__.py,sha256=YiDAjiuz-PHTtYk5TQYKLi6o-z1n55iT8fCz2MOJ7Ug,158
 kolibri/backend/tensorflow/tasks/base_model.py,sha256=65B2aFnfGHdW81NaKYSP7Y3OISpv9RqHuh09TRr9V3I,5384
-kolibri/backend/tensorflow/tasks/dnn_estimator.py,sha256=By1QKu-R3kLTLq9Sg19ZqIrVAuI-l3vKNjwl17ld67I,7406
 kolibri/backend/tensorflow/tasks/structured/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolibri/backend/tensorflow/tasks/structured/base_model.py,sha256=4bpQ8ZLrQiF0LG5TKJoarKKZRbAg2pDprgAhLwbLvPQ,7867
+kolibri/backend/tensorflow/tasks/structured/base_model.py,sha256=B-vi8RUq_PH0OCwjm3oY1L7zgG-QGPKbGSF09aRwiuM,7871
 kolibri/backend/tensorflow/tasks/structured/regression/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolibri/backend/tensorflow/tasks/structured/regression/base_model.py,sha256=86z0a9oqBAqwzu9_HZ88dEIfHnmFl-PcUzD9BdfYeac,4755
-kolibri/backend/tensorflow/tasks/structured/regression/dnn_regression_estimator.py,sha256=W2xhZ0DxLzj-4utoC1u3Y57iZl6CQLXim1mOrvsfLFo,1949
-kolibri/backend/tensorflow/tasks/structured/regression/models.py,sha256=Mr4QhcYDd9R7QwpM1gvFTBX3IVjU3Cll9mFXFjY8G4Q,2750
-kolibri/backend/tensorflow/tasks/text/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-kolibri/backend/tensorflow/tasks/text/base_model.py,sha256=kS2AFHsRAoFaPp6_JduOYDIVR_OWngNFWWA7giUKVqA,6014
-kolibri/backend/tensorflow/tasks/text/classification/__init__.py,sha256=hMFZuTiLnInwxMbPve4uQ49BIawLswayp08cgOrg-XM,22
-kolibri/backend/tensorflow/tasks/text/classification/base_model.py,sha256=oZjBYREvV47oYeF5p_FwNLQPBSBo7Z-UX-yHKU2dK0E,9041
-kolibri/backend/tensorflow/tasks/text/classification/cnn_attention_model.py,sha256=8x2RbOEqOPktZhrAnOIh-aa0GbcIYoBN164M5iHBuFQ,3394
-kolibri/backend/tensorflow/tasks/text/classification/dpcnn_model.py,sha256=IpttaCKuAcSgcTnd7JCF_EQPGKSlF2-cZq3S1h9VnCI,6180
-kolibri/backend/tensorflow/tasks/text/classification/models.py,sha256=EssYI2J4Ctlpf48LmnXFqbgJ2blrd5CSY4GORB_ItQk,28584
-kolibri/backend/tensorflow/tasks/text/classification/multi_input_output_model.py,sha256=iANFvuS5Xtp0OpoPy0pjcO_7FfPrHoOGHAP1ulAH9go,7451
-kolibri/backend/tensorflow/tasks/text/classification/auto/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolibri/backend/tensorflow/tasks/text/classification/auto/models.py,sha256=-Y0R12rBc7_7JPK8VFolgfoi912QD3vYD-a0qjjXpRg,253
-kolibri/backend/tensorflow/tasks/text/labeling/__init__.py,sha256=6aLsH6iz069ah2ZBN9liBYKE1COsPE_9BTQZ0LTwLBQ,120
-kolibri/backend/tensorflow/tasks/text/labeling/base_model.py,sha256=O_sTuwvrIkSn6f_rJDDOSXDqaK-FfMfLJjHuWk3lM08,8548
-kolibri/backend/tensorflow/tasks/text/labeling/experimental.py,sha256=sCJlZVtquZathLDWzirA8IFKVeQ7zCtRbPuXbNC6zF8,3104
-kolibri/backend/tensorflow/tasks/text/labeling/models.py,sha256=aC6mFntQjVtkyb4Po2YLcBCyR5d57JqghuZq4jIQsJ8,9335
-kolibri/backend/tensorflow/tasks/text/seq2seq/__init__.py,sha256=GsayKUERKFOKdAta5cq05-D2-_J4SnV4IXpfeKHQ-Ag,64
-kolibri/backend/tensorflow/tasks/text/seq2seq/model.py,sha256=RLAelNBIydAbX-F_v6fSyaHq7MprWFfsgqpqzYFnx68,13778
-kolibri/backend/tensorflow/transformer/__init__.py,sha256=TqarSL-nyDdzb-QLPdA9FkDZvhtMMQzrFwaNSEbvG5I,9322
-kolibri/backend/tensorflow/transformer/attention.py,sha256=jcDsvmr7J-NGzXMZfUZchO2h5fUgGeAd8maYwznRgdo,6388
-kolibri/backend/tensorflow/transformer/model.py,sha256=Y3KOTmWpy75GdL-JaYayviY_z_8iw4VSAej5ROtV1kY,2957
+kolibri/backend/tensorflow/tasks/structured/regression/base_model.py,sha256=1iHN7zgmYSVU8Nmk7yRdEEddTKWhA-2AT9s9fgPGpUo,4756
+kolibri/backend/tensorflow/tasks/structured/regression/dnn_regression_estimator.py,sha256=1OTqKfyA3ENR5oDpna34giLj-3KP-gw6ls9dYUn52Tc,1929
+kolibri/backend/tensorflow/tasks/structured/regression/models.py,sha256=47GzPOWFmpo5jDM93ofatpvM-CHNFQiNMhikBnH7NSs,2744
+kolibri/backend/tensorflow/tasks/structured/synthetic/__init__.py,sha256=giGGv5q006zyg_mRJ3YMvfD70Cu8G5xaQG5Dam1oYY4,517
+kolibri/backend/tensorflow/tasks/structured/synthetic/_synthesizer.py,sha256=stqks121_GGCrK3HYbSsWKuRFofItGoH49RdpAFVuSE,20393
+kolibri/backend/tensorflow/tasks/text/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+kolibri/backend/tensorflow/tasks/text/classification/__init__.py,sha256=uYlWW1MNO2ExgPqOTAxInwJwcJrYDfdEayKl2dglL_8,417
+kolibri/backend/tensorflow/tasks/text/classification/base_model.py,sha256=EvKrpejqTz1Jpscrw02SI0YfhY8YKK1njitvodytqpc,15208
+kolibri/backend/tensorflow/tasks/text/classification/cnn_attention_model.py,sha256=aD68hdmk7T2xivOJO7L_EqqZ1m6vags-r2-VhX70ajM,3381
+kolibri/backend/tensorflow/tasks/text/classification/dpcnn_model.py,sha256=ZqKBHrCq3MtXffhvKzuy-kYS-aKdVtgMqsq7TmQ1eGA,6196
+kolibri/backend/tensorflow/tasks/text/classification/models.py,sha256=N-V_KnBho6ZrvB-WtFWV6zhb-zjoZ9iL6JcqDJqbWlo,28815
+kolibri/backend/tensorflow/tasks/text/labeling/__init__.py,sha256=xBawfhRs7fLDjoHpNtsBEV9xC7bGz7oMBd3PUMNLrrE,429
+kolibri/backend/tensorflow/tasks/text/labeling/base_model.py,sha256=12QbuknnEotKAtmNW2C-7d7ZYsprJUVHSb1ztkBOFGk,17329
+kolibri/backend/tensorflow/tasks/text/labeling/bi_gru_crf_model.py,sha256=EdfePyM4aSdP1JV8y2NYOBWla4sAlwrOYToGsk4iNIk,2846
+kolibri/backend/tensorflow/tasks/text/labeling/bi_gru_model.py,sha256=0ShDFcG055PKuv3Ts95FFVdY4E_18adSDsjDAd8b8GU,2249
+kolibri/backend/tensorflow/tasks/text/labeling/bi_lstm_crf_model.py,sha256=aeTeNw48JIpMtIk-kFncPT7Aq4SBWYfIg57Epw5fHq0,2991
+kolibri/backend/tensorflow/tasks/text/labeling/bi_lstm_model.py,sha256=qenOQPwgH7alvjQB1usXOzVxjDpLHoXfna2wUipzZU4,2295
+kolibri/backend/tensorflow/tasks/text/labeling/cnn_lstm_model.py,sha256=iukD4J4IUU237iFUlI6DQJi4sJTbq3-kLX_WJYyoDrs,1440
+kolibri/backend/tensorflow/tasks/text/seq2seq/__init__.py,sha256=oAlC4r3AbO9F-FMU9BBU7_y08ytDLdFX_HbvEWsbgT4,84
+kolibri/backend/tensorflow/tasks/text/seq2seq/generator.py,sha256=Rj4vvPHgoSfRO1cL8XNsRtS4ecLWy7RIR0l-RcWdkZA,2443
+kolibri/backend/tensorflow/tasks/text/seq2seq/model.py,sha256=nY0eIEiPnE9Qf4AAVtacrgKCG8cNoocEwLCgM_zqbYI,13913
+kolibri/backend/tensorflow/utils/__init__.py,sha256=DzVFqcCWM7ufMbd5Nz3yVsbJT4GPU1SW5KJjOovBxso,1203
+kolibri/backend/tensorflow/utils/_load_demo.py,sha256=zP1gwDXGjoMbZLihKfY2RQmBGmkOdxEhRK6jtjxPfmQ,740
+kolibri/backend/tensorflow/utils/data.py,sha256=-QbFsfR7mrkqT14XKiaeSIMpeLvxdzqNmcRdK-xsb3c,919
+kolibri/backend/tensorflow/utils/model.py,sha256=1wCouP0vRXvReR__qaCmyl6yrrotlcM7iDiBBt5kHqI,1629
+kolibri/backend/tensorflow/utils/multi_label.py,sha256=Tbdks_UaClvw73eaSi0TBdVxjKzfofBAtT5X_PGE3dQ,1131
+kolibri/backend/tensorflow/utils/serialize.py,sha256=7BNzozD9ri4SxwOpA86CBx6zOSo4Z1TUug8QhES-IFs,862
 kolibri/backend/torch/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/backend/torch/base_model.py,sha256=iemXUwH_6oS-VTQvyZ9MII_4KiTgXdBJmJFhRfL7H44,12666
+kolibri/backend/torch/models.py,sha256=H_iE2AgsZ0YyquBfpY6TzqqYh1XfJM866pY40d2P1EI,8161
 kolibri/backend/torch/utils.py,sha256=-AcqQwgxtSmsC9ZBGkhBUiXb2slTE7-p-2vqGmfmw_o,305
+kolibri/backend/torch/golem_utils/__init__.py,sha256=-fATNCo203nO81sb36u7l2wxPeAoyI6K_rW0UP3EZfU,671
+kolibri/backend/torch/golem_utils/golem_model.py,sha256=sEMXtKXG1GQGm1BP2_2-BmY0wdf4ceXBSS3IZIvzbew,4438
+kolibri/backend/torch/golem_utils/train.py,sha256=apdo4cXdD8Ohdv-v2zp9Q3MhuSU71kV5UAAzPSm9qK4,2545
+kolibri/backend/torch/golem_utils/utils.py,sha256=Yer0BK5mJU4B0A4pqnlhAsoA_LlZ8g-9kuw19VEYYuo,1636
 kolibri/backend/torch/layers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/backend/torch/layers/crf.py,sha256=ToesvgWmCuozItH5lyrh7rHAPlkke_jhkWQTqL7kEAI,5973
 kolibri/backend/torch/tasks/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/backend/torch/tasks/text/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/backend/torch/tasks/text/labeling/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/backend/torch/tasks/text/labeling/bi_lstm_crf.py,sha256=sG-TaWrFUzqD8gvU4zBj6PaLGZQgViPXI58fCEfrzOU,1836
+kolibri/backend/torch/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+kolibri/backend/torch/utils/lbfgsb_scipy.py,sha256=GYuoBToii0T_pLBM5WQ5-UBACsbwD6wsYp0sOH_bwUU,4009
+kolibri/backend/torch/utils/locally_connected.py,sha256=Dbpobd6wAUDT6jKjaTASeSkqzOHCNVXnQpRohECX_g0,2864
+kolibri/bin/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+kolibri/bin/datasets_configs.json,sha256=Kxp26pPdkKw0PMYBP0TrtXGYw76GrCKV3wceLMnYGF8,471
+kolibri/bin/kolibri-download.py,sha256=rNBRMaJqGe7CYu7PQ914JPm31KJFdwy86nQijNmXPIE,2731
 kolibri/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolibri/core/component.py,sha256=Dy0dL5aDy0nlGTZAqUcrO6BnywG2o8Rj4FiHD6Cgf4c,18066
+kolibri/core/component.py,sha256=wA7WjvrwjTX9mKNICljviJvbGjPnJi-AUOzB3p60dH8,18812
+kolibri/core/document.py,sha256=cdzVFthXwfOy6mJ5gZsoKR2LW3yiZXY32fJVyEpFRT0,223
 kolibri/core/entity.py,sha256=yZxwmhwauYfjV-XNJ7Oot2VxlkoZACGcpHvetsQfb0E,1111
-kolibri/core/modules.py,sha256=NFoZIc1ZgDA1J0d2ndcZMNhoDrnh4AY2oWZd_H8sukI,3987
-kolibri/core/pipeline.py,sha256=9ilb4hH5asZ913xw5QahN8ds1Kadta_FEvEZt1tRR64,14623
-kolibri/core/serializable.py,sha256=Fafmw0iN3mDYq5gNzOk7lYckpoHxeWZTCiRwDqvOIi8,2429
+kolibri/core/modules.py,sha256=5VrM8GuhUpRumiekX_xbxnjmQkYpvPUEjeFF6alAC1g,4052
+kolibri/core/pipeline.py,sha256=hHFjzCAMmMBIN86g0EU76s6Kkt18ocMqiiKOJVzHoIw,17570
+kolibri/core/serializable.py,sha256=swVmR9xjz3jS-9oAwXTP1HXk0VSdkLJ02bDiOipgZ7Q,2289
 kolibri/core/vocabulary.py,sha256=0UxUN6DU-1yI3Q0ZsZ_zXW7xCCLF1aCs6F4Bbbx7-EI,5771
 kolibri/data/__init__.py,sha256=wvL5w69hP4g8zuc-XKZ4FtbyFfWtzjbA_aD3sT-yKUM,110
+kolibri/data/auto_downloader.py,sha256=4Sj3RrDSVIjUduox15o45BJNWpOW_p6DvvoNsjrNSmM,4452
+kolibri/data/base_stream.py,sha256=PPW9u8j5MZRi1ImThILOk_j323aDZPuULRbNYki3-Aw,2246
+kolibri/data/blob.py,sha256=sC0uNm34hpOw6oHQ53rYVPlj6TBCOy_ibbb3ElgRuzI,5113
+kolibri/data/dataset.py,sha256=OrpruQm7e6UacDY2WEVhg8on7_ySzzIS72WqDLYWsCY,29540
+kolibri/data/document.py,sha256=0thot_UdGo7SE_fkQB75NA_GmSu2Ews-h12V40ms86s,234
 kolibri/data/downloader.py,sha256=THQtLJtNtHvjC7s-PaPp8KTudsuMubdmuLZE3kfdhcg,39086
+kolibri/data/file_stream.py,sha256=W8x64Tp8xVX2t0h7DDCW67pQ7gK9BTEclpY9DSGk2b0,10372
+kolibri/data/iterator.py,sha256=-ymNquPlYE35emY66yGvEUccb91S0bP4emj4CscRfLY,534
+kolibri/data/resources.py,sha256=_YBXQXvpEeCHbKAG24FkJsjE4hFX-lVeodFq9tiAGSc,743
+kolibri/data/schemes.py,sha256=KzxsSXR0mtvtCKOfXwNMggWGacy6l0850OCbb1wwgZ8,10130
 kolibri/data/settings.py,sha256=uIsB2x_nUF7HgV4X59OeS8ZWMerQUx_zgbz_P3IzZDY,42659
+kolibri/data/streams.py,sha256=k1xJjvS8k898DvQ2ysGR9nijKiuHTzx-pj8U6Bx4dGM,5610
+kolibri/data/text.py,sha256=XHJKENpOng8Z-qI_AqJe_IXvJtTTHOk-MYJp15mPtJU,7910
 kolibri/data/utils.py,sha256=qsfoDgX_OnRiUlLOxFfCu1aw1KlllTuYDnAZ0ZjuvFc,43976
+kolibri/data/format/__init__.py,sha256=uDK8Bs_c3O4o9znYhK7_huuU5PVF-UnoWmHUOLG8z1w,94
+kolibri/data/format/conll.py,sha256=6WoRsOLmh5lJxNqnDu72U1HzBoYjOO3HVz8dHew4Hyo,539
+kolibri/data/format/csv.py,sha256=Eh1PAmR0KymT2O91b5tSdz6kazgkYUzDWLQ8L-j2FpY,385
+kolibri/data/loaders/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+kolibri/data/loaders/arxiv.py,sha256=eRtDWuZoi6_zWAqI6kgD6vrgZpIoZssN_tDS22ayJmk,960
+kolibri/data/loaders/base.py,sha256=trP2pKAKJNwgy9R4CZkMqpVzqRVnZj1y4bczAg6IjP0,2516
+kolibri/data/loaders/csv_loader.py,sha256=ZLzya45-yPUU1fBEoX4CEDZG_7SjX-IIcEDpGpoVjYI,2238
+kolibri/data/loaders/pdf.py,sha256=Ujjo2_IR0pw02oJkT-PVcMkHQxNMDbGy285_Ejsgg38,4577
+kolibri/data/loaders/text.py,sha256=O1jDBrBoSnzH7qzNUJJNVrgr5BVSxv7UeXczhhOUObg,1973
+kolibri/data/loaders/web_base.py,sha256=dV_Yvs3XHaqbpslv1rYA0e4jBdTxPcqAlGvlCRtf5KE,7710
+kolibri/data/parsers/__init__.py,sha256=baNNfl4z18YV8-iKDbqItlmX1cfxecwVij9mhd06Xco,242
+kolibri/data/parsers/audio.py,sha256=NhtUnaS1h_LNJfZC1gOEhwUm_SNhskvEFFR8VtYxwf0,1929
+kolibri/data/parsers/base.py,sha256=Hd9-bhhLVVG3yXq7BLPvUBj9dF-fe0ko1oLhhIggqt0,1090
+kolibri/data/parsers/generic.py,sha256=EWz3IO4lcpxQaOmSLJ1QRGmd9AU8BuIua-RU2GPNeW0,2429
+kolibri/data/parsers/pdf.py,sha256=_b79sA1UINfFS9_l2kzHViy0yj37jbpZ-1OOTNHGDoY,813
+kolibri/data/parsers/registry.py,sha256=p_RUnZHliQ2tjA1Wz3fzXPqd5VSGWgnv2qU0wCkLFvQ,906
+kolibri/data/parsers/txt.py,sha256=2ivussOQTAAfnwViDxCVGr2-yzU5EeXf0tDJpyYVDYw,453
+kolibri/data/parsers/html/__init__.py,sha256=7CXsB8u2YPoy4INDcZjViRi63MYiJh9MP1Wgt1xlB3c,85
+kolibri/data/parsers/html/bs4.py,sha256=khCq3Uomz2uNe0-bMgxWSnhtBDxA9QW7g9Te4WQdZDU,1567
+kolibri/data/parsers/html/hyperlinks.py,sha256=iT-XAVxHAjCanBNiC7IlSVe4wDRbooSr71AGyOUD8a8,929
 kolibri/data/text/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/data/text/base_stream.py,sha256=PPW9u8j5MZRi1ImThILOk_j323aDZPuULRbNYki3-Aw,2246
-kolibri/data/text/corpus.py,sha256=BDMSDQ7QiwmWzZCRDilgq0Rlqi9rUoAo_squJXAUuoA,8152
+kolibri/data/text/corpus.py,sha256=o6q41efYzDO8q2q6u9iTOQLiKlQM-vul3LdJ9mXFXrY,1236
 kolibri/data/text/dataset.py,sha256=36A30UagP1CC_pVXBIbzYg_SAAbBRbZ0Koq3SZ0t2FI,29550
 kolibri/data/text/file_stream.py,sha256=3yFhFSxvWI0c5k1uWcNnAWMq4J69uUhX4OwkZ0yOwBs,10385
-kolibri/data/text/generators.py,sha256=jn3pEI7oqIb-E8l9J6UuHBYfrAORYSaAZcFzTaosZfM,6806
+kolibri/data/text/generators.py,sha256=8-JYIGrESuvW2f5I2HH0rHBJTwc3si7iyACTgaCbiuQ,5145
 kolibri/data/text/iterator.py,sha256=-ymNquPlYE35emY66yGvEUccb91S0bP4emj4CscRfLY,534
 kolibri/data/text/schemes.py,sha256=KzxsSXR0mtvtCKOfXwNMggWGacy6l0850OCbb1wwgZ8,10130
 kolibri/data/text/streams.py,sha256=_b7zrums7g0TbUEyCmvmPzm3yUmdd6AoJV0jznwG0Zg,5615
 kolibri/data/text/text.py,sha256=cVjgVEEryAJ5WeZGSHpmNxPMVozvp-PP9fiUpHl5vD8,7915
 kolibri/data/text/format/__init__.py,sha256=IqnXlvGOxl1dY6AJ2MBElCZtC4GVUpi9MLlvHqGBoS4,104
 kolibri/data/text/format/conll.py,sha256=6WoRsOLmh5lJxNqnDu72U1HzBoYjOO3HVz8dHew4Hyo,539
 kolibri/data/text/format/csv.py,sha256=Eh1PAmR0KymT2O91b5tSdz6kazgkYUzDWLQ8L-j2FpY,385
 kolibri/data/text/quality/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolibri/data/text/quality/cosineSimilarity.py,sha256=fzlk4W54X_UcEemBXQkJ0IogCOPyIxbYDuqr3D5RK14,4891
+kolibri/data/text/quality/cosineSimilarity.py,sha256=Tr9R691SyZwSxAaNLbkMQ5BcxAgs4xtZkp2NMWp27yw,4796
 kolibri/data/text/quality/mismatch.py,sha256=SjpkfcMslACEYszf2eKYspG11uWR8qKd4K710Us4aLA,983
 kolibri/data/text/quality/pairwise_cos_sim.py,sha256=tf9w4psOF2gtIo3COpztGApbIJf3-l1XnGRv1XBd_p8,166
 kolibri/data/text/quality/similar.py,sha256=mB9gmlQQvO5Wz3tMfagxMxVmqE_fCCwdDO7iLrh8DWw,837
 kolibri/datasets/__init__.py,sha256=awAxR-MpCbwZIXUR0d7F3kcLvklSiNdnroKQWDfcGww,47
-kolibri/datasets/read_data.py,sha256=QhBfAb7EXJ6nXfMA8k13svKIDYn0axlroZ4Iddck2Eo,1736
+kolibri/datasets/read_data.py,sha256=GYHC_13TFe1vXyjSv3UA96Jq9ybmMX7jw8ZCU_iF1RA,1800
 kolibri/datasets/reader/__init__.py,sha256=o7bfU3MkVAkCcsCYXOojuTuJi6LvJBqnmwLzTzHqwpI,61
 kolibri/datasets/reader/base_reader.py,sha256=Df1WRgXhzuEqVhzP7_i_8oYW4x5Ywyy6YUTSN-methU,3092
 kolibri/datasets/reader/classification.py,sha256=75VNks-Cr3nw8EM_OLHsFVsO1O5pJ8TC50su0u31law,4055
 kolibri/datasets/reader/conll.py,sha256=ee7aeaXODO_ufwsrtJUsZsUK4nQuuBjE6BUf2Mvm7Fw,2213
 kolibri/datasets/reader/dialogs_reader.py,sha256=llouerY5qR_11vki_HwCX5nxy96hZxhbin8xLoZ19eY,30779
 kolibri/datasets/reader/dstc2.py,sha256=qdo7u17o8QXpr9t_g9gOEEWnxajDFABqNHmJnAhSaIE,8005
 kolibri/datasets/reader/snips.py,sha256=DK5nMedUODd_QxMc-A6wqrBzL4sqvlBBUf3GHJu0L4E,4919
+kolibri/distances/__init__.py,sha256=vj1jylpEJy9SasTDWAsDrpsvpUszqcJy1kWHlEHO5YA,3531
+kolibri/distances/base_categorical.py,sha256=ZSczZIPKuD8BuzZy1xpsKu2Lp6nyqDCo8Vjq3yX6Mww,4899
+kolibri/distances/eskin.py,sha256=oY_zkG1o9vAvVzwoJ_bjc24bxUXNdiwnIKSHfH8KsDE,2551
+kolibri/distances/goodall.py,sha256=uPldsbVmCSjOl9VFwaP9DZBiNDA6PBarzV0cj5AAEzc,3907
+kolibri/distances/heom.py,sha256=nqdxIslLz1f9YMGaFkE_CH5HomIrxI-KyRcve0cP9kE,6368
+kolibri/distances/hvdm.py,sha256=_NDhpymuotj_Bp3k28lIZhFDoi1UgR6LzvSUsXhBcVA,5015
+kolibri/distances/lin.py,sha256=EH16eOET6Og5I_zXcZq1de8-avfDxcDnSm-ifaQo5zU,1226
 kolibri/evaluation/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/evaluation/classifier_evaluator.py,sha256=JL2ZtWepQMiEK8Nx3LYl3BhZUPkl-N3ikaYuzQTLbL8,7885
 kolibri/evaluation/clustering_evaluator.py,sha256=16otU4Hibi3wJe8cQvV43fXMeY6MFFZ7sJWC1Enz4pU,2489
 kolibri/evaluation/model_plot.py,sha256=L2EN1MNuqJIwJzL4HP4HoHz2BejaEVJu3LzXwXKdGcI,41666
-kolibri/evaluation/metrics/__init__.py,sha256=hBUwGFTqPhJ8-87Qgf0Jr_8xqyA4vtxLb-virS1Y3VQ,694
+kolibri/evaluation/metrics/__init__.py,sha256=gUQJyU1hj-utN4UunH8Zz9wlEdlFYsw73dKsMr9o0xw,809
 kolibri/evaluation/metrics/anomaly.py,sha256=-fBHIodYVXKjl1xhNv_QV1epU3KcRfFQzllBEyx0I6o,5578
 kolibri/evaluation/metrics/base_metric.py,sha256=ryxG5v3SVW9918zMl7VR0A8Q335KYPNTHAQUOr983aY,1792
 kolibri/evaluation/metrics/classification.py,sha256=Xl-WMMJYJvjo7ClPcWFH5ROXnaNP4GvRrmKI1297yAU,9438
 kolibri/evaluation/metrics/clustering.py,sha256=Qx735h4wkA50TIT4DGqRa8uLjknHnZA-ya9HaOhJ-MI,7198
 kolibri/evaluation/metrics/metric_utils.py,sha256=D0RRmoSe22WXvw1m4UEU5NXGCi0l2lTewe6WcyZ0hM0,8757
-kolibri/evaluation/metrics/regression.py,sha256=zYYY2qGwfwERSoE5oa44FXGbh19ho93qHUXzXpO_yfU,9345
+kolibri/evaluation/metrics/regression.py,sha256=mF-dGCw1VcO7gV1RWWKqbmOkRIzjgyNGjKFbjszwKH4,9491
 kolibri/evaluation/metrics/time_series.py,sha256=vrvkl1I4Xw5R1RNaYJQJVcuC4Cx5YrIFdqVrCnupPYE,10235
+kolibri/evaluators/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+kolibri/evaluators/classifier_evaluator.py,sha256=GiteMeSwumoeMByG9XSUC9YnRZzfAZ5rPHhuQMyozRI,8796
+kolibri/evaluators/clustering_evaluator.py,sha256=16otU4Hibi3wJe8cQvV43fXMeY6MFFZ7sJWC1Enz4pU,2489
+kolibri/evaluators/model_plot.py,sha256=gdLEoRCNopIzL0ttpaDXjC7UW4Gw9rKixSgd4jK3j40,41682
+kolibri/evaluators/synthetic_data.py,sha256=oXjUFZL-ymejZvsiflI8_MPERQvQ64513NwWJAn2MoM,3215
 kolibri/experiment_tracking/__init__.py,sha256=d46MxvQvEJ9wivSpovwn8NWXqsNAAvLiwxd1VKwlWIE,224
-kolibri/experiment_tracking/experiment_logger.py,sha256=GBbQ_Mu0rH2b7N860H7voUpBFyMBCrwsnMNXB7X63w8,8528
-kolibri/experiment_tracking/mlflow_logger.py,sha256=faz2iYHpHC1oYpadjluuefts02-F4kak5aEluZqHhCw,5623
+kolibri/experiment_tracking/experiment_logger.py,sha256=_1pq2zNAa9logTwaqWAkaB9MTFw-u6DjhPJqKMUmc0M,6170
+kolibri/experiment_tracking/mlflow_logger.py,sha256=jdp7XkWMblm_lnRgWmwip01Euape7UMCQGeldQM3Gz0,4971
 kolibri/explainers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/explainers/shap_explainer.py,sha256=F_ULVxCYLbcB7vTnpEwcHp_Wv-FOhBHHzwNBR--I10M,12089
 kolibri/features/__init__.py,sha256=cRgYNxwXZ_lbHWAH7a0fhbb0WY6IOFInECJhpMXrlT0,227
 kolibri/features/base_feature.py,sha256=b0LKWapmxIM44vvKYSfTr4nkUPldq25FQU2Or1nbn5o,2781
 kolibri/features/basefeaturizer.py,sha256=WEG-HGyF2RTXMtlGUWEeZk7u2Pv8bEqV7NTix3hYAM4,1431
 kolibri/features/tabular/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/features/tabular/time_serie_featurizer.py,sha256=k_C_En9EXsALMXwU7QtPaD-oYJ6y7jrxF0LH-3--Ndo,1763
 kolibri/features/text/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/features/text/feature_functions.py,sha256=8yHQPqUpIvTD9BMk022fzT2gt3a7GDo4UOPQUDO8umY,8352
-kolibri/features/text/hashing_tfidf_vectorizer.py,sha256=C2EpTG19J7E2lkEz9iCzwswBddBe5fue0_oBzYifJ58,10019
-kolibri/features/text/text_features.py,sha256=CEpdvtw4OqEZIGVCbrf79pBA3KhKKc2HEDcAMxPPeZk,5730
-kolibri/features/text/tf_idf_featurizer.py,sha256=tjYkmgC61QaMmZvCMatc1v7bqkA-o5cC5laKlLWwlQo,6275
-kolibri/features/text/tf_idf_topics_vectorizer.py,sha256=iGRopL6w8eKVDerGBC-FDqzTPrtG-stBttoZWkwPfms,5782
-kolibri/features/text/tfidf_weighted_embedder.py,sha256=X-VI0Na3gyb8D4GWg4dZvOXHgI4SSqhIROdQKU-dTLk,8331
-kolibri/features/text/embedders/__init__.py,sha256=4XKXi62qhFSgn2TJL8hEt3uLUiwV9UqhTWFAc7PsBkg,342
-kolibri/features/text/embedders/abstract_embedder.py,sha256=XR-6CWTBGXBPDB_Fv8CI1QbyVvXC63nvnrtLDKvDbcY,3700
-kolibri/features/text/embedders/bow_embedder.py,sha256=ymwISEN7_0fJU_u4iUrHlnYhn4RIm_636gGoJaVkgOE,1234
-kolibri/features/text/embedders/elmo_embedder.py,sha256=orqJCpwtte9rGFgvSkpc2TZ4V7UgAJHa8aK51pFN9YI,13793
-kolibri/features/text/embedders/fasttext_embedder.py,sha256=o4PHW1KJP9u_On7ogqZC0rlvVycH0jC9YxhUkV7UjNE,1581
-kolibri/features/text/embedders/glove_embedder.py,sha256=_8F2UY1xuETmZMXNvhQWcJxBqqhGdpgaxVAE0V8tNZU,2040
-kolibri/features/text/embedders/transformers_embedder.py,sha256=cVtxlIa-XgJGNUQjL4GPppbQquExaqajJRiy3hOt6CE,4920
+kolibri/features/text/hashing_tfidf_vectorizer.py,sha256=w9qipim7EjjyQp0eCLojmt2KzWK0Ili4HLBrLoOWuOM,10000
+kolibri/features/text/text_features.py,sha256=xbSwlero_jBAXotzq76QdD0GMHcbNaEWkSnV8L6ePv0,5801
+kolibri/features/text/tf_idf_featurizer.py,sha256=KJ-83jIkbQASZT_DIm64sph-nxTfdGMCUEsZRI6uqEA,6336
+kolibri/features/text/tf_idf_topics_vectorizer.py,sha256=qtam33XebaraRSbTT1n-zAVvSIVr0-5GjUoPCxXl9v0,5853
+kolibri/features/text/tfidf_weighted_embedder.py,sha256=rG5GRZset6-Aut823fQp2bwBOr8jYVxydIG4BQWInc0,8121
+kolibri/features/text/embedders/__init__.py,sha256=wo9ZBw8yOosILo8DstG3CwiRAUWFMYj7zNav-KTM6jY,346
+kolibri/features/text/embedders/base.py,sha256=_QMlSNhdpScR60MRA1xcxj6bKhSi6f38-VZGGMeyDPU,3709
+kolibri/features/text/embedders/bow_embedder.py,sha256=tfFMxTVN_CLxZnFeUs82ftnp-mR7hgnnbWX5H102wiM,1347
+kolibri/features/text/embedders/elmo_embedder.py,sha256=nXFKG-Bv4uYNC9ke6uY31qvf3u4qnd4SAszKUC57NCc,9928
+kolibri/features/text/embedders/fasttext_embedder.py,sha256=S5dSvUWjfR-xiW4MUR6TJ9Gzevn2dKKmxrKd1svpJyE,1568
+kolibri/features/text/embedders/glove_embedder.py,sha256=bvJCLA2HAC05x1aJpGcxMC3wXcGTgK-GoZR8RzSgyE4,2027
+kolibri/features/text/embedders/llamacpp.py,sha256=tvYZ3kCJiIl9X8PVi6akfBYw_9f785sPUa-d8gMoGSA,4096
+kolibri/features/text/embedders/openai.py,sha256=1wl9fVxSIVOTcK0-Et46kLiOU2BdJIfHd9Djky7oPgs,17705
+kolibri/features/text/embedders/tensorflow_hub.py,sha256=QZIZ7IUH2n33EOV7H6bHXx0QHwJ2kc-Zgbr6skacl1s,2466
 kolibri/features/timeseries/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/features/timeseries/features_utils.py,sha256=ErwwBJds2M8ELkH5qmkU_EF-gftjDELJTC-EfGNrHlQ,31971
 kolibri/features/timeseries/ts_featurizer.py,sha256=AXx4RYzRve1rBnKRYKV9S5-wFjXvc4fSTyi5db6kBgs,10656
-kolibri/features/timeseries/utils.py,sha256=aNzzBdwbXUBIfHl7x6di_XpXauP0CwIAPzXjMVRiXfo,7658
+kolibri/features/timeseries/utils.py,sha256=bBVaXfSmvxk7CHtQYOOoYzd1vNQzS4ZrxVfvkw-DtQU,7659
 kolibri/features/timeseries/feature_extraction/__init__.py,sha256=YK6iWKahGZ3sk6wCYkKtZB9Hsp6t0NlX4aTGBDvqSlE,358
 kolibri/features/timeseries/feature_extraction/data.py,sha256=iCxVcnnmHlYfiKeDqfRM-wsTmK4rV4L0HW5gVC8uEpc,16661
 kolibri/features/timeseries/feature_extraction/extraction.py,sha256=OG4h6ZRbNTb8LPq8gEX15gGpbt4Wr2bEZSFCE_AQINo,13772
 kolibri/features/timeseries/feature_extraction/feature_calculators.py,sha256=N6mKmL0E27YSEhbTpCrUtcabx4cZaGqdPL_jKzXwbd4,81555
 kolibri/features/timeseries/feature_extraction/settings.py,sha256=kCF9IW8xl1rlKRHwilEK5z9NAG1N-x6JBWLu-fhkZDQ,14105
 kolibri/features/timeseries/feature_selection/__init__.py,sha256=dQcqBIzkIO3rg-kHZnUjfYKLJEjWXCC055tnZhvOplM,606
 kolibri/features/timeseries/feature_selection/relevance.py,sha256=cVtu-dtgaKvFCFERtppVkWEpCFGktI92PAzjaJnEbsU,15671
@@ -213,200 +364,219 @@
 kolibri/formers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/formers/tabular/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/formers/tabular/clustering.py,sha256=oFDHoHtgfRybp07DQak3qMhdvzl_gQKmKpte2KnZqcg,1043
 kolibri/formers/text/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/formers/text/classifier.py,sha256=hC-1Mg4brwzxwbi4-WST5U35QXKsgMsRRarK-d1nNzk,4315
 kolibri/formers/text/sentiment.py,sha256=bDtublKNNJTK0ZLHPQy-VfSELx3swUnFFegDwV4Gllk,230
 kolibri/formers/text/similarity.py,sha256=XYWHPev_HliftwoieOhu8P1ylGlMVHXekyRi6nTh9IU,4515
-kolibri/formers/text/topic_former.py,sha256=nthS1jowPDaSP9aCDW3HSt1Q8sO0bpMcT94Dp7N4pQg,40764
-kolibri/indexers/__init__.py,sha256=oPiRB4GlUMtVKiDvaQb5CfWs99tP_804LnViV7kHrCo,438
-kolibri/indexers/base_indexer.py,sha256=cpBaPMwr701gkLuMzB1uXPQ7pmVuiXU8PvNpZP2Rccc,6836
-kolibri/indexers/label_indexer.py,sha256=0cS9zQm0v7Ww8Vpv04KFU0bPBU5F34qjhCUoKUbTncs,3339
+kolibri/formers/text/topic_former.py,sha256=vMKyUWLKM-PZC5U_w62YoGPpz32Rx1-XX5KNMlTRkwc,40754
+kolibri/indexers/__init__.py,sha256=wcuPgVWstBsNdihWHuWF5oF5tTlVn_tcK2lhdKQ0pAA,219
+kolibri/indexers/base_indexer.py,sha256=emBSHilL-FZ2bEdXjT45UiqQ4keskP7qSQx_z2ZFOrw,2680
+kolibri/indexers/kolibri_label_encoder.py,sha256=r6m52A_WH_r6pQ_H91CNjH9IfTU__9uFc2ID3fucOOY,1239
+kolibri/indexers/label_indexer.py,sha256=UkK3KQNOZN-0oVUFW_vnx57aYVytU4Xpd9drHx3sGaY,3570
 kolibri/indexers/multi_content_indexer.py,sha256=v6NoarZ01DqWcVz5NvP2Te67cRU6VJGuEW2ElxyUEPk,1248
 kolibri/indexers/multi_target_indexer.py,sha256=w8a87da5TklAoT9UpKYae9IEKHTXXgHBf84hUCpanp4,2394
-kolibri/indexers/sequence_char_indexer.py,sha256=B0lbX4kugqvTheJpYobJrfs1hp1kjMRJitQsYAxrJSM,4944
-kolibri/indexers/sequence_indexer.py,sha256=XFgKbq97LYkXy6wiwBU4JyN36s7L8ietsSqatmf-_wM,4883
+kolibri/indexers/sequence_char_indexer.py,sha256=Dybu74o1NSKuumnJ12HhxJCUueoYQ6SjXYZVW36gAXA,4944
+kolibri/indexers/sequence_indexer.py,sha256=BuZ2ZnB5rGGRVVyIwwxte8ECUxPEAEjrfp_1BnQO0tg,6012
 kolibri/indexers/text_indexer.py,sha256=Oa9FLoh9tX_f2bmztV57CCzN9ick-xbVzCgzXb-C9-s,5940
 kolibri/knowledge/__init__.py,sha256=xN5_d2ADMEkBYwdXEs6g_YXbRQZj5g6puJkqdIJoiWY,43
 kolibri/knowledge/domain.py,sha256=4QZoMJ1_8x1heIqs_lhNLbZHqRGob7HCteEJCRHiwwA,1173
+kolibri/mlflow/__init__.py,sha256=JnwNiHnvbdlCzy_a3jc2K2jMplIiVy-XORbP-UMZsYQ,11163
 kolibri/optimizers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+kolibri/optimizers/metric.py,sha256=MUdonc4U_QD30ibtgaRk2bvCmC9P2H2A93zSLiGyeSU,9226
 kolibri/optimizers/optuna/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolibri/optimizers/optuna/objective.py,sha256=6Lz9qMRAFJ-PBLfvgEhq5LFh8cReuf-FMA6RH5lU78o,10410
-kolibri/optimizers/optuna/tuner.py,sha256=QS5F91dXTF6mp5tS6yYj5xAWssXmdy58Np_AoOxFUqc,2933
+kolibri/optimizers/optuna/objective.py,sha256=Lfy-gM_wS7a6v2gvTghdcJevtCT-Xc38LIoe3qD6TMA,10868
+kolibri/optimizers/optuna/tuner.py,sha256=96yTW8G-RjIrWZgnDajU2cxgq0XUbycCZGq6EKuZGaE,2889
 kolibri/output/__init__.py,sha256=x_t2N3HMKp2b6W5uNUN-_hoI2Sm7Hb__4JNhp-1reVY,49
 kolibri/output/display.py,sha256=Tj5b1EkB4ksNL64miE2_rlQpuzGF0ZTz0VTiEwABqiU,3303
 kolibri/output/display_backend.py,sha256=DxtzEdwJCiTstacbno2kE_MIVw21iPXFovM44fQ3ylU,5694
 kolibri/output/display_component.py,sha256=WitpBw7KotKa3gAn3zlc_5B1-Ak671RckeCAY3poi0M,1637
 kolibri/output/progress_bar.py,sha256=sRG4KjXSySjPXXved6m5pzkxaIsp-KTUuoooHH_wjSE,4514
 kolibri/preprocess/__init__.py,sha256=4qOGbQoCuV3KQjC_R5CrQADL_fLGxXbBqZTH63SYKuc,40
-kolibri/preprocess/preprocessors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolibri/preprocess/preprocessors/bert_preprocessor.py,sha256=1_HM6lyYZGPHGitEyOG9Pg8Kwz_QgY17PjUYbSdoXuI,14975
-kolibri/preprocess/preprocessors/capitalization.py,sha256=dN9THRZFVdZy9McGAk4PBdDD61vcwFB-lT3_qJaJQjI,4942
-kolibri/preprocess/preprocessors/char_splitter.py,sha256=zrmNERhg0-kUzSNLN-PtlFEe5ewOrxaZAXB31hsx7jY,596
-kolibri/preprocess/preprocessors/dirty_comments_preprocessor.py,sha256=SyVhcYtfbKdFZRcQZiOj9skrqiFko8x9xR_F3hSWoKs,3356
-kolibri/preprocess/preprocessors/mask.py,sha256=5Wi-MvSbNounQQhqCaBpbi1uFCHwmeMtra93iBbm8XU,1183
-kolibri/preprocess/preprocessors/ner_preprocessor.py,sha256=qaSgi-zzWCV0nFLMdQl0OfHiPqTh__6amnTyfEFeMO8,7324
-kolibri/preprocess/preprocessors/odqa_preprocessors.py,sha256=3AgIq_Jnv-oUMTQbvSAz16sCPsg-8SjjvFcU_DJMq00,6619
-kolibri/preprocess/preprocessors/random_embeddings_matrix.py,sha256=DgfNJ5lqObj7r9KCBz_zkQkh637tyc9QbS6LZgV7f6c,1236
-kolibri/preprocess/preprocessors/re_preprocessor.py,sha256=ospT9c4vOGsPmEiHCUSzT5vI2QmyFAp3UgjUScNM0OM,10390
-kolibri/preprocess/preprocessors/response_base_loader.py,sha256=_jDE7emXQVFdy-nG9G9ocPEEq7g6DD8pncJ_jLJ7y_Y,2501
-kolibri/preprocess/preprocessors/sanitizer.py,sha256=ApequiZwwPYdGWRSj-WYm2hLzAEez_62xcSkBug7A20,2330
-kolibri/preprocess/preprocessors/sentseg_preprocessor.py,sha256=H5MuUzKcS-qUCu58Z9QEzlDvBZell5aMy2jyDW2y3vE,574
-kolibri/preprocess/preprocessors/siamese_preprocessor.py,sha256=JFrnR_9t4LitMVhMyfsjUEN2dwT4009vtSOCiRzmtFQ,5931
-kolibri/preprocess/preprocessors/squad_preprocessor.py,sha256=gttfUC-Apcj3gpMqpP-2hmM863caJormsP1XWVW46mE,20411
-kolibri/preprocess/preprocessors/str_token_reverser.py,sha256=Y93TK47G1cpZfEJvuhNE4Zz-D9yLyYFZb2vclzAQQMg,1883
-kolibri/preprocess/preprocessors/str_utf8_encoder.py,sha256=tLPWdn3swO_hgr-DkWLydxS5HZqk-ImezFA_3Cam5lU,7566
-kolibri/preprocess/preprocessors/transformers_preprocessor.py,sha256=SsYEBG6tF8wvSCUkWuGZQq633ymxjqYt6DfQJmBNNbM,2657
-kolibri/preprocess/tabular/__init__.py,sha256=BtJOPDa2n4UcKGrzo2PLNmAFFKkuRr83ZyEx-IIKg8s,1624
+kolibri/preprocess/tabular/DataFrameVectorizer.py,sha256=eWqvb_8I08KxkmguorSsHwch2r-7iMlsMgsUJGaKtic,13211
+kolibri/preprocess/tabular/__init__.py,sha256=KaLJx5eEa3njvm_luQiaLOHrWdaUInWxKGSeYw10-4k,1780
 kolibri/preprocess/tabular/binning.py,sha256=CS7AEBXSFzSP1uQquLsntaFyIkpnFFus2J8WRJP0BKg,3030
 kolibri/preprocess/tabular/boruta_py.py,sha256=9p0KaYupLBKHTp1Snf5iELe5q6YdWoC2Ik3FKHXt5Jg,8728
+kolibri/preprocess/tabular/category_transformer.py,sha256=0LbMOqUnz_NIfiLkmfp2mIm1ydoWBAzo2oPstz7rU1Y,1907
 kolibri/preprocess/tabular/cluster.py,sha256=Rlv4NeDxGMosq-QVZfD1k0Jd_upongJkI9I51qpYzqc,5219
-kolibri/preprocess/tabular/columns_transfromer.py,sha256=800xvcSlh4PUE8WDdtyML1wsDtAt89wU_ilPnyNy0RU,1584
+kolibri/preprocess/tabular/columns_remover.py,sha256=Ku2jJxEbS-U7GVyRdw-4991MfLiGxkArMJgQxJVe898,1062
+kolibri/preprocess/tabular/columns_transfromer.py,sha256=DD9Z7c2-kZxXAsxyoVIC-n5hmLO3vYrKJ3H5PJw1KVY,1521
 kolibri/preprocess/tabular/data_imputer.py,sha256=LSlbZK3JV4hlbZde_UD1yekmRUHJzB-6yKzbqhXwneY,11658
-kolibri/preprocess/tabular/dummy_converter.py,sha256=x1mofFqRzA2be7slsl2rTInXH1U4j6-TxEg-cpXxRaY,2968
-kolibri/preprocess/tabular/feature_interaction.py,sha256=jblp2YMcvQ7bgydNs6Gg-zgs-sDejqAsHORy9zlnUJg,13109
-kolibri/preprocess/tabular/feature_selection.py,sha256=zfK4Zi7Ml1XXiJmtWpYETZt4GGHL2W5PdP-9KjPs-0k,10195
-kolibri/preprocess/tabular/infer_datatype.py,sha256=3XKktpk4OR0yO2IneczH8RdFU86NIgGRy_vpy2powb4,3783
-kolibri/preprocess/tabular/multicollinearity.py,sha256=Ty-usNqOK32_Aqm2q_cQCyPdS-9gmGlnzEDjTPlakzQ,13298
-kolibri/preprocess/tabular/normalize.py,sha256=oCPQ2H5QieKrZ2sdtzpwnNANoEcNtid1jW-zJ8LgP_U,4279
-kolibri/preprocess/tabular/one_hot_encoder_multi.py,sha256=WXt2nDSbEJTijPyYP5h7Apn6AMNx8fPsb-Fv_01r6oc,2490
+kolibri/preprocess/tabular/dummy_converter.py,sha256=dD1vWudMr0quL_PafNQP3MVLiaHTAvX5hVoWtguW8_M,2970
+kolibri/preprocess/tabular/feature_interaction.py,sha256=fjb7S6G2ZtWw1HyG5vRhcIDITCLqzJt273dKuQcZsqc,13500
+kolibri/preprocess/tabular/feature_selection.py,sha256=n47sT_pSRwbOyPyYTJpz8D8o2qiXBvDBRtmF70UJR5o,10314
+kolibri/preprocess/tabular/infer_datatype.py,sha256=amr8t18H7zmdaeo7xo0X5VKOXGVUwVX8m1oraZBzeVQ,4365
+kolibri/preprocess/tabular/multicollinearity.py,sha256=i4cOJuCaUQu2-gUN9NvnORf-TdMo6DZk4PdkoE3ifQc,13584
+kolibri/preprocess/tabular/normalize.py,sha256=4xiEz8MQyWOglX26kjsNFEoR3oz_eDbcsrHDGQ13qEk,4341
+kolibri/preprocess/tabular/one_hot_encoder_multi.py,sha256=JvxBuBb5EggRPS6Wm5nV1FPszK14iMpqjCeuMK4kU0o,2494
 kolibri/preprocess/tabular/ordinal_transformer.py,sha256=PLw2ywCwh65pRNGEnJaKnPIfu9cIVTd5k8QMhr1E86o,1620
 kolibri/preprocess/tabular/outlier_remover.py,sha256=SGRUgiwbG9uHAEADzx57rwHBxhRsjqG0eAhototu-bY,2616
 kolibri/preprocess/tabular/preprocess.py,sha256=D1w5xhuQkQtUn9tJCc9udj3UyXetChJDW8TihOba808,149882
-kolibri/preprocess/tabular/preprocessing_pipeline.py,sha256=CuWRopra0wZx_e9G8pd0xe4WbIhq6VNfc0zDn7gDkpk,20154
+kolibri/preprocess/tabular/preprocessing_pipeline.py,sha256=VlzeilnyBgIQH_iLbsoCVZzQzmchaKTRvOZb4NznEUU,20056
 kolibri/preprocess/tabular/rare_levels.py,sha256=uwgSuUj3numf-vA7DBTM1LLGpzWWSsSUVU1Pew6rJq4,3454
 kolibri/preprocess/tabular/reduce_cardinality.py,sha256=uMKsS0iL9bZFY3FtFOjildUksJen7zyT3jIowA5EFXM,8598
 kolibri/preprocess/tabular/reduce_dimensionality.py,sha256=OIUxm9JY3goCb1lgrkwtDFno4_YMkocgGkDTgF5W4Mg,4848
 kolibri/preprocess/tabular/regression_target_transformer.py,sha256=EauWaMcIbA6D0daXaF12v8ErZFsuW8exvSzdnIBBniU,1801
 kolibri/preprocess/tabular/similar_features.py,sha256=jXynt5mbHiMk1zYEPt-M6wYGg3VTnw2FsOwLGUXP720,2003
 kolibri/preprocess/tabular/time_features_extractor.py,sha256=sunqoXHlECNM6zFVEdzCpOsgo8kOtmXv__stz5ct5lM,4003
 kolibri/preprocess/tabular/univar_outliers.py,sha256=_8x62kIWWyZTD1OukwmvTIpji7KGhu228Kb8upb2meA,1808
 kolibri/preprocess/tabular/zero_variance_remover.py,sha256=dgQ-iCT9jMRhfdA23O4fqd51rTXiu3aqLk29LG_-jag,3531
 kolibri/preprocess/text/__init__.py,sha256=za9pwXIQtW8e_h0T2Xxv3i18jk3d0tIW9XlrOqgVU5U,76
-kolibri/preprocess/text/collocation_analyzer.py,sha256=uRKh8rb0xBT3dYuNyHgwCjLn3mv4uagG-EZReee1tZg,4396
+kolibri/preprocess/text/capitalization.py,sha256=8pCYnV8nBs2-7fPY260L__E7m-FwZFipSEZgYviozeU,4058
+kolibri/preprocess/text/char_splitter.py,sha256=zrmNERhg0-kUzSNLN-PtlFEe5ewOrxaZAXB31hsx7jY,596
+kolibri/preprocess/text/collocation_analyzer.py,sha256=7bNlIvYbGS9YIlz9WA7sZRIw9JP0bN5qODCDdOV68Xc,4297
 kolibri/preprocess/text/context_builder.py,sha256=_NCBCO4hge6iY31BKN_zv_BK2ZLMBIeRKJF0mZDUVxA,1412
-kolibri/preprocess/text/email_cleaner.py,sha256=PmdYPiRgIPr73gKqdu9l94b708o1ukSXfP8cO-aDn_I,1871
+kolibri/preprocess/text/dirty_comments_preprocessor.py,sha256=9s5ZlnNjFQoDBUdgV7nr6PXbEz2FDce2akZB2NAcEJs,3356
+kolibri/preprocess/text/doc_chuncker.py,sha256=r5oRsvhd54RB0H8fpTCkscmFxZIOwI3svnFG-CKNWQ8,5305
+kolibri/preprocess/text/mask.py,sha256=5Wi-MvSbNounQQhqCaBpbi1uFCHwmeMtra93iBbm8XU,1183
+kolibri/preprocess/text/ner_preprocessor.py,sha256=mGegEVq3GxqQ4EcUSOE0LEJcg-ssqA7lDwlGlHExBiQ,7307
+kolibri/preprocess/text/random_embeddings_matrix.py,sha256=fwXQjmkVTt9lhJcuSo1OodQY8ir-5aY97uiYQHNOunU,1229
+kolibri/preprocess/text/re_preprocessor.py,sha256=HXCcM0kD9eNL-iHWxQ60tgpYZSNGlBn1zATRlC1zoEo,10274
+kolibri/preprocess/text/siamese_preprocessor.py,sha256=1IGGUNhkTAXPcSElL733qAauHlmYDHDpl8KucAUd6to,5800
+kolibri/preprocess/text/str_token_reverser.py,sha256=Y93TK47G1cpZfEJvuhNE4Zz-D9yLyYFZb2vclzAQQMg,1883
+kolibri/preprocess/text/str_utf8_encoder.py,sha256=tLPWdn3swO_hgr-DkWLydxS5HZqk-ImezFA_3Cam5lU,7566
+kolibri/preprocess/text/text_splitter.py,sha256=O8eKhykh3TgQi2TBB0K8sPel_SxFu4Gn0s_tF9CzPuQ,6299
+kolibri/preprocess/text/transformers_preprocessor.py,sha256=SsYEBG6tF8wvSCUkWuGZQq633ymxjqYt6DfQJmBNNbM,2657
 kolibri/preprocess/text/cleaning/__email_configs.py,sha256=y2exE6858pMbzJYxiQj9jKxfA8P000hjc23XQkOdV1I,5288
 kolibri/preprocess/text/cleaning/__init__.py,sha256=41XUW4heGY_GuytXG6wyxAq1Zc-YPekqmw7VrrCDFqg,67
 kolibri/preprocess/text/cleaning/cleaning_scripts.py,sha256=SQwRaB54fpBQ7JxLCFo0yYhKzCvD9DQcOHJabUpAYC0,4348
-kolibri/preprocess/text/cleaning/email2text.py,sha256=NlWPnUj5pq91Sd67wIXqmEYTtYove6mj8YG3Ts61k9c,23553
+kolibri/preprocess/text/cleaning/email2text.py,sha256=KUWq-s51g3vfLqsM-HQ3g-19qQpVRwsiXTFDYVPFKJo,23554
+kolibri/preprocess/text/cleaning/email_cleaner.py,sha256=PmdYPiRgIPr73gKqdu9l94b708o1ukSXfP8cO-aDn_I,1871
 kolibri/preprocess/text/cleaning/email_parser.py,sha256=QXH5VFsQgh9sPwQNL53QVnl5IY_RjMaG5XeK_RgpJ-w,1425
 kolibri/preprocess/text/cleaning/header_parser.py,sha256=zyWFbtKYyETQO3ZDgRtlvWRJqCGWA1qvT3DUqz2k4Kc,3279
 kolibri/preprocess/text/language_detection/__init__.py,sha256=erG9ZLwf8735lWLBYp3gnfTqS8HWVabsVVgeLDNvsy0,82
 kolibri/preprocess/text/language_detection/lang_detect.py,sha256=kr75usxaSyCDA7o67SQxqfJGHkB0Chx-be60t-dFsRI,1420
 kolibri/preprocess/text/translation/Translate_.py,sha256=jB7Nwka0SW1wvN0KryIZIJOHnQKBnZyxCSmSr2m_2mk,7047
 kolibri/preprocess/text/translation/__init__.py,sha256=WRb9MqHA1lNoWO7lFYuHB7bMZysgOek_pOxZW8o6-QU,1079
 kolibri/preprocess/text/translation/client.py,sha256=87OTe1NcH6kr4ja8dlP9OTGsqKgrdpw3pP0F6NNBURI,9890
 kolibri/preprocess/text/translation/constants.py,sha256=qQ5ANUGmVkTIaJsW8AyxcfDw9J8qYgbe4gGrvWZAlcQ,9746
 kolibri/preprocess/text/translation/models.py,sha256=zNBDehv23u0hOCOSB7bI2ua0k_H1KoST574TpzoeeV0,1601
 kolibri/preprocess/text/translation/translate.py,sha256=K6OH-k5z8WV0PN-IRFutIjmFwUvKTsewbJYS8ZmUuxc,6090
 kolibri/preprocess/text/translation/utils.py,sha256=Vt_iwckxPP4QprnScc3bo3nA_ldpH7I9YJtTdtnfyLc,2640
 kolibri/preprocess/timeseries/__init__.py,sha256=1e4qvaiog7L8InRf96O_lirDnfm_X0uuQujFvlFkaPY,65
-kolibri/preprocess/timeseries/multi_window_generator.py,sha256=buUAG81pXIqFRR2YzGVKQc6RvyNjwCwwOJA7FE1o70U,15014
-kolibri/preprocess/timeseries/multi_window_generator_.py,sha256=p9kiuVJdN9RXGFeXAthcMTxGyoHerePFXQbbSs4fnH0,10757
+kolibri/preprocess/timeseries/multi_window_generator.py,sha256=MxpuPbsUbwFHsaIFn9n7Es46rDU65xEpuO9zBKL88PA,16072
+kolibri/preprocess/timeseries/multi_window_generator_back.py,sha256=Ku9frlTSO-ZxCtYgK9DaZTGxvw67M8rSR19BlI_3c6M,15304
 kolibri/preprocess/timeseries/time_series_from_array.py,sha256=cMO1TrfkfSFbjFfyWvJfcQ4gOGCalRecYSn-RrjjyjE,7919
 kolibri/preprocess/timeseries/window.py,sha256=GHranCvImg3YPDyIc0Q0cyGzS97EslqVOBEx63pLEk8,8504
 kolibri/preprocess/timeseries/window_generator.py,sha256=Wzu7aI2U1rJxitvE8CWxQGdx7TgYV_RQERgwRwzQVI4,7843
-kolibri/samplers/__init__.py,sha256=lzKBX2_t8UIHR9Vfe4ldAyH4tpVDgA7-yFhKrJ9QxsQ,2014
+kolibri/samplers/__init__.py,sha256=okTiWs_9U0t4ULsYdXncHA69yySvGyffsu5EafV-gqc,2131
 kolibri/samplers/auto_smpler.py,sha256=BTKAOuhBPluY_7jE-GH-uSlPJFhaZR91K5BRXwz_Aso,5095
+kolibri/samplers/conditional.py,sha256=NuG4biV8skcvwQsE6yre_0qgJA4lCX0TOjp-AjRMqs8,5952
+kolibri/samplers/data_sampler.py,sha256=E1baN6v4xiLZnvLsyGOYe6YZEi95yCvYH9uXa7WNnpA,2651
+kolibri/samplers/smoteR.py,sha256=Th0uUXoFoSxNtMsWjLcEljeZ3iKXc7bbMm-0899NM1c,7780
+kolibri/scripts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+kolibri/scripts/check_requirements.py,sha256=vkXTcHAycdLwrcsmrNRFYN5P1W29jYjDVoqEcofGlXE,988
+kolibri/scripts/install_plugin_deps.py,sha256=R2a1ntBiAiDoWylg6WXndRanOoyVEbpOd9_MS02zxf8,1284
 kolibri/stopwords/__init__.py,sha256=Tf5aza_sJkBdVAZOrYZd8N6R_Mk_8uy2UhoMnpm5NRQ,52
 kolibri/stopwords/stp_wrd.py,sha256=xdNBdBu2C5HoarWEzFeydr9BpQEt_A5zFe-KCu4hkaU,2016
-kolibri/task/__init__.py,sha256=Vb5YnMO2Txl85Mlrf8rG4NfAT5Bv4SKPCieKqx9kIe8,32
+kolibri/synthetic_data/__init__.py,sha256=bQcGicM--cTHq9sjR7ShLRji-PVTpqGJvcDATi7A3Zc,495
+kolibri/synthetic_data/anonymization.py,sha256=vCpZFS-l9ZsWg8Si6ht3VCyHetFNR3QsWKZpzxd4liA,3060
+kolibri/synthetic_data/base.py,sha256=dLLF15GuDK9znxuFoZVhjo0hLQiCtwS3kn0N1unEAMY,45818
+kolibri/synthetic_data/base_contraint.py,sha256=hB7OuFde0rDDYdO4u4I5orIJWZQAQmrSpd3-EE7ZmYk,18063
+kolibri/synthetic_data/copulagan.py,sha256=f6OqW69dNcS3HN13Nsk1pO8nztq_7CBis67aW-B3cJ4,11071
+kolibri/synthetic_data/copulas.py,sha256=kjjZ-uh8NG_3nG8tDpeTnGjwoZgPUYZD7wnzg59u99Y,14946
+kolibri/synthetic_data/ctgan_synthesizer.py,sha256=jT1BP4XaxGTEqDEwjh6fwWbPvI0JU-HLETw9kJVwZyc,9468
+kolibri/synthetic_data/data_processor.py,sha256=6e46FcOZXDXEvfBwUo_U33Ehd3IFiqINv4YkE2Z8pqg,35479
+kolibri/synthetic_data/metadata.py,sha256=787Xqw_VK5CQChNbD2Ij91CLdGPxmcC8r3I61P8IzCs,21080
+kolibri/synthetic_data/single_table.py,sha256=CB7KFUB539JMVXvOjUTIOMAHYEgohGPLubECUYVp-5U,7180
+kolibri/synthetic_data/synthpop.py,sha256=dGyRjkH2n6eSRTEptaJA8I93Q79ygkT5esiRwUQfOr8,3227
+kolibri/synthetic_data/utils.py,sha256=1jNPZpMEkF4TcHXQqUiwnxWzy0sTg7liW_e-qo05DzU,10163
+kolibri/synthetic_data/benchmark/__init__.py,sha256=aiqLsRMgabuatrfpJnq1jqd009p9gj7lZJRKVMkqUpg,1186
+kolibri/synthetic_data/benchmark/benchmark.py,sha256=b6ex4d8tLA-JgZZbQbIu5CFr0d6t7Yvf3uKEY47fIKk,15188
+kolibri/synthetic_data/benchmark/data.py,sha256=kVnSpw8ENhe_gtjcMToCdpuPz6vLaJKG83z4H0Gp45I,6232
+kolibri/synthetic_data/benchmark/metrics.py,sha256=kBEcSyhckAC-008cs2mNpiZnqp1WJTQp5KOLTy5uyOM,3309
+kolibri/synthetic_data/benchmark/ml.py,sha256=mHIFudjNgXCLYvhhV8XkUYfLTybRa9Y4hzJ3_dsJxBw,2241
+kolibri/synthetic_data/benchmark/privacy.py,sha256=0PKRJah9S7QhIPMriiOtcvHxF683csjck4Lhmb2Vf7o,2051
+kolibri/synthetic_data/benchmark/reporting.py,sha256=oeZg9jHxl37L61ZZ5iPNuFgfwMFWr_RHrGFCwOx2dN4,4985
+kolibri/synthetic_data/benchmark/utility.py,sha256=Ql52PiyxTycjh06jq1tdD_rKcdpis-nWD_7cDUCMd8E,2239
+kolibri/synthetic_data/benchmark/utils.py,sha256=Wi2FVTOVUvaUCUIsA_J9bFBKvEYYDbfXD_8hqo-ZYpA,4880
+kolibri/synthetic_data/benchmark/synthesizers/__init__.py,sha256=i18Pt0Z2_quop994s6T2HptWXbZnbH4GquXyC5DCppc,1063
+kolibri/synthetic_data/benchmark/synthesizers/base.py,sha256=GEuxzhmk0sk0jxeHOLW0YM9fB_y_XZU9LQ_SZ4SwsQg,1992
+kolibri/synthetic_data/benchmark/synthesizers/generate.py,sha256=V1DBF1AEk0gxDAa3LBu3zSghI-zZQ2ZzcbzPysb3OwE,7232
+kolibri/synthetic_data/benchmark/synthesizers/identity.py,sha256=Ly5uf8ZqYHF4o0xdHpQbDx-e6EkZWTfpyP6WPuI71lw,1337
+kolibri/synthetic_data/benchmark/synthesizers/independent.py,sha256=sEw6cHtpAR20koqi9UD1Zn-G5l6WYff4y_G3BhSBgfM,2114
+kolibri/synthetic_data/benchmark/synthesizers/sd.py,sha256=KGSHmYLLg7w7G7uQYd1vVmRTyX2pOukqyy_45oQTobs,3491
+kolibri/synthetic_data/benchmark/synthesizers/uniform.py,sha256=QMGg6K7Gfc6ZyC8WGJ_yquNZAEE7VjJxmvCAukE-ZnY,1665
+kolibri/task/__init__.py,sha256=9BbEOf8w2GeEtMmA8PFZe5vu_v7NSO9OQBcgZvfSsOI,66
+kolibri/task/dnn_estimator.py,sha256=h3wVQh-yMexDJiAsXDl-oED2UXx8uMadymWHO86eEG8,7685
 kolibri/task/audio/__init__.py,sha256=eWvDe5wjqDEyLXTjDp50L9S79wTBiKLdJpAVbUuUifo,104
-kolibri/task/audio/base_model.py,sha256=hZmD4raJ-nl9-FV2lZYamwQ4WBEYN5ypMpQJ7H2N5cs,9852
+kolibri/task/audio/base_model.py,sha256=cqnn55k7J33H8JeQdPuLPCixIAWWIkBMDpvdG-pbtjI,9853
 kolibri/task/audio/classification/__init__.py,sha256=ab4coaEpeyuUsJTC7q81YcnWwRXOE7rbpd2wapdhVys,75
 kolibri/task/audio/classification/dnn_audio_estimator.py,sha256=NO7R87hnAZ8H3NSUfaqLn_tWA3NPRBf0Oz5fGfzeUWU,3231
 kolibri/task/audio/classification/models.py,sha256=IXlSey8RTN2-h7kSrnz5oouap8DhwwzOGrmhODjHs6k,10451
-kolibri/task/audio/nemo/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolibri/task/audio/nemo/asr.py,sha256=p0KxdLRurydMWjo11V7pNdmC6-PSriblCc5kLmEmrP0,7898
-kolibri/task/audio/nemo/common.py,sha256=ETX0d7UohAQXSW6mMeIRK9F8mSWbj6A88yzH9rL9BOw,4329
-kolibri/task/audio/nemo/tts.py,sha256=4e2dPkUoN9m735Sxx7Wfz2EFmbl4EA6e6p_orneeeOI,9128
-kolibri/task/audio/nemo/vocoder.py,sha256=xDu5A4wQ7RjYXqzeT8XuTRZustzStLInjTkmiA0YnRs,5353
-kolibri/task/tabular/__init__.py,sha256=AidTBgYotZoC6ul3XgQRzcVQ7RNgyiQ3LSHHFAcHTf8,63
+kolibri/task/tabular/__init__.py,sha256=ZI9Lr-ZHjCxk5aiY31tWwNy7RcdS72QNHLPc54bM1sI,156
 kolibri/task/tabular/anomaly/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/task/tabular/anomaly/anomaly_estimator.py,sha256=L5IHRAq8G0lDGpVb8SIejE0kY82XteNx8KU8bx7fwPs,1437
 kolibri/task/tabular/anomaly/half_space_trees.py,sha256=2WGQmjTMLhW1m58bjCO93tdl8bp4KWr4oAGpnOLDL3Q,18943
 kolibri/task/tabular/anomaly/models.py,sha256=Hszw2cxZtSQYVhqe01WZZRzZrK3FR_-fWMohowBCDFY,700
 kolibri/task/tabular/anomaly/one_class_anomaly_dector.py,sha256=NaWijpY2l9ja4i-0JItG-WF9IJjcTk_VPBh0VnrgSaw,742
 kolibri/task/tabular/anomaly/semi_supervised_anomaly_dector.py,sha256=t3kAumzTDLOE88rRTwAfVuhvanyMa4IeaiqpExk2S5E,3274
 kolibri/task/tabular/anomaly/unsupervised_anomaly_dector.py,sha256=hfv3scoWA8k2AhsB3sI-EU8a0CWTFjSV4VqAPTRwfSY,4617
 kolibri/task/tabular/clustering/__init__.py,sha256=tGKCWNXTceLGjxO76Wg8WbO2DYZQiUexAQPhxvtwqK0,74
-kolibri/task/tabular/clustering/clustering.py,sha256=Yk-W0y2Br0gNKL6yxhJtc9FBBwPI3vubX_pkNPPTT9M,4475
+kolibri/task/tabular/clustering/clustering.py,sha256=3rjnynWJGtXdPULS_-6YLXPkquXTCH4ivL3V6prpUNE,4518
 kolibri/task/tabular/regression/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolibri/task/tabular/regression/sklearn_regression_estimator.py,sha256=u_jhpdN_L1NFs3SKLxdiHx6pv_jAqXUG0sFcS-ZIKho,2094
+kolibri/task/tabular/regression/dnn_regression_estimator.py,sha256=Ncm65lAr822BlcjG3fHeuFuTv__REWgtD4MkF5NCtDw,1874
+kolibri/task/tabular/regression/sklearn_regression_estimator.py,sha256=KDDDxrpjeNTA1PRBJyrqU17nNjstPG7B48aF6GXdBmY,2170
 kolibri/task/tabular/rulemining/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/task/tabular/rulemining/association_rules.py,sha256=_9mMxCmc8f6J6Cr_532xNVbtgVNVuTRJ_EMQTR8AgEY,9912
 kolibri/task/text/__init__.py,sha256=wy0HhZdrwePNnZIxZJFeQepcRweCbIuB7_v8ZS_e3ak,140
-kolibri/task/text/classification/__init__.py,sha256=6hODYmWa2L1KwNsILmtjJAXrIoHW0kWrOixlNAxF7kI,94
-kolibri/task/text/classification/dnn_classification_estimator.py,sha256=LkIHoEFC0vEfqOviQhaDVXI1VHEbfcvr64ETU0h97XY,4243
-kolibri/task/text/classification/sklearn_classification_estimator.py,sha256=y_xB4bUHaB7MfDCzxPNoohd6odqSqbDGHWAsQmPv414,3128
-kolibri/task/text/entities/__init__.py,sha256=d6Rm5d1yVZUx3V5ThocVXBBcs_Bf51TUAWp5w5JXUcw,3151
+kolibri/task/text/classification/__init__.py,sha256=YrTKGSQR4ykA_15LIkdMlRsOKwcQJJst0n056gXxUx4,190
+kolibri/task/text/classification/dnn_classification_estimator.py,sha256=B9vKwuxJQFR0N-HVDNsmczopwsq5JfmW2bq73XfSeOI,4316
+kolibri/task/text/classification/sklearn_classification_estimator.py,sha256=As4q2fhbjSNu6FB-MGWjgyr-OsQknpGmcOMYMCS2z0Q,3199
+kolibri/task/text/classification/sklearn_estimator.py,sha256=wMBqMU3ay_LQ10aMjhJRflv5s71x_mzcyNeI9iQ5MnE,3407
+kolibri/task/text/entities/__init__.py,sha256=SKUlmOOjZ4Xl7bX8aQjhdprL-nAMmTxiSKc7FhRs3AY,3145
 kolibri/task/text/entities/common_reg_extractor.py,sha256=za0fjoLJuthsD6HIS8RiC5RXzZMOUPJx9TKPZJh6_zM,1990
 kolibri/task/text/entities/crf_entity_extractor.py,sha256=5IGuKTVmYifF2VISf2zc824qTOQVgdFESKGMo9wSE6M,17418
 kolibri/task/text/entities/dictionaryExtractor.py,sha256=3w-VRkpc-QH0skCRGr_chtKdOPSJC3ISeyt6ddcfEnw,949
+kolibri/task/text/entities/entity.py,sha256=yZxwmhwauYfjV-XNJ7Oot2VxlkoZACGcpHvetsQfb0E,1111
+kolibri/task/text/entities/entity_extractor.py,sha256=qSync2Cz2CM_uc9ldIU0KTGKiiVKeyJc8NgYETl43Kg,3007
 kolibri/task/text/entities/entity_synonyms.py,sha256=aSjkSDcggx35BVM9BFoqZOHJ8UP3DaioSZUfULoGGdk,4171
 kolibri/task/text/entities/lstm_entity_extractor.py,sha256=8mJSKAaZeVXMZj8sqecV4sfbM5LrLEOZ8NPCcMP2lOc,6339
 kolibri/task/text/entities/person_extractor.py,sha256=kM7FvNTJpKjCuebgBzXPjJ1xBjVoeCDnVi84qV6Z9lo,3633
 kolibri/task/text/entities/preprocessing.py,sha256=4OSlF1IS0pK1Gr_eJUb5j2VgnW0bc5zykw81IWvozEM,2279
 kolibri/task/text/entities/regex_extractor.py,sha256=BvyqvGx5wJM1TjHBO8TxFqqhVGhOgdziGtyTX8c6caI,2668
 kolibri/task/text/entities/templated_extractor.py,sha256=14sbsSMTvJzDqOwkdhP-pluIaPzSYEg0u5-x_HP0a7w,6945
 kolibri/task/text/entities/test.py,sha256=Aj6kzEwqhtG8CKnb00J_Gr3Pfmd_qRWlMWDtUokj__M,3498
 kolibri/task/text/entities_back/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/task/text/entities_back/common_reg_extractor.py,sha256=7SvlvMvne4e-Lv02_nQYu3beniCeqExaIi7-K4Le8Zw,6458
 kolibri/task/text/entities_back/crf_entity_extractor.py,sha256=fRLiLvrbTUOyL2Bw9NKsC3pXsdd8w6HIoo-vFRzFU88,18309
 kolibri/task/text/entities_back/dictionaryExtractor.py,sha256=j8td9mUO2MrOMsLUj82NEuCxo1U-XIestorFcLzDM6Y,1011
-kolibri/task/text/entities_back/entity_extractor.py,sha256=otn44g8u3A7eG2b_IiWnTAwMzPjSefq5m_2vL4b7GCY,3003
+kolibri/task/text/entities_back/entity_extractor.py,sha256=mSjCZA4CpGiOBV-PCEE0GGwTi0V0qeWXOmIPrtttstg,2997
 kolibri/task/text/entities_back/entity_synonyms.py,sha256=gDV7Tn8FFs_Rk6K8Lavy2r3JpyeRTBuEvF_wfOXHvsk,4343
 kolibri/task/text/entities_back/person_extractor.py,sha256=M6IC3kvUllQCdVrMyOOZjpvwwS86LqXAI0t__5XJ2Qs,3188
 kolibri/task/text/entities_back/preprocessing.py,sha256=CsKkBhy116JAHrEPFdPSdvWX2X2iXeSF6eJvFUC3_3c,2295
 kolibri/task/text/entities_back/regex_extractor.py,sha256=-x11jf6gkHoq-kF3BWh8pYh9BpBOxj1r1x_pMThqxoM,2644
 kolibri/task/text/entities_back/templated_extractor.py,sha256=pOhBMy0Qd36IJ7veT0zMlu0BGUCDG6jKXccLqnJZhbc,6419
 kolibri/task/text/intents/__init__.py,sha256=fDcNlTbX0Nag981_mCZpKs2T5PsFukb3tjC4eXQDQ9M,5
-kolibri/task/text/intents/intent_catcher.py,sha256=h-11CC9b8DTycbSvr6I7m5qEm5k7z1pU7psB34EBr2A,10307
+kolibri/task/text/intents/intent_catcher.py,sha256=wLneCQLlnYV6e-a8JkibK-lQo7II31wuWu1w0ovd3BQ,10289
 kolibri/task/text/intents/intent_expressions.py,sha256=dswwNGVQsFKlFaorkxgj9vzwf1ShmU2xoNSdyxmHw-w,3811
 kolibri/task/text/intents/domains/__init__.py,sha256=Bot0OZIu4znfbUPsbgvgcnlf4rnVHXQfIDBlTjqQd-4,1437
-kolibri/task/text/qa/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolibri/task/text/qa/entity_detection_parser.py,sha256=pVqYmcrkfpwbYYI0xxinrh9b9hDuhVgpwhMVOksjDxM,8959
-kolibri/task/text/qa/entity_linking.py,sha256=MkFBnbmXq476qzkyvDZ9HRI5oG0iPci2txQsSz8fV_Y,22335
-kolibri/task/text/qa/kbqa_entity_linking.py,sha256=J1x8r4m_UXg29XrS14oA4-CUXXR_mIdSt3qjVBOTCrs,23543
-kolibri/task/text/qa/query_generator.py,sha256=t-yVrHvdX2fY3toVpo7cF_p1I13hRqum4PgxTfuBxEM,12545
-kolibri/task/text/qa/query_generator_base.py,sha256=DfrTMP-qEmTvxI0PD7EcgV4FxXOfBkUtvD7o5Kb2L2g,13495
-kolibri/task/text/qa/query_generator_online.py,sha256=VbIF20jvG0PJlz0d_zmjP6jhZxfRVgtLQu63kYEMWFg,10222
-kolibri/task/text/qa/rel_ranking_bert_infer.py,sha256=lxfUUAXbvaKG5tL-DJwr4gXzQXggS04Nui3SshQ17nY,9552
-kolibri/task/text/qa/rel_ranking_infer.py,sha256=urPcY0a_8XJt7Q_e7OZs3Z2wUpduQ4AcfZ2SyRyanOM,3938
-kolibri/task/text/qa/sentence_answer.py,sha256=uokB3sb1RCwbfou4CWSDUOJswMGRFJNT5hJkzzxyYnQ,7257
-kolibri/task/text/qa/template_matcher.py,sha256=vQzIKVfCLR8dZ4NN3Bh5qCHmopYHIhBNBcE8vFK2Nt4,6657
-kolibri/task/text/qa/tree_to_sparql.py,sha256=vE9fl3UJXnCBiF9T87OZOhsVDksnVmbD9-Ds-UukuSc,30317
-kolibri/task/text/qa/utils.py,sha256=ZfYHGQ2JFyUCAFinnT6pEJO4jVV_iBbSLThLNZcxDOY,6141
-kolibri/task/text/qa/wiki_parser.py,sha256=Smi81mIQ7gV4unWx7vYXaOu_i8PBJBGm8YMWGJ-h-Xk,15627
-kolibri/task/text/qa/wiki_parser_online.py,sha256=LlMJLaA72hRoPXiPAMr7hnJ2n_rs476zbU7pnl18xk4,4572
-kolibri/task/text/qa/squad/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolibri/task/text/qa/squad/squad.py,sha256=3Zu0MkUYn5HZ65VLQxtQs1h8N-iOMud6Or3s4HyB4LI,16890
-kolibri/task/text/qa/squad/utils.py,sha256=f4el5nE6GP-TydHusVIuYJCvHIspcWLapBlyOD_SdJs,10294
-kolibri/task/text/relations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolibri/task/text/relations/losses.py,sha256=PWOI1S93GtB_4M_k34qMsqbivfpK9I86tjQgq9biZzM,2434
-kolibri/task/text/relations/relation_extraction_bert.py,sha256=IMVYg4O0GLR11Toxjw8oXZwJUWDfoAp5Z2hp7ZfxELE,6541
-kolibri/task/text/retrieval/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolibri/task/text/retrieval/logit_ranker.py,sha256=lPmOdQmRWO691fQf_koXp6OeuD_hsfGaZmHwWmIG09o,6170
-kolibri/task/text/retrieval/pop_ranker.py,sha256=C44kqCmHsUIWpqL1M4qvWdOp-LDjx8qAFVD9XpLsOJ8,3537
-kolibri/task/text/retrieval/tfidf_ranker.py,sha256=By3yvRk_WOgpITvDK98S_Um9_Txb_nB4pLjHPM2226s,2326
-kolibri/task/text/retrieval/utils.py,sha256=vLKBpTOxOAiVgsV__sNIuW0xzoHkhSt2V_fxFAoPebU,631
 kolibri/task/text/sentiment/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
 kolibri/task/text/sentiment/lexicon_sentiment.py,sha256=YNPcwJaDvn8PbdBFqGwgOghmapQitXZVhj3eGzoXDzU,12971
 kolibri/task/text/sentiment/util.py,sha256=QD4S8_Km9BAXZuYU1CeBfUHVHboChtKi3W1vXYIIAF8,32780
 kolibri/task/text/sentiment/vader.py,sha256=SQF11vyVwJARaB5h2UYim5BdRjEsqrJM4T4EMySMH18,22769
+kolibri/task/text/similarity/__init__.py,sha256=x0QE9QwARft5UVnWwaVl1MpH4NOEidXnpE_8WckESdo,2587
+kolibri/task/text/similarity/arxiv.py,sha256=M_AsKDzDgdTdgNVjzAnYyrFfYMrS0hcNOTzRSIJJVQs,559
+kolibri/task/text/similarity/docarray.py,sha256=BIEHjqewtNLD6wpN4b34yf9CP7gcyap-J8CPaYEbMBI,6717
+kolibri/task/text/similarity/knn.py,sha256=LZXBaOlxn55qT8heZeZN1-tJE3p-7gYOUZG9YMXSxXo,2361
+kolibri/task/text/similarity/llama_index.py,sha256=opGeqCqugtaeR46_VVEihuGHDZn66TmpvTs3DIiISvU,2907
+kolibri/task/text/similarity/merger_retriever.py,sha256=ZW560fBnjZeGvyxeYB7K4hfOK0u66od0PNNLznAssnA,2907
+kolibri/task/text/similarity/pupmed.py,sha256=PS6rSTjCykhGrg2lCq5mh2voOUyt0trSwuke_klMLVo,569
+kolibri/task/text/similarity/svm.py,sha256=dyi2bmM3OBW3XkFGkeEjNa0AJfpWIcK3YgM87LEg8vQ,2953
+kolibri/task/text/similarity/tfidf.py,sha256=etGpiFTk4dv8Atx1mCpouKZ7Ubcz6RdntIWt5N2pJY4,2470
+kolibri/task/text/similarity/wikipedia.py,sha256=Vguf-S9l7dWVu_lkbGet54RiqXrfLjE3QVm8u1BrcU0,579
 kolibri/task/text/spelling/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/task/text/spelling/brillmoore/__init__.py,sha256=NQiWdo45nHyrRcDRnbqufELCly5Gx3wDAQZBijoOdrE,36
-kolibri/task/text/spelling/brillmoore/error_model.py,sha256=LmXMIHDdlzvCQ02n1ojmd8-tPSMQG2Xfra4hPYMyMh4,10846
+kolibri/task/text/spelling/brillmoore/error_model.py,sha256=FuynXhjKZ_HyJsixgAZtQH2fVbpMvx1dYmVE8iBi4dg,10769
 kolibri/task/text/spelling/electors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolibri/task/text/spelling/electors/kenlm_elector.py,sha256=SkwZXAoi4zDNQe62TYQ_NvLhwGO6nCxqm7dGWxUIGJk,2861
-kolibri/task/text/spelling/electors/top1_elector.py,sha256=wXFWxU22NOWnpK7mH4yOOUf3vYYJCGxHdxrtyM5a-7Y,1446
+kolibri/task/text/spelling/electors/kenlm_elector.py,sha256=H3I2hrosBpby1i8ADeynN0D8hoZzPIwvGat_HHsPiY0,2815
+kolibri/task/text/spelling/electors/top1_elector.py,sha256=wgfHATkEe7IU7jDLQr67EhIjSSwslHuM0gBCLeDxxcE,1421
 kolibri/task/text/spelling/levenshtein/__init__.py,sha256=VHiN2Sv2iY0OxHEKA0kmVDYP35WQh80OckogjZRV8Pg,61
 kolibri/task/text/spelling/levenshtein/levenshtein_searcher.py,sha256=boARfAEmqKjnCDw85fwSm1u16TUuaT6lJgcvBmBPPOI,33386
-kolibri/task/text/spelling/levenshtein/searcher_component.py,sha256=vR9K_8fSlPnEv0e1l9XxiHZstMRBOT5eTwdvVJmCEdE,3423
+kolibri/task/text/spelling/levenshtein/searcher_component.py,sha256=GH23nSTAs1HNj8cq_4lkZ2WlM4CegONazDAtOAf7u7Q,3406
 kolibri/task/text/spelling/levenshtein/tabled_trie.py,sha256=iR8FNBe0OKw9RvnVYQE8CXLze2RgUemhhosHw1JPK80,20586
 kolibri/task/text/topics/__init__.py,sha256=g0CWthZqZr8Jvi6DAV-3a9NXg6RqK9uQbLsjXdNHskE,152
 kolibri/task/text/topics/baseTopic.py,sha256=U1R2M-d000ggiEkkxFI1IkqXpzfZQr5Anp-RmYjbpes,3563
 kolibri/task/text/topics/mallet.py,sha256=ZAvXycvp3PaLU9kLMk5TGRg922lYa8KMI8sZH8ZmmwI,24958
 kolibri/task/text/topics/topics_estimator.py,sha256=iVG5kp0Tv4PhAC3awy7q6_jZVyNLDwSbQNb9bKaS1Jk,14976
 kolibri/task/timeseries/__init__.py,sha256=2q2W_Du5Flox9oLOSqUE6po3mjDyrp_Y1IA3s_hjgjI,58
 kolibri/task/timeseries/dataset.py,sha256=R4bFOTqHbRjsFmbPoKKjbSS8P6xKfryW7AWgZViUk40,23782
@@ -419,74 +589,111 @@
 kolibri/task/timeseries/analysis/feature_relevance/relevance_table.py,sha256=VvtAdg0v5QlqnKCtSIuZs5FQgX3P7IhdKsyxhozVmtE,2919
 kolibri/task/timeseries/analysis/outliers/__init__.py,sha256=KXxUdUXCOAey8kkK_CZpdYcsqjbt5HEMs_mI7Wb-bK0,583
 kolibri/task/timeseries/analysis/outliers/density_outliers.py,sha256=NLjzCKwrDvIUS5Y1hh7Bd74bu48Ok4BJ57E67c6mAU8,5017
 kolibri/task/timeseries/analysis/outliers/hist_outliers.py,sha256=lRVmbNYAvSjTmYKbiKXFFHZb4w2DDryrRU9_JiHKQsE,13178
 kolibri/task/timeseries/analysis/outliers/median_outliers.py,sha256=LOIVmtYKezbFcfM0gZqztPqEx56sWy7O0gDgyeeyg5A,1878
 kolibri/task/timeseries/analysis/outliers/prediction_interval_outliers.py,sha256=Kap9gxlRsKKyxoHqwsd74RBN9f1XO3YFr7cMlyF21XU,2998
 kolibri/task/timeseries/analysis/outliers/sequence_outliers.py,sha256=PiaW43p09ATc0P9dYIEKztiIqQoP2bw3q60YnHEJlPQ,3501
-kolibri/tokenizers/__init__.py,sha256=YNIIckSTcxzJiEHbKhuqSd3GWti0N4dNqdWuFa_Va98,1411
-kolibri/tokenizers/bert_tokenizer.py,sha256=V7JOAkvK8236d922HaqlWqEBQYW2ERXJss6FFQBiGL8,4709
+kolibri/tokenizers/__init__.py,sha256=Jj-Y5GOcx1YNO-gf9yajTbW4hCNE15lWexB5JgHOxN0,1470
+kolibri/tokenizers/bert_tokenizer.py,sha256=IqspexqV_7byM3UvdYRU8TIgoL6ycfAdZs0M6dcImQI,4690
 kolibri/tokenizers/char_tokenizer.py,sha256=YevabURuHJ716HKCWiiORZHc_Cs9KDeDx7_3c5MLoDI,3999
 kolibri/tokenizers/kolibri_tokenizer.py,sha256=ofvGQVkI6lC7nhIwViYHDceVptTFwhbKOJmwr2sZMts,7103
 kolibri/tokenizers/multi_word_tokenizer.py,sha256=jt9WQPm3OrK7m77CFVZ0seUlI_e5U0TkaJkNGoa5k1c,2361
 kolibri/tokenizers/regex_tokenizer.py,sha256=tHtenqZnad4gD1kPGj1A3Zm7nm8_XMiBIJzyx5RqXJA,2661
 kolibri/tokenizers/sentence_tokenizer.py,sha256=1obx34ndBgLP3oipTAgCpiVtnUJgBRTYqYYB4gN4WzU,1025
 kolibri/tokenizers/tokenizer.py,sha256=So7J0D02ib0-tRZzuIXj4cggVsZyv3iGt8iyv1KDNXc,2708
 kolibri/tokenizers/ugc_tokenizer.py,sha256=-Ja9ICY5mgwaLb09B6RvXRTlF2Ao5j17VZcvTBDIZUk,6936
-kolibri/tokenizers/word_tokenizer.py,sha256=7I6A1pEkQQwJ8CMdC32Wk9mcZegYNqGmj1JqlXvtBfY,2340
+kolibri/tokenizers/word_tokenizer.py,sha256=D-aYGuTFpwK9vEZaSwW0sorhg7WgGHeJNMKZ-bGJig4,2404
 kolibri/tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/tools/_regex.py,sha256=4xOVvbQMT7mF4Lk8VbaBQ1jxovHd8irZMfT-4BdnDhM,411
+kolibri/tools/arxiv.py,sha256=B0xvh51ZX6_1_ix8_JdHwIwGEbXMra9yOI4VWdTT0rM,841
+kolibri/tools/bing_search.py,sha256=84MmQav3HKN1DifgVfWK4xgBLljueYGQKGQFGEr6570,1208
+kolibri/tools/ddg_search.py,sha256=um7jz6HUmyRDSfF7p7v8Jg58KvpcYaDVoMbEmwiIsGs,1441
 kolibri/tools/gebbrisg_detector.py,sha256=P93bR1lQwM6YM7btNoFXzwg7pQEw44MThj9zaZ2ldGk,2063
+kolibri/tools/google_search.py,sha256=_whh0Nw0uZSoMZH8SLhYfwfiTebqmNwEUrgBWitDQec,1231
 kolibri/tools/keywords.py,sha256=S-aObU6a_m-YLqWvja_qkcfOSrRXpWmpYIPK7nRmMp8,25525
+kolibri/tools/openweathermap.py,sha256=qTaS8R2N_Fl2iJ74L2LOB2JtDsNjPr9Mxf76r_yLw3M,777
+kolibri/tools/pubmed.py,sha256=svWnpq8NC23m4vNnPvvHhP1ZfmIAj5pKFihqmSD0Yzc,853
 kolibri/tools/regexes.py,sha256=Q3QQyx6qpmqb7uqLMWtOgvREIX0NXy-bny2-O7T2hGE,1828
 kolibri/tools/scanner.py,sha256=559YiFUmFD5LclMm_dGINI8WIvzKENejomUC0U6j1sE,17263
+kolibri/tools/wikipedia.py,sha256=kjcNWdkMl6HEImbdv4N0Gz9UuUh0_4LCnU_3wZf1N4g,690
+kolibri/tools/wolfram_alpha.py,sha256=IsOQ1dvyR4ByaNx_YJqmju4pf0vTM4R4zGAHtQ_v--E,699
 kolibri/tools/word_frequencies.py,sha256=ndfI99FfphDO-Xtq12Wnix3Sk7aVFBDOG2ze6UIfJTA,13056
-kolibri/utils/__init__.py,sha256=mne_21Gep-3uP9a0ODTqU_usYbyZkBJt02bEIVx81cg,1754
+kolibri/tools/youtube_search.py,sha256=maPdPdoH0YLujc5SW7r8QSjyQREalWNEw4hnqjcAj0M,1447
+kolibri/utils/__init__.py,sha256=lyBPk7FM0T7nXKOw2pDxIpq4cZwxiMhsKqTNl5tzGDU,4826
 kolibri/utils/cm.py,sha256=xXf6K8l8mORue2EfCIM5NzvpkAISlWjO3InvmB0cMoc,11174
-kolibri/utils/common.py,sha256=dVxHy58meQFVGw4FY_y25zxVATRtVHt-hapd8LEy8NE,6589
+kolibri/utils/common.py,sha256=c3razuYtX7ELiRYNTSEXQXpBSq81ssWg9u3iZsKzzcY,6904
 kolibri/utils/config.py,sha256=qmcpjeS9B9J8zcKV79Wd4nmL_urBj_h-vTAIX8fowkM,3173
-kolibri/utils/cross_validation.py,sha256=7VJCHEkXTs0qh_FZ5LTsQM8X5y9QKOKI4F3nfxSvByE,11887
+kolibri/utils/cross_validation.py,sha256=oxYpuuEhHMEcVLx0g0EZ0AuppyZMBRO3-mtdpnZT3RA,12009
 kolibri/utils/distribution.py,sha256=rJFXEUUgixpyueTBH6ZHlbq0Uig1-LvHkEVg48sr76U,14474
+kolibri/utils/environement.py,sha256=IB9Cp5DrBy1RrPqHKix9mUVVWhUA0Aji8Imy3WydxX8,873
+kolibri/utils/language_info.py,sha256=MxLTC_9odTRgNKDgN_w4mrMEYuWyfih_dxwGTwAUW64,3259
 kolibri/utils/log_normalizer.py,sha256=jiqdte_24Ge1I9qVme4nBa4X8jikzgydGqKBsbobEt4,544
-kolibri/utils/timeseries_functions.py,sha256=V6p3BenopiLKYvzrurSARGpImSwlzvriH78x83wSGuQ,28841
+kolibri/utils/mathext.py,sha256=wBa1EobE3bzdQqPfTA71c8eNKtiirJd5rD5hhm0gP5U,5686
+kolibri/utils/matrix.py,sha256=8N-2XU398bUxonr7n2vlST9mXe4qEFYCVAGTEWH56Jg,2904
+kolibri/utils/nb_clusters.py,sha256=V485u3qTggAhVKUIHgFw7OqfXgl3Q7DdVk8APvB8VYw,3158
+kolibri/utils/parallel.py,sha256=da-WNpIKjaqqprIQmiWHDqjG1fa5ZXKv8K4SEDcqPDA,631
+kolibri/utils/progress_bar.py,sha256=Ket95lzKqFnGn5VffYqu1pDkUI6MlXduhZTI7-3i3sQ,2361
+kolibri/utils/serializable.py,sha256=YRJ6K6Jeln5WbQFESPawalle7TRgnBKJu48JaV-V4yc,4618
+kolibri/utils/spinner.py,sha256=aqAo-XgaLhUoLGw2NMTRyWlObdQqgbAOBT4AeyWw-1E,2280
+kolibri/utils/text_encoding.py,sha256=zUcnsMMEy6uKIC90HvrpRTo_EH7D3K7YIEAm_ZdOxcA,1252
+kolibri/utils/timeseries_functions.py,sha256=7OCP8mEzrYPPQmvVCgVnBLTeb9oXOVj7PVElmRObQqM,28893
+kolibri/utils/timeseries_functions_back.py,sha256=CSrLMBWD4cHQuWOJL2ugjk5KZon4L7nWQasnm92JRPg,28840
+kolibri/utils/wrappers/__init__.py,sha256=K1NT89U8c5kwZbu9FsuyApldYG6uR3lU3DKclnYi_nA,547
+kolibri/utils/wrappers/arxiv.py,sha256=G8qfcXZnJ7n3TSweX6Rv165hPVhC2BuJ92F_fF3XRLM,5589
+kolibri/utils/wrappers/bing_search.py,sha256=Z2TswSoSjfrBuJEiGVYPinN9oeOfK2xxcUaBrV8stYQ,3344
+kolibri/utils/wrappers/duckduckgo_search.py,sha256=jo6w_47aIH36p5s6iCkrkz7XFsjss7Z-pc-ktZa369s,3330
+kolibri/utils/wrappers/google_search.py,sha256=e05mMdBXh1c5U0eXR9lK9bLqH3ZtIEDMFuss44dHue8,4910
+kolibri/utils/wrappers/openweathermap.py,sha256=jrG4NZKz7C5hCepXu-wk1yMI8jX4BcZv_qPlshiDzoM,2431
+kolibri/utils/wrappers/pupmed.py,sha256=Pf9fis-Uh5R5SDv0lhvOBi4Ek-pc04iDKekusJTRNPU,5742
+kolibri/utils/wrappers/wikipedia.py,sha256=2xaWnOd3SYRh0lJ8R2PI2QmziWi484Ixjt1zPfZrwiY,4035
+kolibri/utils/wrappers/wolfram_alpha.py,sha256=2-M6hMCyFule-FPMhb5ub3F_zK-VW62MZZU-RiEXlLY,2000
+kolibri/vectordb/__init__.py,sha256=iGEalx59TuD4tdW5pJwf-BVavRUo7T4sBCXxjSK0O3s,347
+kolibri/vectordb/base.py,sha256=pVTyZ0dVgM9z5cRLs1xCtUkWnbZx63LVygNan6bcipE,16298
+kolibri/vectordb/faiss.py,sha256=2bpSbGvCAMdC3vczvMnoo0rW0os7wB6eD7iTErfj39Y,23410
+kolibri/vectordb/redis.py,sha256=oHAn3vPWkJMqjENG2QYEC7aKcVbTF0PfdYCJjgiW6w8,21803
+kolibri/vectordb/sklearn.py,sha256=lQMz81ZG6wkR06a1NR_0D8cQ15j-bqMspy_ViW0Nd80,12276
+kolibri/vectordb/utils.py,sha256=nK3i82sNwurJJDc1mg9iBoAx08qpyecPPTodqYAXqH8,1462
+kolibri/vectordb/docarray/__init__.py,sha256=KK4uIKLQqG6pit4EJgfZH2fICaeZvu3xvpfnhrBJ5JU,204
+kolibri/vectordb/docarray/base.py,sha256=irUR9UEjuYYkWJ43oRhfpqdNJLq3fv9NckluempVeNE,6872
+kolibri/vectordb/docarray/hnsw.py,sha256=k0q_5iDxIVda9vAGP0RvoJwkVsH6aPYtkDX-5rMQ8O0,4062
+kolibri/vectordb/docarray/in_memory.py,sha256=lkMYlJHssuAc4ZI7ia_UsfKLSdXbOyAFoyjbD0yONmw,2416
+kolibri/vectordb/docstore/__init__.py,sha256=uP5oA4wBVJ3P-tMqF_dAyZ0aSpLIFKNpXe7WtSGVgfQ,280
+kolibri/vectordb/docstore/arbitrary_fn.py,sha256=t36gwb_lJ8ng68Q4h5OIxCbuM8P-39A1eRuUSvbLkpA,924
+kolibri/vectordb/docstore/base.py,sha256=FKOH5Pgty0KxQu9fTNpK7CdH7khNvClOF5HJPq2leaY,694
+kolibri/vectordb/docstore/in_memory.py,sha256=PYDLIdJ4PJOEM9rpyd04nSxFghc75CzTBDspSaX5a4o,973
+kolibri/vectordb/docstore/wikipedia.py,sha256=E0cNtCh1Cvio_Qm54soJT8AiJZsO98NniATF63wtVtc,1376
 kolibri/visualizations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kolibri/visualizations/classification_plots.py,sha256=dnFOQjbXk2KTn41wyDAneMNHv3VSwaKQ-P7CKtsevy4,53405
 kolibri/visualizations/pipeline.py,sha256=KXNnLW2yfzSosb_CcZX3KttAnFhqKi20ZZvqMqMFhZU,15746
 kolibri/visualizations/regression_plots.py,sha256=Hr9xL-Fi9J9ElLR8qbmXFS0XOXAbVacIrOmi7Luh22w,34339
 kolibri/visualizations/utils.py,sha256=YWNyh28EY6QcQ11cr2i72LiEv1cj9MBhJgv3-aEuXJw,15565
-test_backup/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-test_backup/dnn/__init__.py,sha256=BcvK8F7U0aOC9u5ADIgnkXcTUSCuMzqxWQocYYYFw30,2623
-test_backup/dnn/audio/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-test_backup/dnn/audio/test_classification/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-test_backup/dnn/audio/test_classification/test_pipeline_model.py,sha256=k_c4Mke7iMrxbi81MN_Aal_9NiWCxOqMY7p-6LF9bdc,2435
-test_backup/dnn/text/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-test_backup/dnn/text/test_classification/__init__.py,sha256=HQIsf2WMZW1DWIT9yGZCRWvo7_MH-Y6GsTSwlz1gJ9Y,176
-test_backup/dnn/text/test_classification/test_bi_gru_model.py,sha256=d1_cyg1DUI72-B5bKf3MTUe5bIsqYj943sjpoHctU-g,575
-test_backup/dnn/text/test_classification/test_bi_lstm_model.py,sha256=5mL9TDU56sgLFIsiyvKa7P_XLKKCdg7-10q0cgDkGig,4129
-test_backup/dnn/text/test_classification/test_cnn_attention_model.py,sha256=lHL-0e3JGOcYvaKCht6dpQG6Q1zjNrRAR_6SV9_WU4M,718
-test_backup/dnn/text/test_classification/test_cnn_gru_model.py,sha256=u-pPtNAQNKOuOQpcCGr3mka3_g3ddEXHLlqxcMbJmlI,581
-test_backup/dnn/text/test_classification/test_cnn_lstm_model.py,sha256=fDIsYXMX_V8sI1PLtR9uALNDRHpvMd1qJty6Sid-Duc,584
-test_backup/dnn/text/test_classification/test_cnn_model.py,sha256=e_qFyBaj-NXp8AY0JyiZvuoHLLtDDBEmO1FW2qoIOiU,571
-test_backup/dnn/text/test_embeddings/__init__.py,sha256=-GqoftNECZBtC8F82KWJrdSD05BcKBrrL0ElHEEUHyk,36
-test_backup/dnn/text/test_embeddings/test_default_embedding.py,sha256=L6BfhT5EZ3GN9ySUDKXa0XkfiXPuElSn5-teWgNVQvo,2235
-test_backup/dnn/text/test_embeddings/test_word_embedding.py,sha256=Nyy8_b4csxoRUSHCFTtnToflT4Iz-NeLWwghbHfznDA,819
-test_backup/dnn/text/test_indexer/__init__.py,sha256=-GqoftNECZBtC8F82KWJrdSD05BcKBrrL0ElHEEUHyk,36
-test_backup/dnn/text/test_indexer/test_label_indexer.py,sha256=E3kKDI_jDZ5OSk9Hfv3yUXgAa2kV2H9mkJv4hy-qveY,1692
-test_backup/dnn/text/test_indexer/test_multi_content_indexer.py,sha256=RTi1-Z4ZvZIQwDfh2mZSZ0f_7FmevkrkA8gvi0cSkxo,1149
-test_backup/dnn/text/test_indexer/test_multi_target_indexer.py,sha256=u0Silw_HrsG3DT0nDe9yindeBjStAPIvOvxyKWUXROM,1618
-test_backup/dnn/text/test_indexer/test_sequence_char_indexer.py,sha256=lkC1Hj9D_3cFB6jk8haZ_SeOEtpb5D-SxF8pZMDJMpg,1040
-test_backup/dnn/text/test_indexer/test_sequence_indexer.py,sha256=UDiEnVxNvASHaFxuAq3woY43X-HFSJ_XSqfYdEAVfW0,2080
-test_backup/dnn/text/test_labeling/__init__.py,sha256=8GNeI935Ac0YjYpEZXe21qsHksFEV5ya1JKEQFF0k94,55
-test_backup/dnn/text/test_labeling/test_bi_gru_model.py,sha256=Lk7iNE143jwoDeWKUpc4Ql0qcHfcXOefAQm54U-qlw4,1642
-test_backup/dnn/text/test_labeling/test_bi_lstm_crf_model.py,sha256=eNQ0CmrsiGLZjP9q95et6bmQspImyWQ0C_NTnRlTV78,375
-test_backup/dnn/text/test_labeling/test_bi_lstm_model.py,sha256=Ey2k-ssTm8PXeX-yZb1r-7OlkL4ugs5BLnOp2FUrrKY,2738
-test_backup/dnn/text/test_labeling/test_cnn_lstm_model.py,sha256=Jm6_jqeC3XVZ3-TDoiM6uigxKSlZgoHcUzGPjUnH_sk,371
-test_backup/dnn/text/test_seq2seq/__init__.py,sha256=-GqoftNECZBtC8F82KWJrdSD05BcKBrrL0ElHEEUHyk,36
-test_backup/dnn/text/test_seq2seq/test_seq2seq.py,sha256=OHpT2hKwa5UlTGNzsAH_1f8PUZZ1aeLVRrW2PzHss6s,889
-test_backup/entities/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-test_backup/entities/test.py,sha256=eCs9onCMFIhoDVts8PyZD7q6Oa8ADGHMc3dV3OcokuA,7837
-test_backup/optuna/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-test_backup/optuna/test_optuna.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-kolibri_ml-1.1.8.dist-info/METADATA,sha256=BQRTsfZOmjDhGuH0kXtPoh6ER_Dtuus9kOUPvBKkTaI,4594
-kolibri_ml-1.1.8.dist-info/WHEEL,sha256=00yskusixUoUt5ob_CiUp6LsnN5lqzTJpoqOFg_FVIc,92
-kolibri_ml-1.1.8.dist-info/top_level.txt,sha256=k0n6LfyF9is1aJ7TjPcu79b1EQTACOS4Be6xJy8qQ7I,20
-kolibri_ml-1.1.8.dist-info/RECORD,,
+tests/__init__.py,sha256=cLEG0Ty3GCvE16djVZjDu8rlBEUAVjwMZXa9fQlxVt0,52
+tests/test_data_transformer.py,sha256=Wy8Uqsl0DAzcOyn1-IYWEa1hHcMoy_eQUx9DBSwqJNc,20075
+tests/test_pipeline.py,sha256=BhvJX-IqJ_5EWnVj-VfXiM2LzR3-y9DGf3hZEaxEs50,960
+tests/utils.py,sha256=vvK537soXHoQnfBgTZw7yAtUjMO0pUWSSLcy8fH1pEg,557
+tests/entities/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/entities/test.py,sha256=KmyrZiq52x4rE5gmX3o_5tXDnqwJzihazIYWEr179-g,7812
+tests/optuna/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/optuna/test_optuna.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+tests/synthesizer/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+tests/synthesizer/data_modules/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/synthesizer/data_modules/test_conditional.py,sha256=BIkps93AFQNPFLu0xYgmJpOIKg6zd6-IzzN7BjBCti8,2865
+tests/synthesizer/data_modules/test_sampler.py,sha256=jW0BCEdnGMMkqvmfS_e4SyeauLY0-7H8ZnUHr1QoD7c,1131
+tests/synthesizer/data_modules/test_transformer.py,sha256=rSr3IxgNmtCYWRnoluoYtkgVo-qB_Fmu33A-dkxu69E,2949
+tests/synthesizer/layers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/synthesizer/layers/test_gen_activation.py,sha256=0-PVulR2vmvn_NKf0idurlrFR9FVRVyI4YWWfJNoATo,7960
+tests/synthesizer/layers/test_layer_utils.py,sha256=QoOYzrnk8ZTZelOH7rBkWbc1GVfd7Aq-ENfeXzjSOK4,1429
+tests/synthesizer/layers/test_residual.py,sha256=gJXtux2qfOU1NAYYvmUUOOSPTYjyYs1V6O5pPfani1o,4793
+tests/synthesizer/losses/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/synthesizer/losses/test_conditional_loss.py,sha256=0M-0-jADLCloslFs13GBqpLch_qvH7hatu3VvnaebhE,1128
+tests/synthesizer/losses/test_gradient_penalty.py,sha256=59gDBEWqfW91QiijmW1oAZJNY_r0T8lu2CINX-z_bhU,812
+tests/synthesizer/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/synthesizer/models/test_critic.py,sha256=A3Kgay2o4n0HkbIu9n1TDxRMw8G37r3HLdhb2qh0eSk,1214
+tests/synthesizer/models/test_generator.py,sha256=RI3E5_RKcCxnMSN4y0am6ar4ey-pxp5DQ8_LhHXa4ZQ,4972
+tests/synthesizer/synthesizer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/synthesizer/synthesizer/test_synthesizer.py,sha256=qfsM8Okg8bW8V5NTKe657OiBFc7xKcD2dvkbqFm3_qg,4090
+kolibri_ml-1.1.80.dist-info/LICENCE.txt,sha256=eKw0ToK5-JtbuPy1tofBiXFxGgk1zhq5x0mB7gnTxc8,34572
+kolibri_ml-1.1.80.dist-info/METADATA,sha256=LS5gG83zFKotg6eDijwD0Dm_5RcmW6HGzEiLNr3VJ0E,4885
+kolibri_ml-1.1.80.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+kolibri_ml-1.1.80.dist-info/top_level.txt,sha256=yZ09x7U41HE_HCr8pIum9-4eicynuHE26_L6DqI97b8,14
+kolibri_ml-1.1.80.dist-info/RECORD,,
```

