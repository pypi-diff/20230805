# Comparing `tmp/darts-0.9.0.tar.gz` & `tmp/darts-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/julien/unit8/darts/dist/tmp0ah7ztz4/darts-0.9.0.tar", last modified: Fri Jul  9 15:44:37 2021, max compression
+gzip compressed data, was "/Users/julien/unit8/darts/dist/tmp0tpu_7pu/darts-0.9.1.tar", last modified: Sat Jul 17 13:20:17 2021, max compression
```

## Comparing `darts-0.9.0.tar` & `darts-0.9.1.tar`

### file list

```diff
@@ -1,222 +1,226 @@
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.616452 darts-0.9.0/
--rw-r--r--   0 julien     (501) staff       (20)      253 2021-07-09 15:44:02.000000 darts-0.9.0/.bumpversion.cfg
--rw-r--r--   0 julien     (501) staff       (20)       48 2020-08-26 18:23:45.000000 darts-0.9.0/.dockerignore
--rw-r--r--   0 julien     (501) staff       (20)      154 2020-10-07 09:45:20.000000 darts-0.9.0/.gitattributes
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.335234 darts-0.9.0/.github/
--rw-r--r--   0 julien     (501) staff       (20)      530 2020-10-07 09:45:20.000000 darts-0.9.0/.github/CODEOWNERS
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.336305 darts-0.9.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 julien     (501) staff       (20)      544 2020-08-26 18:23:59.000000 darts-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 julien     (501) staff       (20)      624 2020-08-26 18:23:59.000000 darts-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 julien     (501) staff       (20)      497 2020-08-26 18:23:59.000000 darts-0.9.0/.github/pull_request_template.md
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.338021 darts-0.9.0/.github/workflows/
--rw-r--r--   0 julien     (501) staff       (20)     4049 2021-05-21 08:07:27.000000 darts-0.9.0/.github/workflows/develop.yml
--rw-r--r--   0 julien     (501) staff       (20)     4087 2021-05-21 08:07:27.000000 darts-0.9.0/.github/workflows/merge.yml
--rw-r--r--   0 julien     (501) staff       (20)     5589 2021-05-21 08:07:27.000000 darts-0.9.0/.github/workflows/release.yml
--rw-r--r--   0 julien     (501) staff       (20)      230 2020-10-07 09:45:20.000000 darts-0.9.0/.gitignore
--rw-r--r--   0 julien     (501) staff       (20)    20403 2021-07-09 15:18:43.000000 darts-0.9.0/CHANGELOG.md
--rw-r--r--   0 julien     (501) staff       (20)     2463 2021-05-21 08:07:27.000000 darts-0.9.0/CONTRIBUTE.md
--rw-r--r--   0 julien     (501) staff       (20)      694 2021-02-03 09:29:17.000000 darts-0.9.0/Dockerfile
--rw-r--r--   0 julien     (501) staff       (20)    11338 2020-08-26 18:23:45.000000 darts-0.9.0/LICENSE
--rw-r--r--   0 julien     (501) staff       (20)       19 2021-04-14 13:41:53.000000 darts-0.9.0/MANIFEST.in
--rw-r--r--   0 julien     (501) staff       (20)    10596 2021-07-09 15:44:37.616642 darts-0.9.0/PKG-INFO
--rw-r--r--   0 julien     (501) staff       (20)     9359 2021-07-09 15:18:43.000000 darts-0.9.0/README.md
--rw-r--r--   0 julien     (501) staff       (20)     4316 2021-05-21 08:07:27.000000 darts-0.9.0/build.gradle
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.338579 darts-0.9.0/conda_recipe/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.339305 darts-0.9.0/conda_recipe/darts/
--rw-r--r--   0 julien     (501) staff       (20)      699 2021-07-09 15:44:02.000000 darts-0.9.0/conda_recipe/darts/meta.yaml
--rw-r--r--   0 julien     (501) staff       (20)      133 2021-04-19 19:17:01.000000 darts-0.9.0/conda_recipe/environment.yml
--rwxr-xr-x   0 julien     (501) staff       (20)      556 2020-10-07 09:45:20.000000 darts-0.9.0/coverage.sh
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.368282 darts-0.9.0/darts/
--rw-r--r--   0 julien     (501) staff       (20)      902 2021-07-09 15:44:02.000000 darts-0.9.0/darts/__init__.py
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.376438 darts-0.9.0/darts/dataprocessing/
--rw-r--r--   0 julien     (501) staff       (20)       72 2020-11-09 21:16:27.000000 darts-0.9.0/darts/dataprocessing/__init__.py
--rw-r--r--   0 julien     (501) staff       (20)     8437 2021-05-21 08:07:27.000000 darts-0.9.0/darts/dataprocessing/pipeline.py
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.382013 darts-0.9.0/darts/dataprocessing/transformers/
--rw-r--r--   0 julien     (501) staff       (20)      385 2020-11-09 21:16:27.000000 darts-0.9.0/darts/dataprocessing/transformers/__init__.py
--rw-r--r--   0 julien     (501) staff       (20)     7470 2021-05-21 08:07:27.000000 darts-0.9.0/darts/dataprocessing/transformers/base_data_transformer.py
--rw-r--r--   0 julien     (501) staff       (20)     5916 2021-07-09 15:18:43.000000 darts-0.9.0/darts/dataprocessing/transformers/boxcox.py
--rw-r--r--   0 julien     (501) staff       (20)     7896 2021-05-21 08:07:27.000000 darts-0.9.0/darts/dataprocessing/transformers/fittable_data_transformer.py
--rw-r--r--   0 julien     (501) staff       (20)     6919 2021-05-21 08:07:27.000000 darts-0.9.0/darts/dataprocessing/transformers/invertible_data_transformer.py
--rw-r--r--   0 julien     (501) staff       (20)     5113 2021-05-21 08:07:27.000000 darts-0.9.0/darts/dataprocessing/transformers/mappers.py
--rw-r--r--   0 julien     (501) staff       (20)     2401 2021-05-21 08:07:27.000000 darts-0.9.0/darts/dataprocessing/transformers/missing_values_filler.py
--rw-r--r--   0 julien     (501) staff       (20)     4557 2021-07-09 15:18:43.000000 darts-0.9.0/darts/dataprocessing/transformers/scaler.py
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.383459 darts-0.9.0/darts/datasets/
--rw-r--r--   0 julien     (501) staff       (20)     7778 2021-07-07 15:04:10.000000 darts-0.9.0/darts/datasets/__init__.py
--rw-r--r--   0 julien     (501) staff       (20)     5000 2021-07-09 15:18:43.000000 darts-0.9.0/darts/datasets/dataset_loaders.py
--rw-r--r--   0 julien     (501) staff       (20)     5861 2020-08-26 18:23:45.000000 darts-0.9.0/darts/logging.py
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.384843 darts-0.9.0/darts/metrics/
--rw-r--r--   0 julien     (501) staff       (20)      135 2020-11-10 15:38:18.000000 darts-0.9.0/darts/metrics/__init__.py
--rw-r--r--   0 julien     (501) staff       (20)    42819 2021-07-09 15:18:43.000000 darts-0.9.0/darts/metrics/metrics.py
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.423169 darts-0.9.0/darts/models/
--rw-r--r--   0 julien     (501) staff       (20)     1564 2021-07-09 15:18:43.000000 darts-0.9.0/darts/models/__init__.py
--rw-r--r--   0 julien     (501) staff       (20)     3663 2021-07-09 15:18:43.000000 darts-0.9.0/darts/models/arima.py
--rw-r--r--   0 julien     (501) staff       (20)     2351 2021-07-09 15:18:43.000000 darts-0.9.0/darts/models/auto_arima.py
--rw-r--r--   0 julien     (501) staff       (20)     3982 2021-07-09 15:18:43.000000 darts-0.9.0/darts/models/baselines.py
--rw-r--r--   0 julien     (501) staff       (20)     8009 2021-07-09 15:18:43.000000 darts-0.9.0/darts/models/block_rnn_model.py
--rw-r--r--   0 julien     (501) staff       (20)     2527 2021-07-09 15:18:43.000000 darts-0.9.0/darts/models/ensemble_model.py
--rw-r--r--   0 julien     (501) staff       (20)     3777 2021-07-09 15:18:43.000000 darts-0.9.0/darts/models/exponential_smoothing.py
--rw-r--r--   0 julien     (501) staff       (20)    12858 2021-07-09 15:18:43.000000 darts-0.9.0/darts/models/fft.py
--rw-r--r--   0 julien     (501) staff       (20)     2739 2021-07-09 15:18:43.000000 darts-0.9.0/darts/models/filtering_model.py
--rw-r--r--   0 julien     (501) staff       (20)    40688 2021-07-09 15:18:43.000000 darts-0.9.0/darts/models/forecasting_model.py
--rw-r--r--   0 julien     (501) staff       (20)     2852 2021-07-09 15:18:43.000000 darts-0.9.0/darts/models/gaussian_process_filter.py
--rw-r--r--   0 julien     (501) staff       (20)     7058 2021-07-09 15:18:43.000000 darts-0.9.0/darts/models/kalman_filter.py
--rw-r--r--   0 julien     (501) staff       (20)     1809 2021-05-21 08:07:27.000000 darts-0.9.0/darts/models/linear_regression_model.py
--rw-r--r--   0 julien     (501) staff       (20)    19280 2021-07-09 15:18:43.000000 darts-0.9.0/darts/models/nbeats.py
--rw-r--r--   0 julien     (501) staff       (20)     3390 2021-07-09 15:18:43.000000 darts-0.9.0/darts/models/prophet.py
--rw-r--r--   0 julien     (501) staff       (20)     2691 2021-05-21 08:07:27.000000 darts-0.9.0/darts/models/random_forest.py
--rw-r--r--   0 julien     (501) staff       (20)     3920 2021-06-30 06:58:58.000000 darts-0.9.0/darts/models/regression_ensemble_model.py
--rw-r--r--   0 julien     (501) staff       (20)    13412 2021-07-09 15:18:43.000000 darts-0.9.0/darts/models/regression_model.py
--rw-r--r--   0 julien     (501) staff       (20)     8588 2021-07-09 15:18:43.000000 darts-0.9.0/darts/models/rnn_model.py
--rw-r--r--   0 julien     (501) staff       (20)    12144 2021-07-09 15:18:43.000000 darts-0.9.0/darts/models/tcn_model.py
--rw-r--r--   0 julien     (501) staff       (20)    17126 2021-07-09 15:18:43.000000 darts-0.9.0/darts/models/theta.py
--rw-r--r--   0 julien     (501) staff       (20)    45586 2021-07-09 15:18:43.000000 darts-0.9.0/darts/models/torch_forecasting_model.py
--rw-r--r--   0 julien     (501) staff       (20)    12791 2021-02-02 10:11:33.000000 darts-0.9.0/darts/models/transformer_model.py
--rw-r--r--   0 julien     (501) staff       (20)     3504 2021-07-09 15:18:43.000000 darts-0.9.0/darts/models/varima.py
--rw-r--r--   0 julien     (501) staff       (20)        0 2020-10-07 09:45:20.000000 darts-0.9.0/darts/py.typed
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.436840 darts-0.9.0/darts/tests/
--rw-r--r--   0 julien     (501) staff       (20)        0 2020-08-26 18:23:45.000000 darts-0.9.0/darts/tests/__init__.py
--rw-r--r--   0 julien     (501) staff       (20)      574 2021-02-02 10:11:33.000000 darts-0.9.0/darts/tests/base_test_class.py
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.437606 darts-0.9.0/darts/tests/dataprocessing/
--rw-r--r--   0 julien     (501) staff       (20)        0 2020-11-09 21:16:27.000000 darts-0.9.0/darts/tests/dataprocessing/__init__.py
--rw-r--r--   0 julien     (501) staff       (20)     9919 2021-05-21 08:07:27.000000 darts-0.9.0/darts/tests/dataprocessing/test_pipeline.py
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.477774 darts-0.9.0/darts/tests/dataprocessing/transformers/
--rw-r--r--   0 julien     (501) staff       (20)        0 2020-11-09 21:16:27.000000 darts-0.9.0/darts/tests/dataprocessing/transformers/__init__.py
--rw-r--r--   0 julien     (501) staff       (20)      958 2021-05-21 08:07:27.000000 darts-0.9.0/darts/tests/dataprocessing/transformers/test_base_data_transformer.py
--rw-r--r--   0 julien     (501) staff       (20)     3033 2021-07-09 15:18:43.000000 darts-0.9.0/darts/tests/dataprocessing/transformers/test_boxcox.py
--rw-r--r--   0 julien     (501) staff       (20)     2953 2021-05-21 08:07:27.000000 darts-0.9.0/darts/tests/dataprocessing/transformers/test_data_transformer.py
--rw-r--r--   0 julien     (501) staff       (20)     2710 2021-05-21 08:07:27.000000 darts-0.9.0/darts/tests/dataprocessing/transformers/test_mappers.py
--rw-r--r--   0 julien     (501) staff       (20)     1571 2021-05-21 08:07:27.000000 darts-0.9.0/darts/tests/dataprocessing/transformers/test_missing_values_filler.py
--rw-r--r--   0 julien     (501) staff       (20)     2756 2021-07-09 15:18:43.000000 darts-0.9.0/darts/tests/test_4theta.py
--rw-r--r--   0 julien     (501) staff       (20)     3599 2021-07-09 15:18:43.000000 darts-0.9.0/darts/tests/test_NBEATS.py
--rw-r--r--   0 julien     (501) staff       (20)     6781 2021-06-30 06:58:58.000000 darts-0.9.0/darts/tests/test_TCN.py
--rw-r--r--   0 julien     (501) staff       (20)    12923 2021-07-09 15:18:43.000000 darts-0.9.0/darts/tests/test_backtesting.py
--rw-r--r--   0 julien     (501) staff       (20)     3426 2021-07-09 15:18:43.000000 darts-0.9.0/darts/tests/test_block_RNN.py
--rw-r--r--   0 julien     (501) staff       (20)     2297 2021-07-07 15:04:10.000000 darts-0.9.0/darts/tests/test_dataset_loaders.py
--rw-r--r--   0 julien     (501) staff       (20)     6413 2021-07-09 15:18:43.000000 darts-0.9.0/darts/tests/test_datasets.py
--rw-r--r--   0 julien     (501) staff       (20)     1745 2021-05-21 08:07:27.000000 darts-0.9.0/darts/tests/test_ensemble_models.py
--rw-r--r--   0 julien     (501) staff       (20)     1972 2021-02-02 10:11:33.000000 darts-0.9.0/darts/tests/test_fft.py
--rwxr-xr-x   0 julien     (501) staff       (20)     2614 2021-07-09 15:18:43.000000 darts-0.9.0/darts/tests/test_filters.py
--rw-r--r--   0 julien     (501) staff       (20)    15515 2021-07-09 15:18:43.000000 darts-0.9.0/darts/tests/test_global_forecasting_models.py
--rw-r--r--   0 julien     (501) staff       (20)     6198 2021-07-09 15:18:43.000000 darts-0.9.0/darts/tests/test_local_forecasting_models.py
--rw-r--r--   0 julien     (501) staff       (20)     3258 2021-07-09 15:18:43.000000 darts-0.9.0/darts/tests/test_logging.py
--rw-r--r--   0 julien     (501) staff       (20)    13191 2021-07-09 15:18:43.000000 darts-0.9.0/darts/tests/test_metrics.py
--rw-r--r--   0 julien     (501) staff       (20)     3638 2021-02-02 10:11:33.000000 darts-0.9.0/darts/tests/test_missing_values.py
--rw-r--r--   0 julien     (501) staff       (20)     4065 2021-07-09 15:18:43.000000 darts-0.9.0/darts/tests/test_probabilistic_models.py
--rw-r--r--   0 julien     (501) staff       (20)     3435 2021-07-09 15:18:43.000000 darts-0.9.0/darts/tests/test_regression_ensemble_model.py
--rw-r--r--   0 julien     (501) staff       (20)     9080 2021-07-09 15:18:43.000000 darts-0.9.0/darts/tests/test_regression_models.py
--rw-r--r--   0 julien     (501) staff       (20)      700 2021-02-02 10:11:33.000000 darts-0.9.0/darts/tests/test_statistics.py
--rw-r--r--   0 julien     (501) staff       (20)    30739 2021-07-09 15:18:43.000000 darts-0.9.0/darts/tests/test_timeseries.py
--rw-r--r--   0 julien     (501) staff       (20)     3489 2021-07-09 15:18:43.000000 darts-0.9.0/darts/tests/test_timeseries_generation.py
--rw-r--r--   0 julien     (501) staff       (20)     7810 2021-07-09 15:18:43.000000 darts-0.9.0/darts/tests/test_timeseries_multivariate.py
--rw-r--r--   0 julien     (501) staff       (20)     5667 2021-07-09 15:18:43.000000 darts-0.9.0/darts/tests/test_torch_forecasting_model.py
--rw-r--r--   0 julien     (501) staff       (20)     3447 2021-06-30 06:58:58.000000 darts-0.9.0/darts/tests/test_transformer_model.py
--rw-r--r--   0 julien     (501) staff       (20)     2594 2021-02-02 10:11:33.000000 darts-0.9.0/darts/tests/test_utils.py
--rw-r--r--   0 julien     (501) staff       (20)     4400 2021-02-02 10:11:33.000000 darts-0.9.0/darts/tests/test_utils_torch.py
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.478548 darts-0.9.0/darts/tests/utils/
--rw-r--r--   0 julien     (501) staff       (20)        0 2021-07-07 15:04:10.000000 darts-0.9.0/darts/tests/utils/__init__.py
--rw-r--r--   0 julien     (501) staff       (20)     9799 2021-07-07 15:04:10.000000 darts-0.9.0/darts/tests/utils/test_model_selection.py
--rw-r--r--   0 julien     (501) staff       (20)    85040 2021-07-09 15:18:43.000000 darts-0.9.0/darts/timeseries.py
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.482624 darts-0.9.0/darts/utils/
--rw-r--r--   0 julien     (501) staff       (20)      165 2021-05-21 08:07:27.000000 darts-0.9.0/darts/utils/__init__.py
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.486078 darts-0.9.0/darts/utils/data/
--rw-r--r--   0 julien     (501) staff       (20)      335 2021-02-02 10:11:33.000000 darts-0.9.0/darts/utils/data/__init__.py
--rw-r--r--   0 julien     (501) staff       (20)     6983 2021-02-02 10:11:33.000000 darts-0.9.0/darts/utils/data/horizon_based_dataset.py
--rw-r--r--   0 julien     (501) staff       (20)     6241 2021-02-02 10:11:33.000000 darts-0.9.0/darts/utils/data/sequential_dataset.py
--rw-r--r--   0 julien     (501) staff       (20)     7392 2021-07-09 15:18:43.000000 darts-0.9.0/darts/utils/data/shifted_dataset.py
--rw-r--r--   0 julien     (501) staff       (20)     6888 2021-07-09 15:18:43.000000 darts-0.9.0/darts/utils/data/simple_inference_dataset.py
--rw-r--r--   0 julien     (501) staff       (20)     2467 2021-07-09 15:18:43.000000 darts-0.9.0/darts/utils/data/timeseries_dataset.py
--rw-r--r--   0 julien     (501) staff       (20)     3265 2021-07-09 15:18:43.000000 darts-0.9.0/darts/utils/likelihood_models.py
--rw-r--r--   0 julien     (501) staff       (20)     4754 2021-07-09 15:18:43.000000 darts-0.9.0/darts/utils/missing_values.py
--rw-r--r--   0 julien     (501) staff       (20)    10186 2021-07-09 15:18:43.000000 darts-0.9.0/darts/utils/model_selection.py
--rw-r--r--   0 julien     (501) staff       (20)    11627 2021-07-09 15:18:43.000000 darts-0.9.0/darts/utils/statistics.py
--rw-r--r--   0 julien     (501) staff       (20)    11159 2021-07-09 15:18:43.000000 darts-0.9.0/darts/utils/timeseries_generation.py
--rw-r--r--   0 julien     (501) staff       (20)     2032 2021-07-09 15:18:43.000000 darts-0.9.0/darts/utils/torch.py
--rw-r--r--   0 julien     (501) staff       (20)     8666 2021-07-09 15:18:43.000000 darts-0.9.0/darts/utils/utils.py
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.375226 darts-0.9.0/darts.egg-info/
--rw-r--r--   0 julien     (501) staff       (20)    10596 2021-07-09 15:44:37.000000 darts-0.9.0/darts.egg-info/PKG-INFO
--rw-r--r--   0 julien     (501) staff       (20)     5901 2021-07-09 15:44:37.000000 darts-0.9.0/darts.egg-info/SOURCES.txt
--rw-r--r--   0 julien     (501) staff       (20)        1 2021-07-09 15:44:37.000000 darts-0.9.0/darts.egg-info/dependency_links.txt
--rw-r--r--   0 julien     (501) staff       (20)        1 2021-03-25 09:43:07.000000 darts-0.9.0/darts.egg-info/not-zip-safe
--rw-r--r--   0 julien     (501) staff       (20)      290 2021-07-09 15:44:37.000000 darts-0.9.0/darts.egg-info/requires.txt
--rw-r--r--   0 julien     (501) staff       (20)        6 2021-07-09 15:44:37.000000 darts-0.9.0/darts.egg-info/top_level.txt
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.512846 darts-0.9.0/datasets/
--rw-r--r--   0 julien     (501) staff       (20)     1746 2021-07-07 15:04:10.000000 darts-0.9.0/datasets/AirPassengers.csv
--rw-r--r--   0 julien     (501) staff       (20)     3176 2021-07-07 15:04:10.000000 darts-0.9.0/datasets/ausbeer.csv
--rw-r--r--   0 julien     (501) staff       (20)  6062625 2021-07-07 15:04:10.000000 darts-0.9.0/datasets/energy_dataset.csv
--rw-r--r--   0 julien     (501) staff       (20)     3382 2021-07-07 15:04:10.000000 darts-0.9.0/datasets/gasrate_co2.csv
--rw-r--r--   0 julien     (501) staff       (20)    15976 2021-07-07 15:04:10.000000 darts-0.9.0/datasets/heart_rate.csv
--rw-r--r--   0 julien     (501) staff       (20)     2993 2021-07-07 15:04:10.000000 darts-0.9.0/datasets/ice_cream_heater.csv
--rw-r--r--   0 julien     (501) staff       (20)     2196 2021-07-07 15:04:10.000000 darts-0.9.0/datasets/monthly-milk-incomplete.csv
--rw-r--r--   0 julien     (501) staff       (20)     2378 2021-07-07 15:04:10.000000 darts-0.9.0/datasets/monthly-milk.csv
--rw-r--r--   0 julien     (501) staff       (20)    42219 2021-07-07 15:04:10.000000 darts-0.9.0/datasets/monthly-sunspots.csv
--rw-r--r--   0 julien     (501) staff       (20)    24196 2021-07-07 15:04:10.000000 darts-0.9.0/datasets/taylor.csv
--rw-r--r--   0 julien     (501) staff       (20)    55847 2021-07-07 15:04:10.000000 darts-0.9.0/datasets/temps.csv
--rw-r--r--   0 julien     (501) staff       (20)    26373 2021-07-07 15:04:10.000000 darts-0.9.0/datasets/us_gasoline.csv
--rw-r--r--   0 julien     (501) staff       (20)     3003 2021-07-07 15:04:10.000000 darts-0.9.0/datasets/wineind.csv
--rw-r--r--   0 julien     (501) staff       (20)     1915 2021-07-07 15:04:10.000000 darts-0.9.0/datasets/woolyrnq.csv
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.513517 darts-0.9.0/docs/
--rw-r--r--   0 julien     (501) staff       (20)     1008 2021-02-02 10:11:33.000000 darts-0.9.0/docs/Makefile
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.515292 darts-0.9.0/docs/source/
--rw-r--r--   0 julien     (501) staff       (20)     3177 2021-07-09 15:44:02.000000 darts-0.9.0/docs/source/conf.py
--rw-r--r--   0 julien     (501) staff       (20)     1904 2021-02-03 09:29:17.000000 darts-0.9.0/docs/source/examples.rst
--rw-r--r--   0 julien     (501) staff       (20)      276 2021-01-31 13:26:04.000000 darts-0.9.0/docs/source/index.rst
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.516344 darts-0.9.0/docs/source/static/
--rw-r--r--   0 julien     (501) staff       (20)        0 2020-08-26 18:23:45.000000 darts-0.9.0/docs/source/static/.gitkeep
--rw-r--r--   0 julien     (501) staff       (20)    84068 2020-08-26 18:23:45.000000 darts-0.9.0/docs/source/static/darts-logo-trim.png
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.518703 darts-0.9.0/docs/templates/
--rw-r--r--   0 julien     (501) staff       (20)      103 2021-01-31 13:23:05.000000 darts-0.9.0/docs/templates/module.rst_t
--rw-r--r--   0 julien     (501) staff       (20)      582 2021-01-31 13:27:59.000000 darts-0.9.0/docs/templates/package.rst_t
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.557494 darts-0.9.0/examples/
--rw-r--r--   0 julien     (501) staff       (20)   642786 2021-07-09 15:18:43.000000 darts-0.9.0/examples/01-darts-intro.ipynb
--rw-r--r--   0 julien     (501) staff       (20)   311945 2021-07-09 15:18:43.000000 darts-0.9.0/examples/02-multi-time-series-and-covariates.ipynb
--rw-r--r--   0 julien     (501) staff       (20)   390534 2021-07-09 15:18:43.000000 darts-0.9.0/examples/03-data-processing.ipynb
--rw-r--r--   0 julien     (501) staff       (20)   221195 2021-07-07 15:04:10.000000 darts-0.9.0/examples/04-FFT-examples.ipynb
--rw-r--r--   0 julien     (501) staff       (20)   211992 2021-07-09 15:18:43.000000 darts-0.9.0/examples/05-RNN-examples.ipynb
--rw-r--r--   0 julien     (501) staff       (20)   200249 2021-07-09 15:18:43.000000 darts-0.9.0/examples/06-TCN-examples.ipynb
--rw-r--r--   0 julien     (501) staff       (20)   198701 2021-07-07 15:04:10.000000 darts-0.9.0/examples/07-Transformer-examples.ipynb
--rw-r--r--   0 julien     (501) staff       (20)   240623 2021-07-07 15:04:10.000000 darts-0.9.0/examples/08-NBEATS-examples.ipynb
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.567665 darts-0.9.0/examples/M4_competition/
--rw-r--r--   0 julien     (501) staff       (20)    33825 2021-07-09 15:18:43.000000 darts-0.9.0/examples/M4_competition/M4_competition_benchmark.ipynb
--rw-r--r--   0 julien     (501) staff       (20)     1553 2020-10-07 09:45:20.000000 darts-0.9.0/examples/M4_competition/M4_metrics.py
--rw-r--r--   0 julien     (501) staff       (20)     2632 2020-12-21 14:57:41.000000 darts-0.9.0/examples/M4_competition/create_ts.py
--rw-r--r--   0 julien     (501) staff       (20)     1180 2020-10-07 09:45:20.000000 darts-0.9.0/examples/M4_competition/download_data_M4.py
--rw-r--r--   0 julien     (501) staff       (20)     2649 2020-11-08 13:54:23.000000 darts-0.9.0/examples/M4_competition/evaluate_arima.py
--rw-r--r--   0 julien     (501) staff       (20)     4883 2021-07-09 15:18:43.000000 darts-0.9.0/examples/M4_competition/evaluate_baselines.py
--rw-r--r--   0 julien     (501) staff       (20)    11417 2021-07-09 15:18:43.000000 darts-0.9.0/examples/M4_competition/evaluate_ensembling.py
--rw-r--r--   0 julien     (501) staff       (20)     3272 2021-02-02 10:11:33.000000 darts-0.9.0/examples/M4_competition/evaluate_fft.py
--rw-r--r--   0 julien     (501) staff       (20)    11717 2021-07-09 15:18:43.000000 darts-0.9.0/examples/M4_competition/evaluate_groe_R.py
--rw-r--r--   0 julien     (501) staff       (20)     5493 2021-07-09 15:18:43.000000 darts-0.9.0/examples/M4_competition/evaluate_naive2_with_R.py
--rw-r--r--   0 julien     (501) staff       (20)     3551 2021-07-09 15:18:43.000000 darts-0.9.0/examples/M4_competition/evaluate_prophet.py
--rw-r--r--   0 julien     (501) staff       (20)     4682 2021-07-09 15:18:43.000000 darts-0.9.0/examples/M4_competition/evaluate_theta_methods.py
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.320577 darts-0.9.0/examples/static/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.572368 darts-0.9.0/examples/static/images/
--rw-r--r--   0 julien     (501) staff       (20)    53317 2021-02-02 10:11:33.000000 darts-0.9.0/examples/static/images/global_io.png
--rw-r--r--   0 julien     (501) staff       (20)    66469 2021-02-02 10:11:33.000000 darts-0.9.0/examples/static/images/global_io_covs.png
--rw-r--r--   0 julien     (501) staff       (20)    85947 2021-02-02 10:11:33.000000 darts-0.9.0/examples/static/images/seq_dataset_multi_ts.png
--rw-r--r--   0 julien     (501) staff       (20)    42967 2021-02-02 10:11:33.000000 darts-0.9.0/examples/static/images/seq_dataset_one_ts.png
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.574246 darts-0.9.0/examples/utils/
--rw-r--r--   0 julien     (501) staff       (20)       52 2020-10-07 09:45:20.000000 darts-0.9.0/examples/utils/__init__.py
--rw-r--r--   0 julien     (501) staff       (20)      333 2020-10-07 09:45:20.000000 darts-0.9.0/examples/utils/utils.py
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.321053 darts-0.9.0/gradle/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.576281 darts-0.9.0/gradle/wrapper/
--rw-r--r--   0 julien     (501) staff       (20)    58695 2020-10-07 09:45:20.000000 darts-0.9.0/gradle/wrapper/gradle-wrapper.jar
--rw-r--r--   0 julien     (501) staff       (20)      200 2020-10-07 09:45:20.000000 darts-0.9.0/gradle/wrapper/gradle-wrapper.properties
--rwxr-xr-x   0 julien     (501) staff       (20)     5764 2020-10-07 09:45:20.000000 darts-0.9.0/gradlew
--rw-r--r--   0 julien     (501) staff       (20)     3056 2020-10-07 09:45:20.000000 darts-0.9.0/gradlew.bat
--rwxr-xr-x   0 julien     (501) staff       (20)      232 2021-04-26 18:51:16.000000 darts-0.9.0/make_dists.sh
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.580189 darts-0.9.0/requirements/
--rw-r--r--   0 julien     (501) staff       (20)      208 2021-07-09 15:18:43.000000 darts-0.9.0/requirements/core.txt
--rw-r--r--   0 julien     (501) staff       (20)       83 2020-11-09 21:16:27.000000 darts-0.9.0/requirements/dev-all.txt
--rw-r--r--   0 julien     (501) staff       (20)       67 2021-04-19 19:17:01.000000 darts-0.9.0/requirements/dev.txt
--rw-r--r--   0 julien     (501) staff       (20)       33 2021-04-14 10:48:20.000000 darts-0.9.0/requirements/fbprophet.txt
--rw-r--r--   0 julien     (501) staff       (20)       15 2021-04-19 19:17:01.000000 darts-0.9.0/requirements/pmdarima.txt
--rw-r--r--   0 julien     (501) staff       (20)      381 2021-05-21 08:07:27.000000 darts-0.9.0/requirements/release.txt
--rw-r--r--   0 julien     (501) staff       (20)       32 2021-04-19 19:17:01.000000 darts-0.9.0/requirements/torch.txt
--rw-r--r--   0 julien     (501) staff       (20)       27 2020-10-07 09:45:20.000000 darts-0.9.0/settings.gradle
--rw-r--r--   0 julien     (501) staff       (20)      145 2021-07-09 15:44:37.617242 darts-0.9.0/setup.cfg
--rw-r--r--   0 julien     (501) staff       (20)     2098 2021-07-09 15:44:02.000000 darts-0.9.0/setup.py
--rw-r--r--   0 julien     (501) staff       (20)     2275 2021-07-09 15:18:43.000000 darts-0.9.0/setup_u8darts.py
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.321418 darts-0.9.0/static/
-drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-09 15:44:37.615974 darts-0.9.0/static/images/
--rw-r--r--   0 julien     (501) staff       (20)    84068 2020-08-26 18:23:45.000000 darts-0.9.0/static/images/darts-logo-trim.png
--rw-r--r--   0 julien     (501) staff       (20)    57635 2021-07-09 15:18:43.000000 darts-0.9.0/static/images/example.png
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.443031 darts-0.9.1/
+-rw-r--r--   0 julien     (501) staff       (20)      253 2021-07-17 13:19:40.000000 darts-0.9.1/.bumpversion.cfg
+-rw-r--r--   0 julien     (501) staff       (20)       48 2020-08-26 18:23:45.000000 darts-0.9.1/.dockerignore
+-rw-r--r--   0 julien     (501) staff       (20)      154 2020-10-07 09:45:20.000000 darts-0.9.1/.gitattributes
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.204559 darts-0.9.1/.github/
+-rw-r--r--   0 julien     (501) staff       (20)      530 2020-10-07 09:45:20.000000 darts-0.9.1/.github/CODEOWNERS
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.205953 darts-0.9.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 julien     (501) staff       (20)      544 2020-08-26 18:23:59.000000 darts-0.9.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 julien     (501) staff       (20)      624 2020-08-26 18:23:59.000000 darts-0.9.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 julien     (501) staff       (20)      497 2020-08-26 18:23:59.000000 darts-0.9.1/.github/pull_request_template.md
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.206925 darts-0.9.1/.github/workflows/
+-rw-r--r--   0 julien     (501) staff       (20)     3931 2021-07-17 12:56:13.000000 darts-0.9.1/.github/workflows/develop.yml
+-rw-r--r--   0 julien     (501) staff       (20)     4055 2021-07-17 12:56:13.000000 darts-0.9.1/.github/workflows/merge.yml
+-rw-r--r--   0 julien     (501) staff       (20)     5589 2021-07-17 12:56:13.000000 darts-0.9.1/.github/workflows/release.yml
+-rw-r--r--   0 julien     (501) staff       (20)      314 2021-07-17 12:56:13.000000 darts-0.9.1/.gitignore
+-rw-r--r--   0 julien     (501) staff       (20)    21593 2021-07-17 12:56:13.000000 darts-0.9.1/CHANGELOG.md
+-rw-r--r--   0 julien     (501) staff       (20)     2463 2021-05-21 08:07:27.000000 darts-0.9.1/CONTRIBUTE.md
+-rw-r--r--   0 julien     (501) staff       (20)      694 2021-02-03 09:29:17.000000 darts-0.9.1/Dockerfile
+-rw-r--r--   0 julien     (501) staff       (20)    11338 2020-08-26 18:23:45.000000 darts-0.9.1/LICENSE
+-rw-r--r--   0 julien     (501) staff       (20)       19 2021-07-17 12:56:13.000000 darts-0.9.1/MANIFEST.in
+-rw-r--r--   0 julien     (501) staff       (20)    10561 2021-07-17 13:20:17.443236 darts-0.9.1/PKG-INFO
+-rw-r--r--   0 julien     (501) staff       (20)     9324 2021-07-17 12:56:13.000000 darts-0.9.1/README.md
+-rw-r--r--   0 julien     (501) staff       (20)     4679 2021-07-17 12:56:13.000000 darts-0.9.1/build.gradle
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.207156 darts-0.9.1/conda_recipe/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.208065 darts-0.9.1/conda_recipe/darts/
+-rw-r--r--   0 julien     (501) staff       (20)      699 2021-07-17 13:19:40.000000 darts-0.9.1/conda_recipe/darts/meta.yaml
+-rw-r--r--   0 julien     (501) staff       (20)      133 2021-04-19 19:17:01.000000 darts-0.9.1/conda_recipe/environment.yml
+-rwxr-xr-x   0 julien     (501) staff       (20)      556 2020-10-07 09:45:20.000000 darts-0.9.1/coverage.sh
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.209375 darts-0.9.1/darts/
+-rw-r--r--   0 julien     (501) staff       (20)      902 2021-07-17 13:19:40.000000 darts-0.9.1/darts/__init__.py
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.233263 darts-0.9.1/darts/dataprocessing/
+-rw-r--r--   0 julien     (501) staff       (20)       72 2020-11-09 21:16:27.000000 darts-0.9.1/darts/dataprocessing/__init__.py
+-rw-r--r--   0 julien     (501) staff       (20)     8437 2021-05-21 08:07:27.000000 darts-0.9.1/darts/dataprocessing/pipeline.py
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.240032 darts-0.9.1/darts/dataprocessing/transformers/
+-rw-r--r--   0 julien     (501) staff       (20)      385 2020-11-09 21:16:27.000000 darts-0.9.1/darts/dataprocessing/transformers/__init__.py
+-rw-r--r--   0 julien     (501) staff       (20)     7470 2021-05-21 08:07:27.000000 darts-0.9.1/darts/dataprocessing/transformers/base_data_transformer.py
+-rw-r--r--   0 julien     (501) staff       (20)     5916 2021-07-09 15:18:43.000000 darts-0.9.1/darts/dataprocessing/transformers/boxcox.py
+-rw-r--r--   0 julien     (501) staff       (20)     7896 2021-05-21 08:07:27.000000 darts-0.9.1/darts/dataprocessing/transformers/fittable_data_transformer.py
+-rw-r--r--   0 julien     (501) staff       (20)     6919 2021-05-21 08:07:27.000000 darts-0.9.1/darts/dataprocessing/transformers/invertible_data_transformer.py
+-rw-r--r--   0 julien     (501) staff       (20)     5113 2021-05-21 08:07:27.000000 darts-0.9.1/darts/dataprocessing/transformers/mappers.py
+-rw-r--r--   0 julien     (501) staff       (20)     2401 2021-05-21 08:07:27.000000 darts-0.9.1/darts/dataprocessing/transformers/missing_values_filler.py
+-rw-r--r--   0 julien     (501) staff       (20)     4557 2021-07-09 15:18:43.000000 darts-0.9.1/darts/dataprocessing/transformers/scaler.py
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.241283 darts-0.9.1/darts/datasets/
+-rw-r--r--   0 julien     (501) staff       (20)     7822 2021-07-17 12:56:13.000000 darts-0.9.1/darts/datasets/__init__.py
+-rw-r--r--   0 julien     (501) staff       (20)     5097 2021-07-17 12:56:13.000000 darts-0.9.1/darts/datasets/dataset_loaders.py
+-rw-r--r--   0 julien     (501) staff       (20)     5861 2020-08-26 18:23:45.000000 darts-0.9.1/darts/logging.py
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.242850 darts-0.9.1/darts/metrics/
+-rw-r--r--   0 julien     (501) staff       (20)      135 2020-11-10 15:38:18.000000 darts-0.9.1/darts/metrics/__init__.py
+-rw-r--r--   0 julien     (501) staff       (20)    42819 2021-07-09 15:18:43.000000 darts-0.9.1/darts/metrics/metrics.py
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.261366 darts-0.9.1/darts/models/
+-rw-r--r--   0 julien     (501) staff       (20)     1562 2021-07-17 12:56:13.000000 darts-0.9.1/darts/models/__init__.py
+-rw-r--r--   0 julien     (501) staff       (20)     3663 2021-07-09 15:18:43.000000 darts-0.9.1/darts/models/arima.py
+-rw-r--r--   0 julien     (501) staff       (20)     2351 2021-07-09 15:18:43.000000 darts-0.9.1/darts/models/auto_arima.py
+-rw-r--r--   0 julien     (501) staff       (20)     3982 2021-07-09 15:18:43.000000 darts-0.9.1/darts/models/baselines.py
+-rw-r--r--   0 julien     (501) staff       (20)     8021 2021-07-17 12:56:13.000000 darts-0.9.1/darts/models/block_rnn_model.py
+-rw-r--r--   0 julien     (501) staff       (20)     2527 2021-07-09 15:18:43.000000 darts-0.9.1/darts/models/ensemble_model.py
+-rw-r--r--   0 julien     (501) staff       (20)     3777 2021-07-09 15:18:43.000000 darts-0.9.1/darts/models/exponential_smoothing.py
+-rw-r--r--   0 julien     (501) staff       (20)    12858 2021-07-09 15:18:43.000000 darts-0.9.1/darts/models/fft.py
+-rw-r--r--   0 julien     (501) staff       (20)     2739 2021-07-09 15:18:43.000000 darts-0.9.1/darts/models/filtering_model.py
+-rw-r--r--   0 julien     (501) staff       (20)    41071 2021-07-17 12:56:13.000000 darts-0.9.1/darts/models/forecasting_model.py
+-rw-r--r--   0 julien     (501) staff       (20)     3087 2021-07-17 12:56:13.000000 darts-0.9.1/darts/models/gaussian_process_filter.py
+-rw-r--r--   0 julien     (501) staff       (20)     7058 2021-07-09 15:18:43.000000 darts-0.9.1/darts/models/kalman_filter.py
+-rw-r--r--   0 julien     (501) staff       (20)     1809 2021-05-21 08:07:27.000000 darts-0.9.1/darts/models/linear_regression_model.py
+-rw-r--r--   0 julien     (501) staff       (20)    19280 2021-07-09 15:18:43.000000 darts-0.9.1/darts/models/nbeats.py
+-rw-r--r--   0 julien     (501) staff       (20)     3384 2021-07-17 12:56:13.000000 darts-0.9.1/darts/models/prophet.py
+-rw-r--r--   0 julien     (501) staff       (20)     2691 2021-05-21 08:07:27.000000 darts-0.9.1/darts/models/random_forest.py
+-rw-r--r--   0 julien     (501) staff       (20)     3920 2021-06-30 06:58:58.000000 darts-0.9.1/darts/models/regression_ensemble_model.py
+-rw-r--r--   0 julien     (501) staff       (20)    13412 2021-07-09 15:18:43.000000 darts-0.9.1/darts/models/regression_model.py
+-rw-r--r--   0 julien     (501) staff       (20)     8588 2021-07-09 15:18:43.000000 darts-0.9.1/darts/models/rnn_model.py
+-rw-r--r--   0 julien     (501) staff       (20)    12144 2021-07-09 15:18:43.000000 darts-0.9.1/darts/models/tcn_model.py
+-rw-r--r--   0 julien     (501) staff       (20)    17126 2021-07-09 15:18:43.000000 darts-0.9.1/darts/models/theta.py
+-rw-r--r--   0 julien     (501) staff       (20)    45602 2021-07-17 12:56:13.000000 darts-0.9.1/darts/models/torch_forecasting_model.py
+-rw-r--r--   0 julien     (501) staff       (20)    12791 2021-02-02 10:11:33.000000 darts-0.9.1/darts/models/transformer_model.py
+-rw-r--r--   0 julien     (501) staff       (20)     3504 2021-07-09 15:18:43.000000 darts-0.9.1/darts/models/varima.py
+-rw-r--r--   0 julien     (501) staff       (20)        0 2020-10-07 09:45:20.000000 darts-0.9.1/darts/py.typed
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.306434 darts-0.9.1/darts/tests/
+-rw-r--r--   0 julien     (501) staff       (20)        0 2020-08-26 18:23:45.000000 darts-0.9.1/darts/tests/__init__.py
+-rw-r--r--   0 julien     (501) staff       (20)      574 2021-02-02 10:11:33.000000 darts-0.9.1/darts/tests/base_test_class.py
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.307724 darts-0.9.1/darts/tests/dataprocessing/
+-rw-r--r--   0 julien     (501) staff       (20)        0 2020-11-09 21:16:27.000000 darts-0.9.1/darts/tests/dataprocessing/__init__.py
+-rw-r--r--   0 julien     (501) staff       (20)     9919 2021-05-21 08:07:27.000000 darts-0.9.1/darts/tests/dataprocessing/test_pipeline.py
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.312077 darts-0.9.1/darts/tests/dataprocessing/transformers/
+-rw-r--r--   0 julien     (501) staff       (20)        0 2020-11-09 21:16:27.000000 darts-0.9.1/darts/tests/dataprocessing/transformers/__init__.py
+-rw-r--r--   0 julien     (501) staff       (20)      958 2021-05-21 08:07:27.000000 darts-0.9.1/darts/tests/dataprocessing/transformers/test_base_data_transformer.py
+-rw-r--r--   0 julien     (501) staff       (20)     3033 2021-07-09 15:18:43.000000 darts-0.9.1/darts/tests/dataprocessing/transformers/test_boxcox.py
+-rw-r--r--   0 julien     (501) staff       (20)     2953 2021-05-21 08:07:27.000000 darts-0.9.1/darts/tests/dataprocessing/transformers/test_data_transformer.py
+-rw-r--r--   0 julien     (501) staff       (20)     2710 2021-05-21 08:07:27.000000 darts-0.9.1/darts/tests/dataprocessing/transformers/test_mappers.py
+-rw-r--r--   0 julien     (501) staff       (20)     1571 2021-05-21 08:07:27.000000 darts-0.9.1/darts/tests/dataprocessing/transformers/test_missing_values_filler.py
+-rw-r--r--   0 julien     (501) staff       (20)     2756 2021-07-09 15:18:43.000000 darts-0.9.1/darts/tests/test_4theta.py
+-rw-r--r--   0 julien     (501) staff       (20)     3599 2021-07-09 15:18:43.000000 darts-0.9.1/darts/tests/test_NBEATS.py
+-rw-r--r--   0 julien     (501) staff       (20)     6781 2021-06-30 06:58:58.000000 darts-0.9.1/darts/tests/test_TCN.py
+-rw-r--r--   0 julien     (501) staff       (20)    13436 2021-07-17 12:56:13.000000 darts-0.9.1/darts/tests/test_backtesting.py
+-rw-r--r--   0 julien     (501) staff       (20)     3426 2021-07-09 15:18:43.000000 darts-0.9.1/darts/tests/test_block_RNN.py
+-rw-r--r--   0 julien     (501) staff       (20)     2297 2021-07-16 11:32:33.000000 darts-0.9.1/darts/tests/test_dataset_loaders.py
+-rw-r--r--   0 julien     (501) staff       (20)     6413 2021-07-09 15:18:43.000000 darts-0.9.1/darts/tests/test_datasets.py
+-rw-r--r--   0 julien     (501) staff       (20)     1745 2021-05-21 08:07:27.000000 darts-0.9.1/darts/tests/test_ensemble_models.py
+-rw-r--r--   0 julien     (501) staff       (20)     1972 2021-02-02 10:11:33.000000 darts-0.9.1/darts/tests/test_fft.py
+-rwxr-xr-x   0 julien     (501) staff       (20)     4773 2021-07-17 12:56:13.000000 darts-0.9.1/darts/tests/test_filters.py
+-rw-r--r--   0 julien     (501) staff       (20)    15515 2021-07-09 15:18:43.000000 darts-0.9.1/darts/tests/test_global_forecasting_models.py
+-rw-r--r--   0 julien     (501) staff       (20)     6198 2021-07-09 15:18:43.000000 darts-0.9.1/darts/tests/test_local_forecasting_models.py
+-rw-r--r--   0 julien     (501) staff       (20)     3258 2021-07-09 15:18:43.000000 darts-0.9.1/darts/tests/test_logging.py
+-rw-r--r--   0 julien     (501) staff       (20)    13191 2021-07-09 15:18:43.000000 darts-0.9.1/darts/tests/test_metrics.py
+-rw-r--r--   0 julien     (501) staff       (20)     3638 2021-02-02 10:11:33.000000 darts-0.9.1/darts/tests/test_missing_values.py
+-rw-r--r--   0 julien     (501) staff       (20)     4065 2021-07-09 15:18:43.000000 darts-0.9.1/darts/tests/test_probabilistic_models.py
+-rw-r--r--   0 julien     (501) staff       (20)     3435 2021-07-09 15:18:43.000000 darts-0.9.1/darts/tests/test_regression_ensemble_model.py
+-rw-r--r--   0 julien     (501) staff       (20)     9080 2021-07-09 15:18:43.000000 darts-0.9.1/darts/tests/test_regression_models.py
+-rw-r--r--   0 julien     (501) staff       (20)      700 2021-02-02 10:11:33.000000 darts-0.9.1/darts/tests/test_statistics.py
+-rw-r--r--   0 julien     (501) staff       (20)    31771 2021-07-17 12:56:13.000000 darts-0.9.1/darts/tests/test_timeseries.py
+-rw-r--r--   0 julien     (501) staff       (20)     3489 2021-07-09 15:18:43.000000 darts-0.9.1/darts/tests/test_timeseries_generation.py
+-rw-r--r--   0 julien     (501) staff       (20)     7810 2021-07-09 15:18:43.000000 darts-0.9.1/darts/tests/test_timeseries_multivariate.py
+-rw-r--r--   0 julien     (501) staff       (20)     5667 2021-07-09 15:18:43.000000 darts-0.9.1/darts/tests/test_torch_forecasting_model.py
+-rw-r--r--   0 julien     (501) staff       (20)     3447 2021-06-30 06:58:58.000000 darts-0.9.1/darts/tests/test_transformer_model.py
+-rw-r--r--   0 julien     (501) staff       (20)     2594 2021-02-02 10:11:33.000000 darts-0.9.1/darts/tests/test_utils.py
+-rw-r--r--   0 julien     (501) staff       (20)     4400 2021-02-02 10:11:33.000000 darts-0.9.1/darts/tests/test_utils_torch.py
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.313133 darts-0.9.1/darts/tests/utils/
+-rw-r--r--   0 julien     (501) staff       (20)        0 2021-07-07 15:04:10.000000 darts-0.9.1/darts/tests/utils/__init__.py
+-rw-r--r--   0 julien     (501) staff       (20)     9799 2021-07-07 15:04:10.000000 darts-0.9.1/darts/tests/utils/test_model_selection.py
+-rw-r--r--   0 julien     (501) staff       (20)    88381 2021-07-17 12:56:13.000000 darts-0.9.1/darts/timeseries.py
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.319635 darts-0.9.1/darts/utils/
+-rw-r--r--   0 julien     (501) staff       (20)      165 2021-05-21 08:07:27.000000 darts-0.9.1/darts/utils/__init__.py
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.323704 darts-0.9.1/darts/utils/data/
+-rw-r--r--   0 julien     (501) staff       (20)      335 2021-02-02 10:11:33.000000 darts-0.9.1/darts/utils/data/__init__.py
+-rw-r--r--   0 julien     (501) staff       (20)     6983 2021-02-02 10:11:33.000000 darts-0.9.1/darts/utils/data/horizon_based_dataset.py
+-rw-r--r--   0 julien     (501) staff       (20)     6241 2021-02-02 10:11:33.000000 darts-0.9.1/darts/utils/data/sequential_dataset.py
+-rw-r--r--   0 julien     (501) staff       (20)     7392 2021-07-09 15:18:43.000000 darts-0.9.1/darts/utils/data/shifted_dataset.py
+-rw-r--r--   0 julien     (501) staff       (20)     6888 2021-07-09 15:18:43.000000 darts-0.9.1/darts/utils/data/simple_inference_dataset.py
+-rw-r--r--   0 julien     (501) staff       (20)     2467 2021-07-09 15:18:43.000000 darts-0.9.1/darts/utils/data/timeseries_dataset.py
+-rw-r--r--   0 julien     (501) staff       (20)     3265 2021-07-09 15:18:43.000000 darts-0.9.1/darts/utils/likelihood_models.py
+-rw-r--r--   0 julien     (501) staff       (20)     4754 2021-07-09 15:18:43.000000 darts-0.9.1/darts/utils/missing_values.py
+-rw-r--r--   0 julien     (501) staff       (20)    10186 2021-07-09 15:18:43.000000 darts-0.9.1/darts/utils/model_selection.py
+-rw-r--r--   0 julien     (501) staff       (20)    11627 2021-07-09 15:18:43.000000 darts-0.9.1/darts/utils/statistics.py
+-rw-r--r--   0 julien     (501) staff       (20)    11159 2021-07-09 15:18:43.000000 darts-0.9.1/darts/utils/timeseries_generation.py
+-rw-r--r--   0 julien     (501) staff       (20)     2032 2021-07-09 15:18:43.000000 darts-0.9.1/darts/utils/torch.py
+-rw-r--r--   0 julien     (501) staff       (20)     8697 2021-07-17 12:56:13.000000 darts-0.9.1/darts/utils/utils.py
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.231811 darts-0.9.1/darts.egg-info/
+-rw-r--r--   0 julien     (501) staff       (20)    10561 2021-07-17 13:20:17.000000 darts-0.9.1/darts.egg-info/PKG-INFO
+-rw-r--r--   0 julien     (501) staff       (20)     6024 2021-07-17 13:20:17.000000 darts-0.9.1/darts.egg-info/SOURCES.txt
+-rw-r--r--   0 julien     (501) staff       (20)        1 2021-07-17 13:20:17.000000 darts-0.9.1/darts.egg-info/dependency_links.txt
+-rw-r--r--   0 julien     (501) staff       (20)        1 2021-03-25 09:43:07.000000 darts-0.9.1/darts.egg-info/not-zip-safe
+-rw-r--r--   0 julien     (501) staff       (20)      311 2021-07-17 13:20:17.000000 darts-0.9.1/darts.egg-info/requires.txt
+-rw-r--r--   0 julien     (501) staff       (20)        6 2021-07-17 13:20:17.000000 darts-0.9.1/darts.egg-info/top_level.txt
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.351994 darts-0.9.1/datasets/
+-rw-r--r--   0 julien     (501) staff       (20)     1746 2021-07-07 15:04:10.000000 darts-0.9.1/datasets/AirPassengers.csv
+-rw-r--r--   0 julien     (501) staff       (20)     3176 2021-07-07 15:04:10.000000 darts-0.9.1/datasets/ausbeer.csv
+-rw-r--r--   0 julien     (501) staff       (20)  6062625 2021-07-07 15:04:10.000000 darts-0.9.1/datasets/energy_dataset.csv
+-rw-r--r--   0 julien     (501) staff       (20)     3382 2021-07-07 15:04:10.000000 darts-0.9.1/datasets/gasrate_co2.csv
+-rw-r--r--   0 julien     (501) staff       (20)    15976 2021-07-07 15:04:10.000000 darts-0.9.1/datasets/heart_rate.csv
+-rw-r--r--   0 julien     (501) staff       (20)     2993 2021-07-07 15:04:10.000000 darts-0.9.1/datasets/ice_cream_heater.csv
+-rw-r--r--   0 julien     (501) staff       (20)     2196 2021-07-07 15:04:10.000000 darts-0.9.1/datasets/monthly-milk-incomplete.csv
+-rw-r--r--   0 julien     (501) staff       (20)     2378 2021-07-07 15:04:10.000000 darts-0.9.1/datasets/monthly-milk.csv
+-rw-r--r--   0 julien     (501) staff       (20)    42219 2021-07-07 15:04:10.000000 darts-0.9.1/datasets/monthly-sunspots.csv
+-rw-r--r--   0 julien     (501) staff       (20)    24196 2021-07-07 15:04:10.000000 darts-0.9.1/datasets/taylor.csv
+-rw-r--r--   0 julien     (501) staff       (20)    55847 2021-07-07 15:04:10.000000 darts-0.9.1/datasets/temps.csv
+-rw-r--r--   0 julien     (501) staff       (20)    26373 2021-07-07 15:04:10.000000 darts-0.9.1/datasets/us_gasoline.csv
+-rw-r--r--   0 julien     (501) staff       (20)     3003 2021-07-07 15:04:10.000000 darts-0.9.1/datasets/wineind.csv
+-rw-r--r--   0 julien     (501) staff       (20)     1915 2021-07-07 15:04:10.000000 darts-0.9.1/datasets/woolyrnq.csv
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.352636 darts-0.9.1/docs/
+-rw-r--r--   0 julien     (501) staff       (20)     1009 2021-07-17 12:56:13.000000 darts-0.9.1/docs/Makefile
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.353899 darts-0.9.1/docs/source/
+-rw-r--r--   0 julien     (501) staff       (20)     3178 2021-07-17 13:19:40.000000 darts-0.9.1/docs/source/conf.py
+-rw-r--r--   0 julien     (501) staff       (20)     2690 2021-07-17 12:56:13.000000 darts-0.9.1/docs/source/examples.rst
+-rw-r--r--   0 julien     (501) staff       (20)      276 2021-01-31 13:26:04.000000 darts-0.9.1/docs/source/index.rst
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.355395 darts-0.9.1/docs/source/static/
+-rw-r--r--   0 julien     (501) staff       (20)        0 2020-08-26 18:23:45.000000 darts-0.9.1/docs/source/static/.gitkeep
+-rw-r--r--   0 julien     (501) staff       (20)    84068 2020-08-26 18:23:45.000000 darts-0.9.1/docs/source/static/darts-logo-trim.png
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.361125 darts-0.9.1/docs/templates/
+-rw-r--r--   0 julien     (501) staff       (20)      103 2021-01-31 13:23:05.000000 darts-0.9.1/docs/templates/module.rst_t
+-rw-r--r--   0 julien     (501) staff       (20)      582 2021-01-31 13:27:59.000000 darts-0.9.1/docs/templates/package.rst_t
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.399888 darts-0.9.1/examples/
+-rw-r--r--   0 julien     (501) staff       (20)   642786 2021-07-09 15:18:43.000000 darts-0.9.1/examples/01-darts-intro.ipynb
+-rw-r--r--   0 julien     (501) staff       (20)   311945 2021-07-09 15:18:43.000000 darts-0.9.1/examples/02-multi-time-series-and-covariates.ipynb
+-rw-r--r--   0 julien     (501) staff       (20)   390534 2021-07-09 15:18:43.000000 darts-0.9.1/examples/03-data-processing.ipynb
+-rw-r--r--   0 julien     (501) staff       (20)   221195 2021-07-07 15:04:10.000000 darts-0.9.1/examples/04-FFT-examples.ipynb
+-rw-r--r--   0 julien     (501) staff       (20)   211992 2021-07-09 15:18:43.000000 darts-0.9.1/examples/05-RNN-examples.ipynb
+-rw-r--r--   0 julien     (501) staff       (20)   200249 2021-07-09 15:18:43.000000 darts-0.9.1/examples/06-TCN-examples.ipynb
+-rw-r--r--   0 julien     (501) staff       (20)   198701 2021-07-07 15:04:10.000000 darts-0.9.1/examples/07-Transformer-examples.ipynb
+-rw-r--r--   0 julien     (501) staff       (20)   240623 2021-07-07 15:04:10.000000 darts-0.9.1/examples/08-NBEATS-examples.ipynb
+-rw-r--r--   0 julien     (501) staff       (20)   229008 2021-07-09 15:18:43.000000 darts-0.9.1/examples/09-DeepAR-examples.ipynb
+-rw-r--r--   0 julien     (501) staff       (20)   247532 2021-07-09 15:18:43.000000 darts-0.9.1/examples/10-DeepTCN-examples.ipynb
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.427238 darts-0.9.1/examples/M4_competition/
+-rw-r--r--   0 julien     (501) staff       (20)    33825 2021-07-09 15:18:43.000000 darts-0.9.1/examples/M4_competition/M4_competition_benchmark.ipynb
+-rw-r--r--   0 julien     (501) staff       (20)     1553 2020-10-07 09:45:20.000000 darts-0.9.1/examples/M4_competition/M4_metrics.py
+-rw-r--r--   0 julien     (501) staff       (20)     2632 2020-12-21 14:57:41.000000 darts-0.9.1/examples/M4_competition/create_ts.py
+-rw-r--r--   0 julien     (501) staff       (20)     1180 2020-10-07 09:45:20.000000 darts-0.9.1/examples/M4_competition/download_data_M4.py
+-rw-r--r--   0 julien     (501) staff       (20)     2649 2020-11-08 13:54:23.000000 darts-0.9.1/examples/M4_competition/evaluate_arima.py
+-rw-r--r--   0 julien     (501) staff       (20)     4883 2021-07-09 15:18:43.000000 darts-0.9.1/examples/M4_competition/evaluate_baselines.py
+-rw-r--r--   0 julien     (501) staff       (20)    11417 2021-07-09 15:18:43.000000 darts-0.9.1/examples/M4_competition/evaluate_ensembling.py
+-rw-r--r--   0 julien     (501) staff       (20)     3272 2021-02-02 10:11:33.000000 darts-0.9.1/examples/M4_competition/evaluate_fft.py
+-rw-r--r--   0 julien     (501) staff       (20)    11717 2021-07-09 15:18:43.000000 darts-0.9.1/examples/M4_competition/evaluate_groe_R.py
+-rw-r--r--   0 julien     (501) staff       (20)     5493 2021-07-09 15:18:43.000000 darts-0.9.1/examples/M4_competition/evaluate_naive2_with_R.py
+-rw-r--r--   0 julien     (501) staff       (20)     3551 2021-07-09 15:18:43.000000 darts-0.9.1/examples/M4_competition/evaluate_prophet.py
+-rw-r--r--   0 julien     (501) staff       (20)     4682 2021-07-09 15:18:43.000000 darts-0.9.1/examples/M4_competition/evaluate_theta_methods.py
+-rw-r--r--   0 julien     (501) staff       (20)    51933 2021-07-09 15:18:43.000000 darts-0.9.1/examples/future-covariates-example.ipynb
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.191202 darts-0.9.1/examples/static/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.431712 darts-0.9.1/examples/static/images/
+-rw-r--r--   0 julien     (501) staff       (20)    53317 2021-02-02 10:11:33.000000 darts-0.9.1/examples/static/images/global_io.png
+-rw-r--r--   0 julien     (501) staff       (20)    66469 2021-02-02 10:11:33.000000 darts-0.9.1/examples/static/images/global_io_covs.png
+-rw-r--r--   0 julien     (501) staff       (20)    85947 2021-02-02 10:11:33.000000 darts-0.9.1/examples/static/images/seq_dataset_multi_ts.png
+-rw-r--r--   0 julien     (501) staff       (20)    42967 2021-02-02 10:11:33.000000 darts-0.9.1/examples/static/images/seq_dataset_one_ts.png
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.433513 darts-0.9.1/examples/utils/
+-rw-r--r--   0 julien     (501) staff       (20)       52 2020-10-07 09:45:20.000000 darts-0.9.1/examples/utils/__init__.py
+-rw-r--r--   0 julien     (501) staff       (20)      333 2020-10-07 09:45:20.000000 darts-0.9.1/examples/utils/utils.py
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.191596 darts-0.9.1/gradle/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.436003 darts-0.9.1/gradle/wrapper/
+-rw-r--r--   0 julien     (501) staff       (20)    58695 2020-10-07 09:45:20.000000 darts-0.9.1/gradle/wrapper/gradle-wrapper.jar
+-rw-r--r--   0 julien     (501) staff       (20)      200 2020-10-07 09:45:20.000000 darts-0.9.1/gradle/wrapper/gradle-wrapper.properties
+-rwxr-xr-x   0 julien     (501) staff       (20)     5764 2020-10-07 09:45:20.000000 darts-0.9.1/gradlew
+-rw-r--r--   0 julien     (501) staff       (20)     3056 2020-10-07 09:45:20.000000 darts-0.9.1/gradlew.bat
+-rwxr-xr-x   0 julien     (501) staff       (20)      232 2021-04-26 18:51:16.000000 darts-0.9.1/make_dists.sh
+-rw-r--r--   0 julien     (501) staff       (20)      104 2021-07-17 12:56:13.000000 darts-0.9.1/pyproject.toml
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.439234 darts-0.9.1/requirements/
+-rw-r--r--   0 julien     (501) staff       (20)      215 2021-07-17 12:56:13.000000 darts-0.9.1/requirements/core.txt
+-rw-r--r--   0 julien     (501) staff       (20)       81 2021-07-17 12:56:13.000000 darts-0.9.1/requirements/dev-all.txt
+-rw-r--r--   0 julien     (501) staff       (20)       67 2021-04-19 19:17:01.000000 darts-0.9.1/requirements/dev.txt
+-rw-r--r--   0 julien     (501) staff       (20)       15 2021-07-17 12:56:13.000000 darts-0.9.1/requirements/pmdarima.txt
+-rw-r--r--   0 julien     (501) staff       (20)       40 2021-07-17 12:56:13.000000 darts-0.9.1/requirements/prophet.txt
+-rw-r--r--   0 julien     (501) staff       (20)      264 2021-07-17 12:56:13.000000 darts-0.9.1/requirements/release.txt
+-rw-r--r--   0 julien     (501) staff       (20)       39 2021-07-17 12:56:13.000000 darts-0.9.1/requirements/torch.txt
+-rw-r--r--   0 julien     (501) staff       (20)       27 2020-10-07 09:45:20.000000 darts-0.9.1/settings.gradle
+-rw-r--r--   0 julien     (501) staff       (20)      145 2021-07-17 13:20:17.443848 darts-0.9.1/setup.cfg
+-rw-r--r--   0 julien     (501) staff       (20)     2092 2021-07-17 13:19:40.000000 darts-0.9.1/setup.py
+-rw-r--r--   0 julien     (501) staff       (20)     2265 2021-07-17 12:56:13.000000 darts-0.9.1/setup_u8darts.py
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.192009 darts-0.9.1/static/
+drwxr-xr-x   0 julien     (501) staff       (20)        0 2021-07-17 13:20:17.441790 darts-0.9.1/static/images/
+-rw-r--r--   0 julien     (501) staff       (20)    84068 2020-08-26 18:23:45.000000 darts-0.9.1/static/images/darts-logo-trim.png
+-rw-r--r--   0 julien     (501) staff       (20)    57635 2021-07-09 15:18:43.000000 darts-0.9.1/static/images/example.png
```

### Comparing `darts-0.9.0/.github/CODEOWNERS` & `darts-0.9.1/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md` & `darts-0.9.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md` & `darts-0.9.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/.github/workflows/develop.yml` & `darts-0.9.1/.github/workflows/merge.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-name: darts develop workflow
+name: darts PR merge workflow
 
 on:
-  pull_request:
+  push:
     branches:
       - develop
+      - master
 
 jobs:
   tests:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [macos-latest, ubuntu-latest]
         python-version: [3.7, 3.8, 3.9]
-        flavour: ['core', 'all']
+        flavour: ['all']
 
     steps:
       - name: "1. Clone repository"
         uses: actions/checkout@v2
 
       - name: "2. Set up Python ${{ matrix.python-version }}"
         uses: actions/setup-python@v1
@@ -34,94 +35,95 @@
         uses: actions/cache@v2
         with:
           path: ~/.gradle/caches
           key: tests-${{ runner.os }}-gradle-${{ hashFiles('gradle/wrapper/gradle-wrapper.properties', 'build.gradle') }}
 
       - name: "4. Setup pip"
         run: |
-          ./gradlew setupPip
+          ./gradlew installPipLatest
 
       - name: "5. Attach cache for pip"
         uses: actions/cache@v1
         id: cache
         with:
           path: ~/.cache/pip
-          key: tests-${{ runner.os }}-${{ matrix.python-version }}-pip-${{ hashFiles('requirements/core.txt', 'requirements/dev.txt', 'requirements/fbprophet.txt', 'requirements/pmdarima.txt', 'requirements/torch.txt') }}
+          key: tests-${{ runner.os }}-${{ matrix.python-version }}-pip-${{ hashFiles('requirements-latest.txt') }}
 
       - name: "6. Tests"
         run: |
           ./gradlew "test_${{matrix.flavour}}"
 
-  docs:
+  check-examples:
     runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        example-name: [01-darts-intro.ipynb, 02-multi-time-series-and-covariates.ipynb, 03-data-processing.ipynb, 04-FFT-examples.ipynb, 05-RNN-examples.ipynb]
     steps:
       - name: "1. Clone repository"
         uses: actions/checkout@v2
 
-      - name: "2. Set up Python 3.8"
+      - name: "2. Set up Python 3.9"
         uses: actions/setup-python@v1
         with:
-          python-version: 3.8
-
-      - name: "3. Install pandoc"
-        run: |
-          sudo apt-get install -y pandoc
+          python-version: 3.9
 
-        # downloading gradle multiple times in parallel can yield to connection errors
-      - name: "4. Cache gradle distribution"
+      # downloading gradle multiple times in parallel can yield to connection errors
+      - name: "3. Cache gradle distribution"
         uses: actions/cache@v2
         with:
           path: ~/.gradle/wrapper/dists
           key: tests-${{ runner.os }}-gradle-${{ hashFiles('gradle/wrapper/gradle-wrapper.properties') }}
 
-      - name: "4.1 Cache gradle packages"
+      - name: "3.1 Cache gradle packages"
         uses: actions/cache@v2
         with:
           path: ~/.gradle/caches
           key: tests-${{ runner.os }}-gradle-${{ hashFiles('gradle/wrapper/gradle-wrapper.properties', 'build.gradle') }}
 
-      - name: "5. Setup pip"
+      # TODO: why is this a matrix? there is no pip caching, and we restart this for each item in the matrix
+      - name: "4. Run examples ${{matrix.example-name}}"
         run: |
-          ./gradlew setupPip
-
-      - name: "6. Attach cache for pip"
-        uses: actions/cache@v1
-        id: cache
-        with:
-          path: ~/.cache/pip
-          key: tests-${{ runner.os }}-3.8-pip-${{ hashFiles('requirements/core.txt', 'requirements/release.txt') }}
+          ./gradlew checkExample -PexampleName=${{matrix.example-name}}
 
-      - name: "7. Build docs"
-        run: |
-          ./gradlew buildDocs
-  
-  check-examples:
+  docs:
     runs-on: ubuntu-latest
-    strategy:
-      matrix:
-        example-name: [04-FFT-examples.ipynb, 05-RNN-examples.ipynb, 01-darts-intro.ipynb, 03-data-processing.ipynb, 02-multi-time-series-and-covariates.ipynb]
+
     steps:
       - name: "1. Clone repository"
         uses: actions/checkout@v2
 
-      - name: "2. Set up Python 3.8"
+      - name: "2. Set up Python 3.9"
         uses: actions/setup-python@v1
         with:
-          python-version: 3.8
+          python-version: 3.9
 
-        # downloading gradle multiple times in parallel can yield to connection errors
-      - name: "3. Cache gradle distribution"
+      - name: "3. Install pandoc"
+        run: |
+          sudo apt-get install -y pandoc
+
+      # downloading gradle multiple times in parallel can yield to connection errors
+      - name: "4. Cache gradle distribution"
         uses: actions/cache@v2
         with:
           path: ~/.gradle/wrapper/dists
           key: tests-${{ runner.os }}-gradle-${{ hashFiles('gradle/wrapper/gradle-wrapper.properties') }}
 
-      - name: "3.1 Cache gradle packages"
+      - name: "4.1 Cache gradle packages"
         uses: actions/cache@v2
         with:
           path: ~/.gradle/caches
           key: tests-${{ runner.os }}-gradle-${{ hashFiles('gradle/wrapper/gradle-wrapper.properties', 'build.gradle') }}
 
-      - name: "4. Run examples ${{matrix.example-name}}"
+      - name: "5. Setup pip"
         run: |
-          ./gradlew checkExample -PexampleName=${{matrix.example-name}}
+          ./gradlew setupPip
 
+      - name: "6. Attach cache for pip"
+        uses: actions/cache@v1
+        id: cache
+        with:
+          path: ~/.cache/pip
+          key: release-${{ runner.os }}-3.9-pip-${{ hashFiles('requirements/core.txt', 'requirements/release.txt') }}
+
+      - name: "7. Build docs"
+        run: |
+          ./gradlew buildDocs
```

### Comparing `darts-0.9.0/.github/workflows/merge.yml` & `darts-0.9.1/.github/workflows/develop.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-name: darts PR merge workflow
+name: darts develop workflow
 
 on:
-  push:
+  pull_request:
     branches:
       - develop
-      - master
 
 jobs:
   tests:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [macos-latest, ubuntu-latest]
-        python-version: [3.7, 3.8, 3.9]
-        flavour: ['core', 'all', 'pmdarima', 'torch', 'fbprophet']
+        python-version: [3.9]
+        flavour: ['all']
 
     steps:
       - name: "1. Clone repository"
         uses: actions/checkout@v2
 
       - name: "2. Set up Python ${{ matrix.python-version }}"
         uses: actions/setup-python@v1
@@ -35,94 +34,93 @@
         uses: actions/cache@v2
         with:
           path: ~/.gradle/caches
           key: tests-${{ runner.os }}-gradle-${{ hashFiles('gradle/wrapper/gradle-wrapper.properties', 'build.gradle') }}
 
       - name: "4. Setup pip"
         run: |
-          ./gradlew setupPip
+          ./gradlew installPipLatest
 
       - name: "5. Attach cache for pip"
         uses: actions/cache@v1
         id: cache
         with:
           path: ~/.cache/pip
-          key: tests-${{ runner.os }}-${{ matrix.python-version }}-pip-${{ hashFiles('requirements/core.txt', 'requirements/dev.txt', 'requirements/fbprophet.txt', 'requirements/pmdarima.txt', 'requirements/torch.txt') }}
+          key: tests-${{ runner.os }}-${{ matrix.python-version }}-pip-${{ hashFiles('requirements-latest.txt') }}
 
       - name: "6. Tests"
         run: |
           ./gradlew "test_${{matrix.flavour}}"
 
-  check-examples:
+  docs:
     runs-on: ubuntu-latest
-    strategy:
-      matrix:
-        example-name: [01-darts-intro.ipynb, 02-multi-time-series-and-covariates.ipynb, 03-data-processing.ipynb, 04-FFT-examples.ipynb, 05-RNN-examples.ipynb]
     steps:
       - name: "1. Clone repository"
         uses: actions/checkout@v2
 
-      - name: "2. Set up Python 3.8"
+      - name: "2. Set up Python 3.9"
         uses: actions/setup-python@v1
         with:
-          python-version: 3.8
+          python-version: 3.9
 
-      # downloading gradle multiple times in parallel can yield to connection errors
-      - name: "3. Cache gradle distribution"
+      - name: "3. Install pandoc"
+        run: |
+          sudo apt-get install -y pandoc
+
+        # downloading gradle multiple times in parallel can yield to connection errors
+      - name: "4. Cache gradle distribution"
         uses: actions/cache@v2
         with:
           path: ~/.gradle/wrapper/dists
           key: tests-${{ runner.os }}-gradle-${{ hashFiles('gradle/wrapper/gradle-wrapper.properties') }}
 
-      - name: "3.1 Cache gradle packages"
+      - name: "4.1 Cache gradle packages"
         uses: actions/cache@v2
         with:
           path: ~/.gradle/caches
           key: tests-${{ runner.os }}-gradle-${{ hashFiles('gradle/wrapper/gradle-wrapper.properties', 'build.gradle') }}
 
-      - name: "4. Run examples ${{matrix.example-name}}"
+      - name: "5. Setup pip"
         run: |
-          ./gradlew checkExample -PexampleName=${{matrix.example-name}}
+          ./gradlew setupPip
 
-  docs:
-    runs-on: ubuntu-latest
+      - name: "6. Attach cache for pip"
+        uses: actions/cache@v1
+        id: cache
+        with:
+          path: ~/.cache/pip
+          key: tests-${{ runner.os }}-3.9-pip-${{ hashFiles('requirements/core.txt', 'requirements/release.txt') }}
 
+      - name: "7. Build docs"
+        run: |
+          ./gradlew buildDocs
+  
+  check-examples:
+    runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        example-name: [04-FFT-examples.ipynb, 05-RNN-examples.ipynb, 01-darts-intro.ipynb, 03-data-processing.ipynb, 02-multi-time-series-and-covariates.ipynb]
     steps:
       - name: "1. Clone repository"
         uses: actions/checkout@v2
 
-      - name: "2. Set up Python 3.8"
+      - name: "2. Set up Python 3.9"
         uses: actions/setup-python@v1
         with:
-          python-version: 3.8
-
-      - name: "3. Install pandoc"
-        run: |
-          sudo apt-get install -y pandoc
+          python-version: 3.9
 
-      # downloading gradle multiple times in parallel can yield to connection errors
-      - name: "4. Cache gradle distribution"
+        # downloading gradle multiple times in parallel can yield to connection errors
+      - name: "3. Cache gradle distribution"
         uses: actions/cache@v2
         with:
           path: ~/.gradle/wrapper/dists
           key: tests-${{ runner.os }}-gradle-${{ hashFiles('gradle/wrapper/gradle-wrapper.properties') }}
 
-      - name: "4.1 Cache gradle packages"
+      - name: "3.1 Cache gradle packages"
         uses: actions/cache@v2
         with:
           path: ~/.gradle/caches
           key: tests-${{ runner.os }}-gradle-${{ hashFiles('gradle/wrapper/gradle-wrapper.properties', 'build.gradle') }}
 
-      - name: "5. Setup pip"
-        run: |
-          ./gradlew setupPip
-
-      - name: "6. Attach cache for pip"
-        uses: actions/cache@v1
-        id: cache
-        with:
-          path: ~/.cache/pip
-          key: release-${{ runner.os }}-3.8-pip-${{ hashFiles('requirements/core.txt', 'requirements/release.txt') }}
-
-      - name: "7. Build docs"
+      - name: "4. Run examples ${{matrix.example-name}}"
         run: |
-          ./gradlew buildDocs
+          ./gradlew checkExample -PexampleName=${{matrix.example-name}}
```

### Comparing `darts-0.9.0/.github/workflows/release.yml` & `darts-0.9.1/.github/workflows/release.yml`

 * *Files 0% similar despite different names*

```diff
@@ -13,18 +13,18 @@
     steps:
       - name: "1. Clone repository"
         uses: actions/checkout@v2
         with:
           token: ${{ secrets.RELEASE_WORKFLOW_TOKEN }}
           fetch-depth: '1'
 
-      - name: "2. Set up Python 3.8"
+      - name: "2. Set up Python 3.9"
         uses: actions/setup-python@v1
         with:
-          python-version: 3.8
+          python-version: 3.9
 
       - name: "3. Update pip"
         run: |
           python -m pip install --upgrade pip
 
       - name: "4. Attach cache for pip"
         uses: actions/cache@v1
@@ -124,18 +124,18 @@
   deploy-docs:
     runs-on: ubuntu-latest
     needs: [release]
     steps:
       - name: "1. Clone repository"
         uses: actions/checkout@v2
 
-      - name: "2. Set up Python 3.8"
+      - name: "2. Set up Python 3.9"
         uses: actions/setup-python@v1
         with:
-          python-version: 3.8
+          python-version: 3.9
 
       - name: "3. Install pandoc"
         run: |
           sudo apt-get install -y pandoc
 
         # downloading gradle multiple times in parallel can yield to connection errors
       - name: "4. Cache gradle distribution"
```

### Comparing `darts-0.9.0/CHANGELOG.md` & `darts-0.9.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,40 @@
 
 # Changelog
 
 Darts is still in an early development phase and we cannot always guarantee backwards compatibility. Changes that may **break code which uses a previous release of Darts** are marked with a "&#x1F534;".
 
 ## [Unreleased](https://github.com/unit8co/darts/tree/develop)
-[Full Changelog](https://github.com/unit8co/darts/compare/0.9.0...develop)
+[Full Changelog](https://github.com/unit8co/darts/compare/0.9.1...develop)
+
+## [0.9.1](https://github.com/unit8co/darts/tree/0.9.1) (2021-07-17)
+### For users of the library:
+
+**Added:**
+- Improved `GaussianProcessFilter`, now handling missing values, and better handling
+time series indexed by datetimes.
+- Improved Gaussian Process notebook.
+
+**Fixed:**
+- `TimeSeries` now supports indexing using `pandas.Int64Index` and not just `pandas.RangeIndex`,
+which solves some indexing issues.
+- We have changed all factory methods of `TimeSeries` to have `fill_missing_dates=False` by
+default. This is because in some cases inferring the frequency for missing dates and
+resampling the series is causing significant performance overhead.
+- Fixed backtesting to make it work with integer-indexed series.
+- Fixed a bug that was causing inference to crash on GPUs for some models.
+- Fixed the default folder name, which was causing issues on Windows systems.
+- We have slightly improved the documentation rendering and fixed the titles 
+of the documentation pages for `RNNModel` and `BlockRNNModel` to distinguish them.
+
+**Changed:**
+- The dependencies are not pinned to some exact versions anymore.
+
+### For developers of the library:
+- We have fixed the building process.
 
 ## [0.9.0](https://github.com/unit8co/darts/tree/0.9.0) (2021-07-09)
 ### For users of the library:
 
 **Added:**
 - Multiple forecasting models can now produce probabilistic forecasts by specifying a `num_samples` parameter when calling `predict()`. Stochastic forecasts are stored by utilizing the new `samples` dimension in the refactored `TimeSeries` class (see 'Changed' section). Models supporting probabilistic predictions so far are `ARIMA`, `ExponentialSmoothing`, `RNNModel` and `TCNModel`.
 - Introduced `LikelihoodModel` class which is used by probabilistic `TorchForecastingModel` classes in order to make predictions in the form of parametrized distributions of different types.
```

### Comparing `darts-0.9.0/CONTRIBUTE.md` & `darts-0.9.1/CONTRIBUTE.md`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/Dockerfile` & `darts-0.9.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/LICENSE` & `darts-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/PKG-INFO` & `darts-0.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darts
-Version: 0.9.0
+Version: 0.9.1
 Summary: A python library for easy manipulation and forecasting of time series.
 Home-page: https://unit8co.github.io/darts/
 Maintainer: Unit8 SA
 Maintainer-email: darts@unit8.co
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/unit8co/darts/issues
 Project-URL: Documentation, https://unit8co.github.io/darts/
@@ -139,30 +139,29 @@
 inferences of the underlying states/values.
 
 ## Forecasting Models
 Here's a breakdown of the forecasting models currently implemented in Darts. We are constantly working
 on bringing more models and features.
 
 Model | Univariate | Multivariate | Probabilistic | Multiple-series training | Past-observed covariates support | Future-known covariates support
---- | --- | --- | --- | --- | --- | --- |
-`ARIMA` | x | | x | | | |
-`VARIMA` | x | x | | | | |
-`AutoARIMA` | x | | | | | |
-`ExponentialSmoothing` | x | | x | | | |
-`Theta` and `FourTheta` | x | | | | | |
-`Prophet` | x | | | | | |
-`FFT` (Fast Fourier Transform) | x | | | | | |
-Regression Models (incl `RandomForest` and `LinearRegressionModel`) | x | | | | | |
-`RNNModel` (incl. LSTM and GRU); equivalent to DeepAR in its probabilistic version | x | x | x | x | x | x |
-`BlockRNNModel` (incl. LSTM and GRU) | x | x | | x | x | (x) |
-`NBEATSModel` | x | x | | x | x | (x) |
-`TCNModel` | x | x | x | x | x | (x) |
-`TransformerModel` | x | x | | x | x | (x) |
-Naive Baselines | x | | | | | |
-
+--- | --- | --- | --- | --- | --- | ---
+`ARIMA` | x | | x | | |
+`VARIMA` | x | x | | | |
+`AutoARIMA` | x | | | | |
+`ExponentialSmoothing` | x | | x | | |
+`Theta` and `FourTheta` | x | | | | |
+`Prophet` | x | | | | |
+`FFT` (Fast Fourier Transform) | x | | | | |
+Regression Models (incl `RandomForest` and `LinearRegressionModel`) | x | | | | |
+`RNNModel` (incl. LSTM and GRU); equivalent to DeepAR in its probabilistic version | x | x | x | x | x | x
+`BlockRNNModel` (incl. LSTM and GRU) | x | x | | x | x | ( x )
+`NBEATSModel` | x | x | | x | x | ( x )
+`TCNModel` | x | x | x | x | x | ( x )
+`TransformerModel` | x | x | | x | x | ( x )
+Naive Baselines | x | | | | |
 
 ## Contribute
 
 The development is ongoing, and there are many new features that we want to add.
 We welcome pull requests and issues on GitHub.
 
 Before working on a contribution (a new feature or a fix), [**check our contribution guidelines**](CONTRIBUTE.md).
@@ -172,20 +171,20 @@
 
 If what you want to tell us is not a suitable github issue, feel free to send us an email at <a href="mailto:darts@unit8.co">darts@unit8.co</a> for darts related matters or <a href="mailto:info@unit8.co">info@unit8.co</a> for any other inquiries.
 
 ## Installation Guide
 
 ### Preconditions
 
-Some of the models depend on `fbprophet` and `torch`, which have non-Python dependencies.
+Some of the models depend on `prophet` and `torch`, which have non-Python dependencies.
 A Conda environment is thus recommended because it will handle all of those in one go.
 
 The following steps assume running inside a conda environment.
 If that's not possible, first follow the official instructions to install
-[fbprophet](https://facebook.github.io/prophet/docs/installation.html#python)
+[prophet](https://facebook.github.io/prophet/docs/installation.html#python)
 and [torch](https://pytorch.org/get-started/locally/), then skip to
 [Install darts](#install-darts)
 
 To create a conda environment for Python 3.7
 (after installing [conda](https://docs.conda.io/en/latest/miniconda.html)):
 
     conda create --name <env-name> python=3.7
@@ -193,30 +192,30 @@
 Don't forget to activate your virtual environment
 
     conda activate <env-name>
 
 
 #### MAC
 
-    conda install -c conda-forge -c pytorch pip fbprophet pytorch
+    conda install -c conda-forge -c pytorch pip prophet pytorch
 
 #### Linux and Windows
 
-    conda install -c conda-forge -c pytorch pip fbprophet pytorch cpuonly
+    conda install -c conda-forge -c pytorch pip prophet pytorch cpuonly
 
 ### Install darts
 
 Install Darts with all available models: `pip install darts`.
 
 As some models have relatively heavy (or non-Python) dependencies,
 we also maintain the `u8darts` package, which provides the following alternate lighter install options:
 
 * Install core only (without neural networks, Prophet or AutoARIMA): `pip install u8darts`
 * Install core + neural networks (PyTorch): `pip install 'u8darts[torch]'`
-* Install core + Facebook Prophet: `pip install 'u8darts[fbprophet]'`
+* Install core + Facebook Prophet: `pip install 'u8darts[prophet]'`
 * Install core + AutoARIMA: `pip install 'u8darts[pmdarima]'`
 
 ### Running the examples only, without installing:
 
 If the conda setup is causing too many problems, we also provide a Docker image with everything set up for you and ready-to-use Python notebooks with demo examples.
 To run the example notebooks without installing our libraries natively on your machine, you can use our Docker image:
 ```bash
@@ -240,15 +239,15 @@
 alternatively you can run
 ```bash
 ./gradlew unitTest_all # to run only unittests
 ./gradlew coverageTest # to run coverage
 ./gradlew lint         # to run linter
 ```
 
-To run the tests for specific flavours of the library, replace `_all` with `_core`, `_fbprophet`, `_pmdarima` or `_torch`.
+To run the tests for specific flavours of the library, replace `_all` with `_core`, `_prophet`, `_pmdarima` or `_torch`.
 
 ### Documentation
 
 To build documantation locally just run
 ```bash
 ./gradlew buildDocs
 ```
```

### Comparing `darts-0.9.0/README.md` & `darts-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -108,30 +108,29 @@
 inferences of the underlying states/values.
 
 ## Forecasting Models
 Here's a breakdown of the forecasting models currently implemented in Darts. We are constantly working
 on bringing more models and features.
 
 Model | Univariate | Multivariate | Probabilistic | Multiple-series training | Past-observed covariates support | Future-known covariates support
---- | --- | --- | --- | --- | --- | --- |
-`ARIMA` | x | | x | | | |
-`VARIMA` | x | x | | | | |
-`AutoARIMA` | x | | | | | |
-`ExponentialSmoothing` | x | | x | | | |
-`Theta` and `FourTheta` | x | | | | | |
-`Prophet` | x | | | | | |
-`FFT` (Fast Fourier Transform) | x | | | | | |
-Regression Models (incl `RandomForest` and `LinearRegressionModel`) | x | | | | | |
-`RNNModel` (incl. LSTM and GRU); equivalent to DeepAR in its probabilistic version | x | x | x | x | x | x |
-`BlockRNNModel` (incl. LSTM and GRU) | x | x | | x | x | (x) |
-`NBEATSModel` | x | x | | x | x | (x) |
-`TCNModel` | x | x | x | x | x | (x) |
-`TransformerModel` | x | x | | x | x | (x) |
-Naive Baselines | x | | | | | |
-
+--- | --- | --- | --- | --- | --- | ---
+`ARIMA` | x | | x | | |
+`VARIMA` | x | x | | | |
+`AutoARIMA` | x | | | | |
+`ExponentialSmoothing` | x | | x | | |
+`Theta` and `FourTheta` | x | | | | |
+`Prophet` | x | | | | |
+`FFT` (Fast Fourier Transform) | x | | | | |
+Regression Models (incl `RandomForest` and `LinearRegressionModel`) | x | | | | |
+`RNNModel` (incl. LSTM and GRU); equivalent to DeepAR in its probabilistic version | x | x | x | x | x | x
+`BlockRNNModel` (incl. LSTM and GRU) | x | x | | x | x | ( x )
+`NBEATSModel` | x | x | | x | x | ( x )
+`TCNModel` | x | x | x | x | x | ( x )
+`TransformerModel` | x | x | | x | x | ( x )
+Naive Baselines | x | | | | |
 
 ## Contribute
 
 The development is ongoing, and there are many new features that we want to add.
 We welcome pull requests and issues on GitHub.
 
 Before working on a contribution (a new feature or a fix), [**check our contribution guidelines**](CONTRIBUTE.md).
@@ -141,20 +140,20 @@
 
 If what you want to tell us is not a suitable github issue, feel free to send us an email at <a href="mailto:darts@unit8.co">darts@unit8.co</a> for darts related matters or <a href="mailto:info@unit8.co">info@unit8.co</a> for any other inquiries.
 
 ## Installation Guide
 
 ### Preconditions
 
-Some of the models depend on `fbprophet` and `torch`, which have non-Python dependencies.
+Some of the models depend on `prophet` and `torch`, which have non-Python dependencies.
 A Conda environment is thus recommended because it will handle all of those in one go.
 
 The following steps assume running inside a conda environment.
 If that's not possible, first follow the official instructions to install
-[fbprophet](https://facebook.github.io/prophet/docs/installation.html#python)
+[prophet](https://facebook.github.io/prophet/docs/installation.html#python)
 and [torch](https://pytorch.org/get-started/locally/), then skip to
 [Install darts](#install-darts)
 
 To create a conda environment for Python 3.7
 (after installing [conda](https://docs.conda.io/en/latest/miniconda.html)):
 
     conda create --name <env-name> python=3.7
@@ -162,30 +161,30 @@
 Don't forget to activate your virtual environment
 
     conda activate <env-name>
 
 
 #### MAC
 
-    conda install -c conda-forge -c pytorch pip fbprophet pytorch
+    conda install -c conda-forge -c pytorch pip prophet pytorch
 
 #### Linux and Windows
 
-    conda install -c conda-forge -c pytorch pip fbprophet pytorch cpuonly
+    conda install -c conda-forge -c pytorch pip prophet pytorch cpuonly
 
 ### Install darts
 
 Install Darts with all available models: `pip install darts`.
 
 As some models have relatively heavy (or non-Python) dependencies,
 we also maintain the `u8darts` package, which provides the following alternate lighter install options:
 
 * Install core only (without neural networks, Prophet or AutoARIMA): `pip install u8darts`
 * Install core + neural networks (PyTorch): `pip install 'u8darts[torch]'`
-* Install core + Facebook Prophet: `pip install 'u8darts[fbprophet]'`
+* Install core + Facebook Prophet: `pip install 'u8darts[prophet]'`
 * Install core + AutoARIMA: `pip install 'u8darts[pmdarima]'`
 
 ### Running the examples only, without installing:
 
 If the conda setup is causing too many problems, we also provide a Docker image with everything set up for you and ready-to-use Python notebooks with demo examples.
 To run the example notebooks without installing our libraries natively on your machine, you can use our Docker image:
 ```bash
@@ -209,15 +208,15 @@
 alternatively you can run
 ```bash
 ./gradlew unitTest_all # to run only unittests
 ./gradlew coverageTest # to run coverage
 ./gradlew lint         # to run linter
 ```
 
-To run the tests for specific flavours of the library, replace `_all` with `_core`, `_fbprophet`, `_pmdarima` or `_torch`.
+To run the tests for specific flavours of the library, replace `_all` with `_core`, `_prophet`, `_pmdarima` or `_torch`.
 
 ### Documentation
 
 To build documantation locally just run
 ```bash
 ./gradlew buildDocs
 ```
```

### Comparing `darts-0.9.0/build.gradle` & `darts-0.9.1/build.gradle`

 * *Files 22% similar despite different names*

```diff
@@ -53,37 +53,52 @@
 }
 
 // setup requirements
 task setupPip(type: Exec) {
     commandLine "python", "-m", "pip", "install", "--upgrade", "pip"
 }
 
+task installPipLatest {
+    dependsOn setupPip
+    doLast {
+        exec {
+            commandLine "pip", "install", "pip-tools"
+        }
+        exec {
+            commandLine "pip-compile", "-o", "requirements-latest.txt"
+        }
+        exec {
+            commandLine "pip", "install", "-r", "requirements-latest.txt"
+        }
+    }
+}
+
 void createPipInstallTask(String flavour) {
    String taskName = "pip_" + flavour;
    String taskArgument = "requirements/" + flavour + ".txt";
    task (taskName, type: Exec) {
       commandLine "pip", "install", "-q", "-r", taskArgument
    }
 }
 
-String[] flavours = ["core", "fbprophet", "pmdarima", "dev", "torch", "release"];
+String[] flavours = ["core", "prophet", "pmdarima", "dev", "torch", "release"];
 
 for(String flavour : flavours) {
     createPipInstallTask(flavour);
 }
 
 task installLocally(type:Exec) {
     commandLine "pip", "install", ".[all]"
 }
 
 task pipInstall() {
     doFirst {
         setupPip
     }
-    dependsOn pip_core, pip_dev, pip_fbprophet, pip_pmdarima, pip_torch, pip_release
+    dependsOn pip_core, pip_dev, pip_prophet, pip_pmdarima, pip_torch, pip_release
 }
 
 // Tests
 void coverageTestSteps() {
     exec {
         commandLine "coverage", "run", "--source=darts/", "-m", "unittest"
     }
@@ -111,27 +126,33 @@
    String taskArgument1 = "unitTest_" + flavour;
    task (taskName) {
         dependsOn(taskArgument1)
         dependsOn lint
    }
 }
 
-flavours = ["core", "fbprophet", "pmdarima", "torch"];
+flavours = ["core", "prophet", "pmdarima", "torch"];
 
 for(String flavour : flavours) {
     createPipRelatedTask(flavour);
 }
 
 task unitTest_all(type: Exec) {
-    dependsOn pip_core, pip_dev, pip_fbprophet, pip_pmdarima, pip_torch
+    dependsOn installPipLatest, pip_dev
+    doFirst {
+        installPipLatest
+    }
     commandLine "python", "-m", "unittest"
 }
 
 task coverageTest_all() {
-    dependsOn pip_core, pip_dev, pip_fbprophet, pip_pmdarima, pip_torch
+    dependsOn installPipLatest, pip_dev
+    doFirst {
+        installPipLatest
+    }
     doLast {
         coverageTestSteps()
     }
 }
 
 task test_all() {
     dependsOn unitTest_all
```

### Comparing `darts-0.9.0/conda_recipe/darts/meta.yaml` & `darts-0.9.1/conda_recipe/darts/meta.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% set data = load_setup_py_data() %}
 
 package:
   name: "darts"
-  version: "0.9.0"
+  version: "0.9.1"
 
 source:
   # root folder, not the package
   path: "../../../darts"
 
 build:
   number: 0
```

### Comparing `darts-0.9.0/coverage.sh` & `darts-0.9.1/coverage.sh`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/__init__.py` & `darts-0.9.1/darts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 
 from .timeseries import TimeSeries
 import matplotlib as mpl
 from matplotlib import cycler
 
 
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 
 colors = cycler(color=['black', '003DFD', 'b512b8', '11a9ba', '0d780f', 'f77f07', 'ba0f0f'])
 
 u8plots_mplstyle = {
     'font.family' : 'sans serif',
     'axes.edgecolor' : 'black',
     'axes.grid' : True,
```

### Comparing `darts-0.9.0/darts/dataprocessing/pipeline.py` & `darts-0.9.1/darts/dataprocessing/pipeline.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/dataprocessing/transformers/base_data_transformer.py` & `darts-0.9.1/darts/dataprocessing/transformers/base_data_transformer.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/dataprocessing/transformers/boxcox.py` & `darts-0.9.1/darts/dataprocessing/transformers/boxcox.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/dataprocessing/transformers/fittable_data_transformer.py` & `darts-0.9.1/darts/dataprocessing/transformers/fittable_data_transformer.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/dataprocessing/transformers/invertible_data_transformer.py` & `darts-0.9.1/darts/dataprocessing/transformers/invertible_data_transformer.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/dataprocessing/transformers/mappers.py` & `darts-0.9.1/darts/dataprocessing/transformers/mappers.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/dataprocessing/transformers/missing_values_filler.py` & `darts-0.9.1/darts/dataprocessing/transformers/missing_values_filler.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/dataprocessing/transformers/scaler.py` & `darts-0.9.1/darts/dataprocessing/transformers/scaler.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/datasets/__init__.py` & `darts-0.9.1/darts/datasets/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,16 @@
 
     def __init__(self):
         super().__init__(metadata=DatasetLoaderMetadata(
             "monthly_milk-incomplete.csv",
             uri=_DEFAULT_PATH+"/monthly-milk-incomplete.csv",
             hash="49b275c7e2f8f28a6a05224be1a049a4",
             header_time="Month",
-            format_time="%Y-%m"
+            format_time="%Y-%m",
+            freq='M'
         ))
 
 
 class SunspotsDataset(DatasetLoaderCSV):
     """
     Monthly Sunspot Numbers, 1749 - 1983
 
@@ -193,15 +194,16 @@
 
     def __init__(self):
         super().__init__(metadata=DatasetLoaderMetadata(
             "temperatures.csv",
             uri=_DEFAULT_PATH+"/temps.csv",
             hash="ce5b5e4929793ec8b6a54711110acebf",
             header_time="Date",
-            format_time="%m/%d/%Y"
+            format_time="%m/%d/%Y",
+            freq='D'
         ))
 
 
 class USGasolineDataset(DatasetLoaderCSV):
     """
     Weekly U.S. Product Supplied of Finished Motor Gasoline between 1991-02-08 and 2021-04-30
```

### Comparing `darts-0.9.0/darts/datasets/dataset_loaders.py` & `darts-0.9.1/darts/datasets/dataset_loaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     # md5 hash of the file to be downloaded
     hash: str
     # used to parse the dataset file
     header_time: str
     # used to convert the string date to pd.Datetime
     # https://docs.python.org/3/library/datetime.html#strftime-and-strptime-behavior
     format_time: str = None
+    # used to indicate the freq when we already know it
+    freq: str = None
 
 
 class DatasetLoadingException(BaseException):
     pass
 
 
 class DatasetLoader(ABC):
@@ -141,9 +143,9 @@
     def __init__(self, metadata: DatasetLoaderMetadata, root_path: Path = None):
         super().__init__(metadata, root_path)
 
     def _load_from_disk(self, path_to_file: Path, metadata: DatasetLoaderMetadata) -> TimeSeries:
         df = pd.read_csv(path_to_file)
         if metadata.header_time is not None:
             df = self._format_time_column(df)
-            return TimeSeries.from_dataframe(df=df, time_col=metadata.header_time)
+            return TimeSeries.from_dataframe(df=df, time_col=metadata.header_time, freq=metadata.freq)
         return TimeSeries.from_dataframe(df)
```

### Comparing `darts-0.9.0/darts/logging.py` & `darts-0.9.1/darts/logging.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/metrics/metrics.py` & `darts-0.9.1/darts/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/models/__init__.py` & `darts-0.9.1/darts/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 except ModuleNotFoundError:
     logger.warning("Support for AutoARIMA is not available. To enable it, install u8darts[pmdarima] or u8darts[all].")
 
 try:
     from .prophet import Prophet
 except ModuleNotFoundError:
     logger.warning("Support Facebook Prophet is not available. "
-                   "To enable it, install u8darts[fbprophet] or u8darts[all].")
+                   "To enable it, install u8darts[prophet] or u8darts[all].")
 
 try:
     from .block_rnn_model import BlockRNNModel
     from .rnn_model import RNNModel
     from .tcn_model import TCNModel
     from .nbeats import NBEATSModel
     from .transformer_model import TransformerModel
```

### Comparing `darts-0.9.0/darts/models/arima.py` & `darts-0.9.1/darts/models/arima.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/models/auto_arima.py` & `darts-0.9.1/darts/models/auto_arima.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/models/baselines.py` & `darts-0.9.1/darts/models/baselines.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/models/block_rnn_model.py` & `darts-0.9.1/darts/models/block_rnn_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-Recurrent Neural Networks
--------------------------
+Block Recurrent Neural Networks
+-------------------------------
 """
 
 import torch.nn as nn
 import torch
 from numpy.random import RandomState
 from typing import List, Optional, Union
```

### Comparing `darts-0.9.0/darts/models/ensemble_model.py` & `darts-0.9.1/darts/models/ensemble_model.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/models/exponential_smoothing.py` & `darts-0.9.1/darts/models/exponential_smoothing.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/models/fft.py` & `darts-0.9.1/darts/models/fft.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/models/filtering_model.py` & `darts-0.9.1/darts/models/filtering_model.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/models/forecasting_model.py` & `darts-0.9.1/darts/models/forecasting_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,17 +297,24 @@
             if last_points_only:
                 last_points_values.append(forecast.all_values()[-1])
                 last_points_times.append(forecast.end_time())
             else:
                 forecasts.append(forecast)
 
         if last_points_only:
-            return TimeSeries.from_times_and_values(pd.DatetimeIndex(last_points_times),
-                                                    np.array(last_points_values),
-                                                    freq=series.freq * stride)
+            if series.has_datetime_index:
+                return TimeSeries.from_times_and_values(pd.DatetimeIndex(last_points_times, freq=series.freq * stride),
+                                                        np.array(last_points_values))
+            else:
+                return TimeSeries.from_times_and_values(pd.RangeIndex(start=last_points_times[0],
+                                                                      stop=last_points_times[-1] + 1,
+                                                                      step=1),
+                                                        np.array(last_points_values))
+
+
         return forecasts
 
     def backtest(self,
                  series: TimeSeries,
                  covariates: Optional[TimeSeries] = None,
                  num_samples: int = 1,
                  start: Union[pd.Timestamp, float, int] = 0.5,
```

### Comparing `darts-0.9.0/darts/models/gaussian_process_filter.py` & `darts-0.9.1/darts/models/gaussian_process_filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Optional
 
+import numpy as np
 from darts.timeseries import TimeSeries
 from sklearn.gaussian_process import GaussianProcessRegressor
 from sklearn.gaussian_process.kernels import Kernel
 
-from .filtering_model import FilteringModel
 from ..utils.utils import raise_if_not
+from .filtering_model import FilteringModel
 
 
 class GaussianProcessFilter(FilteringModel):
     def __init__(self,
                  kernel: Optional[Kernel] = None,
                  **kwargs):
         """ GaussianProcessFilter model
@@ -51,18 +52,23 @@
             A stochastic `TimeSeries` sampled from the Gaussian Process, or its mean
             if `num_samples` is set to 1.
         """
         raise_if_not(series.is_deterministic, 'The input series for the Gaussian Process filter must be '
                                               'deterministic (observations).')
         super().filter(series)
 
-        times = series.time_index.values.reshape(-1, 1)
         values = series.values(copy=False)
+        if series.has_datetime_index:
+            times = np.arange(series.n_timesteps).reshape(-1, 1)
+        else:
+            times = series.time_index.values.reshape(-1, 1)
+
+        not_nan_mask = np.all(~np.isnan(values), axis=1)
 
-        self.model.fit(times, values)
+        self.model.fit(times[not_nan_mask, :], values[not_nan_mask, :])
 
         if num_samples == 1:
-            sampled_states = self.model.predict(times)
+            filtered_values = self.model.predict(times)
         else:
-            sampled_states = self.model.sample_y(times, n_samples=num_samples)
+            filtered_values = self.model.sample_y(times, n_samples=num_samples)
         
-        return TimeSeries.from_times_and_values(series.time_index, sampled_states)
+        return TimeSeries.from_times_and_values(series.time_index, filtered_values)
```

### Comparing `darts-0.9.0/darts/models/kalman_filter.py` & `darts-0.9.1/darts/models/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/models/linear_regression_model.py` & `darts-0.9.1/darts/models/linear_regression_model.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/models/nbeats.py` & `darts-0.9.1/darts/models/nbeats.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/models/prophet.py` & `darts-0.9.1/darts/models/prophet.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Optional
 import logging
 
 from ..timeseries import TimeSeries
 from .forecasting_model import ForecastingModel
 import pandas as pd
 from ..logging import get_logger, execute_and_suppress_output
-import fbprophet
+import prophet
 
 
 logger = get_logger(__name__)
 logger.level = logging.WARNING  # set to warning to suppress prophet logs
 
 
 class Prophet(ForecastingModel):
@@ -39,15 +39,15 @@
             In addition to those countries, Prophet includes holidays for these
             countries: Brazil (BR), Indonesia (ID), India (IN), Malaysia (MY), Vietnam (VN),
             Thailand (TH), Philippines (PH), Turkey (TU), Pakistan (PK), Bangladesh (BD),
             Egypt (EG), China (CN), and Russia (RU).
         prophet_kwargs
             Some optional keyword arguments for Prophet.
             For information about the parameters see:
-            `The Prophet source code <https://github.com/facebook/prophet/blob/master/python/fbprophet/forecaster.py>`_.
+            `The Prophet source code <https://github.com/facebook/prophet/blob/master/python/prophet/forecaster.py>`_.
 
         """
 
         super().__init__()
 
         self.country_holidays = country_holidays
         self.freq = frequency
@@ -63,15 +63,15 @@
 
         in_df = pd.DataFrame(data={
             'ds': series.time_index,
             'y': series.univariate_values()
         })
 
         # TODO: user-provided seasonalities, or "auto" based on stepduration
-        self.model = fbprophet.Prophet(**self.prophet_kwargs)
+        self.model = prophet.Prophet(**self.prophet_kwargs)
         if self.freq is not None:
             if series.freq_str in ['MS', 'M', 'ME']:
                 interval_length = 30.4375
             elif series.freq_str == 'Y':
                 interval_length = 365.25
             else:
                 interval_length = pd.to_timedelta(series.freq_str).days
```

### Comparing `darts-0.9.0/darts/models/random_forest.py` & `darts-0.9.1/darts/models/random_forest.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/models/regression_ensemble_model.py` & `darts-0.9.1/darts/models/regression_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/models/regression_model.py` & `darts-0.9.1/darts/models/regression_model.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/models/rnn_model.py` & `darts-0.9.1/darts/models/rnn_model.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/models/tcn_model.py` & `darts-0.9.1/darts/models/tcn_model.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/models/theta.py` & `darts-0.9.1/darts/models/theta.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/models/torch_forecasting_model.py` & `darts-0.9.1/darts/models/torch_forecasting_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
 
         self.input_chunk_length = input_chunk_length
         self.output_chunk_length = output_chunk_length
         self.log_tensorboard = log_tensorboard
         self.nr_epochs_val_period = nr_epochs_val_period
 
         if model_name is None:
-            current_time = datetime.datetime.now().strftime("%Y-%m-%d_%H:%M:%S.%f")
+            current_time = datetime.datetime.now().strftime("%Y-%m-%d_%H.%M.%S.%f")
             model_name = current_time + "_torch_model_run_" + str(os.getpid())
 
         self.model_name = model_name
         self.work_dir = work_dir
 
         self.n_epochs = n_epochs
         self.total_epochs = 0  # 0 means it wasn't trained yet.
@@ -607,15 +607,15 @@
                                  drop_last=False)
         predictions = []
         iterator = _build_tqdm_iterator(pred_loader, verbose=verbose)
         with torch.no_grad():
             for batch_tuple in iterator:
 
                 # at this point `input_series` contains both the past target series and past covariates
-                input_series = batch_tuple[0]
+                input_series = batch_tuple[0].to(self.device)
                 cov_future = batch_tuple[1] if len(batch_tuple) == 3 else None
 
                 # repeat prediction procedure for every needed sample
                 batch_predictions = []
                 for i in range(num_samples):
                     if self.is_recurrent:
                         batch_prediction = self._predict_batch_recurrent_model(n, input_series, cov_future)
```

### Comparing `darts-0.9.0/darts/models/transformer_model.py` & `darts-0.9.1/darts/models/transformer_model.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/models/varima.py` & `darts-0.9.1/darts/models/varima.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/base_test_class.py` & `darts-0.9.1/darts/tests/base_test_class.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/dataprocessing/test_pipeline.py` & `darts-0.9.1/darts/tests/dataprocessing/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/dataprocessing/transformers/test_base_data_transformer.py` & `darts-0.9.1/darts/tests/dataprocessing/transformers/test_base_data_transformer.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/dataprocessing/transformers/test_boxcox.py` & `darts-0.9.1/darts/tests/dataprocessing/transformers/test_boxcox.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/dataprocessing/transformers/test_data_transformer.py` & `darts-0.9.1/darts/tests/dataprocessing/transformers/test_data_transformer.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/dataprocessing/transformers/test_mappers.py` & `darts-0.9.1/darts/tests/dataprocessing/transformers/test_mappers.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/dataprocessing/transformers/test_missing_values_filler.py` & `darts-0.9.1/darts/tests/dataprocessing/transformers/test_missing_values_filler.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/test_4theta.py` & `darts-0.9.1/darts/tests/test_4theta.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/test_NBEATS.py` & `darts-0.9.1/darts/tests/test_NBEATS.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/test_TCN.py` & `darts-0.9.1/darts/tests/test_TCN.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/test_backtesting.py` & `darts-0.9.1/darts/tests/test_backtesting.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,21 +74,27 @@
 
     return expanding_window_ok and split_ok
 
 
 class BacktestingTestCase(DartsBaseTestClass):
     def test_backtest_forecasting(self):
         linear_series = lt(length=50)
+        linear_series_int = TimeSeries.from_values(linear_series.values())
         linear_series_multi = linear_series.stack(linear_series)
 
         # univariate model + univariate series
         score = NaiveDrift().backtest(linear_series, start=pd.Timestamp('20000201'),
                                       forecast_horizon=3, metric=r2_score)
         self.assertEqual(score, 1.0)
 
+        # test that it also works for time series that are not Datetime-indexed
+        score = NaiveDrift().backtest(linear_series_int, start=0.7,
+                                      forecast_horizon=3, metric=r2_score)
+        self.assertEqual(score, 1.0)
+
         with self.assertRaises(ValueError):
             NaiveDrift().backtest(linear_series, start=pd.Timestamp('20000217'), forecast_horizon=3)
         with self.assertRaises(ValueError):
             NaiveDrift().backtest(linear_series, start=pd.Timestamp('20000217'), forecast_horizon=3,
                                   overlap_end=False)
         NaiveDrift().backtest(linear_series, start=pd.Timestamp('20000216'), forecast_horizon=3)
         NaiveDrift().backtest(linear_series,
@@ -210,17 +216,19 @@
     def test_gridsearch(self):
         np.random.seed(1)
 
         ts_length = 50
         dummy_series = (
             lt(length=ts_length, end_value=10) + st(length=ts_length, value_y_offset=10) + rt(length=ts_length)
         )
+        dummy_series_int_index = TimeSeries.from_values(dummy_series.values())
 
         theta_params = {'theta': list(range(3, 10))}
         self.assertTrue(compare_best_against_random(Theta, theta_params, dummy_series))
+        self.assertTrue(compare_best_against_random(Theta, theta_params, dummy_series_int_index))
 
         fft_params = {'nr_freqs_to_keep': [10, 50, 100], 'trend': [None, 'poly', 'exp']}
         self.assertTrue(compare_best_against_random(FFT, fft_params, dummy_series))
 
         es_params = {'seasonal_periods': list(range(5, 10))}
         self.assertTrue(compare_best_against_random(ExponentialSmoothing, es_params, dummy_series))
```

### Comparing `darts-0.9.0/darts/tests/test_block_RNN.py` & `darts-0.9.1/darts/tests/test_block_RNN.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/test_dataset_loaders.py` & `darts-0.9.1/darts/tests/test_dataset_loaders.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/test_datasets.py` & `darts-0.9.1/darts/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/test_ensemble_models.py` & `darts-0.9.1/darts/tests/test_ensemble_models.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/test_fft.py` & `darts-0.9.1/darts/tests/test_fft.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/test_global_forecasting_models.py` & `darts-0.9.1/darts/tests/test_global_forecasting_models.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/test_local_forecasting_models.py` & `darts-0.9.1/darts/tests/test_local_forecasting_models.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/test_logging.py` & `darts-0.9.1/darts/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/test_metrics.py` & `darts-0.9.1/darts/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/test_missing_values.py` & `darts-0.9.1/darts/tests/test_missing_values.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/test_probabilistic_models.py` & `darts-0.9.1/darts/tests/test_probabilistic_models.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/test_regression_ensemble_model.py` & `darts-0.9.1/darts/tests/test_regression_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/test_regression_models.py` & `darts-0.9.1/darts/tests/test_regression_models.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/test_statistics.py` & `darts-0.9.1/darts/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/test_timeseries.py` & `darts-0.9.1/darts/tests/test_timeseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .base_test_class import DartsBaseTestClass
 from ..timeseries import TimeSeries
 from ..utils.timeseries_generation import linear_timeseries, constant_timeseries
 
 
 class TimeSeriesTestCase(DartsBaseTestClass):
 
-    times = pd.date_range('20130101', '20130110')
+    times = pd.date_range('20130101', '20130110', freq='D')
     pd_series1 = pd.Series(range(10), index=times)
     pd_series2 = pd.Series(range(5, 15), index=times)
     pd_series3 = pd.Series(range(15, 25), index=times)
     series1: TimeSeries = TimeSeries.from_series(pd_series1)
     series2: TimeSeries = TimeSeries.from_series(pd_series2)
     series3: TimeSeries = TimeSeries.from_series(pd_series2)
 
@@ -53,14 +53,29 @@
 
         # creation using from_xarray()
         ar = xr.DataArray(np.random.randn(10, 2, 1),
                           dims=('time', 'component', 'sample'), coords={'time': self.times, 'component': ['a', 'b']},
                           name='time series')
         _ = TimeSeries.from_xarray(ar)
 
+    def test_integer_indexing(self):
+        # sanity checks for the integer-indexed series
+        range_indexed_data = np.random.randn(50, )
+        series_int: TimeSeries = TimeSeries.from_values(range_indexed_data)
+
+        self.assertTrue(series_int[0].values().item() == range_indexed_data[0])
+        self.assertTrue(series_int[10].values().item() == range_indexed_data[10])
+
+        self.assertTrue(np.all(series_int[10:20].univariate_values() == range_indexed_data[10:20]))
+        self.assertTrue(np.all(series_int[10:].univariate_values() == range_indexed_data[10:]))
+
+        self.assertTrue(
+            np.all(series_int[pd.RangeIndex(start=10, stop=40, step=1)].univariate_values() == range_indexed_data[10:40])
+        )
+
     def test_column_names(self):
         # test the column names resolution
         columns_before = [
             ['0', '1', '2'],
             ['v', 'v', 'x'],
             ['v', 'v', 'x', 'v'],
             ['0', '0_1', '0'],
@@ -88,17 +103,18 @@
 
         for q in [0.01, 0.1, 0.5, 0.95]:
             q_ts = ts.quantile_timeseries(quantile=q)
             self.assertTrue((abs(q_ts.values() - np.quantile(values, q=q, axis=2)) < 1e-3).all())
 
     def test_alt_creation(self):
         with self.assertRaises(ValueError):
-            # Series cannot be lower than three without passing frequency as argument to constructor
+            # Series cannot be lower than three without passing frequency as argument to constructor,
+            # if fill_missing_dates is True (otherwise it works)
             index = pd.date_range('20130101', '20130102')
-            TimeSeries.from_times_and_values(index, self.pd_series1.values[:2])
+            TimeSeries.from_times_and_values(index, self.pd_series1.values[:2], fill_missing_dates=True)
         with self.assertRaises(ValueError):
             # all arrays must have same length
             TimeSeries.from_times_and_values(self.pd_series1.index,
                                              self.pd_series1.values[:-1])
 
         # test if reordering is correct
         rand_perm = np.random.permutation(range(1, 11))
@@ -397,23 +413,23 @@
             # Series cannot have date holes without automatic filling
             range_ = pd.date_range('20130101', '20130104').append(pd.date_range('20130106', '20130110'))
             TimeSeries.from_series(pd.Series(range(9), index=range_), fill_missing_dates=False)
 
         with self.assertRaises(ValueError):
             # Main series should have explicit frequency in case of date holes
             range_ = pd.date_range('20130101', '20130104').append(pd.date_range('20130106', '20130110', freq='2D'))
-            TimeSeries.from_series(pd.Series(range(7), index=range_))
+            TimeSeries.from_series(pd.Series(range(7), index=range_), fill_missing_dates=True)
 
         range_ = pd.date_range('20130101', '20130104').append(pd.date_range('20130106', '20130110'))
-        series_test = TimeSeries.from_series(pd.Series(range(9), index=range_))
+        series_test = TimeSeries.from_series(pd.Series(range(9), index=range_), fill_missing_dates=True)
         self.assertEqual(series_test.freq_str, 'D')
 
         range_ = pd.date_range('20130101', '20130104', freq='2D') \
             .append(pd.date_range('20130107', '20130111', freq='2D'))
-        series_test = TimeSeries.from_series(pd.Series(range(5), index=range_))
+        series_test = TimeSeries.from_series(pd.Series(range(5), index=range_), fill_missing_dates=True)
         self.assertEqual(series_test.freq_str, '2D')
         self.assertEqual(series_test.start_time(), range_[0])
         self.assertEqual(series_test.end_time(), range_[-1])
         self.assertTrue(math.isnan(series_test.pd_series().get('20130105')))
 
     def test_resample_timeseries(self):
         times = pd.date_range('20130101', '20130110')
@@ -431,17 +447,18 @@
         self.assertEqual(resampled_timeseries.pd_series().at[pd.Timestamp('20130101')], 0)
         with self.assertRaises(KeyError):
             resampled_timeseries.pd_series().at[pd.Timestamp('20130102')]
 
         self.assertEqual(resampled_timeseries.pd_series().at[pd.Timestamp('20130109')], 8)
 
     def test_short_series_creation(self):
-        # test missing freq argument error
+        # test missing freq argument error when filling missing dates on short time series
         with self.assertRaises(ValueError):
-            TimeSeries.from_times_and_values(pd.date_range('20130101', '20130102'), range(2))
+            TimeSeries.from_times_and_values(pd.date_range('20130101', '20130102'), range(2),
+                                             fill_missing_dates=True)
         # test empty pandas series error
         with self.assertRaises(ValueError):
             TimeSeries.from_series(pd.Series(), freq='D')
         # frequency should be ignored when fill_missing_dates is False
         seriesA = TimeSeries.from_times_and_values(pd.date_range('20130101', '20130105'),
                                                    range(5),
                                                    fill_missing_dates=False,
```

### Comparing `darts-0.9.0/darts/tests/test_timeseries_generation.py` & `darts-0.9.1/darts/tests/test_timeseries_generation.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/test_timeseries_multivariate.py` & `darts-0.9.1/darts/tests/test_timeseries_multivariate.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/test_torch_forecasting_model.py` & `darts-0.9.1/darts/tests/test_torch_forecasting_model.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/test_transformer_model.py` & `darts-0.9.1/darts/tests/test_transformer_model.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/test_utils.py` & `darts-0.9.1/darts/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/test_utils_torch.py` & `darts-0.9.1/darts/tests/test_utils_torch.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/tests/utils/test_model_selection.py` & `darts-0.9.1/darts/tests/utils/test_model_selection.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/timeseries.py` & `darts-0.9.1/darts/timeseries.py`

 * *Files 3% similar despite different names*

```diff
@@ -185,5131 +185,5340 @@
 00000b80: 6f6d 706f 6e65 6e74 7329 2c0a 2020 2020  omponents),.    
 00000b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000ba0: 206c 6f67 6765 7229 0a0a 2020 2020 2020   logger)..      
 00000bb0: 2020 7365 6c66 2e5f 7469 6d65 5f64 696d    self._time_dim
 00000bc0: 203d 2078 612e 6469 6d73 5b30 5d20 2023   = xa.dims[0]  #
 00000bd0: 2068 6f77 2074 6865 2074 696d 6520 6469   how the time di
 00000be0: 6d65 6e73 696f 6e20 6973 206e 616d 6564  mension is named
-00000bf0: 0a0a 2020 2020 2020 2020 6966 2069 7369  ..        if isi
-00000c00: 6e73 7461 6e63 6528 7861 2e67 6574 5f69  nstance(xa.get_i
-00000c10: 6e64 6578 2873 656c 662e 5f74 696d 655f  ndex(self._time_
-00000c20: 6469 6d29 2c20 7064 2e44 6174 6574 696d  dim), pd.Datetim
-00000c30: 6549 6e64 6578 293a 0a20 2020 2020 2020  eIndex):.       
-00000c40: 2020 2020 2023 2057 6520 6f6e 6c79 2073       # We only s
-00000c50: 6f72 7420 7468 6520 7861 7272 6179 2069  ort the xarray i
-00000c60: 6620 6974 2773 2069 6e64 6578 6564 2062  f it's indexed b
-00000c70: 7920 7469 6d65 2e20 5468 6174 2069 7320  y time. That is 
-00000c80: 6265 6361 7573 6520 736f 7274 696e 6720  because sorting 
-00000c90: 7769 7468 2061 2052 616e 6765 496e 6465  with a RangeInde
-00000ca0: 780a 2020 2020 2020 2020 2020 2020 2320  x.            # 
-00000cb0: 7472 616e 7366 6f72 6d73 2074 6865 2052  transforms the R
-00000cc0: 616e 6765 496e 6465 7820 696e 746f 2049  angeIndex into I
-00000cd0: 6e74 3634 496e 6465 782c 2077 6869 6368  nt64Index, which
-00000ce0: 206d 6573 7365 7320 7570 2074 6869 6e67   messes up thing
-00000cf0: 7320 6166 7465 7277 6172 6473 2e0a 0a20  s afterwards... 
-00000d00: 2020 2020 2020 2020 2020 2023 2054 6865             # The
-00000d10: 2066 6f6c 6c6f 7769 6e67 2073 6f72 7469   following sorti
-00000d20: 6e67 2072 6574 7572 6e73 2061 2063 6f70  ng returns a cop
-00000d30: 792c 2077 6869 6368 2077 6520 6172 6520  y, which we are 
-00000d40: 7265 6c79 696e 6720 6f6e 2e0a 0a20 2020  relying on...   
-00000d50: 2020 2020 2020 2020 2023 2041 7320 6f66           # As of
-00000d60: 2078 6172 7261 7920 302e 3138 2e32 2c20   xarray 0.18.2, 
-00000d70: 7468 6973 2073 6f72 7469 6e67 2064 6973  this sorting dis
-00000d80: 6361 7264 7320 7468 6520 6672 6571 206f  cards the freq o
-00000d90: 6620 7468 6520 696e 6465 7820 666f 7220  f the index for 
-00000da0: 736f 6d65 2072 6561 736f 6e0a 2020 2020  some reason.    
-00000db0: 2020 2020 2020 2020 2320 6874 7470 733a          # https:
-00000dc0: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7964  //github.com/pyd
-00000dd0: 6174 612f 7861 7272 6179 2f69 7373 7565  ata/xarray/issue
-00000de0: 732f 3534 3636 0a20 2020 2020 2020 2020  s/5466.         
-00000df0: 2020 2073 656c 662e 5f78 613a 2078 722e     self._xa: xr.
-00000e00: 4461 7461 4172 7261 7920 3d20 7861 2e73  DataArray = xa.s
-00000e10: 6f72 7462 7928 7365 6c66 2e5f 7469 6d65  ortby(self._time
-00000e20: 5f64 696d 290a 2020 2020 2020 2020 656c  _dim).        el
-00000e30: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00000e40: 7365 6c66 2e5f 7861 203d 2078 612e 636f  self._xa = xa.co
-00000e50: 7079 2829 0a0a 2020 2020 2020 2020 7365  py()..        se
-00000e60: 6c66 2e5f 7469 6d65 5f69 6e64 6578 203d  lf._time_index =
-00000e70: 2073 656c 662e 5f78 612e 6765 745f 696e   self._xa.get_in
-00000e80: 6465 7828 7365 6c66 2e5f 7469 6d65 5f64  dex(self._time_d
-00000e90: 696d 290a 0a20 2020 2020 2020 2069 6620  im)..        if 
-00000ea0: 6e6f 7420 6973 696e 7374 616e 6365 2873  not isinstance(s
-00000eb0: 656c 662e 5f74 696d 655f 696e 6465 782c  elf._time_index,
-00000ec0: 2070 642e 4461 7465 7469 6d65 496e 6465   pd.DatetimeInde
-00000ed0: 7829 2061 6e64 206e 6f74 2069 7369 6e73  x) and not isins
-00000ee0: 7461 6e63 6528 7365 6c66 2e5f 7469 6d65  tance(self._time
-00000ef0: 5f69 6e64 6578 2c20 7064 2e52 616e 6765  _index, pd.Range
-00000f00: 496e 6465 7829 3a0a 2020 2020 2020 2020  Index):.        
-00000f10: 2020 2020 7261 6973 655f 6c6f 6728 5661      raise_log(Va
-00000f20: 6c75 6545 7272 6f72 2827 5468 6520 7469  lueError('The ti
-00000f30: 6d65 2064 696d 656e 7369 6f6e 206f 6620  me dimension of 
-00000f40: 7468 6520 4461 7461 4172 7261 7920 6d75  the DataArray mu
-00000f50: 7374 2062 6520 696e 6465 7865 6420 6569  st be indexed ei
-00000f60: 7468 6572 2077 6974 6820 6120 4461 7465  ther with a Date
-00000f70: 7469 6d65 496e 6465 782c 270a 2020 2020  timeIndex,'.    
-00000f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f90: 2020 2020 2020 2020 2020 2020 2027 6f72               'or
-00000fa0: 2077 6974 6820 6120 5261 6e67 6549 6e64   with a RangeInd
-00000fb0: 6578 2e27 292c 206c 6f67 6765 7229 0a0a  ex.'), logger)..
-00000fc0: 2020 2020 2020 2020 7365 6c66 2e5f 6861          self._ha
-00000fd0: 735f 6461 7465 7469 6d65 5f69 6e64 6578  s_datetime_index
-00000fe0: 203d 2069 7369 6e73 7461 6e63 6528 7365   = isinstance(se
-00000ff0: 6c66 2e5f 7469 6d65 5f69 6e64 6578 2c20  lf._time_index, 
-00001000: 7064 2e44 6174 6574 696d 6549 6e64 6578  pd.DatetimeIndex
-00001010: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
-00001020: 6c66 2e5f 6861 735f 6461 7465 7469 6d65  lf._has_datetime
-00001030: 5f69 6e64 6578 3a0a 2020 2020 2020 2020  _index:.        
-00001040: 2020 2020 6672 6571 5f74 6d70 203d 2078      freq_tmp = x
-00001050: 612e 6765 745f 696e 6465 7828 7365 6c66  a.get_index(self
-00001060: 2e5f 7469 6d65 5f64 696d 292e 6672 6571  ._time_dim).freq
-00001070: 2020 2320 7374 6f72 6520 6f72 6967 696e    # store origin
-00001080: 616c 2066 7265 7120 2873 6565 2062 7567  al freq (see bug
-00001090: 206f 6620 736f 7274 6279 2829 2061 626f   of sortby() abo
-000010a0: 7665 292e 0a20 2020 2020 2020 2020 2020  ve)..           
-000010b0: 2073 656c 662e 5f66 7265 713a 2070 642e   self._freq: pd.
-000010c0: 4461 7465 4f66 6673 6574 203d 2066 7265  DateOffset = fre
-000010d0: 715f 746d 700a 2020 2020 2020 2020 2020  q_tmp.          
-000010e0: 2020 7261 6973 655f 6966 2873 656c 662e    raise_if(self.
-000010f0: 5f66 7265 7120 6973 204e 6f6e 652c 0a20  _freq is None,. 
-00001100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001110: 2020 2020 2754 6865 2074 696d 6520 696e      'The time in
-00001120: 6465 7820 6f66 2074 6865 2070 726f 7669  dex of the provi
-00001130: 6465 6420 4461 7461 4172 7261 7920 6973  ded DataArray is
-00001140: 206d 6973 7369 6e67 2074 6865 2066 7265   missing the fre
-00001150: 7120 6174 7472 6962 7574 652e 272c 0a20  q attribute.',. 
-00001160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001170: 2020 2020 6c6f 6767 6572 290a 0a20 2020      logger)..   
-00001180: 2020 2020 2020 2020 2073 656c 662e 5f66           self._f
-00001190: 7265 715f 7374 723a 2073 7472 203d 2073  req_str: str = s
-000011a0: 656c 662e 5f66 7265 712e 6672 6571 7374  elf._freq.freqst
-000011b0: 720a 0a20 2020 2020 2020 2020 2020 2023  r..            #
-000011c0: 2072 6573 6574 2066 7265 7120 696e 7369   reset freq insi
-000011d0: 6465 2074 6865 2078 6172 7261 7920 696e  de the xarray in
-000011e0: 6465 7820 2873 6565 2062 7567 206f 6620  dex (see bug of 
-000011f0: 736f 7274 6279 2829 2061 626f 7665 292e  sortby() above).
-00001200: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00001210: 662e 5f78 612e 6765 745f 696e 6465 7828  f._xa.get_index(
-00001220: 7365 6c66 2e5f 7469 6d65 5f64 696d 292e  self._time_dim).
-00001230: 6672 6571 203d 2066 7265 715f 746d 700a  freq = freq_tmp.
-00001240: 0a20 2020 2020 2020 2020 2020 2023 2057  .            # W
-00001250: 6520 6861 7665 2074 6f20 6368 6563 6b20  e have to check 
-00001260: 6d61 6e75 616c 6c79 2069 6620 7468 6520  manually if the 
-00001270: 696e 6465 7820 6973 2063 6f6d 706c 6574  index is complet
-00001280: 652e 2041 6e6f 7468 6572 2077 6179 2063  e. Another way c
-00001290: 6f75 6c64 2062 6520 746f 2072 656c 790a  ould be to rely.
-000012a0: 2020 2020 2020 2020 2020 2020 2320 6f6e              # on
-000012b0: 2060 696e 6665 7272 6564 5f66 7265 7160   `inferred_freq`
-000012c0: 2062 6569 6e67 2070 7265 7365 6e74 2c20   being present, 
-000012d0: 6275 7420 7468 6973 2066 6169 6c73 2066  but this fails f
-000012e0: 6f72 2073 6572 6965 7320 6f66 206c 656e  or series of len
-000012f0: 6774 6820 3c20 332e 0a20 2020 2020 2020  gth < 3..       
-00001300: 2020 2020 2069 735f 696e 6465 785f 636f       is_index_co
-00001310: 6d70 6c65 7465 203d 206c 656e 2870 642e  mplete = len(pd.
-00001320: 6461 7465 5f72 616e 6765 2873 656c 662e  date_range(self.
-00001330: 5f74 696d 655f 696e 6465 782e 6d69 6e28  _time_index.min(
-00001340: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00001350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001370: 2020 2020 2073 656c 662e 5f74 696d 655f       self._time_
-00001380: 696e 6465 782e 6d61 7828 292c 0a20 2020  index.max(),.   
-00001390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000013c0: 7265 713d 7365 6c66 2e5f 6672 6571 292e  req=self._freq).
-000013d0: 6469 6666 6572 656e 6365 2873 656c 662e  difference(self.
-000013e0: 5f74 696d 655f 696e 6465 7829 2920 3d3d  _time_index)) ==
-000013f0: 2030 0a0a 2020 2020 2020 2020 2020 2020   0..            
-00001400: 7261 6973 655f 6966 5f6e 6f74 2869 735f  raise_if_not(is_
-00001410: 696e 6465 785f 636f 6d70 6c65 7465 2c20  index_complete, 
-00001420: 274e 6f74 2061 6c6c 2074 696d 6573 7461  'Not all timesta
-00001430: 6d70 7320 7365 656d 2074 6f20 6265 2070  mps seem to be p
-00001440: 7265 7365 6e74 2069 6e20 7468 6520 7469  resent in the ti
-00001450: 6d65 2069 6e64 6578 2e20 446f 6573 2027  me index. Does '
-00001460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000bf0: 0a0a 2020 2020 2020 2020 2320 5468 6520  ..        # The 
+00000c00: 666f 6c6c 6f77 696e 6720 736f 7274 696e  following sortin
+00000c10: 6720 7265 7475 726e 7320 6120 636f 7079  g returns a copy
+00000c20: 2c20 7768 6963 6820 7765 2061 7265 2072  , which we are r
+00000c30: 656c 7969 6e67 206f 6e2e 0a20 2020 2020  elying on..     
+00000c40: 2020 2023 2041 7320 6f66 2078 6172 7261     # As of xarra
+00000c50: 7920 302e 3138 2e32 2c20 7468 6973 2073  y 0.18.2, this s
+00000c60: 6f72 7469 6e67 2064 6973 6361 7264 7320  orting discards 
+00000c70: 7468 6520 6672 6571 206f 6620 7468 6520  the freq of the 
+00000c80: 696e 6465 7820 666f 7220 736f 6d65 2072  index for some r
+00000c90: 6561 736f 6e0a 2020 2020 2020 2020 2320  eason.        # 
+00000ca0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000cb0: 6f6d 2f70 7964 6174 612f 7861 7272 6179  om/pydata/xarray
+00000cc0: 2f69 7373 7565 732f 3534 3636 0a20 2020  /issues/5466.   
+00000cd0: 2020 2020 2073 656c 662e 5f78 613a 2078       self._xa: x
+00000ce0: 722e 4461 7461 4172 7261 7920 3d20 7861  r.DataArray = xa
+00000cf0: 2e73 6f72 7462 7928 7365 6c66 2e5f 7469  .sortby(self._ti
+00000d00: 6d65 5f64 696d 290a 0a20 2020 2020 2020  me_dim)..       
+00000d10: 2073 656c 662e 5f74 696d 655f 696e 6465   self._time_inde
+00000d20: 7820 3d20 7365 6c66 2e5f 7861 2e67 6574  x = self._xa.get
+00000d30: 5f69 6e64 6578 2873 656c 662e 5f74 696d  _index(self._tim
+00000d40: 655f 6469 6d29 0a0a 2020 2020 2020 2020  e_dim)..        
+00000d50: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+00000d60: 6528 7365 6c66 2e5f 7469 6d65 5f69 6e64  e(self._time_ind
+00000d70: 6578 2c20 7064 2e44 6174 6574 696d 6549  ex, pd.DatetimeI
+00000d80: 6e64 6578 2920 616e 6420 6e6f 7420 6973  ndex) and not is
+00000d90: 696e 7374 616e 6365 2873 656c 662e 5f74  instance(self._t
+00000da0: 696d 655f 696e 6465 782c 2070 642e 496e  ime_index, pd.In
+00000db0: 7436 3449 6e64 6578 293a 0a20 2020 2020  t64Index):.     
+00000dc0: 2020 2020 2020 2072 6169 7365 5f6c 6f67         raise_log
+00000dd0: 2856 616c 7565 4572 726f 7228 2754 6865  (ValueError('The
+00000de0: 2074 696d 6520 6469 6d65 6e73 696f 6e20   time dimension 
+00000df0: 6f66 2074 6865 2044 6174 6141 7272 6179  of the DataArray
+00000e00: 206d 7573 7420 6265 2069 6e64 6578 6564   must be indexed
+00000e10: 2065 6974 6865 7220 7769 7468 2061 2044   either with a D
+00000e20: 6174 6574 696d 6549 6e64 6578 2c27 0a20  atetimeIndex,'. 
+00000e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e50: 276f 7220 7769 7468 2061 6e20 496e 7436  'or with an Int6
+00000e60: 3449 6e64 6578 2028 7468 6973 2063 616e  4Index (this can
+00000e70: 2069 6e63 6c75 6465 2061 2052 616e 6765   include a Range
+00000e80: 496e 6465 7829 2e27 292c 206c 6f67 6765  Index).'), logge
+00000e90: 7229 0a0a 2020 2020 2020 2020 7365 6c66  r)..        self
+00000ea0: 2e5f 6861 735f 6461 7465 7469 6d65 5f69  ._has_datetime_i
+00000eb0: 6e64 6578 203d 2069 7369 6e73 7461 6e63  ndex = isinstanc
+00000ec0: 6528 7365 6c66 2e5f 7469 6d65 5f69 6e64  e(self._time_ind
+00000ed0: 6578 2c20 7064 2e44 6174 6574 696d 6549  ex, pd.DatetimeI
+00000ee0: 6e64 6578 290a 0a20 2020 2020 2020 2069  ndex)..        i
+00000ef0: 6620 7365 6c66 2e5f 6861 735f 6461 7465  f self._has_date
+00000f00: 7469 6d65 5f69 6e64 6578 3a0a 2020 2020  time_index:.    
+00000f10: 2020 2020 2020 2020 6672 6571 5f74 6d70          freq_tmp
+00000f20: 203d 2078 612e 6765 745f 696e 6465 7828   = xa.get_index(
+00000f30: 7365 6c66 2e5f 7469 6d65 5f64 696d 292e  self._time_dim).
+00000f40: 6672 6571 2020 2320 7374 6f72 6520 6f72  freq  # store or
+00000f50: 6967 696e 616c 2066 7265 7120 2873 6565  iginal freq (see
+00000f60: 2062 7567 206f 6620 736f 7274 6279 2829   bug of sortby()
+00000f70: 2061 626f 7665 292e 0a20 2020 2020 2020   above)..       
+00000f80: 2020 2020 2073 656c 662e 5f66 7265 713a       self._freq:
+00000f90: 2070 642e 4461 7465 4f66 6673 6574 203d   pd.DateOffset =
+00000fa0: 2028 6672 6571 5f74 6d70 2069 6620 6672   (freq_tmp if fr
+00000fb0: 6571 5f74 6d70 2069 7320 6e6f 7420 4e6f  eq_tmp is not No
+00000fc0: 6e65 2065 6c73 650a 2020 2020 2020 2020  ne else.        
+00000fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ff0: 2074 6f5f 6f66 6673 6574 2873 656c 662e   to_offset(self.
+00001000: 5f78 612e 6765 745f 696e 6465 7828 7365  _xa.get_index(se
+00001010: 6c66 2e5f 7469 6d65 5f64 696d 292e 696e  lf._time_dim).in
+00001020: 6665 7272 6564 5f66 7265 7129 290a 2020  ferred_freq)).  
+00001030: 2020 2020 2020 2020 2020 7261 6973 655f            raise_
+00001040: 6966 2873 656c 662e 5f66 7265 7120 6973  if(self._freq is
+00001050: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+00001060: 2020 2020 2020 2020 2020 2020 2754 6865              'The
+00001070: 2074 696d 6520 696e 6465 7820 6f66 2074   time index of t
+00001080: 6865 2070 726f 7669 6465 6420 4461 7461  he provided Data
+00001090: 4172 7261 7920 6973 206d 6973 7369 6e67  Array is missing
+000010a0: 2074 6865 2066 7265 7120 6174 7472 6962   the freq attrib
+000010b0: 7574 652c 2061 6e64 2074 6865 2027 0a20  ute, and the '. 
+000010c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010d0: 2020 2020 2766 7265 7175 656e 6379 2063      'frequency c
+000010e0: 616e 6e6f 7420 6265 2069 6e66 6572 7265  annot be inferre
+000010f0: 642e 272c 0a20 2020 2020 2020 2020 2020  d.',.           
+00001100: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00001110: 290a 0a20 2020 2020 2020 2020 2020 2073  )..            s
+00001120: 656c 662e 5f66 7265 715f 7374 723a 2073  elf._freq_str: s
+00001130: 7472 203d 2073 656c 662e 5f66 7265 712e  tr = self._freq.
+00001140: 6672 6571 7374 720a 0a20 2020 2020 2020  freqstr..       
+00001150: 2020 2020 2023 2072 6573 6574 2066 7265       # reset fre
+00001160: 7120 696e 7369 6465 2074 6865 2078 6172  q inside the xar
+00001170: 7261 7920 696e 6465 7820 2873 6565 2062  ray index (see b
+00001180: 7567 206f 6620 736f 7274 6279 2829 2061  ug of sortby() a
+00001190: 626f 7665 292e 0a20 2020 2020 2020 2020  bove)..         
+000011a0: 2020 2073 656c 662e 5f78 612e 6765 745f     self._xa.get_
+000011b0: 696e 6465 7828 7365 6c66 2e5f 7469 6d65  index(self._time
+000011c0: 5f64 696d 292e 6672 6571 203d 2073 656c  _dim).freq = sel
+000011d0: 662e 5f66 7265 710a 0a20 2020 2020 2020  f._freq..       
+000011e0: 2020 2020 2023 2057 6520 6861 7665 2074       # We have t
+000011f0: 6f20 6368 6563 6b20 6d61 6e75 616c 6c79  o check manually
+00001200: 2069 6620 7468 6520 696e 6465 7820 6973   if the index is
+00001210: 2063 6f6d 706c 6574 652e 2041 6e6f 7468   complete. Anoth
+00001220: 6572 2077 6179 2063 6f75 6c64 2062 6520  er way could be 
+00001230: 746f 2072 656c 790a 2020 2020 2020 2020  to rely.        
+00001240: 2020 2020 2320 6f6e 2060 696e 6665 7272      # on `inferr
+00001250: 6564 5f66 7265 7160 2062 6569 6e67 2070  ed_freq` being p
+00001260: 7265 7365 6e74 2c20 6275 7420 7468 6973  resent, but this
+00001270: 2066 6169 6c73 2066 6f72 2073 6572 6965   fails for serie
+00001280: 7320 6f66 206c 656e 6774 6820 3c20 332e  s of length < 3.
+00001290: 0a20 2020 2020 2020 2020 2020 2069 735f  .            is_
+000012a0: 696e 6465 785f 636f 6d70 6c65 7465 203d  index_complete =
+000012b0: 206c 656e 2870 642e 6461 7465 5f72 616e   len(pd.date_ran
+000012c0: 6765 2873 656c 662e 5f74 696d 655f 696e  ge(self._time_in
+000012d0: 6465 782e 6d69 6e28 292c 0a20 2020 2020  dex.min(),.     
+000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001300: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00001310: 662e 5f74 696d 655f 696e 6465 782e 6d61  f._time_index.ma
+00001320: 7828 292c 0a20 2020 2020 2020 2020 2020  x(),.           
+00001330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001350: 2020 2020 2020 2066 7265 713d 7365 6c66         freq=self
+00001360: 2e5f 6672 6571 292e 6469 6666 6572 656e  ._freq).differen
+00001370: 6365 2873 656c 662e 5f74 696d 655f 696e  ce(self._time_in
+00001380: 6465 7829 2920 3d3d 2030 0a0a 2020 2020  dex)) == 0..    
+00001390: 2020 2020 2020 2020 7261 6973 655f 6966          raise_if
+000013a0: 5f6e 6f74 2869 735f 696e 6465 785f 636f  _not(is_index_co
+000013b0: 6d70 6c65 7465 2c20 274e 6f74 2061 6c6c  mplete, 'Not all
+000013c0: 2074 696d 6573 7461 6d70 7320 7365 656d   timestamps seem
+000013d0: 2074 6f20 6265 2070 7265 7365 6e74 2069   to be present i
+000013e0: 6e20 7468 6520 7469 6d65 2069 6e64 6578  n the time index
+000013f0: 2e20 446f 6573 2027 0a20 2020 2020 2020  . Does '.       
+00001400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001420: 2020 2020 2027 7468 6520 7365 7269 6573       'the series
+00001430: 2063 6f6e 7461 696e 2068 6f6c 6573 3f20   contain holes? 
+00001440: 4966 2079 6f75 2061 7265 2075 7369 6e67  If you are using
+00001450: 2061 2066 6163 746f 7279 206d 6574 686f   a factory metho
+00001460: 642c 2027 0a20 2020 2020 2020 2020 2020  d, '.           
 00001470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001480: 2020 2020 2020 2020 2020 2020 2027 7468               'th
-00001490: 6520 7365 7269 6573 2063 6f6e 7461 696e  e series contain
-000014a0: 2068 6f6c 6573 3f20 4966 2079 6f75 2061   holes? If you a
-000014b0: 7265 2075 7369 6e67 2061 2063 6f6e 7374  re using a const
-000014c0: 7275 6374 6f72 206d 6574 686f 642c 2027  ructor method, '
-000014d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000014e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014f0: 2020 2020 2020 2020 2020 2020 2027 7472               'tr
-00001500: 7920 7370 6563 6966 7969 6e67 2060 6669  y specifying `fi
-00001510: 6c6c 5f6d 6973 7369 6e67 5f64 6174 6573  ll_missing_dates
-00001520: 3d54 7275 6560 2027 0a20 2020 2020 2020  =True` '.       
-00001530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001550: 2020 2020 2027 6f72 2073 7065 6369 6679       'or specify
-00001560: 2074 6865 2060 6672 6571 6020 7061 7261   the `freq` para
-00001570: 6d65 7465 722e 272c 206c 6f67 6765 7229  meter.', logger)
-00001580: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00001590: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000015a0: 5f66 7265 7120 3d20 310a 2020 2020 2020  _freq = 1.      
-000015b0: 2020 2020 2020 7365 6c66 2e5f 6672 6571        self._freq
-000015c0: 5f73 7472 203d 204e 6f6e 650a 0a20 2020  _str = None..   
-000015d0: 2022 2222 200a 2020 2020 4661 6374 6f72   """ .    Factor
-000015e0: 7920 4d65 7468 6f64 730a 2020 2020 3d3d  y Methods.    ==
-000015f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020  =============.  
-00001600: 2020 2222 220a 0a20 2020 2040 7374 6174    """..    @stat
-00001610: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
-00001620: 2066 726f 6d5f 7861 7272 6179 2878 613a   from_xarray(xa:
-00001630: 2078 722e 4461 7461 4172 7261 792c 0a20   xr.DataArray,. 
-00001640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001650: 2020 2066 696c 6c5f 6d69 7373 696e 675f     fill_missing_
-00001660: 6461 7465 733a 204f 7074 696f 6e61 6c5b  dates: Optional[
-00001670: 626f 6f6c 5d20 3d20 5472 7565 2c0a 2020  bool] = True,.  
-00001680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001690: 2020 6672 6571 3a20 4f70 7469 6f6e 616c    freq: Optional
-000016a0: 5b73 7472 5d20 3d20 4e6f 6e65 2920 2d3e  [str] = None) ->
-000016b0: 2027 5469 6d65 5365 7269 6573 273a 0a20   'TimeSeries':. 
-000016c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000016d0: 2020 2052 6574 7572 6e73 2061 2054 696d     Returns a Tim
-000016e0: 6553 6572 6965 7320 696e 7374 616e 6365  eSeries instance
-000016f0: 2062 7569 6c74 2066 726f 6d20 616e 2078   built from an x
-00001700: 6172 7261 7920 4461 7461 4172 7261 792e  array DataArray.
-00001710: 0a20 2020 2020 2020 2054 6865 2064 696d  .        The dim
-00001720: 656e 7369 6f6e 7320 6f66 2074 6865 2044  ensions of the D
-00001730: 6174 6141 7272 6179 2068 6176 6520 746f  ataArray have to
-00001740: 2062 6520 2874 696d 652c 2063 6f6d 706f   be (time, compo
-00001750: 6e65 6e74 2c20 7361 6d70 6c65 292c 2069  nent, sample), i
-00001760: 6e20 7468 6973 206f 7264 6572 2e20 5468  n this order. Th
-00001770: 6520 7469 6d65 0a20 2020 2020 2020 2064  e time.        d
-00001780: 696d 656e 7369 6f6e 2063 616e 2068 6176  imension can hav
-00001790: 6520 616e 2061 7262 6974 7261 7279 206e  e an arbitrary n
-000017a0: 616d 652c 2062 7574 2063 6f6d 706f 6e65  ame, but compone
-000017b0: 6e74 2061 6e64 2073 616d 706c 6520 6d75  nt and sample mu
-000017c0: 7374 2062 6520 6e61 6d65 6420 2263 6f6d  st be named "com
-000017d0: 706f 6e65 6e74 2220 616e 6420 2273 616d  ponent" and "sam
-000017e0: 706c 6522 2c0a 2020 2020 2020 2020 7265  ple",.        re
-000017f0: 7370 6563 7469 7665 6c79 2e0a 0a20 2020  spectively...   
-00001800: 2020 2020 2049 6620 7477 6f20 636f 6d70       If two comp
-00001810: 6f6e 656e 7473 2068 6176 6520 7468 6520  onents have the 
-00001820: 7361 6d65 206e 616d 6520 6f72 2061 7265  same name or are
-00001830: 206e 6f74 2073 7472 696e 6773 2c20 7468   not strings, th
-00001840: 6973 206d 6574 686f 6420 7769 6c6c 2064  is method will d
-00001850: 6973 616d 6269 6775 6174 6520 7468 6520  isambiguate the 
-00001860: 636f 6d70 6f6e 656e 7473 0a20 2020 2020  components.     
-00001870: 2020 206e 616d 6573 2062 7920 6170 7065     names by appe
-00001880: 6e64 696e 6720 6120 7375 6666 6978 206f  nding a suffix o
-00001890: 6620 7468 6520 666f 726d 2022 3c6e 616d  f the form "<nam
-000018a0: 653e 5f4e 2220 746f 2074 6865 204e 2d74  e>_N" to the N-t
-000018b0: 6820 636f 6c75 6d6e 2077 6974 6820 6e61  h column with na
-000018c0: 6d65 2022 6e61 6d65 222e 0a0a 2020 2020  me "name"...    
-000018d0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-000018e0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-000018f0: 2d0a 2020 2020 2020 2020 7861 0a20 2020  -.        xa.   
-00001900: 2020 2020 2020 2020 2054 6865 2078 6172           The xar
-00001910: 7261 7920 4461 7461 4172 7261 790a 2020  ray DataArray.  
-00001920: 2020 2020 2020 6669 6c6c 5f6d 6973 7369        fill_missi
-00001930: 6e67 5f64 6174 6573 0a20 2020 2020 2020  ng_dates.       
-00001940: 2020 2020 204f 7074 696f 6e61 6c6c 792c       Optionally,
-00001950: 2061 2062 6f6f 6c65 616e 2076 616c 7565   a boolean value
-00001960: 2069 6e64 6963 6174 696e 6720 7768 6574   indicating whet
-00001970: 6865 7220 746f 2066 696c 6c20 6d69 7373  her to fill miss
-00001980: 696e 6720 6461 7465 7320 7769 7468 204e  ing dates with N
-00001990: 614e 2076 616c 7565 732e 2054 6869 7320  aN values. This 
-000019a0: 7265 7175 6972 6573 0a20 2020 2020 2020  requires.       
-000019b0: 2020 2020 2065 6974 6865 7220 6120 7072       either a pr
-000019c0: 6f76 6964 6564 2060 6672 6571 6020 6f72  ovided `freq` or
-000019d0: 2074 6865 2070 6f73 7369 6269 6c69 7479   the possibility
-000019e0: 2074 6f20 696e 6665 7220 7468 6520 6672   to infer the fr
-000019f0: 6571 7565 6e63 7920 6672 6f6d 2074 6865  equency from the
-00001a00: 2070 726f 7669 6465 6420 7469 6d65 7374   provided timest
-00001a10: 616d 7073 2e0a 2020 2020 2020 2020 6672  amps..        fr
-00001a20: 6571 0a20 2020 2020 2020 2020 2020 204f  eq.            O
-00001a30: 7074 696f 6e61 6c6c 792c 2061 2073 7472  ptionally, a str
-00001a40: 696e 6720 7265 7072 6573 656e 7469 6e67  ing representing
-00001a50: 2074 6865 2066 7265 7175 656e 6379 206f   the frequency o
-00001a60: 6620 7468 6520 5061 6e64 6173 2044 6174  f the Pandas Dat
-00001a70: 6146 7261 6d65 2e20 5468 6973 2069 7320  aFrame. This is 
-00001a80: 7573 6566 756c 2069 6e20 6f72 6465 7220  useful in order 
-00001a90: 746f 2066 696c 6c0a 2020 2020 2020 2020  to fill.        
-00001aa0: 2020 2020 696e 206d 6973 7369 6e67 2076      in missing v
-00001ab0: 616c 7565 7320 6966 2073 6f6d 6520 6461  alues if some da
-00001ac0: 7465 7320 6172 6520 6d69 7373 696e 6720  tes are missing 
-00001ad0: 616e 6420 6066 696c 6c5f 6d69 7373 696e  and `fill_missin
-00001ae0: 675f 6461 7465 7360 2069 7320 7365 7420  g_dates` is set 
-00001af0: 746f 2060 5472 7565 602e 0a0a 2020 2020  to `True`...    
-00001b00: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00001b10: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00001b20: 2020 2020 5469 6d65 5365 7269 6573 0a20      TimeSeries. 
-00001b30: 2020 2020 2020 2020 2020 2041 2075 6e69             A uni
-00001b40: 7661 7269 6174 6520 6f72 206d 756c 7469  variate or multi
-00001b50: 7661 7269 6174 6520 6465 7465 726d 696e  variate determin
-00001b60: 6973 7469 6320 5469 6d65 5365 7269 6573  istic TimeSeries
-00001b70: 2063 6f6e 7374 7275 6374 6564 2066 726f   constructed fro
-00001b80: 6d20 7468 6520 696e 7075 7473 2e0a 2020  m the inputs..  
-00001b90: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-00001ba0: 2020 2023 206f 7074 696f 6e61 6c6c 7920     # optionally 
-00001bb0: 6669 6c6c 206d 6973 7369 6e67 2064 6174  fill missing dat
-00001bc0: 6573 3b20 646f 2069 7420 6f6e 6c79 2077  es; do it only w
-00001bd0: 6865 6e20 7468 6572 6520 6973 2061 2044  hen there is a D
-00001be0: 6174 6574 696d 6549 6e64 6578 2028 616e  atetimeIndex (an
-00001bf0: 6420 6e6f 7420 6120 5261 6e67 6549 6e64  d not a RangeInd
-00001c00: 6578 290a 2020 2020 2020 2020 6966 2066  ex).        if f
-00001c10: 696c 6c5f 6d69 7373 696e 675f 6461 7465  ill_missing_date
-00001c20: 7320 616e 6420 6973 696e 7374 616e 6365  s and isinstance
-00001c30: 2878 612e 6765 745f 696e 6465 7828 7861  (xa.get_index(xa
-00001c40: 2e64 696d 735b 305d 292c 2070 642e 4461  .dims[0]), pd.Da
-00001c50: 7465 7469 6d65 496e 6465 7829 3a0a 2020  tetimeIndex):.  
-00001c60: 2020 2020 2020 2020 2020 736f 7274 6564            sorted
-00001c70: 5f78 6120 3d20 7861 2e73 6f72 7462 7928  _xa = xa.sortby(
-00001c80: 7861 2e64 696d 735b 305d 290a 2020 2020  xa.dims[0]).    
-00001c90: 2020 2020 2020 2020 7469 6d65 5f69 6e64          time_ind
-00001ca0: 6578 203d 2073 6f72 7465 645f 7861 2e67  ex = sorted_xa.g
-00001cb0: 6574 5f69 6e64 6578 2878 612e 6469 6d73  et_index(xa.dims
-00001cc0: 5b30 5d29 0a0a 2020 2020 2020 2020 2020  [0])..          
-00001cd0: 2020 6966 206e 6f74 2066 7265 713a 0a20    if not freq:. 
-00001ce0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00001cf0: 616d 706c 6573 5f73 697a 6520 3d20 330a  amples_size = 3.
-00001d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d10: 6f62 7365 7276 6564 5f66 7265 7175 656e  observed_frequen
-00001d20: 6369 6573 203d 205b 0a20 2020 2020 2020  cies = [.       
-00001d30: 2020 2020 2020 2020 2020 2020 2074 696d               tim
-00001d40: 655f 696e 6465 785b 783a 7820 2b20 7361  e_index[x:x + sa
-00001d50: 6d70 6c65 735f 7369 7a65 5d2e 696e 6665  mples_size].infe
-00001d60: 7272 6564 5f66 7265 710a 2020 2020 2020  rred_freq.      
-00001d70: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00001d80: 7220 780a 2020 2020 2020 2020 2020 2020  r x.            
-00001d90: 2020 2020 2020 2020 696e 2072 616e 6765          in range
-00001da0: 286c 656e 2874 696d 655f 696e 6465 7829  (len(time_index)
-00001db0: 202d 2073 616d 706c 6573 5f73 697a 6520   - samples_size 
-00001dc0: 2b20 3129 5d0a 0a20 2020 2020 2020 2020  + 1)]..         
-00001dd0: 2020 2020 2020 206f 6273 6572 7665 645f         observed_
-00001de0: 6672 6571 7565 6e63 6965 7320 3d20 7365  frequencies = se
-00001df0: 7428 6669 6c74 6572 284e 6f6e 652e 5f5f  t(filter(None.__
-00001e00: 6e65 5f5f 2c20 6f62 7365 7276 6564 5f66  ne__, observed_f
-00001e10: 7265 7175 656e 6369 6573 2929 0a0a 2020  requencies))..  
-00001e20: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-00001e30: 6973 655f 6966 5f6e 6f74 280a 2020 2020  ise_if_not(.    
-00001e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e50: 6c65 6e28 6f62 7365 7276 6564 5f66 7265  len(observed_fre
-00001e60: 7175 656e 6369 6573 2920 3d3d 2031 2c0a  quencies) == 1,.
-00001e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e80: 2020 2020 2243 6f75 6c64 206e 6f74 2069      "Could not i
-00001e90: 6e66 6572 2065 7870 6c69 6369 7420 6672  nfer explicit fr
-00001ea0: 6571 7565 6e63 792e 204f 6273 6572 7665  equency. Observe
-00001eb0: 6420 6672 6571 7565 6e63 6965 733a 2022  d frequencies: "
-00001ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001ed0: 2020 2020 202b 2028 276e 6f6e 6527 2069       + ('none' i
-00001ee0: 6620 6c65 6e28 6f62 7365 7276 6564 5f66  f len(observed_f
-00001ef0: 7265 7175 656e 6369 6573 2920 3d3d 2030  requencies) == 0
-00001f00: 2065 6c73 6520 7374 7228 6f62 7365 7276   else str(observ
-00001f10: 6564 5f66 7265 7175 656e 6369 6573 2929  ed_frequencies))
-00001f20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001f30: 2020 2020 202b 2028 222e 2049 7320 5365       + (". Is Se
-00001f40: 7269 6573 2074 6f6f 2073 686f 7274 2028  ries too short (
-00001f50: 6e3d 7b7d 293f 222e 666f 726d 6174 2873  n={})?".format(s
-00001f60: 616d 706c 6573 5f73 697a 652d 3129 2069  amples_size-1) i
-00001f70: 6620 6c65 6e28 6f62 7365 7276 6564 5f66  f len(observed_f
-00001f80: 7265 7175 656e 6369 6573 2920 3d3d 2030  requencies) == 0
-00001f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001fa0: 2020 2020 2020 2020 656c 7365 2027 2e27          else '.'
-00001fb0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00001fc0: 2020 2020 2020 206c 6f67 6765 7229 0a0a         logger)..
-00001fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fe0: 6672 6571 203d 206f 6273 6572 7665 645f  freq = observed_
-00001ff0: 6672 6571 7565 6e63 6965 732e 706f 7028  frequencies.pop(
-00002000: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
-00002010: 2054 4f44 4f3a 2069 6620 7072 6f76 6964   TODO: if provid
-00002020: 6564 2066 7265 7120 646f 6573 6e27 7420  ed freq doesn't 
-00002030: 6d61 7463 6820 7468 6520 6672 6571 2069  match the freq i
-00002040: 6e20 696e 6465 7820 6569 7468 6572 2072  n index either r
-00002050: 6169 7365 2061 6e20 6572 726f 7220 6f72  aise an error or
-00002060: 2063 6f72 7265 6374 0a20 2020 2020 2020   correct.       
-00002070: 2020 2020 2078 615f 203d 2073 6f72 7465       xa_ = sorte
-00002080: 645f 7861 2e72 6573 616d 706c 6528 7b78  d_xa.resample({x
-00002090: 612e 6469 6d73 5b30 5d3a 2066 7265 717d  a.dims[0]: freq}
-000020a0: 292e 6173 6672 6571 2829 0a20 2020 2020  ).asfreq().     
-000020b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000020c0: 2020 2020 2078 615f 203d 2078 610a 0a20       xa_ = xa.. 
-000020d0: 2020 2020 2020 2023 2063 6c65 616e 2063         # clean c
-000020e0: 6f6d 706f 6e65 6e74 7320 2863 6f6c 756d  omponents (colum
-000020f0: 6e73 2920 6e61 6d65 7320 6966 206e 6565  ns) names if nee
-00002100: 6465 6420 2869 6620 6e61 6d65 7320 6172  ded (if names ar
-00002110: 6520 6e6f 7420 756e 6971 7565 2c20 6f72  e not unique, or
-00002120: 206e 6f74 2073 7472 696e 6773 290a 2020   not strings).  
-00002130: 2020 2020 2020 636f 6d70 6f6e 656e 7473        components
-00002140: 203d 2078 615f 2e67 6574 5f69 6e64 6578   = xa_.get_index
-00002150: 2844 494d 535b 315d 290a 2020 2020 2020  (DIMS[1]).      
-00002160: 2020 6966 206c 656e 2873 6574 2863 6f6d    if len(set(com
-00002170: 706f 6e65 6e74 7329 2920 213d 206c 656e  ponents)) != len
-00002180: 2863 6f6d 706f 6e65 6e74 7329 206f 7220  (components) or 
-00002190: 616e 7928 5b6e 6f74 2069 7369 6e73 7461  any([not isinsta
-000021a0: 6e63 6528 732c 2073 7472 2920 666f 7220  nce(s, str) for 
-000021b0: 7320 696e 2063 6f6d 706f 6e65 6e74 735d  s in components]
-000021c0: 293a 0a0a 2020 2020 2020 2020 2020 2020  ):..            
-000021d0: 6465 6620 5f63 6c65 616e 5f63 6f6d 706f  def _clean_compo
-000021e0: 6e65 6e74 5f6c 6973 7428 636f 6c75 6d6e  nent_list(column
-000021f0: 7329 202d 3e20 4c69 7374 5b73 7472 5d3a  s) -> List[str]:
-00002200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002210: 2023 2072 6574 7572 6e20 6120 6c69 7374   # return a list
-00002220: 206f 6620 7374 7269 6e67 2063 6f6e 7461   of string conta
-00002230: 696e 696e 6720 636f 6c75 6d6e 206e 616d  ining column nam
-00002240: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
-00002250: 2020 2023 206d 616b 6520 6561 6368 2063     # make each c
-00002260: 6f6c 756d 6e20 6e61 6d65 2075 6e69 7175  olumn name uniqu
-00002270: 6520 696e 2063 6173 6520 736f 6d65 2063  e in case some c
-00002280: 6f6c 756d 6e73 2068 6176 6520 7468 6520  olumns have the 
-00002290: 7361 6d65 206e 616d 6573 0a20 2020 2020  same names.     
-000022a0: 2020 2020 2020 2020 2020 2063 6c69 7374             clist
-000022b0: 203d 2063 6f6c 756d 6e73 2e74 6f5f 6c69   = columns.to_li
-000022c0: 7374 2829 0a0a 2020 2020 2020 2020 2020  st()..          
-000022d0: 2020 2020 2020 2320 636f 6e76 6572 7420        # convert 
-000022e0: 6576 6572 7974 6869 6e67 2074 6f20 7374  everything to st
-000022f0: 7269 6e67 2069 6620 6e65 6564 6564 0a20  ring if needed. 
-00002300: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00002310: 6f72 2069 2c20 636f 6c75 6d6e 2069 6e20  or i, column in 
-00002320: 656e 756d 6572 6174 6528 636c 6973 7429  enumerate(clist)
-00002330: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002340: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
-00002350: 6e73 7461 6e63 6528 636f 6c75 6d6e 2c20  nstance(column, 
-00002360: 7374 7229 3a0a 2020 2020 2020 2020 2020  str):.          
-00002370: 2020 2020 2020 2020 2020 2020 2020 636c                cl
-00002380: 6973 745b 695d 203d 2073 7472 2863 6f6c  ist[i] = str(col
-00002390: 756d 6e29 0a0a 2020 2020 2020 2020 2020  umn)..          
-000023a0: 2020 2020 2020 6861 735f 6475 706c 6963        has_duplic
-000023b0: 6174 6520 3d20 6c65 6e28 7365 7428 636c  ate = len(set(cl
-000023c0: 6973 7429 2920 213d 206c 656e 2863 6c69  ist)) != len(cli
-000023d0: 7374 290a 2020 2020 2020 2020 2020 2020  st).            
-000023e0: 2020 2020 7768 696c 6520 6861 735f 6475      while has_du
-000023f0: 706c 6963 6174 653a 0a20 2020 2020 2020  plicate:.       
-00002400: 2020 2020 2020 2020 2020 2020 2023 2077               # w
-00002410: 6520 6d61 7920 6861 7665 2074 6f20 6c6f  e may have to lo
-00002420: 6f70 2073 6576 6572 616c 2074 696d 6573  op several times
-00002430: 2028 652e 672e 2077 6520 636f 756c 6420   (e.g. we could 
-00002440: 6861 7665 2063 6f6c 756d 6e73 205b 2230  have columns ["0
-00002450: 222c 2022 305f 3122 2c20 2230 225d 2061  ", "0_1", "0"] a
-00002460: 6e64 206e 6f74 0a20 2020 2020 2020 2020  nd not.         
-00002470: 2020 2020 2020 2020 2020 2023 206e 6f74             # not
-00002480: 6963 696e 6720 7768 656e 2072 656e 616d  icing when renam
-00002490: 696e 6720 7468 6520 6c61 7374 2022 3022  ing the last "0"
-000024a0: 2069 6e74 6f20 2230 5f31 2220 7468 6174   into "0_1" that
-000024b0: 2022 305f 3122 2061 6c72 6561 6479 2065   "0_1" already e
-000024c0: 7869 7374 732e 2e2e 290a 2020 2020 2020  xists...).      
-000024d0: 2020 2020 2020 2020 2020 2020 2020 6e61                na
-000024e0: 6d65 5f74 6f5f 6f63 6375 7265 6e63 6520  me_to_occurence 
-000024f0: 3d20 6465 6661 756c 7464 6963 7428 696e  = defaultdict(in
-00002500: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
-00002510: 2020 2020 2020 2066 6f72 2069 2c20 636f         for i, co
-00002520: 6c75 6d6e 2069 6e20 656e 756d 6572 6174  lumn in enumerat
-00002530: 6528 636c 6973 7429 3a0a 2020 2020 2020  e(clist):.      
-00002540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002550: 2020 6e61 6d65 5f74 6f5f 6f63 6375 7265    name_to_occure
-00002560: 6e63 655b 636c 6973 745b 695d 5d20 2b3d  nce[clist[i]] +=
-00002570: 2031 0a0a 2020 2020 2020 2020 2020 2020   1..            
-00002580: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00002590: 616d 655f 746f 5f6f 6363 7572 656e 6365  ame_to_occurence
-000025a0: 5b63 6c69 7374 5b69 5d5d 203e 2031 3a0a  [clist[i]] > 1:.
-000025b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025c0: 2020 2020 2020 2020 2020 2020 636c 6973              clis
-000025d0: 745b 695d 203d 2063 6c69 7374 5b69 5d20  t[i] = clist[i] 
-000025e0: 2b20 275f 7b7d 272e 666f 726d 6174 286e  + '_{}'.format(n
-000025f0: 616d 655f 746f 5f6f 6363 7572 656e 6365  ame_to_occurence
-00002600: 5b63 6c69 7374 5b69 5d5d 2d31 290a 0a20  [clist[i]]-1).. 
-00002610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002620: 2020 2068 6173 5f64 7570 6c69 6361 7465     has_duplicate
-00002630: 203d 206c 656e 2873 6574 2863 6c69 7374   = len(set(clist
-00002640: 2929 2021 3d20 6c65 6e28 636c 6973 7429  )) != len(clist)
-00002650: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002660: 2020 7265 7475 726e 2063 6c69 7374 0a0a    return clist..
-00002670: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-00002680: 5f69 6e64 6578 5f6e 616d 6520 3d20 7861  _index_name = xa
-00002690: 5f2e 6469 6d73 5b30 5d0a 2020 2020 2020  _.dims[0].      
-000026a0: 2020 2020 2020 636f 6c75 6d6e 735f 6c69        columns_li
-000026b0: 7374 203d 205f 636c 6561 6e5f 636f 6d70  st = _clean_comp
-000026c0: 6f6e 656e 745f 6c69 7374 2863 6f6d 706f  onent_list(compo
-000026d0: 6e65 6e74 7329 0a0a 2020 2020 2020 2020  nents)..        
-000026e0: 2020 2020 2320 544f 444f 3a20 6973 2074      # TODO: is t
-000026f0: 6865 7265 2061 2077 6179 2074 6f20 6a75  here a way to ju
-00002700: 7374 2075 7064 6174 6520 7468 6520 636f  st update the co
-00002710: 6d70 6f6e 656e 7420 696e 6465 7820 7769  mponent index wi
-00002720: 7468 6f75 7420 7265 2d63 7265 6174 696e  thout re-creatin
-00002730: 6720 6120 6e65 7720 4461 7461 4172 7261  g a new DataArra
-00002740: 793f 0a20 2020 2020 2020 2020 2020 2078  y?.            x
-00002750: 615f 203d 2078 722e 4461 7461 4172 7261  a_ = xr.DataArra
-00002760: 7928 7861 5f2e 7661 6c75 6573 2c0a 2020  y(xa_.values,.  
-00002770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002780: 2020 2020 2020 2020 2020 2020 2064 696d               dim
-00002790: 733d 7861 5f2e 6469 6d73 2c0a 2020 2020  s=xa_.dims,.    
-000027a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027b0: 2020 2020 2020 2020 2020 2063 6f6f 7264             coord
-000027c0: 733d 7b74 696d 655f 696e 6465 785f 6e61  s={time_index_na
-000027d0: 6d65 3a20 7861 5f2e 6765 745f 696e 6465  me: xa_.get_inde
-000027e0: 7828 7469 6d65 5f69 6e64 6578 5f6e 616d  x(time_index_nam
-000027f0: 6529 2c20 4449 4d53 5b31 5d3a 2063 6f6c  e), DIMS[1]: col
-00002800: 756d 6e73 5f6c 6973 747d 290a 0a20 2020  umns_list})..   
-00002810: 2020 2020 2023 2057 6520 6361 7374 2074       # We cast t
-00002820: 6865 2061 7272 6179 2074 6f20 666c 6f61  he array to floa
-00002830: 740a 2020 2020 2020 2020 2320 544f 444f  t.        # TODO
-00002840: 3a20 6973 2061 7374 7970 6528 2920 616c  : is astype() al
-00002850: 7761 7973 2063 6f70 7969 6e67 3f20 286d  ways copying? (m
-00002860: 6967 6874 2062 6520 736c 6967 6874 6c79  ight be slightly
-00002870: 2069 6e65 6666 6963 6965 6e74 2069 6620   inefficient if 
-00002880: 6172 7261 7920 6973 2061 6c72 6561 6479  array is already
-00002890: 2066 6c6f 6174 290a 2020 2020 2020 2020   float).        
-000028a0: 7265 7475 726e 2054 696d 6553 6572 6965  return TimeSerie
-000028b0: 7328 7861 5f2e 6173 7479 7065 286e 702e  s(xa_.astype(np.
-000028c0: 666c 6f61 7429 290a 0a20 2020 2040 7374  float))..    @st
-000028d0: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
-000028e0: 6566 2066 726f 6d5f 6461 7461 6672 616d  ef from_datafram
-000028f0: 6528 6466 3a20 7064 2e44 6174 6146 7261  e(df: pd.DataFra
-00002900: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-00002910: 2020 2020 2020 2020 2020 2074 696d 655f             time_
-00002920: 636f 6c3a 204f 7074 696f 6e61 6c5b 7374  col: Optional[st
-00002930: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
-00002940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002950: 2020 7661 6c75 655f 636f 6c73 3a20 4f70    value_cols: Op
-00002960: 7469 6f6e 616c 5b55 6e69 6f6e 5b4c 6973  tional[Union[Lis
-00002970: 745b 7374 725d 2c20 7374 725d 5d20 3d20  t[str], str]] = 
-00002980: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00002990: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-000029a0: 6c5f 6d69 7373 696e 675f 6461 7465 733a  l_missing_dates:
-000029b0: 204f 7074 696f 6e61 6c5b 626f 6f6c 5d20   Optional[bool] 
-000029c0: 3d20 5472 7565 2c0a 2020 2020 2020 2020  = True,.        
-000029d0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-000029e0: 7265 713a 204f 7074 696f 6e61 6c5b 7374  req: Optional[st
-000029f0: 725d 203d 204e 6f6e 652c 2920 2d3e 2027  r] = None,) -> '
-00002a00: 5469 6d65 5365 7269 6573 273a 0a20 2020  TimeSeries':.   
-00002a10: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00002a20: 2052 6574 7572 6e73 2061 2064 6574 6572   Returns a deter
-00002a30: 6d69 6e69 7374 6963 2054 696d 6553 6572  ministic TimeSer
-00002a40: 6965 7320 696e 7374 616e 6365 2062 7569  ies instance bui
-00002a50: 6c74 2066 726f 6d20 6120 7365 6c65 6374  lt from a select
-00002a60: 696f 6e20 6f66 2063 6f6c 756d 6e73 206f  ion of columns o
-00002a70: 6620 6120 4461 7461 4672 616d 652e 0a20  f a DataFrame.. 
-00002a80: 2020 2020 2020 204f 6e65 2063 6f6c 756d         One colum
-00002a90: 6e20 286f 7220 7468 6520 4461 7461 4672  n (or the DataFr
-00002aa0: 616d 6520 696e 6465 7829 2068 6173 2074  ame index) has t
-00002ab0: 6f20 7265 7072 6573 656e 7420 7468 6520  o represent the 
-00002ac0: 7469 6d65 2c0a 2020 2020 2020 2020 616e  time,.        an
-00002ad0: 6420 6120 6c69 7374 206f 6620 636f 6c75  d a list of colu
-00002ae0: 6d6e 7320 6076 616c 7565 5f63 6f6c 7360  mns `value_cols`
-00002af0: 2068 6173 2074 6f20 7265 7072 6573 656e   has to represen
-00002b00: 7420 7468 6520 7661 6c75 6573 2066 6f72  t the values for
-00002b10: 2074 6869 7320 7469 6d65 2073 6572 6965   this time serie
-00002b20: 732e 0a0a 2020 2020 2020 2020 5061 7261  s...        Para
-00002b30: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-00002b40: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-00002b50: 2020 6466 0a20 2020 2020 2020 2020 2020    df.           
-00002b60: 2054 6865 2044 6174 6146 7261 6d65 0a20   The DataFrame. 
-00002b70: 2020 2020 2020 2074 696d 655f 636f 6c0a         time_col.
-00002b80: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00002b90: 7469 6d65 2063 6f6c 756d 6e20 6e61 6d65  time column name
-00002ba0: 2e20 4966 2073 6574 2c20 7468 6520 636f  . If set, the co
-00002bb0: 6c75 6d6e 2077 696c 6c20 6265 2063 6173  lumn will be cas
-00002bc0: 7420 746f 2061 2070 616e 6461 7320 4461  t to a pandas Da
-00002bd0: 7465 7469 6d65 496e 6465 782e 0a20 2020  tetimeIndex..   
-00002be0: 2020 2020 2020 2020 2049 6620 6e6f 7420           If not 
-00002bf0: 7365 742c 2074 6865 2044 6174 6146 7261  set, the DataFra
-00002c00: 6d65 2069 6e64 6578 2077 696c 6c20 6265  me index will be
-00002c10: 2075 7365 642e 2049 6e20 7468 6973 2063   used. In this c
-00002c20: 6173 6520 7468 6520 4461 7461 4672 616d  ase the DataFram
-00002c30: 6520 6d75 7374 2063 6f6e 7461 696e 2061  e must contain a
-00002c40: 6e20 696e 6465 7820 7468 6174 2069 730a  n index that is.
-00002c50: 2020 2020 2020 2020 2020 2020 6569 7468              eith
-00002c60: 6572 2061 2070 616e 6461 7320 4461 7465  er a pandas Date
-00002c70: 7469 6d65 496e 6465 7820 6f72 2061 2070  timeIndex or a p
-00002c80: 616e 6461 7320 5261 6e67 6549 6e64 6578  andas RangeIndex
-00002c90: 2e0a 2020 2020 2020 2020 7661 6c75 655f  ..        value_
-00002ca0: 636f 6c73 0a20 2020 2020 2020 2020 2020  cols.           
-00002cb0: 2041 2073 7472 696e 6720 6f72 206c 6973   A string or lis
-00002cc0: 7420 6f66 2073 7472 696e 6773 2072 6570  t of strings rep
-00002cd0: 7265 7365 6e74 696e 6720 7468 6520 7661  resenting the va
-00002ce0: 6c75 6520 636f 6c75 6d6e 2873 2920 746f  lue column(s) to
-00002cf0: 2062 6520 6578 7472 6163 7465 6420 6672   be extracted fr
-00002d00: 6f6d 2074 6865 2044 6174 6146 7261 6d65  om the DataFrame
-00002d10: 2e20 4966 2073 6574 2074 6f0a 2020 2020  . If set to.    
-00002d20: 2020 2020 2020 2020 604e 6f6e 6560 2c20          `None`, 
-00002d30: 7468 6520 7768 6f6c 6520 4461 7461 4672  the whole DataFr
-00002d40: 616d 6520 7769 6c6c 2062 6520 7573 6564  ame will be used
-00002d50: 2e0a 2020 2020 2020 2020 6669 6c6c 5f6d  ..        fill_m
-00002d60: 6973 7369 6e67 5f64 6174 6573 0a20 2020  issing_dates.   
-00002d70: 2020 2020 2020 2020 204f 7074 696f 6e61           Optiona
-00002d80: 6c6c 792c 2061 2062 6f6f 6c65 616e 2076  lly, a boolean v
-00002d90: 616c 7565 2069 6e64 6963 6174 696e 6720  alue indicating 
-00002da0: 7768 6574 6865 7220 746f 2066 696c 6c20  whether to fill 
-00002db0: 6d69 7373 696e 6720 6461 7465 7320 7769  missing dates wi
-00002dc0: 7468 204e 614e 2076 616c 7565 732e 2054  th NaN values. T
-00002dd0: 6869 7320 7265 7175 6972 6573 0a20 2020  his requires.   
-00002de0: 2020 2020 2020 2020 2065 6974 6865 7220           either 
-00002df0: 6120 7072 6f76 6964 6564 2060 6672 6571  a provided `freq
-00002e00: 6020 6f72 2074 6865 2070 6f73 7369 6269  ` or the possibi
-00002e10: 6c69 7479 2074 6f20 696e 6665 7220 7468  lity to infer th
-00002e20: 6520 6672 6571 7565 6e63 7920 6672 6f6d  e frequency from
-00002e30: 2074 6865 2070 726f 7669 6465 6420 7469   the provided ti
-00002e40: 6d65 7374 616d 7073 2e0a 2020 2020 2020  mestamps..      
-00002e50: 2020 6672 6571 0a20 2020 2020 2020 2020    freq.         
-00002e60: 2020 204f 7074 696f 6e61 6c6c 792c 2061     Optionally, a
-00002e70: 2073 7472 696e 6720 7265 7072 6573 656e   string represen
-00002e80: 7469 6e67 2074 6865 2066 7265 7175 656e  ting the frequen
-00002e90: 6379 206f 6620 7468 6520 5061 6e64 6173  cy of the Pandas
-00002ea0: 2044 6174 6146 7261 6d65 2e20 5468 6973   DataFrame. This
-00002eb0: 2069 7320 7573 6566 756c 2069 6e20 6f72   is useful in or
-00002ec0: 6465 7220 746f 2066 696c 6c0a 2020 2020  der to fill.    
-00002ed0: 2020 2020 2020 2020 696e 206d 6973 7369          in missi
-00002ee0: 6e67 2076 616c 7565 7320 6966 2073 6f6d  ng values if som
-00002ef0: 6520 6461 7465 7320 6172 6520 6d69 7373  e dates are miss
-00002f00: 696e 6720 616e 6420 6066 696c 6c5f 6d69  ing and `fill_mi
-00002f10: 7373 696e 675f 6461 7465 7360 2069 7320  ssing_dates` is 
-00002f20: 7365 7420 746f 2060 5472 7565 602e 0a0a  set to `True`...
-00002f30: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-00002f40: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-00002f50: 2020 2020 2020 2020 5469 6d65 5365 7269          TimeSeri
-00002f60: 6573 0a20 2020 2020 2020 2020 2020 2041  es.            A
-00002f70: 2075 6e69 7661 7269 6174 6520 6f72 206d   univariate or m
-00002f80: 756c 7469 7661 7269 6174 6520 6465 7465  ultivariate dete
-00002f90: 726d 696e 6973 7469 6320 5469 6d65 5365  rministic TimeSe
-00002fa0: 7269 6573 2063 6f6e 7374 7275 6374 6564  ries constructed
-00002fb0: 2066 726f 6d20 7468 6520 696e 7075 7473   from the inputs
-00002fc0: 2e0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
-00002fd0: 2020 2020 2020 2023 2067 6574 2076 616c         # get val
-00002fe0: 7565 730a 2020 2020 2020 2020 6966 2076  ues.        if v
-00002ff0: 616c 7565 5f63 6f6c 7320 6973 204e 6f6e  alue_cols is Non
-00003000: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00003010: 6572 6965 735f 6466 203d 2064 662e 6c6f  eries_df = df.lo
-00003020: 635b 3a2c 2064 662e 636f 6c75 6d6e 7320  c[:, df.columns 
-00003030: 213d 2074 696d 655f 636f 6c5d 0a20 2020  != time_col].   
-00003040: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00003050: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00003060: 616e 6365 2876 616c 7565 5f63 6f6c 732c  ance(value_cols,
-00003070: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
-00003080: 2020 2020 2020 2076 616c 7565 5f63 6f6c         value_col
-00003090: 7320 3d20 5b76 616c 7565 5f63 6f6c 735d  s = [value_cols]
-000030a0: 0a20 2020 2020 2020 2020 2020 2073 6572  .            ser
-000030b0: 6965 735f 6466 203d 2064 665b 7661 6c75  ies_df = df[valu
-000030c0: 655f 636f 6c73 5d0a 0a20 2020 2020 2020  e_cols]..       
-000030d0: 2023 2067 6574 2074 696d 6520 696e 6465   # get time inde
-000030e0: 780a 2020 2020 2020 2020 6966 2074 696d  x.        if tim
-000030f0: 655f 636f 6c3a 0a20 2020 2020 2020 2020  e_col:.         
-00003100: 2020 2074 696d 655f 696e 6465 7820 3d20     time_index = 
-00003110: 7064 2e44 6174 6574 696d 6549 6e64 6578  pd.DatetimeIndex
-00003120: 2864 665b 7469 6d65 5f63 6f6c 5d29 0a20  (df[time_col]). 
-00003130: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00003140: 2020 2020 2020 2020 2072 6169 7365 5f69           raise_i
-00003150: 665f 6e6f 7428 6973 696e 7374 616e 6365  f_not(isinstance
-00003160: 2864 662e 696e 6465 782c 2070 642e 5261  (df.index, pd.Ra
-00003170: 6e67 6549 6e64 6578 2920 6f72 2069 7369  ngeIndex) or isi
-00003180: 6e73 7461 6e63 6528 6466 2e69 6e64 6578  nstance(df.index
-00003190: 2c20 7064 2e44 6174 6574 696d 6549 6e64  , pd.DatetimeInd
-000031a0: 6578 292c 0a20 2020 2020 2020 2020 2020  ex),.           
-000031b0: 2020 2020 2020 2020 2020 2020 2020 2749                'I
-000031c0: 6620 7469 6d65 5f63 6f6c 2069 7320 6e6f  f time_col is no
-000031d0: 7420 7370 6563 6966 6965 642c 2074 6865  t specified, the
-000031e0: 2044 6174 6146 7261 6d65 206d 7573 7420   DataFrame must 
-000031f0: 6265 2069 6e64 6578 6564 2065 6974 6865  be indexed eithe
-00003200: 7220 7769 7468 270a 2020 2020 2020 2020  r with'.        
-00003210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003220: 2027 6120 4461 7465 7469 6d65 496e 6465   'a DatetimeInde
-00003230: 782c 206f 7220 7769 7468 2061 2052 616e  x, or with a Ran
-00003240: 6765 496e 6465 782e 272c 206c 6f67 6765  geIndex.', logge
-00003250: 7229 0a20 2020 2020 2020 2020 2020 2074  r).            t
-00003260: 696d 655f 696e 6465 7820 3d20 6466 2e69  ime_index = df.i
-00003270: 6e64 6578 0a0a 2020 2020 2020 2020 6966  ndex..        if
-00003280: 206e 6f74 2074 696d 655f 696e 6465 782e   not time_index.
-00003290: 6e61 6d65 3a0a 2020 2020 2020 2020 2020  name:.          
-000032a0: 2020 7469 6d65 5f69 6e64 6578 2e6e 616d    time_index.nam
-000032b0: 6520 3d20 4449 4d53 5b30 5d0a 0a20 2020  e = DIMS[0]..   
-000032c0: 2020 2020 2078 6120 3d20 7872 2e44 6174       xa = xr.Dat
-000032d0: 6141 7272 6179 2873 6572 6965 735f 6466  aArray(series_df
-000032e0: 2e76 616c 7565 735b 3a2c 203a 2c20 6e70  .values[:, :, np
-000032f0: 2e6e 6577 6178 6973 5d2c 0a20 2020 2020  .newaxis],.     
-00003300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003310: 2020 2020 2064 696d 733d 2874 696d 655f       dims=(time_
-00003320: 696e 6465 782e 6e61 6d65 2c29 202b 2044  index.name,) + D
-00003330: 494d 535b 2d32 3a5d 2c0a 2020 2020 2020  IMS[-2:],.      
-00003340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003350: 2020 2020 636f 6f72 6473 3d7b 7469 6d65      coords={time
-00003360: 5f69 6e64 6578 2e6e 616d 653a 2074 696d  _index.name: tim
-00003370: 655f 696e 6465 782c 2044 494d 535b 315d  e_index, DIMS[1]
-00003380: 3a20 7365 7269 6573 5f64 662e 636f 6c75  : series_df.colu
-00003390: 6d6e 737d 290a 0a20 2020 2020 2020 2072  mns})..        r
-000033a0: 6574 7572 6e20 5469 6d65 5365 7269 6573  eturn TimeSeries
-000033b0: 2e66 726f 6d5f 7861 7272 6179 2878 613d  .from_xarray(xa=
-000033c0: 7861 2c20 6669 6c6c 5f6d 6973 7369 6e67  xa, fill_missing
-000033d0: 5f64 6174 6573 3d66 696c 6c5f 6d69 7373  _dates=fill_miss
-000033e0: 696e 675f 6461 7465 732c 2066 7265 713d  ing_dates, freq=
-000033f0: 6672 6571 290a 0a20 2020 2040 7374 6174  freq)..    @stat
-00003400: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
-00003410: 2066 726f 6d5f 7365 7269 6573 2870 645f   from_series(pd_
-00003420: 7365 7269 6573 3a20 7064 2e53 6572 6965  series: pd.Serie
-00003430: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-00003440: 2020 2020 2020 2066 696c 6c5f 6d69 7373         fill_miss
-00003450: 696e 675f 6461 7465 733a 204f 7074 696f  ing_dates: Optio
-00003460: 6e61 6c5b 626f 6f6c 5d20 3d20 5472 7565  nal[bool] = True
-00003470: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003480: 2020 2020 2020 6672 6571 3a20 4f70 7469        freq: Opti
-00003490: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-000034a0: 2c29 202d 3e20 2754 696d 6553 6572 6965  ,) -> 'TimeSerie
-000034b0: 7327 3a0a 2020 2020 2020 2020 2222 220a  s':.        """.
-000034c0: 2020 2020 2020 2020 5265 7475 726e 7320          Returns 
-000034d0: 6120 756e 6976 6172 6961 7465 2061 6e64  a univariate and
-000034e0: 2064 6574 6572 6d69 6e69 7374 6963 2054   deterministic T
-000034f0: 696d 6553 6572 6965 7320 6275 696c 7420  imeSeries built 
-00003500: 6672 6f6d 2061 2070 616e 6461 7320 5365  from a pandas Se
-00003510: 7269 6573 2e0a 0a20 2020 2020 2020 2050  ries...        P
-00003520: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-00003530: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-00003540: 2020 2020 2070 645f 7365 7269 6573 0a20       pd_series. 
-00003550: 2020 2020 2020 2020 2020 2054 6865 2070             The p
-00003560: 616e 6461 7320 5365 7269 6573 2069 6e73  andas Series ins
-00003570: 7461 6e63 652e 0a20 2020 2020 2020 2066  tance..        f
-00003580: 696c 6c5f 6d69 7373 696e 675f 6461 7465  ill_missing_date
-00003590: 730a 2020 2020 2020 2020 2020 2020 4f70  s.            Op
-000035a0: 7469 6f6e 616c 6c79 2c20 6120 626f 6f6c  tionally, a bool
-000035b0: 6561 6e20 7661 6c75 6520 696e 6469 6361  ean value indica
-000035c0: 7469 6e67 2077 6865 7468 6572 2074 6f20  ting whether to 
-000035d0: 6669 6c6c 206d 6973 7369 6e67 2064 6174  fill missing dat
-000035e0: 6573 2077 6974 6820 4e61 4e20 7661 6c75  es with NaN valu
-000035f0: 6573 2e20 5468 6973 2072 6571 7569 7265  es. This require
-00003600: 730a 2020 2020 2020 2020 2020 2020 6569  s.            ei
-00003610: 7468 6572 2061 2070 726f 7669 6465 6420  ther a provided 
-00003620: 6066 7265 7160 206f 7220 7468 6520 706f  `freq` or the po
-00003630: 7373 6962 696c 6974 7920 746f 2069 6e66  ssibility to inf
-00003640: 6572 2074 6865 2066 7265 7175 656e 6379  er the frequency
-00003650: 2066 726f 6d20 7468 6520 7072 6f76 6964   from the provid
-00003660: 6564 2074 696d 6573 7461 6d70 732e 0a20  ed timestamps.. 
-00003670: 2020 2020 2020 2066 7265 710a 2020 2020         freq.    
-00003680: 2020 2020 2020 2020 4f70 7469 6f6e 616c          Optional
-00003690: 6c79 2c20 6120 7374 7269 6e67 2072 6570  ly, a string rep
-000036a0: 7265 7365 6e74 696e 6720 7468 6520 6672  resenting the fr
-000036b0: 6571 7565 6e63 7920 6f66 2074 6865 2050  equency of the P
-000036c0: 616e 6461 7320 4461 7461 4672 616d 652e  andas DataFrame.
-000036d0: 2054 6869 7320 6973 2075 7365 6675 6c20   This is useful 
-000036e0: 696e 206f 7264 6572 2074 6f20 6669 6c6c  in order to fill
-000036f0: 0a20 2020 2020 2020 2020 2020 2069 6e20  .            in 
-00003700: 6d69 7373 696e 6720 7661 6c75 6573 2069  missing values i
-00003710: 6620 736f 6d65 2064 6174 6573 2061 7265  f some dates are
-00003720: 206d 6973 7369 6e67 2061 6e64 2060 6669   missing and `fi
-00003730: 6c6c 5f6d 6973 7369 6e67 5f64 6174 6573  ll_missing_dates
-00003740: 6020 6973 2073 6574 2074 6f20 6054 7275  ` is set to `Tru
-00003750: 6560 2e0a 0a20 2020 2020 2020 2052 6574  e`...        Ret
-00003760: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-00003770: 2d2d 2d2d 0a20 2020 2020 2020 2054 696d  ----.        Tim
-00003780: 6553 6572 6965 730a 2020 2020 2020 2020  eSeries.        
-00003790: 2020 2020 4120 756e 6976 6172 6961 7465      A univariate
-000037a0: 2061 6e64 2064 6574 6572 6d69 6e69 7374   and determinist
-000037b0: 6963 2054 696d 6553 6572 6965 7320 636f  ic TimeSeries co
-000037c0: 6e73 7472 7563 7465 6420 6672 6f6d 2074  nstructed from t
-000037d0: 6865 2069 6e70 7574 732e 0a20 2020 2020  he inputs..     
-000037e0: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-000037f0: 6466 203d 2070 642e 4461 7461 4672 616d  df = pd.DataFram
-00003800: 6528 7064 5f73 6572 6965 7329 0a20 2020  e(pd_series).   
-00003810: 2020 2020 2072 6574 7572 6e20 5469 6d65       return Time
-00003820: 5365 7269 6573 2e66 726f 6d5f 6461 7461  Series.from_data
-00003830: 6672 616d 6528 6466 2c0a 2020 2020 2020  frame(df,.      
-00003840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003860: 2020 2074 696d 655f 636f 6c3d 4e6f 6e65     time_col=None
-00003870: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003890: 2020 2020 2020 2020 2020 2076 616c 7565             value
-000038a0: 5f63 6f6c 733d 4e6f 6e65 2c0a 2020 2020  _cols=None,.    
-000038b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038d0: 2020 2020 2066 696c 6c5f 6d69 7373 696e       fill_missin
-000038e0: 675f 6461 7465 733d 6669 6c6c 5f6d 6973  g_dates=fill_mis
-000038f0: 7369 6e67 5f64 6174 6573 2c0a 2020 2020  sing_dates,.    
-00003900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003920: 2020 2020 2066 7265 713d 6672 6571 290a       freq=freq).
-00003930: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
-00003940: 6f64 0a20 2020 2064 6566 2066 726f 6d5f  od.    def from_
-00003950: 7469 6d65 735f 616e 645f 7661 6c75 6573  times_and_values
-00003960: 2874 696d 6573 3a20 556e 696f 6e5b 7064  (times: Union[pd
-00003970: 2e44 6174 6574 696d 6549 6e64 6578 2c20  .DatetimeIndex, 
-00003980: 7064 2e52 616e 6765 496e 6465 785d 2c0a  pd.RangeIndex],.
-00003990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039a0: 2020 2020 2020 2020 2020 2020 2020 7661                va
-000039b0: 6c75 6573 3a20 6e70 2e6e 6461 7272 6179  lues: np.ndarray
-000039c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000039d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039e0: 6669 6c6c 5f6d 6973 7369 6e67 5f64 6174  fill_missing_dat
-000039f0: 6573 3a20 4f70 7469 6f6e 616c 5b62 6f6f  es: Optional[boo
-00003a00: 6c5d 203d 2054 7275 652c 0a20 2020 2020  l] = True,.     
-00003a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a20: 2020 2020 2020 2020 2066 7265 713a 204f           freq: O
-00003a30: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-00003a40: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00003a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a60: 2020 2063 6f6c 756d 6e73 3a20 4f70 7469     columns: Opti
-00003a70: 6f6e 616c 5b70 642e 5f74 7970 696e 672e  onal[pd._typing.
-00003a80: 4178 6573 5d20 3d20 4e6f 6e65 2920 2d3e  Axes] = None) ->
-00003a90: 2027 5469 6d65 5365 7269 6573 273a 0a20   'TimeSeries':. 
-00003aa0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00003ab0: 2020 2052 6574 7572 6e73 2061 2054 696d     Returns a Tim
-00003ac0: 6553 6572 6965 7320 6275 696c 7420 6672  eSeries built fr
-00003ad0: 6f6d 2061 6e20 696e 6465 7820 616e 6420  om an index and 
-00003ae0: 7661 6c75 6520 6172 7261 792e 0a0a 2020  value array...  
-00003af0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00003b00: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00003b10: 2d2d 2d0a 2020 2020 2020 2020 7469 6d65  ---.        time
-00003b20: 730a 2020 2020 2020 2020 2020 2020 4120  s.            A 
-00003b30: 6070 616e 6461 732e 4461 7465 5469 6d65  `pandas.DateTime
-00003b40: 496e 6465 7860 206f 7220 6070 616e 6461  Index` or `panda
-00003b50: 732e 5261 6e67 6549 6e64 6578 6020 7265  s.RangeIndex` re
-00003b60: 7072 6573 656e 7469 6e67 2074 6865 2074  presenting the t
-00003b70: 696d 6520 6178 6973 2066 6f72 2074 6865  ime axis for the
-00003b80: 2074 696d 6520 7365 7269 6573 2e0a 2020   time series..  
-00003b90: 2020 2020 2020 7661 6c75 6573 0a20 2020        values.   
-00003ba0: 2020 2020 2020 2020 2041 204e 756d 7079           A Numpy
-00003bb0: 2061 7272 6179 206f 6620 7661 6c75 6573   array of values
-00003bc0: 2066 6f72 2074 6865 2054 696d 6553 6572   for the TimeSer
-00003bd0: 6965 732e 2042 6f74 6820 322d 6469 6d65  ies. Both 2-dime
-00003be0: 6e73 696f 6e61 6c20 6172 7261 7973 2c20  nsional arrays, 
-00003bf0: 666f 7220 6465 7465 726d 696e 6973 7469  for deterministi
-00003c00: 6320 7365 7269 6573 2c0a 2020 2020 2020  c series,.      
-00003c10: 2020 2020 2020 616e 6420 332d 6469 6d65        and 3-dime
-00003c20: 6e73 696f 6e61 6c20 6172 7261 7973 2c20  nsional arrays, 
-00003c30: 666f 7220 7072 6f62 6162 696c 6973 7469  for probabilisti
-00003c40: 6320 7365 7269 6573 2c20 6172 6520 6163  c series, are ac
-00003c50: 6365 7074 6564 2e20 496e 2074 6865 2066  cepted. In the f
-00003c60: 6f72 6d65 7220 6361 7365 2074 6865 2064  ormer case the d
-00003c70: 696d 656e 7369 6f6e 730a 2020 2020 2020  imensions.      
-00003c80: 2020 2020 2020 7368 6f75 6c64 2062 6520        should be 
-00003c90: 2874 696d 652c 2063 6f6d 706f 6e65 6e74  (time, component
-00003ca0: 292c 2061 6e64 2069 6e20 7468 6520 6c61  ), and in the la
-00003cb0: 7474 6572 2063 6173 6520 2874 696d 652c  tter case (time,
-00003cc0: 2063 6f6d 706f 6e65 6e74 2c20 7361 6d70   component, samp
-00003cd0: 6c65 292e 0a20 2020 2020 2020 2066 696c  le)..        fil
-00003ce0: 6c5f 6d69 7373 696e 675f 6461 7465 730a  l_missing_dates.
-00003cf0: 2020 2020 2020 2020 2020 2020 4f70 7469              Opti
-00003d00: 6f6e 616c 6c79 2c20 6120 626f 6f6c 6561  onally, a boolea
-00003d10: 6e20 7661 6c75 6520 696e 6469 6361 7469  n value indicati
-00003d20: 6e67 2077 6865 7468 6572 2074 6f20 6669  ng whether to fi
-00003d30: 6c6c 206d 6973 7369 6e67 2064 6174 6573  ll missing dates
-00003d40: 2077 6974 6820 4e61 4e20 7661 6c75 6573   with NaN values
-00003d50: 2e20 5468 6973 2072 6571 7569 7265 730a  . This requires.
-00003d60: 2020 2020 2020 2020 2020 2020 6569 7468              eith
-00003d70: 6572 2061 2070 726f 7669 6465 6420 6066  er a provided `f
-00003d80: 7265 7160 206f 7220 7468 6520 706f 7373  req` or the poss
-00003d90: 6962 696c 6974 7920 746f 2069 6e66 6572  ibility to infer
-00003da0: 2074 6865 2066 7265 7175 656e 6379 2066   the frequency f
-00003db0: 726f 6d20 7468 6520 7072 6f76 6964 6564  rom the provided
-00003dc0: 2074 696d 6573 7461 6d70 732e 0a20 2020   timestamps..   
-00003dd0: 2020 2020 2066 7265 710a 2020 2020 2020       freq.      
-00003de0: 2020 2020 2020 4f70 7469 6f6e 616c 6c79        Optionally
-00003df0: 2c20 6120 7374 7269 6e67 2072 6570 7265  , a string repre
-00003e00: 7365 6e74 696e 6720 7468 6520 6672 6571  senting the freq
-00003e10: 7565 6e63 7920 6f66 2074 6865 2050 616e  uency of the Pan
-00003e20: 6461 7320 4461 7461 4672 616d 652e 2054  das DataFrame. T
-00003e30: 6869 7320 6973 2075 7365 6675 6c20 696e  his is useful in
-00003e40: 206f 7264 6572 2074 6f20 6669 6c6c 0a20   order to fill. 
-00003e50: 2020 2020 2020 2020 2020 2069 6e20 6d69             in mi
-00003e60: 7373 696e 6720 7661 6c75 6573 2069 6620  ssing values if 
-00003e70: 736f 6d65 2064 6174 6573 2061 7265 206d  some dates are m
-00003e80: 6973 7369 6e67 2061 6e64 2060 6669 6c6c  issing and `fill
-00003e90: 5f6d 6973 7369 6e67 5f64 6174 6573 6020  _missing_dates` 
-00003ea0: 6973 2073 6574 2074 6f20 6054 7275 6560  is set to `True`
-00003eb0: 2e0a 2020 2020 2020 2020 636f 6c75 6d6e  ..        column
-00003ec0: 730a 2020 2020 2020 2020 2020 2020 436f  s.            Co
-00003ed0: 6c75 6d6e 7320 746f 2062 6520 7573 6564  lumns to be used
-00003ee0: 2062 7920 7468 6520 756e 6465 726c 7969   by the underlyi
-00003ef0: 6e67 2070 616e 6461 7320 4461 7461 4672  ng pandas DataFr
-00003f00: 616d 652e 0a0a 2020 2020 2020 2020 5265  ame...        Re
-00003f10: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
-00003f20: 2d2d 2d2d 2d0a 2020 2020 2020 2020 5469  -----.        Ti
-00003f30: 6d65 5365 7269 6573 0a20 2020 2020 2020  meSeries.       
-00003f40: 2020 2020 2041 2054 696d 6553 6572 6965       A TimeSerie
-00003f50: 7320 636f 6e73 7472 7563 7465 6420 6672  s constructed fr
-00003f60: 6f6d 2074 6865 2069 6e70 7574 732e 0a20  om the inputs.. 
-00003f70: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-00003f80: 2020 2020 7261 6973 655f 6966 5f6e 6f74      raise_if_not
-00003f90: 2869 7369 6e73 7461 6e63 6528 7469 6d65  (isinstance(time
-00003fa0: 732c 2070 642e 5261 6e67 6549 6e64 6578  s, pd.RangeIndex
-00003fb0: 2920 6f72 2069 7369 6e73 7461 6e63 6528  ) or isinstance(
-00003fc0: 7469 6d65 732c 2070 642e 4461 7465 7469  times, pd.Dateti
-00003fd0: 6d65 496e 6465 7829 2c0a 2020 2020 2020  meIndex),.      
-00003fe0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00003ff0: 7468 6520 6074 696d 6573 6020 6172 6775  the `times` argu
-00004000: 6d65 6e74 206d 7573 7420 6265 2061 2052  ment must be a R
-00004010: 616e 6765 496e 6465 7820 6f72 2061 2044  angeIndex or a D
-00004020: 6174 6554 696d 6549 6e64 6578 2e20 5573  ateTimeIndex. Us
-00004030: 6520 270a 2020 2020 2020 2020 2020 2020  e '.            
-00004040: 2020 2020 2020 2020 2027 5469 6d65 5365           'TimeSe
-00004050: 7269 6573 2e66 726f 6d5f 7661 6c75 6573  ries.from_values
-00004060: 2829 2069 6620 796f 7520 7761 6e74 2074  () if you want t
-00004070: 6f20 7573 6520 616e 2061 7574 6f6d 6174  o use an automat
-00004080: 6963 2052 616e 6765 496e 6465 782e 2729  ic RangeIndex.')
-00004090: 0a0a 2020 2020 2020 2020 7469 6d65 735f  ..        times_
-000040a0: 6e61 6d65 203d 2044 494d 535b 305d 2069  name = DIMS[0] i
-000040b0: 6620 6e6f 7420 7469 6d65 732e 6e61 6d65  f not times.name
-000040c0: 2065 6c73 6520 7469 6d65 732e 6e61 6d65   else times.name
-000040d0: 0a0a 2020 2020 2020 2020 7661 6c75 6573  ..        values
-000040e0: 203d 206e 702e 6172 7261 7928 7661 6c75   = np.array(valu
-000040f0: 6573 290a 2020 2020 2020 2020 6966 206c  es).        if l
-00004100: 656e 2876 616c 7565 732e 7368 6170 6529  en(values.shape)
-00004110: 203d 3d20 313a 0a20 2020 2020 2020 2020   == 1:.         
-00004120: 2020 2076 616c 7565 7320 3d20 6e70 2e65     values = np.e
-00004130: 7870 616e 645f 6469 6d73 2876 616c 7565  xpand_dims(value
-00004140: 732c 2031 290a 2020 2020 2020 2020 6966  s, 1).        if
-00004150: 206c 656e 2876 616c 7565 732e 7368 6170   len(values.shap
-00004160: 6529 203d 3d20 323a 0a20 2020 2020 2020  e) == 2:.       
-00004170: 2020 2020 2076 616c 7565 7320 3d20 6e70       values = np
-00004180: 2e65 7870 616e 645f 6469 6d73 2876 616c  .expand_dims(val
-00004190: 7565 732c 2032 290a 0a20 2020 2020 2020  ues, 2)..       
-000041a0: 2063 6f6f 7264 7320 3d20 7b74 696d 6573   coords = {times
-000041b0: 5f6e 616d 653a 2074 696d 6573 7d0a 2020  _name: times}.  
-000041c0: 2020 2020 2020 6966 2063 6f6c 756d 6e73        if columns
-000041d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000041e0: 2020 2020 2020 2020 2020 636f 6f72 6473            coords
-000041f0: 5b44 494d 535b 315d 5d20 3d20 636f 6c75  [DIMS[1]] = colu
-00004200: 6d6e 730a 0a20 2020 2020 2020 2078 6120  mns..        xa 
-00004210: 3d20 7872 2e44 6174 6141 7272 6179 2876  = xr.DataArray(v
-00004220: 616c 7565 732c 0a20 2020 2020 2020 2020  alues,.         
-00004230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004240: 2064 696d 733d 2874 696d 6573 5f6e 616d   dims=(times_nam
-00004250: 652c 2920 2b20 4449 4d53 5b2d 323a 5d2c  e,) + DIMS[-2:],
-00004260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004270: 2020 2020 2020 2020 2020 2063 6f6f 7264             coord
-00004280: 733d 636f 6f72 6473 290a 0a20 2020 2020  s=coords)..     
-00004290: 2020 2072 6574 7572 6e20 5469 6d65 5365     return TimeSe
-000042a0: 7269 6573 2e66 726f 6d5f 7861 7272 6179  ries.from_xarray
-000042b0: 2878 613d 7861 2c20 6669 6c6c 5f6d 6973  (xa=xa, fill_mis
-000042c0: 7369 6e67 5f64 6174 6573 3d66 696c 6c5f  sing_dates=fill_
-000042d0: 6d69 7373 696e 675f 6461 7465 732c 2066  missing_dates, f
-000042e0: 7265 713d 6672 6571 290a 0a20 2020 2040  req=freq)..    @
-000042f0: 7374 6174 6963 6d65 7468 6f64 0a20 2020  staticmethod.   
-00004300: 2064 6566 2066 726f 6d5f 7661 6c75 6573   def from_values
-00004310: 2876 616c 7565 733a 206e 702e 6e64 6172  (values: np.ndar
-00004320: 7261 792c 0a20 2020 2020 2020 2020 2020  ray,.           
-00004330: 2020 2020 2020 2020 2066 696c 6c5f 6d69           fill_mi
-00004340: 7373 696e 675f 6461 7465 733a 204f 7074  ssing_dates: Opt
-00004350: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 5472  ional[bool] = Tr
-00004360: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00004370: 2020 2020 2020 2020 6672 6571 3a20 4f70          freq: Op
-00004380: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00004390: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-000043a0: 2020 2020 2020 2020 636f 6c75 6d6e 733a          columns:
-000043b0: 204f 7074 696f 6e61 6c5b 7064 2e5f 7479   Optional[pd._ty
-000043c0: 7069 6e67 2e41 7865 735d 203d 204e 6f6e  ping.Axes] = Non
-000043d0: 6529 202d 3e20 2754 696d 6553 6572 6965  e) -> 'TimeSerie
-000043e0: 7327 3a0a 0a20 2020 2020 2020 2074 696d  s':..        tim
-000043f0: 655f 696e 6465 7820 3d20 7064 2e52 616e  e_index = pd.Ran
-00004400: 6765 496e 6465 7828 302c 206c 656e 2876  geIndex(0, len(v
-00004410: 616c 7565 7329 2c20 3129 0a0a 2020 2020  alues), 1)..    
-00004420: 2020 2020 7661 6c75 6573 5f20 3d20 6e70      values_ = np
-00004430: 2e72 6573 6861 7065 2876 616c 7565 732c  .reshape(values,
-00004440: 2028 6c65 6e28 7661 6c75 6573 292c 2031   (len(values), 1
-00004450: 2929 2069 6620 6c65 6e28 7661 6c75 6573  )) if len(values
-00004460: 2e73 6861 7065 2920 3d3d 2031 2065 6c73  .shape) == 1 els
-00004470: 6520 7661 6c75 6573 0a20 2020 2020 2020  e values.       
-00004480: 2072 6574 7572 6e20 5469 6d65 5365 7269   return TimeSeri
-00004490: 6573 2e66 726f 6d5f 7469 6d65 735f 616e  es.from_times_an
-000044a0: 645f 7661 6c75 6573 2874 696d 6573 3d74  d_values(times=t
-000044b0: 696d 655f 696e 6465 782c 0a20 2020 2020  ime_index,.     
-000044c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044e0: 2020 2020 2020 2020 2020 2076 616c 7565             value
-000044f0: 733d 7661 6c75 6573 5f2c 0a20 2020 2020  s=values_,.     
-00004500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004520: 2020 2020 2020 2020 2020 2066 696c 6c5f             fill_
-00004530: 6d69 7373 696e 675f 6461 7465 733d 6669  missing_dates=fi
-00004540: 6c6c 5f6d 6973 7369 6e67 5f64 6174 6573  ll_missing_dates
-00004550: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00004560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004580: 2020 6672 6571 3d66 7265 712c 0a20 2020    freq=freq,.   
-00004590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045b0: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-000045c0: 756d 6e73 3d63 6f6c 756d 6e73 290a 0a20  umns=columns).. 
-000045d0: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
-000045e0: 0a20 2020 2064 6566 2066 726f 6d5f 6a73  .    def from_js
-000045f0: 6f6e 286a 736f 6e5f 7374 723a 2073 7472  on(json_str: str
-00004600: 2920 2d3e 2027 5469 6d65 5365 7269 6573  ) -> 'TimeSeries
-00004610: 273a 0a20 2020 2020 2020 2022 2222 0a20  ':.        """. 
-00004620: 2020 2020 2020 2043 6f6e 7665 7274 7320         Converts 
-00004630: 7468 6520 4a53 4f4e 2053 7472 696e 6720  the JSON String 
-00004640: 7265 7072 6573 656e 7461 7469 6f6e 206f  representation o
-00004650: 6620 6120 6054 696d 6553 6572 6965 7360  f a `TimeSeries`
-00004660: 206f 626a 6563 7420 2870 726f 6475 6365   object (produce
-00004670: 6420 7573 696e 6720 6054 696d 6553 6572  d using `TimeSer
-00004680: 6965 732e 746f 5f6a 736f 6e28 2960 290a  ies.to_json()`).
-00004690: 2020 2020 2020 2020 696e 746f 2061 2060          into a `
-000046a0: 5469 6d65 5365 7269 6573 6020 6f62 6a65  TimeSeries` obje
-000046b0: 6374 0a0a 2020 2020 2020 2020 4174 2074  ct..        At t
-000046c0: 6865 206d 6f6d 656e 7420 7468 6973 206f  he moment this o
-000046d0: 6e6c 7920 7375 7070 6f72 7473 2064 6574  nly supports det
-000046e0: 6572 6d69 6e69 7374 6963 2074 696d 6520  erministic time 
-000046f0: 7365 7269 6573 2028 692e 652e 2c20 6d61  series (i.e., ma
-00004700: 6465 206f 6620 3120 7361 6d70 6c65 292e  de of 1 sample).
-00004710: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00004720: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-00004730: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00004740: 6a73 6f6e 5f73 7472 0a20 2020 2020 2020  json_str.       
-00004750: 2020 2020 2054 6865 204a 534f 4e20 5374       The JSON St
-00004760: 7269 6e67 2074 6f20 636f 6e76 6572 740a  ring to convert.
-00004770: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00004780: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00004790: 0a20 2020 2020 2020 2054 696d 6553 6572  .        TimeSer
-000047a0: 6965 730a 2020 2020 2020 2020 2020 2020  ies.            
-000047b0: 5468 6520 7469 6d65 2073 6572 6965 7320  The time series 
-000047c0: 6f62 6a65 6374 2063 6f6e 7665 7274 6564  object converted
-000047d0: 2066 726f 6d20 7468 6520 4a53 4f4e 2053   from the JSON S
-000047e0: 7472 696e 670a 2020 2020 2020 2020 2222  tring.        ""
-000047f0: 220a 2020 2020 2020 2020 6466 203d 2070  ".        df = p
-00004800: 642e 7265 6164 5f6a 736f 6e28 6a73 6f6e  d.read_json(json
-00004810: 5f73 7472 2c20 6f72 6965 6e74 3d27 7370  _str, orient='sp
-00004820: 6c69 7427 290a 2020 2020 2020 2020 7265  lit').        re
-00004830: 7475 726e 2054 696d 6553 6572 6965 732e  turn TimeSeries.
-00004840: 6672 6f6d 5f64 6174 6166 7261 6d65 2864  from_dataframe(d
-00004850: 6629 0a0a 2020 2020 2222 220a 2020 2020  f)..    """.    
-00004860: 5072 6f70 6572 7469 6573 0a20 2020 203d  Properties.    =
-00004870: 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020 2222  =========.    ""
-00004880: 220a 0a20 2020 2040 7072 6f70 6572 7479  "..    @property
-00004890: 0a20 2020 2064 6566 206e 5f73 616d 706c  .    def n_sampl
-000048a0: 6573 2873 656c 6629 3a0a 2020 2020 2020  es(self):.      
-000048b0: 2020 7265 7475 726e 206c 656e 2873 656c    return len(sel
-000048c0: 662e 5f78 612e 7361 6d70 6c65 290a 0a20  f._xa.sample).. 
-000048d0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-000048e0: 2064 6566 206e 5f63 6f6d 706f 6e65 6e74   def n_component
-000048f0: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
-00004900: 2072 6574 7572 6e20 6c65 6e28 7365 6c66   return len(self
-00004910: 2e5f 7861 2e63 6f6d 706f 6e65 6e74 290a  ._xa.component).
-00004920: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00004930: 2020 2064 6566 2077 6964 7468 2873 656c     def width(sel
-00004940: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-00004950: 726e 2073 656c 662e 6e5f 636f 6d70 6f6e  rn self.n_compon
-00004960: 656e 7473 0a0a 2020 2020 4070 726f 7065  ents..    @prope
-00004970: 7274 790a 2020 2020 6465 6620 6e5f 7469  rty.    def n_ti
-00004980: 6d65 7374 6570 7328 7365 6c66 293a 0a20  mesteps(self):. 
-00004990: 2020 2020 2020 2072 6574 7572 6e20 6c65         return le
-000049a0: 6e28 7365 6c66 2e5f 7469 6d65 5f69 6e64  n(self._time_ind
-000049b0: 6578 290a 0a20 2020 2040 7072 6f70 6572  ex)..    @proper
-000049c0: 7479 0a20 2020 2064 6566 2069 735f 6465  ty.    def is_de
-000049d0: 7465 726d 696e 6973 7469 6328 7365 6c66  terministic(self
-000049e0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-000049f0: 6e20 7365 6c66 2e6e 5f73 616d 706c 6573  n self.n_samples
-00004a00: 203d 3d20 310a 0a20 2020 2040 7072 6f70   == 1..    @prop
-00004a10: 6572 7479 0a20 2020 2064 6566 2069 735f  erty.    def is_
-00004a20: 7374 6f63 6861 7374 6963 2873 656c 6629  stochastic(self)
-00004a30: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00004a40: 206e 6f74 2073 656c 662e 6973 5f64 6574   not self.is_det
-00004a50: 6572 6d69 6e69 7374 6963 0a0a 2020 2020  erministic..    
-00004a60: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00004a70: 6620 6973 5f70 726f 6261 6269 6c69 7374  f is_probabilist
-00004a80: 6963 2873 656c 6629 3a0a 2020 2020 2020  ic(self):.      
-00004a90: 2020 7265 7475 726e 2073 656c 662e 6973    return self.is
-00004aa0: 5f73 746f 6368 6173 7469 630a 0a20 2020  _stochastic..   
-00004ab0: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00004ac0: 6566 2069 735f 756e 6976 6172 6961 7465  ef is_univariate
-00004ad0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00004ae0: 7265 7475 726e 2073 656c 662e 6e5f 636f  return self.n_co
-00004af0: 6d70 6f6e 656e 7473 203d 3d20 310a 0a20  mponents == 1.. 
-00004b00: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00004b10: 2064 6566 2066 7265 7128 7365 6c66 293a   def freq(self):
-00004b20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00004b30: 7365 6c66 2e5f 6672 6571 0a0a 2020 2020  self._freq..    
-00004b40: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00004b50: 6620 6672 6571 5f73 7472 2873 656c 6629  f freq_str(self)
-00004b60: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00004b70: 2073 656c 662e 5f66 7265 715f 7374 720a   self._freq_str.
-00004b80: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00004b90: 2020 2064 6566 2063 6f6d 706f 6e65 6e74     def component
-00004ba0: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
-00004bb0: 2022 2222 0a20 2020 2020 2020 2054 6865   """.        The
-00004bc0: 206e 616d 6573 206f 6620 7468 6520 636f   names of the co
-00004bd0: 6d70 6f6e 656e 7473 2028 6571 7569 7661  mponents (equiva
-00004be0: 6c65 6e74 2074 6f20 4461 7461 4672 616d  lent to DataFram
-00004bf0: 6520 636f 6c75 6d6e 7329 2061 7320 6120  e columns) as a 
-00004c00: 5061 6e64 6173 2049 6e64 6578 0a20 2020  Pandas Index.   
-00004c10: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00004c20: 2072 6574 7572 6e20 7365 6c66 2e5f 7861   return self._xa
-00004c30: 2e67 6574 5f69 6e64 6578 2844 494d 535b  .get_index(DIMS[
-00004c40: 315d 292e 636f 7079 2829 0a0a 2020 2020  1]).copy()..    
-00004c50: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
-00004c60: 6620 636f 6c75 6d6e 7328 7365 6c66 293a  f columns(self):
-00004c70: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00004c80: 2020 2020 2053 616d 6520 6173 2060 636f       Same as `co
-00004c90: 6d70 6f6e 656e 7473 6020 7072 6f70 6572  mponents` proper
-00004ca0: 7479 0a20 2020 2020 2020 2022 2222 0a20  ty.        """. 
-00004cb0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00004cc0: 6c66 2e63 6f6d 706f 6e65 6e74 730a 0a20  lf.components.. 
-00004cd0: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-00004ce0: 2064 6566 2074 696d 655f 696e 6465 7828   def time_index(
-00004cf0: 7365 6c66 2920 2d3e 2055 6e69 6f6e 5b70  self) -> Union[p
-00004d00: 642e 4461 7465 7469 6d65 496e 6465 782c  d.DatetimeIndex,
-00004d10: 2070 642e 5261 6e67 6549 6e64 6578 5d3a   pd.RangeIndex]:
-00004d20: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00004d30: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-00004d40: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-00004d50: 2020 2020 2055 6e69 6f6e 5b70 642e 4461       Union[pd.Da
-00004d60: 7465 7469 6d65 496e 6465 782c 2070 642e  tetimeIndex, pd.
-00004d70: 5261 6e67 6549 6e64 6578 5d0a 2020 2020  RangeIndex].    
-00004d80: 2020 2020 2020 2020 5468 6520 7469 6d65          The time
-00004d90: 2069 6e64 6578 206f 6620 7468 6973 2074   index of this t
-00004da0: 696d 6520 7365 7269 6573 2e0a 2020 2020  ime series..    
-00004db0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00004dc0: 7265 7475 726e 2073 656c 662e 5f74 696d  return self._tim
-00004dd0: 655f 696e 6465 782e 636f 7079 2829 0a0a  e_index.copy()..
-00004de0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
-00004df0: 2020 6465 6620 6861 735f 6461 7465 7469    def has_dateti
-00004e00: 6d65 5f69 6e64 6578 2873 656c 6629 202d  me_index(self) -
-00004e10: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
-00004e20: 2222 220a 2020 2020 2020 2020 5768 6574  """.        Whet
-00004e30: 6865 7220 7468 6973 2073 6572 6965 7320  her this series 
-00004e40: 6973 2069 6e64 6578 6564 2077 6974 6820  is indexed with 
-00004e50: 6120 4461 7465 7469 6d65 496e 6465 7820  a DatetimeIndex 
-00004e60: 286f 7468 6572 7769 7365 2069 7420 6973  (otherwise it is
-00004e70: 2069 6e64 6578 6564 2077 6974 6820 6120   indexed with a 
-00004e80: 5261 6e67 6549 6e64 6578 290a 2020 2020  RangeIndex).    
-00004e90: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00004ea0: 7265 7475 726e 2073 656c 662e 5f68 6173  return self._has
-00004eb0: 5f64 6174 6574 696d 655f 696e 6465 780a  _datetime_index.
-00004ec0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00004ed0: 2020 2064 6566 2068 6173 5f72 616e 6765     def has_range
-00004ee0: 5f69 6e64 6578 2873 656c 6629 202d 3e20  _index(self) -> 
-00004ef0: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
-00004f00: 220a 2020 2020 2020 2020 5768 6574 6865  ".        Whethe
-00004f10: 7220 7468 6973 2073 6572 6965 7320 6973  r this series is
-00004f20: 2069 6e64 6578 6564 2077 6974 6820 6120   indexed with a 
-00004f30: 5261 6e67 6549 6e64 6578 2028 6f74 6865  RangeIndex (othe
-00004f40: 7277 6973 6520 6974 2069 7320 696e 6465  rwise it is inde
-00004f50: 7865 6420 7769 7468 2061 2044 6174 6574  xed with a Datet
-00004f60: 696d 6549 6e64 6578 290a 2020 2020 2020  imeIndex).      
-00004f70: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
-00004f80: 7475 726e 206e 6f74 2073 656c 662e 5f68  turn not self._h
-00004f90: 6173 5f64 6174 6574 696d 655f 696e 6465  as_datetime_inde
-00004fa0: 780a 0a20 2020 2040 7072 6f70 6572 7479  x..    @property
-00004fb0: 0a20 2020 2064 6566 2064 7572 6174 696f  .    def duratio
-00004fc0: 6e28 7365 6c66 2920 2d3e 2055 6e69 6f6e  n(self) -> Union
-00004fd0: 5b70 642e 5469 6d65 6465 6c74 612c 2069  [pd.Timedelta, i
-00004fe0: 6e74 5d3a 0a20 2020 2020 2020 2022 2222  nt]:.        """
-00004ff0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00005000: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00005010: 0a20 2020 2020 2020 2055 6e69 6f6e 5b70  .        Union[p
-00005020: 616e 6461 732e 5469 6d65 6465 6c74 612c  andas.Timedelta,
-00005030: 2069 6e74 5d0a 2020 2020 2020 2020 2020   int].          
-00005040: 2020 5468 6520 6475 7261 7469 6f6e 206f    The duration o
-00005050: 6620 7468 6973 2074 696d 6520 7365 7269  f this time seri
-00005060: 6573 3b20 6173 2061 2054 696d 6564 656c  es; as a Timedel
-00005070: 7461 2069 6620 7468 6520 7365 7269 6573  ta if the series
-00005080: 2069 7320 696e 6465 7865 6420 6279 2061   is indexed by a
-00005090: 2044 6174 6574 696d 6569 6e64 6578 2c0a   Datetimeindex,.
-000050a0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-000050b0: 696e 7420 6f74 6865 7277 6973 652e 0a20  int otherwise.. 
-000050c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000050d0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-000050e0: 7469 6d65 5f69 6e64 6578 5b2d 315d 202d  time_index[-1] -
-000050f0: 2073 656c 662e 5f74 696d 655f 696e 6465   self._time_inde
-00005100: 785b 305d 0a0a 2020 2020 2222 2220 0a20  x[0]..    """ . 
-00005110: 2020 2053 6f6d 6520 6173 7365 7274 730a     Some asserts.
-00005120: 2020 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d      ============
-00005130: 3d0a 2020 2020 2222 220a 2020 2020 2320  =.    """.    # 
-00005140: 544f 444f 3a20 7075 7420 6174 2074 6865  TODO: put at the
-00005150: 2062 6f74 746f 6d0a 0a20 2020 2064 6566   bottom..    def
-00005160: 205f 6173 7365 7274 5f75 6e69 7661 7269   _assert_univari
-00005170: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-00005180: 2020 2069 6620 6e6f 7420 7365 6c66 2e69     if not self.i
-00005190: 735f 756e 6976 6172 6961 7465 3a0a 2020  s_univariate:.  
-000051a0: 2020 2020 2020 2020 2020 7261 6973 655f            raise_
-000051b0: 6c6f 6728 4173 7365 7274 696f 6e45 7272  log(AssertionErr
-000051c0: 6f72 2827 4f6e 6c79 2075 6e69 7661 7269  or('Only univari
-000051d0: 6174 6520 5469 6d65 5365 7269 6573 2069  ate TimeSeries i
-000051e0: 6e73 7461 6e63 6573 2073 7570 706f 7274  nstances support
-000051f0: 2074 6869 7320 6d65 7468 6f64 2729 2c20   this method'), 
-00005200: 6c6f 6767 6572 290a 0a20 2020 2064 6566  logger)..    def
-00005210: 205f 6173 7365 7274 5f64 6574 6572 6d69   _assert_determi
-00005220: 6e69 7374 6963 2873 656c 6629 3a0a 2020  nistic(self):.  
-00005230: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-00005240: 662e 6973 5f64 6574 6572 6d69 6e69 7374  f.is_determinist
-00005250: 6963 3a0a 2020 2020 2020 2020 2020 2020  ic:.            
-00005260: 7261 6973 655f 6c6f 6728 4173 7365 7274  raise_log(Assert
-00005270: 696f 6e45 7272 6f72 2827 4f6e 6c79 2064  ionError('Only d
-00005280: 6574 6572 6d69 6e69 7374 6963 2054 696d  eterministic Tim
-00005290: 6553 6572 6965 7320 2877 6974 6820 3120  eSeries (with 1 
-000052a0: 7361 6d70 6c65 2920 696e 7374 616e 6365  sample) instance
-000052b0: 7320 7375 7070 6f72 7420 7468 6973 206d  s support this m
-000052c0: 6574 686f 6427 292c 0a20 2020 2020 2020  ethod'),.       
-000052d0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-000052e0: 6f67 6765 7229 0a0a 2020 2020 6465 6620  ogger)..    def 
-000052f0: 5f61 7373 6572 745f 7374 6f63 6861 7374  _assert_stochast
-00005300: 6963 2873 656c 6629 3a0a 2020 2020 2020  ic(self):.      
-00005310: 2020 6966 206e 6f74 2073 656c 662e 6973    if not self.is
-00005320: 5f73 746f 6368 6173 7469 633a 0a20 2020  _stochastic:.   
-00005330: 2020 2020 2020 2020 2072 6169 7365 5f6c           raise_l
-00005340: 6f67 2841 7373 6572 7469 6f6e 4572 726f  og(AssertionErro
-00005350: 7228 274f 6e6c 7920 6e6f 6e2d 6465 7465  r('Only non-dete
-00005360: 726d 696e 6973 7469 6320 5469 6d65 5365  rministic TimeSe
-00005370: 7269 6573 2028 7769 7468 206d 6f72 6520  ries (with more 
-00005380: 7468 616e 2031 2073 616d 706c 6573 2920  than 1 samples) 
-00005390: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-000053a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053b0: 2020 2020 2020 2027 696e 7374 616e 6365         'instance
-000053c0: 7320 7375 7070 6f72 7420 7468 6973 206d  s support this m
-000053d0: 6574 686f 6427 292c 0a20 2020 2020 2020  ethod'),.       
-000053e0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-000053f0: 6f67 6765 7229 0a0a 2020 2020 6465 6620  ogger)..    def 
-00005400: 5f72 6169 7365 5f69 665f 6e6f 745f 7769  _raise_if_not_wi
-00005410: 7468 696e 2873 656c 662c 2074 733a 2055  thin(self, ts: U
-00005420: 6e69 6f6e 5b70 642e 5469 6d65 7374 616d  nion[pd.Timestam
-00005430: 702c 2069 6e74 5d29 3a0a 2020 2020 2020  p, int]):.      
-00005440: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00005450: 7473 2c20 7064 2e54 696d 6573 7461 6d70  ts, pd.Timestamp
-00005460: 293a 0a20 2020 2020 2020 2020 2020 2023  ):.            #
-00005470: 204e 6f74 2074 6861 7420 7468 6520 636f   Not that the co
-00005480: 6e76 6572 7365 2064 6f65 736e 2774 2061  nverse doesn't a
-00005490: 7070 6c79 2028 6120 7469 6d65 2d69 6e64  pply (a time-ind
-000054a0: 6578 6564 2073 6572 6965 7320 6361 6e20  exed series can 
-000054b0: 6265 2063 616c 6c65 6420 7769 7468 2061  be called with a
-000054c0: 6e20 696e 7465 6765 7229 0a20 2020 2020  n integer).     
-000054d0: 2020 2020 2020 2072 6169 7365 5f69 665f         raise_if_
-000054e0: 6e6f 7428 7365 6c66 2e5f 6861 735f 6461  not(self._has_da
-000054f0: 7465 7469 6d65 5f69 6e64 6578 2c0a 2020  tetime_index,.  
-00005500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005510: 2020 2020 2020 2027 4675 6e63 7469 6f6e         'Function
-00005520: 2063 616c 6c65 6420 7769 7468 2061 2074   called with a t
-00005530: 696d 6573 7461 6d70 2c20 6275 7420 7365  imestamp, but se
-00005540: 7269 6573 206e 6f74 2074 696d 652d 696e  ries not time-in
-00005550: 6465 7865 642e 272c 0a20 2020 2020 2020  dexed.',.       
-00005560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005570: 2020 6c6f 6767 6572 290a 2020 2020 2020    logger).      
-00005580: 2020 2020 2020 6973 5f69 6e73 6964 6520        is_inside 
-00005590: 3d20 7365 6c66 2e73 7461 7274 5f74 696d  = self.start_tim
-000055a0: 6528 2920 3c3d 2074 7320 3c3d 2073 656c  e() <= ts <= sel
-000055b0: 662e 656e 645f 7469 6d65 2829 0a20 2020  f.end_time().   
-000055c0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000055d0: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
-000055e0: 6861 735f 6461 7465 7469 6d65 5f69 6e64  has_datetime_ind
-000055f0: 6578 3a0a 2020 2020 2020 2020 2020 2020  ex:.            
-00005600: 2020 2020 6973 5f69 6e73 6964 6520 3d20      is_inside = 
-00005610: 3020 3c3d 2074 7320 3c3d 206c 656e 2873  0 <= ts <= len(s
-00005620: 656c 6629 0a20 2020 2020 2020 2020 2020  elf).           
-00005630: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00005640: 2020 2020 2020 2069 735f 696e 7369 6465         is_inside
-00005650: 203d 2073 656c 662e 7374 6172 745f 7469   = self.start_ti
-00005660: 6d65 2829 203c 3d20 7473 203c 3d20 7365  me() <= ts <= se
-00005670: 6c66 2e65 6e64 5f74 696d 6528 290a 0a20  lf.end_time().. 
-00005680: 2020 2020 2020 2072 6169 7365 5f69 665f         raise_if_
-00005690: 6e6f 7428 6973 5f69 6e73 6964 652c 2027  not(is_inside, '
-000056a0: 5469 6d65 7374 616d 7020 6d75 7374 2062  Timestamp must b
-000056b0: 6520 6265 7477 6565 6e20 7b7d 2061 6e64  e between {} and
-000056c0: 207b 7d27 2e66 6f72 6d61 7428 7365 6c66   {}'.format(self
-000056d0: 2e73 7461 7274 5f74 696d 6528 292c 0a20  .start_time(),. 
-000056e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005720: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00005730: 2e65 6e64 5f74 696d 6528 2929 2c0a 2020  .end_time()),.  
-00005740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005750: 2020 206c 6f67 6765 7229 0a0a 2020 2020     logger)..    
-00005760: 6465 6620 5f67 6574 5f66 6972 7374 5f74  def _get_first_t
-00005770: 696d 6573 7461 6d70 5f61 6674 6572 2873  imestamp_after(s
-00005780: 656c 662c 2074 733a 2070 642e 5469 6d65  elf, ts: pd.Time
-00005790: 7374 616d 7029 202d 3e20 7064 2e54 696d  stamp) -> pd.Tim
-000057a0: 6573 7461 6d70 3a0a 2020 2020 2020 2020  estamp:.        
-000057b0: 7265 7475 726e 206e 6578 7428 6669 6c74  return next(filt
-000057c0: 6572 286c 616d 6264 6120 743a 2074 203e  er(lambda t: t >
-000057d0: 3d20 7473 2c20 7365 6c66 2e5f 7469 6d65  = ts, self._time
-000057e0: 5f69 6e64 6578 2929 0a0a 2020 2020 6465  _index))..    de
-000057f0: 6620 5f67 6574 5f6c 6173 745f 7469 6d65  f _get_last_time
-00005800: 7374 616d 705f 6265 666f 7265 2873 656c  stamp_before(sel
-00005810: 662c 2074 733a 2070 642e 5469 6d65 7374  f, ts: pd.Timest
-00005820: 616d 7029 202d 3e20 7064 2e54 696d 6573  amp) -> pd.Times
-00005830: 7461 6d70 3a0a 2020 2020 2020 2020 7265  tamp:.        re
-00005840: 7475 726e 206e 6578 7428 6669 6c74 6572  turn next(filter
-00005850: 286c 616d 6264 6120 743a 2074 203c 3d20  (lambda t: t <= 
-00005860: 7473 2c20 7365 6c66 2e5f 7469 6d65 5f69  ts, self._time_i
-00005870: 6e64 6578 5b3a 3a2d 315d 2929 0a0a 2020  ndex[::-1]))..  
-00005880: 2020 2222 220a 2020 2020 4578 706f 7274    """.    Export
-00005890: 2066 756e 6374 696f 6e73 0a20 2020 203d   functions.    =
-000058a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
-000058b0: 2020 2020 2222 220a 0a20 2020 2064 6566      """..    def
-000058c0: 2064 6174 615f 6172 7261 7928 7365 6c66   data_array(self
-000058d0: 2c20 636f 7079 3d54 7275 6529 202d 3e20  , copy=True) -> 
-000058e0: 7872 2e44 6174 6141 7272 6179 3a0a 2020  xr.DataArray:.  
-000058f0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00005900: 2020 5265 7475 726e 7320 7468 6520 7861    Returns the xa
-00005910: 7272 6179 2044 6174 6141 7272 6179 2072  rray DataArray r
-00005920: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
-00005930: 2074 6869 7320 7469 6d65 2073 6572 6965   this time serie
-00005940: 732e 0a0a 2020 2020 2020 2020 5061 7261  s...        Para
-00005950: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-00005960: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-00005970: 2020 636f 7079 0a20 2020 2020 2020 2020    copy.         
-00005980: 2020 2057 6865 7468 6572 2074 6f20 7265     Whether to re
-00005990: 7475 726e 2061 2063 6f70 7920 6f66 2074  turn a copy of t
-000059a0: 6865 2073 6572 6965 732e 204c 6561 7665  he series. Leave
-000059b0: 2069 7420 746f 2054 7275 6520 756e 6c65   it to True unle
-000059c0: 7373 2079 6f75 206b 6e6f 7720 7768 6174  ss you know what
-000059d0: 2079 6f75 2061 7265 2064 6f69 6e67 2e0a   you are doing..
-000059e0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-000059f0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00005a00: 0a20 2020 2020 2020 2078 6172 7261 792e  .        xarray.
-00005a10: 4461 7461 4172 7261 790a 2020 2020 2020  DataArray.      
-00005a20: 2020 2020 2020 5468 6520 7861 7272 6179        The xarray
-00005a30: 2044 6174 6141 7272 6179 2075 6e64 6572   DataArray under
-00005a40: 6c79 696e 6720 7468 6973 2074 696d 6520  lying this time 
-00005a50: 7365 7269 6573 2e0a 2020 2020 2020 2020  series..        
-00005a60: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-00005a70: 726e 2073 656c 662e 5f78 612e 636f 7079  rn self._xa.copy
-00005a80: 2829 2069 6620 636f 7079 2065 6c73 6520  () if copy else 
-00005a90: 7365 6c66 2e5f 7861 0a0a 2020 2020 6465  self._xa..    de
-00005aa0: 6620 7064 5f73 6572 6965 7328 7365 6c66  f pd_series(self
-00005ab0: 2c20 636f 7079 3d54 7275 6529 202d 3e20  , copy=True) -> 
-00005ac0: 7064 2e53 6572 6965 733a 0a20 2020 2020  pd.Series:.     
-00005ad0: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-00005ae0: 6574 7572 6e73 2061 2050 616e 6461 7320  eturns a Pandas 
-00005af0: 5365 7269 6573 2072 6570 7265 7365 6e74  Series represent
-00005b00: 6174 696f 6e20 6f66 2074 6869 7320 7469  ation of this ti
-00005b10: 6d65 2073 6572 6965 732e 0a20 2020 2020  me series..     
-00005b20: 2020 2057 6f72 6b73 206f 6e6c 7920 666f     Works only fo
-00005b30: 7220 756e 6976 6172 6961 7465 2073 6572  r univariate ser
-00005b40: 6965 7320 7468 6174 2061 7265 2064 6574  ies that are det
-00005b50: 6572 6d69 6e69 7374 6963 2028 692e 652e  erministic (i.e.
-00005b60: 2c20 6d61 6465 206f 6620 3120 7361 6d70  , made of 1 samp
-00005b70: 6c65 292e 0a0a 2020 2020 2020 2020 5061  le)...        Pa
-00005b80: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-00005b90: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00005ba0: 2020 2020 636f 7079 0a20 2020 2020 2020      copy.       
-00005bb0: 2020 2020 2057 6865 7468 6572 2074 6f20       Whether to 
-00005bc0: 7265 7475 726e 2061 2063 6f70 7920 6f66  return a copy of
-00005bd0: 2074 6865 2073 6572 6965 732e 204c 6561   the series. Lea
-00005be0: 7665 2069 7420 746f 2054 7275 6520 756e  ve it to True un
-00005bf0: 6c65 7373 2079 6f75 206b 6e6f 7720 7768  less you know wh
-00005c00: 6174 2079 6f75 2061 7265 2064 6f69 6e67  at you are doing
-00005c10: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00005c20: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
-00005c30: 2d2d 0a20 2020 2020 2020 2070 616e 6461  --.        panda
-00005c40: 732e 5365 7269 6573 0a20 2020 2020 2020  s.Series.       
-00005c50: 2020 2020 2041 2050 616e 6461 7320 5365       A Pandas Se
-00005c60: 7269 6573 2072 6570 7265 7365 6e74 6174  ries representat
-00005c70: 696f 6e20 6f66 2074 6869 7320 756e 6976  ion of this univ
-00005c80: 6172 6961 7465 2074 696d 6520 7365 7269  ariate time seri
-00005c90: 6573 2e0a 2020 2020 2020 2020 2222 220a  es..        """.
-00005ca0: 2020 2020 2020 2020 7365 6c66 2e5f 6173          self._as
-00005cb0: 7365 7274 5f75 6e69 7661 7269 6174 6528  sert_univariate(
-00005cc0: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
-00005cd0: 6173 7365 7274 5f64 6574 6572 6d69 6e69  assert_determini
-00005ce0: 7374 6963 2829 0a20 2020 2020 2020 2069  stic().        i
-00005cf0: 6620 636f 7079 3a0a 2020 2020 2020 2020  f copy:.        
-00005d00: 2020 2020 7265 7475 726e 2070 642e 5365      return pd.Se
-00005d10: 7269 6573 2873 656c 662e 5f78 615b 3a2c  ries(self._xa[:,
-00005d20: 2030 2c20 305d 2e63 6f70 7928 292c 2069   0, 0].copy(), i
-00005d30: 6e64 6578 3d73 656c 662e 5f74 696d 655f  ndex=self._time_
-00005d40: 696e 6465 782e 636f 7079 2829 290a 2020  index.copy()).  
-00005d50: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00005d60: 2020 2020 2020 2020 7265 7475 726e 2070          return p
-00005d70: 642e 5365 7269 6573 2873 656c 662e 5f78  d.Series(self._x
-00005d80: 615b 3a2c 2030 2c20 305d 2c20 696e 6465  a[:, 0, 0], inde
-00005d90: 783d 7365 6c66 2e5f 7469 6d65 5f69 6e64  x=self._time_ind
-00005da0: 6578 290a 0a20 2020 2064 6566 2070 645f  ex)..    def pd_
-00005db0: 6461 7461 6672 616d 6528 7365 6c66 2c20  dataframe(self, 
-00005dc0: 636f 7079 3d54 7275 6529 202d 3e20 7064  copy=True) -> pd
-00005dd0: 2e44 6174 6146 7261 6d65 3a0a 2020 2020  .DataFrame:.    
-00005de0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00005df0: 5265 7475 726e 7320 6120 5061 6e64 6173  Returns a Pandas
-00005e00: 2044 6174 6146 7261 6d65 2072 6570 7265   DataFrame repre
-00005e10: 7365 6e74 6174 696f 6e20 6f66 2074 6869  sentation of thi
-00005e20: 7320 7469 6d65 2073 6572 6965 732e 0a20  s time series.. 
-00005e30: 2020 2020 2020 2045 6163 6820 6f66 2074         Each of t
-00005e40: 6865 2073 6572 6965 7320 636f 6d70 6f6e  he series compon
-00005e50: 656e 7473 2077 696c 6c20 6170 7065 6172  ents will appear
-00005e60: 2061 7320 6120 636f 6c75 6d6e 2069 6e20   as a column in 
-00005e70: 7468 6520 4461 7461 4672 616d 652e 0a20  the DataFrame.. 
-00005e80: 2020 2020 2020 2057 6f72 6b73 206f 6e6c         Works onl
-00005e90: 7920 666f 7220 6465 7465 726d 696e 6973  y for determinis
-00005ea0: 7469 6320 7365 7269 6573 2028 692e 652e  tic series (i.e.
-00005eb0: 2c20 6d61 6465 206f 6620 3120 7361 6d70  , made of 1 samp
-00005ec0: 6c65 292e 0a0a 2020 2020 2020 2020 5061  le)...        Pa
-00005ed0: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-00005ee0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00005ef0: 2020 2020 636f 7079 0a20 2020 2020 2020      copy.       
-00005f00: 2020 2020 2057 6865 7468 6572 2074 6f20       Whether to 
-00005f10: 7265 7475 726e 2061 2063 6f70 7920 6f66  return a copy of
-00005f20: 2074 6865 2064 6174 6166 7261 6d65 2e20   the dataframe. 
-00005f30: 4c65 6176 6520 6974 2074 6f20 5472 7565  Leave it to True
-00005f40: 2075 6e6c 6573 7320 796f 7520 6b6e 6f77   unless you know
-00005f50: 2077 6861 7420 796f 7520 6172 6520 646f   what you are do
-00005f60: 696e 672e 0a0a 2020 2020 2020 2020 5265  ing...        Re
-00005f70: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
-00005f80: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7061  -----.        pa
-00005f90: 6e64 6173 2e44 6174 6146 7261 6d65 0a20  ndas.DataFrame. 
-00005fa0: 2020 2020 2020 2020 2020 2054 6865 2050             The P
-00005fb0: 616e 6461 7320 4461 7461 4672 616d 6520  andas DataFrame 
-00005fc0: 7265 7072 6573 656e 7461 7469 6f6e 206f  representation o
-00005fd0: 6620 7468 6973 2074 696d 6520 7365 7269  f this time seri
-00005fe0: 6573 0a20 2020 2020 2020 2022 2222 0a20  es.        """. 
-00005ff0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-00006000: 6c66 2e69 735f 6465 7465 726d 696e 6973  lf.is_determinis
-00006010: 7469 633a 0a20 2020 2020 2020 2020 2020  tic:.           
-00006020: 2072 6169 7365 5f6c 6f67 2841 7373 6572   raise_log(Asser
-00006030: 7469 6f6e 4572 726f 7228 2754 6865 2070  tionError('The p
-00006040: 645f 6461 7461 6672 616d 6528 2920 6d65  d_dataframe() me
-00006050: 7468 6f64 2063 616e 206f 6e6c 7920 7265  thod can only re
-00006060: 7475 726e 2044 6174 6146 7261 6d65 7320  turn DataFrames 
-00006070: 6f66 2064 6574 6572 6d69 6e69 7374 6963  of deterministic
-00006080: 2027 0a20 2020 2020 2020 2020 2020 2020   '.             
-00006090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060a0: 2020 2020 2020 2020 2774 696d 6520 7365          'time se
-000060b0: 7269 6573 2c20 616e 6420 7468 6973 2073  ries, and this s
-000060c0: 6572 6965 7320 6973 206e 6f74 2064 6574  eries is not det
-000060d0: 6572 6d69 6e69 7374 6963 2028 6974 2063  erministic (it c
-000060e0: 6f6e 7461 696e 7320 7365 7665 7261 6c20  ontains several 
-000060f0: 7361 6d70 6c65 7329 2e20 270a 2020 2020  samples). '.    
-00006100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006120: 2027 436f 6e73 6964 6572 2063 616c 6c69   'Consider calli
-00006130: 6e67 2071 7561 6e74 696c 655f 6466 2829  ng quantile_df()
-00006140: 2069 6e73 7465 6164 2e27 2929 0a20 2020   instead.')).   
-00006150: 2020 2020 2069 6620 636f 7079 3a0a 2020       if copy:.  
-00006160: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00006170: 2070 642e 4461 7461 4672 616d 6528 7365   pd.DataFrame(se
-00006180: 6c66 2e5f 7861 5b3a 2c20 3a2c 2030 5d2e  lf._xa[:, :, 0].
-00006190: 7661 6c75 6573 2e63 6f70 7928 292c 0a20  values.copy(),. 
-000061a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000061c0: 6e64 6578 3d73 656c 662e 5f74 696d 655f  ndex=self._time_
-000061d0: 696e 6465 782e 636f 7079 2829 2c0a 2020  index.copy(),.  
+00001480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001490: 2027 7472 7920 7370 6563 6966 7969 6e67   'try specifying
+000014a0: 2060 6669 6c6c 5f6d 6973 7369 6e67 5f64   `fill_missing_d
+000014b0: 6174 6573 3d54 7275 6560 2027 0a20 2020  ates=True` '.   
+000014c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014e0: 2020 2020 2020 2020 2027 6f72 2073 7065           'or spe
+000014f0: 6369 6679 2074 6865 2060 6672 6571 6020  cify the `freq` 
+00001500: 7061 7261 6d65 7465 722e 272c 206c 6f67  parameter.', log
+00001510: 6765 7229 0a20 2020 2020 2020 2065 6c73  ger).        els
+00001520: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00001530: 656c 662e 5f66 7265 7120 3d20 310a 2020  elf._freq = 1.  
+00001540: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00001550: 6672 6571 5f73 7472 203d 204e 6f6e 650a  freq_str = None.
+00001560: 0a20 2020 2022 2222 200a 2020 2020 4661  .    """ .    Fa
+00001570: 6374 6f72 7920 4d65 7468 6f64 730a 2020  ctory Methods.  
+00001580: 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d    ==============
+00001590: 3d0a 2020 2020 2222 220a 0a20 2020 2040  =.    """..    @
+000015a0: 7374 6174 6963 6d65 7468 6f64 0a20 2020  staticmethod.   
+000015b0: 2064 6566 2066 726f 6d5f 7861 7272 6179   def from_xarray
+000015c0: 2878 613a 2078 722e 4461 7461 4172 7261  (xa: xr.DataArra
+000015d0: 792c 0a20 2020 2020 2020 2020 2020 2020  y,.             
+000015e0: 2020 2020 2020 2066 696c 6c5f 6d69 7373         fill_miss
+000015f0: 696e 675f 6461 7465 733a 204f 7074 696f  ing_dates: Optio
+00001600: 6e61 6c5b 626f 6f6c 5d20 3d20 4661 6c73  nal[bool] = Fals
+00001610: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00001620: 2020 2020 2020 2066 7265 713a 204f 7074         freq: Opt
+00001630: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
+00001640: 6529 202d 3e20 2754 696d 6553 6572 6965  e) -> 'TimeSerie
+00001650: 7327 3a0a 2020 2020 2020 2020 2222 220a  s':.        """.
+00001660: 2020 2020 2020 2020 5265 7475 726e 7320          Returns 
+00001670: 6120 5469 6d65 5365 7269 6573 2069 6e73  a TimeSeries ins
+00001680: 7461 6e63 6520 6275 696c 7420 6672 6f6d  tance built from
+00001690: 2061 6e20 7861 7272 6179 2044 6174 6141   an xarray DataA
+000016a0: 7272 6179 2e0a 2020 2020 2020 2020 5468  rray..        Th
+000016b0: 6520 6469 6d65 6e73 696f 6e73 206f 6620  e dimensions of 
+000016c0: 7468 6520 4461 7461 4172 7261 7920 6861  the DataArray ha
+000016d0: 7665 2074 6f20 6265 2028 7469 6d65 2c20  ve to be (time, 
+000016e0: 636f 6d70 6f6e 656e 742c 2073 616d 706c  component, sampl
+000016f0: 6529 2c20 696e 2074 6869 7320 6f72 6465  e), in this orde
+00001700: 722e 2054 6865 2074 696d 650a 2020 2020  r. The time.    
+00001710: 2020 2020 6469 6d65 6e73 696f 6e20 6361      dimension ca
+00001720: 6e20 6861 7665 2061 6e20 6172 6269 7472  n have an arbitr
+00001730: 6172 7920 6e61 6d65 2c20 6275 7420 636f  ary name, but co
+00001740: 6d70 6f6e 656e 7420 616e 6420 7361 6d70  mponent and samp
+00001750: 6c65 206d 7573 7420 6265 206e 616d 6564  le must be named
+00001760: 2022 636f 6d70 6f6e 656e 7422 2061 6e64   "component" and
+00001770: 2022 7361 6d70 6c65 222c 0a20 2020 2020   "sample",.     
+00001780: 2020 2072 6573 7065 6374 6976 656c 792e     respectively.
+00001790: 0a0a 2020 2020 2020 2020 5468 6520 6669  ..        The fi
+000017a0: 7273 7420 6469 6d65 6e73 696f 6e20 2874  rst dimension (t
+000017b0: 696d 6529 2c20 616e 6420 7365 636f 6e64  ime), and second
+000017c0: 2064 696d 656e 7369 6f6e 2028 636f 6d70   dimension (comp
+000017d0: 6f6e 656e 7429 206d 7573 7420 6265 2069  onent) must be i
+000017e0: 6e64 6578 6564 2028 692e 652e 2c20 6861  ndexed (i.e., ha
+000017f0: 7665 2063 6f6f 7264 696e 6174 6573 292e  ve coordinates).
+00001800: 0a20 2020 2020 2020 2054 6865 2074 696d  .        The tim
+00001810: 6520 6d75 7374 2062 6520 696e 6465 7865  e must be indexe
+00001820: 6420 6569 7468 6572 2077 6974 6820 6120  d either with a 
+00001830: 7061 6e64 6173 2044 6174 6574 696d 6549  pandas DatetimeI
+00001840: 6e64 6578 206f 7220 6120 7061 6e64 6173  ndex or a pandas
+00001850: 2049 6e74 3634 496e 6465 782e 2049 6620   Int64Index. If 
+00001860: 6120 4461 7465 7469 6d65 496e 6465 7820  a DatetimeIndex 
+00001870: 6973 0a20 2020 2020 2020 2075 7365 642c  is.        used,
+00001880: 2069 7420 6973 2062 6574 7465 7220 6966   it is better if
+00001890: 2069 7420 6861 7320 6e6f 2068 6f6c 6573   it has no holes
+000018a0: 3b20 616c 7468 6f75 6768 2073 6574 7469  ; although setti
+000018b0: 6e67 2060 6669 6c6c 5f6d 6973 7369 6e67  ng `fill_missing
+000018c0: 5f64 6174 6573 6020 6361 6e20 696e 2073  _dates` can in s
+000018d0: 6f6d 6520 6361 7365 7320 736f 6c76 6520  ome cases solve 
+000018e0: 7468 6573 650a 2020 2020 2020 2020 6973  these.        is
+000018f0: 7375 6573 2028 6669 6c6c 696e 6720 686f  sues (filling ho
+00001900: 6c65 7320 7769 7468 204e 614e 2920 6174  les with NaN) at
+00001910: 2061 2070 6572 666f 726d 616e 6365 2063   a performance c
+00001920: 6f73 742e 0a0a 2020 2020 2020 2020 4966  ost...        If
+00001930: 2074 776f 2063 6f6d 706f 6e65 6e74 7320   two components 
+00001940: 6861 7665 2074 6865 2073 616d 6520 6e61  have the same na
+00001950: 6d65 206f 7220 6172 6520 6e6f 7420 7374  me or are not st
+00001960: 7269 6e67 732c 2074 6869 7320 6d65 7468  rings, this meth
+00001970: 6f64 2077 696c 6c20 6469 7361 6d62 6967  od will disambig
+00001980: 7561 7465 2074 6865 2063 6f6d 706f 6e65  uate the compone
+00001990: 6e74 730a 2020 2020 2020 2020 6e61 6d65  nts.        name
+000019a0: 7320 6279 2061 7070 656e 6469 6e67 2061  s by appending a
+000019b0: 2073 7566 6669 7820 6f66 2074 6865 2066   suffix of the f
+000019c0: 6f72 6d20 223c 6e61 6d65 3e5f 4e22 2074  orm "<name>_N" t
+000019d0: 6f20 7468 6520 4e2d 7468 2063 6f6c 756d  o the N-th colum
+000019e0: 6e20 7769 7468 206e 616d 6520 226e 616d  n with name "nam
+000019f0: 6522 2e0a 0a20 2020 2020 2020 2050 6172  e"...        Par
+00001a00: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+00001a10: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00001a20: 2020 2078 610a 2020 2020 2020 2020 2020     xa.          
+00001a30: 2020 5468 6520 7861 7272 6179 2044 6174    The xarray Dat
+00001a40: 6141 7272 6179 0a20 2020 2020 2020 2066  aArray.        f
+00001a50: 696c 6c5f 6d69 7373 696e 675f 6461 7465  ill_missing_date
+00001a60: 730a 2020 2020 2020 2020 2020 2020 4f70  s.            Op
+00001a70: 7469 6f6e 616c 6c79 2c20 6120 626f 6f6c  tionally, a bool
+00001a80: 6561 6e20 7661 6c75 6520 696e 6469 6361  ean value indica
+00001a90: 7469 6e67 2077 6865 7468 6572 2074 6f20  ting whether to 
+00001aa0: 6669 6c6c 206d 6973 7369 6e67 2064 6174  fill missing dat
+00001ab0: 6573 2077 6974 6820 4e61 4e20 7661 6c75  es with NaN valu
+00001ac0: 6573 2e20 5468 6973 2072 6571 7569 7265  es. This require
+00001ad0: 730a 2020 2020 2020 2020 2020 2020 6569  s.            ei
+00001ae0: 7468 6572 2061 2070 726f 7669 6465 6420  ther a provided 
+00001af0: 6066 7265 7160 206f 7220 7468 6520 706f  `freq` or the po
+00001b00: 7373 6962 696c 6974 7920 746f 2069 6e66  ssibility to inf
+00001b10: 6572 2074 6865 2066 7265 7175 656e 6379  er the frequency
+00001b20: 2066 726f 6d20 7468 6520 7072 6f76 6964   from the provid
+00001b30: 6564 2074 696d 6573 7461 6d70 732e 0a20  ed timestamps.. 
+00001b40: 2020 2020 2020 2020 2020 2049 6e66 6572             Infer
+00001b50: 7269 6e67 2074 6865 2066 7265 7175 656e  ring the frequen
+00001b60: 6379 2061 6e64 2072 6573 616d 706c 696e  cy and resamplin
+00001b70: 6720 7468 6520 6461 7461 2063 616e 2069  g the data can i
+00001b80: 6e64 7563 6520 6120 7369 676e 6966 6963  nduce a signific
+00001b90: 616e 7420 7065 7266 6f72 6d61 6e63 6520  ant performance 
+00001ba0: 6f76 6572 6865 6164 2e0a 2020 2020 2020  overhead..      
+00001bb0: 2020 6672 6571 0a20 2020 2020 2020 2020    freq.         
+00001bc0: 2020 204f 7074 696f 6e61 6c6c 792c 2061     Optionally, a
+00001bd0: 2073 7472 696e 6720 7265 7072 6573 656e   string represen
+00001be0: 7469 6e67 2074 6865 2066 7265 7175 656e  ting the frequen
+00001bf0: 6379 206f 6620 7468 6520 5061 6e64 6173  cy of the Pandas
+00001c00: 2044 6174 6146 7261 6d65 2e20 5468 6973   DataFrame. This
+00001c10: 2069 7320 7573 6566 756c 2069 6e20 6f72   is useful in or
+00001c20: 6465 7220 746f 2066 696c 6c0a 2020 2020  der to fill.    
+00001c30: 2020 2020 2020 2020 696e 206d 6973 7369          in missi
+00001c40: 6e67 2076 616c 7565 7320 6966 2073 6f6d  ng values if som
+00001c50: 6520 6461 7465 7320 6172 6520 6d69 7373  e dates are miss
+00001c60: 696e 6720 616e 6420 6066 696c 6c5f 6d69  ing and `fill_mi
+00001c70: 7373 696e 675f 6461 7465 7360 2069 7320  ssing_dates` is 
+00001c80: 7365 7420 746f 2060 5472 7565 602e 0a0a  set to `True`...
+00001c90: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+00001ca0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+00001cb0: 2020 2020 2020 2020 5469 6d65 5365 7269          TimeSeri
+00001cc0: 6573 0a20 2020 2020 2020 2020 2020 2041  es.            A
+00001cd0: 2075 6e69 7661 7269 6174 6520 6f72 206d   univariate or m
+00001ce0: 756c 7469 7661 7269 6174 6520 6465 7465  ultivariate dete
+00001cf0: 726d 696e 6973 7469 6320 5469 6d65 5365  rministic TimeSe
+00001d00: 7269 6573 2063 6f6e 7374 7275 6374 6564  ries constructed
+00001d10: 2066 726f 6d20 7468 6520 696e 7075 7473   from the inputs
+00001d20: 2e0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
+00001d30: 2020 2020 2020 2023 206f 7074 696f 6e61         # optiona
+00001d40: 6c6c 7920 6669 6c6c 206d 6973 7369 6e67  lly fill missing
+00001d50: 2064 6174 6573 3b20 646f 2069 7420 6f6e   dates; do it on
+00001d60: 6c79 2077 6865 6e20 7468 6572 6520 6973  ly when there is
+00001d70: 2061 2044 6174 6574 696d 6549 6e64 6578   a DatetimeIndex
+00001d80: 2028 616e 6420 6e6f 7420 6120 496e 7436   (and not a Int6
+00001d90: 3449 6e64 6578 290a 2020 2020 2020 2020  4Index).        
+00001da0: 6966 2066 696c 6c5f 6d69 7373 696e 675f  if fill_missing_
+00001db0: 6461 7465 7320 616e 6420 6973 696e 7374  dates and isinst
+00001dc0: 616e 6365 2878 612e 6765 745f 696e 6465  ance(xa.get_inde
+00001dd0: 7828 7861 2e64 696d 735b 305d 292c 2070  x(xa.dims[0]), p
+00001de0: 642e 4461 7465 7469 6d65 496e 6465 7829  d.DatetimeIndex)
+00001df0: 3a0a 2020 2020 2020 2020 2020 2020 736f  :.            so
+00001e00: 7274 6564 5f78 6120 3d20 7861 2e73 6f72  rted_xa = xa.sor
+00001e10: 7462 7928 7861 2e64 696d 735b 305d 290a  tby(xa.dims[0]).
+00001e20: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+00001e30: 5f69 6e64 6578 203d 2073 6f72 7465 645f  _index = sorted_
+00001e40: 7861 2e67 6574 5f69 6e64 6578 2878 612e  xa.get_index(xa.
+00001e50: 6469 6d73 5b30 5d29 0a0a 2020 2020 2020  dims[0])..      
+00001e60: 2020 2020 2020 6966 206e 6f74 2066 7265        if not fre
+00001e70: 713a 0a20 2020 2020 2020 2020 2020 2020  q:.             
+00001e80: 2020 2023 2046 4958 4d45 3a20 5468 6973     # FIXME: This
+00001e90: 2069 7320 7461 6b69 6e67 206c 6f6e 672c   is taking long,
+00001ea0: 2065 7370 6563 6961 6c6c 7920 6f6e 206c   especially on l
+00001eb0: 6f6e 6765 7220 7365 7269 6573 0a20 2020  onger series.   
+00001ec0: 2020 2020 2020 2020 2020 2020 2023 2046               # F
+00001ed0: 4958 4d45 3a20 626f 7468 2063 6f6e 7374  IXME: both const
+00001ee0: 7275 6374 696e 6720 6f62 7365 7276 6564  ructing observed
+00001ef0: 5f66 7265 7175 656e 6369 6573 2c20 6173  _frequencies, as
+00001f00: 2077 656c 6c20 6173 2072 6573 616d 706c   well as resampl
+00001f10: 696e 6720 7468 6520 4461 7461 4172 7261  ing the DataArra
+00001f20: 7920 6172 6520 7461 6b69 6e67 206c 6f6e  y are taking lon
+00001f30: 670a 2020 2020 2020 2020 2020 2020 2020  g.              
+00001f40: 2020 2320 4649 584d 453a 2063 616e 2077    # FIXME: can w
+00001f50: 6520 646f 2062 6574 7465 723f 0a20 2020  e do better?.   
+00001f60: 2020 2020 2020 2020 2020 2020 2073 616d               sam
+00001f70: 706c 6573 5f73 697a 6520 3d20 330a 2020  ples_size = 3.  
+00001f80: 2020 2020 2020 2020 2020 2020 2020 6f62                ob
+00001f90: 7365 7276 6564 5f66 7265 7175 656e 6369  served_frequenci
+00001fa0: 6573 203d 205b 0a20 2020 2020 2020 2020  es = [.         
+00001fb0: 2020 2020 2020 2020 2020 2074 696d 655f             time_
+00001fc0: 696e 6465 785b 783a 7820 2b20 7361 6d70  index[x:x + samp
+00001fd0: 6c65 735f 7369 7a65 5d2e 696e 6665 7272  les_size].inferr
+00001fe0: 6564 5f66 7265 710a 2020 2020 2020 2020  ed_freq.        
+00001ff0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00002000: 780a 2020 2020 2020 2020 2020 2020 2020  x.              
+00002010: 2020 2020 2020 696e 2072 616e 6765 286c        in range(l
+00002020: 656e 2874 696d 655f 696e 6465 7829 202d  en(time_index) -
+00002030: 2073 616d 706c 6573 5f73 697a 6520 2b20   samples_size + 
+00002040: 3129 5d0a 0a20 2020 2020 2020 2020 2020  1)]..           
+00002050: 2020 2020 206f 6273 6572 7665 645f 6672       observed_fr
+00002060: 6571 7565 6e63 6965 7320 3d20 7365 7428  equencies = set(
+00002070: 6669 6c74 6572 284e 6f6e 652e 5f5f 6e65  filter(None.__ne
+00002080: 5f5f 2c20 6f62 7365 7276 6564 5f66 7265  __, observed_fre
+00002090: 7175 656e 6369 6573 2929 0a0a 2020 2020  quencies))..    
+000020a0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+000020b0: 655f 6966 5f6e 6f74 280a 2020 2020 2020  e_if_not(.      
+000020c0: 2020 2020 2020 2020 2020 2020 2020 6c65                le
+000020d0: 6e28 6f62 7365 7276 6564 5f66 7265 7175  n(observed_frequ
+000020e0: 656e 6369 6573 2920 3d3d 2031 2c0a 2020  encies) == 1,.  
+000020f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002100: 2020 2243 6f75 6c64 206e 6f74 2069 6e66    "Could not inf
+00002110: 6572 2065 7870 6c69 6369 7420 6672 6571  er explicit freq
+00002120: 7565 6e63 792e 204f 6273 6572 7665 6420  uency. Observed 
+00002130: 6672 6571 7565 6e63 6965 733a 2022 0a20  frequencies: ". 
+00002140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002150: 2020 202b 2028 276e 6f6e 6527 2069 6620     + ('none' if 
+00002160: 6c65 6e28 6f62 7365 7276 6564 5f66 7265  len(observed_fre
+00002170: 7175 656e 6369 6573 2920 3d3d 2030 2065  quencies) == 0 e
+00002180: 6c73 6520 7374 7228 6f62 7365 7276 6564  lse str(observed
+00002190: 5f66 7265 7175 656e 6369 6573 2929 0a20  _frequencies)). 
+000021a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021b0: 2020 202b 2028 222e 2049 7320 5365 7269     + (". Is Seri
+000021c0: 6573 2074 6f6f 2073 686f 7274 2028 6e3d  es too short (n=
+000021d0: 7b7d 293f 222e 666f 726d 6174 2873 616d  {})?".format(sam
+000021e0: 706c 6573 5f73 697a 652d 3129 2069 6620  ples_size-1) if 
+000021f0: 6c65 6e28 6f62 7365 7276 6564 5f66 7265  len(observed_fre
+00002200: 7175 656e 6369 6573 2920 3d3d 2030 0a20  quencies) == 0. 
+00002210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002220: 2020 2020 2020 656c 7365 2027 2e27 292c        else '.'),
+00002230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002240: 2020 2020 206c 6f67 6765 7229 0a0a 2020       logger)..  
+00002250: 2020 2020 2020 2020 2020 2020 2020 6672                fr
+00002260: 6571 203d 206f 6273 6572 7665 645f 6672  eq = observed_fr
+00002270: 6571 7565 6e63 6965 732e 706f 7028 290a  equencies.pop().
+00002280: 0a20 2020 2020 2020 2020 2020 2078 615f  .            xa_
+00002290: 203d 2073 6f72 7465 645f 7861 2e72 6573   = sorted_xa.res
+000022a0: 616d 706c 6528 7b78 612e 6469 6d73 5b30  ample({xa.dims[0
+000022b0: 5d3a 2066 7265 717d 292e 6173 6672 6571  ]: freq}).asfreq
+000022c0: 2829 0a0a 2020 2020 2020 2020 656c 6966  ()..        elif
+000022d0: 2069 7369 6e73 7461 6e63 6528 7861 2e67   isinstance(xa.g
+000022e0: 6574 5f69 6e64 6578 2878 612e 6469 6d73  et_index(xa.dims
+000022f0: 5b30 5d29 2c20 7064 2e44 6174 6574 696d  [0]), pd.Datetim
+00002300: 6549 6e64 6578 2920 616e 6420 5c0a 2020  eIndex) and \.  
+00002310: 2020 2020 2020 2020 2020 2020 2020 6672                fr
+00002320: 6571 2069 7320 6e6f 7420 4e6f 6e65 2061  eq is not None a
+00002330: 6e64 205c 0a20 2020 2020 2020 2020 2020  nd \.           
+00002340: 2020 2020 2078 612e 6765 745f 696e 6465       xa.get_inde
+00002350: 7828 7861 2e64 696d 735b 305d 292e 6672  x(xa.dims[0]).fr
+00002360: 6571 2069 7320 4e6f 6e65 3a0a 2020 2020  eq is None:.    
+00002370: 2020 2020 2020 2020 2320 5468 6520 7072          # The pr
+00002380: 6f76 6964 6564 2069 6e64 6578 2064 6f65  ovided index doe
+00002390: 7320 6e6f 7420 6861 7665 2061 2066 7265  s not have a fre
+000023a0: 713b 2075 7369 6e67 2074 6865 2070 726f  q; using the pro
+000023b0: 7669 6465 6420 6672 6571 0a20 2020 2020  vided freq.     
+000023c0: 2020 2020 2020 2078 615f 203d 2078 612e         xa_ = xa.
+000023d0: 7265 7361 6d70 6c65 287b 7861 2e64 696d  resample({xa.dim
+000023e0: 735b 305d 3a20 6672 6571 7d29 2e61 7366  s[0]: freq}).asf
+000023f0: 7265 7128 290a 2020 2020 2020 2020 656c  req().        el
+00002400: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00002410: 7861 5f20 3d20 7861 0a0a 2020 2020 2020  xa_ = xa..      
+00002420: 2020 2320 636c 6561 6e20 636f 6d70 6f6e    # clean compon
+00002430: 656e 7473 2028 636f 6c75 6d6e 7329 206e  ents (columns) n
+00002440: 616d 6573 2069 6620 6e65 6564 6564 2028  ames if needed (
+00002450: 6966 206e 616d 6573 2061 7265 206e 6f74  if names are not
+00002460: 2075 6e69 7175 652c 206f 7220 6e6f 7420   unique, or not 
+00002470: 7374 7269 6e67 7329 0a20 2020 2020 2020  strings).       
+00002480: 2063 6f6d 706f 6e65 6e74 7320 3d20 7861   components = xa
+00002490: 5f2e 6765 745f 696e 6465 7828 4449 4d53  _.get_index(DIMS
+000024a0: 5b31 5d29 0a20 2020 2020 2020 2069 6620  [1]).        if 
+000024b0: 6c65 6e28 7365 7428 636f 6d70 6f6e 656e  len(set(componen
+000024c0: 7473 2929 2021 3d20 6c65 6e28 636f 6d70  ts)) != len(comp
+000024d0: 6f6e 656e 7473 2920 6f72 2061 6e79 285b  onents) or any([
+000024e0: 6e6f 7420 6973 696e 7374 616e 6365 2873  not isinstance(s
+000024f0: 2c20 7374 7229 2066 6f72 2073 2069 6e20  , str) for s in 
+00002500: 636f 6d70 6f6e 656e 7473 5d29 3a0a 0a20  components]):.. 
+00002510: 2020 2020 2020 2020 2020 2064 6566 205f             def _
+00002520: 636c 6561 6e5f 636f 6d70 6f6e 656e 745f  clean_component_
+00002530: 6c69 7374 2863 6f6c 756d 6e73 2920 2d3e  list(columns) ->
+00002540: 204c 6973 745b 7374 725d 3a0a 2020 2020   List[str]:.    
+00002550: 2020 2020 2020 2020 2020 2020 2320 7265              # re
+00002560: 7475 726e 2061 206c 6973 7420 6f66 2073  turn a list of s
+00002570: 7472 696e 6720 636f 6e74 6169 6e69 6e67  tring containing
+00002580: 2063 6f6c 756d 6e20 6e61 6d65 730a 2020   column names.  
+00002590: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+000025a0: 6d61 6b65 2065 6163 6820 636f 6c75 6d6e  make each column
+000025b0: 206e 616d 6520 756e 6971 7565 2069 6e20   name unique in 
+000025c0: 6361 7365 2073 6f6d 6520 636f 6c75 6d6e  case some column
+000025d0: 7320 6861 7665 2074 6865 2073 616d 6520  s have the same 
+000025e0: 6e61 6d65 730a 2020 2020 2020 2020 2020  names.          
+000025f0: 2020 2020 2020 636c 6973 7420 3d20 636f        clist = co
+00002600: 6c75 6d6e 732e 746f 5f6c 6973 7428 290a  lumns.to_list().
+00002610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002620: 2023 2063 6f6e 7665 7274 2065 7665 7279   # convert every
+00002630: 7468 696e 6720 746f 2073 7472 696e 6720  thing to string 
+00002640: 6966 206e 6565 6465 640a 2020 2020 2020  if needed.      
+00002650: 2020 2020 2020 2020 2020 666f 7220 692c            for i,
+00002660: 2063 6f6c 756d 6e20 696e 2065 6e75 6d65   column in enume
+00002670: 7261 7465 2863 6c69 7374 293a 0a20 2020  rate(clist):.   
+00002680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002690: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
+000026a0: 6365 2863 6f6c 756d 6e2c 2073 7472 293a  ce(column, str):
+000026b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000026c0: 2020 2020 2020 2020 2063 6c69 7374 5b69           clist[i
+000026d0: 5d20 3d20 7374 7228 636f 6c75 6d6e 290a  ] = str(column).
+000026e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000026f0: 2068 6173 5f64 7570 6c69 6361 7465 203d   has_duplicate =
+00002700: 206c 656e 2873 6574 2863 6c69 7374 2929   len(set(clist))
+00002710: 2021 3d20 6c65 6e28 636c 6973 7429 0a20   != len(clist). 
+00002720: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00002730: 6869 6c65 2068 6173 5f64 7570 6c69 6361  hile has_duplica
+00002740: 7465 3a0a 2020 2020 2020 2020 2020 2020  te:.            
+00002750: 2020 2020 2020 2020 2320 7765 206d 6179          # we may
+00002760: 2068 6176 6520 746f 206c 6f6f 7020 7365   have to loop se
+00002770: 7665 7261 6c20 7469 6d65 7320 2865 2e67  veral times (e.g
+00002780: 2e20 7765 2063 6f75 6c64 2068 6176 6520  . we could have 
+00002790: 636f 6c75 6d6e 7320 5b22 3022 2c20 2230  columns ["0", "0
+000027a0: 5f31 222c 2022 3022 5d20 616e 6420 6e6f  _1", "0"] and no
+000027b0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+000027c0: 2020 2020 2020 2320 6e6f 7469 6369 6e67        # noticing
+000027d0: 2077 6865 6e20 7265 6e61 6d69 6e67 2074   when renaming t
+000027e0: 6865 206c 6173 7420 2230 2220 696e 746f  he last "0" into
+000027f0: 2022 305f 3122 2074 6861 7420 2230 5f31   "0_1" that "0_1
+00002800: 2220 616c 7265 6164 7920 6578 6973 7473  " already exists
+00002810: 2e2e 2e29 0a20 2020 2020 2020 2020 2020  ...).           
+00002820: 2020 2020 2020 2020 206e 616d 655f 746f           name_to
+00002830: 5f6f 6363 7572 656e 6365 203d 2064 6566  _occurence = def
+00002840: 6175 6c74 6469 6374 2869 6e74 290a 2020  aultdict(int).  
+00002850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002860: 2020 666f 7220 692c 2063 6f6c 756d 6e20    for i, column 
+00002870: 696e 2065 6e75 6d65 7261 7465 2863 6c69  in enumerate(cli
+00002880: 7374 293a 0a20 2020 2020 2020 2020 2020  st):.           
+00002890: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+000028a0: 655f 746f 5f6f 6363 7572 656e 6365 5b63  e_to_occurence[c
+000028b0: 6c69 7374 5b69 5d5d 202b 3d20 310a 0a20  list[i]] += 1.. 
+000028c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028d0: 2020 2020 2020 2069 6620 6e61 6d65 5f74         if name_t
+000028e0: 6f5f 6f63 6375 7265 6e63 655b 636c 6973  o_occurence[clis
+000028f0: 745b 695d 5d20 3e20 313a 0a20 2020 2020  t[i]] > 1:.     
+00002900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002910: 2020 2020 2020 2063 6c69 7374 5b69 5d20         clist[i] 
+00002920: 3d20 636c 6973 745b 695d 202b 2027 5f7b  = clist[i] + '_{
+00002930: 7d27 2e66 6f72 6d61 7428 6e61 6d65 5f74  }'.format(name_t
+00002940: 6f5f 6f63 6375 7265 6e63 655b 636c 6973  o_occurence[clis
+00002950: 745b 695d 5d2d 3129 0a0a 2020 2020 2020  t[i]]-1)..      
+00002960: 2020 2020 2020 2020 2020 2020 2020 6861                ha
+00002970: 735f 6475 706c 6963 6174 6520 3d20 6c65  s_duplicate = le
+00002980: 6e28 7365 7428 636c 6973 7429 2920 213d  n(set(clist)) !=
+00002990: 206c 656e 2863 6c69 7374 290a 0a20 2020   len(clist)..   
+000029a0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+000029b0: 7572 6e20 636c 6973 740a 0a20 2020 2020  urn clist..     
+000029c0: 2020 2020 2020 2074 696d 655f 696e 6465         time_inde
+000029d0: 785f 6e61 6d65 203d 2078 615f 2e64 696d  x_name = xa_.dim
+000029e0: 735b 305d 0a20 2020 2020 2020 2020 2020  s[0].           
+000029f0: 2063 6f6c 756d 6e73 5f6c 6973 7420 3d20   columns_list = 
+00002a00: 5f63 6c65 616e 5f63 6f6d 706f 6e65 6e74  _clean_component
+00002a10: 5f6c 6973 7428 636f 6d70 6f6e 656e 7473  _list(components
+00002a20: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
+00002a30: 2054 4f44 4f3a 2069 7320 7468 6572 6520   TODO: is there 
+00002a40: 6120 7761 7920 746f 206a 7573 7420 7570  a way to just up
+00002a50: 6461 7465 2074 6865 2063 6f6d 706f 6e65  date the compone
+00002a60: 6e74 2069 6e64 6578 2077 6974 686f 7574  nt index without
+00002a70: 2072 652d 6372 6561 7469 6e67 2061 206e   re-creating a n
+00002a80: 6577 2044 6174 6141 7272 6179 3f0a 2020  ew DataArray?.  
+00002a90: 2020 2020 2020 2020 2020 7861 5f20 3d20            xa_ = 
+00002aa0: 7872 2e44 6174 6141 7272 6179 2878 615f  xr.DataArray(xa_
+00002ab0: 2e76 616c 7565 732c 0a20 2020 2020 2020  .values,.       
+00002ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ad0: 2020 2020 2020 2020 6469 6d73 3d78 615f          dims=xa_
+00002ae0: 2e64 696d 732c 0a20 2020 2020 2020 2020  .dims,.         
+00002af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b00: 2020 2020 2020 636f 6f72 6473 3d7b 7469        coords={ti
+00002b10: 6d65 5f69 6e64 6578 5f6e 616d 653a 2078  me_index_name: x
+00002b20: 615f 2e67 6574 5f69 6e64 6578 2874 696d  a_.get_index(tim
+00002b30: 655f 696e 6465 785f 6e61 6d65 292c 2044  e_index_name), D
+00002b40: 494d 535b 315d 3a20 636f 6c75 6d6e 735f  IMS[1]: columns_
+00002b50: 6c69 7374 7d29 0a0a 2020 2020 2020 2020  list})..        
+00002b60: 2320 5765 2063 6173 7420 7468 6520 6172  # We cast the ar
+00002b70: 7261 7920 746f 2066 6c6f 6174 0a20 2020  ray to float.   
+00002b80: 2020 2020 2023 2054 4f44 4f3a 2069 7320       # TODO: is 
+00002b90: 6173 7479 7065 2829 2061 6c77 6179 7320  astype() always 
+00002ba0: 636f 7079 696e 673f 2028 6d69 6768 7420  copying? (might 
+00002bb0: 6265 2073 6c69 6768 746c 7920 696e 6566  be slightly inef
+00002bc0: 6669 6369 656e 7420 6966 2061 7272 6179  ficient if array
+00002bd0: 2069 7320 616c 7265 6164 7920 666c 6f61   is already floa
+00002be0: 7429 0a20 2020 2020 2020 2072 6574 7572  t).        retur
+00002bf0: 6e20 5469 6d65 5365 7269 6573 2878 615f  n TimeSeries(xa_
+00002c00: 2e61 7374 7970 6528 6e70 2e66 6c6f 6174  .astype(np.float
+00002c10: 2929 0a0a 2020 2020 4073 7461 7469 636d  ))..    @staticm
+00002c20: 6574 686f 640a 2020 2020 6465 6620 6672  ethod.    def fr
+00002c30: 6f6d 5f64 6174 6166 7261 6d65 2864 663a  om_dataframe(df:
+00002c40: 2070 642e 4461 7461 4672 616d 652c 0a20   pd.DataFrame,. 
+00002c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c60: 2020 2020 2020 7469 6d65 5f63 6f6c 3a20        time_col: 
+00002c70: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00002c80: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00002c90: 2020 2020 2020 2020 2020 2020 2076 616c               val
+00002ca0: 7565 5f63 6f6c 733a 204f 7074 696f 6e61  ue_cols: Optiona
+00002cb0: 6c5b 556e 696f 6e5b 4c69 7374 5b73 7472  l[Union[List[str
+00002cc0: 5d2c 2073 7472 5d5d 203d 204e 6f6e 652c  ], str]] = None,
+00002cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002ce0: 2020 2020 2020 2020 6669 6c6c 5f6d 6973          fill_mis
+00002cf0: 7369 6e67 5f64 6174 6573 3a20 4f70 7469  sing_dates: Opti
+00002d00: 6f6e 616c 5b62 6f6f 6c5d 203d 2046 616c  onal[bool] = Fal
+00002d10: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+00002d20: 2020 2020 2020 2020 2020 2066 7265 713a             freq:
+00002d30: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00002d40: 204e 6f6e 652c 2920 2d3e 2027 5469 6d65   None,) -> 'Time
+00002d50: 5365 7269 6573 273a 0a20 2020 2020 2020  Series':.       
+00002d60: 2022 2222 0a20 2020 2020 2020 2052 6574   """.        Ret
+00002d70: 7572 6e73 2061 2064 6574 6572 6d69 6e69  urns a determini
+00002d80: 7374 6963 2054 696d 6553 6572 6965 7320  stic TimeSeries 
+00002d90: 696e 7374 616e 6365 2062 7569 6c74 2066  instance built f
+00002da0: 726f 6d20 6120 7365 6c65 6374 696f 6e20  rom a selection 
+00002db0: 6f66 2063 6f6c 756d 6e73 206f 6620 6120  of columns of a 
+00002dc0: 4461 7461 4672 616d 652e 0a20 2020 2020  DataFrame..     
+00002dd0: 2020 204f 6e65 2063 6f6c 756d 6e20 286f     One column (o
+00002de0: 7220 7468 6520 4461 7461 4672 616d 6520  r the DataFrame 
+00002df0: 696e 6465 7829 2068 6173 2074 6f20 7265  index) has to re
+00002e00: 7072 6573 656e 7420 7468 6520 7469 6d65  present the time
+00002e10: 2c0a 2020 2020 2020 2020 616e 6420 6120  ,.        and a 
+00002e20: 6c69 7374 206f 6620 636f 6c75 6d6e 7320  list of columns 
+00002e30: 6076 616c 7565 5f63 6f6c 7360 2068 6173  `value_cols` has
+00002e40: 2074 6f20 7265 7072 6573 656e 7420 7468   to represent th
+00002e50: 6520 7661 6c75 6573 2066 6f72 2074 6869  e values for thi
+00002e60: 7320 7469 6d65 2073 6572 6965 732e 0a0a  s time series...
+00002e70: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00002e80: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+00002e90: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6466  -----.        df
+00002ea0: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+00002eb0: 2044 6174 6146 7261 6d65 0a20 2020 2020   DataFrame.     
+00002ec0: 2020 2074 696d 655f 636f 6c0a 2020 2020     time_col.    
+00002ed0: 2020 2020 2020 2020 5468 6520 7469 6d65          The time
+00002ee0: 2063 6f6c 756d 6e20 6e61 6d65 2e20 4966   column name. If
+00002ef0: 2073 6574 2c20 7468 6520 636f 6c75 6d6e   set, the column
+00002f00: 2077 696c 6c20 6265 2063 6173 7420 746f   will be cast to
+00002f10: 2061 2070 616e 6461 7320 4461 7465 7469   a pandas Dateti
+00002f20: 6d65 496e 6465 782e 0a20 2020 2020 2020  meIndex..       
+00002f30: 2020 2020 2049 6620 6e6f 7420 7365 742c       If not set,
+00002f40: 2074 6865 2044 6174 6146 7261 6d65 2069   the DataFrame i
+00002f50: 6e64 6578 2077 696c 6c20 6265 2075 7365  ndex will be use
+00002f60: 642e 2049 6e20 7468 6973 2063 6173 6520  d. In this case 
+00002f70: 7468 6520 4461 7461 4672 616d 6520 6d75  the DataFrame mu
+00002f80: 7374 2063 6f6e 7461 696e 2061 6e20 696e  st contain an in
+00002f90: 6465 7820 7468 6174 2069 730a 2020 2020  dex that is.    
+00002fa0: 2020 2020 2020 2020 6569 7468 6572 2061          either a
+00002fb0: 2070 616e 6461 7320 4461 7465 7469 6d65   pandas Datetime
+00002fc0: 496e 6465 7820 6f72 2061 2070 616e 6461  Index or a panda
+00002fd0: 7320 496e 7436 3449 6e64 6578 2028 696e  s Int64Index (in
+00002fe0: 636c 2e20 5261 6e67 6549 6e64 6578 292e  cl. RangeIndex).
+00002ff0: 2049 6620 6120 4461 7465 7469 6d65 496e   If a DatetimeIn
+00003000: 6465 7820 6973 0a20 2020 2020 2020 2020  dex is.         
+00003010: 2020 2075 7365 642c 2069 7420 6973 2062     used, it is b
+00003020: 6574 7465 7220 6966 2069 7420 6861 7320  etter if it has 
+00003030: 6e6f 2068 6f6c 6573 3b20 616c 7468 6f75  no holes; althou
+00003040: 6768 2073 6574 7469 6e67 2060 6669 6c6c  gh setting `fill
+00003050: 5f6d 6973 7369 6e67 5f64 6174 6573 6020  _missing_dates` 
+00003060: 6361 6e20 696e 2073 6f6d 6520 6361 7365  can in some case
+00003070: 7320 736f 6c76 6520 7468 6573 650a 2020  s solve these.  
+00003080: 2020 2020 2020 2020 2020 6973 7375 6573            issues
+00003090: 2028 6669 6c6c 696e 6720 686f 6c65 7320   (filling holes 
+000030a0: 7769 7468 204e 614e 2920 6174 2061 2070  with NaN) at a p
+000030b0: 6572 666f 726d 616e 6365 2063 6f73 742e  erformance cost.
+000030c0: 0a20 2020 2020 2020 2076 616c 7565 5f63  .        value_c
+000030d0: 6f6c 730a 2020 2020 2020 2020 2020 2020  ols.            
+000030e0: 4120 7374 7269 6e67 206f 7220 6c69 7374  A string or list
+000030f0: 206f 6620 7374 7269 6e67 7320 7265 7072   of strings repr
+00003100: 6573 656e 7469 6e67 2074 6865 2076 616c  esenting the val
+00003110: 7565 2063 6f6c 756d 6e28 7329 2074 6f20  ue column(s) to 
+00003120: 6265 2065 7874 7261 6374 6564 2066 726f  be extracted fro
+00003130: 6d20 7468 6520 4461 7461 4672 616d 652e  m the DataFrame.
+00003140: 2049 6620 7365 7420 746f 0a20 2020 2020   If set to.     
+00003150: 2020 2020 2020 2060 4e6f 6e65 602c 2074         `None`, t
+00003160: 6865 2077 686f 6c65 2044 6174 6146 7261  he whole DataFra
+00003170: 6d65 2077 696c 6c20 6265 2075 7365 642e  me will be used.
+00003180: 0a20 2020 2020 2020 2066 696c 6c5f 6d69  .        fill_mi
+00003190: 7373 696e 675f 6461 7465 730a 2020 2020  ssing_dates.    
+000031a0: 2020 2020 2020 2020 4f70 7469 6f6e 616c          Optional
+000031b0: 6c79 2c20 6120 626f 6f6c 6561 6e20 7661  ly, a boolean va
+000031c0: 6c75 6520 696e 6469 6361 7469 6e67 2077  lue indicating w
+000031d0: 6865 7468 6572 2074 6f20 6669 6c6c 206d  hether to fill m
+000031e0: 6973 7369 6e67 2064 6174 6573 2077 6974  issing dates wit
+000031f0: 6820 4e61 4e20 7661 6c75 6573 2e20 5468  h NaN values. Th
+00003200: 6973 2072 6571 7569 7265 730a 2020 2020  is requires.    
+00003210: 2020 2020 2020 2020 6569 7468 6572 2061          either a
+00003220: 2070 726f 7669 6465 6420 6066 7265 7160   provided `freq`
+00003230: 206f 7220 7468 6520 706f 7373 6962 696c   or the possibil
+00003240: 6974 7920 746f 2069 6e66 6572 2074 6865  ity to infer the
+00003250: 2066 7265 7175 656e 6379 2066 726f 6d20   frequency from 
+00003260: 7468 6520 7072 6f76 6964 6564 2074 696d  the provided tim
+00003270: 6573 7461 6d70 732e 0a20 2020 2020 2020  estamps..       
+00003280: 2020 2020 2049 6e66 6572 7269 6e67 2074       Inferring t
+00003290: 6865 2066 7265 7175 656e 6379 2061 6e64  he frequency and
+000032a0: 2072 6573 616d 706c 696e 6720 7468 6520   resampling the 
+000032b0: 6461 7461 2063 616e 2069 6e64 7563 6520  data can induce 
+000032c0: 6120 7369 676e 6966 6963 616e 7420 7065  a significant pe
+000032d0: 7266 6f72 6d61 6e63 6520 6f76 6572 6865  rformance overhe
+000032e0: 6164 2e0a 2020 2020 2020 2020 6672 6571  ad..        freq
+000032f0: 0a20 2020 2020 2020 2020 2020 204f 7074  .            Opt
+00003300: 696f 6e61 6c6c 792c 2061 2073 7472 696e  ionally, a strin
+00003310: 6720 7265 7072 6573 656e 7469 6e67 2074  g representing t
+00003320: 6865 2066 7265 7175 656e 6379 206f 6620  he frequency of 
+00003330: 7468 6520 5061 6e64 6173 2044 6174 6146  the Pandas DataF
+00003340: 7261 6d65 2e20 5468 6973 2069 7320 7573  rame. This is us
+00003350: 6566 756c 2069 6e20 6f72 6465 7220 746f  eful in order to
+00003360: 2066 696c 6c0a 2020 2020 2020 2020 2020   fill.          
+00003370: 2020 696e 206d 6973 7369 6e67 2076 616c    in missing val
+00003380: 7565 7320 6966 2073 6f6d 6520 6461 7465  ues if some date
+00003390: 7320 6172 6520 6d69 7373 696e 6720 616e  s are missing an
+000033a0: 6420 6066 696c 6c5f 6d69 7373 696e 675f  d `fill_missing_
+000033b0: 6461 7465 7360 2069 7320 7365 7420 746f  dates` is set to
+000033c0: 2060 5472 7565 602e 0a0a 2020 2020 2020   `True`...      
+000033d0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+000033e0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+000033f0: 2020 5469 6d65 5365 7269 6573 0a20 2020    TimeSeries.   
+00003400: 2020 2020 2020 2020 2041 2075 6e69 7661           A univa
+00003410: 7269 6174 6520 6f72 206d 756c 7469 7661  riate or multiva
+00003420: 7269 6174 6520 6465 7465 726d 696e 6973  riate determinis
+00003430: 7469 6320 5469 6d65 5365 7269 6573 2063  tic TimeSeries c
+00003440: 6f6e 7374 7275 6374 6564 2066 726f 6d20  onstructed from 
+00003450: 7468 6520 696e 7075 7473 2e0a 2020 2020  the inputs..    
+00003460: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+00003470: 2023 2067 6574 2076 616c 7565 730a 2020   # get values.  
+00003480: 2020 2020 2020 6966 2076 616c 7565 5f63        if value_c
+00003490: 6f6c 7320 6973 204e 6f6e 653a 0a20 2020  ols is None:.   
+000034a0: 2020 2020 2020 2020 2073 6572 6965 735f           series_
+000034b0: 6466 203d 2064 662e 6c6f 635b 3a2c 2064  df = df.loc[:, d
+000034c0: 662e 636f 6c75 6d6e 7320 213d 2074 696d  f.columns != tim
+000034d0: 655f 636f 6c5d 0a20 2020 2020 2020 2065  e_col].        e
+000034e0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000034f0: 2069 6620 6973 696e 7374 616e 6365 2876   if isinstance(v
+00003500: 616c 7565 5f63 6f6c 732c 2073 7472 293a  alue_cols, str):
+00003510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003520: 2076 616c 7565 5f63 6f6c 7320 3d20 5b76   value_cols = [v
+00003530: 616c 7565 5f63 6f6c 735d 0a20 2020 2020  alue_cols].     
+00003540: 2020 2020 2020 2073 6572 6965 735f 6466         series_df
+00003550: 203d 2064 665b 7661 6c75 655f 636f 6c73   = df[value_cols
+00003560: 5d0a 0a20 2020 2020 2020 2023 2067 6574  ]..        # get
+00003570: 2074 696d 6520 696e 6465 780a 2020 2020   time index.    
+00003580: 2020 2020 6966 2074 696d 655f 636f 6c3a      if time_col:
+00003590: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
+000035a0: 655f 696e 6465 7820 3d20 7064 2e44 6174  e_index = pd.Dat
+000035b0: 6574 696d 6549 6e64 6578 2864 665b 7469  etimeIndex(df[ti
+000035c0: 6d65 5f63 6f6c 5d29 0a20 2020 2020 2020  me_col]).       
+000035d0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000035e0: 2020 2072 6169 7365 5f69 665f 6e6f 7428     raise_if_not(
+000035f0: 6973 696e 7374 616e 6365 2864 662e 696e  isinstance(df.in
+00003600: 6465 782c 2070 642e 496e 7436 3449 6e64  dex, pd.Int64Ind
+00003610: 6578 2920 6f72 2069 7369 6e73 7461 6e63  ex) or isinstanc
+00003620: 6528 6466 2e69 6e64 6578 2c20 7064 2e44  e(df.index, pd.D
+00003630: 6174 6574 696d 6549 6e64 6578 292c 0a20  atetimeIndex),. 
+00003640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003650: 2020 2020 2020 2020 2749 6620 7469 6d65          'If time
+00003660: 5f63 6f6c 2069 7320 6e6f 7420 7370 6563  _col is not spec
+00003670: 6966 6965 642c 2074 6865 2044 6174 6146  ified, the DataF
+00003680: 7261 6d65 206d 7573 7420 6265 2069 6e64  rame must be ind
+00003690: 6578 6564 2065 6974 6865 7220 7769 7468  exed either with
+000036a0: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+000036b0: 2020 2020 2020 2020 2020 2027 6120 4461             'a Da
+000036c0: 7465 7469 6d65 496e 6465 782c 206f 7220  tetimeIndex, or 
+000036d0: 7769 7468 2061 2049 6e74 3634 496e 6465  with a Int64Inde
+000036e0: 7820 2869 6e63 6c2e 2052 616e 6765 496e  x (incl. RangeIn
+000036f0: 6465 7829 2e27 2c20 6c6f 6767 6572 290a  dex).', logger).
+00003700: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+00003710: 5f69 6e64 6578 203d 2064 662e 696e 6465  _index = df.inde
+00003720: 780a 0a20 2020 2020 2020 2069 6620 6e6f  x..        if no
+00003730: 7420 7469 6d65 5f69 6e64 6578 2e6e 616d  t time_index.nam
+00003740: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
+00003750: 696d 655f 696e 6465 782e 6e61 6d65 203d  ime_index.name =
+00003760: 2044 494d 535b 305d 0a0a 2020 2020 2020   DIMS[0]..      
+00003770: 2020 7861 203d 2078 722e 4461 7461 4172    xa = xr.DataAr
+00003780: 7261 7928 7365 7269 6573 5f64 662e 7661  ray(series_df.va
+00003790: 6c75 6573 5b3a 2c20 3a2c 206e 702e 6e65  lues[:, :, np.ne
+000037a0: 7761 7869 735d 2c0a 2020 2020 2020 2020  waxis],.        
+000037b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000037c0: 2020 6469 6d73 3d28 7469 6d65 5f69 6e64    dims=(time_ind
+000037d0: 6578 2e6e 616d 652c 2920 2b20 4449 4d53  ex.name,) + DIMS
+000037e0: 5b2d 323a 5d2c 0a20 2020 2020 2020 2020  [-2:],.         
+000037f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003800: 2063 6f6f 7264 733d 7b74 696d 655f 696e   coords={time_in
+00003810: 6465 782e 6e61 6d65 3a20 7469 6d65 5f69  dex.name: time_i
+00003820: 6e64 6578 2c20 4449 4d53 5b31 5d3a 2073  ndex, DIMS[1]: s
+00003830: 6572 6965 735f 6466 2e63 6f6c 756d 6e73  eries_df.columns
+00003840: 7d29 0a0a 2020 2020 2020 2020 7265 7475  })..        retu
+00003850: 726e 2054 696d 6553 6572 6965 732e 6672  rn TimeSeries.fr
+00003860: 6f6d 5f78 6172 7261 7928 7861 3d78 612c  om_xarray(xa=xa,
+00003870: 2066 696c 6c5f 6d69 7373 696e 675f 6461   fill_missing_da
+00003880: 7465 733d 6669 6c6c 5f6d 6973 7369 6e67  tes=fill_missing
+00003890: 5f64 6174 6573 2c20 6672 6571 3d66 7265  _dates, freq=fre
+000038a0: 7129 0a0a 2020 2020 4073 7461 7469 636d  q)..    @staticm
+000038b0: 6574 686f 640a 2020 2020 6465 6620 6672  ethod.    def fr
+000038c0: 6f6d 5f73 6572 6965 7328 7064 5f73 6572  om_series(pd_ser
+000038d0: 6965 733a 2070 642e 5365 7269 6573 2c0a  ies: pd.Series,.
+000038e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038f0: 2020 2020 6669 6c6c 5f6d 6973 7369 6e67      fill_missing
+00003900: 5f64 6174 6573 3a20 4f70 7469 6f6e 616c  _dates: Optional
+00003910: 5b62 6f6f 6c5d 203d 2046 616c 7365 2c0a  [bool] = False,.
+00003920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003930: 2020 2020 6672 6571 3a20 4f70 7469 6f6e      freq: Option
+00003940: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c29  al[str] = None,)
+00003950: 202d 3e20 2754 696d 6553 6572 6965 7327   -> 'TimeSeries'
+00003960: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00003970: 2020 2020 2020 5265 7475 726e 7320 6120        Returns a 
+00003980: 756e 6976 6172 6961 7465 2061 6e64 2064  univariate and d
+00003990: 6574 6572 6d69 6e69 7374 6963 2054 696d  eterministic Tim
+000039a0: 6553 6572 6965 7320 6275 696c 7420 6672  eSeries built fr
+000039b0: 6f6d 2061 2070 616e 6461 7320 5365 7269  om a pandas Seri
+000039c0: 6573 2e0a 0a20 2020 2020 2020 2054 6865  es...        The
+000039d0: 2073 6572 6965 7320 6d75 7374 2063 6f6e   series must con
+000039e0: 7461 696e 2061 6e20 696e 6465 7820 7468  tain an index th
+000039f0: 6174 2069 730a 2020 2020 2020 2020 6569  at is.        ei
+00003a00: 7468 6572 2061 2070 616e 6461 7320 4461  ther a pandas Da
+00003a10: 7465 7469 6d65 496e 6465 7820 6f72 2061  tetimeIndex or a
+00003a20: 2070 616e 6461 7320 496e 7436 3449 6e64   pandas Int64Ind
+00003a30: 6578 2028 696e 636c 2e20 5261 6e67 6549  ex (incl. RangeI
+00003a40: 6e64 6578 292e 2049 6620 6120 4461 7465  ndex). If a Date
+00003a50: 7469 6d65 496e 6465 7820 6973 0a20 2020  timeIndex is.   
+00003a60: 2020 2020 2075 7365 642c 2069 7420 6973       used, it is
+00003a70: 2062 6574 7465 7220 6966 2069 7420 6861   better if it ha
+00003a80: 7320 6e6f 2068 6f6c 6573 3b20 616c 7468  s no holes; alth
+00003a90: 6f75 6768 2073 6574 7469 6e67 2060 6669  ough setting `fi
+00003aa0: 6c6c 5f6d 6973 7369 6e67 5f64 6174 6573  ll_missing_dates
+00003ab0: 6020 6361 6e20 696e 2073 6f6d 6520 6361  ` can in some ca
+00003ac0: 7365 7320 736f 6c76 6520 7468 6573 650a  ses solve these.
+00003ad0: 2020 2020 2020 2020 6973 7375 6573 2028          issues (
+00003ae0: 6669 6c6c 696e 6720 686f 6c65 7320 7769  filling holes wi
+00003af0: 7468 204e 614e 2920 6174 2061 2070 6572  th NaN) at a per
+00003b00: 666f 726d 616e 6365 2063 6f73 742e 0a0a  formance cost...
+00003b10: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00003b20: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+00003b30: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7064  -----.        pd
+00003b40: 5f73 6572 6965 730a 2020 2020 2020 2020  _series.        
+00003b50: 2020 2020 5468 6520 7061 6e64 6173 2053      The pandas S
+00003b60: 6572 6965 7320 696e 7374 616e 6365 2e0a  eries instance..
+00003b70: 2020 2020 2020 2020 6669 6c6c 5f6d 6973          fill_mis
+00003b80: 7369 6e67 5f64 6174 6573 0a20 2020 2020  sing_dates.     
+00003b90: 2020 2020 2020 204f 7074 696f 6e61 6c6c         Optionall
+00003ba0: 792c 2061 2062 6f6f 6c65 616e 2076 616c  y, a boolean val
+00003bb0: 7565 2069 6e64 6963 6174 696e 6720 7768  ue indicating wh
+00003bc0: 6574 6865 7220 746f 2066 696c 6c20 6d69  ether to fill mi
+00003bd0: 7373 696e 6720 6461 7465 7320 7769 7468  ssing dates with
+00003be0: 204e 614e 2076 616c 7565 732e 2054 6869   NaN values. Thi
+00003bf0: 7320 7265 7175 6972 6573 0a20 2020 2020  s requires.     
+00003c00: 2020 2020 2020 2065 6974 6865 7220 6120         either a 
+00003c10: 7072 6f76 6964 6564 2060 6672 6571 6020  provided `freq` 
+00003c20: 6f72 2074 6865 2070 6f73 7369 6269 6c69  or the possibili
+00003c30: 7479 2074 6f20 696e 6665 7220 7468 6520  ty to infer the 
+00003c40: 6672 6571 7565 6e63 7920 6672 6f6d 2074  frequency from t
+00003c50: 6865 2070 726f 7669 6465 6420 7469 6d65  he provided time
+00003c60: 7374 616d 7073 2e0a 2020 2020 2020 2020  stamps..        
+00003c70: 2020 2020 496e 6665 7272 696e 6720 7468      Inferring th
+00003c80: 6520 6672 6571 7565 6e63 7920 616e 6420  e frequency and 
+00003c90: 7265 7361 6d70 6c69 6e67 2074 6865 2064  resampling the d
+00003ca0: 6174 6120 6361 6e20 696e 6475 6365 2061  ata can induce a
+00003cb0: 2073 6967 6e69 6669 6361 6e74 2070 6572   significant per
+00003cc0: 666f 726d 616e 6365 206f 7665 7268 6561  formance overhea
+00003cd0: 642e 0a20 2020 2020 2020 2066 7265 710a  d..        freq.
+00003ce0: 2020 2020 2020 2020 2020 2020 4f70 7469              Opti
+00003cf0: 6f6e 616c 6c79 2c20 6120 7374 7269 6e67  onally, a string
+00003d00: 2072 6570 7265 7365 6e74 696e 6720 7468   representing th
+00003d10: 6520 6672 6571 7565 6e63 7920 6f66 2074  e frequency of t
+00003d20: 6865 2050 616e 6461 7320 4461 7461 4672  he Pandas DataFr
+00003d30: 616d 652e 2054 6869 7320 6973 2075 7365  ame. This is use
+00003d40: 6675 6c20 696e 206f 7264 6572 2074 6f20  ful in order to 
+00003d50: 6669 6c6c 0a20 2020 2020 2020 2020 2020  fill.           
+00003d60: 2069 6e20 6d69 7373 696e 6720 7661 6c75   in missing valu
+00003d70: 6573 2069 6620 736f 6d65 2064 6174 6573  es if some dates
+00003d80: 2061 7265 206d 6973 7369 6e67 2061 6e64   are missing and
+00003d90: 2060 6669 6c6c 5f6d 6973 7369 6e67 5f64   `fill_missing_d
+00003da0: 6174 6573 6020 6973 2073 6574 2074 6f20  ates` is set to 
+00003db0: 6054 7275 6560 2e0a 0a20 2020 2020 2020  `True`...       
+00003dc0: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+00003dd0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+00003de0: 2054 696d 6553 6572 6965 730a 2020 2020   TimeSeries.    
+00003df0: 2020 2020 2020 2020 4120 756e 6976 6172          A univar
+00003e00: 6961 7465 2061 6e64 2064 6574 6572 6d69  iate and determi
+00003e10: 6e69 7374 6963 2054 696d 6553 6572 6965  nistic TimeSerie
+00003e20: 7320 636f 6e73 7472 7563 7465 6420 6672  s constructed fr
+00003e30: 6f6d 2074 6865 2069 6e70 7574 732e 0a20  om the inputs.. 
+00003e40: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+00003e50: 2020 2020 6466 203d 2070 642e 4461 7461      df = pd.Data
+00003e60: 4672 616d 6528 7064 5f73 6572 6965 7329  Frame(pd_series)
+00003e70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00003e80: 5469 6d65 5365 7269 6573 2e66 726f 6d5f  TimeSeries.from_
+00003e90: 6461 7461 6672 616d 6528 6466 2c0a 2020  dataframe(df,.  
+00003ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ec0: 2020 2020 2020 2074 696d 655f 636f 6c3d         time_col=
+00003ed0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00003ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ef0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00003f00: 616c 7565 5f63 6f6c 733d 4e6f 6e65 2c0a  alue_cols=None,.
+00003f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f30: 2020 2020 2020 2020 2066 696c 6c5f 6d69           fill_mi
+00003f40: 7373 696e 675f 6461 7465 733d 6669 6c6c  ssing_dates=fill
+00003f50: 5f6d 6973 7369 6e67 5f64 6174 6573 2c0a  _missing_dates,.
+00003f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f80: 2020 2020 2020 2020 2066 7265 713d 6672           freq=fr
+00003f90: 6571 290a 0a20 2020 2040 7374 6174 6963  eq)..    @static
+00003fa0: 6d65 7468 6f64 0a20 2020 2064 6566 2066  method.    def f
+00003fb0: 726f 6d5f 7469 6d65 735f 616e 645f 7661  rom_times_and_va
+00003fc0: 6c75 6573 2874 696d 6573 3a20 556e 696f  lues(times: Unio
+00003fd0: 6e5b 7064 2e44 6174 6574 696d 6549 6e64  n[pd.DatetimeInd
+00003fe0: 6578 2c20 7064 2e49 6e74 3634 496e 6465  ex, pd.Int64Inde
+00003ff0: 785d 2c0a 2020 2020 2020 2020 2020 2020  x],.            
+00004000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004010: 2020 7661 6c75 6573 3a20 6e70 2e6e 6461    values: np.nda
+00004020: 7272 6179 2c0a 2020 2020 2020 2020 2020  rray,.          
+00004030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004040: 2020 2020 6669 6c6c 5f6d 6973 7369 6e67      fill_missing
+00004050: 5f64 6174 6573 3a20 4f70 7469 6f6e 616c  _dates: Optional
+00004060: 5b62 6f6f 6c5d 203d 2046 616c 7365 2c0a  [bool] = False,.
+00004070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004080: 2020 2020 2020 2020 2020 2020 2020 6672                fr
+00004090: 6571 3a20 4f70 7469 6f6e 616c 5b73 7472  eq: Optional[str
+000040a0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+000040b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040c0: 2020 2020 2020 2020 636f 6c75 6d6e 733a          columns:
+000040d0: 204f 7074 696f 6e61 6c5b 7064 2e5f 7479   Optional[pd._ty
+000040e0: 7069 6e67 2e41 7865 735d 203d 204e 6f6e  ping.Axes] = Non
+000040f0: 6529 202d 3e20 2754 696d 6553 6572 6965  e) -> 'TimeSerie
+00004100: 7327 3a0a 2020 2020 2020 2020 2222 220a  s':.        """.
+00004110: 2020 2020 2020 2020 5265 7475 726e 7320          Returns 
+00004120: 6120 5469 6d65 5365 7269 6573 2062 7569  a TimeSeries bui
+00004130: 6c74 2066 726f 6d20 616e 2069 6e64 6578  lt from an index
+00004140: 2061 6e64 2076 616c 7565 2061 7272 6179   and value array
+00004150: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00004160: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+00004170: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00004180: 2074 696d 6573 0a20 2020 2020 2020 2020   times.         
+00004190: 2020 2041 2060 7061 6e64 6173 2e44 6174     A `pandas.Dat
+000041a0: 6554 696d 6549 6e64 6578 6020 6f72 2060  eTimeIndex` or `
+000041b0: 7061 6e64 6173 2e49 6e74 3634 496e 6465  pandas.Int64Inde
+000041c0: 7860 2028 6f72 2060 7061 6e64 6173 2e52  x` (or `pandas.R
+000041d0: 616e 6765 496e 6465 7860 2920 7265 7072  angeIndex`) repr
+000041e0: 6573 656e 7469 6e67 2074 6865 2074 696d  esenting the tim
+000041f0: 6520 6178 6973 0a20 2020 2020 2020 2020  e axis.         
+00004200: 2020 2066 6f72 2074 6865 2074 696d 6520     for the time 
+00004210: 7365 7269 6573 2e20 4966 2061 2044 6174  series. If a Dat
+00004220: 6574 696d 6549 6e64 6578 2069 730a 2020  etimeIndex is.  
+00004230: 2020 2020 2020 2020 2020 7573 6564 2c20            used, 
+00004240: 6974 2069 7320 6265 7474 6572 2069 6620  it is better if 
+00004250: 6974 2068 6173 206e 6f20 686f 6c65 733b  it has no holes;
+00004260: 2061 6c74 686f 7567 6820 7365 7474 696e   although settin
+00004270: 6720 6066 696c 6c5f 6d69 7373 696e 675f  g `fill_missing_
+00004280: 6461 7465 7360 2063 616e 2069 6e20 736f  dates` can in so
+00004290: 6d65 2063 6173 6573 2073 6f6c 7665 2074  me cases solve t
+000042a0: 6865 7365 0a20 2020 2020 2020 2020 2020  hese.           
+000042b0: 2069 7373 7565 7320 2866 696c 6c69 6e67   issues (filling
+000042c0: 2068 6f6c 6573 2077 6974 6820 4e61 4e29   holes with NaN)
+000042d0: 2061 7420 6120 7065 7266 6f72 6d61 6e63   at a performanc
+000042e0: 6520 636f 7374 2e0a 2020 2020 2020 2020  e cost..        
+000042f0: 7661 6c75 6573 0a20 2020 2020 2020 2020  values.         
+00004300: 2020 2041 204e 756d 7079 2061 7272 6179     A Numpy array
+00004310: 206f 6620 7661 6c75 6573 2066 6f72 2074   of values for t
+00004320: 6865 2054 696d 6553 6572 6965 732e 2042  he TimeSeries. B
+00004330: 6f74 6820 322d 6469 6d65 6e73 696f 6e61  oth 2-dimensiona
+00004340: 6c20 6172 7261 7973 2c20 666f 7220 6465  l arrays, for de
+00004350: 7465 726d 696e 6973 7469 6320 7365 7269  terministic seri
+00004360: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+00004370: 616e 6420 332d 6469 6d65 6e73 696f 6e61  and 3-dimensiona
+00004380: 6c20 6172 7261 7973 2c20 666f 7220 7072  l arrays, for pr
+00004390: 6f62 6162 696c 6973 7469 6320 7365 7269  obabilistic seri
+000043a0: 6573 2c20 6172 6520 6163 6365 7074 6564  es, are accepted
+000043b0: 2e20 496e 2074 6865 2066 6f72 6d65 7220  . In the former 
+000043c0: 6361 7365 2074 6865 2064 696d 656e 7369  case the dimensi
+000043d0: 6f6e 730a 2020 2020 2020 2020 2020 2020  ons.            
+000043e0: 7368 6f75 6c64 2062 6520 2874 696d 652c  should be (time,
+000043f0: 2063 6f6d 706f 6e65 6e74 292c 2061 6e64   component), and
+00004400: 2069 6e20 7468 6520 6c61 7474 6572 2063   in the latter c
+00004410: 6173 6520 2874 696d 652c 2063 6f6d 706f  ase (time, compo
+00004420: 6e65 6e74 2c20 7361 6d70 6c65 292e 0a20  nent, sample).. 
+00004430: 2020 2020 2020 2066 696c 6c5f 6d69 7373         fill_miss
+00004440: 696e 675f 6461 7465 730a 2020 2020 2020  ing_dates.      
+00004450: 2020 2020 2020 4f70 7469 6f6e 616c 6c79        Optionally
+00004460: 2c20 6120 626f 6f6c 6561 6e20 7661 6c75  , a boolean valu
+00004470: 6520 696e 6469 6361 7469 6e67 2077 6865  e indicating whe
+00004480: 7468 6572 2074 6f20 6669 6c6c 206d 6973  ther to fill mis
+00004490: 7369 6e67 2064 6174 6573 2077 6974 6820  sing dates with 
+000044a0: 4e61 4e20 7661 6c75 6573 2e20 5468 6973  NaN values. This
+000044b0: 2072 6571 7569 7265 730a 2020 2020 2020   requires.      
+000044c0: 2020 2020 2020 6569 7468 6572 2061 2070        either a p
+000044d0: 726f 7669 6465 6420 6066 7265 7160 206f  rovided `freq` o
+000044e0: 7220 7468 6520 706f 7373 6962 696c 6974  r the possibilit
+000044f0: 7920 746f 2069 6e66 6572 2074 6865 2066  y to infer the f
+00004500: 7265 7175 656e 6379 2066 726f 6d20 7468  requency from th
+00004510: 6520 7072 6f76 6964 6564 2074 696d 6573  e provided times
+00004520: 7461 6d70 732e 0a20 2020 2020 2020 2020  tamps..         
+00004530: 2020 2049 6e66 6572 7269 6e67 2074 6865     Inferring the
+00004540: 2066 7265 7175 656e 6379 2061 6e64 2072   frequency and r
+00004550: 6573 616d 706c 696e 6720 7468 6520 6461  esampling the da
+00004560: 7461 2063 616e 2069 6e64 7563 6520 6120  ta can induce a 
+00004570: 7369 676e 6966 6963 616e 7420 7065 7266  significant perf
+00004580: 6f72 6d61 6e63 6520 6f76 6572 6865 6164  ormance overhead
+00004590: 2e0a 2020 2020 2020 2020 6672 6571 0a20  ..        freq. 
+000045a0: 2020 2020 2020 2020 2020 204f 7074 696f             Optio
+000045b0: 6e61 6c6c 792c 2061 2073 7472 696e 6720  nally, a string 
+000045c0: 7265 7072 6573 656e 7469 6e67 2074 6865  representing the
+000045d0: 2066 7265 7175 656e 6379 206f 6620 7468   frequency of th
+000045e0: 6520 5061 6e64 6173 2044 6174 6146 7261  e Pandas DataFra
+000045f0: 6d65 2e20 5468 6973 2069 7320 7573 6566  me. This is usef
+00004600: 756c 2069 6e20 6f72 6465 7220 746f 2066  ul in order to f
+00004610: 696c 6c0a 2020 2020 2020 2020 2020 2020  ill.            
+00004620: 696e 206d 6973 7369 6e67 2076 616c 7565  in missing value
+00004630: 7320 6966 2073 6f6d 6520 6461 7465 7320  s if some dates 
+00004640: 6172 6520 6d69 7373 696e 6720 616e 6420  are missing and 
+00004650: 6066 696c 6c5f 6d69 7373 696e 675f 6461  `fill_missing_da
+00004660: 7465 7360 2069 7320 7365 7420 746f 2060  tes` is set to `
+00004670: 5472 7565 602e 0a20 2020 2020 2020 2063  True`..        c
+00004680: 6f6c 756d 6e73 0a20 2020 2020 2020 2020  olumns.         
+00004690: 2020 2043 6f6c 756d 6e73 2074 6f20 6265     Columns to be
+000046a0: 2075 7365 6420 6279 2074 6865 2075 6e64   used by the und
+000046b0: 6572 6c79 696e 6720 7061 6e64 6173 2044  erlying pandas D
+000046c0: 6174 6146 7261 6d65 2e0a 0a20 2020 2020  ataFrame...     
+000046d0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+000046e0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+000046f0: 2020 2054 696d 6553 6572 6965 730a 2020     TimeSeries.  
+00004700: 2020 2020 2020 2020 2020 4120 5469 6d65            A Time
+00004710: 5365 7269 6573 2063 6f6e 7374 7275 6374  Series construct
+00004720: 6564 2066 726f 6d20 7468 6520 696e 7075  ed from the inpu
+00004730: 7473 2e0a 2020 2020 2020 2020 2222 220a  ts..        """.
+00004740: 0a20 2020 2020 2020 2072 6169 7365 5f69  .        raise_i
+00004750: 665f 6e6f 7428 6973 696e 7374 616e 6365  f_not(isinstance
+00004760: 2874 696d 6573 2c20 7064 2e49 6e74 3634  (times, pd.Int64
+00004770: 496e 6465 7829 206f 7220 6973 696e 7374  Index) or isinst
+00004780: 616e 6365 2874 696d 6573 2c20 7064 2e44  ance(times, pd.D
+00004790: 6174 6574 696d 6549 6e64 6578 292c 0a20  atetimeIndex),. 
+000047a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047b0: 2020 2020 2774 6865 2060 7469 6d65 7360      'the `times`
+000047c0: 2061 7267 756d 656e 7420 6d75 7374 2062   argument must b
+000047d0: 6520 6120 496e 7436 3449 6e64 6578 2028  e a Int64Index (
+000047e0: 6f72 2052 616e 6765 496e 6465 7829 2c20  or RangeIndex), 
+000047f0: 6f72 2061 2044 6174 6554 696d 6549 6e64  or a DateTimeInd
+00004800: 6578 2e20 5573 6520 270a 2020 2020 2020  ex. Use '.      
+00004810: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00004820: 5469 6d65 5365 7269 6573 2e66 726f 6d5f  TimeSeries.from_
+00004830: 7661 6c75 6573 2829 2069 6620 796f 7520  values() if you 
+00004840: 7761 6e74 2074 6f20 7573 6520 616e 2061  want to use an a
+00004850: 7574 6f6d 6174 6963 2052 616e 6765 496e  utomatic RangeIn
+00004860: 6465 782e 2729 0a0a 2020 2020 2020 2020  dex.')..        
+00004870: 7469 6d65 735f 6e61 6d65 203d 2044 494d  times_name = DIM
+00004880: 535b 305d 2069 6620 6e6f 7420 7469 6d65  S[0] if not time
+00004890: 732e 6e61 6d65 2065 6c73 6520 7469 6d65  s.name else time
+000048a0: 732e 6e61 6d65 0a0a 2020 2020 2020 2020  s.name..        
+000048b0: 7661 6c75 6573 203d 206e 702e 6172 7261  values = np.arra
+000048c0: 7928 7661 6c75 6573 290a 2020 2020 2020  y(values).      
+000048d0: 2020 6966 206c 656e 2876 616c 7565 732e    if len(values.
+000048e0: 7368 6170 6529 203d 3d20 313a 0a20 2020  shape) == 1:.   
+000048f0: 2020 2020 2020 2020 2076 616c 7565 7320           values 
+00004900: 3d20 6e70 2e65 7870 616e 645f 6469 6d73  = np.expand_dims
+00004910: 2876 616c 7565 732c 2031 290a 2020 2020  (values, 1).    
+00004920: 2020 2020 6966 206c 656e 2876 616c 7565      if len(value
+00004930: 732e 7368 6170 6529 203d 3d20 323a 0a20  s.shape) == 2:. 
+00004940: 2020 2020 2020 2020 2020 2076 616c 7565             value
+00004950: 7320 3d20 6e70 2e65 7870 616e 645f 6469  s = np.expand_di
+00004960: 6d73 2876 616c 7565 732c 2032 290a 0a20  ms(values, 2).. 
+00004970: 2020 2020 2020 2063 6f6f 7264 7320 3d20         coords = 
+00004980: 7b74 696d 6573 5f6e 616d 653a 2074 696d  {times_name: tim
+00004990: 6573 7d0a 2020 2020 2020 2020 6966 2063  es}.        if c
+000049a0: 6f6c 756d 6e73 2069 7320 6e6f 7420 4e6f  olumns is not No
+000049b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000049c0: 636f 6f72 6473 5b44 494d 535b 315d 5d20  coords[DIMS[1]] 
+000049d0: 3d20 636f 6c75 6d6e 730a 0a20 2020 2020  = columns..     
+000049e0: 2020 2078 6120 3d20 7872 2e44 6174 6141     xa = xr.DataA
+000049f0: 7272 6179 2876 616c 7565 732c 0a20 2020  rray(values,.   
+00004a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a10: 2020 2020 2020 2064 696d 733d 2874 696d         dims=(tim
+00004a20: 6573 5f6e 616d 652c 2920 2b20 4449 4d53  es_name,) + DIMS
+00004a30: 5b2d 323a 5d2c 0a20 2020 2020 2020 2020  [-2:],.         
+00004a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a50: 2063 6f6f 7264 733d 636f 6f72 6473 290a   coords=coords).
+00004a60: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00004a70: 5469 6d65 5365 7269 6573 2e66 726f 6d5f  TimeSeries.from_
+00004a80: 7861 7272 6179 2878 613d 7861 2c20 6669  xarray(xa=xa, fi
+00004a90: 6c6c 5f6d 6973 7369 6e67 5f64 6174 6573  ll_missing_dates
+00004aa0: 3d66 696c 6c5f 6d69 7373 696e 675f 6461  =fill_missing_da
+00004ab0: 7465 732c 2066 7265 713d 6672 6571 290a  tes, freq=freq).
+00004ac0: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
+00004ad0: 6f64 0a20 2020 2064 6566 2066 726f 6d5f  od.    def from_
+00004ae0: 7661 6c75 6573 2876 616c 7565 733a 206e  values(values: n
+00004af0: 702e 6e64 6172 7261 792c 0a20 2020 2020  p.ndarray,.     
+00004b00: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00004b10: 696c 6c5f 6d69 7373 696e 675f 6461 7465  ill_missing_date
+00004b20: 733a 204f 7074 696f 6e61 6c5b 626f 6f6c  s: Optional[bool
+00004b30: 5d20 3d20 4661 6c73 652c 0a20 2020 2020  ] = False,.     
+00004b40: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00004b50: 7265 713a 204f 7074 696f 6e61 6c5b 7374  req: Optional[st
+00004b60: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+00004b70: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00004b80: 6f6c 756d 6e73 3a20 4f70 7469 6f6e 616c  olumns: Optional
+00004b90: 5b70 642e 5f74 7970 696e 672e 4178 6573  [pd._typing.Axes
+00004ba0: 5d20 3d20 4e6f 6e65 2920 2d3e 2027 5469  ] = None) -> 'Ti
+00004bb0: 6d65 5365 7269 6573 273a 0a20 2020 2020  meSeries':.     
+00004bc0: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
+00004bd0: 6574 7572 6e73 2061 2054 696d 6553 6572  eturns a TimeSer
+00004be0: 6965 7320 6275 696c 7420 6672 6f6d 2061  ies built from a
+00004bf0: 6e20 6172 7261 7920 6f66 2076 616c 7565  n array of value
+00004c00: 732e 0a20 2020 2020 2020 2054 6865 2073  s..        The s
+00004c10: 6572 6965 7320 7769 6c6c 2068 6176 6520  eries will have 
+00004c20: 616e 2069 6e74 6567 6572 2069 6e64 6578  an integer index
+00004c30: 2028 496e 7436 3449 6e64 6578 292e 0a0a   (Int64Index)...
+00004c40: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00004c50: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+00004c60: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7661  -----.        va
+00004c70: 6c75 6573 0a20 2020 2020 2020 2020 2020  lues.           
+00004c80: 2041 204e 756d 7079 2061 7272 6179 206f   A Numpy array o
+00004c90: 6620 7661 6c75 6573 2066 6f72 2074 6865  f values for the
+00004ca0: 2054 696d 6553 6572 6965 732e 2042 6f74   TimeSeries. Bot
+00004cb0: 6820 322d 6469 6d65 6e73 696f 6e61 6c20  h 2-dimensional 
+00004cc0: 6172 7261 7973 2c20 666f 7220 6465 7465  arrays, for dete
+00004cd0: 726d 696e 6973 7469 6320 7365 7269 6573  rministic series
+00004ce0: 2c0a 2020 2020 2020 2020 2020 2020 616e  ,.            an
+00004cf0: 6420 332d 6469 6d65 6e73 696f 6e61 6c20  d 3-dimensional 
+00004d00: 6172 7261 7973 2c20 666f 7220 7072 6f62  arrays, for prob
+00004d10: 6162 696c 6973 7469 6320 7365 7269 6573  abilistic series
+00004d20: 2c20 6172 6520 6163 6365 7074 6564 2e20  , are accepted. 
+00004d30: 496e 2074 6865 2066 6f72 6d65 7220 6361  In the former ca
+00004d40: 7365 2074 6865 2064 696d 656e 7369 6f6e  se the dimension
+00004d50: 730a 2020 2020 2020 2020 2020 2020 7368  s.            sh
+00004d60: 6f75 6c64 2062 6520 2874 696d 652c 2063  ould be (time, c
+00004d70: 6f6d 706f 6e65 6e74 292c 2061 6e64 2069  omponent), and i
+00004d80: 6e20 7468 6520 6c61 7474 6572 2063 6173  n the latter cas
+00004d90: 6520 2874 696d 652c 2063 6f6d 706f 6e65  e (time, compone
+00004da0: 6e74 2c20 7361 6d70 6c65 292e 0a20 2020  nt, sample)..   
+00004db0: 2020 2020 2066 696c 6c5f 6d69 7373 696e       fill_missin
+00004dc0: 675f 6461 7465 730a 2020 2020 2020 2020  g_dates.        
+00004dd0: 2020 2020 4f70 7469 6f6e 616c 6c79 2c20      Optionally, 
+00004de0: 6120 626f 6f6c 6561 6e20 7661 6c75 6520  a boolean value 
+00004df0: 696e 6469 6361 7469 6e67 2077 6865 7468  indicating wheth
+00004e00: 6572 2074 6f20 6669 6c6c 206d 6973 7369  er to fill missi
+00004e10: 6e67 2064 6174 6573 2077 6974 6820 4e61  ng dates with Na
+00004e20: 4e20 7661 6c75 6573 2e20 5468 6973 2072  N values. This r
+00004e30: 6571 7569 7265 730a 2020 2020 2020 2020  equires.        
+00004e40: 2020 2020 6569 7468 6572 2061 2070 726f      either a pro
+00004e50: 7669 6465 6420 6066 7265 7160 206f 7220  vided `freq` or 
+00004e60: 7468 6520 706f 7373 6962 696c 6974 7920  the possibility 
+00004e70: 746f 2069 6e66 6572 2074 6865 2066 7265  to infer the fre
+00004e80: 7175 656e 6379 2066 726f 6d20 7468 6520  quency from the 
+00004e90: 7072 6f76 6964 6564 2074 696d 6573 7461  provided timesta
+00004ea0: 6d70 732e 0a20 2020 2020 2020 2020 2020  mps..           
+00004eb0: 2049 6e66 6572 7269 6e67 2074 6865 2066   Inferring the f
+00004ec0: 7265 7175 656e 6379 2061 6e64 2072 6573  requency and res
+00004ed0: 616d 706c 696e 6720 7468 6520 6461 7461  ampling the data
+00004ee0: 2063 616e 2069 6e64 7563 6520 6120 7369   can induce a si
+00004ef0: 676e 6966 6963 616e 7420 7065 7266 6f72  gnificant perfor
+00004f00: 6d61 6e63 6520 6f76 6572 6865 6164 2e0a  mance overhead..
+00004f10: 2020 2020 2020 2020 6672 6571 0a20 2020          freq.   
+00004f20: 2020 2020 2020 2020 204f 7074 696f 6e61           Optiona
+00004f30: 6c6c 792c 2061 2073 7472 696e 6720 7265  lly, a string re
+00004f40: 7072 6573 656e 7469 6e67 2074 6865 2066  presenting the f
+00004f50: 7265 7175 656e 6379 206f 6620 7468 6520  requency of the 
+00004f60: 5061 6e64 6173 2044 6174 6146 7261 6d65  Pandas DataFrame
+00004f70: 2e20 5468 6973 2069 7320 7573 6566 756c  . This is useful
+00004f80: 2069 6e20 6f72 6465 7220 746f 2066 696c   in order to fil
+00004f90: 6c0a 2020 2020 2020 2020 2020 2020 696e  l.            in
+00004fa0: 206d 6973 7369 6e67 2076 616c 7565 7320   missing values 
+00004fb0: 6966 2073 6f6d 6520 6461 7465 7320 6172  if some dates ar
+00004fc0: 6520 6d69 7373 696e 6720 616e 6420 6066  e missing and `f
+00004fd0: 696c 6c5f 6d69 7373 696e 675f 6461 7465  ill_missing_date
+00004fe0: 7360 2069 7320 7365 7420 746f 2060 5472  s` is set to `Tr
+00004ff0: 7565 602e 0a20 2020 2020 2020 2063 6f6c  ue`..        col
+00005000: 756d 6e73 0a20 2020 2020 2020 2020 2020  umns.           
+00005010: 2043 6f6c 756d 6e73 2074 6f20 6265 2075   Columns to be u
+00005020: 7365 6420 6279 2074 6865 2075 6e64 6572  sed by the under
+00005030: 6c79 696e 6720 7061 6e64 6173 2044 6174  lying pandas Dat
+00005040: 6146 7261 6d65 2e0a 0a20 2020 2020 2020  aFrame...       
+00005050: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+00005060: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+00005070: 2054 696d 6553 6572 6965 730a 2020 2020   TimeSeries.    
+00005080: 2020 2020 2020 2020 4120 5469 6d65 5365          A TimeSe
+00005090: 7269 6573 2063 6f6e 7374 7275 6374 6564  ries constructed
+000050a0: 2066 726f 6d20 7468 6520 696e 7075 7473   from the inputs
+000050b0: 2e0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
+000050c0: 2020 2020 2020 2074 696d 655f 696e 6465         time_inde
+000050d0: 7820 3d20 7064 2e52 616e 6765 496e 6465  x = pd.RangeInde
+000050e0: 7828 302c 206c 656e 2876 616c 7565 7329  x(0, len(values)
+000050f0: 2c20 3129 0a0a 2020 2020 2020 2020 7661  , 1)..        va
+00005100: 6c75 6573 5f20 3d20 6e70 2e72 6573 6861  lues_ = np.resha
+00005110: 7065 2876 616c 7565 732c 2028 6c65 6e28  pe(values, (len(
+00005120: 7661 6c75 6573 292c 2031 2929 2069 6620  values), 1)) if 
+00005130: 6c65 6e28 7661 6c75 6573 2e73 6861 7065  len(values.shape
+00005140: 2920 3d3d 2031 2065 6c73 6520 7661 6c75  ) == 1 else valu
+00005150: 6573 0a20 2020 2020 2020 2072 6574 7572  es.        retur
+00005160: 6e20 5469 6d65 5365 7269 6573 2e66 726f  n TimeSeries.fro
+00005170: 6d5f 7469 6d65 735f 616e 645f 7661 6c75  m_times_and_valu
+00005180: 6573 2874 696d 6573 3d74 696d 655f 696e  es(times=time_in
+00005190: 6465 782c 0a20 2020 2020 2020 2020 2020  dex,.           
+000051a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051c0: 2020 2020 2076 616c 7565 733d 7661 6c75       values=valu
+000051d0: 6573 5f2c 0a20 2020 2020 2020 2020 2020  es_,.           
+000051e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005200: 2020 2020 2066 696c 6c5f 6d69 7373 696e       fill_missin
+00005210: 675f 6461 7465 733d 6669 6c6c 5f6d 6973  g_dates=fill_mis
+00005220: 7369 6e67 5f64 6174 6573 2c0a 2020 2020  sing_dates,.    
+00005230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005250: 2020 2020 2020 2020 2020 2020 6672 6571              freq
+00005260: 3d66 7265 712c 0a20 2020 2020 2020 2020  =freq,.         
+00005270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005290: 2020 2020 2020 2063 6f6c 756d 6e73 3d63         columns=c
+000052a0: 6f6c 756d 6e73 290a 0a20 2020 2040 7374  olumns)..    @st
+000052b0: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
+000052c0: 6566 2066 726f 6d5f 6a73 6f6e 286a 736f  ef from_json(jso
+000052d0: 6e5f 7374 723a 2073 7472 2920 2d3e 2027  n_str: str) -> '
+000052e0: 5469 6d65 5365 7269 6573 273a 0a20 2020  TimeSeries':.   
+000052f0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00005300: 2043 6f6e 7665 7274 7320 7468 6520 4a53   Converts the JS
+00005310: 4f4e 2053 7472 696e 6720 7265 7072 6573  ON String repres
+00005320: 656e 7461 7469 6f6e 206f 6620 6120 6054  entation of a `T
+00005330: 696d 6553 6572 6965 7360 206f 626a 6563  imeSeries` objec
+00005340: 7420 2870 726f 6475 6365 6420 7573 696e  t (produced usin
+00005350: 6720 6054 696d 6553 6572 6965 732e 746f  g `TimeSeries.to
+00005360: 5f6a 736f 6e28 2960 290a 2020 2020 2020  _json()`).      
+00005370: 2020 696e 746f 2061 2060 5469 6d65 5365    into a `TimeSe
+00005380: 7269 6573 6020 6f62 6a65 6374 0a0a 2020  ries` object..  
+00005390: 2020 2020 2020 4174 2074 6865 206d 6f6d        At the mom
+000053a0: 656e 7420 7468 6973 206f 6e6c 7920 7375  ent this only su
+000053b0: 7070 6f72 7473 2064 6574 6572 6d69 6e69  pports determini
+000053c0: 7374 6963 2074 696d 6520 7365 7269 6573  stic time series
+000053d0: 2028 692e 652e 2c20 6d61 6465 206f 6620   (i.e., made of 
+000053e0: 3120 7361 6d70 6c65 292e 0a0a 2020 2020  1 sample)...    
+000053f0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00005400: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00005410: 2d0a 2020 2020 2020 2020 6a73 6f6e 5f73  -.        json_s
+00005420: 7472 0a20 2020 2020 2020 2020 2020 2054  tr.            T
+00005430: 6865 204a 534f 4e20 5374 7269 6e67 2074  he JSON String t
+00005440: 6f20 636f 6e76 6572 740a 0a20 2020 2020  o convert..     
+00005450: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+00005460: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+00005470: 2020 2054 696d 6553 6572 6965 730a 2020     TimeSeries.  
+00005480: 2020 2020 2020 2020 2020 5468 6520 7469            The ti
+00005490: 6d65 2073 6572 6965 7320 6f62 6a65 6374  me series object
+000054a0: 2063 6f6e 7665 7274 6564 2066 726f 6d20   converted from 
+000054b0: 7468 6520 4a53 4f4e 2053 7472 696e 670a  the JSON String.
+000054c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000054d0: 2020 2020 6466 203d 2070 642e 7265 6164      df = pd.read
+000054e0: 5f6a 736f 6e28 6a73 6f6e 5f73 7472 2c20  _json(json_str, 
+000054f0: 6f72 6965 6e74 3d27 7370 6c69 7427 290a  orient='split').
+00005500: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+00005510: 696d 6553 6572 6965 732e 6672 6f6d 5f64  imeSeries.from_d
+00005520: 6174 6166 7261 6d65 2864 6629 0a0a 2020  ataframe(df)..  
+00005530: 2020 2222 220a 2020 2020 5072 6f70 6572    """.    Proper
+00005540: 7469 6573 0a20 2020 203d 3d3d 3d3d 3d3d  ties.    =======
+00005550: 3d3d 3d0a 2020 2020 2222 220a 0a20 2020  ===.    """..   
+00005560: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
+00005570: 6566 206e 5f73 616d 706c 6573 2873 656c  ef n_samples(sel
+00005580: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
+00005590: 726e 206c 656e 2873 656c 662e 5f78 612e  rn len(self._xa.
+000055a0: 7361 6d70 6c65 290a 0a20 2020 2040 7072  sample)..    @pr
+000055b0: 6f70 6572 7479 0a20 2020 2064 6566 206e  operty.    def n
+000055c0: 5f63 6f6d 706f 6e65 6e74 7328 7365 6c66  _components(self
+000055d0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+000055e0: 6e20 6c65 6e28 7365 6c66 2e5f 7861 2e63  n len(self._xa.c
+000055f0: 6f6d 706f 6e65 6e74 290a 0a20 2020 2040  omponent)..    @
+00005600: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00005610: 2077 6964 7468 2873 656c 6629 3a0a 2020   width(self):.  
+00005620: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00005630: 662e 6e5f 636f 6d70 6f6e 656e 7473 0a0a  f.n_components..
+00005640: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00005650: 2020 6465 6620 6e5f 7469 6d65 7374 6570    def n_timestep
+00005660: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+00005670: 2072 6574 7572 6e20 6c65 6e28 7365 6c66   return len(self
+00005680: 2e5f 7469 6d65 5f69 6e64 6578 290a 0a20  ._time_index).. 
+00005690: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+000056a0: 2064 6566 2069 735f 6465 7465 726d 696e   def is_determin
+000056b0: 6973 7469 6328 7365 6c66 293a 0a20 2020  istic(self):.   
+000056c0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+000056d0: 2e6e 5f73 616d 706c 6573 203d 3d20 310a  .n_samples == 1.
+000056e0: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
+000056f0: 2020 2064 6566 2069 735f 7374 6f63 6861     def is_stocha
+00005700: 7374 6963 2873 656c 6629 3a0a 2020 2020  stic(self):.    
+00005710: 2020 2020 7265 7475 726e 206e 6f74 2073      return not s
+00005720: 656c 662e 6973 5f64 6574 6572 6d69 6e69  elf.is_determini
+00005730: 7374 6963 0a0a 2020 2020 4070 726f 7065  stic..    @prope
+00005740: 7274 790a 2020 2020 6465 6620 6973 5f70  rty.    def is_p
+00005750: 726f 6261 6269 6c69 7374 6963 2873 656c  robabilistic(sel
+00005760: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
+00005770: 726e 2073 656c 662e 6973 5f73 746f 6368  rn self.is_stoch
+00005780: 6173 7469 630a 0a20 2020 2040 7072 6f70  astic..    @prop
+00005790: 6572 7479 0a20 2020 2064 6566 2069 735f  erty.    def is_
+000057a0: 756e 6976 6172 6961 7465 2873 656c 6629  univariate(self)
+000057b0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+000057c0: 2073 656c 662e 6e5f 636f 6d70 6f6e 656e   self.n_componen
+000057d0: 7473 203d 3d20 310a 0a20 2020 2040 7072  ts == 1..    @pr
+000057e0: 6f70 6572 7479 0a20 2020 2064 6566 2066  operty.    def f
+000057f0: 7265 7128 7365 6c66 293a 0a20 2020 2020  req(self):.     
+00005800: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00005810: 6672 6571 0a0a 2020 2020 4070 726f 7065  freq..    @prope
+00005820: 7274 790a 2020 2020 6465 6620 6672 6571  rty.    def freq
+00005830: 5f73 7472 2873 656c 6629 3a0a 2020 2020  _str(self):.    
+00005840: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00005850: 5f66 7265 715f 7374 720a 0a20 2020 2040  _freq_str..    @
+00005860: 7072 6f70 6572 7479 0a20 2020 2064 6566  property.    def
+00005870: 2063 6f6d 706f 6e65 6e74 7328 7365 6c66   components(self
+00005880: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00005890: 2020 2020 2020 2054 6865 206e 616d 6573         The names
+000058a0: 206f 6620 7468 6520 636f 6d70 6f6e 656e   of the componen
+000058b0: 7473 2028 6571 7569 7661 6c65 6e74 2074  ts (equivalent t
+000058c0: 6f20 4461 7461 4672 616d 6520 636f 6c75  o DataFrame colu
+000058d0: 6d6e 7329 2061 7320 6120 5061 6e64 6173  mns) as a Pandas
+000058e0: 2049 6e64 6578 0a20 2020 2020 2020 2022   Index.        "
+000058f0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+00005900: 6e20 7365 6c66 2e5f 7861 2e67 6574 5f69  n self._xa.get_i
+00005910: 6e64 6578 2844 494d 535b 315d 292e 636f  ndex(DIMS[1]).co
+00005920: 7079 2829 0a0a 2020 2020 4070 726f 7065  py()..    @prope
+00005930: 7274 790a 2020 2020 6465 6620 636f 6c75  rty.    def colu
+00005940: 6d6e 7328 7365 6c66 293a 0a20 2020 2020  mns(self):.     
+00005950: 2020 2022 2222 0a20 2020 2020 2020 2053     """.        S
+00005960: 616d 6520 6173 2060 636f 6d70 6f6e 656e  ame as `componen
+00005970: 7473 6020 7072 6f70 6572 7479 0a20 2020  ts` property.   
+00005980: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00005990: 2072 6574 7572 6e20 7365 6c66 2e63 6f6d   return self.com
+000059a0: 706f 6e65 6e74 730a 0a20 2020 2040 7072  ponents..    @pr
+000059b0: 6f70 6572 7479 0a20 2020 2064 6566 2074  operty.    def t
+000059c0: 696d 655f 696e 6465 7828 7365 6c66 2920  ime_index(self) 
+000059d0: 2d3e 2055 6e69 6f6e 5b70 642e 4461 7465  -> Union[pd.Date
+000059e0: 7469 6d65 496e 6465 782c 2070 642e 496e  timeIndex, pd.In
+000059f0: 7436 3449 6e64 6578 5d3a 0a20 2020 2020  t64Index]:.     
+00005a00: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
+00005a10: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+00005a20: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2055  ------.        U
+00005a30: 6e69 6f6e 5b70 642e 4461 7465 7469 6d65  nion[pd.Datetime
+00005a40: 496e 6465 782c 2070 642e 496e 7436 3449  Index, pd.Int64I
+00005a50: 6e64 6578 5d0a 2020 2020 2020 2020 2020  ndex].          
+00005a60: 2020 5468 6520 7469 6d65 2069 6e64 6578    The time index
+00005a70: 206f 6620 7468 6973 2074 696d 6520 7365   of this time se
+00005a80: 7269 6573 2e0a 2020 2020 2020 2020 2222  ries..        ""
+00005a90: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+00005aa0: 2073 656c 662e 5f74 696d 655f 696e 6465   self._time_inde
+00005ab0: 782e 636f 7079 2829 0a0a 2020 2020 4070  x.copy()..    @p
+00005ac0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
+00005ad0: 6861 735f 6461 7465 7469 6d65 5f69 6e64  has_datetime_ind
+00005ae0: 6578 2873 656c 6629 202d 3e20 626f 6f6c  ex(self) -> bool
+00005af0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00005b00: 2020 2020 2020 5768 6574 6865 7220 7468        Whether th
+00005b10: 6973 2073 6572 6965 7320 6973 2069 6e64  is series is ind
+00005b20: 6578 6564 2077 6974 6820 6120 4461 7465  exed with a Date
+00005b30: 7469 6d65 496e 6465 7820 286f 7468 6572  timeIndex (other
+00005b40: 7769 7365 2069 7420 6973 2069 6e64 6578  wise it is index
+00005b50: 6564 2077 6974 6820 616e 2049 6e74 3634  ed with an Int64
+00005b60: 496e 6465 7829 0a20 2020 2020 2020 2022  Index).        "
+00005b70: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+00005b80: 6e20 7365 6c66 2e5f 6861 735f 6461 7465  n self._has_date
+00005b90: 7469 6d65 5f69 6e64 6578 0a0a 2020 2020  time_index..    
+00005ba0: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+00005bb0: 6620 6861 735f 7261 6e67 655f 696e 6465  f has_range_inde
+00005bc0: 7828 7365 6c66 2920 2d3e 2062 6f6f 6c3a  x(self) -> bool:
+00005bd0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00005be0: 2020 2020 2057 6865 7468 6572 2074 6869       Whether thi
+00005bf0: 7320 7365 7269 6573 2069 7320 696e 6465  s series is inde
+00005c00: 7865 6420 7769 7468 2061 6e20 496e 7436  xed with an Int6
+00005c10: 3449 6e64 6578 2028 6f74 6865 7277 6973  4Index (otherwis
+00005c20: 6520 6974 2069 7320 696e 6465 7865 6420  e it is indexed 
+00005c30: 7769 7468 2061 2044 6174 6574 696d 6549  with a DatetimeI
+00005c40: 6e64 6578 290a 2020 2020 2020 2020 2222  ndex).        ""
+00005c50: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+00005c60: 206e 6f74 2073 656c 662e 5f68 6173 5f64   not self._has_d
+00005c70: 6174 6574 696d 655f 696e 6465 780a 0a20  atetime_index.. 
+00005c80: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
+00005c90: 2064 6566 2064 7572 6174 696f 6e28 7365   def duration(se
+00005ca0: 6c66 2920 2d3e 2055 6e69 6f6e 5b70 642e  lf) -> Union[pd.
+00005cb0: 5469 6d65 6465 6c74 612c 2069 6e74 5d3a  Timedelta, int]:
+00005cc0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00005cd0: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+00005ce0: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+00005cf0: 2020 2020 2055 6e69 6f6e 5b70 616e 6461       Union[panda
+00005d00: 732e 5469 6d65 6465 6c74 612c 2069 6e74  s.Timedelta, int
+00005d10: 5d0a 2020 2020 2020 2020 2020 2020 5468  ].            Th
+00005d20: 6520 6475 7261 7469 6f6e 206f 6620 7468  e duration of th
+00005d30: 6973 2074 696d 6520 7365 7269 6573 3b20  is time series; 
+00005d40: 6173 2061 2054 696d 6564 656c 7461 2069  as a Timedelta i
+00005d50: 6620 7468 6520 7365 7269 6573 2069 7320  f the series is 
+00005d60: 696e 6465 7865 6420 6279 2061 2044 6174  indexed by a Dat
+00005d70: 6574 696d 6569 6e64 6578 2c0a 2020 2020  etimeindex,.    
+00005d80: 2020 2020 2020 2020 616e 6420 696e 7420          and int 
+00005d90: 6f74 6865 7277 6973 652e 0a20 2020 2020  otherwise..     
+00005da0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+00005db0: 6574 7572 6e20 7365 6c66 2e5f 7469 6d65  eturn self._time
+00005dc0: 5f69 6e64 6578 5b2d 315d 202d 2073 656c  _index[-1] - sel
+00005dd0: 662e 5f74 696d 655f 696e 6465 785b 305d  f._time_index[0]
+00005de0: 0a0a 2020 2020 2222 2220 0a20 2020 2053  ..    """ .    S
+00005df0: 6f6d 6520 6173 7365 7274 730a 2020 2020  ome asserts.    
+00005e00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020  =============.  
+00005e10: 2020 2222 220a 2020 2020 2320 544f 444f    """.    # TODO
+00005e20: 3a20 7075 7420 6174 2074 6865 2062 6f74  : put at the bot
+00005e30: 746f 6d0a 0a20 2020 2064 6566 205f 6173  tom..    def _as
+00005e40: 7365 7274 5f75 6e69 7661 7269 6174 6528  sert_univariate(
+00005e50: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
+00005e60: 6620 6e6f 7420 7365 6c66 2e69 735f 756e  f not self.is_un
+00005e70: 6976 6172 6961 7465 3a0a 2020 2020 2020  ivariate:.      
+00005e80: 2020 2020 2020 7261 6973 655f 6c6f 6728        raise_log(
+00005e90: 4173 7365 7274 696f 6e45 7272 6f72 2827  AssertionError('
+00005ea0: 4f6e 6c79 2075 6e69 7661 7269 6174 6520  Only univariate 
+00005eb0: 5469 6d65 5365 7269 6573 2069 6e73 7461  TimeSeries insta
+00005ec0: 6e63 6573 2073 7570 706f 7274 2074 6869  nces support thi
+00005ed0: 7320 6d65 7468 6f64 2729 2c20 6c6f 6767  s method'), logg
+00005ee0: 6572 290a 0a20 2020 2064 6566 205f 6173  er)..    def _as
+00005ef0: 7365 7274 5f64 6574 6572 6d69 6e69 7374  sert_determinist
+00005f00: 6963 2873 656c 6629 3a0a 2020 2020 2020  ic(self):.      
+00005f10: 2020 6966 206e 6f74 2073 656c 662e 6973    if not self.is
+00005f20: 5f64 6574 6572 6d69 6e69 7374 6963 3a0a  _deterministic:.
+00005f30: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00005f40: 655f 6c6f 6728 4173 7365 7274 696f 6e45  e_log(AssertionE
+00005f50: 7272 6f72 2827 4f6e 6c79 2064 6574 6572  rror('Only deter
+00005f60: 6d69 6e69 7374 6963 2054 696d 6553 6572  ministic TimeSer
+00005f70: 6965 7320 2877 6974 6820 3120 7361 6d70  ies (with 1 samp
+00005f80: 6c65 2920 696e 7374 616e 6365 7320 7375  le) instances su
+00005f90: 7070 6f72 7420 7468 6973 206d 6574 686f  pport this metho
+00005fa0: 6427 292c 0a20 2020 2020 2020 2020 2020  d'),.           
+00005fb0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00005fc0: 7229 0a0a 2020 2020 6465 6620 5f61 7373  r)..    def _ass
+00005fd0: 6572 745f 7374 6f63 6861 7374 6963 2873  ert_stochastic(s
+00005fe0: 656c 6629 3a0a 2020 2020 2020 2020 6966  elf):.        if
+00005ff0: 206e 6f74 2073 656c 662e 6973 5f73 746f   not self.is_sto
+00006000: 6368 6173 7469 633a 0a20 2020 2020 2020  chastic:.       
+00006010: 2020 2020 2072 6169 7365 5f6c 6f67 2841       raise_log(A
+00006020: 7373 6572 7469 6f6e 4572 726f 7228 274f  ssertionError('O
+00006030: 6e6c 7920 6e6f 6e2d 6465 7465 726d 696e  nly non-determin
+00006040: 6973 7469 6320 5469 6d65 5365 7269 6573  istic TimeSeries
+00006050: 2028 7769 7468 206d 6f72 6520 7468 616e   (with more than
+00006060: 2031 2073 616d 706c 6573 2920 270a 2020   1 samples) '.  
+00006070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006090: 2020 2027 696e 7374 616e 6365 7320 7375     'instances su
+000060a0: 7070 6f72 7420 7468 6973 206d 6574 686f  pport this metho
+000060b0: 6427 292c 0a20 2020 2020 2020 2020 2020  d'),.           
+000060c0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+000060d0: 7229 0a0a 2020 2020 6465 6620 5f72 6169  r)..    def _rai
+000060e0: 7365 5f69 665f 6e6f 745f 7769 7468 696e  se_if_not_within
+000060f0: 2873 656c 662c 2074 733a 2055 6e69 6f6e  (self, ts: Union
+00006100: 5b70 642e 5469 6d65 7374 616d 702c 2069  [pd.Timestamp, i
+00006110: 6e74 5d29 3a0a 2020 2020 2020 2020 6966  nt]):.        if
+00006120: 2069 7369 6e73 7461 6e63 6528 7473 2c20   isinstance(ts, 
+00006130: 7064 2e54 696d 6573 7461 6d70 293a 0a20  pd.Timestamp):. 
+00006140: 2020 2020 2020 2020 2020 2023 204e 6f74             # Not
+00006150: 2074 6861 7420 7468 6520 636f 6e76 6572   that the conver
+00006160: 7365 2064 6f65 736e 2774 2061 7070 6c79  se doesn't apply
+00006170: 2028 6120 7469 6d65 2d69 6e64 6578 6564   (a time-indexed
+00006180: 2073 6572 6965 7320 6361 6e20 6265 2063   series can be c
+00006190: 616c 6c65 6420 7769 7468 2061 6e20 696e  alled with an in
+000061a0: 7465 6765 7229 0a20 2020 2020 2020 2020  teger).         
+000061b0: 2020 2072 6169 7365 5f69 665f 6e6f 7428     raise_if_not(
+000061c0: 7365 6c66 2e5f 6861 735f 6461 7465 7469  self._has_dateti
+000061d0: 6d65 5f69 6e64 6578 2c0a 2020 2020 2020  me_index,.      
 000061e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061f0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00006200: 6c75 6d6e 733d 7365 6c66 2e5f 7861 2e67  lumns=self._xa.g
-00006210: 6574 5f69 6e64 6578 2827 636f 6d70 6f6e  et_index('compon
-00006220: 656e 7427 292e 636f 7079 2829 290a 2020  ent').copy()).  
-00006230: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00006240: 2020 2020 2020 2020 7265 7475 726e 2070          return p
-00006250: 642e 4461 7461 4672 616d 6528 7365 6c66  d.DataFrame(self
-00006260: 2e5f 7861 5b3a 2c20 3a2c 2030 5d2e 7661  ._xa[:, :, 0].va
-00006270: 6c75 6573 2c0a 2020 2020 2020 2020 2020  lues,.          
-00006280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006290: 2020 2020 2020 696e 6465 783d 7365 6c66        index=self
-000062a0: 2e5f 7469 6d65 5f69 6e64 6578 2c0a 2020  ._time_index,.  
-000062b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062c0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000062d0: 6c75 6d6e 733d 7365 6c66 2e5f 7861 2e67  lumns=self._xa.g
-000062e0: 6574 5f69 6e64 6578 2827 636f 6d70 6f6e  et_index('compon
-000062f0: 656e 7427 2929 0a0a 2020 2020 6465 6620  ent'))..    def 
-00006300: 7175 616e 7469 6c65 5f64 6628 7365 6c66  quantile_df(self
-00006310: 2c20 7175 616e 7469 6c65 3d30 2e35 2920  , quantile=0.5) 
-00006320: 2d3e 2070 642e 4461 7461 4672 616d 653a  -> pd.DataFrame:
-00006330: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00006340: 2020 2020 2052 6574 7572 6e73 2061 2050       Returns a P
-00006350: 616e 6461 7320 4461 7461 4672 616d 6520  andas DataFrame 
-00006360: 636f 6e74 6169 6e69 6e67 2074 6865 2073  containing the s
-00006370: 696e 676c 6520 6465 7369 7265 6420 7175  ingle desired qu
-00006380: 616e 7469 6c65 206f 6620 6561 6368 2063  antile of each c
-00006390: 6f6d 706f 6e65 6e74 2028 6f76 6572 2074  omponent (over t
-000063a0: 6865 2073 616d 706c 6573 292e 0a20 2020  he samples)..   
-000063b0: 2020 2020 2045 6163 6820 6f66 2074 6865       Each of the
-000063c0: 2073 6572 6965 7320 636f 6d70 6f6e 656e   series componen
-000063d0: 7473 2077 696c 6c20 6170 7065 6172 2061  ts will appear a
-000063e0: 7320 6120 636f 6c75 6d6e 2069 6e20 7468  s a column in th
-000063f0: 6520 4461 7461 4672 616d 652e 2054 6865  e DataFrame. The
-00006400: 2063 6f6c 756d 6e20 7769 6c6c 2062 6520   column will be 
-00006410: 6e61 6d65 640a 2020 2020 2020 2020 223c  named.        "<
-00006420: 636f 6d70 6f6e 656e 743e 5f58 222c 2077  component>_X", w
-00006430: 6865 7265 2022 3c63 6f6d 706f 6e65 6e74  here "<component
-00006440: 3e22 2069 7320 7468 6520 636f 6c75 6d6e  >" is the column
-00006450: 206e 616d 6520 636f 7272 6573 706f 6e64   name correspond
-00006460: 696e 6720 746f 2074 6869 7320 636f 6d70  ing to this comp
-00006470: 6f6e 656e 742c 2061 6e64 2022 5822 0a20  onent, and "X". 
-00006480: 2020 2020 2020 2069 7320 7468 6520 7175         is the qu
-00006490: 616e 7469 6c65 2076 616c 7565 2e0a 2020  antile value..  
-000064a0: 2020 2020 2020 5468 6520 7175 616e 7469        The quanti
-000064b0: 6c65 2063 6f6c 756d 6e73 2072 6570 7265  le columns repre
-000064c0: 7365 6e74 2074 6865 206d 6172 6769 6e61  sent the margina
-000064d0: 6c20 6469 7374 7269 6275 7469 6f6e 7320  l distributions 
-000064e0: 6f66 2074 6865 2063 6f6d 706f 6e65 6e74  of the component
-000064f0: 7320 6f66 2074 6869 7320 7365 7269 6573  s of this series
-00006500: 2e0a 0a20 2020 2020 2020 2054 6869 7320  ...        This 
-00006510: 776f 726b 7320 6f6e 6c79 206f 6e20 7374  works only on st
-00006520: 6f63 6861 7374 6963 2073 6572 6965 7320  ochastic series 
-00006530: 2869 2e65 2e2c 2077 6974 6820 6d6f 7265  (i.e., with more
-00006540: 2074 6861 6e20 3120 7361 6d70 6c65 290a   than 1 sample).
-00006550: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00006560: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-00006570: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2071  ------.        q
-00006580: 7561 6e74 696c 650a 2020 2020 2020 2020  uantile.        
-00006590: 2020 2020 5468 6520 6465 7369 7265 6420      The desired 
-000065a0: 7175 616e 7469 6c65 2076 616c 7565 2e20  quantile value. 
-000065b0: 5468 6520 7661 6c75 6520 6d75 7374 2062  The value must b
-000065c0: 6520 7265 7072 6573 656e 7465 6420 6173  e represented as
-000065d0: 2061 2066 7261 6374 696f 6e0a 2020 2020   a fraction.    
-000065e0: 2020 2020 2020 2020 2862 6574 7765 656e          (between
-000065f0: 2030 2061 6e64 2031 2069 6e63 6c75 7369   0 and 1 inclusi
-00006600: 7665 292e 2046 6f72 2069 6e73 7461 6e63  ve). For instanc
-00006610: 652c 2060 302e 3560 2077 696c 6c20 7265  e, `0.5` will re
-00006620: 7475 726e 2061 2044 6174 6146 7261 6d65  turn a DataFrame
-00006630: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-00006640: 7461 696e 696e 6720 7468 6520 6d65 6469  taining the medi
-00006650: 616e 206f 6620 7468 6520 286d 6172 6769  an of the (margi
-00006660: 6e61 6c29 2064 6973 7472 6962 7574 696f  nal) distributio
-00006670: 6e20 6f66 2065 6163 6820 636f 6d70 6f6e  n of each compon
-00006680: 656e 742e 0a0a 2020 2020 2020 2020 5265  ent...        Re
-00006690: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
-000066a0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7061  -----.        pa
-000066b0: 6e64 6173 2e44 6174 6146 7261 6d65 0a20  ndas.DataFrame. 
-000066c0: 2020 2020 2020 2020 2020 2054 6865 2050             The P
-000066d0: 616e 6461 7320 4461 7461 4672 616d 6520  andas DataFrame 
-000066e0: 636f 6e74 6169 6e69 6e67 2074 6865 2064  containing the d
-000066f0: 6573 6972 6564 2071 7561 6e74 696c 6520  esired quantile 
-00006700: 666f 7220 6561 6368 2063 6f6d 706f 6e65  for each compone
-00006710: 6e74 2e0a 2020 2020 2020 2020 2222 220a  nt..        """.
-00006720: 2020 2020 2020 2020 7365 6c66 2e5f 6173          self._as
-00006730: 7365 7274 5f73 746f 6368 6173 7469 6328  sert_stochastic(
-00006740: 290a 2020 2020 2020 2020 7261 6973 655f  ).        raise_
-00006750: 6966 5f6e 6f74 2830 203c 3d20 7175 616e  if_not(0 <= quan
-00006760: 7469 6c65 203c 3d20 312c 0a20 2020 2020  tile <= 1,.     
-00006770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006780: 2754 6865 2071 7561 6e74 696c 6520 7661  'The quantile va
-00006790: 6c75 6573 206d 7573 7420 6265 2065 7870  lues must be exp
-000067a0: 7265 7373 6564 2061 7320 6672 6163 7469  ressed as fracti
-000067b0: 6f6e 2028 6265 7477 6565 6e20 3020 616e  on (between 0 an
-000067c0: 6420 3120 696e 636c 7573 6976 6529 2e27  d 1 inclusive).'
-000067d0: 2c20 6c6f 6767 6572 290a 0a20 2020 2020  , logger)..     
-000067e0: 2020 2023 2063 6f6c 756d 6e20 6e61 6d65     # column name
-000067f0: 730a 2020 2020 2020 2020 636e 616d 6573  s.        cnames
-00006800: 203d 205b 7320 2b20 275f 7b7d 272e 666f   = [s + '_{}'.fo
-00006810: 726d 6174 2871 7561 6e74 696c 6529 2066  rmat(quantile) f
-00006820: 6f72 2073 2069 6e20 7365 6c66 2e63 6f6c  or s in self.col
-00006830: 756d 6e73 5d0a 0a20 2020 2020 2020 2072  umns]..        r
-00006840: 6574 7572 6e20 7064 2e44 6174 6146 7261  eturn pd.DataFra
-00006850: 6d65 2873 656c 662e 5f78 612e 7175 616e  me(self._xa.quan
-00006860: 7469 6c65 2871 3d71 7561 6e74 696c 652c  tile(q=quantile,
-00006870: 2064 696d 3d44 494d 535b 325d 292c 0a20   dim=DIMS[2]),. 
-00006880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006890: 2020 2020 2020 2020 2020 2069 6e64 6578             index
-000068a0: 3d73 656c 662e 5f74 696d 655f 696e 6465  =self._time_inde
-000068b0: 782c 0a20 2020 2020 2020 2020 2020 2020  x,.             
-000068c0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000068d0: 6f6c 756d 6e73 3d63 6e61 6d65 7329 0a0a  olumns=cnames)..
-000068e0: 2020 2020 6465 6620 7175 616e 7469 6c65      def quantile
-000068f0: 5f74 696d 6573 6572 6965 7328 7365 6c66  _timeseries(self
-00006900: 2c20 7175 616e 7469 6c65 3d30 2e35 2920  , quantile=0.5) 
-00006910: 2d3e 2027 5469 6d65 5365 7269 6573 273a  -> 'TimeSeries':
-00006920: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00006930: 2020 2020 2052 6574 7572 6e73 2061 2064       Returns a d
-00006940: 6574 6572 6d69 6e69 7374 6963 2060 5469  eterministic `Ti
-00006950: 6d65 5365 7269 6573 6020 636f 6e74 6169  meSeries` contai
-00006960: 6e69 6e67 2074 6865 2073 696e 676c 6520  ning the single 
-00006970: 6465 7369 7265 6420 7175 616e 7469 6c65  desired quantile
-00006980: 206f 6620 6561 6368 2063 6f6d 706f 6e65   of each compone
-00006990: 6e74 0a20 2020 2020 2020 2028 6f76 6572  nt.        (over
-000069a0: 2074 6865 2073 616d 706c 6573 2920 6f66   the samples) of
-000069b0: 2074 6869 7320 7374 6f63 6861 7374 6963   this stochastic
-000069c0: 2060 5469 6d65 5365 7269 6573 602e 0a20   `TimeSeries`.. 
-000069d0: 2020 2020 2020 2054 6865 2063 6f6d 706f         The compo
-000069e0: 6e65 6e74 7320 696e 2074 6865 206e 6577  nents in the new
-000069f0: 2073 6572 6965 7320 6172 6520 6e61 6d65   series are name
-00006a00: 6420 223c 636f 6d70 6f6e 656e 743e 5f58  d "<component>_X
-00006a10: 222c 2077 6865 7265 2022 3c63 6f6d 706f  ", where "<compo
-00006a20: 6e65 6e74 3e22 0a20 2020 2020 2020 2069  nent>".        i
-00006a30: 7320 7468 6520 636f 6c75 6d6e 206e 616d  s the column nam
-00006a40: 6520 636f 7272 6573 706f 6e64 696e 6720  e corresponding 
-00006a50: 746f 2074 6869 7320 636f 6d70 6f6e 656e  to this componen
-00006a60: 742c 2061 6e64 2022 5822 2069 7320 7468  t, and "X" is th
-00006a70: 6520 7175 616e 7469 6c65 2076 616c 7565  e quantile value
-00006a80: 2e0a 2020 2020 2020 2020 5468 6520 7175  ..        The qu
-00006a90: 616e 7469 6c65 2063 6f6c 756d 6e73 2072  antile columns r
-00006aa0: 6570 7265 7365 6e74 2074 6865 206d 6172  epresent the mar
-00006ab0: 6769 6e61 6c20 6469 7374 7269 6275 7469  ginal distributi
-00006ac0: 6f6e 7320 6f66 2074 6865 2063 6f6d 706f  ons of the compo
-00006ad0: 6e65 6e74 7320 6f66 2074 6869 7320 7365  nents of this se
-00006ae0: 7269 6573 2e0a 0a20 2020 2020 2020 2054  ries...        T
-00006af0: 6869 7320 776f 726b 7320 6f6e 6c79 206f  his works only o
-00006b00: 6e20 7374 6f63 6861 7374 6963 2073 6572  n stochastic ser
-00006b10: 6965 7320 2869 2e65 2e2c 2077 6974 6820  ies (i.e., with 
-00006b20: 6d6f 7265 2074 6861 6e20 3120 7361 6d70  more than 1 samp
-00006b30: 6c65 290a 0a20 2020 2020 2020 2050 6172  le)..        Par
-00006b40: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-00006b50: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-00006b60: 2020 2071 7561 6e74 696c 650a 2020 2020     quantile.    
-00006b70: 2020 2020 2020 2020 5468 6520 6465 7369          The desi
-00006b80: 7265 6420 7175 616e 7469 6c65 2076 616c  red quantile val
-00006b90: 7565 2e20 5468 6520 7661 6c75 6520 6d75  ue. The value mu
-00006ba0: 7374 2062 6520 7265 7072 6573 656e 7465  st be represente
-00006bb0: 6420 6173 2061 2066 7261 6374 696f 6e0a  d as a fraction.
-00006bc0: 2020 2020 2020 2020 2020 2020 2862 6574              (bet
-00006bd0: 7765 656e 2030 2061 6e64 2031 2069 6e63  ween 0 and 1 inc
-00006be0: 6c75 7369 7665 292e 2046 6f72 2069 6e73  lusive). For ins
-00006bf0: 7461 6e63 652c 2060 302e 3560 2077 696c  tance, `0.5` wil
-00006c00: 6c20 7265 7475 726e 2061 2054 696d 6553  l return a TimeS
-00006c10: 6572 6965 730a 2020 2020 2020 2020 2020  eries.          
-00006c20: 2020 636f 6e74 6169 6e69 6e67 2074 6865    containing the
-00006c30: 206d 6564 6961 6e20 6f66 2074 6865 2028   median of the (
-00006c40: 6d61 7267 696e 616c 2920 6469 7374 7269  marginal) distri
-00006c50: 6275 7469 6f6e 206f 6620 6561 6368 2063  bution of each c
-00006c60: 6f6d 706f 6e65 6e74 2e0a 0a20 2020 2020  omponent...     
-00006c70: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-00006c80: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-00006c90: 2020 2054 696d 6553 6572 6965 730a 2020     TimeSeries.  
-00006ca0: 2020 2020 2020 2020 2020 5468 6520 5469            The Ti
-00006cb0: 6d65 5365 7269 6573 2063 6f6e 7461 696e  meSeries contain
-00006cc0: 696e 6720 7468 6520 6465 7369 7265 6420  ing the desired 
-00006cd0: 7175 616e 7469 6c65 2066 6f72 2065 6163  quantile for eac
-00006ce0: 6820 636f 6d70 6f6e 656e 742e 0a20 2020  h component..   
-00006cf0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00006d00: 2072 6574 7572 6e20 5469 6d65 5365 7269   return TimeSeri
-00006d10: 6573 2e66 726f 6d5f 6461 7461 6672 616d  es.from_datafram
-00006d20: 6528 7365 6c66 2e71 7561 6e74 696c 655f  e(self.quantile_
-00006d30: 6466 2871 7561 6e74 696c 6529 290a 0a20  df(quantile)).. 
-00006d40: 2020 2064 6566 2071 7561 6e74 696c 6573     def quantiles
-00006d50: 5f64 6628 7365 6c66 2c20 7175 616e 7469  _df(self, quanti
-00006d60: 6c65 733a 2054 7570 6c65 5b66 6c6f 6174  les: Tuple[float
-00006d70: 5d20 3d20 2830 2e31 2c20 302e 352c 2030  ] = (0.1, 0.5, 0
-00006d80: 2e39 2929 202d 3e20 7064 2e44 6174 6146  .9)) -> pd.DataF
-00006d90: 7261 6d65 3a0a 2020 2020 2020 2020 2222  rame:.        ""
-00006da0: 220a 2020 2020 2020 2020 5265 7475 726e  ".        Return
-00006db0: 7320 6120 5061 6e64 6173 2044 6174 6146  s a Pandas DataF
-00006dc0: 7261 6d65 2063 6f6e 7461 696e 696e 6720  rame containing 
-00006dd0: 7468 6520 6465 7369 7265 6420 7175 616e  the desired quan
-00006de0: 7469 6c65 7320 6f66 2065 6163 6820 636f  tiles of each co
-00006df0: 6d70 6f6e 656e 7420 286f 7665 7220 7468  mponent (over th
-00006e00: 6520 7361 6d70 6c65 7329 2e0a 2020 2020  e samples)..    
-00006e10: 2020 2020 4561 6368 206f 6620 7468 6520      Each of the 
-00006e20: 7365 7269 6573 2063 6f6d 706f 6e65 6e74  series component
-00006e30: 7320 7769 6c6c 2061 7070 6561 7220 6173  s will appear as
-00006e40: 2061 2063 6f6c 756d 6e20 696e 2074 6865   a column in the
-00006e50: 2044 6174 6146 7261 6d65 2e20 5468 6520   DataFrame. The 
-00006e60: 636f 6c75 6d6e 2077 696c 6c20 6265 206e  column will be n
-00006e70: 616d 6564 0a20 2020 2020 2020 2022 3c63  amed.        "<c
-00006e80: 6f6d 706f 6e65 6e74 3e5f 5822 2c20 7768  omponent>_X", wh
-00006e90: 6572 6520 223c 636f 6d70 6f6e 656e 743e  ere "<component>
-00006ea0: 2220 6973 2074 6865 2063 6f6c 756d 6e20  " is the column 
-00006eb0: 6e61 6d65 2063 6f72 7265 7370 6f6e 6469  name correspondi
-00006ec0: 6e67 2074 6f20 7468 6973 2063 6f6d 706f  ng to this compo
-00006ed0: 6e65 6e74 2c20 616e 6420 2258 220a 2020  nent, and "X".  
-00006ee0: 2020 2020 2020 6973 2074 6865 2071 7561        is the qua
-00006ef0: 6e74 696c 6520 7661 6c75 652e 0a20 2020  ntile value..   
-00006f00: 2020 2020 2054 6865 2071 7561 6e74 696c       The quantil
-00006f10: 6573 2072 6570 7265 7365 6e74 2074 6865  es represent the
-00006f20: 206d 6172 6769 6e61 6c20 6469 7374 7269   marginal distri
-00006f30: 6275 7469 6f6e 7320 6f66 2074 6865 2063  butions of the c
-00006f40: 6f6d 706f 6e65 6e74 7320 6f66 2074 6869  omponents of thi
-00006f50: 7320 7365 7269 6573 2e0a 0a20 2020 2020  s series...     
-00006f60: 2020 2054 6869 7320 776f 726b 7320 6f6e     This works on
-00006f70: 6c79 206f 6e20 7374 6f63 6861 7374 6963  ly on stochastic
-00006f80: 2073 6572 6965 7320 2869 2e65 2e2c 2077   series (i.e., w
-00006f90: 6974 6820 6d6f 7265 2074 6861 6e20 3120  ith more than 1 
-00006fa0: 7361 6d70 6c65 290a 0a20 2020 2020 2020  sample)..       
-00006fb0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00006fc0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00006fd0: 2020 2020 2020 2071 7561 6e74 696c 6573         quantiles
-00006fe0: 0a20 2020 2020 2020 2020 2020 2054 7570  .            Tup
-00006ff0: 6c65 2063 6f6e 7461 696e 696e 6720 7468  le containing th
-00007000: 6520 6465 7369 7265 6420 7175 616e 7469  e desired quanti
-00007010: 6c65 732e 2054 6865 2076 616c 7565 7320  les. The values 
-00007020: 6d75 7374 2062 6520 7265 7072 6573 656e  must be represen
-00007030: 7465 6420 6173 2066 7261 6374 696f 6e73  ted as fractions
-00007040: 0a20 2020 2020 2020 2020 2020 2028 6265  .            (be
-00007050: 7477 6565 6e20 3020 616e 6420 3120 696e  tween 0 and 1 in
-00007060: 636c 7573 6976 6529 2e20 466f 7220 696e  clusive). For in
-00007070: 7374 616e 6365 2c20 6028 302e 312c 2030  stance, `(0.1, 0
-00007080: 2e35 2c20 302e 3929 6020 7769 6c6c 2072  .5, 0.9)` will r
-00007090: 6574 7572 6e20 6120 4461 7461 4672 616d  eturn a DataFram
-000070a0: 650a 2020 2020 2020 2020 2020 2020 636f  e.            co
-000070b0: 6e74 6169 6e69 6e67 2074 6865 2031 3074  ntaining the 10t
-000070c0: 682d 7065 7263 656e 7469 6c65 2c20 6d65  h-percentile, me
-000070d0: 6469 616e 2061 6e64 2039 3074 682d 7065  dian and 90th-pe
-000070e0: 7263 656e 7469 6c65 206f 6620 7468 6520  rcentile of the 
-000070f0: 286d 6172 6769 6e61 6c29 2064 6973 7472  (marginal) distr
-00007100: 6962 7574 696f 6e20 6f66 2065 6163 6820  ibution of each 
-00007110: 636f 6d70 6f6e 656e 742e 0a0a 2020 2020  component...    
-00007120: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00007130: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00007140: 2020 2020 7061 6e64 6173 2e44 6174 6146      pandas.DataF
-00007150: 7261 6d65 0a20 2020 2020 2020 2020 2020  rame.           
-00007160: 2054 6865 2050 616e 6461 7320 4461 7461   The Pandas Data
-00007170: 4672 616d 6520 636f 6e74 6169 6e69 6e67  Frame containing
-00007180: 2074 6865 2071 7561 6e74 696c 6573 2066   the quantiles f
-00007190: 6f72 2065 6163 6820 636f 6d70 6f6e 656e  or each componen
-000071a0: 742e 0a20 2020 2020 2020 2022 2222 0a20  t..        """. 
-000071b0: 2020 2020 2020 2023 2054 4f44 4f3a 2074         # TODO: t
-000071c0: 6865 7265 206d 6967 6874 2062 6520 6120  here might be a 
-000071d0: 736c 6967 6874 6c79 206d 6f72 6520 6566  slightly more ef
-000071e0: 6669 6369 656e 7420 7761 7920 746f 2064  ficient way to d
-000071f0: 6f20 6974 2066 6f72 2073 6576 6572 616c  o it for several
-00007200: 2071 7561 6e74 696c 6573 2061 7420 6f6e   quantiles at on
-00007210: 6365 2077 6974 6820 7861 7272 6179 2e2e  ce with xarray..
-00007220: 2e0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00007230: 2070 642e 636f 6e63 6174 285b 7365 6c66   pd.concat([self
-00007240: 2e71 7561 6e74 696c 655f 6466 2871 7561  .quantile_df(qua
-00007250: 6e74 696c 6529 2066 6f72 2071 7561 6e74  ntile) for quant
-00007260: 696c 6520 696e 2071 7561 6e74 696c 6573  ile in quantiles
-00007270: 5d2c 2061 7869 733d 3129 0a0a 2020 2020  ], axis=1)..    
-00007280: 6465 6620 7374 6172 745f 7469 6d65 2873  def start_time(s
-00007290: 656c 6629 202d 3e20 556e 696f 6e5b 7064  elf) -> Union[pd
-000072a0: 2e54 696d 6573 7461 6d70 2c20 696e 745d  .Timestamp, int]
-000072b0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000072c0: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
-000072d0: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-000072e0: 2020 2020 2020 556e 696f 6e5b 7061 6e64        Union[pand
-000072f0: 6173 2e54 696d 6573 7461 6d70 2c20 696e  as.Timestamp, in
-00007300: 745d 0a20 2020 2020 2020 2020 2020 2041  t].            A
-00007310: 2074 696d 6573 7461 6d70 2063 6f6e 7461   timestamp conta
-00007320: 696e 696e 6720 7468 6520 6669 7273 7420  ining the first 
-00007330: 7469 6d65 206f 6620 7468 6520 5469 6d65  time of the Time
-00007340: 5365 7269 6573 2028 6966 2069 6e64 6578  Series (if index
-00007350: 6564 2062 7920 4461 7465 7469 6d65 496e  ed by DatetimeIn
-00007360: 6465 7829 2c0a 2020 2020 2020 2020 2020  dex),.          
-00007370: 2020 6f72 2061 6e20 696e 7465 6765 7220    or an integer 
-00007380: 2869 6620 696e 6465 7865 6420 6279 2052  (if indexed by R
-00007390: 616e 6765 496e 6465 7829 0a20 2020 2020  angeIndex).     
-000073a0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-000073b0: 6574 7572 6e20 7365 6c66 2e5f 7469 6d65  eturn self._time
-000073c0: 5f69 6e64 6578 5b30 5d0a 0a20 2020 2064  _index[0]..    d
-000073d0: 6566 2065 6e64 5f74 696d 6528 7365 6c66  ef end_time(self
-000073e0: 2920 2d3e 2055 6e69 6f6e 5b70 642e 5469  ) -> Union[pd.Ti
-000073f0: 6d65 7374 616d 702c 2069 6e74 5d3a 0a20  mestamp, int]:. 
-00007400: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00007410: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-00007420: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-00007430: 2020 2055 6e69 6f6e 5b70 616e 6461 732e     Union[pandas.
-00007440: 5469 6d65 7374 616d 702c 2069 6e74 5d0a  Timestamp, int].
-00007450: 2020 2020 2020 2020 2020 2020 4120 7469              A ti
-00007460: 6d65 7374 616d 7020 636f 6e74 6169 6e69  mestamp containi
-00007470: 6e67 2074 6865 206c 6173 7420 7469 6d65  ng the last time
-00007480: 206f 6620 7468 6520 5469 6d65 5365 7269   of the TimeSeri
-00007490: 6573 2028 6966 2069 6e64 6578 6564 2062  es (if indexed b
-000074a0: 7920 4461 7465 7469 6d65 496e 6465 7829  y DatetimeIndex)
-000074b0: 2c0a 2020 2020 2020 2020 2020 2020 6f72  ,.            or
-000074c0: 2061 6e20 696e 7465 6765 7220 2869 6620   an integer (if 
-000074d0: 696e 6465 7865 6420 6279 2052 616e 6765  indexed by Range
-000074e0: 496e 6465 7829 0a20 2020 2020 2020 2022  Index).        "
-000074f0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-00007500: 6e20 7365 6c66 2e5f 7469 6d65 5f69 6e64  n self._time_ind
-00007510: 6578 5b2d 315d 0a0a 2020 2020 6465 6620  ex[-1]..    def 
-00007520: 6669 7273 745f 7661 6c75 6528 7365 6c66  first_value(self
-00007530: 2920 2d3e 2066 6c6f 6174 3a0a 2020 2020  ) -> float:.    
-00007540: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00007550: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
-00007560: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00007570: 666c 6f61 740a 2020 2020 2020 2020 2020  float.          
-00007580: 2020 5468 6520 6669 7273 7420 7661 6c75    The first valu
-00007590: 6520 6f66 2074 6869 7320 756e 6976 6172  e of this univar
-000075a0: 6961 7465 2064 6574 6572 6d69 6e69 7374  iate determinist
-000075b0: 6963 2074 696d 6520 7365 7269 6573 0a20  ic time series. 
-000075c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000075d0: 2020 2073 656c 662e 5f61 7373 6572 745f     self._assert_
-000075e0: 756e 6976 6172 6961 7465 2829 0a20 2020  univariate().   
-000075f0: 2020 2020 2073 656c 662e 5f61 7373 6572       self._asser
-00007600: 745f 6465 7465 726d 696e 6973 7469 6328  t_deterministic(
-00007610: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00007620: 2066 6c6f 6174 2873 656c 662e 5f78 615b   float(self._xa[
-00007630: 302c 2030 2c20 305d 290a 0a20 2020 2064  0, 0, 0])..    d
-00007640: 6566 206c 6173 745f 7661 6c75 6528 7365  ef last_value(se
-00007650: 6c66 2920 2d3e 2066 6c6f 6174 3a0a 2020  lf) -> float:.  
-00007660: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00007670: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-00007680: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-00007690: 2020 666c 6f61 740a 2020 2020 2020 2020    float.        
-000076a0: 2020 2020 5468 6520 6c61 7374 2076 616c      The last val
-000076b0: 7565 206f 6620 7468 6973 2075 6e69 7661  ue of this univa
-000076c0: 7269 6174 6520 6465 7465 726d 696e 6973  riate determinis
-000076d0: 7469 6320 7469 6d65 2073 6572 6965 730a  tic time series.
-000076e0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000076f0: 2020 2020 7365 6c66 2e5f 6173 7365 7274      self._assert
-00007700: 5f75 6e69 7661 7269 6174 6528 290a 2020  _univariate().  
-00007710: 2020 2020 2020 7365 6c66 2e5f 6173 7365        self._asse
-00007720: 7274 5f64 6574 6572 6d69 6e69 7374 6963  rt_deterministic
-00007730: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
-00007740: 6e20 666c 6f61 7428 7365 6c66 2e5f 7861  n float(self._xa
-00007750: 5b2d 312c 2030 2c20 305d 290a 0a20 2020  [-1, 0, 0])..   
-00007760: 2064 6566 2066 6972 7374 5f76 616c 7565   def first_value
-00007770: 7328 7365 6c66 2920 2d3e 206e 702e 6e64  s(self) -> np.nd
-00007780: 6172 7261 793a 0a20 2020 2020 2020 2022  array:.        "
-00007790: 2222 0a20 2020 2020 2020 2052 6574 7572  "".        Retur
-000077a0: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
-000077b0: 2d2d 0a20 2020 2020 2020 206e 702e 6e64  --.        np.nd
-000077c0: 6172 7261 790a 2020 2020 2020 2020 2020  array.          
-000077d0: 2020 5468 6520 6669 7273 7420 7661 6c75    The first valu
-000077e0: 6573 206f 6620 6576 6572 7920 636f 6d70  es of every comp
-000077f0: 6f6e 656e 7420 6f66 2074 6869 7320 6465  onent of this de
-00007800: 7465 726d 696e 6973 7469 6320 7469 6d65  terministic time
-00007810: 2073 6572 6965 730a 2020 2020 2020 2020   series.        
-00007820: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
-00007830: 2e5f 6173 7365 7274 5f64 6574 6572 6d69  ._assert_determi
-00007840: 6e69 7374 6963 2829 0a20 2020 2020 2020  nistic().       
-00007850: 2072 6574 7572 6e20 7365 6c66 2e5f 7861   return self._xa
-00007860: 2e76 616c 7565 735b 302c 203a 2c20 305d  .values[0, :, 0]
-00007870: 2e63 6f70 7928 290a 0a20 2020 2064 6566  .copy()..    def
-00007880: 206c 6173 745f 7661 6c75 6573 2873 656c   last_values(sel
-00007890: 6629 202d 3e20 6e70 2e6e 6461 7272 6179  f) -> np.ndarray
-000078a0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000078b0: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
-000078c0: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-000078d0: 2020 2020 2020 6e70 2e6e 6461 7272 6179        np.ndarray
-000078e0: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-000078f0: 206c 6173 7420 7661 6c75 6573 206f 6620   last values of 
-00007900: 6576 6572 7920 636f 6d70 6f6e 656e 7420  every component 
-00007910: 6f66 2074 6869 7320 6465 7465 726d 696e  of this determin
-00007920: 6973 7469 6320 7469 6d65 2073 6572 6965  istic time serie
-00007930: 730a 2020 2020 2020 2020 2222 220a 2020  s.        """.  
-00007940: 2020 2020 2020 7365 6c66 2e5f 6173 7365        self._asse
-00007950: 7274 5f64 6574 6572 6d69 6e69 7374 6963  rt_deterministic
-00007960: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
-00007970: 6e20 7365 6c66 2e5f 7861 2e76 616c 7565  n self._xa.value
-00007980: 735b 2d31 2c20 3a2c 2030 5d2e 636f 7079  s[-1, :, 0].copy
-00007990: 2829 0a0a 2020 2020 6465 6620 7661 6c75  ()..    def valu
-000079a0: 6573 2873 656c 662c 2063 6f70 793d 5472  es(self, copy=Tr
-000079b0: 7565 2c20 7361 6d70 6c65 3d30 2920 2d3e  ue, sample=0) ->
-000079c0: 206e 702e 6e64 6172 7261 793a 0a20 2020   np.ndarray:.   
-000079d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000079e0: 2052 6574 7572 6e73 2061 2032 2d44 204e   Returns a 2-D N
-000079f0: 756d 7079 2061 7272 6179 206f 6620 6469  umpy array of di
-00007a00: 6d65 6e73 696f 6e20 2874 696d 652c 2063  mension (time, c
-00007a10: 6f6d 706f 6e65 6e74 292c 2063 6f6e 7461  omponent), conta
-00007a20: 696e 696e 6720 7468 6973 2073 6572 6965  ining this serie
-00007a30: 7327 2076 616c 7565 7320 666f 7220 6f6e  s' values for on
-00007a40: 6520 7361 6d70 6c65 2e0a 2020 2020 2020  e sample..      
-00007a50: 2020 4966 2074 6869 7320 7365 7269 6573    If this series
-00007a60: 2069 7320 6465 7465 726d 696e 6973 7469   is deterministi
-00007a70: 632c 2069 7420 636f 6e74 6169 6e73 206f  c, it contains o
-00007a80: 6e6c 7920 6f6e 6520 7361 6d70 6c65 2061  nly one sample a
-00007a90: 6e64 206f 6e6c 7920 6073 616d 706c 653d  nd only `sample=
-00007aa0: 3060 2063 616e 2062 6520 7573 6564 2e0a  0` can be used..
-00007ab0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00007ac0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-00007ad0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2063  ------.        c
-00007ae0: 6f70 790a 2020 2020 2020 2020 2020 2020  opy.            
-00007af0: 5768 6574 6865 7220 746f 2072 6574 7572  Whether to retur
-00007b00: 6e20 6120 636f 7079 206f 6620 7468 6520  n a copy of the 
-00007b10: 7661 6c75 6573 2c20 6f74 6865 7277 6973  values, otherwis
-00007b20: 6520 7265 7475 726e 7320 6120 7669 6577  e returns a view
-00007b30: 2e0a 2020 2020 2020 2020 2020 2020 4c65  ..            Le
-00007b40: 6176 6520 6974 2074 6f20 5472 7565 2075  ave it to True u
-00007b50: 6e6c 6573 7320 796f 7520 6b6e 6f77 2077  nless you know w
-00007b60: 6861 7420 796f 7520 6172 6520 646f 696e  hat you are doin
-00007b70: 672e 0a0a 2020 2020 2020 2020 5265 7475  g...        Retu
-00007b80: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-00007b90: 2d2d 2d0a 2020 2020 2020 2020 6e75 6d70  ---.        nump
-00007ba0: 792e 6e64 6172 7261 790a 2020 2020 2020  y.ndarray.      
-00007bb0: 2020 2020 2020 5468 6520 7661 6c75 6573        The values
-00007bc0: 2063 6f6d 706f 7369 6e67 2074 6865 2074   composing the t
-00007bd0: 696d 6520 7365 7269 6573 2e0a 2020 2020  ime series..    
-00007be0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00007bf0: 7261 6973 655f 6966 2873 656c 662e 6973  raise_if(self.is
-00007c00: 5f64 6574 6572 6d69 6e69 7374 6963 2061  _deterministic a
-00007c10: 6e64 2073 616d 706c 6520 213d 2030 2c20  nd sample != 0, 
-00007c20: 2754 6869 7320 7365 7269 6573 2063 6f6e  'This series con
-00007c30: 7461 696e 7320 6f6e 6520 7361 6d70 6c65  tains one sample
-00007c40: 206f 6e6c 7920 2864 6574 6572 6d69 6e69   only (determini
-00007c50: 7374 6963 292c 270a 2020 2020 2020 2020  stic),'.        
-00007c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c90: 2773 6f20 6f6e 6c79 2073 616d 706c 653d  'so only sample=
-00007ca0: 3020 6973 2061 6363 6570 7465 642e 272c  0 is accepted.',
-00007cb0: 206c 6f67 6765 7229 0a20 2020 2020 2020   logger).       
-00007cc0: 2069 6620 636f 7079 3a0a 2020 2020 2020   if copy:.      
-00007cd0: 2020 2020 2020 7265 7475 726e 206e 702e        return np.
-00007ce0: 636f 7079 2873 656c 662e 5f78 612e 7661  copy(self._xa.va
-00007cf0: 6c75 6573 5b3a 2c20 3a2c 2073 616d 706c  lues[:, :, sampl
-00007d00: 655d 290a 2020 2020 2020 2020 656c 7365  e]).        else
-00007d10: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00007d20: 7475 726e 2073 656c 662e 5f78 612e 7661  turn self._xa.va
-00007d30: 6c75 6573 5b3a 2c20 3a2c 2073 616d 706c  lues[:, :, sampl
-00007d40: 655d 0a0a 2020 2020 6465 6620 616c 6c5f  e]..    def all_
-00007d50: 7661 6c75 6573 2873 656c 662c 2063 6f70  values(self, cop
-00007d60: 793d 5472 7565 2920 2d3e 206e 702e 6e64  y=True) -> np.nd
-00007d70: 6172 7261 793a 0a20 2020 2020 2020 2022  array:.        "
-00007d80: 2222 0a20 2020 2020 2020 2052 6574 7572  "".        Retur
-00007d90: 6e73 2061 2033 2d44 204e 756d 7079 2061  ns a 3-D Numpy a
-00007da0: 7272 6179 206f 6620 6469 6d65 6e73 696f  rray of dimensio
-00007db0: 6e20 2874 696d 652c 2063 6f6d 706f 6e65  n (time, compone
-00007dc0: 6e74 2c20 7361 6d70 6c65 292c 0a20 2020  nt, sample),.   
-00007dd0: 2020 2020 2063 6f6e 7461 696e 696e 6720       containing 
-00007de0: 7468 6973 2073 6572 6965 7327 2076 616c  this series' val
-00007df0: 7565 7320 666f 7220 616c 6c20 7361 6d70  ues for all samp
-00007e00: 6c65 732e 0a0a 2020 2020 2020 2020 5061  les...        Pa
-00007e10: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-00007e20: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00007e30: 2020 2020 636f 7079 0a20 2020 2020 2020      copy.       
-00007e40: 2020 2020 2057 6865 7468 6572 2074 6f20       Whether to 
-00007e50: 7265 7475 726e 2061 2063 6f70 7920 6f66  return a copy of
-00007e60: 2074 6865 2076 616c 7565 732c 206f 7468   the values, oth
-00007e70: 6572 7769 7365 2072 6574 7572 6e73 2061  erwise returns a
-00007e80: 2076 6965 772e 0a20 2020 2020 2020 2020   view..         
-00007e90: 2020 204c 6561 7665 2069 7420 746f 2054     Leave it to T
-00007ea0: 7275 6520 756e 6c65 7373 2079 6f75 206b  rue unless you k
-00007eb0: 6e6f 7720 7768 6174 2079 6f75 2061 7265  now what you are
-00007ec0: 2064 6f69 6e67 2e0a 0a20 2020 2020 2020   doing...       
-00007ed0: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-00007ee0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-00007ef0: 206e 756d 7079 2e6e 6461 7272 6179 0a20   numpy.ndarray. 
-00007f00: 2020 2020 2020 2020 2020 2054 6865 2076             The v
-00007f10: 616c 7565 7320 636f 6d70 6f73 696e 6720  alues composing 
-00007f20: 7468 6520 7469 6d65 2073 6572 6965 732e  the time series.
-00007f30: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00007f40: 2020 2020 2069 6620 636f 7079 3a0a 2020       if copy:.  
-00007f50: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00007f60: 206e 702e 636f 7079 2873 656c 662e 5f78   np.copy(self._x
-00007f70: 612e 7661 6c75 6573 290a 2020 2020 2020  a.values).      
-00007f80: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00007f90: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00007fa0: 5f78 612e 7661 6c75 6573 0a0a 2020 2020  _xa.values..    
-00007fb0: 6465 6620 756e 6976 6172 6961 7465 5f76  def univariate_v
-00007fc0: 616c 7565 7328 7365 6c66 2c20 636f 7079  alues(self, copy
-00007fd0: 3d54 7275 652c 2073 616d 706c 653d 3029  =True, sample=0)
-00007fe0: 202d 3e20 6e70 2e6e 6461 7272 6179 3a0a   -> np.ndarray:.
-00007ff0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00008000: 2020 2020 5265 7475 726e 7320 6120 312d      Returns a 1-
-00008010: 4420 4e75 6d70 7920 6172 7261 7920 6f66  D Numpy array of
-00008020: 2064 696d 656e 7369 6f6e 2028 7469 6d65   dimension (time
-00008030: 2c29 2c20 636f 6e74 6169 6e69 6e67 2074  ,), containing t
-00008040: 6869 7320 756e 6976 6172 6961 7465 2073  his univariate s
-00008050: 6572 6965 7327 2076 616c 7565 7320 666f  eries' values fo
-00008060: 7220 6f6e 6520 7361 6d70 6c65 2e0a 2020  r one sample..  
-00008070: 2020 2020 2020 4966 2074 6869 7320 7365        If this se
-00008080: 7269 6573 2069 7320 6465 7465 726d 696e  ries is determin
-00008090: 6973 7469 632c 2069 7420 636f 6e74 6169  istic, it contai
-000080a0: 6e73 206f 6e6c 7920 6f6e 6520 7361 6d70  ns only one samp
-000080b0: 6c65 2061 6e64 206f 6e6c 7920 6073 616d  le and only `sam
-000080c0: 706c 653d 3060 2063 616e 2062 6520 7573  ple=0` can be us
-000080d0: 6564 2e0a 0a20 2020 2020 2020 2050 6172  ed...        Par
-000080e0: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-000080f0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-00008100: 2020 2063 6f70 790a 2020 2020 2020 2020     copy.        
-00008110: 2020 2020 5768 6574 6865 7220 746f 2072      Whether to r
-00008120: 6574 7572 6e20 6120 636f 7079 206f 6620  eturn a copy of 
-00008130: 7468 6520 7661 6c75 6573 2e20 4c65 6176  the values. Leav
-00008140: 6520 6974 2074 6f20 5472 7565 2075 6e6c  e it to True unl
-00008150: 6573 7320 796f 7520 6b6e 6f77 2077 6861  ess you know wha
-00008160: 7420 796f 7520 6172 6520 646f 696e 672e  t you are doing.
-00008170: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00008180: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00008190: 2d0a 2020 2020 2020 2020 6e75 6d70 792e  -.        numpy.
-000081a0: 6e64 6172 7261 790a 2020 2020 2020 2020  ndarray.        
-000081b0: 2020 2020 5468 6520 7661 6c75 6573 2063      The values c
-000081c0: 6f6d 706f 7369 6e67 2074 6865 2074 696d  omposing the tim
-000081d0: 6520 7365 7269 6573 2067 7561 7261 6e74  e series guarant
-000081e0: 6565 6420 746f 2062 6520 756e 6976 6172  eed to be univar
-000081f0: 6961 7465 2e0a 2020 2020 2020 2020 2222  iate..        ""
-00008200: 220a 0a20 2020 2020 2020 2073 656c 662e  "..        self.
-00008210: 5f61 7373 6572 745f 756e 6976 6172 6961  _assert_univaria
-00008220: 7465 2829 0a20 2020 2020 2020 2069 6620  te().        if 
-00008230: 636f 7079 3a0a 2020 2020 2020 2020 2020  copy:.          
-00008240: 2020 7265 7475 726e 206e 702e 636f 7079    return np.copy
-00008250: 2873 656c 662e 5f78 615b 3a2c 2030 2c20  (self._xa[:, 0, 
-00008260: 7361 6d70 6c65 5d2e 7661 6c75 6573 290a  sample].values).
-00008270: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00008280: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00008290: 2073 656c 662e 5f78 615b 3a2c 2030 2c20   self._xa[:, 0, 
-000082a0: 7361 6d70 6c65 5d2e 7661 6c75 6573 0a0a  sample].values..
-000082b0: 2020 2020 2222 220a 2020 2020 4f74 6865      """.    Othe
-000082c0: 7220 6d65 7468 6f64 730a 2020 2020 3d3d  r methods.    ==
-000082d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020  ===========.    
-000082e0: 2222 220a 0a20 2020 2064 6566 2067 6170  """..    def gap
-000082f0: 7328 7365 6c66 2920 2d3e 2070 642e 4461  s(self) -> pd.Da
-00008300: 7461 4672 616d 653a 0a20 2020 2020 2020  taFrame:.       
-00008310: 2022 2222 0a20 2020 2020 2020 2041 2066   """.        A f
-00008320: 756e 6374 696f 6e20 746f 2063 6f6d 7075  unction to compu
-00008330: 7465 2061 6e64 2072 6574 7572 6e20 6761  te and return ga
-00008340: 7073 2069 6e20 7468 6520 5469 6d65 5365  ps in the TimeSe
-00008350: 7269 6573 2e20 576f 726b 7320 6f6e 6c79  ries. Works only
-00008360: 206f 6e20 6465 7465 726d 696e 6973 7469   on deterministi
-00008370: 6320 7469 6d65 2073 6572 6965 7320 2831  c time series (1
-00008380: 2073 616d 706c 6529 2e0a 0a20 2020 2020   sample)...     
-00008390: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-000083a0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-000083b0: 2020 2070 642e 4461 7461 4672 616d 650a     pd.DataFrame.
-000083c0: 2020 2020 2020 2020 2020 2020 4120 7061              A pa
-000083d0: 6e64 6173 2e44 6174 6146 7261 6d65 2063  ndas.DataFrame c
-000083e0: 6f6e 7461 696e 696e 6720 6120 726f 7720  ontaining a row 
-000083f0: 666f 7220 6576 6572 7920 6761 7020 2872  for every gap (r
-00008400: 6f77 7320 7769 7468 2061 6c6c 2d4e 614e  ows with all-NaN
-00008410: 2076 616c 7565 7320 696e 2075 6e64 6572   values in under
-00008420: 6c79 696e 6720 4461 7461 4672 616d 6529  lying DataFrame)
-00008430: 0a20 2020 2020 2020 2020 2020 2069 6e20  .            in 
-00008440: 7468 6973 2074 696d 6520 7365 7269 6573  this time series
-00008450: 2e20 5468 6520 4461 7461 4672 616d 6520  . The DataFrame 
-00008460: 636f 6e74 6169 6e73 2074 6872 6565 2063  contains three c
-00008470: 6f6c 756d 6e73 2074 6861 7420 696e 636c  olumns that incl
-00008480: 7564 6520 7468 6520 7374 6172 7420 616e  ude the start an
-00008490: 6420 656e 6420 7469 6d65 2073 7461 6d70  d end time stamp
-000084a0: 730a 2020 2020 2020 2020 2020 2020 6f66  s.            of
-000084b0: 2074 6865 2067 6170 2061 6e64 2074 6865   the gap and the
-000084c0: 2069 6e74 6567 6572 206c 656e 6774 6820   integer length 
-000084d0: 6f66 2074 6865 2067 6170 2028 696e 2060  of the gap (in `
-000084e0: 7365 6c66 2e66 7265 7160 2075 6e69 7473  self.freq` units
-000084f0: 2069 6620 7468 6520 7365 7269 6573 2069   if the series i
-00008500: 7320 696e 6465 7865 640a 2020 2020 2020  s indexed.      
-00008510: 2020 2020 2020 6279 2061 2044 6174 6574        by a Datet
-00008520: 696d 6549 6e64 6578 292e 0a20 2020 2020  imeIndex)..     
-00008530: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-00008540: 6466 203d 2073 656c 662e 7064 5f64 6174  df = self.pd_dat
-00008550: 6166 7261 6d65 2829 0a0a 2020 2020 2020  aframe()..      
-00008560: 2020 6973 5f6e 616e 5f73 6572 6965 7320    is_nan_series 
-00008570: 3d20 6466 2e69 736e 6128 292e 616c 6c28  = df.isna().all(
-00008580: 6178 6973 3d31 292e 6173 7479 7065 2869  axis=1).astype(i
-00008590: 6e74 290a 2020 2020 2020 2020 6469 6666  nt).        diff
-000085a0: 203d 2070 642e 5365 7269 6573 286e 702e   = pd.Series(np.
-000085b0: 6469 6666 2869 735f 6e61 6e5f 7365 7269  diff(is_nan_seri
-000085c0: 6573 2e76 616c 7565 7329 2c20 696e 6465  es.values), inde
-000085d0: 783d 6973 5f6e 616e 5f73 6572 6965 732e  x=is_nan_series.
-000085e0: 696e 6465 785b 3a2d 315d 290a 2020 2020  index[:-1]).    
-000085f0: 2020 2020 6761 705f 7374 6172 7473 203d      gap_starts =
-00008600: 2064 6966 665b 6469 6666 203d 3d20 315d   diff[diff == 1]
-00008610: 2e69 6e64 6578 202b 2073 656c 662e 5f66  .index + self._f
-00008620: 7265 710a 2020 2020 2020 2020 6761 705f  req.        gap_
-00008630: 656e 6473 203d 2064 6966 665b 6469 6666  ends = diff[diff
-00008640: 203d 3d20 2d31 5d2e 696e 6465 780a 0a20   == -1].index.. 
-00008650: 2020 2020 2020 2069 6620 6973 5f6e 616e         if is_nan
-00008660: 5f73 6572 6965 732e 696c 6f63 5b30 5d20  _series.iloc[0] 
-00008670: 3d3d 2031 3a0a 2020 2020 2020 2020 2020  == 1:.          
-00008680: 2020 6761 705f 7374 6172 7473 203d 2067    gap_starts = g
-00008690: 6170 5f73 7461 7274 732e 696e 7365 7274  ap_starts.insert
-000086a0: 2830 2c20 7365 6c66 2e73 7461 7274 5f74  (0, self.start_t
-000086b0: 696d 6528 2929 0a20 2020 2020 2020 2069  ime()).        i
-000086c0: 6620 6973 5f6e 616e 5f73 6572 6965 732e  f is_nan_series.
-000086d0: 696c 6f63 5b2d 315d 203d 3d20 313a 0a20  iloc[-1] == 1:. 
-000086e0: 2020 2020 2020 2020 2020 2067 6170 5f65             gap_e
-000086f0: 6e64 7320 3d20 6761 705f 656e 6473 2e69  nds = gap_ends.i
-00008700: 6e73 6572 7428 6c65 6e28 6761 705f 656e  nsert(len(gap_en
-00008710: 6473 292c 2073 656c 662e 656e 645f 7469  ds), self.end_ti
-00008720: 6d65 2829 290a 0a20 2020 2020 2020 2067  me())..        g
-00008730: 6170 5f64 6620 3d20 7064 2e44 6174 6146  ap_df = pd.DataF
-00008740: 7261 6d65 2829 0a20 2020 2020 2020 2067  rame().        g
-00008750: 6170 5f64 665b 2767 6170 5f73 7461 7274  ap_df['gap_start
-00008760: 275d 203d 2067 6170 5f73 7461 7274 730a  '] = gap_starts.
-00008770: 2020 2020 2020 2020 6761 705f 6466 5b27          gap_df['
-00008780: 6761 705f 656e 6427 5d20 3d20 6761 705f  gap_end'] = gap_
-00008790: 656e 6473 0a0a 2020 2020 2020 2020 6465  ends..        de
-000087a0: 6620 696e 7476 6c28 7374 6172 742c 2065  f intvl(start, e
-000087b0: 6e64 293a 0a20 2020 2020 2020 2020 2020  nd):.           
-000087c0: 2069 6620 7365 6c66 2e5f 6861 735f 6461   if self._has_da
-000087d0: 7465 7469 6d65 5f69 6e64 6578 3a0a 2020  tetime_index:.  
-000087e0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000087f0: 7475 726e 2070 642e 6461 7465 5f72 616e  turn pd.date_ran
-00008800: 6765 2873 7461 7274 3d73 7461 7274 2c20  ge(start=start, 
-00008810: 656e 643d 656e 642c 2066 7265 713d 7365  end=end, freq=se
-00008820: 6c66 2e5f 6672 6571 292e 7369 7a65 0a20  lf._freq).size. 
-00008830: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00008840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008850: 2072 6574 7572 6e20 7374 6172 7420 2d20   return start - 
-00008860: 656e 640a 0a20 2020 2020 2020 2067 6170  end..        gap
-00008870: 5f64 665b 2767 6170 5f73 697a 6527 5d20  _df['gap_size'] 
-00008880: 3d20 6761 705f 6466 2e61 7070 6c79 280a  = gap_df.apply(.
-00008890: 2020 2020 2020 2020 2020 2020 6c61 6d62              lamb
-000088a0: 6461 2072 6f77 3a20 696e 7476 6c28 7374  da row: intvl(st
-000088b0: 6172 743d 726f 772e 6761 705f 7374 6172  art=row.gap_star
-000088c0: 742c 2065 6e64 3d72 6f77 2e67 6170 5f65  t, end=row.gap_e
-000088d0: 6e64 292c 2061 7869 733d 310a 2020 2020  nd), axis=1.    
-000088e0: 2020 2020 290a 0a20 2020 2020 2020 2072      )..        r
-000088f0: 6574 7572 6e20 6761 705f 6466 0a0a 2020  eturn gap_df..  
-00008900: 2020 6465 6620 636f 7079 2873 656c 6629    def copy(self)
-00008910: 202d 3e20 2754 696d 6553 6572 6965 7327   -> 'TimeSeries'
-00008920: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00008930: 2020 2020 2020 4d61 6b65 2061 2063 6f70        Make a cop
-00008940: 7920 6f66 2074 6869 7320 7469 6d65 2073  y of this time s
-00008950: 6572 6965 7320 6f62 6a65 6374 0a0a 2020  eries object..  
-00008960: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
-00008970: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-00008980: 2020 2020 2020 5469 6d65 5365 7269 6573        TimeSeries
-00008990: 0a20 2020 2020 2020 2020 2020 2041 2063  .            A c
-000089a0: 6f70 7920 6f66 2074 6869 7320 7469 6d65  opy of this time
-000089b0: 2073 6572 6965 732e 0a20 2020 2020 2020   series..       
-000089c0: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-000089d0: 7572 6e20 5469 6d65 5365 7269 6573 2873  urn TimeSeries(s
-000089e0: 656c 662e 5f78 6129 2020 2320 7468 6520  elf._xa)  # the 
-000089f0: 7861 7272 6179 2077 696c 6c20 6265 2063  xarray will be c
-00008a00: 6f70 6965 6420 696e 2074 6865 2054 696d  opied in the Tim
-00008a10: 6553 6572 6965 7320 636f 6e73 7472 7563  eSeries construc
-00008a20: 746f 720a 0a20 2020 2064 6566 2067 6574  tor..    def get
-00008a30: 5f69 6e64 6578 5f61 745f 706f 696e 7428  _index_at_point(
-00008a40: 7365 6c66 2c20 706f 696e 743a 2055 6e69  self, point: Uni
-00008a50: 6f6e 5b70 642e 5469 6d65 7374 616d 702c  on[pd.Timestamp,
-00008a60: 2066 6c6f 6174 2c20 696e 745d 2c20 6166   float, int], af
-00008a70: 7465 723d 5472 7565 2920 2d3e 2069 6e74  ter=True) -> int
-00008a80: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00008a90: 2020 2020 2020 436f 6e76 6572 7473 2061        Converts a
-00008aa0: 2070 6f69 6e74 2069 6e74 6f20 616e 2069   point into an i
-00008ab0: 6e74 6567 6572 2069 6e64 6578 0a0a 2020  nteger index..  
-00008ac0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00008ad0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00008ae0: 2d2d 2d0a 2020 2020 2020 2020 706f 696e  ---.        poin
-00008af0: 740a 2020 2020 2020 2020 2020 2020 5468  t.            Th
-00008b00: 6973 2070 6172 616d 6574 6572 2073 7570  is parameter sup
-00008b10: 706f 7274 7320 3320 6469 6666 6572 656e  ports 3 differen
-00008b20: 7420 6461 7461 2074 7970 6573 3a20 6070  t data types: `p
-00008b30: 642e 5469 6d65 7374 616d 7060 2c20 6066  d.Timestamp`, `f
-00008b40: 6c6f 6174 6020 616e 6420 6069 6e74 602e  loat` and `int`.
-00008b50: 0a0a 2020 2020 2020 2020 2020 2020 6070  ..            `p
-00008b60: 642e 5469 6d65 7374 616d 7060 2077 6f72  d.Timestamp` wor
-00008b70: 6b20 6f6e 6c79 206f 6e20 7365 7269 6573  k only on series
-00008b80: 2074 6861 7420 6172 6520 696e 6465 7865   that are indexe
-00008b90: 6420 7769 7468 2061 2060 7064 2e44 6174  d with a `pd.Dat
-00008ba0: 6574 696d 6549 6e64 6578 602e 2049 6e20  etimeIndex`. In 
-00008bb0: 7375 6368 2063 6173 6573 2c20 7468 6520  such cases, the 
-00008bc0: 7265 7475 726e 6564 0a20 2020 2020 2020  returned.       
-00008bd0: 2020 2020 2070 6f69 6e74 2077 696c 6c20       point will 
-00008be0: 6265 2074 6865 2069 6e64 6578 206f 6620  be the index of 
-00008bf0: 7468 6973 2074 696d 6573 7461 6d70 2069  this timestamp i
-00008c00: 6620 6974 2069 7320 7072 6573 656e 7420  f it is present 
-00008c10: 696e 2074 6865 2073 6572 6965 7320 7469  in the series ti
-00008c20: 6d65 2069 6e64 6578 2e20 4974 2069 7427  me index. It it'
-00008c30: 7320 6e6f 7420 7072 6573 656e 740a 2020  s not present.  
-00008c40: 2020 2020 2020 2020 2020 696e 2074 6865            in the
-00008c50: 2074 696d 6520 696e 6465 782c 2074 6865   time index, the
-00008c60: 2069 6e64 6578 206f 6620 7468 6520 6e65   index of the ne
-00008c70: 7874 2074 696d 6573 7461 6d70 2069 7320  xt timestamp is 
-00008c80: 7265 7475 726e 6564 2069 6620 6061 6674  returned if `aft
-00008c90: 6572 3d54 7275 6560 2028 6966 2069 7420  er=True` (if it 
-00008ca0: 6578 6973 7473 2069 6e20 7468 6520 7365  exists in the se
-00008cb0: 7269 6573 292c 0a20 2020 2020 2020 2020  ries),.         
-00008cc0: 2020 206f 7468 6572 7769 7365 2074 6865     otherwise the
-00008cd0: 2069 6e64 6578 206f 6620 7468 6520 7072   index of the pr
-00008ce0: 6576 696f 7573 2074 696d 6573 7461 6d70  evious timestamp
-00008cf0: 2069 7320 7265 7475 726e 6564 2028 6966   is returned (if
-00008d00: 2069 7420 6578 6973 7473 2069 6e20 7468   it exists in th
-00008d10: 6520 7365 7269 6573 292e 0a0a 2020 2020  e series)...    
-00008d20: 2020 2020 2020 2020 496e 2063 6173 6520          In case 
-00008d30: 6f66 2061 2060 666c 6f61 7460 2c20 7468  of a `float`, th
-00008d40: 6520 7061 7261 6d65 7465 7220 7769 6c6c  e parameter will
-00008d50: 2062 6520 7472 6561 7465 6420 6173 2074   be treated as t
-00008d60: 6865 2070 726f 706f 7274 696f 6e20 6f66  he proportion of
-00008d70: 2074 6865 2074 696d 6520 7365 7269 6573   the time series
-00008d80: 0a20 2020 2020 2020 2020 2020 2074 6861  .            tha
-00008d90: 7420 7368 6f75 6c64 206c 6965 2062 6566  t should lie bef
-00008da0: 6f72 6520 7468 6520 706f 696e 742e 0a0a  ore the point...
-00008db0: 2020 2020 2020 2020 2020 2020 496e 2074              In t
-00008dc0: 6865 2063 6173 6520 6f66 2060 696e 7460  he case of `int`
-00008dd0: 2c20 7468 6520 7061 7261 6d65 7465 7220  , the parameter 
-00008de0: 7769 6c6c 2072 6574 7572 6e65 6420 6173  will returned as
-00008df0: 2073 7563 682c 2070 726f 7669 6465 6420   such, provided 
-00008e00: 7468 6174 2069 7420 6973 2069 6e20 7468  that it is in th
-00008e10: 6520 7365 7269 6573 2e20 4f74 6865 7277  e series. Otherw
-00008e20: 6973 650a 2020 2020 2020 2020 2020 2020  ise.            
-00008e30: 6974 2077 696c 6c20 7261 6973 6520 6120  it will raise a 
-00008e40: 5661 6c75 6545 7272 6f72 2e0a 2020 2020  ValueError..    
-00008e50: 2020 2020 6166 7465 720a 2020 2020 2020      after.      
-00008e60: 2020 2020 2020 4966 2074 6865 2070 726f        If the pro
-00008e70: 7669 6465 6420 7061 6e64 6173 2054 696d  vided pandas Tim
-00008e80: 6573 7461 6d70 2069 7320 6e6f 7420 696e  estamp is not in
-00008e90: 2074 6865 2074 696d 6520 7365 7269 6573   the time series
-00008ea0: 2069 6e64 6578 2c20 7768 6574 6865 7220   index, whether 
-00008eb0: 746f 2072 6574 7572 6e20 7468 6520 696e  to return the in
-00008ec0: 6465 7820 6f66 2074 6865 0a20 2020 2020  dex of the.     
-00008ed0: 2020 2020 2020 206e 6578 7420 7469 6d65         next time
-00008ee0: 7374 616d 7020 6f72 2074 6865 2069 6e64  stamp or the ind
-00008ef0: 6578 206f 6620 7468 6520 7072 6576 696f  ex of the previo
-00008f00: 7573 206f 6e65 2e0a 0a20 2020 2020 2020  us one...       
-00008f10: 2022 2222 0a20 2020 2020 2020 2070 6f69   """.        poi
-00008f20: 6e74 5f69 6e64 6578 203d 202d 310a 2020  nt_index = -1.  
-00008f30: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00008f40: 6e63 6528 706f 696e 742c 2066 6c6f 6174  nce(point, float
-00008f50: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-00008f60: 6169 7365 5f69 665f 6e6f 7428 302e 203c  aise_if_not(0. <
-00008f70: 3d20 706f 696e 7420 3c3d 2031 2e2c 2027  = point <= 1., '
-00008f80: 706f 696e 7420 2866 6c6f 6174 2920 7368  point (float) sh
-00008f90: 6f75 6c64 2062 6520 6265 7477 6565 6e20  ould be between 
-00008fa0: 302e 3020 616e 6420 312e 302e 272c 206c  0.0 and 1.0.', l
-00008fb0: 6f67 6765 7229 0a20 2020 2020 2020 2020  ogger).         
-00008fc0: 2020 2070 6f69 6e74 5f69 6e64 6578 203d     point_index =
-00008fd0: 2069 6e74 2828 6c65 6e28 7365 6c66 2920   int((len(self) 
-00008fe0: 2d20 3129 202a 2070 6f69 6e74 290a 2020  - 1) * point).  
-00008ff0: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
-00009000: 7461 6e63 6528 706f 696e 742c 2069 6e74  tance(point, int
-00009010: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-00009020: 6169 7365 5f69 6628 706f 696e 7420 6e6f  aise_if(point no
-00009030: 7420 696e 2072 616e 6765 286c 656e 2873  t in range(len(s
-00009040: 656c 6629 292c 2022 706f 696e 7420 2869  elf)), "point (i
-00009050: 6e74 2920 7368 6f75 6c64 2062 6520 6120  nt) should be a 
-00009060: 7661 6c69 6420 696e 6465 7820 696e 2073  valid index in s
-00009070: 6572 6965 7322 2c20 6c6f 6767 6572 290a  eries", logger).
-00009080: 2020 2020 2020 2020 2020 2020 706f 696e              poin
-00009090: 745f 696e 6465 7820 3d20 706f 696e 740a  t_index = point.
-000090a0: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
-000090b0: 6e73 7461 6e63 6528 706f 696e 742c 2070  nstance(point, p
-000090c0: 642e 5469 6d65 7374 616d 7029 3a0a 2020  d.Timestamp):.  
-000090d0: 2020 2020 2020 2020 2020 7261 6973 655f            raise_
-000090e0: 6966 5f6e 6f74 2873 656c 662e 5f68 6173  if_not(self._has
-000090f0: 5f64 6174 6574 696d 655f 696e 6465 782c  _datetime_index,
-00009100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009110: 2020 2020 2020 2020 2020 2741 2054 696d            'A Tim
-00009120: 6573 7461 6d70 2068 6173 2062 6565 6e20  estamp has been 
-00009130: 7072 6f76 6964 6564 2c20 6275 7420 7468  provided, but th
-00009140: 6973 2073 6572 6965 7320 6973 206e 6f74  is series is not
-00009150: 2074 696d 652d 696e 6465 7865 642e 272c   time-indexed.',
-00009160: 206c 6f67 6765 7229 0a20 2020 2020 2020   logger).       
-00009170: 2020 2020 2073 656c 662e 5f72 6169 7365       self._raise
-00009180: 5f69 665f 6e6f 745f 7769 7468 696e 2870  _if_not_within(p
-00009190: 6f69 6e74 290a 2020 2020 2020 2020 2020  oint).          
-000091a0: 2020 6966 2070 6f69 6e74 2069 6e20 7365    if point in se
-000091b0: 6c66 3a0a 2020 2020 2020 2020 2020 2020  lf:.            
-000091c0: 2020 2020 706f 696e 745f 696e 6465 7820      point_index 
-000091d0: 3d20 7365 6c66 2e5f 7469 6d65 5f69 6e64  = self._time_ind
-000091e0: 6578 2e67 6574 5f6c 6f63 2870 6f69 6e74  ex.get_loc(point
-000091f0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-00009200: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00009210: 2020 2020 706f 696e 745f 696e 6465 7820      point_index 
-00009220: 3d20 7365 6c66 2e5f 7469 6d65 5f69 6e64  = self._time_ind
-00009230: 6578 2e67 6574 5f6c 6f63 2873 656c 662e  ex.get_loc(self.
-00009240: 5f67 6574 5f66 6972 7374 5f74 696d 6573  _get_first_times
-00009250: 7461 6d70 5f61 6674 6572 2870 6f69 6e74  tamp_after(point
-00009260: 2920 6966 2061 6674 6572 2065 6c73 650a  ) if after else.
-00009270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092a0: 2020 2020 2020 2073 656c 662e 5f67 6574         self._get
-000092b0: 5f6c 6173 745f 7469 6d65 7374 616d 705f  _last_timestamp_
-000092c0: 6265 666f 7265 2870 6f69 6e74 2929 0a20  before(point)). 
-000092d0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000092e0: 2020 2020 2020 2020 2072 6169 7365 5f6c           raise_l
-000092f0: 6f67 2854 7970 6545 7272 6f72 2822 6070  og(TypeError("`p
-00009300: 6f69 6e74 6020 6e65 6564 7320 746f 2062  oint` needs to b
-00009310: 6520 6569 7468 6572 2060 666c 6f61 7460  e either `float`
-00009320: 2c20 6069 6e74 6020 6f72 2060 7064 2e54  , `int` or `pd.T
-00009330: 696d 6573 7461 6d70 6022 292c 206c 6f67  imestamp`"), log
-00009340: 6765 7229 0a20 2020 2020 2020 2072 6574  ger).        ret
-00009350: 7572 6e20 706f 696e 745f 696e 6465 780a  urn point_index.
-00009360: 0a20 2020 2064 6566 2067 6574 5f74 696d  .    def get_tim
-00009370: 6573 7461 6d70 5f61 745f 706f 696e 7428  estamp_at_point(
-00009380: 7365 6c66 2c20 706f 696e 743a 2055 6e69  self, point: Uni
-00009390: 6f6e 5b70 642e 5469 6d65 7374 616d 702c  on[pd.Timestamp,
-000093a0: 2066 6c6f 6174 2c20 696e 745d 2920 2d3e   float, int]) ->
-000093b0: 2070 642e 5469 6d65 7374 616d 703a 0a20   pd.Timestamp:. 
-000093c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000093d0: 2020 2043 6f6e 7665 7274 7320 6120 706f     Converts a po
-000093e0: 696e 7420 696e 746f 2061 2070 616e 6461  int into a panda
-000093f0: 732e 5469 6d65 7374 616d 7020 696e 2074  s.Timestamp in t
-00009400: 6865 2074 696d 6520 7365 7269 6573 0a0a  he time series..
-00009410: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00009420: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-00009430: 2d2d 2d2d 2d0a 2020 2020 2020 2020 706f  -----.        po
-00009440: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
-00009450: 5468 6973 2070 6172 616d 6574 6572 2073  This parameter s
-00009460: 7570 706f 7274 7320 3320 6469 6666 6572  upports 3 differ
-00009470: 656e 7420 6461 7461 2074 7970 6573 3a20  ent data types: 
-00009480: 6066 6c6f 6174 602c 2060 696e 7460 2061  `float`, `int` a
-00009490: 6e64 2060 7061 6e64 6173 2e54 696d 6573  nd `pandas.Times
-000094a0: 7461 6d70 602e 0a20 2020 2020 2020 2020  tamp`..         
-000094b0: 2020 2049 6e20 6361 7365 206f 6620 6120     In case of a 
-000094c0: 6066 6c6f 6174 602c 2074 6865 2070 6172  `float`, the par
-000094d0: 616d 6574 6572 2077 696c 6c20 6265 2074  ameter will be t
-000094e0: 7265 6174 6564 2061 7320 7468 6520 7072  reated as the pr
-000094f0: 6f70 6f72 7469 6f6e 206f 6620 7468 6520  oportion of the 
-00009500: 7469 6d65 2073 6572 6965 730a 2020 2020  time series.    
-00009510: 2020 2020 2020 2020 7468 6174 2073 686f          that sho
-00009520: 756c 6420 6c69 6520 6265 666f 7265 2074  uld lie before t
-00009530: 6865 2070 6f69 6e74 2e0a 2020 2020 2020  he point..      
-00009540: 2020 2020 2020 496e 2074 6865 2063 6173        In the cas
-00009550: 6520 6f66 2060 696e 7460 2c20 7468 6520  e of `int`, the 
-00009560: 7061 7261 6d65 7465 7220 7769 6c6c 2062  parameter will b
-00009570: 6520 7472 6561 7465 6420 6173 2061 6e20  e treated as an 
-00009580: 696e 7465 6765 7220 696e 6465 7820 746f  integer index to
-00009590: 2074 6865 2074 696d 6520 696e 6465 7820   the time index 
-000095a0: 6f66 0a20 2020 2020 2020 2020 2020 2060  of.            `
-000095b0: 7365 7269 6573 602e 2057 696c 6c20 7261  series`. Will ra
-000095c0: 6973 6520 6120 5661 6c75 6545 7272 6f72  ise a ValueError
-000095d0: 2069 6620 6e6f 7420 6120 7661 6c69 6420   if not a valid 
-000095e0: 696e 6465 7820 696e 2060 7365 7269 6573  index in `series
-000095f0: 600a 2020 2020 2020 2020 2020 2020 496e  `.            In
-00009600: 2063 6173 6520 6f66 2061 2060 7061 6e64   case of a `pand
-00009610: 6173 2e54 696d 6573 7461 6d70 602c 2070  as.Timestamp`, p
-00009620: 6f69 6e74 2077 696c 6c20 6265 2072 6574  oint will be ret
-00009630: 7572 6e65 6420 6173 2069 7320 7072 6f76  urned as is prov
-00009640: 6964 6564 2074 6861 7420 7468 6520 7469  ided that the ti
-00009650: 6d65 7374 616d 700a 2020 2020 2020 2020  mestamp.        
-00009660: 2020 2020 6973 2070 7265 7365 6e74 2069      is present i
-00009670: 6e20 7468 6520 7365 7269 6573 2074 696d  n the series tim
-00009680: 6520 696e 6465 782c 206f 7468 6572 7769  e index, otherwi
-00009690: 7365 2077 696c 6c20 7261 6973 6520 6120  se will raise a 
-000096a0: 5661 6c75 6545 7272 6f72 2e0a 2020 2020  ValueError..    
-000096b0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000096c0: 7261 6973 655f 6966 5f6e 6f74 2873 656c  raise_if_not(sel
-000096d0: 662e 5f68 6173 5f64 6174 6574 696d 655f  f._has_datetime_
-000096e0: 696e 6465 782c 2027 4361 6c6c 6564 2067  index, 'Called g
-000096f0: 6574 5f74 696d 6573 7461 6d70 5f61 745f  et_timestamp_at_
-00009700: 706f 696e 7428 2920 6275 7420 7468 6973  point() but this
-00009710: 2073 6572 6965 7320 270a 2020 2020 2020   series '.      
-00009720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009740: 2020 2020 2020 2020 2027 6973 206e 6f74           'is not
-00009750: 2069 6e64 6578 6564 2077 6974 6820 6120   indexed with a 
-00009760: 4461 7465 7469 6d65 496e 6465 782e 272c  DatetimeIndex.',
-00009770: 206c 6f67 6765 7229 0a20 2020 2020 2020   logger).       
-00009780: 2069 6478 203d 2073 656c 662e 6765 745f   idx = self.get_
-00009790: 696e 6465 785f 6174 5f70 6f69 6e74 2870  index_at_point(p
-000097a0: 6f69 6e74 290a 2020 2020 2020 2020 7265  oint).        re
-000097b0: 7475 726e 2073 656c 662e 5f74 696d 655f  turn self._time_
-000097c0: 696e 6465 785b 6964 785d 0a0a 2020 2020  index[idx]..    
-000097d0: 6465 6620 5f73 706c 6974 5f61 7428 7365  def _split_at(se
-000097e0: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-000097f0: 2020 2020 2020 7370 6c69 745f 706f 696e        split_poin
-00009800: 743a 2055 6e69 6f6e 5b70 642e 5469 6d65  t: Union[pd.Time
-00009810: 7374 616d 702c 2066 6c6f 6174 2c20 696e  stamp, float, in
-00009820: 745d 2c0a 2020 2020 2020 2020 2020 2020  t],.            
-00009830: 2020 2020 2020 6166 7465 723a 2062 6f6f        after: boo
-00009840: 6c20 3d20 5472 7565 2920 2d3e 2054 7570  l = True) -> Tup
-00009850: 6c65 5b27 5469 6d65 5365 7269 6573 272c  le['TimeSeries',
-00009860: 2027 5469 6d65 5365 7269 6573 275d 3a0a   'TimeSeries']:.
-00009870: 0a20 2020 2020 2020 2070 6f69 6e74 5f69  .        point_i
-00009880: 6e64 6578 203d 2073 656c 662e 6765 745f  ndex = self.get_
-00009890: 696e 6465 785f 6174 5f70 6f69 6e74 2873  index_at_point(s
-000098a0: 706c 6974 5f70 6f69 6e74 2c20 6166 7465  plit_point, afte
-000098b0: 7229 0a20 2020 2020 2020 2072 6574 7572  r).        retur
-000098c0: 6e20 7365 6c66 5b3a 706f 696e 745f 696e  n self[:point_in
-000098d0: 6465 782b 2831 2069 6620 6166 7465 7220  dex+(1 if after 
-000098e0: 656c 7365 2030 295d 2c20 7365 6c66 5b70  else 0)], self[p
-000098f0: 6f69 6e74 5f69 6e64 6578 2b28 3120 6966  oint_index+(1 if
-00009900: 2061 6674 6572 2065 6c73 6520 3029 3a5d   after else 0):]
-00009910: 0a0a 2020 2020 6465 6620 7370 6c69 745f  ..    def split_
-00009920: 6166 7465 7228 7365 6c66 2c20 7370 6c69  after(self, spli
-00009930: 745f 706f 696e 743a 2055 6e69 6f6e 5b70  t_point: Union[p
-00009940: 642e 5469 6d65 7374 616d 702c 2066 6c6f  d.Timestamp, flo
-00009950: 6174 2c20 696e 745d 2920 2d3e 2054 7570  at, int]) -> Tup
-00009960: 6c65 5b27 5469 6d65 5365 7269 6573 272c  le['TimeSeries',
-00009970: 2027 5469 6d65 5365 7269 6573 275d 3a0a   'TimeSeries']:.
-00009980: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00009990: 2020 2020 5370 6c69 7473 2074 6865 2054      Splits the T
-000099a0: 696d 6553 6572 6965 7320 696e 2074 776f  imeSeries in two
-000099b0: 2c20 6166 7465 7220 6120 7072 6f76 6964  , after a provid
-000099c0: 6564 2060 7370 6c69 745f 706f 696e 7460  ed `split_point`
-000099d0: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-000099e0: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-000099f0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-00009a00: 2073 706c 6974 5f70 6f69 6e74 0a20 2020   split_point.   
-00009a10: 2020 2020 2020 2020 2041 2074 696d 6573           A times
-00009a20: 7461 6d70 2c20 666c 6f61 7420 6f72 2069  tamp, float or i
-00009a30: 6e74 6567 6572 2e20 4966 2066 6c6f 6174  nteger. If float
-00009a40: 2c20 7265 7072 6573 656e 7473 2074 6865  , represents the
-00009a50: 2070 726f 706f 7274 696f 6e20 6f66 2074   proportion of t
-00009a60: 6865 2073 6572 6965 7320 746f 2069 6e63  he series to inc
-00009a70: 6c75 6465 2069 6e20 7468 650a 2020 2020  lude in the.    
-00009a80: 2020 2020 2020 2020 6669 7273 7420 5469          first Ti
-00009a90: 6d65 5365 7269 6573 2028 6d75 7374 2062  meSeries (must b
-00009aa0: 6520 6265 7477 6565 6e20 302e 3020 616e  e between 0.0 an
-00009ab0: 6420 312e 3029 2e20 4966 2069 6e74 6567  d 1.0). If integ
-00009ac0: 6572 2c20 7265 7072 6573 656e 7473 2074  er, represents t
-00009ad0: 6865 2069 6e64 6578 2070 6f73 6974 696f  he index positio
-00009ae0: 6e20 6166 7465 720a 2020 2020 2020 2020  n after.        
-00009af0: 2020 2020 7768 6963 6820 7468 6520 7370      which the sp
-00009b00: 6c69 7420 6973 2070 6572 666f 726d 6564  lit is performed
-00009b10: 2e20 4120 7064 2e54 696d 6573 7461 6d70  . A pd.Timestamp
-00009b20: 2063 616e 2062 6520 7072 6f76 6964 6564   can be provided
-00009b30: 2066 6f72 2054 696d 6553 6572 6965 7320   for TimeSeries 
-00009b40: 7468 6174 2061 7265 2069 6e64 6578 6564  that are indexed
-00009b50: 2062 7920 610a 2020 2020 2020 2020 2020   by a.          
-00009b60: 2020 7064 2e44 6174 6574 696d 6549 6e64    pd.DatetimeInd
-00009b70: 6578 2e20 496e 2073 7563 6820 6361 7365  ex. In such case
-00009b80: 732c 2074 6865 2074 696d 6573 7461 6d70  s, the timestamp
-00009b90: 2077 696c 6c20 6265 2063 6f6e 7461 696e   will be contain
-00009ba0: 6564 2069 6e20 7468 6520 6669 7273 7420  ed in the first 
-00009bb0: 5469 6d65 5365 7269 6573 2c20 6275 7420  TimeSeries, but 
-00009bc0: 6e6f 740a 2020 2020 2020 2020 2020 2020  not.            
-00009bd0: 696e 2074 6865 2073 6563 6f6e 6420 6f6e  in the second on
-00009be0: 652e 2054 6865 2074 696d 6573 7461 6d70  e. The timestamp
-00009bf0: 2069 7473 656c 6620 646f 6573 206e 6f74   itself does not
-00009c00: 2068 6176 6520 746f 2061 7070 6561 7220   have to appear 
-00009c10: 696e 2074 6865 206f 7269 6769 6e61 6c20  in the original 
-00009c20: 5469 6d65 5365 7269 6573 2069 6e64 6578  TimeSeries index
-00009c30: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00009c40: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
-00009c50: 2d2d 0a20 2020 2020 2020 2054 7570 6c65  --.        Tuple
-00009c60: 5b54 696d 6553 6572 6965 732c 2054 696d  [TimeSeries, Tim
-00009c70: 6553 6572 6965 735d 0a20 2020 2020 2020  eSeries].       
-00009c80: 2020 2020 2041 2074 7570 6c65 206f 6620       A tuple of 
-00009c90: 7477 6f20 7469 6d65 2073 6572 6965 732e  two time series.
-00009ca0: 2054 6865 2066 6972 7374 2074 696d 6520   The first time 
-00009cb0: 7365 7269 6573 2063 6f6e 7461 696e 7320  series contains 
-00009cc0: 7468 6520 6669 7273 7420 7361 6d70 6c65  the first sample
-00009cd0: 7320 7570 2074 6f20 7468 6520 6073 706c  s up to the `spl
-00009ce0: 6974 5f70 6f69 6e74 602c 0a20 2020 2020  it_point`,.     
-00009cf0: 2020 2020 2020 2061 6e64 2074 6865 2073         and the s
-00009d00: 6563 6f6e 6420 636f 6e74 6169 6e73 2074  econd contains t
-00009d10: 6865 2072 656d 6169 6e69 6e67 206f 6e65  he remaining one
-00009d20: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-00009d30: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00009d40: 6c66 2e5f 7370 6c69 745f 6174 2873 706c  lf._split_at(spl
-00009d50: 6974 5f70 6f69 6e74 2c20 6166 7465 723d  it_point, after=
-00009d60: 5472 7565 290a 0a20 2020 2064 6566 2073  True)..    def s
-00009d70: 706c 6974 5f62 6566 6f72 6528 7365 6c66  plit_before(self
-00009d80: 2c20 7370 6c69 745f 706f 696e 743a 2055  , split_point: U
-00009d90: 6e69 6f6e 5b70 642e 5469 6d65 7374 616d  nion[pd.Timestam
-00009da0: 702c 2066 6c6f 6174 2c20 696e 745d 2920  p, float, int]) 
-00009db0: 2d3e 2054 7570 6c65 5b27 5469 6d65 5365  -> Tuple['TimeSe
-00009dc0: 7269 6573 272c 2027 5469 6d65 5365 7269  ries', 'TimeSeri
-00009dd0: 6573 275d 3a0a 2020 2020 2020 2020 2222  es']:.        ""
-00009de0: 220a 2020 2020 2020 2020 5370 6c69 7473  ".        Splits
-00009df0: 2074 6865 2054 696d 6553 6572 6965 7320   the TimeSeries 
-00009e00: 696e 2074 776f 2c20 6265 666f 7265 2061  in two, before a
-00009e10: 2070 726f 7669 6465 6420 6073 706c 6974   provided `split
-00009e20: 5f70 6f69 6e74 602e 0a0a 2020 2020 2020  _point`...      
-00009e30: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00009e40: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
-00009e50: 2020 2020 2020 2020 7370 6c69 745f 706f          split_po
-00009e60: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
-00009e70: 4120 7469 6d65 7374 616d 702c 2066 6c6f  A timestamp, flo
-00009e80: 6174 206f 7220 696e 7465 6765 722e 2049  at or integer. I
-00009e90: 6620 666c 6f61 742c 2072 6570 7265 7365  f float, represe
-00009ea0: 6e74 7320 7468 6520 7072 6f70 6f72 7469  nts the proporti
-00009eb0: 6f6e 206f 6620 7468 6520 7365 7269 6573  on of the series
-00009ec0: 2074 6f20 696e 636c 7564 6520 696e 2074   to include in t
-00009ed0: 6865 0a20 2020 2020 2020 2020 2020 2066  he.            f
-00009ee0: 6972 7374 2054 696d 6553 6572 6965 7320  irst TimeSeries 
-00009ef0: 286d 7573 7420 6265 2062 6574 7765 656e  (must be between
-00009f00: 2030 2e30 2061 6e64 2031 2e30 292e 2049   0.0 and 1.0). I
-00009f10: 6620 696e 7465 6765 722c 2072 6570 7265  f integer, repre
-00009f20: 7365 6e74 7320 7468 6520 696e 6465 7820  sents the index 
-00009f30: 706f 7369 7469 6f6e 2062 6566 6f72 650a  position before.
-00009f40: 2020 2020 2020 2020 2020 2020 7768 6963              whic
-00009f50: 6820 7468 6520 7370 6c69 7420 6973 2070  h the split is p
-00009f60: 6572 666f 726d 6564 2e20 4120 7064 2e54  erformed. A pd.T
-00009f70: 696d 6573 7461 6d70 2063 616e 2062 6520  imestamp can be 
-00009f80: 7072 6f76 6964 6564 2066 6f72 2054 696d  provided for Tim
-00009f90: 6553 6572 6965 7320 7468 6174 2061 7265  eSeries that are
-00009fa0: 2069 6e64 6578 6564 2062 7920 610a 2020   indexed by a.  
-00009fb0: 2020 2020 2020 2020 2020 7064 2e44 6174            pd.Dat
-00009fc0: 6574 696d 6549 6e64 6578 2e20 496e 2073  etimeIndex. In s
-00009fd0: 7563 6820 6361 7365 732c 2074 6865 2074  uch cases, the t
-00009fe0: 696d 6573 7461 6d70 2077 696c 6c20 6265  imestamp will be
-00009ff0: 2063 6f6e 7461 696e 6564 2069 6e20 7468   contained in th
-0000a000: 6520 7365 636f 6e64 2054 696d 6553 6572  e second TimeSer
-0000a010: 6965 732c 2062 7574 206e 6f74 0a20 2020  ies, but not.   
-0000a020: 2020 2020 2020 2020 2069 6e20 7468 6520           in the 
-0000a030: 6669 7273 7420 6f6e 652e 2054 6865 2074  first one. The t
-0000a040: 696d 6573 7461 6d70 2069 7473 656c 6620  imestamp itself 
-0000a050: 646f 6573 206e 6f74 2068 6176 6520 746f  does not have to
-0000a060: 2061 7070 6561 7220 696e 2074 6865 206f   appear in the o
-0000a070: 7269 6769 6e61 6c20 5469 6d65 5365 7269  riginal TimeSeri
-0000a080: 6573 2069 6e64 6578 2e0a 0a20 2020 2020  es index...     
-0000a090: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-0000a0a0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-0000a0b0: 2020 2054 7570 6c65 5b54 696d 6553 6572     Tuple[TimeSer
-0000a0c0: 6965 732c 2054 696d 6553 6572 6965 735d  ies, TimeSeries]
-0000a0d0: 0a20 2020 2020 2020 2020 2020 2041 2074  .            A t
-0000a0e0: 7570 6c65 206f 6620 7477 6f20 7469 6d65  uple of two time
-0000a0f0: 2073 6572 6965 732e 2054 6865 2066 6972   series. The fir
-0000a100: 7374 2074 696d 6520 7365 7269 6573 2063  st time series c
-0000a110: 6f6e 7461 696e 7320 7468 6520 6669 7273  ontains the firs
-0000a120: 7420 7361 6d70 6c65 7320 7570 2074 6f20  t samples up to 
-0000a130: 7468 6520 6073 706c 6974 5f70 6f69 6e74  the `split_point
-0000a140: 602c 0a20 2020 2020 2020 2020 2020 2061  `,.            a
-0000a150: 6e64 2074 6865 2073 6563 6f6e 6420 636f  nd the second co
-0000a160: 6e74 6169 6e73 2074 6865 2072 656d 6169  ntains the remai
-0000a170: 6e69 6e67 206f 6e65 732e 0a20 2020 2020  ning ones..     
-0000a180: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-0000a190: 6574 7572 6e20 7365 6c66 2e5f 7370 6c69  eturn self._spli
-0000a1a0: 745f 6174 2873 706c 6974 5f70 6f69 6e74  t_at(split_point
-0000a1b0: 2c20 6166 7465 723d 4661 6c73 6529 0a0a  , after=False)..
-0000a1c0: 2020 2020 6465 6620 6472 6f70 5f61 6674      def drop_aft
-0000a1d0: 6572 2873 656c 662c 2073 706c 6974 5f70  er(self, split_p
-0000a1e0: 6f69 6e74 3a20 556e 696f 6e5b 7064 2e54  oint: Union[pd.T
-0000a1f0: 696d 6573 7461 6d70 2c20 666c 6f61 742c  imestamp, float,
-0000a200: 2069 6e74 5d29 3a0a 2020 2020 2020 2020   int]):.        
-0000a210: 2222 220a 2020 2020 2020 2020 4472 6f70  """.        Drop
-0000a220: 7320 6576 6572 7974 6869 6e67 2061 6674  s everything aft
-0000a230: 6572 2074 6865 2070 726f 7669 6465 6420  er the provided 
-0000a240: 7469 6d65 7374 616d 7020 6074 7360 2c20  timestamp `ts`, 
-0000a250: 696e 636c 7564 6564 2e0a 2020 2020 2020  included..      
-0000a260: 2020 5468 6520 7469 6d65 7374 616d 7020    The timestamp 
-0000a270: 6d61 7920 6e6f 7420 6265 2069 6e20 7468  may not be in th
-0000a280: 6520 5469 6d65 5365 7269 6573 2e20 4966  e TimeSeries. If
-0000a290: 2069 7420 6973 2c20 7468 6520 7469 6d65   it is, the time
-0000a2a0: 7374 616d 7020 7769 6c6c 2062 6520 6472  stamp will be dr
-0000a2b0: 6f70 7065 642e 0a0a 2020 2020 2020 2020  opped...        
-0000a2c0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-0000a2d0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-0000a2e0: 2020 2020 2020 7370 6c69 745f 706f 696e        split_poin
-0000a2f0: 740a 2020 2020 2020 2020 2020 2020 5468  t.            Th
-0000a300: 6520 7469 6d65 7374 616d 7020 7468 6174  e timestamp that
-0000a310: 2069 6e64 6963 6174 6573 2063 7574 2d6f   indicates cut-o
-0000a320: 6666 2074 696d 652e 0a0a 2020 2020 2020  ff time...      
-0000a330: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-0000a340: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-0000a350: 2020 5469 6d65 5365 7269 6573 0a20 2020    TimeSeries.   
-0000a360: 2020 2020 2020 2020 2041 206e 6577 2054           A new T
-0000a370: 696d 6553 6572 6965 732c 2061 6674 6572  imeSeries, after
-0000a380: 2060 7473 602e 0a20 2020 2020 2020 2022   `ts`..        "
-0000a390: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-0000a3a0: 6e20 7365 6c66 2e73 706c 6974 5f62 6566  n self.split_bef
-0000a3b0: 6f72 6528 7370 6c69 745f 706f 696e 7429  ore(split_point)
-0000a3c0: 5b30 5d0a 0a20 2020 2064 6566 2064 726f  [0]..    def dro
-0000a3d0: 705f 6265 666f 7265 2873 656c 662c 2073  p_before(self, s
-0000a3e0: 706c 6974 5f70 6f69 6e74 3a20 556e 696f  plit_point: Unio
-0000a3f0: 6e5b 7064 2e54 696d 6573 7461 6d70 2c20  n[pd.Timestamp, 
-0000a400: 666c 6f61 742c 2069 6e74 5d29 3a0a 2020  float, int]):.  
-0000a410: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000a420: 2020 4472 6f70 7320 6576 6572 7974 6869    Drops everythi
-0000a430: 6e67 2062 6566 6f72 6520 7468 6520 7072  ng before the pr
-0000a440: 6f76 6964 6564 2074 696d 6573 7461 6d70  ovided timestamp
-0000a450: 2060 7473 602c 2069 6e63 6c75 6465 642e   `ts`, included.
-0000a460: 0a20 2020 2020 2020 2054 6865 2074 696d  .        The tim
-0000a470: 6573 7461 6d70 206d 6179 206e 6f74 2062  estamp may not b
-0000a480: 6520 696e 2074 6865 2054 696d 6553 6572  e in the TimeSer
-0000a490: 6965 732e 2049 6620 6974 2069 732c 2074  ies. If it is, t
-0000a4a0: 6865 2074 696d 6573 7461 6d70 2077 696c  he timestamp wil
-0000a4b0: 6c20 6265 2064 726f 7070 6564 2e0a 0a20  l be dropped... 
-0000a4c0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-0000a4d0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-0000a4e0: 2d2d 2d2d 0a20 2020 2020 2020 2073 706c  ----.        spl
-0000a4f0: 6974 5f70 6f69 6e74 0a20 2020 2020 2020  it_point.       
-0000a500: 2020 2020 2054 6865 2074 696d 6573 7461       The timesta
-0000a510: 6d70 2074 6861 7420 696e 6469 6361 7465  mp that indicate
-0000a520: 7320 6375 742d 6f66 6620 7469 6d65 2e0a  s cut-off time..
-0000a530: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-0000a540: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-0000a550: 0a20 2020 2020 2020 2054 696d 6553 6572  .        TimeSer
-0000a560: 6965 730a 2020 2020 2020 2020 2020 2020  ies.            
-0000a570: 4120 6e65 7720 5469 6d65 5365 7269 6573  A new TimeSeries
-0000a580: 2c20 6166 7465 7220 6074 7360 2e0a 2020  , after `ts`..  
-0000a590: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000a5a0: 2020 7265 7475 726e 2073 656c 662e 7370    return self.sp
-0000a5b0: 6c69 745f 6166 7465 7228 7370 6c69 745f  lit_after(split_
-0000a5c0: 706f 696e 7429 5b31 5d0a 0a20 2020 2064  point)[1]..    d
-0000a5d0: 6566 2073 6c69 6365 2873 656c 662c 2073  ef slice(self, s
-0000a5e0: 7461 7274 5f74 733a 2055 6e69 6f6e 5b70  tart_ts: Union[p
-0000a5f0: 642e 5469 6d65 7374 616d 702c 2069 6e74  d.Timestamp, int
-0000a600: 5d2c 2065 6e64 5f74 733a 2055 6e69 6f6e  ], end_ts: Union
-0000a610: 5b70 642e 5469 6d65 7374 616d 702c 2069  [pd.Timestamp, i
-0000a620: 6e74 5d29 3a0a 2020 2020 2020 2020 2222  nt]):.        ""
-0000a630: 220a 2020 2020 2020 2020 5265 7475 726e  ".        Return
-0000a640: 7320 6120 6e65 7720 5469 6d65 5365 7269  s a new TimeSeri
-0000a650: 6573 2c20 7374 6172 7469 6e67 206c 6174  es, starting lat
-0000a660: 6572 2074 6861 6e20 6073 7461 7274 5f74  er than `start_t
-0000a670: 7360 2061 6e64 2065 6e64 696e 6720 6265  s` and ending be
-0000a680: 666f 7265 2060 656e 645f 7473 602c 2069  fore `end_ts`, i
-0000a690: 6e63 6c75 7369 7665 206f 6e20 626f 7468  nclusive on both
-0000a6a0: 2065 6e64 732e 0a20 2020 2020 2020 2054   ends..        T
-0000a6b0: 6865 2074 696d 6573 7461 6d70 7320 646f  he timestamps do
-0000a6c0: 6e27 7420 6861 7665 2074 6f20 6265 2069  n't have to be i
-0000a6d0: 6e20 7468 6520 7365 7269 6573 2e0a 0a20  n the series... 
-0000a6e0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-0000a6f0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-0000a700: 2d2d 2d2d 0a20 2020 2020 2020 2073 7461  ----.        sta
-0000a710: 7274 5f74 730a 2020 2020 2020 2020 2020  rt_ts.          
-0000a720: 2020 5468 6520 7469 6d65 7374 616d 7020    The timestamp 
-0000a730: 7468 6174 2069 6e64 6963 6174 6573 2074  that indicates t
-0000a740: 6865 206c 6566 7420 6375 742d 6f66 662e  he left cut-off.
-0000a750: 0a20 2020 2020 2020 2065 6e64 5f74 730a  .        end_ts.
-0000a760: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-0000a770: 7469 6d65 7374 616d 7020 7468 6174 2069  timestamp that i
-0000a780: 6e64 6963 6174 6573 2074 6865 2072 6967  ndicates the rig
-0000a790: 6874 2063 7574 2d6f 6666 2e0a 0a20 2020  ht cut-off...   
-0000a7a0: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-0000a7b0: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-0000a7c0: 2020 2020 2054 696d 6553 6572 6965 730a       TimeSeries.
-0000a7d0: 2020 2020 2020 2020 2020 2020 4120 6e65              A ne
-0000a7e0: 7720 7365 7269 6573 2c20 7769 7468 2069  w series, with i
-0000a7f0: 6e64 6963 6573 2067 7265 6174 6572 206f  ndices greater o
-0000a800: 7220 6571 7561 6c20 7468 616e 2060 7374  r equal than `st
-0000a810: 6172 745f 7473 6020 616e 6420 736d 616c  art_ts` and smal
-0000a820: 6c65 7220 6f72 2065 7175 616c 2074 6861  ler or equal tha
-0000a830: 6e20 6065 6e64 5f74 7360 2e0a 2020 2020  n `end_ts`..    
-0000a840: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000a850: 7261 6973 655f 6966 5f6e 6f74 2874 7970  raise_if_not(typ
-0000a860: 6528 7374 6172 745f 7473 2920 3d3d 2074  e(start_ts) == t
-0000a870: 7970 6528 656e 645f 7473 292c 2027 5468  ype(end_ts), 'Th
-0000a880: 6520 7477 6f20 7469 6d65 7374 616d 7073  e two timestamps
-0000a890: 2070 726f 7669 6465 6420 746f 2073 6c69   provided to sli
-0000a8a0: 6365 2829 2068 6176 6520 746f 2062 6520  ce() have to be 
-0000a8b0: 6f66 2074 6865 2027 0a20 2020 2020 2020  of the '.       
-0000a8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8e0: 2020 2020 2020 2020 2020 2020 2020 2773                's
-0000a8f0: 616d 6520 7479 7065 2e27 2c20 6c6f 6767  ame type.', logg
-0000a900: 6572 290a 2020 2020 2020 2020 6966 2069  er).        if i
-0000a910: 7369 6e73 7461 6e63 6528 7374 6172 745f  sinstance(start_
-0000a920: 7473 2c20 7064 2e54 696d 6573 7461 6d70  ts, pd.Timestamp
-0000a930: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-0000a940: 6169 7365 5f69 665f 6e6f 7428 7365 6c66  aise_if_not(self
-0000a950: 2e5f 6861 735f 6461 7465 7469 6d65 5f69  ._has_datetime_i
-0000a960: 6e64 6578 2c20 2754 696d 6573 7461 6d70  ndex, 'Timestamp
-0000a970: 7320 6861 7665 2062 6565 6e20 7072 6f76  s have been prov
-0000a980: 6964 6564 2074 6f20 736c 6963 6528 292c  ided to slice(),
-0000a990: 2062 7574 2074 6865 2073 6572 6965 7320   but the series 
-0000a9a0: 6973 2027 0a20 2020 2020 2020 2020 2020  is '.           
-0000a9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a9d0: 2020 2020 2020 2020 2769 6e64 6578 6564          'indexed
-0000a9e0: 2075 7369 6e67 2061 6e20 696e 7465 6765   using an intege
-0000a9f0: 722d 6261 7365 6420 5261 6e67 6549 6e64  r-based RangeInd
-0000aa00: 6578 2e27 2c20 6c6f 6767 6572 290a 2020  ex.', logger).  
-0000aa10: 2020 2020 2020 2020 2020 6964 7820 3d20            idx = 
-0000aa20: 7064 2e44 6174 6574 696d 6549 6e64 6578  pd.DatetimeIndex
-0000aa30: 2866 696c 7465 7228 6c61 6d62 6461 2074  (filter(lambda t
-0000aa40: 3a20 7374 6172 745f 7473 203c 3d20 7420  : start_ts <= t 
-0000aa50: 3c3d 2065 6e64 5f74 732c 2073 656c 662e  <= end_ts, self.
-0000aa60: 5f74 696d 655f 696e 6465 7829 290a 2020  _time_index)).  
-0000aa70: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000aa80: 2020 2020 2020 2020 7261 6973 655f 6966          raise_if
-0000aa90: 2873 656c 662e 5f68 6173 5f64 6174 6574  (self._has_datet
-0000aaa0: 696d 655f 696e 6465 782c 2027 7374 6172  ime_index, 'star
-0000aab0: 7420 616e 6420 656e 6420 7469 6d65 7320  t and end times 
-0000aac0: 6861 7665 2062 6565 6e20 7072 6f76 6964  have been provid
-0000aad0: 6564 2061 7320 696e 7465 6765 7273 2074  ed as integers t
-0000aae0: 6f20 736c 6963 6528 292c 2062 7574 2027  o slice(), but '
-0000aaf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ab00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab20: 2774 6865 2073 6572 6965 7320 6973 2069  'the series is i
-0000ab30: 6e64 6578 6564 2077 6974 6820 6120 4461  ndexed with a Da
-0000ab40: 7465 7469 6d65 496e 6465 782e 272c 206c  tetimeIndex.', l
-0000ab50: 6f67 6765 7229 0a20 2020 2020 2020 2020  ogger).         
-0000ab60: 2020 2069 6478 203d 2070 642e 5261 6e67     idx = pd.Rang
-0000ab70: 6549 6e64 6578 2873 7461 7274 5f74 732c  eIndex(start_ts,
-0000ab80: 2065 6e64 5f74 732c 2073 7465 703d 3129   end_ts, step=1)
-0000ab90: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000aba0: 7365 6c66 5b69 6478 5d0a 0a20 2020 2064  self[idx]..    d
-0000abb0: 6566 2073 6c69 6365 5f6e 5f70 6f69 6e74  ef slice_n_point
-0000abc0: 735f 6166 7465 7228 7365 6c66 2c20 7374  s_after(self, st
-0000abd0: 6172 745f 7473 3a20 556e 696f 6e5b 7064  art_ts: Union[pd
-0000abe0: 2e54 696d 6573 7461 6d70 2c20 696e 745d  .Timestamp, int]
-0000abf0: 2c20 6e3a 2069 6e74 2920 2d3e 2027 5469  , n: int) -> 'Ti
-0000ac00: 6d65 5365 7269 6573 273a 0a20 2020 2020  meSeries':.     
-0000ac10: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-0000ac20: 6574 7572 6e73 2061 206e 6577 2054 696d  eturns a new Tim
-0000ac30: 6553 6572 6965 732c 2073 7461 7274 696e  eSeries, startin
-0000ac40: 6720 6120 6073 7461 7274 5f74 7360 2061  g a `start_ts` a
-0000ac50: 6e64 2068 6176 696e 6720 6174 206d 6f73  nd having at mos
-0000ac60: 7420 606e 6020 706f 696e 7473 2e0a 0a20  t `n` points... 
-0000ac70: 2020 2020 2020 2054 6865 2070 726f 7669         The provi
-0000ac80: 6465 6420 7469 6d65 7374 616d 7073 2077  ded timestamps w
-0000ac90: 696c 6c20 6265 2069 6e63 6c75 6465 6420  ill be included 
-0000aca0: 696e 2074 6865 2073 6572 6965 732e 0a0a  in the series...
-0000acb0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-0000acc0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-0000acd0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7374  -----.        st
-0000ace0: 6172 745f 7473 0a20 2020 2020 2020 2020  art_ts.         
-0000acf0: 2020 2054 6865 2074 696d 6573 7461 6d70     The timestamp
-0000ad00: 206f 7220 696e 6465 7820 7468 6174 2069   or index that i
-0000ad10: 6e64 6963 6174 6573 2074 6865 2073 706c  ndicates the spl
-0000ad20: 6974 7469 6e67 2074 696d 652e 0a20 2020  itting time..   
-0000ad30: 2020 2020 206e 0a20 2020 2020 2020 2020       n.         
-0000ad40: 2020 2054 6865 206d 6178 696d 616c 206c     The maximal l
-0000ad50: 656e 6774 6820 6f66 2074 6865 206e 6577  ength of the new
-0000ad60: 2054 696d 6553 6572 6965 732e 0a0a 2020   TimeSeries...  
-0000ad70: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
-0000ad80: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-0000ad90: 2020 2020 2020 5469 6d65 5365 7269 6573        TimeSeries
-0000ada0: 0a20 2020 2020 2020 2020 2020 2041 206e  .            A n
-0000adb0: 6577 2054 696d 6553 6572 6965 732c 2077  ew TimeSeries, w
-0000adc0: 6974 6820 6c65 6e67 7468 2061 7420 6d6f  ith length at mo
-0000add0: 7374 2060 6e60 2c20 7374 6172 7469 6e67  st `n`, starting
-0000ade0: 2061 7420 6073 7461 7274 5f74 7360 0a20   at `start_ts`. 
-0000adf0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000ae00: 2020 2072 6169 7365 5f69 665f 6e6f 7428     raise_if_not(
-0000ae10: 6e20 3e20 302c 2027 6e20 7368 6f75 6c64  n > 0, 'n should
-0000ae20: 2062 6520 6120 706f 7369 7469 7665 2069   be a positive i
-0000ae30: 6e74 6567 6572 2e27 2c20 6c6f 6767 6572  nteger.', logger
-0000ae40: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
-0000ae50: 7261 6973 655f 6966 5f6e 6f74 5f77 6974  raise_if_not_wit
-0000ae60: 6869 6e28 7374 6172 745f 7473 290a 0a20  hin(start_ts).. 
-0000ae70: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-0000ae80: 616e 6365 2873 7461 7274 5f74 732c 2069  ance(start_ts, i
-0000ae90: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
-0000aea0: 2072 6574 7572 6e20 7365 6c66 5b73 7461   return self[sta
-0000aeb0: 7274 5f74 733a 7374 6172 745f 7473 2b6e  rt_ts:start_ts+n
-0000aec0: 5d0a 2020 2020 2020 2020 656c 6966 2069  ].        elif i
-0000aed0: 7369 6e73 7461 6e63 6528 7374 6172 745f  sinstance(start_
-0000aee0: 7473 2c20 7064 2e54 696d 6573 7461 6d70  ts, pd.Timestamp
-0000aef0: 293a 0a20 2020 2020 2020 2020 2020 2023  ):.            #
-0000af00: 2067 6574 2066 6972 7374 2074 696d 6573   get first times
-0000af10: 7461 6d70 2067 7265 6174 6572 206f 7220  tamp greater or 
-0000af20: 6571 7561 6c20 746f 2073 7461 7274 5f74  equal to start_t
-0000af30: 730a 2020 2020 2020 2020 2020 2020 7473  s.            ts
-0000af40: 7320 3d20 7365 6c66 2e5f 6765 745f 6669  s = self._get_fi
-0000af50: 7273 745f 7469 6d65 7374 616d 705f 6166  rst_timestamp_af
-0000af60: 7465 7228 7374 6172 745f 7473 290a 2020  ter(start_ts).  
-0000af70: 2020 2020 2020 2020 2020 706f 696e 745f            point_
-0000af80: 696e 6465 7820 3d20 7365 6c66 2e67 6574  index = self.get
-0000af90: 5f69 6e64 6578 5f61 745f 706f 696e 7428  _index_at_point(
-0000afa0: 7473 7329 0a20 2020 2020 2020 2020 2020  tss).           
-0000afb0: 2072 6574 7572 6e20 7365 6c66 5b70 6f69   return self[poi
-0000afc0: 6e74 5f69 6e64 6578 3a70 6f69 6e74 5f69  nt_index:point_i
-0000afd0: 6e64 6578 202b 206e 5d0a 2020 2020 2020  ndex + n].      
-0000afe0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000aff0: 2020 2020 7261 6973 655f 6c6f 6728 5661      raise_log(Va
-0000b000: 6c75 6545 7272 6f72 2827 7374 6172 745f  lueError('start_
-0000b010: 7473 206d 7573 7420 6265 2061 6e20 696e  ts must be an in
-0000b020: 7420 6f72 2061 2070 616e 6461 7320 5469  t or a pandas Ti
-0000b030: 6d65 7374 616d 702e 2729 2c20 6c6f 6767  mestamp.'), logg
-0000b040: 6572 290a 0a20 2020 2064 6566 2073 6c69  er)..    def sli
-0000b050: 6365 5f6e 5f70 6f69 6e74 735f 6265 666f  ce_n_points_befo
-0000b060: 7265 2873 656c 662c 2065 6e64 5f74 733a  re(self, end_ts:
-0000b070: 2055 6e69 6f6e 5b70 642e 5469 6d65 7374   Union[pd.Timest
-0000b080: 616d 702c 2069 6e74 5d2c 206e 3a20 696e  amp, int], n: in
-0000b090: 7429 202d 3e20 2754 696d 6553 6572 6965  t) -> 'TimeSerie
-0000b0a0: 7327 3a0a 2020 2020 2020 2020 2222 220a  s':.        """.
-0000b0b0: 2020 2020 2020 2020 5265 7475 726e 7320          Returns 
-0000b0c0: 6120 6e65 7720 5469 6d65 5365 7269 6573  a new TimeSeries
-0000b0d0: 2c20 656e 6469 6e67 2061 7420 6073 7461  , ending at `sta
-0000b0e0: 7274 5f74 7360 2061 6e64 2068 6176 696e  rt_ts` and havin
-0000b0f0: 6720 6174 206d 6f73 7420 606e 6020 706f  g at most `n` po
-0000b100: 696e 7473 2e0a 0a20 2020 2020 2020 2054  ints...        T
-0000b110: 6865 2070 726f 7669 6465 6420 7469 6d65  he provided time
-0000b120: 7374 616d 7073 2077 696c 6c20 6265 2069  stamps will be i
-0000b130: 6e63 6c75 6465 6420 696e 2074 6865 2073  ncluded in the s
-0000b140: 6572 6965 732e 0a0a 2020 2020 2020 2020  eries...        
-0000b150: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-0000b160: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-0000b170: 2020 2020 2020 656e 645f 7473 0a20 2020        end_ts.   
-0000b180: 2020 2020 2020 2020 2054 6865 2074 696d           The tim
-0000b190: 6573 7461 6d70 206f 7220 696e 6465 7820  estamp or index 
-0000b1a0: 7468 6174 2069 6e64 6963 6174 6573 2074  that indicates t
-0000b1b0: 6865 2073 706c 6974 7469 6e67 2074 696d  he splitting tim
-0000b1c0: 652e 0a20 2020 2020 2020 206e 0a20 2020  e..        n.   
-0000b1d0: 2020 2020 2020 2020 2054 6865 206d 6178           The max
-0000b1e0: 696d 616c 206c 656e 6774 6820 6f66 2074  imal length of t
-0000b1f0: 6865 206e 6577 2054 696d 6553 6572 6965  he new TimeSerie
-0000b200: 732e 0a0a 2020 2020 2020 2020 5265 7475  s...        Retu
-0000b210: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-0000b220: 2d2d 2d0a 2020 2020 2020 2020 5469 6d65  ---.        Time
-0000b230: 5365 7269 6573 0a20 2020 2020 2020 2020  Series.         
-0000b240: 2020 2041 206e 6577 2054 696d 6553 6572     A new TimeSer
-0000b250: 6965 732c 2077 6974 6820 6c65 6e67 7468  ies, with length
-0000b260: 2061 7420 6d6f 7374 2060 6e60 2c20 656e   at most `n`, en
-0000b270: 6469 6e67 2061 7420 6073 7461 7274 5f74  ding at `start_t
-0000b280: 7360 0a20 2020 2020 2020 2022 2222 0a0a  s`.        """..
-0000b290: 2020 2020 2020 2020 7261 6973 655f 6966          raise_if
-0000b2a0: 5f6e 6f74 286e 203e 2030 2c20 276e 2073  _not(n > 0, 'n s
-0000b2b0: 686f 756c 6420 6265 2061 2070 6f73 6974  hould be a posit
-0000b2c0: 6976 6520 696e 7465 6765 722e 272c 206c  ive integer.', l
-0000b2d0: 6f67 6765 7229 0a20 2020 2020 2020 2073  ogger).        s
-0000b2e0: 656c 662e 5f72 6169 7365 5f69 665f 6e6f  elf._raise_if_no
-0000b2f0: 745f 7769 7468 696e 2865 6e64 5f74 7329  t_within(end_ts)
-0000b300: 0a0a 2020 2020 2020 2020 6966 2069 7369  ..        if isi
-0000b310: 6e73 7461 6e63 6528 656e 645f 7473 2c20  nstance(end_ts, 
-0000b320: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
-0000b330: 2020 7265 7475 726e 2073 656c 665b 656e    return self[en
-0000b340: 645f 7473 2d6e 2b31 3a65 6e64 5f74 732b  d_ts-n+1:end_ts+
-0000b350: 315d 0a20 2020 2020 2020 2065 6c69 6620  1].        elif 
-0000b360: 6973 696e 7374 616e 6365 2865 6e64 5f74  isinstance(end_t
-0000b370: 732c 2070 642e 5469 6d65 7374 616d 7029  s, pd.Timestamp)
-0000b380: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-0000b390: 6765 7420 6c61 7374 2074 696d 6573 7461  get last timesta
-0000b3a0: 6d70 2073 6d61 6c6c 6572 206f 7220 6571  mp smaller or eq
-0000b3b0: 7561 6c20 746f 2073 7461 7274 5f74 730a  ual to start_ts.
-0000b3c0: 2020 2020 2020 2020 2020 2020 7473 7320              tss 
-0000b3d0: 3d20 7365 6c66 2e5f 6765 745f 6c61 7374  = self._get_last
-0000b3e0: 5f74 696d 6573 7461 6d70 5f62 6566 6f72  _timestamp_befor
-0000b3f0: 6528 656e 645f 7473 290a 2020 2020 2020  e(end_ts).      
-0000b400: 2020 2020 2020 706f 696e 745f 696e 6465        point_inde
-0000b410: 7820 3d20 7365 6c66 2e67 6574 5f69 6e64  x = self.get_ind
-0000b420: 6578 5f61 745f 706f 696e 7428 7473 7329  ex_at_point(tss)
-0000b430: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000b440: 7572 6e20 7365 6c66 5b6d 6178 2830 2c20  urn self[max(0, 
-0000b450: 706f 696e 745f 696e 6465 782d 6e2b 3129  point_index-n+1)
-0000b460: 3a70 6f69 6e74 5f69 6e64 6578 2b31 5d0a  :point_index+1].
-0000b470: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000b480: 2020 2020 2020 2020 2020 7261 6973 655f            raise_
-0000b490: 6c6f 6728 5661 6c75 6545 7272 6f72 2827  log(ValueError('
-0000b4a0: 7374 6172 745f 7473 206d 7573 7420 6265  start_ts must be
-0000b4b0: 2061 6e20 696e 7420 6f72 2061 2070 616e   an int or a pan
-0000b4c0: 6461 7320 5469 6d65 7374 616d 702e 2729  das Timestamp.')
-0000b4d0: 2c20 6c6f 6767 6572 290a 0a20 2020 2064  , logger)..    d
-0000b4e0: 6566 2073 6c69 6365 5f69 6e74 6572 7365  ef slice_interse
-0000b4f0: 6374 2873 656c 662c 206f 7468 6572 3a20  ct(self, other: 
-0000b500: 2754 696d 6553 6572 6965 7327 2920 2d3e  'TimeSeries') ->
-0000b510: 2027 5469 6d65 5365 7269 6573 273a 0a20   'TimeSeries':. 
-0000b520: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000b530: 2020 2052 6574 7572 6e73 2061 2054 696d     Returns a Tim
-0000b540: 6553 6572 6965 7320 736c 6963 6520 6f66  eSeries slice of
-0000b550: 2074 6869 7320 7469 6d65 2073 6572 6965   this time serie
-0000b560: 732c 2077 6865 7265 2074 6865 2074 696d  s, where the tim
-0000b570: 6520 696e 6465 7820 6861 7320 6265 656e  e index has been
-0000b580: 2069 6e74 6572 7365 6374 6564 2077 6974   intersected wit
-0000b590: 6820 7468 6520 6f6e 650a 2020 2020 2020  h the one.      
-0000b5a0: 2020 7072 6f76 6964 6564 2069 6e20 6172    provided in ar
-0000b5b0: 6775 6d65 6e74 2e20 4e6f 7465 2074 6861  gument. Note tha
-0000b5c0: 7420 7468 6973 206d 6574 686f 6420 6973  t this method is
-0000b5d0: 2069 6e20 6765 6e65 7261 6c20 2a6e 6f74   in general *not
-0000b5e0: 2a20 7379 6d6d 6574 7269 632e 0a0a 2020  * symmetric...  
-0000b5f0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-0000b600: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-0000b610: 2d2d 2d0a 2020 2020 2020 2020 6f74 6865  ---.        othe
-0000b620: 720a 2020 2020 2020 2020 2020 2020 7468  r.            th
-0000b630: 6520 6f74 6865 7220 7469 6d65 2073 6572  e other time ser
-0000b640: 6965 730a 0a20 2020 2020 2020 2052 6574  ies..        Ret
-0000b650: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-0000b660: 2d2d 2d2d 0a20 2020 2020 2020 2054 696d  ----.        Tim
-0000b670: 6553 6572 6965 730a 2020 2020 2020 2020  eSeries.        
-0000b680: 2020 2020 6120 6e65 7720 7365 7269 6573      a new series
-0000b690: 2c20 636f 6e74 6169 6e69 6e67 2074 6865  , containing the
-0000b6a0: 2076 616c 7565 7320 6f66 2074 6869 7320   values of this 
-0000b6b0: 7365 7269 6573 2c20 6f76 6572 2074 6865  series, over the
-0000b6c0: 2074 696d 652d 7370 616e 2063 6f6d 6d6f   time-span commo
-0000b6d0: 6e20 746f 2062 6f74 6820 7469 6d65 2073  n to both time s
-0000b6e0: 6572 6965 732e 0a20 2020 2020 2020 2022  eries..        "
-0000b6f0: 2222 0a20 2020 2020 2020 2074 696d 655f  "".        time_
-0000b700: 696e 6465 7820 3d20 7365 6c66 2e74 696d  index = self.tim
-0000b710: 655f 696e 6465 782e 696e 7465 7273 6563  e_index.intersec
-0000b720: 7469 6f6e 286f 7468 6572 2e74 696d 655f  tion(other.time_
-0000b730: 696e 6465 7829 0a20 2020 2020 2020 2072  index).        r
-0000b740: 6574 7572 6e20 7365 6c66 5b74 696d 655f  eturn self[time_
-0000b750: 696e 6465 785d 0a0a 2020 2020 6465 6620  index]..    def 
-0000b760: 7374 7269 7028 7365 6c66 2920 2d3e 2027  strip(self) -> '
-0000b770: 5469 6d65 5365 7269 6573 273a 0a20 2020  TimeSeries':.   
-0000b780: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000b790: 2052 6574 7572 6e73 2061 2054 696d 6553   Returns a TimeS
-0000b7a0: 6572 6965 7320 736c 6963 6520 6f66 2074  eries slice of t
-0000b7b0: 6869 7320 6465 7465 726d 696e 6973 7469  his deterministi
-0000b7c0: 6320 7469 6d65 2073 6572 6965 732c 2077  c time series, w
-0000b7d0: 6865 7265 204e 614e 2d6f 6e6c 7920 656e  here NaN-only en
-0000b7e0: 7472 6965 7320 6174 2074 6865 2062 6567  tries at the beg
-0000b7f0: 696e 6e69 6e67 0a20 2020 2020 2020 2061  inning.        a
-0000b800: 6e64 2074 6865 2065 6e64 206f 6620 7468  nd the end of th
-0000b810: 6520 7365 7269 6573 2061 7265 2072 656d  e series are rem
-0000b820: 6f76 6564 2e20 4e6f 2065 6e74 7269 6573  oved. No entries
-0000b830: 2061 6674 6572 2028 616e 6420 696e 636c   after (and incl
-0000b840: 7564 696e 6729 2074 6865 2066 6972 7374  uding) the first
-0000b850: 206e 6f6e 2d4e 614e 2065 6e74 7279 2061   non-NaN entry a
-0000b860: 6e64 0a20 2020 2020 2020 2062 6566 6f72  nd.        befor
-0000b870: 6520 2861 6e64 2069 6e63 6c75 6469 6e67  e (and including
-0000b880: 2920 7468 6520 6c61 7374 206e 6f6e 2d4e  ) the last non-N
-0000b890: 614e 2065 6e74 7279 2061 7265 2072 656d  aN entry are rem
-0000b8a0: 6f76 6564 2e0a 0a20 2020 2020 2020 2054  oved...        T
-0000b8b0: 6869 7320 6d65 7468 6f64 2069 7320 6f6e  his method is on
-0000b8c0: 6c79 2061 7070 6c69 6361 626c 6520 746f  ly applicable to
-0000b8d0: 2064 6574 6572 6d69 6e69 7374 6963 2073   deterministic s
-0000b8e0: 6572 6965 7320 2869 2e65 2e2c 2068 6176  eries (i.e., hav
-0000b8f0: 696e 6720 3120 7361 6d70 6c65 292e 0a0a  ing 1 sample)...
-0000b900: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-0000b910: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-0000b920: 2020 2020 2020 2020 5469 6d65 5365 7269          TimeSeri
-0000b930: 6573 0a20 2020 2020 2020 2020 2020 2061  es.            a
-0000b940: 206e 6577 2073 6572 6965 7320 6261 7365   new series base
-0000b950: 6420 6f6e 2074 6865 206f 7269 6769 6e61  d on the origina
-0000b960: 6c20 7768 6572 6520 4e61 4e2d 6f6e 6c79  l where NaN-only
-0000b970: 2065 6e74 7269 6573 2061 7420 7374 6172   entries at star
-0000b980: 7420 616e 6420 656e 6420 6861 7665 2062  t and end have b
-0000b990: 6565 6e20 7265 6d6f 7665 640a 2020 2020  een removed.    
-0000b9a0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-0000b9b0: 2064 6620 3d20 7365 6c66 2e70 645f 6461   df = self.pd_da
-0000b9c0: 7461 6672 616d 6528 636f 7079 3d46 616c  taframe(copy=Fal
-0000b9d0: 7365 290a 2020 2020 2020 2020 6e65 775f  se).        new_
-0000b9e0: 7374 6172 745f 6964 7820 3d20 6466 2e66  start_idx = df.f
-0000b9f0: 6972 7374 5f76 616c 6964 5f69 6e64 6578  irst_valid_index
-0000ba00: 2829 0a20 2020 2020 2020 206e 6577 5f65  ().        new_e
-0000ba10: 6e64 5f69 6478 203d 2064 662e 6c61 7374  nd_idx = df.last
-0000ba20: 5f76 616c 6964 5f69 6e64 6578 2829 0a20  _valid_index(). 
-0000ba30: 2020 2020 2020 206e 6577 5f73 6572 6965         new_serie
-0000ba40: 7320 3d20 6466 2e6c 6f63 5b6e 6577 5f73  s = df.loc[new_s
-0000ba50: 7461 7274 5f69 6478 3a6e 6577 5f65 6e64  tart_idx:new_end
-0000ba60: 5f69 6478 5d0a 2020 2020 2020 2020 7265  _idx].        re
-0000ba70: 7475 726e 2054 696d 6553 6572 6965 732e  turn TimeSeries.
-0000ba80: 6672 6f6d 5f64 6174 6166 7261 6d65 286e  from_dataframe(n
-0000ba90: 6577 5f73 6572 6965 7329 0a0a 2020 2020  ew_series)..    
-0000baa0: 6465 6620 6c6f 6e67 6573 745f 636f 6e74  def longest_cont
-0000bab0: 6967 756f 7573 5f73 6c69 6365 2873 656c  iguous_slice(sel
-0000bac0: 662c 206d 6178 5f67 6170 5f73 697a 653a  f, max_gap_size:
-0000bad0: 2069 6e74 203d 2030 2920 2d3e 2027 5469   int = 0) -> 'Ti
-0000bae0: 6d65 5365 7269 6573 273a 0a20 2020 2020  meSeries':.     
-0000baf0: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-0000bb00: 6574 7572 6e73 2074 6865 206c 6172 6765  eturns the large
-0000bb10: 7374 2054 696d 6553 6572 6965 7320 736c  st TimeSeries sl
-0000bb20: 6963 6520 6f66 2074 6869 7320 6465 7465  ice of this dete
-0000bb30: 726d 696e 6973 7469 6320 7469 6d65 2073  rministic time s
-0000bb40: 6572 6965 7320 7468 6174 2063 6f6e 7461  eries that conta
-0000bb50: 696e 7320 6e6f 2067 6170 730a 2020 2020  ins no gaps.    
-0000bb60: 2020 2020 2863 6f6e 7469 676f 7573 6520      (contigouse 
-0000bb70: 616c 6c2d 4e61 4e20 726f 7773 2920 6c61  all-NaN rows) la
-0000bb80: 7267 6572 2074 6861 6e20 606d 6178 5f67  rger than `max_g
-0000bb90: 6170 5f73 697a 6560 2e0a 0a20 2020 2020  ap_size`...     
-0000bba0: 2020 2054 6869 7320 6d65 7468 6f64 2069     This method i
-0000bbb0: 7320 6f6e 6c79 2061 7070 6c69 6361 626c  s only applicabl
-0000bbc0: 6520 746f 2064 6574 6572 6d69 6e69 7374  e to determinist
-0000bbd0: 6963 2073 6572 6965 7320 2869 2e65 2e2c  ic series (i.e.,
-0000bbe0: 2068 6176 696e 6720 3120 7361 6d70 6c65   having 1 sample
-0000bbf0: 292e 0a0a 2020 2020 2020 2020 5265 7475  )...        Retu
-0000bc00: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-0000bc10: 2d2d 2d0a 2020 2020 2020 2020 5469 6d65  ---.        Time
-0000bc20: 5365 7269 6573 0a20 2020 2020 2020 2020  Series.         
-0000bc30: 2020 2061 206e 6577 2073 6572 6965 7320     a new series 
-0000bc40: 636f 6e73 7469 7475 7469 6e67 2074 6865  constituting the
-0000bc50: 206c 6172 6765 7374 2073 6c69 6365 206f   largest slice o
-0000bc60: 6620 7468 6520 6f72 6967 696e 616c 2077  f the original w
-0000bc70: 6974 6820 6e6f 206f 7220 626f 756e 6465  ith no or bounde
-0000bc80: 6420 6761 7073 0a20 2020 2020 2020 2022  d gaps.        "
-0000bc90: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
-0000bca0: 7420 286e 702e 6973 6e61 6e28 7365 6c66  t (np.isnan(self
-0000bcb0: 2e5f 7861 2929 2e61 6e79 2829 3a0a 2020  ._xa)).any():.  
-0000bcc0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000bcd0: 2073 656c 662e 636f 7079 2829 0a20 2020   self.copy().   
-0000bce0: 2020 2020 2073 7472 6970 7065 645f 7365       stripped_se
-0000bcf0: 7269 6573 203d 2073 656c 662e 7374 7269  ries = self.stri
-0000bd00: 7028 290a 2020 2020 2020 2020 6761 7073  p().        gaps
-0000bd10: 203d 2073 7472 6970 7065 645f 7365 7269   = stripped_seri
-0000bd20: 6573 2e67 6170 7328 290a 2020 2020 2020  es.gaps().      
-0000bd30: 2020 7265 6c65 7661 6e74 5f67 6170 7320    relevant_gaps 
-0000bd40: 3d20 6761 7073 5b67 6170 735b 2767 6170  = gaps[gaps['gap
-0000bd50: 5f73 697a 6527 5d20 3e20 6d61 785f 6761  _size'] > max_ga
-0000bd60: 705f 7369 7a65 5d0a 0a20 2020 2020 2020  p_size]..       
-0000bd70: 2063 7572 725f 736c 6963 655f 7374 6172   curr_slice_star
-0000bd80: 7420 3d20 7374 7269 7070 6564 5f73 6572  t = stripped_ser
-0000bd90: 6965 732e 7374 6172 745f 7469 6d65 2829  ies.start_time()
-0000bda0: 0a20 2020 2020 2020 206d 6178 5f73 697a  .        max_siz
-0000bdb0: 6520 3d20 7064 2e54 696d 6564 656c 7461  e = pd.Timedelta
-0000bdc0: 2864 6179 733d 3029 2069 6620 7365 6c66  (days=0) if self
-0000bdd0: 2e5f 6861 735f 6461 7465 7469 6d65 5f69  ._has_datetime_i
-0000bde0: 6e64 6578 2065 6c73 6520 300a 2020 2020  ndex else 0.    
-0000bdf0: 2020 2020 6d61 785f 736c 6963 655f 7374      max_slice_st
-0000be00: 6172 7420 3d20 4e6f 6e65 0a20 2020 2020  art = None.     
-0000be10: 2020 206d 6178 5f73 6c69 6365 5f65 6e64     max_slice_end
-0000be20: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-0000be30: 666f 7220 696e 6465 782c 2072 6f77 2069  for index, row i
-0000be40: 6e20 7265 6c65 7661 6e74 5f67 6170 732e  n relevant_gaps.
-0000be50: 6974 6572 726f 7773 2829 3a0a 2020 2020  iterrows():.    
-0000be60: 2020 2020 2020 2020 7369 7a65 203d 2072          size = r
-0000be70: 6f77 5b27 6761 705f 7374 6172 7427 5d20  ow['gap_start'] 
-0000be80: 2d20 6375 7272 5f73 6c69 6365 5f73 7461  - curr_slice_sta
-0000be90: 7274 202d 2073 656c 662e 5f66 7265 710a  rt - self._freq.
-0000bea0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000beb0: 697a 6520 3e20 6d61 785f 7369 7a65 3a0a  ize > max_size:.
-0000bec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bed0: 6d61 785f 7369 7a65 203d 2073 697a 650a  max_size = size.
-0000bee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bef0: 6d61 785f 736c 6963 655f 7374 6172 7420  max_slice_start 
-0000bf00: 3d20 6375 7272 5f73 6c69 6365 5f73 7461  = curr_slice_sta
-0000bf10: 7274 0a20 2020 2020 2020 2020 2020 2020  rt.             
-0000bf20: 2020 206d 6178 5f73 6c69 6365 5f65 6e64     max_slice_end
-0000bf30: 203d 2072 6f77 5b27 6761 705f 7374 6172   = row['gap_star
-0000bf40: 7427 5d20 2d20 7365 6c66 2e5f 6672 6571  t'] - self._freq
-0000bf50: 0a20 2020 2020 2020 2020 2020 2063 7572  .            cur
-0000bf60: 725f 736c 6963 655f 7374 6172 7420 3d20  r_slice_start = 
-0000bf70: 726f 775b 2767 6170 5f65 6e64 275d 202b  row['gap_end'] +
-0000bf80: 2073 656c 662e 5f66 7265 710a 0a20 2020   self._freq..   
-0000bf90: 2020 2020 2069 6620 7374 7269 7070 6564       if stripped
-0000bfa0: 5f73 6572 6965 732e 656e 645f 7469 6d65  _series.end_time
-0000bfb0: 2829 202d 2063 7572 725f 736c 6963 655f  () - curr_slice_
-0000bfc0: 7374 6172 7420 3e20 6d61 785f 7369 7a65  start > max_size
-0000bfd0: 3a0a 2020 2020 2020 2020 2020 2020 6d61  :.            ma
-0000bfe0: 785f 736c 6963 655f 7374 6172 7420 3d20  x_slice_start = 
-0000bff0: 6375 7272 5f73 6c69 6365 5f73 7461 7274  curr_slice_start
-0000c000: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
-0000c010: 5f73 6c69 6365 5f65 6e64 203d 2073 656c  _slice_end = sel
-0000c020: 662e 656e 645f 7469 6d65 2829 0a0a 2020  f.end_time()..  
-0000c030: 2020 2020 2020 7265 7475 726e 2073 7472        return str
-0000c040: 6970 7065 645f 7365 7269 6573 5b6d 6178  ipped_series[max
-0000c050: 5f73 6c69 6365 5f73 7461 7274 3a6d 6178  _slice_start:max
-0000c060: 5f73 6c69 6365 5f65 6e64 5d0a 0a20 2020  _slice_end]..   
-0000c070: 2064 6566 2072 6573 6361 6c65 5f77 6974   def rescale_wit
-0000c080: 685f 7661 6c75 6528 7365 6c66 2c20 7661  h_value(self, va
-0000c090: 6c75 655f 6174 5f66 6972 7374 5f73 7465  lue_at_first_ste
-0000c0a0: 703a 2066 6c6f 6174 2920 2d3e 2027 5469  p: float) -> 'Ti
-0000c0b0: 6d65 5365 7269 6573 273a 0a20 2020 2020  meSeries':.     
-0000c0c0: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-0000c0d0: 6574 7572 6e73 2061 206e 6577 2054 696d  eturns a new Tim
-0000c0e0: 6553 6572 6965 732c 2077 6869 6368 2069  eSeries, which i
-0000c0f0: 7320 6120 6d75 6c74 6970 6c65 206f 6620  s a multiple of 
-0000c100: 7468 6973 2054 696d 6553 6572 6965 7320  this TimeSeries 
-0000c110: 7375 6368 2074 6861 740a 2020 2020 2020  such that.      
-0000c120: 2020 7468 6520 6669 7273 7420 7661 6c75    the first valu
-0000c130: 6520 6973 2060 7661 6c75 655f 6174 5f66  e is `value_at_f
-0000c140: 6972 7374 5f73 7465 7060 2e0a 2020 2020  irst_step`..    
-0000c150: 2020 2020 284e 6f74 653a 206e 756d 6572      (Note: numer
-0000c160: 6963 616c 2065 7272 6f72 7320 6361 6e20  ical errors can 
-0000c170: 6170 7065 6172 2077 6974 6820 6076 616c  appear with `val
-0000c180: 7565 5f61 745f 6669 7273 745f 7374 6570  ue_at_first_step
-0000c190: 203e 2031 652b 3234 6029 2e0a 0a20 2020   > 1e+24`)...   
-0000c1a0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-0000c1b0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-0000c1c0: 2d2d 0a20 2020 2020 2020 2076 616c 7565  --.        value
-0000c1d0: 5f61 745f 6669 7273 745f 7374 6570 0a20  _at_first_step. 
-0000c1e0: 2020 2020 2020 2020 2020 2054 6865 206e             The n
-0000c1f0: 6577 2076 616c 7565 2066 6f72 2074 6865  ew value for the
-0000c200: 2066 6972 7374 2065 6e74 7279 206f 6620   first entry of 
-0000c210: 7468 6520 5469 6d65 5365 7269 6573 2e0a  the TimeSeries..
-0000c220: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-0000c230: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-0000c240: 0a20 2020 2020 2020 2054 696d 6553 6572  .        TimeSer
-0000c250: 6965 730a 2020 2020 2020 2020 2020 2020  ies.            
-0000c260: 4120 6e65 7720 5469 6d65 5365 7269 6573  A new TimeSeries
-0000c270: 2c20 7768 6572 6520 7468 6520 6669 7273  , where the firs
-0000c280: 7420 7661 6c75 6520 6973 2060 7661 6c75  t value is `valu
-0000c290: 655f 6174 5f66 6972 7374 5f73 7465 7060  e_at_first_step`
-0000c2a0: 2061 6e64 206f 7468 6572 2076 616c 7565   and other value
-0000c2b0: 730a 2020 2020 2020 2020 2020 2020 6861  s.            ha
-0000c2c0: 7665 2062 6565 6e20 7363 616c 6564 2061  ve been scaled a
-0000c2d0: 6363 6f72 6469 6e67 6c79 2e0a 2020 2020  ccordingly..    
-0000c2e0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-0000c2f0: 2072 6169 7365 5f69 665f 6e6f 7428 2873   raise_if_not((s
-0000c300: 656c 662e 5f78 615b 302c 203a 2c20 3a5d  elf._xa[0, :, :]
-0000c310: 2021 3d20 3029 2e61 6c6c 2829 2c20 2743   != 0).all(), 'C
-0000c320: 616e 6e6f 7420 7265 7363 616c 6520 7769  annot rescale wi
-0000c330: 7468 2066 6972 7374 2076 616c 7565 2030  th first value 0
-0000c340: 2e27 2c20 6c6f 6767 6572 290a 2020 2020  .', logger).    
-0000c350: 2020 2020 636f 6566 203d 2076 616c 7565      coef = value
-0000c360: 5f61 745f 6669 7273 745f 7374 6570 202f  _at_first_step /
-0000c370: 2073 656c 662e 5f78 612e 6973 656c 287b   self._xa.isel({
-0000c380: 7365 6c66 2e5f 7469 6d65 5f64 696d 3a20  self._time_dim: 
-0000c390: 5b30 5d7d 290a 2020 2020 2020 2020 636f  [0]}).        co
-0000c3a0: 6566 203d 2063 6f65 662e 7661 6c75 6573  ef = coef.values
-0000c3b0: 2e72 6573 6861 7065 2828 7365 6c66 2e6e  .reshape((self.n
-0000c3c0: 5f63 6f6d 706f 6e65 6e74 732c 2073 656c  _components, sel
-0000c3d0: 662e 6e5f 7361 6d70 6c65 7329 2920 2023  f.n_samples))  #
-0000c3e0: 2054 4f44 4f3a 2074 6573 740a 2020 2020   TODO: test.    
-0000c3f0: 2020 2020 6e65 775f 7365 7269 6573 203d      new_series =
-0000c400: 2063 6f65 6620 2a20 7365 6c66 2e5f 7861   coef * self._xa
-0000c410: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000c420: 5469 6d65 5365 7269 6573 286e 6577 5f73  TimeSeries(new_s
-0000c430: 6572 6965 7329 0a0a 2020 2020 6465 6620  eries)..    def 
-0000c440: 7368 6966 7428 7365 6c66 2c20 6e3a 2069  shift(self, n: i
-0000c450: 6e74 2920 2d3e 2027 5469 6d65 5365 7269  nt) -> 'TimeSeri
-0000c460: 6573 273a 0a20 2020 2020 2020 2022 2222  es':.        """
-0000c470: 0a20 2020 2020 2020 2053 6869 6674 7320  .        Shifts 
-0000c480: 7468 6520 7469 6d65 2061 7869 7320 6f66  the time axis of
-0000c490: 2074 6869 7320 5469 6d65 5365 7269 6573   this TimeSeries
-0000c4a0: 2062 7920 606e 6020 7469 6d65 2073 7465   by `n` time ste
-0000c4b0: 7073 2e0a 0a20 2020 2020 2020 2049 6620  ps...        If 
-0000c4c0: 3a6d 6174 683a 606e 203e 2030 602c 2073  :math:`n > 0`, s
-0000c4d0: 6869 6674 7320 696e 2074 6865 2066 7574  hifts in the fut
-0000c4e0: 7572 652e 2049 6620 3a6d 6174 683a 606e  ure. If :math:`n
-0000c4f0: 203c 2030 602c 2073 6869 6674 7320 696e   < 0`, shifts in
-0000c500: 2074 6865 2070 6173 742e 0a0a 2020 2020   the past...    
-0000c510: 2020 2020 466f 7220 6578 616d 706c 652c      For example,
-0000c520: 2077 6974 6820 3a6d 6174 683a 606e 3d32   with :math:`n=2
-0000c530: 6020 616e 6420 6066 7265 713d 274d 2760  ` and `freq='M'`
-0000c540: 2c20 4d61 7263 6820 3230 3133 2062 6563  , March 2013 bec
-0000c550: 6f6d 6573 204d 6179 2032 3031 332e 0a20  omes May 2013.. 
-0000c560: 2020 2020 2020 2057 6974 6820 3a6d 6174         With :mat
-0000c570: 683a 606e 3d2d 3260 2c20 4d61 7263 6820  h:`n=-2`, March 
-0000c580: 3230 3133 2062 6563 6f6d 6573 204a 616e  2013 becomes Jan
-0000c590: 2032 3031 332e 0a0a 2020 2020 2020 2020   2013...        
-0000c5a0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-0000c5b0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-0000c5c0: 2020 2020 2020 6e0a 2020 2020 2020 2020        n.        
-0000c5d0: 2020 2020 5468 6520 6e75 6d62 6572 206f      The number o
-0000c5e0: 6620 7469 6d65 2073 7465 7073 2028 696e  f time steps (in
-0000c5f0: 2073 656c 662e 6672 6571 2075 6e69 7429   self.freq unit)
-0000c600: 2074 6f20 7368 6966 7420 6279 2e20 4361   to shift by. Ca
-0000c610: 6e20 6265 206e 6567 6174 6976 652e 0a0a  n be negative...
-0000c620: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-0000c630: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-0000c640: 2020 2020 2020 2020 5469 6d65 5365 7269          TimeSeri
-0000c650: 6573 0a20 2020 2020 2020 2020 2020 2041  es.            A
-0000c660: 206e 6577 2054 696d 6553 6572 6965 732c   new TimeSeries,
-0000c670: 2077 6974 6820 6120 7368 6966 7465 6420   with a shifted 
-0000c680: 696e 6465 782e 0a20 2020 2020 2020 2022  index..        "
-0000c690: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
-0000c6a0: 7420 6973 696e 7374 616e 6365 286e 2c20  t isinstance(n, 
-0000c6b0: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
-0000c6c0: 2020 6c6f 6767 6572 2e77 6172 6e69 6e67    logger.warning
-0000c6d0: 2866 2254 696d 6553 6572 6965 732e 7368  (f"TimeSeries.sh
-0000c6e0: 6966 7428 293a 2063 6f6e 7665 7274 696e  ift(): convertin
-0000c6f0: 6720 6e20 746f 2069 6e74 2066 726f 6d20  g n to int from 
-0000c700: 7b6e 7d20 746f 207b 696e 7428 6e29 7d22  {n} to {int(n)}"
-0000c710: 290a 2020 2020 2020 2020 2020 2020 6e20  ).            n 
-0000c720: 3d20 696e 7428 6e29 0a0a 2020 2020 2020  = int(n)..      
-0000c730: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-0000c740: 2020 2073 656c 662e 5f74 696d 655f 696e     self._time_in
-0000c750: 6465 785b 2d31 5d20 2b20 6e20 2a20 7365  dex[-1] + n * se
-0000c760: 6c66 2e66 7265 710a 2020 2020 2020 2020  lf.freq.        
-0000c770: 6578 6365 7074 2070 642e 6572 726f 7273  except pd.errors
-0000c780: 2e4f 7574 4f66 426f 756e 6473 4461 7465  .OutOfBoundsDate
-0000c790: 7469 6d65 3a0a 2020 2020 2020 2020 2020  time:.          
-0000c7a0: 2020 7261 6973 655f 6c6f 6728 4f76 6572    raise_log(Over
-0000c7b0: 666c 6f77 4572 726f 7228 2274 6865 2061  flowError("the a
-0000c7c0: 6464 206f 7065 7261 7469 6f6e 2062 6574  dd operation bet
-0000c7d0: 7765 656e 207b 7d20 616e 6420 7b7d 2077  ween {} and {} w
-0000c7e0: 696c 6c20 220a 2020 2020 2020 2020 2020  ill ".          
-0000c7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c800: 2020 2020 2020 2020 2020 226f 7665 7266            "overf
-0000c810: 6c6f 7722 2e66 6f72 6d61 7428 6e20 2a20  low".format(n * 
-0000c820: 7365 6c66 2e66 7265 712c 2073 656c 662e  self.freq, self.
-0000c830: 7469 6d65 5f69 6e64 6578 5b2d 315d 2929  time_index[-1]))
-0000c840: 2c20 6c6f 6767 6572 290a 0a20 2020 2020  , logger)..     
-0000c850: 2020 206e 6577 5f74 696d 655f 696e 6465     new_time_inde
-0000c860: 7820 3d20 7365 6c66 2e5f 7469 6d65 5f69  x = self._time_i
-0000c870: 6e64 6578 2e6d 6170 286c 616d 6264 6120  ndex.map(lambda 
-0000c880: 7473 3a20 7473 202b 206e 202a 2073 656c  ts: ts + n * sel
-0000c890: 662e 6672 6571 290a 2020 2020 2020 2020  f.freq).        
-0000c8a0: 6e65 775f 7861 203d 2073 656c 662e 5f78  new_xa = self._x
-0000c8b0: 612e 6173 7369 676e 5f63 6f6f 7264 7328  a.assign_coords(
-0000c8c0: 7b73 656c 662e 5f78 612e 6469 6d73 5b30  {self._xa.dims[0
-0000c8d0: 5d3a 206e 6577 5f74 696d 655f 696e 6465  ]: new_time_inde
-0000c8e0: 787d 290a 2020 2020 2020 2020 7265 7475  x}).        retu
-0000c8f0: 726e 2054 696d 6553 6572 6965 7328 6e65  rn TimeSeries(ne
-0000c900: 775f 7861 290a 0a20 2020 2064 6566 2064  w_xa)..    def d
-0000c910: 6966 6628 7365 6c66 2c0a 2020 2020 2020  iff(self,.      
-0000c920: 2020 2020 2020 206e 3a20 4f70 7469 6f6e         n: Option
-0000c930: 616c 5b69 6e74 5d20 3d20 312c 0a20 2020  al[int] = 1,.   
-0000c940: 2020 2020 2020 2020 2020 7065 7269 6f64            period
-0000c950: 733a 204f 7074 696f 6e61 6c5b 696e 745d  s: Optional[int]
-0000c960: 203d 2031 2c0a 2020 2020 2020 2020 2020   = 1,.          
-0000c970: 2020 2064 726f 706e 613a 204f 7074 696f     dropna: Optio
-0000c980: 6e61 6c5b 626f 6f6c 5d20 3d20 5472 7565  nal[bool] = True
-0000c990: 2920 2d3e 2027 5469 6d65 5365 7269 6573  ) -> 'TimeSeries
-0000c9a0: 273a 0a20 2020 2020 2020 2022 2222 0a20  ':.        """. 
-0000c9b0: 2020 2020 2020 2052 6574 7572 6e73 2061         Returns a
-0000c9c0: 2064 6966 6665 7265 6e63 6564 2074 696d   differenced tim
-0000c9d0: 6520 7365 7269 6573 2e20 5468 6973 2069  e series. This i
-0000c9e0: 7320 6f66 7465 6e20 7573 6564 2074 6f20  s often used to 
-0000c9f0: 6d61 6b65 2061 2074 696d 6520 7365 7269  make a time seri
-0000ca00: 6573 2073 7461 7469 6f6e 6172 792e 0a0a  es stationary...
-0000ca10: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-0000ca20: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-0000ca30: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6e0a  -----.        n.
-0000ca40: 2020 2020 2020 2020 2020 2020 4f70 7469              Opti
-0000ca50: 6f6e 616c 6c79 2c20 6120 706f 7369 7469  onally, a positi
-0000ca60: 7665 2069 6e74 6567 6572 2069 6e64 6963  ve integer indic
-0000ca70: 6174 696e 6720 7468 6520 6e75 6d62 6572  ating the number
-0000ca80: 206f 6620 6469 6666 6572 656e 6369 6e67   of differencing
-0000ca90: 2073 7465 7073 2028 6465 6661 756c 7420   steps (default 
-0000caa0: 3d20 3129 2e0a 2020 2020 2020 2020 2020  = 1)..          
-0000cab0: 2020 466f 7220 696e 7374 616e 6365 2c20    For instance, 
-0000cac0: 6e3d 3220 636f 6d70 7574 6573 2074 6865  n=2 computes the
-0000cad0: 2073 6563 6f6e 6420 6f72 6465 7220 6469   second order di
-0000cae0: 6666 6572 656e 6365 732e 0a20 2020 2020  fferences..     
-0000caf0: 2020 2070 6572 696f 6473 0a20 2020 2020     periods.     
-0000cb00: 2020 2020 2020 204f 7074 696f 6e61 6c6c         Optionall
-0000cb10: 792c 2070 6572 696f 6473 2074 6f20 7368  y, periods to sh
-0000cb20: 6966 7420 666f 7220 6361 6c63 756c 6174  ift for calculat
-0000cb30: 696e 6720 6469 6666 6572 656e 6365 2e20  ing difference. 
-0000cb40: 466f 7220 696e 7374 616e 6365 2c20 7065  For instance, pe
-0000cb50: 7269 6f64 733d 3132 2063 6f6d 7075 7465  riods=12 compute
-0000cb60: 7320 7468 650a 2020 2020 2020 2020 2020  s the.          
-0000cb70: 2020 6469 6666 6572 656e 6365 2062 6574    difference bet
-0000cb80: 7765 656e 2076 616c 7565 7320 6174 2074  ween values at t
-0000cb90: 696d 6520 6074 6020 616e 6420 7469 6d65  ime `t` and time
-0000cba0: 7320 6074 2d31 3260 2e0a 2020 2020 2020  s `t-12`..      
-0000cbb0: 2020 6472 6f70 6e61 0a20 2020 2020 2020    dropna.       
-0000cbc0: 2020 2020 2057 6865 7468 6572 2074 6f20       Whether to 
-0000cbd0: 6472 6f70 2074 6865 206d 6973 7369 6e67  drop the missing
-0000cbe0: 2076 616c 7565 7320 6166 7465 7220 6561   values after ea
-0000cbf0: 6368 2064 6966 6665 7265 6e63 696e 6720  ch differencing 
-0000cc00: 7374 6570 732e 2049 6620 7365 7420 746f  steps. If set to
-0000cc10: 2046 616c 7365 2c20 7468 6520 636f 7272   False, the corr
-0000cc20: 6573 706f 6e64 696e 670a 2020 2020 2020  esponding.      
-0000cc30: 2020 2020 2020 6669 7273 7420 6070 6572        first `per
-0000cc40: 696f 6473 6020 7469 6d65 2073 7465 7073  iods` time steps
-0000cc50: 2077 696c 6c20 6265 2066 696c 6c65 6420   will be filled 
-0000cc60: 7769 7468 204e 614e 732e 0a0a 2020 2020  with NaNs...    
-0000cc70: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-0000cc80: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-0000cc90: 2020 2020 5469 6d65 5365 7269 6573 0a20      TimeSeries. 
-0000cca0: 2020 2020 2020 2020 2020 2041 2054 696d             A Tim
-0000ccb0: 6553 6572 6965 7320 636f 6e73 7472 7563  eSeries construc
-0000ccc0: 7465 6420 6166 7465 7220 6469 6666 6572  ted after differ
-0000ccd0: 656e 6369 6e67 2e0a 2020 2020 2020 2020  encing..        
-0000cce0: 2222 220a 2020 2020 2020 2020 6966 206e  """.        if n
-0000ccf0: 6f74 2069 7369 6e73 7461 6e63 6528 6e2c  ot isinstance(n,
-0000cd00: 2069 6e74 2920 6f72 206e 203c 2031 3a0a   int) or n < 1:.
-0000cd10: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-0000cd20: 7365 5f6c 6f67 2856 616c 7565 4572 726f  se_log(ValueErro
-0000cd30: 7228 2227 6e27 206d 7573 7420 6265 2061  r("'n' must be a
-0000cd40: 2070 6f73 6974 6976 6520 696e 7465 6765   positive intege
-0000cd50: 7220 3e3d 2031 2e22 292c 206c 6f67 6765  r >= 1."), logge
-0000cd60: 7229 0a20 2020 2020 2020 2069 6620 6e6f  r).        if no
-0000cd70: 7420 6973 696e 7374 616e 6365 2870 6572  t isinstance(per
-0000cd80: 696f 6473 2c20 696e 7429 206f 7220 7065  iods, int) or pe
-0000cd90: 7269 6f64 7320 3c20 313a 0a20 2020 2020  riods < 1:.     
-0000cda0: 2020 2020 2020 2020 7261 6973 655f 6c6f          raise_lo
-0000cdb0: 6728 5661 6c75 6545 7272 6f72 2822 2770  g(ValueError("'p
-0000cdc0: 6572 696f 6473 2720 6d75 7374 2062 6520  eriods' must be 
-0000cdd0: 616e 2069 6e74 6567 6572 203e 3d20 312e  an integer >= 1.
-0000cde0: 2229 2c20 6c6f 6767 6572 290a 0a20 2020  "), logger)..   
-0000cdf0: 2020 2020 2064 6566 205f 636f 6d70 7574       def _comput
-0000ce00: 655f 6469 6666 2878 613a 2078 722e 4461  e_diff(xa: xr.Da
-0000ce10: 7461 4172 7261 7929 3a0a 2020 2020 2020  taArray):.      
-0000ce20: 2020 2020 2020 2320 7861 7272 6179 2064        # xarray d
-0000ce30: 6f65 736e 2774 2073 7570 706f 7274 2050  oesn't support P
-0000ce40: 616e 6461 7320 2270 6572 696f 6422 2073  andas "period" s
-0000ce50: 6f20 636f 6d70 7574 6520 6469 6666 2829  o compute diff()
-0000ce60: 206f 7572 7365 6c76 6573 0a20 2020 2020   ourselves.     
-0000ce70: 2020 2020 2020 2069 6620 6e6f 7420 6472         if not dr
-0000ce80: 6f70 6e61 3a0a 2020 2020 2020 2020 2020  opna:.          
-0000ce90: 2020 2020 2020 2320 496e 2074 6869 7320        # In this 
-0000cea0: 6361 7365 2074 6865 206e 6577 2044 6174  case the new Dat
-0000ceb0: 6141 7272 6179 2077 696c 6c20 6861 7665  aArray will have
-0000cec0: 2074 6865 2073 616d 6520 7369 7a65 2061   the same size a
-0000ced0: 6e64 2066 696c 6c65 6420 7769 7468 204e  nd filled with N
-0000cee0: 614e 730a 2020 2020 2020 2020 2020 2020  aNs.            
-0000cef0: 2020 2020 6e65 775f 7861 5f20 3d20 7861      new_xa_ = xa
-0000cf00: 2e63 6f70 7928 290a 2020 2020 2020 2020  .copy().        
-0000cf10: 2020 2020 2020 2020 6e65 775f 7861 5f2e          new_xa_.
-0000cf20: 7661 6c75 6573 5b3a 7065 7269 6f64 732c  values[:periods,
-0000cf30: 203a 2c20 3a5d 203d 206e 702e 6e61 6e0a   :, :] = np.nan.
-0000cf40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf50: 6e65 775f 7861 5f2e 7661 6c75 6573 5b70  new_xa_.values[p
-0000cf60: 6572 696f 6473 3a2c 203a 2c20 3a5d 203d  eriods:, :, :] =
-0000cf70: 2078 612e 7661 6c75 6573 5b70 6572 696f   xa.values[perio
-0000cf80: 6473 3a2c 203a 2c20 3a5d 202d 2078 612e  ds:, :, :] - xa.
-0000cf90: 7661 6c75 6573 5b3a 2d70 6572 696f 6473  values[:-periods
-0000cfa0: 2c20 3a2c 203a 5d0a 2020 2020 2020 2020  , :, :].        
-0000cfb0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000cfc0: 2020 2020 2020 2020 2020 2320 496e 2074            # In t
-0000cfd0: 6869 7320 6361 7365 2074 6865 206e 6577  his case the new
-0000cfe0: 2044 6174 6141 7272 6179 2077 696c 6c20   DataArray will 
-0000cff0: 6265 2073 686f 7274 6572 0a20 2020 2020  be shorter.     
-0000d000: 2020 2020 2020 2020 2020 206e 6577 5f78             new_x
-0000d010: 615f 203d 2078 615b 7065 7269 6f64 733a  a_ = xa[periods:
-0000d020: 2c20 3a2c 203a 5d2e 636f 7079 2829 0a20  , :, :].copy(). 
-0000d030: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000d040: 6577 5f78 615f 2e76 616c 7565 7320 3d20  ew_xa_.values = 
-0000d050: 7861 2e76 616c 7565 735b 7065 7269 6f64  xa.values[period
-0000d060: 733a 2c20 3a2c 203a 5d20 2d20 7861 2e76  s:, :, :] - xa.v
-0000d070: 616c 7565 735b 3a2d 7065 7269 6f64 732c  alues[:-periods,
-0000d080: 203a 2c20 3a5d 0a20 2020 2020 2020 2020   :, :].         
-0000d090: 2020 2072 6574 7572 6e20 6e65 775f 7861     return new_xa
-0000d0a0: 5f0a 0a20 2020 2020 2020 206e 6577 5f78  _..        new_x
-0000d0b0: 6120 3d20 5f63 6f6d 7075 7465 5f64 6966  a = _compute_dif
-0000d0c0: 6628 7365 6c66 2e5f 7861 290a 2020 2020  f(self._xa).    
-0000d0d0: 2020 2020 666f 7220 5f20 696e 2072 616e      for _ in ran
-0000d0e0: 6765 286e 2d31 293a 0a20 2020 2020 2020  ge(n-1):.       
-0000d0f0: 2020 2020 206e 6577 5f78 6120 3d20 5f63       new_xa = _c
-0000d100: 6f6d 7075 7465 5f64 6966 6628 6e65 775f  ompute_diff(new_
-0000d110: 7861 290a 2020 2020 2020 2020 7265 7475  xa).        retu
-0000d120: 726e 2054 696d 6553 6572 6965 7328 6e65  rn TimeSeries(ne
-0000d130: 775f 7861 290a 0a20 2020 2064 6566 2068  w_xa)..    def h
-0000d140: 6173 5f73 616d 655f 7469 6d65 5f61 7328  as_same_time_as(
-0000d150: 7365 6c66 2c20 6f74 6865 723a 2027 5469  self, other: 'Ti
-0000d160: 6d65 5365 7269 6573 2729 202d 3e20 626f  meSeries') -> bo
-0000d170: 6f6c 3a0a 2020 2020 2020 2020 2222 220a  ol:.        """.
-0000d180: 2020 2020 2020 2020 4368 6563 6b73 2077          Checks w
-0000d190: 6865 7468 6572 2074 6869 7320 5469 6d65  hether this Time
-0000d1a0: 5365 7269 6573 2061 6e64 2061 6e6f 7468  Series and anoth
-0000d1b0: 6572 206f 6e65 2068 6176 6520 7468 6520  er one have the 
-0000d1c0: 7361 6d65 2074 696d 6520 696e 6465 782e  same time index.
-0000d1d0: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-0000d1e0: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-0000d1f0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-0000d200: 6f74 6865 720a 2020 2020 2020 2020 2020  other.          
-0000d210: 2020 7468 6520 6f74 6865 7220 7365 7269    the other seri
-0000d220: 6573 0a0a 2020 2020 2020 2020 5265 7475  es..        Retu
-0000d230: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-0000d240: 2d2d 2d0a 2020 2020 2020 2020 626f 6f6c  ---.        bool
-0000d250: 0a20 2020 2020 2020 2020 2020 2054 7275  .            Tru
-0000d260: 6520 6966 2062 6f74 6820 5469 6d65 5365  e if both TimeSe
-0000d270: 7269 6573 2068 6176 6520 7468 6520 7361  ries have the sa
-0000d280: 6d65 2069 6e64 6578 2c20 4661 6c73 6520  me index, False 
-0000d290: 6f74 6865 7277 6973 652e 0a20 2020 2020  otherwise..     
-0000d2a0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-0000d2b0: 6574 7572 6e20 286f 7468 6572 2e74 696d  eturn (other.tim
-0000d2c0: 655f 696e 6465 7820 3d3d 2073 656c 662e  e_index == self.
-0000d2d0: 7469 6d65 5f69 6e64 6578 292e 616c 6c28  time_index).all(
-0000d2e0: 290a 0a20 2020 2064 6566 2061 7070 656e  )..    def appen
-0000d2f0: 6428 7365 6c66 2c20 6f74 6865 723a 2027  d(self, other: '
-0000d300: 5469 6d65 5365 7269 6573 2729 202d 3e20  TimeSeries') -> 
-0000d310: 2754 696d 6553 6572 6965 7327 3a0a 2020  'TimeSeries':.  
-0000d320: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000d330: 2020 4170 7065 6e64 7320 616e 6f74 6865    Appends anothe
-0000d340: 7220 5469 6d65 5365 7269 6573 2074 6f20  r TimeSeries to 
-0000d350: 7468 6973 2054 696d 6553 6572 6965 732c  this TimeSeries,
-0000d360: 2061 6c6f 6e67 2074 6865 2074 696d 6520   along the time 
-0000d370: 6178 6973 2e0a 0a20 2020 2020 2020 2050  axis...        P
-0000d380: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-0000d390: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-0000d3a0: 2020 2020 206f 7468 6572 0a20 2020 2020       other.     
-0000d3b0: 2020 2020 2020 2041 2073 6563 6f6e 6420         A second 
-0000d3c0: 5469 6d65 5365 7269 6573 2e0a 0a20 2020  TimeSeries...   
-0000d3d0: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-0000d3e0: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-0000d3f0: 2020 2020 2054 696d 6553 6572 6965 730a       TimeSeries.
-0000d400: 2020 2020 2020 2020 2020 2020 4120 6e65              A ne
-0000d410: 7720 5469 6d65 5365 7269 6573 2c20 6f62  w TimeSeries, ob
-0000d420: 7461 696e 6564 2062 7920 6170 7065 6e64  tained by append
-0000d430: 696e 6720 7468 6520 7365 636f 6e64 2054  ing the second T
-0000d440: 696d 6553 6572 6965 7320 746f 2074 6865  imeSeries to the
-0000d450: 2066 6972 7374 2e0a 2020 2020 2020 2020   first..        
-0000d460: 2222 220a 2020 2020 2020 2020 7261 6973  """.        rais
-0000d470: 655f 6966 5f6e 6f74 286f 7468 6572 2e68  e_if_not(other.h
-0000d480: 6173 5f64 6174 6574 696d 655f 696e 6465  as_datetime_inde
-0000d490: 7820 3d3d 2073 656c 662e 6861 735f 6461  x == self.has_da
-0000d4a0: 7465 7469 6d65 5f69 6e64 6578 2c0a 2020  tetime_index,.  
-0000d4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4c0: 2020 2027 426f 7468 2073 6572 6965 7320     'Both series 
-0000d4d0: 6d75 7374 2068 6176 6520 7468 6520 7361  must have the sa
-0000d4e0: 6d65 2074 7970 6520 6f66 2074 696d 6520  me type of time 
-0000d4f0: 696e 6465 7820 2865 6974 6865 7220 4461  index (either Da
-0000d500: 7465 7469 6d65 496e 6465 7820 6f72 2052  tetimeIndex or R
-0000d510: 616e 6765 496e 6465 7829 2e27 2c20 6c6f  angeIndex).', lo
-0000d520: 6767 6572 290a 2020 2020 2020 2020 7261  gger).        ra
-0000d530: 6973 655f 6966 5f6e 6f74 286f 7468 6572  ise_if_not(other
-0000d540: 2e66 7265 7120 3d3d 2073 656c 662e 6672  .freq == self.fr
-0000d550: 6571 2c0a 2020 2020 2020 2020 2020 2020  eq,.            
-0000d560: 2020 2020 2020 2020 2027 4170 7065 6e64           'Append
-0000d570: 6564 2054 696d 6553 6572 6965 7320 6d75  ed TimeSeries mu
-0000d580: 7374 2068 6176 6520 7468 6520 7361 6d65  st have the same
-0000d590: 2066 7265 7175 656e 6379 2061 7320 7468   frequency as th
-0000d5a0: 6520 6375 7272 656e 7420 6f6e 6527 2c20  e current one', 
-0000d5b0: 6c6f 6767 6572 290a 2020 2020 2020 2020  logger).        
-0000d5c0: 7261 6973 655f 6966 5f6e 6f74 286f 7468  raise_if_not(oth
-0000d5d0: 6572 2e6e 5f63 6f6d 706f 6e65 6e74 7320  er.n_components 
-0000d5e0: 3d3d 2073 656c 662e 6e5f 636f 6d70 6f6e  == self.n_compon
-0000d5f0: 656e 7473 2c0a 2020 2020 2020 2020 2020  ents,.          
-0000d600: 2020 2020 2020 2020 2020 2027 426f 7468             'Both
-0000d610: 2073 6572 6965 7320 6d75 7374 2068 6176   series must hav
-0000d620: 6520 7468 6520 7361 6d65 206e 756d 6265  e the same numbe
-0000d630: 7220 6f66 2063 6f6d 706f 6e65 6e74 732e  r of components.
-0000d640: 272c 206c 6f67 6765 7229 0a20 2020 2020  ', logger).     
-0000d650: 2020 2072 6169 7365 5f69 665f 6e6f 7428     raise_if_not(
-0000d660: 6f74 6865 722e 6e5f 7361 6d70 6c65 7320  other.n_samples 
-0000d670: 3d3d 2073 656c 662e 6e5f 7361 6d70 6c65  == self.n_sample
-0000d680: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-0000d690: 2020 2020 2020 2020 2742 6f74 6820 7365          'Both se
-0000d6a0: 7269 6573 206d 7573 7420 6861 7665 2074  ries must have t
-0000d6b0: 6865 2073 616d 6520 6e75 6d62 6572 206f  he same number o
-0000d6c0: 6620 636f 6d70 6f6e 656e 7473 2e27 2c20  f components.', 
-0000d6d0: 6c6f 6767 6572 290a 2020 2020 2020 2020  logger).        
-0000d6e0: 6966 2073 656c 662e 5f68 6173 5f64 6174  if self._has_dat
-0000d6f0: 6574 696d 655f 696e 6465 783a 0a20 2020  etime_index:.   
-0000d700: 2020 2020 2020 2020 2072 6169 7365 5f69           raise_i
-0000d710: 665f 6e6f 7428 6f74 6865 722e 7374 6172  f_not(other.star
-0000d720: 745f 7469 6d65 2829 203d 3d20 7365 6c66  t_time() == self
-0000d730: 2e65 6e64 5f74 696d 6528 2920 2b20 7365  .end_time() + se
-0000d740: 6c66 2e66 7265 712c 0a20 2020 2020 2020  lf.freq,.       
-0000d750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d760: 2020 2741 7070 656e 6465 6420 5469 6d65    'Appended Time
-0000d770: 5365 7269 6573 206d 7573 7420 7374 6172  Series must star
-0000d780: 7420 6f6e 6520 7469 6d65 2073 7465 7020  t one time step 
-0000d790: 6166 7465 7220 6375 7272 656e 7420 6f6e  after current on
-0000d7a0: 652e 272c 206c 6f67 6765 7229 0a0a 2020  e.', logger)..  
-0000d7b0: 2020 2020 2020 6f74 6865 725f 7861 203d        other_xa =
-0000d7c0: 206f 7468 6572 2e64 6174 615f 6172 7261   other.data_arra
-0000d7d0: 7928 290a 0a20 2020 2020 2020 206e 6577  y()..        new
-0000d7e0: 5f78 6120 3d20 7872 2e44 6174 6141 7272  _xa = xr.DataArr
-0000d7f0: 6179 286e 702e 636f 6e63 6174 656e 6174  ay(np.concatenat
-0000d800: 6528 2873 656c 662e 5f78 612e 7661 6c75  e((self._xa.valu
-0000d810: 6573 2c20 6f74 6865 725f 7861 2e76 616c  es, other_xa.val
-0000d820: 7565 7329 2c20 6178 6973 3d30 292c 0a20  ues), axis=0),. 
-0000d830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d840: 2020 2020 2020 2020 2020 2020 2064 696d               dim
-0000d850: 733d 7365 6c66 2e5f 7861 2e64 696d 732c  s=self._xa.dims,
-0000d860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d870: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000d880: 6f6f 7264 733d 7b73 656c 662e 5f74 696d  oords={self._tim
-0000d890: 655f 6469 6d3a 2073 656c 662e 5f74 696d  e_dim: self._tim
-0000d8a0: 655f 696e 6465 782e 6170 7065 6e64 286f  e_index.append(o
-0000d8b0: 7468 6572 2e74 696d 655f 696e 6465 7829  ther.time_index)
-0000d8c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000d8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d8e0: 2020 2020 2020 2020 4449 4d53 5b31 5d3a          DIMS[1]:
-0000d8f0: 2073 656c 662e 636f 6d70 6f6e 656e 7473   self.components
-0000d900: 7d29 0a0a 2020 2020 2020 2020 2320 6e65  })..        # ne
-0000d910: 775f 7861 203d 2078 722e 636f 6e63 6174  w_xa = xr.concat
-0000d920: 286f 626a 733d 5b73 656c 662e 5f78 612c  (objs=[self._xa,
-0000d930: 206f 7468 6572 5f78 615d 2c20 6469 6d3d   other_xa], dim=
-0000d940: 7374 7228 7365 6c66 2e5f 7469 6d65 5f64  str(self._time_d
-0000d950: 696d 2929 0a20 2020 2020 2020 2069 6620  im)).        if 
-0000d960: 6e6f 7420 7365 6c66 2e5f 6861 735f 6461  not self._has_da
-0000d970: 7465 7469 6d65 5f69 6e64 6578 3a0a 2020  tetime_index:.  
-0000d980: 2020 2020 2020 2020 2020 6e65 775f 7861            new_xa
-0000d990: 203d 206e 6577 5f78 612e 7265 7365 745f   = new_xa.reset_
-0000d9a0: 696e 6465 7828 6469 6d73 5f6f 725f 6c65  index(dims_or_le
-0000d9b0: 7665 6c73 3d6e 6577 5f78 612e 6469 6d73  vels=new_xa.dims
-0000d9c0: 5b30 5d29 0a0a 2020 2020 2020 2020 7265  [0])..        re
-0000d9d0: 7475 726e 2054 696d 6553 6572 6965 732e  turn TimeSeries.
-0000d9e0: 6672 6f6d 5f78 6172 7261 7928 6e65 775f  from_xarray(new_
-0000d9f0: 7861 2c20 6669 6c6c 5f6d 6973 7369 6e67  xa, fill_missing
-0000da00: 5f64 6174 6573 3d54 7275 652c 2066 7265  _dates=True, fre
-0000da10: 713d 7365 6c66 2e5f 6672 6571 5f73 7472  q=self._freq_str
-0000da20: 290a 0a20 2020 2064 6566 2061 7070 656e  )..    def appen
-0000da30: 645f 7661 6c75 6573 2873 656c 662c 2076  d_values(self, v
-0000da40: 616c 7565 733a 206e 702e 6e64 6172 7261  alues: np.ndarra
-0000da50: 7929 202d 3e20 2754 696d 6553 6572 6965  y) -> 'TimeSerie
-0000da60: 7327 3a0a 2020 2020 2020 2020 2222 220a  s':.        """.
-0000da70: 2020 2020 2020 2020 4170 7065 6e64 7320          Appends 
-0000da80: 7661 6c75 6573 2074 6f20 6375 7272 656e  values to curren
-0000da90: 7420 5469 6d65 5365 7269 6573 2c20 746f  t TimeSeries, to
-0000daa0: 2074 6865 2067 6976 656e 2069 6e64 6963   the given indic
-0000dab0: 6573 2e0a 0a20 2020 2020 2020 2050 6172  es...        Par
-0000dac0: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-0000dad0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-0000dae0: 2020 2076 616c 7565 730a 2020 2020 2020     values.      
-0000daf0: 2020 2020 2020 416e 2061 7272 6179 2077        An array w
-0000db00: 6974 6820 7468 6520 7661 6c75 6573 2074  ith the values t
-0000db10: 6f20 6170 7065 6e64 2e0a 0a20 2020 2020  o append...     
-0000db20: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-0000db30: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-0000db40: 2020 2054 696d 6553 6572 6965 730a 2020     TimeSeries.  
-0000db50: 2020 2020 2020 2020 2020 4120 6e65 7720            A new 
-0000db60: 5469 6d65 5365 7269 6573 2077 6974 6820  TimeSeries with 
-0000db70: 7468 6520 6e65 7720 7661 6c75 6573 2061  the new values a
-0000db80: 7070 656e 6465 640a 2020 2020 2020 2020  ppended.        
-0000db90: 2222 220a 0a20 2020 2020 2020 2023 2054  """..        # T
-0000dba0: 4f44 4f20 7465 7374 0a20 2020 2020 2020  ODO test.       
-0000dbb0: 2069 6620 7365 6c66 2e5f 6861 735f 6461   if self._has_da
-0000dbc0: 7465 7469 6d65 5f69 6e64 6578 3a0a 2020  tetime_index:.  
-0000dbd0: 2020 2020 2020 2020 2020 6964 7820 3d20            idx = 
-0000dbe0: 7064 2e44 6174 6574 696d 6549 6e64 6578  pd.DatetimeIndex
-0000dbf0: 285b 7365 6c66 2e65 6e64 5f74 696d 6528  ([self.end_time(
-0000dc00: 2920 2b20 6920 2a20 7365 6c66 2e5f 6672  ) + i * self._fr
-0000dc10: 6571 2066 6f72 2069 2069 6e20 7261 6e67  eq for i in rang
-0000dc20: 6528 312c 206c 656e 2876 616c 7565 7329  e(1, len(values)
-0000dc30: 2b31 295d 2c20 6672 6571 3d73 656c 662e  +1)], freq=self.
-0000dc40: 5f66 7265 7129 0a20 2020 2020 2020 2065  _freq).        e
-0000dc50: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000dc60: 2069 6478 203d 2070 642e 5261 6e67 6549   idx = pd.RangeI
-0000dc70: 6e64 6578 286c 656e 2873 656c 6629 2c20  ndex(len(self), 
-0000dc80: 6c65 6e28 7365 6c66 292b 6c65 6e28 7661  len(self)+len(va
-0000dc90: 6c75 6573 292c 2031 290a 0a20 2020 2020  lues), 1)..     
-0000dca0: 2020 2072 6574 7572 6e20 7365 6c66 2e61     return self.a
-0000dcb0: 7070 656e 6428 5469 6d65 5365 7269 6573  ppend(TimeSeries
-0000dcc0: 2e66 726f 6d5f 7469 6d65 735f 616e 645f  .from_times_and_
-0000dcd0: 7661 6c75 6573 2876 616c 7565 733d 7661  values(values=va
-0000dce0: 6c75 6573 2c0a 2020 2020 2020 2020 2020  lues,.          
-0000dcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd20: 2020 7469 6d65 733d 6964 782c 0a20 2020    times=idx,.   
-0000dd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd60: 2020 2020 2020 2020 2066 696c 6c5f 6d69           fill_mi
-0000dd70: 7373 696e 675f 6461 7465 733d 4661 6c73  ssing_dates=Fals
-0000dd80: 6529 290a 0a20 2020 2064 6566 2075 7064  e))..    def upd
-0000dd90: 6174 6528 7365 6c66 2c0a 2020 2020 2020  ate(self,.      
-0000dda0: 2020 2020 2020 2020 2069 6e64 6578 3a20           index: 
-0000ddb0: 7064 2e44 6174 6574 696d 6549 6e64 6578  pd.DatetimeIndex
-0000ddc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000ddd0: 2076 616c 7565 733a 206e 702e 6e64 6172   values: np.ndar
-0000dde0: 7261 7920 3d20 4e6f 6e65 2920 2d3e 2027  ray = None) -> '
-0000ddf0: 5469 6d65 5365 7269 6573 273a 0a20 2020  TimeSeries':.   
-0000de00: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000de10: 2055 7064 6174 6573 2074 6865 2054 696d   Updates the Tim
-0000de20: 6553 6572 6965 7320 7769 7468 2074 6865  eSeries with the
-0000de30: 206e 6577 2076 616c 7565 7320 7072 6f76   new values prov
-0000de40: 6964 6564 2e0a 2020 2020 2020 2020 4966  ided..        If
-0000de50: 2069 6e64 6963 6573 2061 7265 206e 6f74   indices are not
-0000de60: 2069 6e20 6f72 6967 696e 616c 2054 696d   in original Tim
-0000de70: 6553 6572 6965 732c 2074 6865 7920 7769  eSeries, they wi
-0000de80: 6c6c 2062 6520 6469 7363 6172 6465 642e  ll be discarded.
-0000de90: 0a20 2020 2020 2020 2055 7365 2060 6e75  .        Use `nu
-0000dea0: 6d70 792e 6e61 6e60 2074 6f20 6967 6e6f  mpy.nan` to igno
-0000deb0: 7265 2061 2073 7065 6369 6669 6320 696e  re a specific in
-0000dec0: 6465 7820 696e 2061 2073 6572 6965 732e  dex in a series.
-0000ded0: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-0000dee0: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-0000def0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-0000df00: 696e 6465 780a 2020 2020 2020 2020 2020  index.          
-0000df10: 2020 4120 6070 616e 6461 732e 4461 7465    A `pandas.Date
-0000df20: 5469 6d65 496e 6465 7860 2063 6f6e 7461  TimeIndex` conta
-0000df30: 696e 696e 6720 7468 6520 696e 6469 6365  ining the indice
-0000df40: 7320 746f 2072 6570 6c61 6365 2e0a 2020  s to replace..  
-0000df50: 2020 2020 2020 7661 6c75 6573 0a20 2020        values.   
-0000df60: 2020 2020 2020 2020 2041 6e20 6172 7261           An arra
-0000df70: 7920 636f 6e74 6169 6e69 6e67 2074 6865  y containing the
-0000df80: 2076 616c 7565 7320 746f 2072 6570 6c61   values to repla
-0000df90: 6365 2028 6f70 7469 6f6e 616c 292e 0a0a  ce (optional)...
-0000dfa0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-0000dfb0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-0000dfc0: 2020 2020 2020 2020 5469 6d65 5365 7269          TimeSeri
-0000dfd0: 6573 0a20 2020 2020 2020 2020 2020 2041  es.            A
-0000dfe0: 206e 6577 2054 696d 6553 6572 6965 7320   new TimeSeries 
-0000dff0: 7769 7468 2075 7064 6174 6564 2076 616c  with updated val
-0000e000: 7565 732e 0a20 2020 2020 2020 2022 2222  ues..        """
-0000e010: 0a20 2020 2020 2020 2023 2054 4f44 4f3a  .        # TODO:
-0000e020: 2049 2064 6f6e 2774 2074 6869 6e6b 2074   I don't think t
-0000e030: 6869 7320 6973 206e 6565 6465 642e 2e2e  his is needed...
-0000e040: 2070 726f 6261 626c 7920 6265 7474 6572   probably better
-0000e050: 2074 6f20 6a75 7374 2063 7265 6174 6520   to just create 
-0000e060: 6120 6e65 7720 5469 6d65 5365 7269 6573  a new TimeSeries
-0000e070: 0a20 2020 2020 2020 2072 6169 7365 204e  .        raise N
-0000e080: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
-0000e090: 6f72 2827 5469 6d65 5365 7269 6573 2e75  or('TimeSeries.u
-0000e0a0: 7064 6174 6528 2920 6973 206e 6f74 2073  pdate() is not s
-0000e0b0: 7570 706f 7274 6564 2061 6e79 6d6f 7265  upported anymore
-0000e0c0: 2e27 290a 0a20 2020 2064 6566 2073 7461  .')..    def sta
-0000e0d0: 636b 2873 656c 662c 206f 7468 6572 3a20  ck(self, other: 
-0000e0e0: 2754 696d 6553 6572 6965 7327 2920 2d3e  'TimeSeries') ->
-0000e0f0: 2027 5469 6d65 5365 7269 6573 273a 0a20   'TimeSeries':. 
-0000e100: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000e110: 2020 2053 7461 636b 7320 616e 6f74 6865     Stacks anothe
-0000e120: 7220 756e 6976 6172 6961 7465 206f 7220  r univariate or 
-0000e130: 6d75 6c74 6976 6172 6961 7465 2054 696d  multivariate Tim
-0000e140: 6553 6572 6965 7320 7769 7468 2074 6865  eSeries with the
-0000e150: 2073 616d 6520 7469 6d65 2069 6e64 6578   same time index
-0000e160: 206f 6e20 746f 7020 6f66 0a20 2020 2020   on top of.     
-0000e170: 2020 2074 6865 2063 7572 7265 6e74 206f     the current o
-0000e180: 6e65 2028 616c 6f6e 6720 7468 6520 636f  ne (along the co
-0000e190: 6d70 6f6e 656e 7420 6178 6973 292c 2061  mponent axis), a
-0000e1a0: 6e64 2072 6574 7572 6e73 2074 6865 206e  nd returns the n
-0000e1b0: 6577 6c79 2066 6f72 6d65 6420 6d75 6c74  ewly formed mult
-0000e1c0: 6976 6172 6961 7465 2054 696d 6553 6572  ivariate TimeSer
-0000e1d0: 6965 7320 7468 6174 2069 6e63 6c75 6465  ies that include
-0000e1e0: 730a 2020 2020 2020 2020 616c 6c20 7468  s.        all th
-0000e1f0: 6520 636f 6d70 6f6e 656e 7473 206f 6620  e components of 
-0000e200: 6073 656c 6660 2061 6e64 206f 6620 606f  `self` and of `o
-0000e210: 7468 6572 602e 0a0a 2020 2020 2020 2020  ther`...        
-0000e220: 5468 6520 7265 7375 6c74 696e 6720 5469  The resulting Ti
-0000e230: 6d65 5365 7269 6573 2077 696c 6c20 6861  meSeries will ha
-0000e240: 7665 2074 6865 2073 616d 6520 6e61 6d65  ve the same name
-0000e250: 2066 6f72 2069 7473 2074 696d 6520 6469   for its time di
-0000e260: 6d65 6e73 696f 6e20 6173 2074 6869 7320  mension as this 
-0000e270: 5469 6d65 5365 7269 6573 2c20 616e 6420  TimeSeries, and 
-0000e280: 7468 650a 2020 2020 2020 2020 7361 6d65  the.        same
-0000e290: 206e 756d 6265 7220 6f66 2073 616d 706c   number of sampl
-0000e2a0: 6573 2e0a 0a20 2020 2020 2020 2050 6172  es...        Par
-0000e2b0: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-0000e2c0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-0000e2d0: 2020 206f 7468 6572 0a20 2020 2020 2020     other.       
-0000e2e0: 2020 2020 2041 2054 696d 6553 6572 6965       A TimeSerie
-0000e2f0: 7320 696e 7374 616e 6365 2077 6974 6820  s instance with 
-0000e300: 7468 6520 7361 6d65 2069 6e64 6578 2061  the same index a
-0000e310: 6e64 2074 6865 2073 616d 6520 6e75 6d62  nd the same numb
-0000e320: 6572 206f 6620 7361 6d70 6c65 7320 6173  er of samples as
-0000e330: 2074 6865 2063 7572 7265 6e74 206f 6e65   the current one
-0000e340: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-0000e350: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
-0000e360: 2d2d 0a20 2020 2020 2020 2054 696d 6553  --.        TimeS
-0000e370: 6572 6965 730a 2020 2020 2020 2020 2020  eries.          
-0000e380: 2020 4120 6e65 7720 6d75 6c74 6976 6172    A new multivar
-0000e390: 6961 7465 2054 696d 6553 6572 6965 7320  iate TimeSeries 
-0000e3a0: 696e 7374 616e 6365 2e0a 2020 2020 2020  instance..      
-0000e3b0: 2020 2222 220a 2020 2020 2020 2020 7261    """.        ra
-0000e3c0: 6973 655f 6966 5f6e 6f74 2873 656c 662e  ise_if_not(self.
-0000e3d0: 6861 735f 7361 6d65 5f74 696d 655f 6173  has_same_time_as
-0000e3e0: 286f 7468 6572 292c 2027 5468 6520 696e  (other), 'The in
-0000e3f0: 6469 6365 7320 6f66 2074 6865 2074 776f  dices of the two
-0000e400: 2054 696d 6553 6572 6965 7320 696e 7374   TimeSeries inst
-0000e410: 616e 6365 7320 270a 2020 2020 2020 2020  ances '.        
-0000e420: 2020 2020 2020 2020 2020 2020 2027 6d75               'mu
-0000e430: 7374 2062 6520 6571 7561 6c27 2c20 6c6f  st be equal', lo
-0000e440: 6767 6572 290a 2020 2020 2020 2020 7261  gger).        ra
-0000e450: 6973 655f 6966 5f6e 6f74 2873 656c 662e  ise_if_not(self.
-0000e460: 6e5f 7361 6d70 6c65 7320 3d3d 206f 7468  n_samples == oth
-0000e470: 6572 2e6e 5f73 616d 706c 6573 2c20 2754  er.n_samples, 'T
-0000e480: 776f 2073 6572 6965 7320 6361 6e20 6265  wo series can be
-0000e490: 2073 7461 636b 6564 206f 6e6c 7920 6966   stacked only if
-0000e4a0: 2074 6865 7920 270a 2020 2020 2020 2020   they '.        
-0000e4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061f0: 2020 2027 4675 6e63 7469 6f6e 2063 616c     'Function cal
+00006200: 6c65 6420 7769 7468 2061 2074 696d 6573  led with a times
+00006210: 7461 6d70 2c20 6275 7420 7365 7269 6573  tamp, but series
+00006220: 206e 6f74 2074 696d 652d 696e 6465 7865   not time-indexe
+00006230: 642e 272c 0a20 2020 2020 2020 2020 2020  d.',.           
+00006240: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00006250: 6767 6572 290a 2020 2020 2020 2020 2020  gger).          
+00006260: 2020 6973 5f69 6e73 6964 6520 3d20 7365    is_inside = se
+00006270: 6c66 2e73 7461 7274 5f74 696d 6528 2920  lf.start_time() 
+00006280: 3c3d 2074 7320 3c3d 2073 656c 662e 656e  <= ts <= self.en
+00006290: 645f 7469 6d65 2829 0a20 2020 2020 2020  d_time().       
+000062a0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000062b0: 2020 2069 6620 7365 6c66 2e5f 6861 735f     if self._has_
+000062c0: 6461 7465 7469 6d65 5f69 6e64 6578 3a0a  datetime_index:.
+000062d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062e0: 6973 5f69 6e73 6964 6520 3d20 3020 3c3d  is_inside = 0 <=
+000062f0: 2074 7320 3c3d 206c 656e 2873 656c 6629   ts <= len(self)
+00006300: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00006310: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00006320: 2020 2069 735f 696e 7369 6465 203d 2073     is_inside = s
+00006330: 656c 662e 7374 6172 745f 7469 6d65 2829  elf.start_time()
+00006340: 203c 3d20 7473 203c 3d20 7365 6c66 2e65   <= ts <= self.e
+00006350: 6e64 5f74 696d 6528 290a 0a20 2020 2020  nd_time()..     
+00006360: 2020 2072 6169 7365 5f69 665f 6e6f 7428     raise_if_not(
+00006370: 6973 5f69 6e73 6964 652c 2027 5469 6d65  is_inside, 'Time
+00006380: 7374 616d 7020 6d75 7374 2062 6520 6265  stamp must be be
+00006390: 7477 6565 6e20 7b7d 2061 6e64 207b 7d27  tween {} and {}'
+000063a0: 2e66 6f72 6d61 7428 7365 6c66 2e73 7461  .format(self.sta
+000063b0: 7274 5f74 696d 6528 292c 0a20 2020 2020  rt_time(),.     
+000063c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006400: 2020 2020 2020 2020 7365 6c66 2e65 6e64          self.end
+00006410: 5f74 696d 6528 2929 2c0a 2020 2020 2020  _time()),.      
+00006420: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00006430: 6f67 6765 7229 0a0a 2020 2020 6465 6620  ogger)..    def 
+00006440: 5f67 6574 5f66 6972 7374 5f74 696d 6573  _get_first_times
+00006450: 7461 6d70 5f61 6674 6572 2873 656c 662c  tamp_after(self,
+00006460: 2074 733a 2070 642e 5469 6d65 7374 616d   ts: pd.Timestam
+00006470: 7029 202d 3e20 7064 2e54 696d 6573 7461  p) -> pd.Timesta
+00006480: 6d70 3a0a 2020 2020 2020 2020 7265 7475  mp:.        retu
+00006490: 726e 206e 6578 7428 6669 6c74 6572 286c  rn next(filter(l
+000064a0: 616d 6264 6120 743a 2074 203e 3d20 7473  ambda t: t >= ts
+000064b0: 2c20 7365 6c66 2e5f 7469 6d65 5f69 6e64  , self._time_ind
+000064c0: 6578 2929 0a0a 2020 2020 6465 6620 5f67  ex))..    def _g
+000064d0: 6574 5f6c 6173 745f 7469 6d65 7374 616d  et_last_timestam
+000064e0: 705f 6265 666f 7265 2873 656c 662c 2074  p_before(self, t
+000064f0: 733a 2070 642e 5469 6d65 7374 616d 7029  s: pd.Timestamp)
+00006500: 202d 3e20 7064 2e54 696d 6573 7461 6d70   -> pd.Timestamp
+00006510: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00006520: 206e 6578 7428 6669 6c74 6572 286c 616d   next(filter(lam
+00006530: 6264 6120 743a 2074 203c 3d20 7473 2c20  bda t: t <= ts, 
+00006540: 7365 6c66 2e5f 7469 6d65 5f69 6e64 6578  self._time_index
+00006550: 5b3a 3a2d 315d 2929 0a0a 2020 2020 2222  [::-1]))..    ""
+00006560: 220a 2020 2020 4578 706f 7274 2066 756e  ".    Export fun
+00006570: 6374 696f 6e73 0a20 2020 203d 3d3d 3d3d  ctions.    =====
+00006580: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020  ===========.    
+00006590: 2222 220a 0a20 2020 2064 6566 2064 6174  """..    def dat
+000065a0: 615f 6172 7261 7928 7365 6c66 2c20 636f  a_array(self, co
+000065b0: 7079 3d54 7275 6529 202d 3e20 7872 2e44  py=True) -> xr.D
+000065c0: 6174 6141 7272 6179 3a0a 2020 2020 2020  ataArray:.      
+000065d0: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
+000065e0: 7475 726e 7320 7468 6520 7861 7272 6179  turns the xarray
+000065f0: 2044 6174 6141 7272 6179 2072 6570 7265   DataArray repre
+00006600: 7365 6e74 6174 696f 6e20 6f66 2074 6869  sentation of thi
+00006610: 7320 7469 6d65 2073 6572 6965 732e 0a0a  s time series...
+00006620: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00006630: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+00006640: 2d2d 2d2d 2d0a 2020 2020 2020 2020 636f  -----.        co
+00006650: 7079 0a20 2020 2020 2020 2020 2020 2057  py.            W
+00006660: 6865 7468 6572 2074 6f20 7265 7475 726e  hether to return
+00006670: 2061 2063 6f70 7920 6f66 2074 6865 2073   a copy of the s
+00006680: 6572 6965 732e 204c 6561 7665 2069 7420  eries. Leave it 
+00006690: 746f 2054 7275 6520 756e 6c65 7373 2079  to True unless y
+000066a0: 6f75 206b 6e6f 7720 7768 6174 2079 6f75  ou know what you
+000066b0: 2061 7265 2064 6f69 6e67 2e0a 0a20 2020   are doing...   
+000066c0: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+000066d0: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+000066e0: 2020 2020 2078 6172 7261 792e 4461 7461       xarray.Data
+000066f0: 4172 7261 790a 2020 2020 2020 2020 2020  Array.          
+00006700: 2020 5468 6520 7861 7272 6179 2044 6174    The xarray Dat
+00006710: 6141 7272 6179 2075 6e64 6572 6c79 696e  aArray underlyin
+00006720: 6720 7468 6973 2074 696d 6520 7365 7269  g this time seri
+00006730: 6573 2e0a 2020 2020 2020 2020 2222 220a  es..        """.
+00006740: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00006750: 656c 662e 5f78 612e 636f 7079 2829 2069  elf._xa.copy() i
+00006760: 6620 636f 7079 2065 6c73 6520 7365 6c66  f copy else self
+00006770: 2e5f 7861 0a0a 2020 2020 6465 6620 7064  ._xa..    def pd
+00006780: 5f73 6572 6965 7328 7365 6c66 2c20 636f  _series(self, co
+00006790: 7079 3d54 7275 6529 202d 3e20 7064 2e53  py=True) -> pd.S
+000067a0: 6572 6965 733a 0a20 2020 2020 2020 2022  eries:.        "
+000067b0: 2222 0a20 2020 2020 2020 2052 6574 7572  "".        Retur
+000067c0: 6e73 2061 2050 616e 6461 7320 5365 7269  ns a Pandas Seri
+000067d0: 6573 2072 6570 7265 7365 6e74 6174 696f  es representatio
+000067e0: 6e20 6f66 2074 6869 7320 7469 6d65 2073  n of this time s
+000067f0: 6572 6965 732e 0a20 2020 2020 2020 2057  eries..        W
+00006800: 6f72 6b73 206f 6e6c 7920 666f 7220 756e  orks only for un
+00006810: 6976 6172 6961 7465 2073 6572 6965 7320  ivariate series 
+00006820: 7468 6174 2061 7265 2064 6574 6572 6d69  that are determi
+00006830: 6e69 7374 6963 2028 692e 652e 2c20 6d61  nistic (i.e., ma
+00006840: 6465 206f 6620 3120 7361 6d70 6c65 292e  de of 1 sample).
+00006850: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+00006860: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+00006870: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00006880: 636f 7079 0a20 2020 2020 2020 2020 2020  copy.           
+00006890: 2057 6865 7468 6572 2074 6f20 7265 7475   Whether to retu
+000068a0: 726e 2061 2063 6f70 7920 6f66 2074 6865  rn a copy of the
+000068b0: 2073 6572 6965 732e 204c 6561 7665 2069   series. Leave i
+000068c0: 7420 746f 2054 7275 6520 756e 6c65 7373  t to True unless
+000068d0: 2079 6f75 206b 6e6f 7720 7768 6174 2079   you know what y
+000068e0: 6f75 2061 7265 2064 6f69 6e67 2e0a 0a20  ou are doing... 
+000068f0: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
+00006900: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
+00006910: 2020 2020 2020 2070 616e 6461 732e 5365         pandas.Se
+00006920: 7269 6573 0a20 2020 2020 2020 2020 2020  ries.           
+00006930: 2041 2050 616e 6461 7320 5365 7269 6573   A Pandas Series
+00006940: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
+00006950: 6f66 2074 6869 7320 756e 6976 6172 6961  of this univaria
+00006960: 7465 2074 696d 6520 7365 7269 6573 2e0a  te time series..
+00006970: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00006980: 2020 2020 7365 6c66 2e5f 6173 7365 7274      self._assert
+00006990: 5f75 6e69 7661 7269 6174 6528 290a 2020  _univariate().  
+000069a0: 2020 2020 2020 7365 6c66 2e5f 6173 7365        self._asse
+000069b0: 7274 5f64 6574 6572 6d69 6e69 7374 6963  rt_deterministic
+000069c0: 2829 0a20 2020 2020 2020 2069 6620 636f  ().        if co
+000069d0: 7079 3a0a 2020 2020 2020 2020 2020 2020  py:.            
+000069e0: 7265 7475 726e 2070 642e 5365 7269 6573  return pd.Series
+000069f0: 2873 656c 662e 5f78 615b 3a2c 2030 2c20  (self._xa[:, 0, 
+00006a00: 305d 2e63 6f70 7928 292c 2069 6e64 6578  0].copy(), index
+00006a10: 3d73 656c 662e 5f74 696d 655f 696e 6465  =self._time_inde
+00006a20: 782e 636f 7079 2829 290a 2020 2020 2020  x.copy()).      
+00006a30: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00006a40: 2020 2020 7265 7475 726e 2070 642e 5365      return pd.Se
+00006a50: 7269 6573 2873 656c 662e 5f78 615b 3a2c  ries(self._xa[:,
+00006a60: 2030 2c20 305d 2c20 696e 6465 783d 7365   0, 0], index=se
+00006a70: 6c66 2e5f 7469 6d65 5f69 6e64 6578 290a  lf._time_index).
+00006a80: 0a20 2020 2064 6566 2070 645f 6461 7461  .    def pd_data
+00006a90: 6672 616d 6528 7365 6c66 2c20 636f 7079  frame(self, copy
+00006aa0: 3d54 7275 6529 202d 3e20 7064 2e44 6174  =True) -> pd.Dat
+00006ab0: 6146 7261 6d65 3a0a 2020 2020 2020 2020  aFrame:.        
+00006ac0: 2222 220a 2020 2020 2020 2020 5265 7475  """.        Retu
+00006ad0: 726e 7320 6120 5061 6e64 6173 2044 6174  rns a Pandas Dat
+00006ae0: 6146 7261 6d65 2072 6570 7265 7365 6e74  aFrame represent
+00006af0: 6174 696f 6e20 6f66 2074 6869 7320 7469  ation of this ti
+00006b00: 6d65 2073 6572 6965 732e 0a20 2020 2020  me series..     
+00006b10: 2020 2045 6163 6820 6f66 2074 6865 2073     Each of the s
+00006b20: 6572 6965 7320 636f 6d70 6f6e 656e 7473  eries components
+00006b30: 2077 696c 6c20 6170 7065 6172 2061 7320   will appear as 
+00006b40: 6120 636f 6c75 6d6e 2069 6e20 7468 6520  a column in the 
+00006b50: 4461 7461 4672 616d 652e 0a20 2020 2020  DataFrame..     
+00006b60: 2020 2057 6f72 6b73 206f 6e6c 7920 666f     Works only fo
+00006b70: 7220 6465 7465 726d 696e 6973 7469 6320  r deterministic 
+00006b80: 7365 7269 6573 2028 692e 652e 2c20 6d61  series (i.e., ma
+00006b90: 6465 206f 6620 3120 7361 6d70 6c65 292e  de of 1 sample).
+00006ba0: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+00006bb0: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+00006bc0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00006bd0: 636f 7079 0a20 2020 2020 2020 2020 2020  copy.           
+00006be0: 2057 6865 7468 6572 2074 6f20 7265 7475   Whether to retu
+00006bf0: 726e 2061 2063 6f70 7920 6f66 2074 6865  rn a copy of the
+00006c00: 2064 6174 6166 7261 6d65 2e20 4c65 6176   dataframe. Leav
+00006c10: 6520 6974 2074 6f20 5472 7565 2075 6e6c  e it to True unl
+00006c20: 6573 7320 796f 7520 6b6e 6f77 2077 6861  ess you know wha
+00006c30: 7420 796f 7520 6172 6520 646f 696e 672e  t you are doing.
+00006c40: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00006c50: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00006c60: 2d0a 2020 2020 2020 2020 7061 6e64 6173  -.        pandas
+00006c70: 2e44 6174 6146 7261 6d65 0a20 2020 2020  .DataFrame.     
+00006c80: 2020 2020 2020 2054 6865 2050 616e 6461         The Panda
+00006c90: 7320 4461 7461 4672 616d 6520 7265 7072  s DataFrame repr
+00006ca0: 6573 656e 7461 7469 6f6e 206f 6620 7468  esentation of th
+00006cb0: 6973 2074 696d 6520 7365 7269 6573 0a20  is time series. 
+00006cc0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00006cd0: 2020 2069 6620 6e6f 7420 7365 6c66 2e69     if not self.i
+00006ce0: 735f 6465 7465 726d 696e 6973 7469 633a  s_deterministic:
+00006cf0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00006d00: 7365 5f6c 6f67 2841 7373 6572 7469 6f6e  se_log(Assertion
+00006d10: 4572 726f 7228 2754 6865 2070 645f 6461  Error('The pd_da
+00006d20: 7461 6672 616d 6528 2920 6d65 7468 6f64  taframe() method
+00006d30: 2063 616e 206f 6e6c 7920 7265 7475 726e   can only return
+00006d40: 2044 6174 6146 7261 6d65 7320 6f66 2064   DataFrames of d
+00006d50: 6574 6572 6d69 6e69 7374 6963 2027 0a20  eterministic '. 
+00006d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d80: 2020 2020 2774 696d 6520 7365 7269 6573      'time series
+00006d90: 2c20 616e 6420 7468 6973 2073 6572 6965  , and this serie
+00006da0: 7320 6973 206e 6f74 2064 6574 6572 6d69  s is not determi
+00006db0: 6e69 7374 6963 2028 6974 2063 6f6e 7461  nistic (it conta
+00006dc0: 696e 7320 7365 7665 7261 6c20 7361 6d70  ins several samp
+00006dd0: 6c65 7329 2e20 270a 2020 2020 2020 2020  les). '.        
+00006de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006df0: 2020 2020 2020 2020 2020 2020 2027 436f               'Co
+00006e00: 6e73 6964 6572 2063 616c 6c69 6e67 2071  nsider calling q
+00006e10: 7561 6e74 696c 655f 6466 2829 2069 6e73  uantile_df() ins
+00006e20: 7465 6164 2e27 2929 0a20 2020 2020 2020  tead.')).       
+00006e30: 2069 6620 636f 7079 3a0a 2020 2020 2020   if copy:.      
+00006e40: 2020 2020 2020 7265 7475 726e 2070 642e        return pd.
+00006e50: 4461 7461 4672 616d 6528 7365 6c66 2e5f  DataFrame(self._
+00006e60: 7861 5b3a 2c20 3a2c 2030 5d2e 7661 6c75  xa[:, :, 0].valu
+00006e70: 6573 2e63 6f70 7928 292c 0a20 2020 2020  es.copy(),.     
+00006e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e90: 2020 2020 2020 2020 2020 2069 6e64 6578             index
+00006ea0: 3d73 656c 662e 5f74 696d 655f 696e 6465  =self._time_inde
+00006eb0: 782e 636f 7079 2829 2c0a 2020 2020 2020  x.copy(),.      
+00006ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ed0: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
+00006ee0: 733d 7365 6c66 2e5f 7861 2e67 6574 5f69  s=self._xa.get_i
+00006ef0: 6e64 6578 2827 636f 6d70 6f6e 656e 7427  ndex('component'
+00006f00: 292e 636f 7079 2829 290a 2020 2020 2020  ).copy()).      
+00006f10: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00006f20: 2020 2020 7265 7475 726e 2070 642e 4461      return pd.Da
+00006f30: 7461 4672 616d 6528 7365 6c66 2e5f 7861  taFrame(self._xa
+00006f40: 5b3a 2c20 3a2c 2030 5d2e 7661 6c75 6573  [:, :, 0].values
+00006f50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f70: 2020 696e 6465 783d 7365 6c66 2e5f 7469    index=self._ti
+00006f80: 6d65 5f69 6e64 6578 2c0a 2020 2020 2020  me_index,.      
+00006f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fa0: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
+00006fb0: 733d 7365 6c66 2e5f 7861 2e67 6574 5f69  s=self._xa.get_i
+00006fc0: 6e64 6578 2827 636f 6d70 6f6e 656e 7427  ndex('component'
+00006fd0: 2929 0a0a 2020 2020 6465 6620 7175 616e  ))..    def quan
+00006fe0: 7469 6c65 5f64 6628 7365 6c66 2c20 7175  tile_df(self, qu
+00006ff0: 616e 7469 6c65 3d30 2e35 2920 2d3e 2070  antile=0.5) -> p
+00007000: 642e 4461 7461 4672 616d 653a 0a20 2020  d.DataFrame:.   
+00007010: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00007020: 2052 6574 7572 6e73 2061 2050 616e 6461   Returns a Panda
+00007030: 7320 4461 7461 4672 616d 6520 636f 6e74  s DataFrame cont
+00007040: 6169 6e69 6e67 2074 6865 2073 696e 676c  aining the singl
+00007050: 6520 6465 7369 7265 6420 7175 616e 7469  e desired quanti
+00007060: 6c65 206f 6620 6561 6368 2063 6f6d 706f  le of each compo
+00007070: 6e65 6e74 2028 6f76 6572 2074 6865 2073  nent (over the s
+00007080: 616d 706c 6573 292e 0a20 2020 2020 2020  amples)..       
+00007090: 2045 6163 6820 6f66 2074 6865 2073 6572   Each of the ser
+000070a0: 6965 7320 636f 6d70 6f6e 656e 7473 2077  ies components w
+000070b0: 696c 6c20 6170 7065 6172 2061 7320 6120  ill appear as a 
+000070c0: 636f 6c75 6d6e 2069 6e20 7468 6520 4461  column in the Da
+000070d0: 7461 4672 616d 652e 2054 6865 2063 6f6c  taFrame. The col
+000070e0: 756d 6e20 7769 6c6c 2062 6520 6e61 6d65  umn will be name
+000070f0: 640a 2020 2020 2020 2020 223c 636f 6d70  d.        "<comp
+00007100: 6f6e 656e 743e 5f58 222c 2077 6865 7265  onent>_X", where
+00007110: 2022 3c63 6f6d 706f 6e65 6e74 3e22 2069   "<component>" i
+00007120: 7320 7468 6520 636f 6c75 6d6e 206e 616d  s the column nam
+00007130: 6520 636f 7272 6573 706f 6e64 696e 6720  e corresponding 
+00007140: 746f 2074 6869 7320 636f 6d70 6f6e 656e  to this componen
+00007150: 742c 2061 6e64 2022 5822 0a20 2020 2020  t, and "X".     
+00007160: 2020 2069 7320 7468 6520 7175 616e 7469     is the quanti
+00007170: 6c65 2076 616c 7565 2e0a 2020 2020 2020  le value..      
+00007180: 2020 5468 6520 7175 616e 7469 6c65 2063    The quantile c
+00007190: 6f6c 756d 6e73 2072 6570 7265 7365 6e74  olumns represent
+000071a0: 2074 6865 206d 6172 6769 6e61 6c20 6469   the marginal di
+000071b0: 7374 7269 6275 7469 6f6e 7320 6f66 2074  stributions of t
+000071c0: 6865 2063 6f6d 706f 6e65 6e74 7320 6f66  he components of
+000071d0: 2074 6869 7320 7365 7269 6573 2e0a 0a20   this series... 
+000071e0: 2020 2020 2020 2054 6869 7320 776f 726b         This work
+000071f0: 7320 6f6e 6c79 206f 6e20 7374 6f63 6861  s only on stocha
+00007200: 7374 6963 2073 6572 6965 7320 2869 2e65  stic series (i.e
+00007210: 2e2c 2077 6974 6820 6d6f 7265 2074 6861  ., with more tha
+00007220: 6e20 3120 7361 6d70 6c65 290a 0a20 2020  n 1 sample)..   
+00007230: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+00007240: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00007250: 2d2d 0a20 2020 2020 2020 2071 7561 6e74  --.        quant
+00007260: 696c 650a 2020 2020 2020 2020 2020 2020  ile.            
+00007270: 5468 6520 6465 7369 7265 6420 7175 616e  The desired quan
+00007280: 7469 6c65 2076 616c 7565 2e20 5468 6520  tile value. The 
+00007290: 7661 6c75 6520 6d75 7374 2062 6520 7265  value must be re
+000072a0: 7072 6573 656e 7465 6420 6173 2061 2066  presented as a f
+000072b0: 7261 6374 696f 6e0a 2020 2020 2020 2020  raction.        
+000072c0: 2020 2020 2862 6574 7765 656e 2030 2061      (between 0 a
+000072d0: 6e64 2031 2069 6e63 6c75 7369 7665 292e  nd 1 inclusive).
+000072e0: 2046 6f72 2069 6e73 7461 6e63 652c 2060   For instance, `
+000072f0: 302e 3560 2077 696c 6c20 7265 7475 726e  0.5` will return
+00007300: 2061 2044 6174 6146 7261 6d65 0a20 2020   a DataFrame.   
+00007310: 2020 2020 2020 2020 2063 6f6e 7461 696e           contain
+00007320: 696e 6720 7468 6520 6d65 6469 616e 206f  ing the median o
+00007330: 6620 7468 6520 286d 6172 6769 6e61 6c29  f the (marginal)
+00007340: 2064 6973 7472 6962 7574 696f 6e20 6f66   distribution of
+00007350: 2065 6163 6820 636f 6d70 6f6e 656e 742e   each component.
+00007360: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00007370: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00007380: 2d0a 2020 2020 2020 2020 7061 6e64 6173  -.        pandas
+00007390: 2e44 6174 6146 7261 6d65 0a20 2020 2020  .DataFrame.     
+000073a0: 2020 2020 2020 2054 6865 2050 616e 6461         The Panda
+000073b0: 7320 4461 7461 4672 616d 6520 636f 6e74  s DataFrame cont
+000073c0: 6169 6e69 6e67 2074 6865 2064 6573 6972  aining the desir
+000073d0: 6564 2071 7561 6e74 696c 6520 666f 7220  ed quantile for 
+000073e0: 6561 6368 2063 6f6d 706f 6e65 6e74 2e0a  each component..
+000073f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00007400: 2020 2020 7365 6c66 2e5f 6173 7365 7274      self._assert
+00007410: 5f73 746f 6368 6173 7469 6328 290a 2020  _stochastic().  
+00007420: 2020 2020 2020 7261 6973 655f 6966 5f6e        raise_if_n
+00007430: 6f74 2830 203c 3d20 7175 616e 7469 6c65  ot(0 <= quantile
+00007440: 203c 3d20 312c 0a20 2020 2020 2020 2020   <= 1,.         
+00007450: 2020 2020 2020 2020 2020 2020 2754 6865              'The
+00007460: 2071 7561 6e74 696c 6520 7661 6c75 6573   quantile values
+00007470: 206d 7573 7420 6265 2065 7870 7265 7373   must be express
+00007480: 6564 2061 7320 6672 6163 7469 6f6e 2028  ed as fraction (
+00007490: 6265 7477 6565 6e20 3020 616e 6420 3120  between 0 and 1 
+000074a0: 696e 636c 7573 6976 6529 2e27 2c20 6c6f  inclusive).', lo
+000074b0: 6767 6572 290a 0a20 2020 2020 2020 2023  gger)..        #
+000074c0: 2063 6f6c 756d 6e20 6e61 6d65 730a 2020   column names.  
+000074d0: 2020 2020 2020 636e 616d 6573 203d 205b        cnames = [
+000074e0: 7320 2b20 275f 7b7d 272e 666f 726d 6174  s + '_{}'.format
+000074f0: 2871 7561 6e74 696c 6529 2066 6f72 2073  (quantile) for s
+00007500: 2069 6e20 7365 6c66 2e63 6f6c 756d 6e73   in self.columns
+00007510: 5d0a 0a20 2020 2020 2020 2072 6574 7572  ]..        retur
+00007520: 6e20 7064 2e44 6174 6146 7261 6d65 2873  n pd.DataFrame(s
+00007530: 656c 662e 5f78 612e 7175 616e 7469 6c65  elf._xa.quantile
+00007540: 2871 3d71 7561 6e74 696c 652c 2064 696d  (q=quantile, dim
+00007550: 3d44 494d 535b 325d 292c 0a20 2020 2020  =DIMS[2]),.     
+00007560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007570: 2020 2020 2020 2069 6e64 6578 3d73 656c         index=sel
+00007580: 662e 5f74 696d 655f 696e 6465 782c 0a20  f._time_index,. 
+00007590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000075a0: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
+000075b0: 6e73 3d63 6e61 6d65 7329 0a0a 2020 2020  ns=cnames)..    
+000075c0: 6465 6620 7175 616e 7469 6c65 5f74 696d  def quantile_tim
+000075d0: 6573 6572 6965 7328 7365 6c66 2c20 7175  eseries(self, qu
+000075e0: 616e 7469 6c65 3d30 2e35 2920 2d3e 2027  antile=0.5) -> '
+000075f0: 5469 6d65 5365 7269 6573 273a 0a20 2020  TimeSeries':.   
+00007600: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00007610: 2052 6574 7572 6e73 2061 2064 6574 6572   Returns a deter
+00007620: 6d69 6e69 7374 6963 2060 5469 6d65 5365  ministic `TimeSe
+00007630: 7269 6573 6020 636f 6e74 6169 6e69 6e67  ries` containing
+00007640: 2074 6865 2073 696e 676c 6520 6465 7369   the single desi
+00007650: 7265 6420 7175 616e 7469 6c65 206f 6620  red quantile of 
+00007660: 6561 6368 2063 6f6d 706f 6e65 6e74 0a20  each component. 
+00007670: 2020 2020 2020 2028 6f76 6572 2074 6865         (over the
+00007680: 2073 616d 706c 6573 2920 6f66 2074 6869   samples) of thi
+00007690: 7320 7374 6f63 6861 7374 6963 2060 5469  s stochastic `Ti
+000076a0: 6d65 5365 7269 6573 602e 0a20 2020 2020  meSeries`..     
+000076b0: 2020 2054 6865 2063 6f6d 706f 6e65 6e74     The component
+000076c0: 7320 696e 2074 6865 206e 6577 2073 6572  s in the new ser
+000076d0: 6965 7320 6172 6520 6e61 6d65 6420 223c  ies are named "<
+000076e0: 636f 6d70 6f6e 656e 743e 5f58 222c 2077  component>_X", w
+000076f0: 6865 7265 2022 3c63 6f6d 706f 6e65 6e74  here "<component
+00007700: 3e22 0a20 2020 2020 2020 2069 7320 7468  >".        is th
+00007710: 6520 636f 6c75 6d6e 206e 616d 6520 636f  e column name co
+00007720: 7272 6573 706f 6e64 696e 6720 746f 2074  rresponding to t
+00007730: 6869 7320 636f 6d70 6f6e 656e 742c 2061  his component, a
+00007740: 6e64 2022 5822 2069 7320 7468 6520 7175  nd "X" is the qu
+00007750: 616e 7469 6c65 2076 616c 7565 2e0a 2020  antile value..  
+00007760: 2020 2020 2020 5468 6520 7175 616e 7469        The quanti
+00007770: 6c65 2063 6f6c 756d 6e73 2072 6570 7265  le columns repre
+00007780: 7365 6e74 2074 6865 206d 6172 6769 6e61  sent the margina
+00007790: 6c20 6469 7374 7269 6275 7469 6f6e 7320  l distributions 
+000077a0: 6f66 2074 6865 2063 6f6d 706f 6e65 6e74  of the component
+000077b0: 7320 6f66 2074 6869 7320 7365 7269 6573  s of this series
+000077c0: 2e0a 0a20 2020 2020 2020 2054 6869 7320  ...        This 
+000077d0: 776f 726b 7320 6f6e 6c79 206f 6e20 7374  works only on st
+000077e0: 6f63 6861 7374 6963 2073 6572 6965 7320  ochastic series 
+000077f0: 2869 2e65 2e2c 2077 6974 6820 6d6f 7265  (i.e., with more
+00007800: 2074 6861 6e20 3120 7361 6d70 6c65 290a   than 1 sample).
+00007810: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00007820: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+00007830: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2071  ------.        q
+00007840: 7561 6e74 696c 650a 2020 2020 2020 2020  uantile.        
+00007850: 2020 2020 5468 6520 6465 7369 7265 6420      The desired 
+00007860: 7175 616e 7469 6c65 2076 616c 7565 2e20  quantile value. 
+00007870: 5468 6520 7661 6c75 6520 6d75 7374 2062  The value must b
+00007880: 6520 7265 7072 6573 656e 7465 6420 6173  e represented as
+00007890: 2061 2066 7261 6374 696f 6e0a 2020 2020   a fraction.    
+000078a0: 2020 2020 2020 2020 2862 6574 7765 656e          (between
+000078b0: 2030 2061 6e64 2031 2069 6e63 6c75 7369   0 and 1 inclusi
+000078c0: 7665 292e 2046 6f72 2069 6e73 7461 6e63  ve). For instanc
+000078d0: 652c 2060 302e 3560 2077 696c 6c20 7265  e, `0.5` will re
+000078e0: 7475 726e 2061 2054 696d 6553 6572 6965  turn a TimeSerie
+000078f0: 730a 2020 2020 2020 2020 2020 2020 636f  s.            co
+00007900: 6e74 6169 6e69 6e67 2074 6865 206d 6564  ntaining the med
+00007910: 6961 6e20 6f66 2074 6865 2028 6d61 7267  ian of the (marg
+00007920: 696e 616c 2920 6469 7374 7269 6275 7469  inal) distributi
+00007930: 6f6e 206f 6620 6561 6368 2063 6f6d 706f  on of each compo
+00007940: 6e65 6e74 2e0a 0a20 2020 2020 2020 2052  nent...        R
+00007950: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+00007960: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2054  ------.        T
+00007970: 696d 6553 6572 6965 730a 2020 2020 2020  imeSeries.      
+00007980: 2020 2020 2020 5468 6520 5469 6d65 5365        The TimeSe
+00007990: 7269 6573 2063 6f6e 7461 696e 696e 6720  ries containing 
+000079a0: 7468 6520 6465 7369 7265 6420 7175 616e  the desired quan
+000079b0: 7469 6c65 2066 6f72 2065 6163 6820 636f  tile for each co
+000079c0: 6d70 6f6e 656e 742e 0a20 2020 2020 2020  mponent..       
+000079d0: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
+000079e0: 7572 6e20 5469 6d65 5365 7269 6573 2e66  urn TimeSeries.f
+000079f0: 726f 6d5f 6461 7461 6672 616d 6528 7365  rom_dataframe(se
+00007a00: 6c66 2e71 7561 6e74 696c 655f 6466 2871  lf.quantile_df(q
+00007a10: 7561 6e74 696c 6529 290a 0a20 2020 2064  uantile))..    d
+00007a20: 6566 2071 7561 6e74 696c 6573 5f64 6628  ef quantiles_df(
+00007a30: 7365 6c66 2c20 7175 616e 7469 6c65 733a  self, quantiles:
+00007a40: 2054 7570 6c65 5b66 6c6f 6174 5d20 3d20   Tuple[float] = 
+00007a50: 2830 2e31 2c20 302e 352c 2030 2e39 2929  (0.1, 0.5, 0.9))
+00007a60: 202d 3e20 7064 2e44 6174 6146 7261 6d65   -> pd.DataFrame
+00007a70: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00007a80: 2020 2020 2020 5265 7475 726e 7320 6120        Returns a 
+00007a90: 5061 6e64 6173 2044 6174 6146 7261 6d65  Pandas DataFrame
+00007aa0: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
+00007ab0: 6465 7369 7265 6420 7175 616e 7469 6c65  desired quantile
+00007ac0: 7320 6f66 2065 6163 6820 636f 6d70 6f6e  s of each compon
+00007ad0: 656e 7420 286f 7665 7220 7468 6520 7361  ent (over the sa
+00007ae0: 6d70 6c65 7329 2e0a 2020 2020 2020 2020  mples)..        
+00007af0: 4561 6368 206f 6620 7468 6520 7365 7269  Each of the seri
+00007b00: 6573 2063 6f6d 706f 6e65 6e74 7320 7769  es components wi
+00007b10: 6c6c 2061 7070 6561 7220 6173 2061 2063  ll appear as a c
+00007b20: 6f6c 756d 6e20 696e 2074 6865 2044 6174  olumn in the Dat
+00007b30: 6146 7261 6d65 2e20 5468 6520 636f 6c75  aFrame. The colu
+00007b40: 6d6e 2077 696c 6c20 6265 206e 616d 6564  mn will be named
+00007b50: 0a20 2020 2020 2020 2022 3c63 6f6d 706f  .        "<compo
+00007b60: 6e65 6e74 3e5f 5822 2c20 7768 6572 6520  nent>_X", where 
+00007b70: 223c 636f 6d70 6f6e 656e 743e 2220 6973  "<component>" is
+00007b80: 2074 6865 2063 6f6c 756d 6e20 6e61 6d65   the column name
+00007b90: 2063 6f72 7265 7370 6f6e 6469 6e67 2074   corresponding t
+00007ba0: 6f20 7468 6973 2063 6f6d 706f 6e65 6e74  o this component
+00007bb0: 2c20 616e 6420 2258 220a 2020 2020 2020  , and "X".      
+00007bc0: 2020 6973 2074 6865 2071 7561 6e74 696c    is the quantil
+00007bd0: 6520 7661 6c75 652e 0a20 2020 2020 2020  e value..       
+00007be0: 2054 6865 2071 7561 6e74 696c 6573 2072   The quantiles r
+00007bf0: 6570 7265 7365 6e74 2074 6865 206d 6172  epresent the mar
+00007c00: 6769 6e61 6c20 6469 7374 7269 6275 7469  ginal distributi
+00007c10: 6f6e 7320 6f66 2074 6865 2063 6f6d 706f  ons of the compo
+00007c20: 6e65 6e74 7320 6f66 2074 6869 7320 7365  nents of this se
+00007c30: 7269 6573 2e0a 0a20 2020 2020 2020 2054  ries...        T
+00007c40: 6869 7320 776f 726b 7320 6f6e 6c79 206f  his works only o
+00007c50: 6e20 7374 6f63 6861 7374 6963 2073 6572  n stochastic ser
+00007c60: 6965 7320 2869 2e65 2e2c 2077 6974 6820  ies (i.e., with 
+00007c70: 6d6f 7265 2074 6861 6e20 3120 7361 6d70  more than 1 samp
+00007c80: 6c65 290a 0a20 2020 2020 2020 2050 6172  le)..        Par
+00007c90: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+00007ca0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00007cb0: 2020 2071 7561 6e74 696c 6573 0a20 2020     quantiles.   
+00007cc0: 2020 2020 2020 2020 2054 7570 6c65 2063           Tuple c
+00007cd0: 6f6e 7461 696e 696e 6720 7468 6520 6465  ontaining the de
+00007ce0: 7369 7265 6420 7175 616e 7469 6c65 732e  sired quantiles.
+00007cf0: 2054 6865 2076 616c 7565 7320 6d75 7374   The values must
+00007d00: 2062 6520 7265 7072 6573 656e 7465 6420   be represented 
+00007d10: 6173 2066 7261 6374 696f 6e73 0a20 2020  as fractions.   
+00007d20: 2020 2020 2020 2020 2028 6265 7477 6565           (betwee
+00007d30: 6e20 3020 616e 6420 3120 696e 636c 7573  n 0 and 1 inclus
+00007d40: 6976 6529 2e20 466f 7220 696e 7374 616e  ive). For instan
+00007d50: 6365 2c20 6028 302e 312c 2030 2e35 2c20  ce, `(0.1, 0.5, 
+00007d60: 302e 3929 6020 7769 6c6c 2072 6574 7572  0.9)` will retur
+00007d70: 6e20 6120 4461 7461 4672 616d 650a 2020  n a DataFrame.  
+00007d80: 2020 2020 2020 2020 2020 636f 6e74 6169            contai
+00007d90: 6e69 6e67 2074 6865 2031 3074 682d 7065  ning the 10th-pe
+00007da0: 7263 656e 7469 6c65 2c20 6d65 6469 616e  rcentile, median
+00007db0: 2061 6e64 2039 3074 682d 7065 7263 656e   and 90th-percen
+00007dc0: 7469 6c65 206f 6620 7468 6520 286d 6172  tile of the (mar
+00007dd0: 6769 6e61 6c29 2064 6973 7472 6962 7574  ginal) distribut
+00007de0: 696f 6e20 6f66 2065 6163 6820 636f 6d70  ion of each comp
+00007df0: 6f6e 656e 742e 0a0a 2020 2020 2020 2020  onent...        
+00007e00: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+00007e10: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00007e20: 7061 6e64 6173 2e44 6174 6146 7261 6d65  pandas.DataFrame
+00007e30: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+00007e40: 2050 616e 6461 7320 4461 7461 4672 616d   Pandas DataFram
+00007e50: 6520 636f 6e74 6169 6e69 6e67 2074 6865  e containing the
+00007e60: 2071 7561 6e74 696c 6573 2066 6f72 2065   quantiles for e
+00007e70: 6163 6820 636f 6d70 6f6e 656e 742e 0a20  ach component.. 
+00007e80: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00007e90: 2020 2023 2054 4f44 4f3a 2074 6865 7265     # TODO: there
+00007ea0: 206d 6967 6874 2062 6520 6120 736c 6967   might be a slig
+00007eb0: 6874 6c79 206d 6f72 6520 6566 6669 6369  htly more effici
+00007ec0: 656e 7420 7761 7920 746f 2064 6f20 6974  ent way to do it
+00007ed0: 2066 6f72 2073 6576 6572 616c 2071 7561   for several qua
+00007ee0: 6e74 696c 6573 2061 7420 6f6e 6365 2077  ntiles at once w
+00007ef0: 6974 6820 7861 7272 6179 2e2e 2e0a 2020  ith xarray....  
+00007f00: 2020 2020 2020 7265 7475 726e 2070 642e        return pd.
+00007f10: 636f 6e63 6174 285b 7365 6c66 2e71 7561  concat([self.qua
+00007f20: 6e74 696c 655f 6466 2871 7561 6e74 696c  ntile_df(quantil
+00007f30: 6529 2066 6f72 2071 7561 6e74 696c 6520  e) for quantile 
+00007f40: 696e 2071 7561 6e74 696c 6573 5d2c 2061  in quantiles], a
+00007f50: 7869 733d 3129 0a0a 2020 2020 6465 6620  xis=1)..    def 
+00007f60: 7374 6172 745f 7469 6d65 2873 656c 6629  start_time(self)
+00007f70: 202d 3e20 556e 696f 6e5b 7064 2e54 696d   -> Union[pd.Tim
+00007f80: 6573 7461 6d70 2c20 696e 745d 3a0a 2020  estamp, int]:.  
+00007f90: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00007fa0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+00007fb0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+00007fc0: 2020 556e 696f 6e5b 7061 6e64 6173 2e54    Union[pandas.T
+00007fd0: 696d 6573 7461 6d70 2c20 696e 745d 0a20  imestamp, int]. 
+00007fe0: 2020 2020 2020 2020 2020 2041 2074 696d             A tim
+00007ff0: 6573 7461 6d70 2063 6f6e 7461 696e 696e  estamp containin
+00008000: 6720 7468 6520 6669 7273 7420 7469 6d65  g the first time
+00008010: 206f 6620 7468 6520 5469 6d65 5365 7269   of the TimeSeri
+00008020: 6573 2028 6966 2069 6e64 6578 6564 2062  es (if indexed b
+00008030: 7920 4461 7465 7469 6d65 496e 6465 7829  y DatetimeIndex)
+00008040: 2c0a 2020 2020 2020 2020 2020 2020 6f72  ,.            or
+00008050: 2061 6e20 696e 7465 6765 7220 2869 6620   an integer (if 
+00008060: 696e 6465 7865 6420 6279 2049 6e74 3634  indexed by Int64
+00008070: 496e 6465 782f 5261 6e67 6549 6e64 6578  Index/RangeIndex
+00008080: 290a 2020 2020 2020 2020 2222 220a 2020  ).        """.  
+00008090: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000080a0: 662e 5f74 696d 655f 696e 6465 785b 305d  f._time_index[0]
+000080b0: 0a0a 2020 2020 6465 6620 656e 645f 7469  ..    def end_ti
+000080c0: 6d65 2873 656c 6629 202d 3e20 556e 696f  me(self) -> Unio
+000080d0: 6e5b 7064 2e54 696d 6573 7461 6d70 2c20  n[pd.Timestamp, 
+000080e0: 696e 745d 3a0a 2020 2020 2020 2020 2222  int]:.        ""
+000080f0: 220a 2020 2020 2020 2020 5265 7475 726e  ".        Return
+00008100: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00008110: 2d0a 2020 2020 2020 2020 556e 696f 6e5b  -.        Union[
+00008120: 7061 6e64 6173 2e54 696d 6573 7461 6d70  pandas.Timestamp
+00008130: 2c20 696e 745d 0a20 2020 2020 2020 2020  , int].         
+00008140: 2020 2041 2074 696d 6573 7461 6d70 2063     A timestamp c
+00008150: 6f6e 7461 696e 696e 6720 7468 6520 6c61  ontaining the la
+00008160: 7374 2074 696d 6520 6f66 2074 6865 2054  st time of the T
+00008170: 696d 6553 6572 6965 7320 2869 6620 696e  imeSeries (if in
+00008180: 6465 7865 6420 6279 2044 6174 6574 696d  dexed by Datetim
+00008190: 6549 6e64 6578 292c 0a20 2020 2020 2020  eIndex),.       
+000081a0: 2020 2020 206f 7220 616e 2069 6e74 6567       or an integ
+000081b0: 6572 2028 6966 2069 6e64 6578 6564 2062  er (if indexed b
+000081c0: 7920 496e 7436 3449 6e64 6578 2f52 616e  y Int64Index/Ran
+000081d0: 6765 496e 6465 7829 0a20 2020 2020 2020  geIndex).       
+000081e0: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
+000081f0: 7572 6e20 7365 6c66 2e5f 7469 6d65 5f69  urn self._time_i
+00008200: 6e64 6578 5b2d 315d 0a0a 2020 2020 6465  ndex[-1]..    de
+00008210: 6620 6669 7273 745f 7661 6c75 6528 7365  f first_value(se
+00008220: 6c66 2920 2d3e 2066 6c6f 6174 3a0a 2020  lf) -> float:.  
+00008230: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00008240: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+00008250: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+00008260: 2020 666c 6f61 740a 2020 2020 2020 2020    float.        
+00008270: 2020 2020 5468 6520 6669 7273 7420 7661      The first va
+00008280: 6c75 6520 6f66 2074 6869 7320 756e 6976  lue of this univ
+00008290: 6172 6961 7465 2064 6574 6572 6d69 6e69  ariate determini
+000082a0: 7374 6963 2074 696d 6520 7365 7269 6573  stic time series
+000082b0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000082c0: 2020 2020 2073 656c 662e 5f61 7373 6572       self._asser
+000082d0: 745f 756e 6976 6172 6961 7465 2829 0a20  t_univariate(). 
+000082e0: 2020 2020 2020 2073 656c 662e 5f61 7373         self._ass
+000082f0: 6572 745f 6465 7465 726d 696e 6973 7469  ert_deterministi
+00008300: 6328 290a 2020 2020 2020 2020 7265 7475  c().        retu
+00008310: 726e 2066 6c6f 6174 2873 656c 662e 5f78  rn float(self._x
+00008320: 615b 302c 2030 2c20 305d 290a 0a20 2020  a[0, 0, 0])..   
+00008330: 2064 6566 206c 6173 745f 7661 6c75 6528   def last_value(
+00008340: 7365 6c66 2920 2d3e 2066 6c6f 6174 3a0a  self) -> float:.
+00008350: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00008360: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+00008370: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00008380: 2020 2020 666c 6f61 740a 2020 2020 2020      float.      
+00008390: 2020 2020 2020 5468 6520 6c61 7374 2076        The last v
+000083a0: 616c 7565 206f 6620 7468 6973 2075 6e69  alue of this uni
+000083b0: 7661 7269 6174 6520 6465 7465 726d 696e  variate determin
+000083c0: 6973 7469 6320 7469 6d65 2073 6572 6965  istic time serie
+000083d0: 730a 2020 2020 2020 2020 2222 220a 2020  s.        """.  
+000083e0: 2020 2020 2020 7365 6c66 2e5f 6173 7365        self._asse
+000083f0: 7274 5f75 6e69 7661 7269 6174 6528 290a  rt_univariate().
+00008400: 2020 2020 2020 2020 7365 6c66 2e5f 6173          self._as
+00008410: 7365 7274 5f64 6574 6572 6d69 6e69 7374  sert_determinist
+00008420: 6963 2829 0a20 2020 2020 2020 2072 6574  ic().        ret
+00008430: 7572 6e20 666c 6f61 7428 7365 6c66 2e5f  urn float(self._
+00008440: 7861 5b2d 312c 2030 2c20 305d 290a 0a20  xa[-1, 0, 0]).. 
+00008450: 2020 2064 6566 2066 6972 7374 5f76 616c     def first_val
+00008460: 7565 7328 7365 6c66 2920 2d3e 206e 702e  ues(self) -> np.
+00008470: 6e64 6172 7261 793a 0a20 2020 2020 2020  ndarray:.       
+00008480: 2022 2222 0a20 2020 2020 2020 2052 6574   """.        Ret
+00008490: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+000084a0: 2d2d 2d2d 0a20 2020 2020 2020 206e 702e  ----.        np.
+000084b0: 6e64 6172 7261 790a 2020 2020 2020 2020  ndarray.        
+000084c0: 2020 2020 5468 6520 6669 7273 7420 7661      The first va
+000084d0: 6c75 6573 206f 6620 6576 6572 7920 636f  lues of every co
+000084e0: 6d70 6f6e 656e 7420 6f66 2074 6869 7320  mponent of this 
+000084f0: 6465 7465 726d 696e 6973 7469 6320 7469  deterministic ti
+00008500: 6d65 2073 6572 6965 730a 2020 2020 2020  me series.      
+00008510: 2020 2222 220a 2020 2020 2020 2020 7365    """.        se
+00008520: 6c66 2e5f 6173 7365 7274 5f64 6574 6572  lf._assert_deter
+00008530: 6d69 6e69 7374 6963 2829 0a20 2020 2020  ministic().     
+00008540: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00008550: 7861 2e76 616c 7565 735b 302c 203a 2c20  xa.values[0, :, 
+00008560: 305d 2e63 6f70 7928 290a 0a20 2020 2064  0].copy()..    d
+00008570: 6566 206c 6173 745f 7661 6c75 6573 2873  ef last_values(s
+00008580: 656c 6629 202d 3e20 6e70 2e6e 6461 7272  elf) -> np.ndarr
+00008590: 6179 3a0a 2020 2020 2020 2020 2222 220a  ay:.        """.
+000085a0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+000085b0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+000085c0: 2020 2020 2020 2020 6e70 2e6e 6461 7272          np.ndarr
+000085d0: 6179 0a20 2020 2020 2020 2020 2020 2054  ay.            T
+000085e0: 6865 206c 6173 7420 7661 6c75 6573 206f  he last values o
+000085f0: 6620 6576 6572 7920 636f 6d70 6f6e 656e  f every componen
+00008600: 7420 6f66 2074 6869 7320 6465 7465 726d  t of this determ
+00008610: 696e 6973 7469 6320 7469 6d65 2073 6572  inistic time ser
+00008620: 6965 730a 2020 2020 2020 2020 2222 220a  ies.        """.
+00008630: 2020 2020 2020 2020 7365 6c66 2e5f 6173          self._as
+00008640: 7365 7274 5f64 6574 6572 6d69 6e69 7374  sert_determinist
+00008650: 6963 2829 0a20 2020 2020 2020 2072 6574  ic().        ret
+00008660: 7572 6e20 7365 6c66 2e5f 7861 2e76 616c  urn self._xa.val
+00008670: 7565 735b 2d31 2c20 3a2c 2030 5d2e 636f  ues[-1, :, 0].co
+00008680: 7079 2829 0a0a 2020 2020 6465 6620 7661  py()..    def va
+00008690: 6c75 6573 2873 656c 662c 2063 6f70 793d  lues(self, copy=
+000086a0: 5472 7565 2c20 7361 6d70 6c65 3d30 2920  True, sample=0) 
+000086b0: 2d3e 206e 702e 6e64 6172 7261 793a 0a20  -> np.ndarray:. 
+000086c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000086d0: 2020 2052 6574 7572 6e73 2061 2032 2d44     Returns a 2-D
+000086e0: 204e 756d 7079 2061 7272 6179 206f 6620   Numpy array of 
+000086f0: 6469 6d65 6e73 696f 6e20 2874 696d 652c  dimension (time,
+00008700: 2063 6f6d 706f 6e65 6e74 292c 2063 6f6e   component), con
+00008710: 7461 696e 696e 6720 7468 6973 2073 6572  taining this ser
+00008720: 6965 7327 2076 616c 7565 7320 666f 7220  ies' values for 
+00008730: 6f6e 6520 7361 6d70 6c65 2e0a 2020 2020  one sample..    
+00008740: 2020 2020 4966 2074 6869 7320 7365 7269      If this seri
+00008750: 6573 2069 7320 6465 7465 726d 696e 6973  es is determinis
+00008760: 7469 632c 2069 7420 636f 6e74 6169 6e73  tic, it contains
+00008770: 206f 6e6c 7920 6f6e 6520 7361 6d70 6c65   only one sample
+00008780: 2061 6e64 206f 6e6c 7920 6073 616d 706c   and only `sampl
+00008790: 653d 3060 2063 616e 2062 6520 7573 6564  e=0` can be used
+000087a0: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+000087b0: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+000087c0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+000087d0: 2063 6f70 790a 2020 2020 2020 2020 2020   copy.          
+000087e0: 2020 5768 6574 6865 7220 746f 2072 6574    Whether to ret
+000087f0: 7572 6e20 6120 636f 7079 206f 6620 7468  urn a copy of th
+00008800: 6520 7661 6c75 6573 2c20 6f74 6865 7277  e values, otherw
+00008810: 6973 6520 7265 7475 726e 7320 6120 7669  ise returns a vi
+00008820: 6577 2e0a 2020 2020 2020 2020 2020 2020  ew..            
+00008830: 4c65 6176 6520 6974 2074 6f20 5472 7565  Leave it to True
+00008840: 2075 6e6c 6573 7320 796f 7520 6b6e 6f77   unless you know
+00008850: 2077 6861 7420 796f 7520 6172 6520 646f   what you are do
+00008860: 696e 672e 0a0a 2020 2020 2020 2020 5265  ing...        Re
+00008870: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+00008880: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6e75  -----.        nu
+00008890: 6d70 792e 6e64 6172 7261 790a 2020 2020  mpy.ndarray.    
+000088a0: 2020 2020 2020 2020 5468 6520 7661 6c75          The valu
+000088b0: 6573 2063 6f6d 706f 7369 6e67 2074 6865  es composing the
+000088c0: 2074 696d 6520 7365 7269 6573 2e0a 2020   time series..  
+000088d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000088e0: 2020 7261 6973 655f 6966 2873 656c 662e    raise_if(self.
+000088f0: 6973 5f64 6574 6572 6d69 6e69 7374 6963  is_deterministic
+00008900: 2061 6e64 2073 616d 706c 6520 213d 2030   and sample != 0
+00008910: 2c20 2754 6869 7320 7365 7269 6573 2063  , 'This series c
+00008920: 6f6e 7461 696e 7320 6f6e 6520 7361 6d70  ontains one samp
+00008930: 6c65 206f 6e6c 7920 2864 6574 6572 6d69  le only (determi
+00008940: 6e69 7374 6963 292c 270a 2020 2020 2020  nistic),'.      
+00008950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008980: 2020 2773 6f20 6f6e 6c79 2073 616d 706c    'so only sampl
+00008990: 653d 3020 6973 2061 6363 6570 7465 642e  e=0 is accepted.
+000089a0: 272c 206c 6f67 6765 7229 0a20 2020 2020  ', logger).     
+000089b0: 2020 2069 6620 636f 7079 3a0a 2020 2020     if copy:.    
+000089c0: 2020 2020 2020 2020 7265 7475 726e 206e          return n
+000089d0: 702e 636f 7079 2873 656c 662e 5f78 612e  p.copy(self._xa.
+000089e0: 7661 6c75 6573 5b3a 2c20 3a2c 2073 616d  values[:, :, sam
+000089f0: 706c 655d 290a 2020 2020 2020 2020 656c  ple]).        el
+00008a00: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00008a10: 7265 7475 726e 2073 656c 662e 5f78 612e  return self._xa.
+00008a20: 7661 6c75 6573 5b3a 2c20 3a2c 2073 616d  values[:, :, sam
+00008a30: 706c 655d 0a0a 2020 2020 6465 6620 616c  ple]..    def al
+00008a40: 6c5f 7661 6c75 6573 2873 656c 662c 2063  l_values(self, c
+00008a50: 6f70 793d 5472 7565 2920 2d3e 206e 702e  opy=True) -> np.
+00008a60: 6e64 6172 7261 793a 0a20 2020 2020 2020  ndarray:.       
+00008a70: 2022 2222 0a20 2020 2020 2020 2052 6574   """.        Ret
+00008a80: 7572 6e73 2061 2033 2d44 204e 756d 7079  urns a 3-D Numpy
+00008a90: 2061 7272 6179 206f 6620 6469 6d65 6e73   array of dimens
+00008aa0: 696f 6e20 2874 696d 652c 2063 6f6d 706f  ion (time, compo
+00008ab0: 6e65 6e74 2c20 7361 6d70 6c65 292c 0a20  nent, sample),. 
+00008ac0: 2020 2020 2020 2063 6f6e 7461 696e 696e         containin
+00008ad0: 6720 7468 6973 2073 6572 6965 7327 2076  g this series' v
+00008ae0: 616c 7565 7320 666f 7220 616c 6c20 7361  alues for all sa
+00008af0: 6d70 6c65 732e 0a0a 2020 2020 2020 2020  mples...        
+00008b00: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+00008b10: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00008b20: 2020 2020 2020 636f 7079 0a20 2020 2020        copy.     
+00008b30: 2020 2020 2020 2057 6865 7468 6572 2074         Whether t
+00008b40: 6f20 7265 7475 726e 2061 2063 6f70 7920  o return a copy 
+00008b50: 6f66 2074 6865 2076 616c 7565 732c 206f  of the values, o
+00008b60: 7468 6572 7769 7365 2072 6574 7572 6e73  therwise returns
+00008b70: 2061 2076 6965 772e 0a20 2020 2020 2020   a view..       
+00008b80: 2020 2020 204c 6561 7665 2069 7420 746f       Leave it to
+00008b90: 2054 7275 6520 756e 6c65 7373 2079 6f75   True unless you
+00008ba0: 206b 6e6f 7720 7768 6174 2079 6f75 2061   know what you a
+00008bb0: 7265 2064 6f69 6e67 2e0a 0a20 2020 2020  re doing...     
+00008bc0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+00008bd0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+00008be0: 2020 206e 756d 7079 2e6e 6461 7272 6179     numpy.ndarray
+00008bf0: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+00008c00: 2076 616c 7565 7320 636f 6d70 6f73 696e   values composin
+00008c10: 6720 7468 6520 7469 6d65 2073 6572 6965  g the time serie
+00008c20: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+00008c30: 2020 2020 2020 2069 6620 636f 7079 3a0a         if copy:.
+00008c40: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00008c50: 726e 206e 702e 636f 7079 2873 656c 662e  rn np.copy(self.
+00008c60: 5f78 612e 7661 6c75 6573 290a 2020 2020  _xa.values).    
+00008c70: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00008c80: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00008c90: 662e 5f78 612e 7661 6c75 6573 0a0a 2020  f._xa.values..  
+00008ca0: 2020 6465 6620 756e 6976 6172 6961 7465    def univariate
+00008cb0: 5f76 616c 7565 7328 7365 6c66 2c20 636f  _values(self, co
+00008cc0: 7079 3d54 7275 652c 2073 616d 706c 653d  py=True, sample=
+00008cd0: 3029 202d 3e20 6e70 2e6e 6461 7272 6179  0) -> np.ndarray
+00008ce0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00008cf0: 2020 2020 2020 5265 7475 726e 7320 6120        Returns a 
+00008d00: 312d 4420 4e75 6d70 7920 6172 7261 7920  1-D Numpy array 
+00008d10: 6f66 2064 696d 656e 7369 6f6e 2028 7469  of dimension (ti
+00008d20: 6d65 2c29 2c20 636f 6e74 6169 6e69 6e67  me,), containing
+00008d30: 2074 6869 7320 756e 6976 6172 6961 7465   this univariate
+00008d40: 2073 6572 6965 7327 2076 616c 7565 7320   series' values 
+00008d50: 666f 7220 6f6e 6520 7361 6d70 6c65 2e0a  for one sample..
+00008d60: 2020 2020 2020 2020 4966 2074 6869 7320          If this 
+00008d70: 7365 7269 6573 2069 7320 6465 7465 726d  series is determ
+00008d80: 696e 6973 7469 632c 2069 7420 636f 6e74  inistic, it cont
+00008d90: 6169 6e73 206f 6e6c 7920 6f6e 6520 7361  ains only one sa
+00008da0: 6d70 6c65 2061 6e64 206f 6e6c 7920 6073  mple and only `s
+00008db0: 616d 706c 653d 3060 2063 616e 2062 6520  ample=0` can be 
+00008dc0: 7573 6564 2e0a 0a20 2020 2020 2020 2050  used...        P
+00008dd0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00008de0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00008df0: 2020 2020 2063 6f70 790a 2020 2020 2020       copy.      
+00008e00: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
+00008e10: 2072 6574 7572 6e20 6120 636f 7079 206f   return a copy o
+00008e20: 6620 7468 6520 7661 6c75 6573 2e20 4c65  f the values. Le
+00008e30: 6176 6520 6974 2074 6f20 5472 7565 2075  ave it to True u
+00008e40: 6e6c 6573 7320 796f 7520 6b6e 6f77 2077  nless you know w
+00008e50: 6861 7420 796f 7520 6172 6520 646f 696e  hat you are doin
+00008e60: 672e 0a0a 2020 2020 2020 2020 5265 7475  g...        Retu
+00008e70: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+00008e80: 2d2d 2d0a 2020 2020 2020 2020 6e75 6d70  ---.        nump
+00008e90: 792e 6e64 6172 7261 790a 2020 2020 2020  y.ndarray.      
+00008ea0: 2020 2020 2020 5468 6520 7661 6c75 6573        The values
+00008eb0: 2063 6f6d 706f 7369 6e67 2074 6865 2074   composing the t
+00008ec0: 696d 6520 7365 7269 6573 2067 7561 7261  ime series guara
+00008ed0: 6e74 6565 6420 746f 2062 6520 756e 6976  nteed to be univ
+00008ee0: 6172 6961 7465 2e0a 2020 2020 2020 2020  ariate..        
+00008ef0: 2222 220a 0a20 2020 2020 2020 2073 656c  """..        sel
+00008f00: 662e 5f61 7373 6572 745f 756e 6976 6172  f._assert_univar
+00008f10: 6961 7465 2829 0a20 2020 2020 2020 2069  iate().        i
+00008f20: 6620 636f 7079 3a0a 2020 2020 2020 2020  f copy:.        
+00008f30: 2020 2020 7265 7475 726e 206e 702e 636f      return np.co
+00008f40: 7079 2873 656c 662e 5f78 615b 3a2c 2030  py(self._xa[:, 0
+00008f50: 2c20 7361 6d70 6c65 5d2e 7661 6c75 6573  , sample].values
+00008f60: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00008f70: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00008f80: 726e 2073 656c 662e 5f78 615b 3a2c 2030  rn self._xa[:, 0
+00008f90: 2c20 7361 6d70 6c65 5d2e 7661 6c75 6573  , sample].values
+00008fa0: 0a0a 2020 2020 2222 220a 2020 2020 4f74  ..    """.    Ot
+00008fb0: 6865 7220 6d65 7468 6f64 730a 2020 2020  her methods.    
+00008fc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020  =============.  
+00008fd0: 2020 2222 220a 0a20 2020 2064 6566 2067    """..    def g
+00008fe0: 6170 7328 7365 6c66 2920 2d3e 2070 642e  aps(self) -> pd.
+00008ff0: 4461 7461 4672 616d 653a 0a20 2020 2020  DataFrame:.     
+00009000: 2020 2022 2222 0a20 2020 2020 2020 2041     """.        A
+00009010: 2066 756e 6374 696f 6e20 746f 2063 6f6d   function to com
+00009020: 7075 7465 2061 6e64 2072 6574 7572 6e20  pute and return 
+00009030: 6761 7073 2069 6e20 7468 6520 5469 6d65  gaps in the Time
+00009040: 5365 7269 6573 2e20 576f 726b 7320 6f6e  Series. Works on
+00009050: 6c79 206f 6e20 6465 7465 726d 696e 6973  ly on determinis
+00009060: 7469 6320 7469 6d65 2073 6572 6965 7320  tic time series 
+00009070: 2831 2073 616d 706c 6529 2e0a 0a20 2020  (1 sample)...   
+00009080: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+00009090: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+000090a0: 2020 2020 2070 642e 4461 7461 4672 616d       pd.DataFram
+000090b0: 650a 2020 2020 2020 2020 2020 2020 4120  e.            A 
+000090c0: 7061 6e64 6173 2e44 6174 6146 7261 6d65  pandas.DataFrame
+000090d0: 2063 6f6e 7461 696e 696e 6720 6120 726f   containing a ro
+000090e0: 7720 666f 7220 6576 6572 7920 6761 7020  w for every gap 
+000090f0: 2872 6f77 7320 7769 7468 2061 6c6c 2d4e  (rows with all-N
+00009100: 614e 2076 616c 7565 7320 696e 2075 6e64  aN values in und
+00009110: 6572 6c79 696e 6720 4461 7461 4672 616d  erlying DataFram
+00009120: 6529 0a20 2020 2020 2020 2020 2020 2069  e).            i
+00009130: 6e20 7468 6973 2074 696d 6520 7365 7269  n this time seri
+00009140: 6573 2e20 5468 6520 4461 7461 4672 616d  es. The DataFram
+00009150: 6520 636f 6e74 6169 6e73 2074 6872 6565  e contains three
+00009160: 2063 6f6c 756d 6e73 2074 6861 7420 696e   columns that in
+00009170: 636c 7564 6520 7468 6520 7374 6172 7420  clude the start 
+00009180: 616e 6420 656e 6420 7469 6d65 2073 7461  and end time sta
+00009190: 6d70 730a 2020 2020 2020 2020 2020 2020  mps.            
+000091a0: 6f66 2074 6865 2067 6170 2061 6e64 2074  of the gap and t
+000091b0: 6865 2069 6e74 6567 6572 206c 656e 6774  he integer lengt
+000091c0: 6820 6f66 2074 6865 2067 6170 2028 696e  h of the gap (in
+000091d0: 2060 7365 6c66 2e66 7265 7160 2075 6e69   `self.freq` uni
+000091e0: 7473 2069 6620 7468 6520 7365 7269 6573  ts if the series
+000091f0: 2069 7320 696e 6465 7865 640a 2020 2020   is indexed.    
+00009200: 2020 2020 2020 2020 6279 2061 2044 6174          by a Dat
+00009210: 6574 696d 6549 6e64 6578 292e 0a20 2020  etimeIndex)..   
+00009220: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00009230: 2020 6466 203d 2073 656c 662e 7064 5f64    df = self.pd_d
+00009240: 6174 6166 7261 6d65 2829 0a0a 2020 2020  ataframe()..    
+00009250: 2020 2020 6973 5f6e 616e 5f73 6572 6965      is_nan_serie
+00009260: 7320 3d20 6466 2e69 736e 6128 292e 616c  s = df.isna().al
+00009270: 6c28 6178 6973 3d31 292e 6173 7479 7065  l(axis=1).astype
+00009280: 2869 6e74 290a 2020 2020 2020 2020 6469  (int).        di
+00009290: 6666 203d 2070 642e 5365 7269 6573 286e  ff = pd.Series(n
+000092a0: 702e 6469 6666 2869 735f 6e61 6e5f 7365  p.diff(is_nan_se
+000092b0: 7269 6573 2e76 616c 7565 7329 2c20 696e  ries.values), in
+000092c0: 6465 783d 6973 5f6e 616e 5f73 6572 6965  dex=is_nan_serie
+000092d0: 732e 696e 6465 785b 3a2d 315d 290a 2020  s.index[:-1]).  
+000092e0: 2020 2020 2020 6761 705f 7374 6172 7473        gap_starts
+000092f0: 203d 2064 6966 665b 6469 6666 203d 3d20   = diff[diff == 
+00009300: 315d 2e69 6e64 6578 202b 2073 656c 662e  1].index + self.
+00009310: 5f66 7265 710a 2020 2020 2020 2020 6761  _freq.        ga
+00009320: 705f 656e 6473 203d 2064 6966 665b 6469  p_ends = diff[di
+00009330: 6666 203d 3d20 2d31 5d2e 696e 6465 780a  ff == -1].index.
+00009340: 0a20 2020 2020 2020 2069 6620 6973 5f6e  .        if is_n
+00009350: 616e 5f73 6572 6965 732e 696c 6f63 5b30  an_series.iloc[0
+00009360: 5d20 3d3d 2031 3a0a 2020 2020 2020 2020  ] == 1:.        
+00009370: 2020 2020 6761 705f 7374 6172 7473 203d      gap_starts =
+00009380: 2067 6170 5f73 7461 7274 732e 696e 7365   gap_starts.inse
+00009390: 7274 2830 2c20 7365 6c66 2e73 7461 7274  rt(0, self.start
+000093a0: 5f74 696d 6528 2929 0a20 2020 2020 2020  _time()).       
+000093b0: 2069 6620 6973 5f6e 616e 5f73 6572 6965   if is_nan_serie
+000093c0: 732e 696c 6f63 5b2d 315d 203d 3d20 313a  s.iloc[-1] == 1:
+000093d0: 0a20 2020 2020 2020 2020 2020 2067 6170  .            gap
+000093e0: 5f65 6e64 7320 3d20 6761 705f 656e 6473  _ends = gap_ends
+000093f0: 2e69 6e73 6572 7428 6c65 6e28 6761 705f  .insert(len(gap_
+00009400: 656e 6473 292c 2073 656c 662e 656e 645f  ends), self.end_
+00009410: 7469 6d65 2829 290a 0a20 2020 2020 2020  time())..       
+00009420: 2067 6170 5f64 6620 3d20 7064 2e44 6174   gap_df = pd.Dat
+00009430: 6146 7261 6d65 2829 0a20 2020 2020 2020  aFrame().       
+00009440: 2067 6170 5f64 665b 2767 6170 5f73 7461   gap_df['gap_sta
+00009450: 7274 275d 203d 2067 6170 5f73 7461 7274  rt'] = gap_start
+00009460: 730a 2020 2020 2020 2020 6761 705f 6466  s.        gap_df
+00009470: 5b27 6761 705f 656e 6427 5d20 3d20 6761  ['gap_end'] = ga
+00009480: 705f 656e 6473 0a0a 2020 2020 2020 2020  p_ends..        
+00009490: 6465 6620 696e 7476 6c28 7374 6172 742c  def intvl(start,
+000094a0: 2065 6e64 293a 0a20 2020 2020 2020 2020   end):.         
+000094b0: 2020 2069 6620 7365 6c66 2e5f 6861 735f     if self._has_
+000094c0: 6461 7465 7469 6d65 5f69 6e64 6578 3a0a  datetime_index:.
+000094d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094e0: 7265 7475 726e 2070 642e 6461 7465 5f72  return pd.date_r
+000094f0: 616e 6765 2873 7461 7274 3d73 7461 7274  ange(start=start
+00009500: 2c20 656e 643d 656e 642c 2066 7265 713d  , end=end, freq=
+00009510: 7365 6c66 2e5f 6672 6571 292e 7369 7a65  self._freq).size
+00009520: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00009530: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00009540: 2020 2072 6574 7572 6e20 7374 6172 7420     return start 
+00009550: 2d20 656e 640a 0a20 2020 2020 2020 2067  - end..        g
+00009560: 6170 5f64 665b 2767 6170 5f73 697a 6527  ap_df['gap_size'
+00009570: 5d20 3d20 6761 705f 6466 2e61 7070 6c79  ] = gap_df.apply
+00009580: 280a 2020 2020 2020 2020 2020 2020 6c61  (.            la
+00009590: 6d62 6461 2072 6f77 3a20 696e 7476 6c28  mbda row: intvl(
+000095a0: 7374 6172 743d 726f 772e 6761 705f 7374  start=row.gap_st
+000095b0: 6172 742c 2065 6e64 3d72 6f77 2e67 6170  art, end=row.gap
+000095c0: 5f65 6e64 292c 2061 7869 733d 310a 2020  _end), axis=1.  
+000095d0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+000095e0: 2072 6574 7572 6e20 6761 705f 6466 0a0a   return gap_df..
+000095f0: 2020 2020 6465 6620 636f 7079 2873 656c      def copy(sel
+00009600: 6629 202d 3e20 2754 696d 6553 6572 6965  f) -> 'TimeSerie
+00009610: 7327 3a0a 2020 2020 2020 2020 2222 220a  s':.        """.
+00009620: 2020 2020 2020 2020 4d61 6b65 2061 2063          Make a c
+00009630: 6f70 7920 6f66 2074 6869 7320 7469 6d65  opy of this time
+00009640: 2073 6572 6965 7320 6f62 6a65 6374 0a0a   series object..
+00009650: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+00009660: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+00009670: 2020 2020 2020 2020 5469 6d65 5365 7269          TimeSeri
+00009680: 6573 0a20 2020 2020 2020 2020 2020 2041  es.            A
+00009690: 2063 6f70 7920 6f66 2074 6869 7320 7469   copy of this ti
+000096a0: 6d65 2073 6572 6965 732e 0a20 2020 2020  me series..     
+000096b0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+000096c0: 6574 7572 6e20 5469 6d65 5365 7269 6573  eturn TimeSeries
+000096d0: 2873 656c 662e 5f78 6129 2020 2320 7468  (self._xa)  # th
+000096e0: 6520 7861 7272 6179 2077 696c 6c20 6265  e xarray will be
+000096f0: 2063 6f70 6965 6420 696e 2074 6865 2054   copied in the T
+00009700: 696d 6553 6572 6965 7320 636f 6e73 7472  imeSeries constr
+00009710: 7563 746f 720a 0a20 2020 2064 6566 2067  uctor..    def g
+00009720: 6574 5f69 6e64 6578 5f61 745f 706f 696e  et_index_at_poin
+00009730: 7428 7365 6c66 2c20 706f 696e 743a 2055  t(self, point: U
+00009740: 6e69 6f6e 5b70 642e 5469 6d65 7374 616d  nion[pd.Timestam
+00009750: 702c 2066 6c6f 6174 2c20 696e 745d 2c20  p, float, int], 
+00009760: 6166 7465 723d 5472 7565 2920 2d3e 2069  after=True) -> i
+00009770: 6e74 3a0a 2020 2020 2020 2020 2222 220a  nt:.        """.
+00009780: 2020 2020 2020 2020 436f 6e76 6572 7473          Converts
+00009790: 2061 2070 6f69 6e74 2069 6e74 6f20 616e   a point into an
+000097a0: 2069 6e74 6567 6572 2069 6e64 6578 0a0a   integer index..
+000097b0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+000097c0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+000097d0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 706f  -----.        po
+000097e0: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
+000097f0: 5468 6973 2070 6172 616d 6574 6572 2073  This parameter s
+00009800: 7570 706f 7274 7320 3320 6469 6666 6572  upports 3 differ
+00009810: 656e 7420 6461 7461 2074 7970 6573 3a20  ent data types: 
+00009820: 6070 642e 5469 6d65 7374 616d 7060 2c20  `pd.Timestamp`, 
+00009830: 6066 6c6f 6174 6020 616e 6420 6069 6e74  `float` and `int
+00009840: 602e 0a0a 2020 2020 2020 2020 2020 2020  `...            
+00009850: 6070 642e 5469 6d65 7374 616d 7060 2077  `pd.Timestamp` w
+00009860: 6f72 6b20 6f6e 6c79 206f 6e20 7365 7269  ork only on seri
+00009870: 6573 2074 6861 7420 6172 6520 696e 6465  es that are inde
+00009880: 7865 6420 7769 7468 2061 2060 7064 2e44  xed with a `pd.D
+00009890: 6174 6574 696d 6549 6e64 6578 602e 2049  atetimeIndex`. I
+000098a0: 6e20 7375 6368 2063 6173 6573 2c20 7468  n such cases, th
+000098b0: 6520 7265 7475 726e 6564 0a20 2020 2020  e returned.     
+000098c0: 2020 2020 2020 2070 6f69 6e74 2077 696c         point wil
+000098d0: 6c20 6265 2074 6865 2069 6e64 6578 206f  l be the index o
+000098e0: 6620 7468 6973 2074 696d 6573 7461 6d70  f this timestamp
+000098f0: 2069 6620 6974 2069 7320 7072 6573 656e   if it is presen
+00009900: 7420 696e 2074 6865 2073 6572 6965 7320  t in the series 
+00009910: 7469 6d65 2069 6e64 6578 2e20 4974 2069  time index. It i
+00009920: 7427 7320 6e6f 7420 7072 6573 656e 740a  t's not present.
+00009930: 2020 2020 2020 2020 2020 2020 696e 2074              in t
+00009940: 6865 2074 696d 6520 696e 6465 782c 2074  he time index, t
+00009950: 6865 2069 6e64 6578 206f 6620 7468 6520  he index of the 
+00009960: 6e65 7874 2074 696d 6573 7461 6d70 2069  next timestamp i
+00009970: 7320 7265 7475 726e 6564 2069 6620 6061  s returned if `a
+00009980: 6674 6572 3d54 7275 6560 2028 6966 2069  fter=True` (if i
+00009990: 7420 6578 6973 7473 2069 6e20 7468 6520  t exists in the 
+000099a0: 7365 7269 6573 292c 0a20 2020 2020 2020  series),.       
+000099b0: 2020 2020 206f 7468 6572 7769 7365 2074       otherwise t
+000099c0: 6865 2069 6e64 6578 206f 6620 7468 6520  he index of the 
+000099d0: 7072 6576 696f 7573 2074 696d 6573 7461  previous timesta
+000099e0: 6d70 2069 7320 7265 7475 726e 6564 2028  mp is returned (
+000099f0: 6966 2069 7420 6578 6973 7473 2069 6e20  if it exists in 
+00009a00: 7468 6520 7365 7269 6573 292e 0a0a 2020  the series)...  
+00009a10: 2020 2020 2020 2020 2020 496e 2063 6173            In cas
+00009a20: 6520 6f66 2061 2060 666c 6f61 7460 2c20  e of a `float`, 
+00009a30: 7468 6520 7061 7261 6d65 7465 7220 7769  the parameter wi
+00009a40: 6c6c 2062 6520 7472 6561 7465 6420 6173  ll be treated as
+00009a50: 2074 6865 2070 726f 706f 7274 696f 6e20   the proportion 
+00009a60: 6f66 2074 6865 2074 696d 6520 7365 7269  of the time seri
+00009a70: 6573 0a20 2020 2020 2020 2020 2020 2074  es.            t
+00009a80: 6861 7420 7368 6f75 6c64 206c 6965 2062  hat should lie b
+00009a90: 6566 6f72 6520 7468 6520 706f 696e 742e  efore the point.
+00009aa0: 0a0a 2020 2020 2020 2020 2020 2020 496e  ..            In
+00009ab0: 2074 6865 2063 6173 6520 6f66 2060 696e   the case of `in
+00009ac0: 7460 2c20 7468 6520 7061 7261 6d65 7465  t`, the paramete
+00009ad0: 7220 7769 6c6c 2072 6574 7572 6e65 6420  r will returned 
+00009ae0: 6173 2073 7563 682c 2070 726f 7669 6465  as such, provide
+00009af0: 6420 7468 6174 2069 7420 6973 2069 6e20  d that it is in 
+00009b00: 7468 6520 7365 7269 6573 2e20 4f74 6865  the series. Othe
+00009b10: 7277 6973 650a 2020 2020 2020 2020 2020  rwise.          
+00009b20: 2020 6974 2077 696c 6c20 7261 6973 6520    it will raise 
+00009b30: 6120 5661 6c75 6545 7272 6f72 2e0a 2020  a ValueError..  
+00009b40: 2020 2020 2020 6166 7465 720a 2020 2020        after.    
+00009b50: 2020 2020 2020 2020 4966 2074 6865 2070          If the p
+00009b60: 726f 7669 6465 6420 7061 6e64 6173 2054  rovided pandas T
+00009b70: 696d 6573 7461 6d70 2069 7320 6e6f 7420  imestamp is not 
+00009b80: 696e 2074 6865 2074 696d 6520 7365 7269  in the time seri
+00009b90: 6573 2069 6e64 6578 2c20 7768 6574 6865  es index, whethe
+00009ba0: 7220 746f 2072 6574 7572 6e20 7468 6520  r to return the 
+00009bb0: 696e 6465 7820 6f66 2074 6865 0a20 2020  index of the.   
+00009bc0: 2020 2020 2020 2020 206e 6578 7420 7469           next ti
+00009bd0: 6d65 7374 616d 7020 6f72 2074 6865 2069  mestamp or the i
+00009be0: 6e64 6578 206f 6620 7468 6520 7072 6576  ndex of the prev
+00009bf0: 696f 7573 206f 6e65 2e0a 0a20 2020 2020  ious one...     
+00009c00: 2020 2022 2222 0a20 2020 2020 2020 2070     """.        p
+00009c10: 6f69 6e74 5f69 6e64 6578 203d 202d 310a  oint_index = -1.
+00009c20: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00009c30: 7461 6e63 6528 706f 696e 742c 2066 6c6f  tance(point, flo
+00009c40: 6174 293a 0a20 2020 2020 2020 2020 2020  at):.           
+00009c50: 2072 6169 7365 5f69 665f 6e6f 7428 302e   raise_if_not(0.
+00009c60: 203c 3d20 706f 696e 7420 3c3d 2031 2e2c   <= point <= 1.,
+00009c70: 2027 706f 696e 7420 2866 6c6f 6174 2920   'point (float) 
+00009c80: 7368 6f75 6c64 2062 6520 6265 7477 6565  should be betwee
+00009c90: 6e20 302e 3020 616e 6420 312e 302e 272c  n 0.0 and 1.0.',
+00009ca0: 206c 6f67 6765 7229 0a20 2020 2020 2020   logger).       
+00009cb0: 2020 2020 2070 6f69 6e74 5f69 6e64 6578       point_index
+00009cc0: 203d 2069 6e74 2828 6c65 6e28 7365 6c66   = int((len(self
+00009cd0: 2920 2d20 3129 202a 2070 6f69 6e74 290a  ) - 1) * point).
+00009ce0: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
+00009cf0: 6e73 7461 6e63 6528 706f 696e 742c 2028  nstance(point, (
+00009d00: 696e 742c 206e 702e 696e 7436 3429 293a  int, np.int64)):
+00009d10: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00009d20: 7365 5f69 6628 706f 696e 7420 6e6f 7420  se_if(point not 
+00009d30: 696e 2072 616e 6765 286c 656e 2873 656c  in range(len(sel
+00009d40: 6629 292c 2022 706f 696e 7420 2869 6e74  f)), "point (int
+00009d50: 2920 7368 6f75 6c64 2062 6520 6120 7661  ) should be a va
+00009d60: 6c69 6420 696e 6465 7820 696e 2073 6572  lid index in ser
+00009d70: 6965 7322 2c20 6c6f 6767 6572 290a 2020  ies", logger).  
+00009d80: 2020 2020 2020 2020 2020 706f 696e 745f            point_
+00009d90: 696e 6465 7820 3d20 706f 696e 740a 2020  index = point.  
+00009da0: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
+00009db0: 7461 6e63 6528 706f 696e 742c 2070 642e  tance(point, pd.
+00009dc0: 5469 6d65 7374 616d 7029 3a0a 2020 2020  Timestamp):.    
+00009dd0: 2020 2020 2020 2020 7261 6973 655f 6966          raise_if
+00009de0: 5f6e 6f74 2873 656c 662e 5f68 6173 5f64  _not(self._has_d
+00009df0: 6174 6574 696d 655f 696e 6465 782c 0a20  atetime_index,. 
+00009e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e10: 2020 2020 2020 2020 2741 2054 696d 6573          'A Times
+00009e20: 7461 6d70 2068 6173 2062 6565 6e20 7072  tamp has been pr
+00009e30: 6f76 6964 6564 2c20 6275 7420 7468 6973  ovided, but this
+00009e40: 2073 6572 6965 7320 6973 206e 6f74 2074   series is not t
+00009e50: 696d 652d 696e 6465 7865 642e 272c 206c  ime-indexed.', l
+00009e60: 6f67 6765 7229 0a20 2020 2020 2020 2020  ogger).         
+00009e70: 2020 2073 656c 662e 5f72 6169 7365 5f69     self._raise_i
+00009e80: 665f 6e6f 745f 7769 7468 696e 2870 6f69  f_not_within(poi
+00009e90: 6e74 290a 2020 2020 2020 2020 2020 2020  nt).            
+00009ea0: 6966 2070 6f69 6e74 2069 6e20 7365 6c66  if point in self
+00009eb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009ec0: 2020 706f 696e 745f 696e 6465 7820 3d20    point_index = 
+00009ed0: 7365 6c66 2e5f 7469 6d65 5f69 6e64 6578  self._time_index
+00009ee0: 2e67 6574 5f6c 6f63 2870 6f69 6e74 290a  .get_loc(point).
+00009ef0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00009f00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009f10: 2020 706f 696e 745f 696e 6465 7820 3d20    point_index = 
+00009f20: 7365 6c66 2e5f 7469 6d65 5f69 6e64 6578  self._time_index
+00009f30: 2e67 6574 5f6c 6f63 2873 656c 662e 5f67  .get_loc(self._g
+00009f40: 6574 5f66 6972 7374 5f74 696d 6573 7461  et_first_timesta
+00009f50: 6d70 5f61 6674 6572 2870 6f69 6e74 2920  mp_after(point) 
+00009f60: 6966 2061 6674 6572 2065 6c73 650a 2020  if after else.  
+00009f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fa0: 2020 2020 2073 656c 662e 5f67 6574 5f6c       self._get_l
+00009fb0: 6173 745f 7469 6d65 7374 616d 705f 6265  ast_timestamp_be
+00009fc0: 666f 7265 2870 6f69 6e74 2929 0a20 2020  fore(point)).   
+00009fd0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00009fe0: 2020 2020 2020 2072 6169 7365 5f6c 6f67         raise_log
+00009ff0: 2854 7970 6545 7272 6f72 2822 6070 6f69  (TypeError("`poi
+0000a000: 6e74 6020 6e65 6564 7320 746f 2062 6520  nt` needs to be 
+0000a010: 6569 7468 6572 2060 666c 6f61 7460 2c20  either `float`, 
+0000a020: 6069 6e74 6020 6f72 2060 7064 2e54 696d  `int` or `pd.Tim
+0000a030: 6573 7461 6d70 6022 292c 206c 6f67 6765  estamp`"), logge
+0000a040: 7229 0a20 2020 2020 2020 2072 6574 7572  r).        retur
+0000a050: 6e20 706f 696e 745f 696e 6465 780a 0a20  n point_index.. 
+0000a060: 2020 2064 6566 2067 6574 5f74 696d 6573     def get_times
+0000a070: 7461 6d70 5f61 745f 706f 696e 7428 7365  tamp_at_point(se
+0000a080: 6c66 2c20 706f 696e 743a 2055 6e69 6f6e  lf, point: Union
+0000a090: 5b70 642e 5469 6d65 7374 616d 702c 2066  [pd.Timestamp, f
+0000a0a0: 6c6f 6174 2c20 696e 745d 2920 2d3e 2070  loat, int]) -> p
+0000a0b0: 642e 5469 6d65 7374 616d 703a 0a20 2020  d.Timestamp:.   
+0000a0c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000a0d0: 2043 6f6e 7665 7274 7320 6120 706f 696e   Converts a poin
+0000a0e0: 7420 696e 746f 2061 2070 616e 6461 732e  t into a pandas.
+0000a0f0: 5469 6d65 7374 616d 7020 2869 6620 4461  Timestamp (if Da
+0000a100: 7465 7469 6d65 2d69 6e64 6578 6564 2920  tetime-indexed) 
+0000a110: 6f72 2069 6e74 6f20 616e 2069 6e74 6567  or into an integ
+0000a120: 6572 2028 6966 2049 6e74 3634 2d69 6e64  er (if Int64-ind
+0000a130: 6578 6564 292e 0a0a 2020 2020 2020 2020  exed)...        
+0000a140: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+0000a150: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+0000a160: 2020 2020 2020 706f 696e 740a 2020 2020        point.    
+0000a170: 2020 2020 2020 2020 5468 6973 2070 6172          This par
+0000a180: 616d 6574 6572 2073 7570 706f 7274 7320  ameter supports 
+0000a190: 3320 6469 6666 6572 656e 7420 6461 7461  3 different data
+0000a1a0: 2074 7970 6573 3a20 6066 6c6f 6174 602c   types: `float`,
+0000a1b0: 2060 696e 7460 2061 6e64 2060 7061 6e64   `int` and `pand
+0000a1c0: 6173 2e54 696d 6573 7461 6d70 602e 0a20  as.Timestamp`.. 
+0000a1d0: 2020 2020 2020 2020 2020 2049 6e20 6361             In ca
+0000a1e0: 7365 206f 6620 6120 6066 6c6f 6174 602c  se of a `float`,
+0000a1f0: 2074 6865 2070 6172 616d 6574 6572 2077   the parameter w
+0000a200: 696c 6c20 6265 2074 7265 6174 6564 2061  ill be treated a
+0000a210: 7320 7468 6520 7072 6f70 6f72 7469 6f6e  s the proportion
+0000a220: 206f 6620 7468 6520 7469 6d65 2073 6572   of the time ser
+0000a230: 6965 730a 2020 2020 2020 2020 2020 2020  ies.            
+0000a240: 7468 6174 2073 686f 756c 6420 6c69 6520  that should lie 
+0000a250: 6265 666f 7265 2074 6865 2070 6f69 6e74  before the point
+0000a260: 2e0a 2020 2020 2020 2020 2020 2020 496e  ..            In
+0000a270: 2074 6865 2063 6173 6520 6f66 2060 696e   the case of `in
+0000a280: 7460 2c20 7468 6520 7061 7261 6d65 7465  t`, the paramete
+0000a290: 7220 7769 6c6c 2062 6520 7472 6561 7465  r will be treate
+0000a2a0: 6420 6173 2061 6e20 696e 7465 6765 7220  d as an integer 
+0000a2b0: 696e 6465 7820 746f 2074 6865 2074 696d  index to the tim
+0000a2c0: 6520 696e 6465 7820 6f66 0a20 2020 2020  e index of.     
+0000a2d0: 2020 2020 2020 2060 7365 7269 6573 602e         `series`.
+0000a2e0: 2057 696c 6c20 7261 6973 6520 6120 5661   Will raise a Va
+0000a2f0: 6c75 6545 7272 6f72 2069 6620 6e6f 7420  lueError if not 
+0000a300: 6120 7661 6c69 6420 696e 6465 7820 696e  a valid index in
+0000a310: 2060 7365 7269 6573 600a 2020 2020 2020   `series`.      
+0000a320: 2020 2020 2020 496e 2063 6173 6520 6f66        In case of
+0000a330: 2061 2060 7061 6e64 6173 2e54 696d 6573   a `pandas.Times
+0000a340: 7461 6d70 602c 2070 6f69 6e74 2077 696c  tamp`, point wil
+0000a350: 6c20 6265 2072 6574 7572 6e65 6420 6173  l be returned as
+0000a360: 2069 7320 7072 6f76 6964 6564 2074 6861   is provided tha
+0000a370: 7420 7468 6520 7469 6d65 7374 616d 700a  t the timestamp.
+0000a380: 2020 2020 2020 2020 2020 2020 6973 2070              is p
+0000a390: 7265 7365 6e74 2069 6e20 7468 6520 7365  resent in the se
+0000a3a0: 7269 6573 2074 696d 6520 696e 6465 782c  ries time index,
+0000a3b0: 206f 7468 6572 7769 7365 2077 696c 6c20   otherwise will 
+0000a3c0: 7261 6973 6520 6120 5661 6c75 6545 7272  raise a ValueErr
+0000a3d0: 6f72 2e0a 2020 2020 2020 2020 2222 220a  or..        """.
+0000a3e0: 2020 2020 2020 2020 6964 7820 3d20 7365          idx = se
+0000a3f0: 6c66 2e67 6574 5f69 6e64 6578 5f61 745f  lf.get_index_at_
+0000a400: 706f 696e 7428 706f 696e 7429 0a20 2020  point(point).   
+0000a410: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000a420: 2e5f 7469 6d65 5f69 6e64 6578 5b69 6478  ._time_index[idx
+0000a430: 5d0a 0a20 2020 2064 6566 205f 7370 6c69  ]..    def _spli
+0000a440: 745f 6174 2873 656c 662c 0a20 2020 2020  t_at(self,.     
+0000a450: 2020 2020 2020 2020 2020 2020 2073 706c               spl
+0000a460: 6974 5f70 6f69 6e74 3a20 556e 696f 6e5b  it_point: Union[
+0000a470: 7064 2e54 696d 6573 7461 6d70 2c20 666c  pd.Timestamp, fl
+0000a480: 6f61 742c 2069 6e74 5d2c 0a20 2020 2020  oat, int],.     
+0000a490: 2020 2020 2020 2020 2020 2020 2061 6674               aft
+0000a4a0: 6572 3a20 626f 6f6c 203d 2054 7275 6529  er: bool = True)
+0000a4b0: 202d 3e20 5475 706c 655b 2754 696d 6553   -> Tuple['TimeS
+0000a4c0: 6572 6965 7327 2c20 2754 696d 6553 6572  eries', 'TimeSer
+0000a4d0: 6965 7327 5d3a 0a0a 2020 2020 2020 2020  ies']:..        
+0000a4e0: 706f 696e 745f 696e 6465 7820 3d20 7365  point_index = se
+0000a4f0: 6c66 2e67 6574 5f69 6e64 6578 5f61 745f  lf.get_index_at_
+0000a500: 706f 696e 7428 7370 6c69 745f 706f 696e  point(split_poin
+0000a510: 742c 2061 6674 6572 290a 2020 2020 2020  t, after).      
+0000a520: 2020 7265 7475 726e 2073 656c 665b 3a70    return self[:p
+0000a530: 6f69 6e74 5f69 6e64 6578 2b28 3120 6966  oint_index+(1 if
+0000a540: 2061 6674 6572 2065 6c73 6520 3029 5d2c   after else 0)],
+0000a550: 2073 656c 665b 706f 696e 745f 696e 6465   self[point_inde
+0000a560: 782b 2831 2069 6620 6166 7465 7220 656c  x+(1 if after el
+0000a570: 7365 2030 293a 5d0a 0a20 2020 2064 6566  se 0):]..    def
+0000a580: 2073 706c 6974 5f61 6674 6572 2873 656c   split_after(sel
+0000a590: 662c 2073 706c 6974 5f70 6f69 6e74 3a20  f, split_point: 
+0000a5a0: 556e 696f 6e5b 7064 2e54 696d 6573 7461  Union[pd.Timesta
+0000a5b0: 6d70 2c20 666c 6f61 742c 2069 6e74 5d29  mp, float, int])
+0000a5c0: 202d 3e20 5475 706c 655b 2754 696d 6553   -> Tuple['TimeS
+0000a5d0: 6572 6965 7327 2c20 2754 696d 6553 6572  eries', 'TimeSer
+0000a5e0: 6965 7327 5d3a 0a20 2020 2020 2020 2022  ies']:.        "
+0000a5f0: 2222 0a20 2020 2020 2020 2053 706c 6974  "".        Split
+0000a600: 7320 7468 6520 5469 6d65 5365 7269 6573  s the TimeSeries
+0000a610: 2069 6e20 7477 6f2c 2061 6674 6572 2061   in two, after a
+0000a620: 2070 726f 7669 6465 6420 6073 706c 6974   provided `split
+0000a630: 5f70 6f69 6e74 602e 0a0a 2020 2020 2020  _point`...      
+0000a640: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+0000a650: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+0000a660: 2020 2020 2020 2020 7370 6c69 745f 706f          split_po
+0000a670: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
+0000a680: 4120 7469 6d65 7374 616d 702c 2066 6c6f  A timestamp, flo
+0000a690: 6174 206f 7220 696e 7465 6765 722e 2049  at or integer. I
+0000a6a0: 6620 666c 6f61 742c 2072 6570 7265 7365  f float, represe
+0000a6b0: 6e74 7320 7468 6520 7072 6f70 6f72 7469  nts the proporti
+0000a6c0: 6f6e 206f 6620 7468 6520 7365 7269 6573  on of the series
+0000a6d0: 2074 6f20 696e 636c 7564 6520 696e 2074   to include in t
+0000a6e0: 6865 0a20 2020 2020 2020 2020 2020 2066  he.            f
+0000a6f0: 6972 7374 2054 696d 6553 6572 6965 7320  irst TimeSeries 
+0000a700: 286d 7573 7420 6265 2062 6574 7765 656e  (must be between
+0000a710: 2030 2e30 2061 6e64 2031 2e30 292e 2049   0.0 and 1.0). I
+0000a720: 6620 696e 7465 6765 722c 2072 6570 7265  f integer, repre
+0000a730: 7365 6e74 7320 7468 6520 696e 6465 7820  sents the index 
+0000a740: 706f 7369 7469 6f6e 2061 6674 6572 0a20  position after. 
+0000a750: 2020 2020 2020 2020 2020 2077 6869 6368             which
+0000a760: 2074 6865 2073 706c 6974 2069 7320 7065   the split is pe
+0000a770: 7266 6f72 6d65 642e 2041 2070 642e 5469  rformed. A pd.Ti
+0000a780: 6d65 7374 616d 7020 6361 6e20 6265 2070  mestamp can be p
+0000a790: 726f 7669 6465 6420 666f 7220 5469 6d65  rovided for Time
+0000a7a0: 5365 7269 6573 2074 6861 7420 6172 6520  Series that are 
+0000a7b0: 696e 6465 7865 6420 6279 2061 0a20 2020  indexed by a.   
+0000a7c0: 2020 2020 2020 2020 2070 642e 4461 7465           pd.Date
+0000a7d0: 7469 6d65 496e 6465 782e 2049 6e20 7375  timeIndex. In su
+0000a7e0: 6368 2063 6173 6573 2c20 7468 6520 7469  ch cases, the ti
+0000a7f0: 6d65 7374 616d 7020 7769 6c6c 2062 6520  mestamp will be 
+0000a800: 636f 6e74 6169 6e65 6420 696e 2074 6865  contained in the
+0000a810: 2066 6972 7374 2054 696d 6553 6572 6965   first TimeSerie
+0000a820: 732c 2062 7574 206e 6f74 0a20 2020 2020  s, but not.     
+0000a830: 2020 2020 2020 2069 6e20 7468 6520 7365         in the se
+0000a840: 636f 6e64 206f 6e65 2e20 5468 6520 7469  cond one. The ti
+0000a850: 6d65 7374 616d 7020 6974 7365 6c66 2064  mestamp itself d
+0000a860: 6f65 7320 6e6f 7420 6861 7665 2074 6f20  oes not have to 
+0000a870: 6170 7065 6172 2069 6e20 7468 6520 6f72  appear in the or
+0000a880: 6967 696e 616c 2054 696d 6553 6572 6965  iginal TimeSerie
+0000a890: 7320 696e 6465 782e 0a0a 2020 2020 2020  s index...      
+0000a8a0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+0000a8b0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+0000a8c0: 2020 5475 706c 655b 5469 6d65 5365 7269    Tuple[TimeSeri
+0000a8d0: 6573 2c20 5469 6d65 5365 7269 6573 5d0a  es, TimeSeries].
+0000a8e0: 2020 2020 2020 2020 2020 2020 4120 7475              A tu
+0000a8f0: 706c 6520 6f66 2074 776f 2074 696d 6520  ple of two time 
+0000a900: 7365 7269 6573 2e20 5468 6520 6669 7273  series. The firs
+0000a910: 7420 7469 6d65 2073 6572 6965 7320 636f  t time series co
+0000a920: 6e74 6169 6e73 2074 6865 2066 6972 7374  ntains the first
+0000a930: 2073 616d 706c 6573 2075 7020 746f 2074   samples up to t
+0000a940: 6865 2060 7370 6c69 745f 706f 696e 7460  he `split_point`
+0000a950: 2c0a 2020 2020 2020 2020 2020 2020 616e  ,.            an
+0000a960: 6420 7468 6520 7365 636f 6e64 2063 6f6e  d the second con
+0000a970: 7461 696e 7320 7468 6520 7265 6d61 696e  tains the remain
+0000a980: 696e 6720 6f6e 6573 2e0a 2020 2020 2020  ing ones..      
+0000a990: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+0000a9a0: 7475 726e 2073 656c 662e 5f73 706c 6974  turn self._split
+0000a9b0: 5f61 7428 7370 6c69 745f 706f 696e 742c  _at(split_point,
+0000a9c0: 2061 6674 6572 3d54 7275 6529 0a0a 2020   after=True)..  
+0000a9d0: 2020 6465 6620 7370 6c69 745f 6265 666f    def split_befo
+0000a9e0: 7265 2873 656c 662c 2073 706c 6974 5f70  re(self, split_p
+0000a9f0: 6f69 6e74 3a20 556e 696f 6e5b 7064 2e54  oint: Union[pd.T
+0000aa00: 696d 6573 7461 6d70 2c20 666c 6f61 742c  imestamp, float,
+0000aa10: 2069 6e74 5d29 202d 3e20 5475 706c 655b   int]) -> Tuple[
+0000aa20: 2754 696d 6553 6572 6965 7327 2c20 2754  'TimeSeries', 'T
+0000aa30: 696d 6553 6572 6965 7327 5d3a 0a20 2020  imeSeries']:.   
+0000aa40: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000aa50: 2053 706c 6974 7320 7468 6520 5469 6d65   Splits the Time
+0000aa60: 5365 7269 6573 2069 6e20 7477 6f2c 2062  Series in two, b
+0000aa70: 6566 6f72 6520 6120 7072 6f76 6964 6564  efore a provided
+0000aa80: 2060 7370 6c69 745f 706f 696e 7460 2e0a   `split_point`..
+0000aa90: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+0000aaa0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+0000aab0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2073  ------.        s
+0000aac0: 706c 6974 5f70 6f69 6e74 0a20 2020 2020  plit_point.     
+0000aad0: 2020 2020 2020 2041 2074 696d 6573 7461         A timesta
+0000aae0: 6d70 2c20 666c 6f61 7420 6f72 2069 6e74  mp, float or int
+0000aaf0: 6567 6572 2e20 4966 2066 6c6f 6174 2c20  eger. If float, 
+0000ab00: 7265 7072 6573 656e 7473 2074 6865 2070  represents the p
+0000ab10: 726f 706f 7274 696f 6e20 6f66 2074 6865  roportion of the
+0000ab20: 2073 6572 6965 7320 746f 2069 6e63 6c75   series to inclu
+0000ab30: 6465 2069 6e20 7468 650a 2020 2020 2020  de in the.      
+0000ab40: 2020 2020 2020 6669 7273 7420 5469 6d65        first Time
+0000ab50: 5365 7269 6573 2028 6d75 7374 2062 6520  Series (must be 
+0000ab60: 6265 7477 6565 6e20 302e 3020 616e 6420  between 0.0 and 
+0000ab70: 312e 3029 2e20 4966 2069 6e74 6567 6572  1.0). If integer
+0000ab80: 2c20 7265 7072 6573 656e 7473 2074 6865  , represents the
+0000ab90: 2069 6e64 6578 2070 6f73 6974 696f 6e20   index position 
+0000aba0: 6265 666f 7265 0a20 2020 2020 2020 2020  before.         
+0000abb0: 2020 2077 6869 6368 2074 6865 2073 706c     which the spl
+0000abc0: 6974 2069 7320 7065 7266 6f72 6d65 642e  it is performed.
+0000abd0: 2041 2070 642e 5469 6d65 7374 616d 7020   A pd.Timestamp 
+0000abe0: 6361 6e20 6265 2070 726f 7669 6465 6420  can be provided 
+0000abf0: 666f 7220 5469 6d65 5365 7269 6573 2074  for TimeSeries t
+0000ac00: 6861 7420 6172 6520 696e 6465 7865 6420  hat are indexed 
+0000ac10: 6279 2061 0a20 2020 2020 2020 2020 2020  by a.           
+0000ac20: 2070 642e 4461 7465 7469 6d65 496e 6465   pd.DatetimeInde
+0000ac30: 782e 2049 6e20 7375 6368 2063 6173 6573  x. In such cases
+0000ac40: 2c20 7468 6520 7469 6d65 7374 616d 7020  , the timestamp 
+0000ac50: 7769 6c6c 2062 6520 636f 6e74 6169 6e65  will be containe
+0000ac60: 6420 696e 2074 6865 2073 6563 6f6e 6420  d in the second 
+0000ac70: 5469 6d65 5365 7269 6573 2c20 6275 7420  TimeSeries, but 
+0000ac80: 6e6f 740a 2020 2020 2020 2020 2020 2020  not.            
+0000ac90: 696e 2074 6865 2066 6972 7374 206f 6e65  in the first one
+0000aca0: 2e20 5468 6520 7469 6d65 7374 616d 7020  . The timestamp 
+0000acb0: 6974 7365 6c66 2064 6f65 7320 6e6f 7420  itself does not 
+0000acc0: 6861 7665 2074 6f20 6170 7065 6172 2069  have to appear i
+0000acd0: 6e20 7468 6520 6f72 6967 696e 616c 2054  n the original T
+0000ace0: 696d 6553 6572 6965 7320 696e 6465 782e  imeSeries index.
+0000acf0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0000ad00: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0000ad10: 2d0a 2020 2020 2020 2020 5475 706c 655b  -.        Tuple[
+0000ad20: 5469 6d65 5365 7269 6573 2c20 5469 6d65  TimeSeries, Time
+0000ad30: 5365 7269 6573 5d0a 2020 2020 2020 2020  Series].        
+0000ad40: 2020 2020 4120 7475 706c 6520 6f66 2074      A tuple of t
+0000ad50: 776f 2074 696d 6520 7365 7269 6573 2e20  wo time series. 
+0000ad60: 5468 6520 6669 7273 7420 7469 6d65 2073  The first time s
+0000ad70: 6572 6965 7320 636f 6e74 6169 6e73 2074  eries contains t
+0000ad80: 6865 2066 6972 7374 2073 616d 706c 6573  he first samples
+0000ad90: 2075 7020 746f 2074 6865 2060 7370 6c69   up to the `spli
+0000ada0: 745f 706f 696e 7460 2c0a 2020 2020 2020  t_point`,.      
+0000adb0: 2020 2020 2020 616e 6420 7468 6520 7365        and the se
+0000adc0: 636f 6e64 2063 6f6e 7461 696e 7320 7468  cond contains th
+0000add0: 6520 7265 6d61 696e 696e 6720 6f6e 6573  e remaining ones
+0000ade0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+0000adf0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000ae00: 662e 5f73 706c 6974 5f61 7428 7370 6c69  f._split_at(spli
+0000ae10: 745f 706f 696e 742c 2061 6674 6572 3d46  t_point, after=F
+0000ae20: 616c 7365 290a 0a20 2020 2064 6566 2064  alse)..    def d
+0000ae30: 726f 705f 6166 7465 7228 7365 6c66 2c20  rop_after(self, 
+0000ae40: 7370 6c69 745f 706f 696e 743a 2055 6e69  split_point: Uni
+0000ae50: 6f6e 5b70 642e 5469 6d65 7374 616d 702c  on[pd.Timestamp,
+0000ae60: 2066 6c6f 6174 2c20 696e 745d 293a 0a20   float, int]):. 
+0000ae70: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000ae80: 2020 2044 726f 7073 2065 7665 7279 7468     Drops everyth
+0000ae90: 696e 6720 6166 7465 7220 7468 6520 7072  ing after the pr
+0000aea0: 6f76 6964 6564 2074 696d 6573 7461 6d70  ovided timestamp
+0000aeb0: 2060 7473 602c 2069 6e63 6c75 6465 642e   `ts`, included.
+0000aec0: 0a20 2020 2020 2020 2054 6865 2074 696d  .        The tim
+0000aed0: 6573 7461 6d70 206d 6179 206e 6f74 2062  estamp may not b
+0000aee0: 6520 696e 2074 6865 2054 696d 6553 6572  e in the TimeSer
+0000aef0: 6965 732e 2049 6620 6974 2069 732c 2074  ies. If it is, t
+0000af00: 6865 2074 696d 6573 7461 6d70 2077 696c  he timestamp wil
+0000af10: 6c20 6265 2064 726f 7070 6564 2e0a 0a20  l be dropped... 
+0000af20: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+0000af30: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0000af40: 2d2d 2d2d 0a20 2020 2020 2020 2073 706c  ----.        spl
+0000af50: 6974 5f70 6f69 6e74 0a20 2020 2020 2020  it_point.       
+0000af60: 2020 2020 2054 6865 2074 696d 6573 7461       The timesta
+0000af70: 6d70 2074 6861 7420 696e 6469 6361 7465  mp that indicate
+0000af80: 7320 6375 742d 6f66 6620 7469 6d65 2e0a  s cut-off time..
+0000af90: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+0000afa0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+0000afb0: 0a20 2020 2020 2020 2054 696d 6553 6572  .        TimeSer
+0000afc0: 6965 730a 2020 2020 2020 2020 2020 2020  ies.            
+0000afd0: 4120 6e65 7720 5469 6d65 5365 7269 6573  A new TimeSeries
+0000afe0: 2c20 6166 7465 7220 6074 7360 2e0a 2020  , after `ts`..  
+0000aff0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000b000: 2020 7265 7475 726e 2073 656c 662e 7370    return self.sp
+0000b010: 6c69 745f 6265 666f 7265 2873 706c 6974  lit_before(split
+0000b020: 5f70 6f69 6e74 295b 305d 0a0a 2020 2020  _point)[0]..    
+0000b030: 6465 6620 6472 6f70 5f62 6566 6f72 6528  def drop_before(
+0000b040: 7365 6c66 2c20 7370 6c69 745f 706f 696e  self, split_poin
+0000b050: 743a 2055 6e69 6f6e 5b70 642e 5469 6d65  t: Union[pd.Time
+0000b060: 7374 616d 702c 2066 6c6f 6174 2c20 696e  stamp, float, in
+0000b070: 745d 293a 0a20 2020 2020 2020 2022 2222  t]):.        """
+0000b080: 0a20 2020 2020 2020 2044 726f 7073 2065  .        Drops e
+0000b090: 7665 7279 7468 696e 6720 6265 666f 7265  verything before
+0000b0a0: 2074 6865 2070 726f 7669 6465 6420 7469   the provided ti
+0000b0b0: 6d65 7374 616d 7020 6074 7360 2c20 696e  mestamp `ts`, in
+0000b0c0: 636c 7564 6564 2e0a 2020 2020 2020 2020  cluded..        
+0000b0d0: 5468 6520 7469 6d65 7374 616d 7020 6d61  The timestamp ma
+0000b0e0: 7920 6e6f 7420 6265 2069 6e20 7468 6520  y not be in the 
+0000b0f0: 5469 6d65 5365 7269 6573 2e20 4966 2069  TimeSeries. If i
+0000b100: 7420 6973 2c20 7468 6520 7469 6d65 7374  t is, the timest
+0000b110: 616d 7020 7769 6c6c 2062 6520 6472 6f70  amp will be drop
+0000b120: 7065 642e 0a0a 2020 2020 2020 2020 5061  ped...        Pa
+0000b130: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+0000b140: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+0000b150: 2020 2020 7370 6c69 745f 706f 696e 740a      split_point.
+0000b160: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+0000b170: 7469 6d65 7374 616d 7020 7468 6174 2069  timestamp that i
+0000b180: 6e64 6963 6174 6573 2063 7574 2d6f 6666  ndicates cut-off
+0000b190: 2074 696d 652e 0a0a 2020 2020 2020 2020   time...        
+0000b1a0: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+0000b1b0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+0000b1c0: 5469 6d65 5365 7269 6573 0a20 2020 2020  TimeSeries.     
+0000b1d0: 2020 2020 2020 2041 206e 6577 2054 696d         A new Tim
+0000b1e0: 6553 6572 6965 732c 2061 6674 6572 2060  eSeries, after `
+0000b1f0: 7473 602e 0a20 2020 2020 2020 2022 2222  ts`..        """
+0000b200: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000b210: 7365 6c66 2e73 706c 6974 5f61 6674 6572  self.split_after
+0000b220: 2873 706c 6974 5f70 6f69 6e74 295b 315d  (split_point)[1]
+0000b230: 0a0a 2020 2020 6465 6620 736c 6963 6528  ..    def slice(
+0000b240: 7365 6c66 2c20 7374 6172 745f 7473 3a20  self, start_ts: 
+0000b250: 556e 696f 6e5b 7064 2e54 696d 6573 7461  Union[pd.Timesta
+0000b260: 6d70 2c20 696e 745d 2c20 656e 645f 7473  mp, int], end_ts
+0000b270: 3a20 556e 696f 6e5b 7064 2e54 696d 6573  : Union[pd.Times
+0000b280: 7461 6d70 2c20 696e 745d 293a 0a20 2020  tamp, int]):.   
+0000b290: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000b2a0: 2052 6574 7572 6e73 2061 206e 6577 2054   Returns a new T
+0000b2b0: 696d 6553 6572 6965 732c 2073 7461 7274  imeSeries, start
+0000b2c0: 696e 6720 6c61 7465 7220 7468 616e 2060  ing later than `
+0000b2d0: 7374 6172 745f 7473 6020 616e 6420 656e  start_ts` and en
+0000b2e0: 6469 6e67 2062 6566 6f72 6520 6065 6e64  ding before `end
+0000b2f0: 5f74 7360 2c20 696e 636c 7573 6976 6520  _ts`, inclusive 
+0000b300: 6f6e 2062 6f74 6820 656e 6473 2e0a 2020  on both ends..  
+0000b310: 2020 2020 2020 5468 6520 7469 6d65 7374        The timest
+0000b320: 616d 7073 2064 6f6e 2774 2068 6176 6520  amps don't have 
+0000b330: 746f 2062 6520 696e 2074 6865 2073 6572  to be in the ser
+0000b340: 6965 732e 0a0a 2020 2020 2020 2020 5061  ies...        Pa
+0000b350: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+0000b360: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+0000b370: 2020 2020 7374 6172 745f 7473 0a20 2020      start_ts.   
+0000b380: 2020 2020 2020 2020 2054 6865 2074 696d           The tim
+0000b390: 6573 7461 6d70 2074 6861 7420 696e 6469  estamp that indi
+0000b3a0: 6361 7465 7320 7468 6520 6c65 6674 2063  cates the left c
+0000b3b0: 7574 2d6f 6666 2e0a 2020 2020 2020 2020  ut-off..        
+0000b3c0: 656e 645f 7473 0a20 2020 2020 2020 2020  end_ts.         
+0000b3d0: 2020 2054 6865 2074 696d 6573 7461 6d70     The timestamp
+0000b3e0: 2074 6861 7420 696e 6469 6361 7465 7320   that indicates 
+0000b3f0: 7468 6520 7269 6768 7420 6375 742d 6f66  the right cut-of
+0000b400: 662e 0a0a 2020 2020 2020 2020 5265 7475  f...        Retu
+0000b410: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+0000b420: 2d2d 2d0a 2020 2020 2020 2020 5469 6d65  ---.        Time
+0000b430: 5365 7269 6573 0a20 2020 2020 2020 2020  Series.         
+0000b440: 2020 2041 206e 6577 2073 6572 6965 732c     A new series,
+0000b450: 2077 6974 6820 696e 6469 6365 7320 6772   with indices gr
+0000b460: 6561 7465 7220 6f72 2065 7175 616c 2074  eater or equal t
+0000b470: 6861 6e20 6073 7461 7274 5f74 7360 2061  han `start_ts` a
+0000b480: 6e64 2073 6d61 6c6c 6572 206f 7220 6571  nd smaller or eq
+0000b490: 7561 6c20 7468 616e 2060 656e 645f 7473  ual than `end_ts
+0000b4a0: 602e 0a20 2020 2020 2020 2022 2222 0a20  `..        """. 
+0000b4b0: 2020 2020 2020 2072 6169 7365 5f69 665f         raise_if_
+0000b4c0: 6e6f 7428 7479 7065 2873 7461 7274 5f74  not(type(start_t
+0000b4d0: 7329 203d 3d20 7479 7065 2865 6e64 5f74  s) == type(end_t
+0000b4e0: 7329 2c20 2754 6865 2074 776f 2074 696d  s), 'The two tim
+0000b4f0: 6573 7461 6d70 7320 7072 6f76 6964 6564  estamps provided
+0000b500: 2074 6f20 736c 6963 6528 2920 6861 7665   to slice() have
+0000b510: 2074 6f20 6265 206f 6620 7468 6520 270a   to be of the '.
+0000b520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b550: 2020 2020 2027 7361 6d65 2074 7970 652e       'same type.
+0000b560: 272c 206c 6f67 6765 7229 0a20 2020 2020  ', logger).     
+0000b570: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+0000b580: 2873 7461 7274 5f74 732c 2070 642e 5469  (start_ts, pd.Ti
+0000b590: 6d65 7374 616d 7029 3a0a 2020 2020 2020  mestamp):.      
+0000b5a0: 2020 2020 2020 7261 6973 655f 6966 5f6e        raise_if_n
+0000b5b0: 6f74 2873 656c 662e 5f68 6173 5f64 6174  ot(self._has_dat
+0000b5c0: 6574 696d 655f 696e 6465 782c 2027 5469  etime_index, 'Ti
+0000b5d0: 6d65 7374 616d 7073 2068 6176 6520 6265  mestamps have be
+0000b5e0: 656e 2070 726f 7669 6465 6420 746f 2073  en provided to s
+0000b5f0: 6c69 6365 2829 2c20 6275 7420 7468 6520  lice(), but the 
+0000b600: 7365 7269 6573 2069 7320 270a 2020 2020  series is '.    
+0000b610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b630: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000b640: 696e 6465 7865 6420 7573 696e 6720 616e  indexed using an
+0000b650: 2069 6e74 6567 6572 2d62 6173 6564 2049   integer-based I
+0000b660: 6e74 3634 496e 6465 782e 272c 206c 6f67  nt64Index.', log
+0000b670: 6765 7229 0a20 2020 2020 2020 2020 2020  ger).           
+0000b680: 2069 6478 203d 2070 642e 4461 7465 7469   idx = pd.Dateti
+0000b690: 6d65 496e 6465 7828 6669 6c74 6572 286c  meIndex(filter(l
+0000b6a0: 616d 6264 6120 743a 2073 7461 7274 5f74  ambda t: start_t
+0000b6b0: 7320 3c3d 2074 203c 3d20 656e 645f 7473  s <= t <= end_ts
+0000b6c0: 2c20 7365 6c66 2e5f 7469 6d65 5f69 6e64  , self._time_ind
+0000b6d0: 6578 2929 0a20 2020 2020 2020 2065 6c73  ex)).        els
+0000b6e0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0000b6f0: 6169 7365 5f69 6628 7365 6c66 2e5f 6861  aise_if(self._ha
+0000b700: 735f 6461 7465 7469 6d65 5f69 6e64 6578  s_datetime_index
+0000b710: 2c20 2773 7461 7274 2061 6e64 2065 6e64  , 'start and end
+0000b720: 2074 696d 6573 2068 6176 6520 6265 656e   times have been
+0000b730: 2070 726f 7669 6465 6420 6173 2069 6e74   provided as int
+0000b740: 6567 6572 7320 746f 2073 6c69 6365 2829  egers to slice()
+0000b750: 2c20 6275 7420 270a 2020 2020 2020 2020  , but '.        
+0000b760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b780: 2020 2020 2020 2027 7468 6520 7365 7269         'the seri
+0000b790: 6573 2069 7320 696e 6465 7865 6420 7769  es is indexed wi
+0000b7a0: 7468 2061 2044 6174 6574 696d 6549 6e64  th a DatetimeInd
+0000b7b0: 6578 2e27 2c20 6c6f 6767 6572 290a 2020  ex.', logger).  
+0000b7c0: 2020 2020 2020 2020 2020 6964 7820 3d20            idx = 
+0000b7d0: 7064 2e52 616e 6765 496e 6465 7828 7374  pd.RangeIndex(st
+0000b7e0: 6172 745f 7473 2c20 656e 645f 7473 2c20  art_ts, end_ts, 
+0000b7f0: 7374 6570 3d31 290a 2020 2020 2020 2020  step=1).        
+0000b800: 7265 7475 726e 2073 656c 665b 6964 785d  return self[idx]
+0000b810: 0a0a 2020 2020 6465 6620 736c 6963 655f  ..    def slice_
+0000b820: 6e5f 706f 696e 7473 5f61 6674 6572 2873  n_points_after(s
+0000b830: 656c 662c 2073 7461 7274 5f74 733a 2055  elf, start_ts: U
+0000b840: 6e69 6f6e 5b70 642e 5469 6d65 7374 616d  nion[pd.Timestam
+0000b850: 702c 2069 6e74 5d2c 206e 3a20 696e 7429  p, int], n: int)
+0000b860: 202d 3e20 2754 696d 6553 6572 6965 7327   -> 'TimeSeries'
+0000b870: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000b880: 2020 2020 2020 5265 7475 726e 7320 6120        Returns a 
+0000b890: 6e65 7720 5469 6d65 5365 7269 6573 2c20  new TimeSeries, 
+0000b8a0: 7374 6172 7469 6e67 2061 2060 7374 6172  starting a `star
+0000b8b0: 745f 7473 6020 616e 6420 6861 7669 6e67  t_ts` and having
+0000b8c0: 2061 7420 6d6f 7374 2060 6e60 2070 6f69   at most `n` poi
+0000b8d0: 6e74 732e 0a0a 2020 2020 2020 2020 5468  nts...        Th
+0000b8e0: 6520 7072 6f76 6964 6564 2074 696d 6573  e provided times
+0000b8f0: 7461 6d70 7320 7769 6c6c 2062 6520 696e  tamps will be in
+0000b900: 636c 7564 6564 2069 6e20 7468 6520 7365  cluded in the se
+0000b910: 7269 6573 2e0a 0a20 2020 2020 2020 2050  ries...        P
+0000b920: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+0000b930: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+0000b940: 2020 2020 2073 7461 7274 5f74 730a 2020       start_ts.  
+0000b950: 2020 2020 2020 2020 2020 5468 6520 7469            The ti
+0000b960: 6d65 7374 616d 7020 6f72 2069 6e64 6578  mestamp or index
+0000b970: 2074 6861 7420 696e 6469 6361 7465 7320   that indicates 
+0000b980: 7468 6520 7370 6c69 7474 696e 6720 7469  the splitting ti
+0000b990: 6d65 2e0a 2020 2020 2020 2020 6e0a 2020  me..        n.  
+0000b9a0: 2020 2020 2020 2020 2020 5468 6520 6d61            The ma
+0000b9b0: 7869 6d61 6c20 6c65 6e67 7468 206f 6620  ximal length of 
+0000b9c0: 7468 6520 6e65 7720 5469 6d65 5365 7269  the new TimeSeri
+0000b9d0: 6573 2e0a 0a20 2020 2020 2020 2052 6574  es...        Ret
+0000b9e0: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+0000b9f0: 2d2d 2d2d 0a20 2020 2020 2020 2054 696d  ----.        Tim
+0000ba00: 6553 6572 6965 730a 2020 2020 2020 2020  eSeries.        
+0000ba10: 2020 2020 4120 6e65 7720 5469 6d65 5365      A new TimeSe
+0000ba20: 7269 6573 2c20 7769 7468 206c 656e 6774  ries, with lengt
+0000ba30: 6820 6174 206d 6f73 7420 606e 602c 2073  h at most `n`, s
+0000ba40: 7461 7274 696e 6720 6174 2060 7374 6172  tarting at `star
+0000ba50: 745f 7473 600a 2020 2020 2020 2020 2222  t_ts`.        ""
+0000ba60: 220a 2020 2020 2020 2020 7261 6973 655f  ".        raise_
+0000ba70: 6966 5f6e 6f74 286e 203e 2030 2c20 276e  if_not(n > 0, 'n
+0000ba80: 2073 686f 756c 6420 6265 2061 2070 6f73   should be a pos
+0000ba90: 6974 6976 6520 696e 7465 6765 722e 272c  itive integer.',
+0000baa0: 206c 6f67 6765 7229 0a20 2020 2020 2020   logger).       
+0000bab0: 2073 656c 662e 5f72 6169 7365 5f69 665f   self._raise_if_
+0000bac0: 6e6f 745f 7769 7468 696e 2873 7461 7274  not_within(start
+0000bad0: 5f74 7329 0a0a 2020 2020 2020 2020 6966  _ts)..        if
+0000bae0: 2069 7369 6e73 7461 6e63 6528 7374 6172   isinstance(star
+0000baf0: 745f 7473 2c20 2869 6e74 2c20 6e70 2e69  t_ts, (int, np.i
+0000bb00: 6e74 3634 2929 3a0a 2020 2020 2020 2020  nt64)):.        
+0000bb10: 2020 2020 7265 7475 726e 2073 656c 665b      return self[
+0000bb20: 7374 6172 745f 7473 3a73 7461 7274 5f74  start_ts:start_t
+0000bb30: 732b 6e5d 0a20 2020 2020 2020 2065 6c69  s+n].        eli
+0000bb40: 6620 6973 696e 7374 616e 6365 2873 7461  f isinstance(sta
+0000bb50: 7274 5f74 732c 2070 642e 5469 6d65 7374  rt_ts, pd.Timest
+0000bb60: 616d 7029 3a0a 2020 2020 2020 2020 2020  amp):.          
+0000bb70: 2020 2320 6765 7420 6669 7273 7420 7469    # get first ti
+0000bb80: 6d65 7374 616d 7020 6772 6561 7465 7220  mestamp greater 
+0000bb90: 6f72 2065 7175 616c 2074 6f20 7374 6172  or equal to star
+0000bba0: 745f 7473 0a20 2020 2020 2020 2020 2020  t_ts.           
+0000bbb0: 2074 7373 203d 2073 656c 662e 5f67 6574   tss = self._get
+0000bbc0: 5f66 6972 7374 5f74 696d 6573 7461 6d70  _first_timestamp
+0000bbd0: 5f61 6674 6572 2873 7461 7274 5f74 7329  _after(start_ts)
+0000bbe0: 0a20 2020 2020 2020 2020 2020 2070 6f69  .            poi
+0000bbf0: 6e74 5f69 6e64 6578 203d 2073 656c 662e  nt_index = self.
+0000bc00: 6765 745f 696e 6465 785f 6174 5f70 6f69  get_index_at_poi
+0000bc10: 6e74 2874 7373 290a 2020 2020 2020 2020  nt(tss).        
+0000bc20: 2020 2020 7265 7475 726e 2073 656c 665b      return self[
+0000bc30: 706f 696e 745f 696e 6465 783a 706f 696e  point_index:poin
+0000bc40: 745f 696e 6465 7820 2b20 6e5d 0a20 2020  t_index + n].   
+0000bc50: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000bc60: 2020 2020 2020 2072 6169 7365 5f6c 6f67         raise_log
+0000bc70: 2856 616c 7565 4572 726f 7228 2773 7461  (ValueError('sta
+0000bc80: 7274 5f74 7320 6d75 7374 2062 6520 616e  rt_ts must be an
+0000bc90: 2069 6e74 206f 7220 6120 7061 6e64 6173   int or a pandas
+0000bca0: 2054 696d 6573 7461 6d70 2e27 292c 206c   Timestamp.'), l
+0000bcb0: 6f67 6765 7229 0a0a 2020 2020 6465 6620  ogger)..    def 
+0000bcc0: 736c 6963 655f 6e5f 706f 696e 7473 5f62  slice_n_points_b
+0000bcd0: 6566 6f72 6528 7365 6c66 2c20 656e 645f  efore(self, end_
+0000bce0: 7473 3a20 556e 696f 6e5b 7064 2e54 696d  ts: Union[pd.Tim
+0000bcf0: 6573 7461 6d70 2c20 696e 745d 2c20 6e3a  estamp, int], n:
+0000bd00: 2069 6e74 2920 2d3e 2027 5469 6d65 5365   int) -> 'TimeSe
+0000bd10: 7269 6573 273a 0a20 2020 2020 2020 2022  ries':.        "
+0000bd20: 2222 0a20 2020 2020 2020 2052 6574 7572  "".        Retur
+0000bd30: 6e73 2061 206e 6577 2054 696d 6553 6572  ns a new TimeSer
+0000bd40: 6965 732c 2065 6e64 696e 6720 6174 2060  ies, ending at `
+0000bd50: 7374 6172 745f 7473 6020 616e 6420 6861  start_ts` and ha
+0000bd60: 7669 6e67 2061 7420 6d6f 7374 2060 6e60  ving at most `n`
+0000bd70: 2070 6f69 6e74 732e 0a0a 2020 2020 2020   points...      
+0000bd80: 2020 5468 6520 7072 6f76 6964 6564 2074    The provided t
+0000bd90: 696d 6573 7461 6d70 7320 7769 6c6c 2062  imestamps will b
+0000bda0: 6520 696e 636c 7564 6564 2069 6e20 7468  e included in th
+0000bdb0: 6520 7365 7269 6573 2e0a 0a20 2020 2020  e series...     
+0000bdc0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+0000bdd0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+0000bde0: 0a20 2020 2020 2020 2065 6e64 5f74 730a  .        end_ts.
+0000bdf0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+0000be00: 7469 6d65 7374 616d 7020 6f72 2069 6e64  timestamp or ind
+0000be10: 6578 2074 6861 7420 696e 6469 6361 7465  ex that indicate
+0000be20: 7320 7468 6520 7370 6c69 7474 696e 6720  s the splitting 
+0000be30: 7469 6d65 2e0a 2020 2020 2020 2020 6e0a  time..        n.
+0000be40: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+0000be50: 6d61 7869 6d61 6c20 6c65 6e67 7468 206f  maximal length o
+0000be60: 6620 7468 6520 6e65 7720 5469 6d65 5365  f the new TimeSe
+0000be70: 7269 6573 2e0a 0a20 2020 2020 2020 2052  ries...        R
+0000be80: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+0000be90: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2054  ------.        T
+0000bea0: 696d 6553 6572 6965 730a 2020 2020 2020  imeSeries.      
+0000beb0: 2020 2020 2020 4120 6e65 7720 5469 6d65        A new Time
+0000bec0: 5365 7269 6573 2c20 7769 7468 206c 656e  Series, with len
+0000bed0: 6774 6820 6174 206d 6f73 7420 606e 602c  gth at most `n`,
+0000bee0: 2065 6e64 696e 6720 6174 2060 7374 6172   ending at `star
+0000bef0: 745f 7473 600a 2020 2020 2020 2020 2222  t_ts`.        ""
+0000bf00: 220a 0a20 2020 2020 2020 2072 6169 7365  "..        raise
+0000bf10: 5f69 665f 6e6f 7428 6e20 3e20 302c 2027  _if_not(n > 0, '
+0000bf20: 6e20 7368 6f75 6c64 2062 6520 6120 706f  n should be a po
+0000bf30: 7369 7469 7665 2069 6e74 6567 6572 2e27  sitive integer.'
+0000bf40: 2c20 6c6f 6767 6572 290a 2020 2020 2020  , logger).      
+0000bf50: 2020 7365 6c66 2e5f 7261 6973 655f 6966    self._raise_if
+0000bf60: 5f6e 6f74 5f77 6974 6869 6e28 656e 645f  _not_within(end_
+0000bf70: 7473 290a 0a20 2020 2020 2020 2069 6620  ts)..        if 
+0000bf80: 6973 696e 7374 616e 6365 2865 6e64 5f74  isinstance(end_t
+0000bf90: 732c 2028 696e 742c 206e 702e 696e 7436  s, (int, np.int6
+0000bfa0: 3429 293a 0a20 2020 2020 2020 2020 2020  4)):.           
+0000bfb0: 2072 6574 7572 6e20 7365 6c66 5b65 6e64   return self[end
+0000bfc0: 5f74 732d 6e2b 313a 656e 645f 7473 2b31  _ts-n+1:end_ts+1
+0000bfd0: 5d0a 2020 2020 2020 2020 656c 6966 2069  ].        elif i
+0000bfe0: 7369 6e73 7461 6e63 6528 656e 645f 7473  sinstance(end_ts
+0000bff0: 2c20 7064 2e54 696d 6573 7461 6d70 293a  , pd.Timestamp):
+0000c000: 0a20 2020 2020 2020 2020 2020 2023 2067  .            # g
+0000c010: 6574 206c 6173 7420 7469 6d65 7374 616d  et last timestam
+0000c020: 7020 736d 616c 6c65 7220 6f72 2065 7175  p smaller or equ
+0000c030: 616c 2074 6f20 7374 6172 745f 7473 0a20  al to start_ts. 
+0000c040: 2020 2020 2020 2020 2020 2074 7373 203d             tss =
+0000c050: 2073 656c 662e 5f67 6574 5f6c 6173 745f   self._get_last_
+0000c060: 7469 6d65 7374 616d 705f 6265 666f 7265  timestamp_before
+0000c070: 2865 6e64 5f74 7329 0a20 2020 2020 2020  (end_ts).       
+0000c080: 2020 2020 2070 6f69 6e74 5f69 6e64 6578       point_index
+0000c090: 203d 2073 656c 662e 6765 745f 696e 6465   = self.get_inde
+0000c0a0: 785f 6174 5f70 6f69 6e74 2874 7373 290a  x_at_point(tss).
+0000c0b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000c0c0: 726e 2073 656c 665b 6d61 7828 302c 2070  rn self[max(0, p
+0000c0d0: 6f69 6e74 5f69 6e64 6578 2d6e 2b31 293a  oint_index-n+1):
+0000c0e0: 706f 696e 745f 696e 6465 782b 315d 0a20  point_index+1]. 
+0000c0f0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000c100: 2020 2020 2020 2020 2072 6169 7365 5f6c           raise_l
+0000c110: 6f67 2856 616c 7565 4572 726f 7228 2773  og(ValueError('s
+0000c120: 7461 7274 5f74 7320 6d75 7374 2062 6520  tart_ts must be 
+0000c130: 616e 2069 6e74 206f 7220 6120 7061 6e64  an int or a pand
+0000c140: 6173 2054 696d 6573 7461 6d70 2e27 292c  as Timestamp.'),
+0000c150: 206c 6f67 6765 7229 0a0a 2020 2020 6465   logger)..    de
+0000c160: 6620 736c 6963 655f 696e 7465 7273 6563  f slice_intersec
+0000c170: 7428 7365 6c66 2c20 6f74 6865 723a 2027  t(self, other: '
+0000c180: 5469 6d65 5365 7269 6573 2729 202d 3e20  TimeSeries') -> 
+0000c190: 2754 696d 6553 6572 6965 7327 3a0a 2020  'TimeSeries':.  
+0000c1a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000c1b0: 2020 5265 7475 726e 7320 6120 5469 6d65    Returns a Time
+0000c1c0: 5365 7269 6573 2073 6c69 6365 206f 6620  Series slice of 
+0000c1d0: 7468 6973 2074 696d 6520 7365 7269 6573  this time series
+0000c1e0: 2c20 7768 6572 6520 7468 6520 7469 6d65  , where the time
+0000c1f0: 2069 6e64 6578 2068 6173 2062 6565 6e20   index has been 
+0000c200: 696e 7465 7273 6563 7465 6420 7769 7468  intersected with
+0000c210: 2074 6865 206f 6e65 0a20 2020 2020 2020   the one.       
+0000c220: 2070 726f 7669 6465 6420 696e 2061 7267   provided in arg
+0000c230: 756d 656e 742e 204e 6f74 6520 7468 6174  ument. Note that
+0000c240: 2074 6869 7320 6d65 7468 6f64 2069 7320   this method is 
+0000c250: 696e 2067 656e 6572 616c 202a 6e6f 742a  in general *not*
+0000c260: 2073 796d 6d65 7472 6963 2e0a 0a20 2020   symmetric...   
+0000c270: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+0000c280: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+0000c290: 2d2d 0a20 2020 2020 2020 206f 7468 6572  --.        other
+0000c2a0: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
+0000c2b0: 206f 7468 6572 2074 696d 6520 7365 7269   other time seri
+0000c2c0: 6573 0a0a 2020 2020 2020 2020 5265 7475  es..        Retu
+0000c2d0: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+0000c2e0: 2d2d 2d0a 2020 2020 2020 2020 5469 6d65  ---.        Time
+0000c2f0: 5365 7269 6573 0a20 2020 2020 2020 2020  Series.         
+0000c300: 2020 2061 206e 6577 2073 6572 6965 732c     a new series,
+0000c310: 2063 6f6e 7461 696e 696e 6720 7468 6520   containing the 
+0000c320: 7661 6c75 6573 206f 6620 7468 6973 2073  values of this s
+0000c330: 6572 6965 732c 206f 7665 7220 7468 6520  eries, over the 
+0000c340: 7469 6d65 2d73 7061 6e20 636f 6d6d 6f6e  time-span common
+0000c350: 2074 6f20 626f 7468 2074 696d 6520 7365   to both time se
+0000c360: 7269 6573 2e0a 2020 2020 2020 2020 2222  ries..        ""
+0000c370: 220a 2020 2020 2020 2020 7469 6d65 5f69  ".        time_i
+0000c380: 6e64 6578 203d 2073 656c 662e 7469 6d65  ndex = self.time
+0000c390: 5f69 6e64 6578 2e69 6e74 6572 7365 6374  _index.intersect
+0000c3a0: 696f 6e28 6f74 6865 722e 7469 6d65 5f69  ion(other.time_i
+0000c3b0: 6e64 6578 290a 2020 2020 2020 2020 7265  ndex).        re
+0000c3c0: 7475 726e 2073 656c 665b 7469 6d65 5f69  turn self[time_i
+0000c3d0: 6e64 6578 5d0a 0a20 2020 2064 6566 2073  ndex]..    def s
+0000c3e0: 7472 6970 2873 656c 6629 202d 3e20 2754  trip(self) -> 'T
+0000c3f0: 696d 6553 6572 6965 7327 3a0a 2020 2020  imeSeries':.    
+0000c400: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000c410: 5265 7475 726e 7320 6120 5469 6d65 5365  Returns a TimeSe
+0000c420: 7269 6573 2073 6c69 6365 206f 6620 7468  ries slice of th
+0000c430: 6973 2064 6574 6572 6d69 6e69 7374 6963  is deterministic
+0000c440: 2074 696d 6520 7365 7269 6573 2c20 7768   time series, wh
+0000c450: 6572 6520 4e61 4e2d 6f6e 6c79 2065 6e74  ere NaN-only ent
+0000c460: 7269 6573 2061 7420 7468 6520 6265 6769  ries at the begi
+0000c470: 6e6e 696e 670a 2020 2020 2020 2020 616e  nning.        an
+0000c480: 6420 7468 6520 656e 6420 6f66 2074 6865  d the end of the
+0000c490: 2073 6572 6965 7320 6172 6520 7265 6d6f   series are remo
+0000c4a0: 7665 642e 204e 6f20 656e 7472 6965 7320  ved. No entries 
+0000c4b0: 6166 7465 7220 2861 6e64 2069 6e63 6c75  after (and inclu
+0000c4c0: 6469 6e67 2920 7468 6520 6669 7273 7420  ding) the first 
+0000c4d0: 6e6f 6e2d 4e61 4e20 656e 7472 7920 616e  non-NaN entry an
+0000c4e0: 640a 2020 2020 2020 2020 6265 666f 7265  d.        before
+0000c4f0: 2028 616e 6420 696e 636c 7564 696e 6729   (and including)
+0000c500: 2074 6865 206c 6173 7420 6e6f 6e2d 4e61   the last non-Na
+0000c510: 4e20 656e 7472 7920 6172 6520 7265 6d6f  N entry are remo
+0000c520: 7665 642e 0a0a 2020 2020 2020 2020 5468  ved...        Th
+0000c530: 6973 206d 6574 686f 6420 6973 206f 6e6c  is method is onl
+0000c540: 7920 6170 706c 6963 6162 6c65 2074 6f20  y applicable to 
+0000c550: 6465 7465 726d 696e 6973 7469 6320 7365  deterministic se
+0000c560: 7269 6573 2028 692e 652e 2c20 6861 7669  ries (i.e., havi
+0000c570: 6e67 2031 2073 616d 706c 6529 2e0a 0a20  ng 1 sample)... 
+0000c580: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
+0000c590: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
+0000c5a0: 2020 2020 2020 2054 696d 6553 6572 6965         TimeSerie
+0000c5b0: 730a 2020 2020 2020 2020 2020 2020 6120  s.            a 
+0000c5c0: 6e65 7720 7365 7269 6573 2062 6173 6564  new series based
+0000c5d0: 206f 6e20 7468 6520 6f72 6967 696e 616c   on the original
+0000c5e0: 2077 6865 7265 204e 614e 2d6f 6e6c 7920   where NaN-only 
+0000c5f0: 656e 7472 6965 7320 6174 2073 7461 7274  entries at start
+0000c600: 2061 6e64 2065 6e64 2068 6176 6520 6265   and end have be
+0000c610: 656e 2072 656d 6f76 6564 0a20 2020 2020  en removed.     
+0000c620: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+0000c630: 6466 203d 2073 656c 662e 7064 5f64 6174  df = self.pd_dat
+0000c640: 6166 7261 6d65 2863 6f70 793d 4661 6c73  aframe(copy=Fals
+0000c650: 6529 0a20 2020 2020 2020 206e 6577 5f73  e).        new_s
+0000c660: 7461 7274 5f69 6478 203d 2064 662e 6669  tart_idx = df.fi
+0000c670: 7273 745f 7661 6c69 645f 696e 6465 7828  rst_valid_index(
+0000c680: 290a 2020 2020 2020 2020 6e65 775f 656e  ).        new_en
+0000c690: 645f 6964 7820 3d20 6466 2e6c 6173 745f  d_idx = df.last_
+0000c6a0: 7661 6c69 645f 696e 6465 7828 290a 2020  valid_index().  
+0000c6b0: 2020 2020 2020 6e65 775f 7365 7269 6573        new_series
+0000c6c0: 203d 2064 662e 6c6f 635b 6e65 775f 7374   = df.loc[new_st
+0000c6d0: 6172 745f 6964 783a 6e65 775f 656e 645f  art_idx:new_end_
+0000c6e0: 6964 785d 0a20 2020 2020 2020 2072 6574  idx].        ret
+0000c6f0: 7572 6e20 5469 6d65 5365 7269 6573 2e66  urn TimeSeries.f
+0000c700: 726f 6d5f 6461 7461 6672 616d 6528 6e65  rom_dataframe(ne
+0000c710: 775f 7365 7269 6573 290a 0a20 2020 2064  w_series)..    d
+0000c720: 6566 206c 6f6e 6765 7374 5f63 6f6e 7469  ef longest_conti
+0000c730: 6775 6f75 735f 736c 6963 6528 7365 6c66  guous_slice(self
+0000c740: 2c20 6d61 785f 6761 705f 7369 7a65 3a20  , max_gap_size: 
+0000c750: 696e 7420 3d20 3029 202d 3e20 2754 696d  int = 0) -> 'Tim
+0000c760: 6553 6572 6965 7327 3a0a 2020 2020 2020  eSeries':.      
+0000c770: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
+0000c780: 7475 726e 7320 7468 6520 6c61 7267 6573  turns the larges
+0000c790: 7420 5469 6d65 5365 7269 6573 2073 6c69  t TimeSeries sli
+0000c7a0: 6365 206f 6620 7468 6973 2064 6574 6572  ce of this deter
+0000c7b0: 6d69 6e69 7374 6963 2074 696d 6520 7365  ministic time se
+0000c7c0: 7269 6573 2074 6861 7420 636f 6e74 6169  ries that contai
+0000c7d0: 6e73 206e 6f20 6761 7073 0a20 2020 2020  ns no gaps.     
+0000c7e0: 2020 2028 636f 6e74 6967 6f75 7365 2061     (contigouse a
+0000c7f0: 6c6c 2d4e 614e 2072 6f77 7329 206c 6172  ll-NaN rows) lar
+0000c800: 6765 7220 7468 616e 2060 6d61 785f 6761  ger than `max_ga
+0000c810: 705f 7369 7a65 602e 0a0a 2020 2020 2020  p_size`...      
+0000c820: 2020 5468 6973 206d 6574 686f 6420 6973    This method is
+0000c830: 206f 6e6c 7920 6170 706c 6963 6162 6c65   only applicable
+0000c840: 2074 6f20 6465 7465 726d 696e 6973 7469   to deterministi
+0000c850: 6320 7365 7269 6573 2028 692e 652e 2c20  c series (i.e., 
+0000c860: 6861 7669 6e67 2031 2073 616d 706c 6529  having 1 sample)
+0000c870: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+0000c880: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+0000c890: 2d2d 0a20 2020 2020 2020 2054 696d 6553  --.        TimeS
+0000c8a0: 6572 6965 730a 2020 2020 2020 2020 2020  eries.          
+0000c8b0: 2020 6120 6e65 7720 7365 7269 6573 2063    a new series c
+0000c8c0: 6f6e 7374 6974 7574 696e 6720 7468 6520  onstituting the 
+0000c8d0: 6c61 7267 6573 7420 736c 6963 6520 6f66  largest slice of
+0000c8e0: 2074 6865 206f 7269 6769 6e61 6c20 7769   the original wi
+0000c8f0: 7468 206e 6f20 6f72 2062 6f75 6e64 6564  th no or bounded
+0000c900: 2067 6170 730a 2020 2020 2020 2020 2222   gaps.        ""
+0000c910: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
+0000c920: 2028 6e70 2e69 736e 616e 2873 656c 662e   (np.isnan(self.
+0000c930: 5f78 6129 292e 616e 7928 293a 0a20 2020  _xa)).any():.   
+0000c940: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000c950: 7365 6c66 2e63 6f70 7928 290a 2020 2020  self.copy().    
+0000c960: 2020 2020 7374 7269 7070 6564 5f73 6572      stripped_ser
+0000c970: 6965 7320 3d20 7365 6c66 2e73 7472 6970  ies = self.strip
+0000c980: 2829 0a20 2020 2020 2020 2067 6170 7320  ().        gaps 
+0000c990: 3d20 7374 7269 7070 6564 5f73 6572 6965  = stripped_serie
+0000c9a0: 732e 6761 7073 2829 0a20 2020 2020 2020  s.gaps().       
+0000c9b0: 2072 656c 6576 616e 745f 6761 7073 203d   relevant_gaps =
+0000c9c0: 2067 6170 735b 6761 7073 5b27 6761 705f   gaps[gaps['gap_
+0000c9d0: 7369 7a65 275d 203e 206d 6178 5f67 6170  size'] > max_gap
+0000c9e0: 5f73 697a 655d 0a0a 2020 2020 2020 2020  _size]..        
+0000c9f0: 6375 7272 5f73 6c69 6365 5f73 7461 7274  curr_slice_start
+0000ca00: 203d 2073 7472 6970 7065 645f 7365 7269   = stripped_seri
+0000ca10: 6573 2e73 7461 7274 5f74 696d 6528 290a  es.start_time().
+0000ca20: 2020 2020 2020 2020 6d61 785f 7369 7a65          max_size
+0000ca30: 203d 2070 642e 5469 6d65 6465 6c74 6128   = pd.Timedelta(
+0000ca40: 6461 7973 3d30 2920 6966 2073 656c 662e  days=0) if self.
+0000ca50: 5f68 6173 5f64 6174 6574 696d 655f 696e  _has_datetime_in
+0000ca60: 6465 7820 656c 7365 2030 0a20 2020 2020  dex else 0.     
+0000ca70: 2020 206d 6178 5f73 6c69 6365 5f73 7461     max_slice_sta
+0000ca80: 7274 203d 204e 6f6e 650a 2020 2020 2020  rt = None.      
+0000ca90: 2020 6d61 785f 736c 6963 655f 656e 6420    max_slice_end 
+0000caa0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2066  = None.        f
+0000cab0: 6f72 2069 6e64 6578 2c20 726f 7720 696e  or index, row in
+0000cac0: 2072 656c 6576 616e 745f 6761 7073 2e69   relevant_gaps.i
+0000cad0: 7465 7272 6f77 7328 293a 0a20 2020 2020  terrows():.     
+0000cae0: 2020 2020 2020 2073 697a 6520 3d20 726f         size = ro
+0000caf0: 775b 2767 6170 5f73 7461 7274 275d 202d  w['gap_start'] -
+0000cb00: 2063 7572 725f 736c 6963 655f 7374 6172   curr_slice_star
+0000cb10: 7420 2d20 7365 6c66 2e5f 6672 6571 0a20  t - self._freq. 
+0000cb20: 2020 2020 2020 2020 2020 2069 6620 7369             if si
+0000cb30: 7a65 203e 206d 6178 5f73 697a 653a 0a20  ze > max_size:. 
+0000cb40: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0000cb50: 6178 5f73 697a 6520 3d20 7369 7a65 0a20  ax_size = size. 
+0000cb60: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0000cb70: 6178 5f73 6c69 6365 5f73 7461 7274 203d  ax_slice_start =
+0000cb80: 2063 7572 725f 736c 6963 655f 7374 6172   curr_slice_star
+0000cb90: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+0000cba0: 2020 6d61 785f 736c 6963 655f 656e 6420    max_slice_end 
+0000cbb0: 3d20 726f 775b 2767 6170 5f73 7461 7274  = row['gap_start
+0000cbc0: 275d 202d 2073 656c 662e 5f66 7265 710a  '] - self._freq.
+0000cbd0: 2020 2020 2020 2020 2020 2020 6375 7272              curr
+0000cbe0: 5f73 6c69 6365 5f73 7461 7274 203d 2072  _slice_start = r
+0000cbf0: 6f77 5b27 6761 705f 656e 6427 5d20 2b20  ow['gap_end'] + 
+0000cc00: 7365 6c66 2e5f 6672 6571 0a0a 2020 2020  self._freq..    
+0000cc10: 2020 2020 6966 2073 7472 6970 7065 645f      if stripped_
+0000cc20: 7365 7269 6573 2e65 6e64 5f74 696d 6528  series.end_time(
+0000cc30: 2920 2d20 6375 7272 5f73 6c69 6365 5f73  ) - curr_slice_s
+0000cc40: 7461 7274 203e 206d 6178 5f73 697a 653a  tart > max_size:
+0000cc50: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
+0000cc60: 5f73 6c69 6365 5f73 7461 7274 203d 2063  _slice_start = c
+0000cc70: 7572 725f 736c 6963 655f 7374 6172 740a  urr_slice_start.
+0000cc80: 2020 2020 2020 2020 2020 2020 6d61 785f              max_
+0000cc90: 736c 6963 655f 656e 6420 3d20 7365 6c66  slice_end = self
+0000cca0: 2e65 6e64 5f74 696d 6528 290a 0a20 2020  .end_time()..   
+0000ccb0: 2020 2020 2072 6574 7572 6e20 7374 7269       return stri
+0000ccc0: 7070 6564 5f73 6572 6965 735b 6d61 785f  pped_series[max_
+0000ccd0: 736c 6963 655f 7374 6172 743a 6d61 785f  slice_start:max_
+0000cce0: 736c 6963 655f 656e 645d 0a0a 2020 2020  slice_end]..    
+0000ccf0: 6465 6620 7265 7363 616c 655f 7769 7468  def rescale_with
+0000cd00: 5f76 616c 7565 2873 656c 662c 2076 616c  _value(self, val
+0000cd10: 7565 5f61 745f 6669 7273 745f 7374 6570  ue_at_first_step
+0000cd20: 3a20 666c 6f61 7429 202d 3e20 2754 696d  : float) -> 'Tim
+0000cd30: 6553 6572 6965 7327 3a0a 2020 2020 2020  eSeries':.      
+0000cd40: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
+0000cd50: 7475 726e 7320 6120 6e65 7720 5469 6d65  turns a new Time
+0000cd60: 5365 7269 6573 2c20 7768 6963 6820 6973  Series, which is
+0000cd70: 2061 206d 756c 7469 706c 6520 6f66 2074   a multiple of t
+0000cd80: 6869 7320 5469 6d65 5365 7269 6573 2073  his TimeSeries s
+0000cd90: 7563 6820 7468 6174 0a20 2020 2020 2020  uch that.       
+0000cda0: 2074 6865 2066 6972 7374 2076 616c 7565   the first value
+0000cdb0: 2069 7320 6076 616c 7565 5f61 745f 6669   is `value_at_fi
+0000cdc0: 7273 745f 7374 6570 602e 0a20 2020 2020  rst_step`..     
+0000cdd0: 2020 2028 4e6f 7465 3a20 6e75 6d65 7269     (Note: numeri
+0000cde0: 6361 6c20 6572 726f 7273 2063 616e 2061  cal errors can a
+0000cdf0: 7070 6561 7220 7769 7468 2060 7661 6c75  ppear with `valu
+0000ce00: 655f 6174 5f66 6972 7374 5f73 7465 7020  e_at_first_step 
+0000ce10: 3e20 3165 2b32 3460 292e 0a0a 2020 2020  > 1e+24`)...    
+0000ce20: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+0000ce30: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+0000ce40: 2d0a 2020 2020 2020 2020 7661 6c75 655f  -.        value_
+0000ce50: 6174 5f66 6972 7374 5f73 7465 700a 2020  at_first_step.  
+0000ce60: 2020 2020 2020 2020 2020 5468 6520 6e65            The ne
+0000ce70: 7720 7661 6c75 6520 666f 7220 7468 6520  w value for the 
+0000ce80: 6669 7273 7420 656e 7472 7920 6f66 2074  first entry of t
+0000ce90: 6865 2054 696d 6553 6572 6965 732e 0a0a  he TimeSeries...
+0000cea0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+0000ceb0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+0000cec0: 2020 2020 2020 2020 5469 6d65 5365 7269          TimeSeri
+0000ced0: 6573 0a20 2020 2020 2020 2020 2020 2041  es.            A
+0000cee0: 206e 6577 2054 696d 6553 6572 6965 732c   new TimeSeries,
+0000cef0: 2077 6865 7265 2074 6865 2066 6972 7374   where the first
+0000cf00: 2076 616c 7565 2069 7320 6076 616c 7565   value is `value
+0000cf10: 5f61 745f 6669 7273 745f 7374 6570 6020  _at_first_step` 
+0000cf20: 616e 6420 6f74 6865 7220 7661 6c75 6573  and other values
+0000cf30: 0a20 2020 2020 2020 2020 2020 2068 6176  .            hav
+0000cf40: 6520 6265 656e 2073 6361 6c65 6420 6163  e been scaled ac
+0000cf50: 636f 7264 696e 676c 792e 0a20 2020 2020  cordingly..     
+0000cf60: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+0000cf70: 7261 6973 655f 6966 5f6e 6f74 2828 7365  raise_if_not((se
+0000cf80: 6c66 2e5f 7861 5b30 2c20 3a2c 203a 5d20  lf._xa[0, :, :] 
+0000cf90: 213d 2030 292e 616c 6c28 292c 2027 4361  != 0).all(), 'Ca
+0000cfa0: 6e6e 6f74 2072 6573 6361 6c65 2077 6974  nnot rescale wit
+0000cfb0: 6820 6669 7273 7420 7661 6c75 6520 302e  h first value 0.
+0000cfc0: 272c 206c 6f67 6765 7229 0a20 2020 2020  ', logger).     
+0000cfd0: 2020 2063 6f65 6620 3d20 7661 6c75 655f     coef = value_
+0000cfe0: 6174 5f66 6972 7374 5f73 7465 7020 2f20  at_first_step / 
+0000cff0: 7365 6c66 2e5f 7861 2e69 7365 6c28 7b73  self._xa.isel({s
+0000d000: 656c 662e 5f74 696d 655f 6469 6d3a 205b  elf._time_dim: [
+0000d010: 305d 7d29 0a20 2020 2020 2020 2063 6f65  0]}).        coe
+0000d020: 6620 3d20 636f 6566 2e76 616c 7565 732e  f = coef.values.
+0000d030: 7265 7368 6170 6528 2873 656c 662e 6e5f  reshape((self.n_
+0000d040: 636f 6d70 6f6e 656e 7473 2c20 7365 6c66  components, self
+0000d050: 2e6e 5f73 616d 706c 6573 2929 2020 2320  .n_samples))  # 
+0000d060: 544f 444f 3a20 7465 7374 0a20 2020 2020  TODO: test.     
+0000d070: 2020 206e 6577 5f73 6572 6965 7320 3d20     new_series = 
+0000d080: 636f 6566 202a 2073 656c 662e 5f78 610a  coef * self._xa.
+0000d090: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+0000d0a0: 696d 6553 6572 6965 7328 6e65 775f 7365  imeSeries(new_se
+0000d0b0: 7269 6573 290a 0a20 2020 2064 6566 2073  ries)..    def s
+0000d0c0: 6869 6674 2873 656c 662c 206e 3a20 696e  hift(self, n: in
+0000d0d0: 7429 202d 3e20 2754 696d 6553 6572 6965  t) -> 'TimeSerie
+0000d0e0: 7327 3a0a 2020 2020 2020 2020 2222 220a  s':.        """.
+0000d0f0: 2020 2020 2020 2020 5368 6966 7473 2074          Shifts t
+0000d100: 6865 2074 696d 6520 6178 6973 206f 6620  he time axis of 
+0000d110: 7468 6973 2054 696d 6553 6572 6965 7320  this TimeSeries 
+0000d120: 6279 2060 6e60 2074 696d 6520 7374 6570  by `n` time step
+0000d130: 732e 0a0a 2020 2020 2020 2020 4966 203a  s...        If :
+0000d140: 6d61 7468 3a60 6e20 3e20 3060 2c20 7368  math:`n > 0`, sh
+0000d150: 6966 7473 2069 6e20 7468 6520 6675 7475  ifts in the futu
+0000d160: 7265 2e20 4966 203a 6d61 7468 3a60 6e20  re. If :math:`n 
+0000d170: 3c20 3060 2c20 7368 6966 7473 2069 6e20  < 0`, shifts in 
+0000d180: 7468 6520 7061 7374 2e0a 0a20 2020 2020  the past...     
+0000d190: 2020 2046 6f72 2065 7861 6d70 6c65 2c20     For example, 
+0000d1a0: 7769 7468 203a 6d61 7468 3a60 6e3d 3260  with :math:`n=2`
+0000d1b0: 2061 6e64 2060 6672 6571 3d27 4d27 602c   and `freq='M'`,
+0000d1c0: 204d 6172 6368 2032 3031 3320 6265 636f   March 2013 beco
+0000d1d0: 6d65 7320 4d61 7920 3230 3133 2e0a 2020  mes May 2013..  
+0000d1e0: 2020 2020 2020 5769 7468 203a 6d61 7468        With :math
+0000d1f0: 3a60 6e3d 2d32 602c 204d 6172 6368 2032  :`n=-2`, March 2
+0000d200: 3031 3320 6265 636f 6d65 7320 4a61 6e20  013 becomes Jan 
+0000d210: 3230 3133 2e0a 0a20 2020 2020 2020 2050  2013...        P
+0000d220: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+0000d230: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+0000d240: 2020 2020 206e 0a20 2020 2020 2020 2020       n.         
+0000d250: 2020 2054 6865 206e 756d 6265 7220 6f66     The number of
+0000d260: 2074 696d 6520 7374 6570 7320 2869 6e20   time steps (in 
+0000d270: 7365 6c66 2e66 7265 7120 756e 6974 2920  self.freq unit) 
+0000d280: 746f 2073 6869 6674 2062 792e 2043 616e  to shift by. Can
+0000d290: 2062 6520 6e65 6761 7469 7665 2e0a 0a20   be negative... 
+0000d2a0: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
+0000d2b0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
+0000d2c0: 2020 2020 2020 2054 696d 6553 6572 6965         TimeSerie
+0000d2d0: 730a 2020 2020 2020 2020 2020 2020 4120  s.            A 
+0000d2e0: 6e65 7720 5469 6d65 5365 7269 6573 2c20  new TimeSeries, 
+0000d2f0: 7769 7468 2061 2073 6869 6674 6564 2069  with a shifted i
+0000d300: 6e64 6578 2e0a 2020 2020 2020 2020 2222  ndex..        ""
+0000d310: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
+0000d320: 2069 7369 6e73 7461 6e63 6528 6e2c 2028   isinstance(n, (
+0000d330: 696e 742c 206e 702e 696e 7436 3429 293a  int, np.int64)):
+0000d340: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+0000d350: 6765 722e 7761 726e 696e 6728 6622 5469  ger.warning(f"Ti
+0000d360: 6d65 5365 7269 6573 2e73 6869 6674 2829  meSeries.shift()
+0000d370: 3a20 636f 6e76 6572 7469 6e67 206e 2074  : converting n t
+0000d380: 6f20 696e 7420 6672 6f6d 207b 6e7d 2074  o int from {n} t
+0000d390: 6f20 7b69 6e74 286e 297d 2229 0a20 2020  o {int(n)}").   
+0000d3a0: 2020 2020 2020 2020 206e 203d 2069 6e74           n = int
+0000d3b0: 286e 290a 0a20 2020 2020 2020 2074 7279  (n)..        try
+0000d3c0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000d3d0: 6c66 2e5f 7469 6d65 5f69 6e64 6578 5b2d  lf._time_index[-
+0000d3e0: 315d 202b 206e 202a 2073 656c 662e 6672  1] + n * self.fr
+0000d3f0: 6571 0a20 2020 2020 2020 2065 7863 6570  eq.        excep
+0000d400: 7420 7064 2e65 7272 6f72 732e 4f75 744f  t pd.errors.OutO
+0000d410: 6642 6f75 6e64 7344 6174 6574 696d 653a  fBoundsDatetime:
+0000d420: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+0000d430: 7365 5f6c 6f67 284f 7665 7266 6c6f 7745  se_log(OverflowE
+0000d440: 7272 6f72 2822 7468 6520 6164 6420 6f70  rror("the add op
+0000d450: 6572 6174 696f 6e20 6265 7477 6565 6e20  eration between 
+0000d460: 7b7d 2061 6e64 207b 7d20 7769 6c6c 2022  {} and {} will "
+0000d470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d490: 2020 2020 2022 6f76 6572 666c 6f77 222e       "overflow".
+0000d4a0: 666f 726d 6174 286e 202a 2073 656c 662e  format(n * self.
+0000d4b0: 6672 6571 2c20 7365 6c66 2e74 696d 655f  freq, self.time_
+0000d4c0: 696e 6465 785b 2d31 5d29 292c 206c 6f67  index[-1])), log
+0000d4d0: 6765 7229 0a0a 2020 2020 2020 2020 6e65  ger)..        ne
+0000d4e0: 775f 7469 6d65 5f69 6e64 6578 203d 2073  w_time_index = s
+0000d4f0: 656c 662e 5f74 696d 655f 696e 6465 782e  elf._time_index.
+0000d500: 6d61 7028 6c61 6d62 6461 2074 733a 2074  map(lambda ts: t
+0000d510: 7320 2b20 6e20 2a20 7365 6c66 2e66 7265  s + n * self.fre
+0000d520: 7129 0a20 2020 2020 2020 206e 6577 5f78  q).        new_x
+0000d530: 6120 3d20 7365 6c66 2e5f 7861 2e61 7373  a = self._xa.ass
+0000d540: 6967 6e5f 636f 6f72 6473 287b 7365 6c66  ign_coords({self
+0000d550: 2e5f 7861 2e64 696d 735b 305d 3a20 6e65  ._xa.dims[0]: ne
+0000d560: 775f 7469 6d65 5f69 6e64 6578 7d29 0a20  w_time_index}). 
+0000d570: 2020 2020 2020 2072 6574 7572 6e20 5469         return Ti
+0000d580: 6d65 5365 7269 6573 286e 6577 5f78 6129  meSeries(new_xa)
+0000d590: 0a0a 2020 2020 6465 6620 6469 6666 2873  ..    def diff(s
+0000d5a0: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+0000d5b0: 2020 6e3a 204f 7074 696f 6e61 6c5b 696e    n: Optional[in
+0000d5c0: 745d 203d 2031 2c0a 2020 2020 2020 2020  t] = 1,.        
+0000d5d0: 2020 2020 2070 6572 696f 6473 3a20 4f70       periods: Op
+0000d5e0: 7469 6f6e 616c 5b69 6e74 5d20 3d20 312c  tional[int] = 1,
+0000d5f0: 0a20 2020 2020 2020 2020 2020 2020 6472  .             dr
+0000d600: 6f70 6e61 3a20 4f70 7469 6f6e 616c 5b62  opna: Optional[b
+0000d610: 6f6f 6c5d 203d 2054 7275 6529 202d 3e20  ool] = True) -> 
+0000d620: 2754 696d 6553 6572 6965 7327 3a0a 2020  'TimeSeries':.  
+0000d630: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000d640: 2020 5265 7475 726e 7320 6120 6469 6666    Returns a diff
+0000d650: 6572 656e 6365 6420 7469 6d65 2073 6572  erenced time ser
+0000d660: 6965 732e 2054 6869 7320 6973 206f 6674  ies. This is oft
+0000d670: 656e 2075 7365 6420 746f 206d 616b 6520  en used to make 
+0000d680: 6120 7469 6d65 2073 6572 6965 7320 7374  a time series st
+0000d690: 6174 696f 6e61 7279 2e0a 0a20 2020 2020  ationary...     
+0000d6a0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+0000d6b0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+0000d6c0: 0a20 2020 2020 2020 206e 0a20 2020 2020  .        n.     
+0000d6d0: 2020 2020 2020 204f 7074 696f 6e61 6c6c         Optionall
+0000d6e0: 792c 2061 2070 6f73 6974 6976 6520 696e  y, a positive in
+0000d6f0: 7465 6765 7220 696e 6469 6361 7469 6e67  teger indicating
+0000d700: 2074 6865 206e 756d 6265 7220 6f66 2064   the number of d
+0000d710: 6966 6665 7265 6e63 696e 6720 7374 6570  ifferencing step
+0000d720: 7320 2864 6566 6175 6c74 203d 2031 292e  s (default = 1).
+0000d730: 0a20 2020 2020 2020 2020 2020 2046 6f72  .            For
+0000d740: 2069 6e73 7461 6e63 652c 206e 3d32 2063   instance, n=2 c
+0000d750: 6f6d 7075 7465 7320 7468 6520 7365 636f  omputes the seco
+0000d760: 6e64 206f 7264 6572 2064 6966 6665 7265  nd order differe
+0000d770: 6e63 6573 2e0a 2020 2020 2020 2020 7065  nces..        pe
+0000d780: 7269 6f64 730a 2020 2020 2020 2020 2020  riods.          
+0000d790: 2020 4f70 7469 6f6e 616c 6c79 2c20 7065    Optionally, pe
+0000d7a0: 7269 6f64 7320 746f 2073 6869 6674 2066  riods to shift f
+0000d7b0: 6f72 2063 616c 6375 6c61 7469 6e67 2064  or calculating d
+0000d7c0: 6966 6665 7265 6e63 652e 2046 6f72 2069  ifference. For i
+0000d7d0: 6e73 7461 6e63 652c 2070 6572 696f 6473  nstance, periods
+0000d7e0: 3d31 3220 636f 6d70 7574 6573 2074 6865  =12 computes the
+0000d7f0: 0a20 2020 2020 2020 2020 2020 2064 6966  .            dif
+0000d800: 6665 7265 6e63 6520 6265 7477 6565 6e20  ference between 
+0000d810: 7661 6c75 6573 2061 7420 7469 6d65 2060  values at time `
+0000d820: 7460 2061 6e64 2074 696d 6573 2060 742d  t` and times `t-
+0000d830: 3132 602e 0a20 2020 2020 2020 2064 726f  12`..        dro
+0000d840: 706e 610a 2020 2020 2020 2020 2020 2020  pna.            
+0000d850: 5768 6574 6865 7220 746f 2064 726f 7020  Whether to drop 
+0000d860: 7468 6520 6d69 7373 696e 6720 7661 6c75  the missing valu
+0000d870: 6573 2061 6674 6572 2065 6163 6820 6469  es after each di
+0000d880: 6666 6572 656e 6369 6e67 2073 7465 7073  fferencing steps
+0000d890: 2e20 4966 2073 6574 2074 6f20 4661 6c73  . If set to Fals
+0000d8a0: 652c 2074 6865 2063 6f72 7265 7370 6f6e  e, the correspon
+0000d8b0: 6469 6e67 0a20 2020 2020 2020 2020 2020  ding.           
+0000d8c0: 2066 6972 7374 2060 7065 7269 6f64 7360   first `periods`
+0000d8d0: 2074 696d 6520 7374 6570 7320 7769 6c6c   time steps will
+0000d8e0: 2062 6520 6669 6c6c 6564 2077 6974 6820   be filled with 
+0000d8f0: 4e61 4e73 2e0a 0a20 2020 2020 2020 2052  NaNs...        R
+0000d900: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+0000d910: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2054  ------.        T
+0000d920: 696d 6553 6572 6965 730a 2020 2020 2020  imeSeries.      
+0000d930: 2020 2020 2020 4120 5469 6d65 5365 7269        A TimeSeri
+0000d940: 6573 2063 6f6e 7374 7275 6374 6564 2061  es constructed a
+0000d950: 6674 6572 2064 6966 6665 7265 6e63 696e  fter differencin
+0000d960: 672e 0a20 2020 2020 2020 2022 2222 0a20  g..        """. 
+0000d970: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
+0000d980: 696e 7374 616e 6365 286e 2c20 696e 7429  instance(n, int)
+0000d990: 206f 7220 6e20 3c20 313a 0a20 2020 2020   or n < 1:.     
+0000d9a0: 2020 2020 2020 2020 7261 6973 655f 6c6f          raise_lo
+0000d9b0: 6728 5661 6c75 6545 7272 6f72 2822 276e  g(ValueError("'n
+0000d9c0: 2720 6d75 7374 2062 6520 6120 706f 7369  ' must be a posi
+0000d9d0: 7469 7665 2069 6e74 6567 6572 203e 3d20  tive integer >= 
+0000d9e0: 312e 2229 2c20 6c6f 6767 6572 290a 2020  1."), logger).  
+0000d9f0: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
+0000da00: 6e73 7461 6e63 6528 7065 7269 6f64 732c  nstance(periods,
+0000da10: 2069 6e74 2920 6f72 2070 6572 696f 6473   int) or periods
+0000da20: 203c 2031 3a0a 2020 2020 2020 2020 2020   < 1:.          
+0000da30: 2020 2072 6169 7365 5f6c 6f67 2856 616c     raise_log(Val
+0000da40: 7565 4572 726f 7228 2227 7065 7269 6f64  ueError("'period
+0000da50: 7327 206d 7573 7420 6265 2061 6e20 696e  s' must be an in
+0000da60: 7465 6765 7220 3e3d 2031 2e22 292c 206c  teger >= 1."), l
+0000da70: 6f67 6765 7229 0a0a 2020 2020 2020 2020  ogger)..        
+0000da80: 6465 6620 5f63 6f6d 7075 7465 5f64 6966  def _compute_dif
+0000da90: 6628 7861 3a20 7872 2e44 6174 6141 7272  f(xa: xr.DataArr
+0000daa0: 6179 293a 0a20 2020 2020 2020 2020 2020  ay):.           
+0000dab0: 2023 2078 6172 7261 7920 646f 6573 6e27   # xarray doesn'
+0000dac0: 7420 7375 7070 6f72 7420 5061 6e64 6173  t support Pandas
+0000dad0: 2022 7065 7269 6f64 2220 736f 2063 6f6d   "period" so com
+0000dae0: 7075 7465 2064 6966 6628 2920 6f75 7273  pute diff() ours
+0000daf0: 656c 7665 730a 2020 2020 2020 2020 2020  elves.          
+0000db00: 2020 6966 206e 6f74 2064 726f 706e 613a    if not dropna:
+0000db10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000db20: 2023 2049 6e20 7468 6973 2063 6173 6520   # In this case 
+0000db30: 7468 6520 6e65 7720 4461 7461 4172 7261  the new DataArra
+0000db40: 7920 7769 6c6c 2068 6176 6520 7468 6520  y will have the 
+0000db50: 7361 6d65 2073 697a 6520 616e 6420 6669  same size and fi
+0000db60: 6c6c 6564 2077 6974 6820 4e61 4e73 0a20  lled with NaNs. 
+0000db70: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000db80: 6577 5f78 615f 203d 2078 612e 636f 7079  ew_xa_ = xa.copy
+0000db90: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+0000dba0: 2020 206e 6577 5f78 615f 2e76 616c 7565     new_xa_.value
+0000dbb0: 735b 3a70 6572 696f 6473 2c20 3a2c 203a  s[:periods, :, :
+0000dbc0: 5d20 3d20 6e70 2e6e 616e 0a20 2020 2020  ] = np.nan.     
+0000dbd0: 2020 2020 2020 2020 2020 206e 6577 5f78             new_x
+0000dbe0: 615f 2e76 616c 7565 735b 7065 7269 6f64  a_.values[period
+0000dbf0: 733a 2c20 3a2c 203a 5d20 3d20 7861 2e76  s:, :, :] = xa.v
+0000dc00: 616c 7565 735b 7065 7269 6f64 733a 2c20  alues[periods:, 
+0000dc10: 3a2c 203a 5d20 2d20 7861 2e76 616c 7565  :, :] - xa.value
+0000dc20: 735b 3a2d 7065 7269 6f64 732c 203a 2c20  s[:-periods, :, 
+0000dc30: 3a5d 0a20 2020 2020 2020 2020 2020 2065  :].            e
+0000dc40: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000dc50: 2020 2020 2023 2049 6e20 7468 6973 2063       # In this c
+0000dc60: 6173 6520 7468 6520 6e65 7720 4461 7461  ase the new Data
+0000dc70: 4172 7261 7920 7769 6c6c 2062 6520 7368  Array will be sh
+0000dc80: 6f72 7465 720a 2020 2020 2020 2020 2020  orter.          
+0000dc90: 2020 2020 2020 6e65 775f 7861 5f20 3d20        new_xa_ = 
+0000dca0: 7861 5b70 6572 696f 6473 3a2c 203a 2c20  xa[periods:, :, 
+0000dcb0: 3a5d 2e63 6f70 7928 290a 2020 2020 2020  :].copy().      
+0000dcc0: 2020 2020 2020 2020 2020 6e65 775f 7861            new_xa
+0000dcd0: 5f2e 7661 6c75 6573 203d 2078 612e 7661  _.values = xa.va
+0000dce0: 6c75 6573 5b70 6572 696f 6473 3a2c 203a  lues[periods:, :
+0000dcf0: 2c20 3a5d 202d 2078 612e 7661 6c75 6573  , :] - xa.values
+0000dd00: 5b3a 2d70 6572 696f 6473 2c20 3a2c 203a  [:-periods, :, :
+0000dd10: 5d0a 2020 2020 2020 2020 2020 2020 7265  ].            re
+0000dd20: 7475 726e 206e 6577 5f78 615f 0a0a 2020  turn new_xa_..  
+0000dd30: 2020 2020 2020 6e65 775f 7861 203d 205f        new_xa = _
+0000dd40: 636f 6d70 7574 655f 6469 6666 2873 656c  compute_diff(sel
+0000dd50: 662e 5f78 6129 0a20 2020 2020 2020 2066  f._xa).        f
+0000dd60: 6f72 205f 2069 6e20 7261 6e67 6528 6e2d  or _ in range(n-
+0000dd70: 3129 3a0a 2020 2020 2020 2020 2020 2020  1):.            
+0000dd80: 6e65 775f 7861 203d 205f 636f 6d70 7574  new_xa = _comput
+0000dd90: 655f 6469 6666 286e 6577 5f78 6129 0a20  e_diff(new_xa). 
+0000dda0: 2020 2020 2020 2072 6574 7572 6e20 5469         return Ti
+0000ddb0: 6d65 5365 7269 6573 286e 6577 5f78 6129  meSeries(new_xa)
+0000ddc0: 0a0a 2020 2020 6465 6620 6861 735f 7361  ..    def has_sa
+0000ddd0: 6d65 5f74 696d 655f 6173 2873 656c 662c  me_time_as(self,
+0000dde0: 206f 7468 6572 3a20 2754 696d 6553 6572   other: 'TimeSer
+0000ddf0: 6965 7327 2920 2d3e 2062 6f6f 6c3a 0a20  ies') -> bool:. 
+0000de00: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000de10: 2020 2043 6865 636b 7320 7768 6574 6865     Checks whethe
+0000de20: 7220 7468 6973 2054 696d 6553 6572 6965  r this TimeSerie
+0000de30: 7320 616e 6420 616e 6f74 6865 7220 6f6e  s and another on
+0000de40: 6520 6861 7665 2074 6865 2073 616d 6520  e have the same 
+0000de50: 7469 6d65 2069 6e64 6578 2e0a 0a20 2020  time index...   
+0000de60: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+0000de70: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+0000de80: 2d2d 0a20 2020 2020 2020 206f 7468 6572  --.        other
+0000de90: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
+0000dea0: 206f 7468 6572 2073 6572 6965 730a 0a20   other series.. 
+0000deb0: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
+0000dec0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
+0000ded0: 2020 2020 2020 2062 6f6f 6c0a 2020 2020         bool.    
+0000dee0: 2020 2020 2020 2020 5472 7565 2069 6620          True if 
+0000def0: 626f 7468 2054 696d 6553 6572 6965 7320  both TimeSeries 
+0000df00: 6861 7665 2074 6865 2073 616d 6520 696e  have the same in
+0000df10: 6465 782c 2046 616c 7365 206f 7468 6572  dex, False other
+0000df20: 7769 7365 2e0a 2020 2020 2020 2020 2222  wise..        ""
+0000df30: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+0000df40: 2028 6f74 6865 722e 7469 6d65 5f69 6e64   (other.time_ind
+0000df50: 6578 203d 3d20 7365 6c66 2e74 696d 655f  ex == self.time_
+0000df60: 696e 6465 7829 2e61 6c6c 2829 0a0a 2020  index).all()..  
+0000df70: 2020 6465 6620 6170 7065 6e64 2873 656c    def append(sel
+0000df80: 662c 206f 7468 6572 3a20 2754 696d 6553  f, other: 'TimeS
+0000df90: 6572 6965 7327 2920 2d3e 2027 5469 6d65  eries') -> 'Time
+0000dfa0: 5365 7269 6573 273a 0a20 2020 2020 2020  Series':.       
+0000dfb0: 2022 2222 0a20 2020 2020 2020 2041 7070   """.        App
+0000dfc0: 656e 6473 2061 6e6f 7468 6572 2054 696d  ends another Tim
+0000dfd0: 6553 6572 6965 7320 746f 2074 6869 7320  eSeries to this 
+0000dfe0: 5469 6d65 5365 7269 6573 2c20 616c 6f6e  TimeSeries, alon
+0000dff0: 6720 7468 6520 7469 6d65 2061 7869 732e  g the time axis.
+0000e000: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+0000e010: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+0000e020: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+0000e030: 6f74 6865 720a 2020 2020 2020 2020 2020  other.          
+0000e040: 2020 4120 7365 636f 6e64 2054 696d 6553    A second TimeS
+0000e050: 6572 6965 732e 0a0a 2020 2020 2020 2020  eries...        
+0000e060: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+0000e070: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+0000e080: 5469 6d65 5365 7269 6573 0a20 2020 2020  TimeSeries.     
+0000e090: 2020 2020 2020 2041 206e 6577 2054 696d         A new Tim
+0000e0a0: 6553 6572 6965 732c 206f 6274 6169 6e65  eSeries, obtaine
+0000e0b0: 6420 6279 2061 7070 656e 6469 6e67 2074  d by appending t
+0000e0c0: 6865 2073 6563 6f6e 6420 5469 6d65 5365  he second TimeSe
+0000e0d0: 7269 6573 2074 6f20 7468 6520 6669 7273  ries to the firs
+0000e0e0: 742e 0a20 2020 2020 2020 2022 2222 0a20  t..        """. 
+0000e0f0: 2020 2020 2020 2072 6169 7365 5f69 665f         raise_if_
+0000e100: 6e6f 7428 6f74 6865 722e 6861 735f 6461  not(other.has_da
+0000e110: 7465 7469 6d65 5f69 6e64 6578 203d 3d20  tetime_index == 
+0000e120: 7365 6c66 2e68 6173 5f64 6174 6574 696d  self.has_datetim
+0000e130: 655f 696e 6465 782c 0a20 2020 2020 2020  e_index,.       
+0000e140: 2020 2020 2020 2020 2020 2020 2020 2742                'B
+0000e150: 6f74 6820 7365 7269 6573 206d 7573 7420  oth series must 
+0000e160: 6861 7665 2074 6865 2073 616d 6520 7479  have the same ty
+0000e170: 7065 206f 6620 7469 6d65 2069 6e64 6578  pe of time index
+0000e180: 2028 6569 7468 6572 2044 6174 6574 696d   (either Datetim
+0000e190: 6549 6e64 6578 206f 7220 496e 7436 3449  eIndex or Int64I
+0000e1a0: 6e64 6578 292e 272c 206c 6f67 6765 7229  ndex).', logger)
+0000e1b0: 0a20 2020 2020 2020 2072 6169 7365 5f69  .        raise_i
+0000e1c0: 665f 6e6f 7428 6f74 6865 722e 6672 6571  f_not(other.freq
+0000e1d0: 203d 3d20 7365 6c66 2e66 7265 712c 0a20   == self.freq,. 
+0000e1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1f0: 2020 2020 2741 7070 656e 6465 6420 5469      'Appended Ti
+0000e200: 6d65 5365 7269 6573 206d 7573 7420 6861  meSeries must ha
+0000e210: 7665 2074 6865 2073 616d 6520 6672 6571  ve the same freq
+0000e220: 7565 6e63 7920 6173 2074 6865 2063 7572  uency as the cur
+0000e230: 7265 6e74 206f 6e65 272c 206c 6f67 6765  rent one', logge
+0000e240: 7229 0a20 2020 2020 2020 2072 6169 7365  r).        raise
+0000e250: 5f69 665f 6e6f 7428 6f74 6865 722e 6e5f  _if_not(other.n_
+0000e260: 636f 6d70 6f6e 656e 7473 203d 3d20 7365  components == se
+0000e270: 6c66 2e6e 5f63 6f6d 706f 6e65 6e74 732c  lf.n_components,
+0000e280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e290: 2020 2020 2020 2742 6f74 6820 7365 7269        'Both seri
+0000e2a0: 6573 206d 7573 7420 6861 7665 2074 6865  es must have the
+0000e2b0: 2073 616d 6520 6e75 6d62 6572 206f 6620   same number of 
+0000e2c0: 636f 6d70 6f6e 656e 7473 2e27 2c20 6c6f  components.', lo
+0000e2d0: 6767 6572 290a 2020 2020 2020 2020 7261  gger).        ra
+0000e2e0: 6973 655f 6966 5f6e 6f74 286f 7468 6572  ise_if_not(other
+0000e2f0: 2e6e 5f73 616d 706c 6573 203d 3d20 7365  .n_samples == se
+0000e300: 6c66 2e6e 5f73 616d 706c 6573 2c0a 2020  lf.n_samples,.  
+0000e310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e320: 2020 2027 426f 7468 2073 6572 6965 7320     'Both series 
+0000e330: 6d75 7374 2068 6176 6520 7468 6520 7361  must have the sa
+0000e340: 6d65 206e 756d 6265 7220 6f66 2063 6f6d  me number of com
+0000e350: 706f 6e65 6e74 732e 272c 206c 6f67 6765  ponents.', logge
+0000e360: 7229 0a20 2020 2020 2020 2069 6620 7365  r).        if se
+0000e370: 6c66 2e5f 6861 735f 6461 7465 7469 6d65  lf._has_datetime
+0000e380: 5f69 6e64 6578 3a0a 2020 2020 2020 2020  _index:.        
+0000e390: 2020 2020 7261 6973 655f 6966 5f6e 6f74      raise_if_not
+0000e3a0: 286f 7468 6572 2e73 7461 7274 5f74 696d  (other.start_tim
+0000e3b0: 6528 2920 3d3d 2073 656c 662e 656e 645f  e() == self.end_
+0000e3c0: 7469 6d65 2829 202b 2073 656c 662e 6672  time() + self.fr
+0000e3d0: 6571 2c0a 2020 2020 2020 2020 2020 2020  eq,.            
+0000e3e0: 2020 2020 2020 2020 2020 2020 2027 4170               'Ap
+0000e3f0: 7065 6e64 6564 2054 696d 6553 6572 6965  pended TimeSerie
+0000e400: 7320 6d75 7374 2073 7461 7274 206f 6e65  s must start one
+0000e410: 2074 696d 6520 7374 6570 2061 6674 6572   time step after
+0000e420: 2063 7572 7265 6e74 206f 6e65 2e27 2c20   current one.', 
+0000e430: 6c6f 6767 6572 290a 0a20 2020 2020 2020  logger)..       
+0000e440: 206f 7468 6572 5f78 6120 3d20 6f74 6865   other_xa = othe
+0000e450: 722e 6461 7461 5f61 7272 6179 2829 0a0a  r.data_array()..
+0000e460: 2020 2020 2020 2020 6e65 775f 7861 203d          new_xa =
+0000e470: 2078 722e 4461 7461 4172 7261 7928 6e70   xr.DataArray(np
+0000e480: 2e63 6f6e 6361 7465 6e61 7465 2828 7365  .concatenate((se
+0000e490: 6c66 2e5f 7861 2e76 616c 7565 732c 206f  lf._xa.values, o
+0000e4a0: 7468 6572 5f78 612e 7661 6c75 6573 292c  ther_xa.values),
+0000e4b0: 2061 7869 733d 3029 2c0a 2020 2020 2020   axis=0),.      
 0000e4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4e0: 2768 6176 6520 7468 6520 7361 6d65 206e  'have the same n
-0000e4f0: 756d 6265 7220 6f66 2073 616d 706c 6573  umber of samples
-0000e500: 2e27 2c20 6c6f 6767 6572 290a 0a20 2020  .', logger)..   
-0000e510: 2020 2020 206f 7468 6572 5f78 6120 3d20       other_xa = 
-0000e520: 6f74 6865 722e 6461 7461 5f61 7272 6179  other.data_array
-0000e530: 2863 6f70 793d 4661 6c73 6529 0a20 2020  (copy=False).   
-0000e540: 2020 2020 2069 6620 6f74 6865 725f 7861       if other_xa
-0000e550: 2e64 696d 735b 305d 2021 3d20 7365 6c66  .dims[0] != self
-0000e560: 2e5f 7469 6d65 5f64 696d 3a0a 2020 2020  ._time_dim:.    
-0000e570: 2020 2020 2020 2020 6e65 775f 6f74 6865          new_othe
-0000e580: 725f 7861 203d 2078 722e 4461 7461 4172  r_xa = xr.DataAr
-0000e590: 7261 7928 6f74 6865 725f 7861 2e76 616c  ray(other_xa.val
-0000e5a0: 7565 732c 0a20 2020 2020 2020 2020 2020  ues,.           
-0000e5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5c0: 2020 2020 2020 2020 2020 2020 2064 696d               dim
-0000e5d0: 733d 7365 6c66 2e5f 7861 2e64 696d 732c  s=self._xa.dims,
-0000e5e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e600: 2020 2020 2020 2020 2063 6f6f 7264 733d           coords=
-0000e610: 7b73 656c 662e 5f74 696d 655f 6469 6d3a  {self._time_dim:
-0000e620: 2073 656c 662e 5f74 696d 655f 696e 6465   self._time_inde
-0000e630: 782c 2044 494d 535b 315d 3a20 6f74 6865  x, DIMS[1]: othe
-0000e640: 722e 636f 6d70 6f6e 656e 7473 7d29 0a20  r.components}). 
-0000e650: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000e660: 2020 2020 2020 2020 206e 6577 5f6f 7468           new_oth
-0000e670: 6572 5f78 6120 3d20 6f74 6865 725f 7861  er_xa = other_xa
-0000e680: 0a0a 2020 2020 2020 2020 6e65 775f 7861  ..        new_xa
-0000e690: 203d 2078 722e 636f 6e63 6174 2828 7365   = xr.concat((se
-0000e6a0: 6c66 2e5f 7861 2c20 6e65 775f 6f74 6865  lf._xa, new_othe
-0000e6b0: 725f 7861 292c 2064 696d 3d44 494d 535b  r_xa), dim=DIMS[
-0000e6c0: 315d 290a 0a20 2020 2020 2020 2023 2077  1])..        # w
-0000e6d0: 6520 6361 6c6c 2074 6865 2066 6163 746f  e call the facto
-0000e6e0: 7279 206d 6574 686f 6420 6865 7265 2074  ry method here t
-0000e6f0: 6f20 6469 7361 6d62 6967 7561 7465 2063  o disambiguate c
-0000e700: 6f6c 756d 6e20 6e61 6d65 7320 6966 206e  olumn names if n
-0000e710: 6565 6465 642e 0a20 2020 2020 2020 2072  eeded..        r
-0000e720: 6574 7572 6e20 5469 6d65 5365 7269 6573  eturn TimeSeries
-0000e730: 2e66 726f 6d5f 7861 7272 6179 286e 6577  .from_xarray(new
-0000e740: 5f78 612c 2066 696c 6c5f 6d69 7373 696e  _xa, fill_missin
-0000e750: 675f 6461 7465 733d 4661 6c73 6529 0a0a  g_dates=False)..
-0000e760: 2020 2020 6465 6620 756e 6976 6172 6961      def univaria
-0000e770: 7465 5f63 6f6d 706f 6e65 6e74 2873 656c  te_component(sel
-0000e780: 662c 2069 6e64 6578 3a20 556e 696f 6e5b  f, index: Union[
-0000e790: 7374 722c 2069 6e74 5d29 202d 3e20 2754  str, int]) -> 'T
-0000e7a0: 696d 6553 6572 6965 7327 3a0a 2020 2020  imeSeries':.    
-0000e7b0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000e7c0: 5265 7472 6965 7665 7320 6f6e 6520 6f66  Retrieves one of
-0000e7d0: 2074 6865 2063 6f6d 706f 6e65 6e74 7320   the components 
-0000e7e0: 6f66 2074 6865 2063 7572 7265 6e74 2054  of the current T
-0000e7f0: 696d 6553 6572 6965 7320 696e 7374 616e  imeSeries instan
-0000e800: 6365 0a20 2020 2020 2020 2061 6e64 2072  ce.        and r
-0000e810: 6574 7572 6e73 2069 7420 6173 206e 6577  eturns it as new
-0000e820: 2075 6e69 7661 7269 6174 6520 5469 6d65   univariate Time
-0000e830: 5365 7269 6573 2069 6e73 7461 6e63 652e  Series instance.
-0000e840: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-0000e850: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-0000e860: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-0000e870: 696e 6465 780a 2020 2020 2020 2020 2020  index.          
-0000e880: 2020 416e 207a 6572 6f2d 696e 6465 7865    An zero-indexe
-0000e890: 6420 696e 7465 6765 7220 696e 6469 6361  d integer indica
-0000e8a0: 7469 6e67 2077 6869 6368 2063 6f6d 706f  ting which compo
-0000e8b0: 6e65 6e74 2074 6f20 7265 7472 6965 7665  nent to retrieve
-0000e8c0: 2e20 4966 2063 6f6d 706f 6e65 6e74 7320  . If components 
-0000e8d0: 6861 7665 206e 616d 6573 2c0a 2020 2020  have names,.    
-0000e8e0: 2020 2020 2020 2020 7468 6973 2063 616e          this can
-0000e8f0: 2062 6520 6120 7374 7269 6e67 2077 6974   be a string wit
-0000e900: 6820 7468 6520 636f 6d70 6f6e 656e 7427  h the component'
-0000e910: 7320 6e61 6d65 2e0a 0a20 2020 2020 2020  s name...       
-0000e920: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-0000e930: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-0000e940: 2054 696d 6553 6572 6965 730a 2020 2020   TimeSeries.    
-0000e950: 2020 2020 2020 2020 4120 6e65 7720 756e          A new un
-0000e960: 6976 6172 6961 7465 2054 696d 6553 6572  ivariate TimeSer
-0000e970: 6965 7320 696e 7374 616e 6365 2e0a 2020  ies instance..  
-0000e980: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000e990: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-0000e9a0: 696e 6465 782c 2069 6e74 293a 0a20 2020  index, int):.   
-0000e9b0: 2020 2020 2020 2020 206e 6577 5f78 6120           new_xa 
-0000e9c0: 3d20 7365 6c66 2e5f 7861 2e69 7365 6c28  = self._xa.isel(
-0000e9d0: 636f 6d70 6f6e 656e 743d 696e 6465 7829  component=index)
-0000e9e0: 2e65 7870 616e 645f 6469 6d73 2844 494d  .expand_dims(DIM
-0000e9f0: 535b 315d 2c20 6178 6973 3d31 290a 2020  S[1], axis=1).  
-0000ea00: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000ea10: 2020 2020 2020 2020 6e65 775f 7861 203d          new_xa =
-0000ea20: 2073 656c 662e 5f78 612e 7365 6c28 636f   self._xa.sel(co
-0000ea30: 6d70 6f6e 656e 743d 696e 6465 7829 2e65  mponent=index).e
-0000ea40: 7870 616e 645f 6469 6d73 2844 494d 535b  xpand_dims(DIMS[
-0000ea50: 315d 2c20 6178 6973 3d31 290a 2020 2020  1], axis=1).    
-0000ea60: 2020 2020 7265 7475 726e 2054 696d 6553      return TimeS
-0000ea70: 6572 6965 7328 6e65 775f 7861 290a 0a20  eries(new_xa).. 
-0000ea80: 2020 2064 6566 2061 6464 5f64 6174 6574     def add_datet
-0000ea90: 696d 655f 6174 7472 6962 7574 6528 7365  ime_attribute(se
-0000eaa0: 6c66 2c20 6174 7472 6962 7574 652c 206f  lf, attribute, o
-0000eab0: 6e65 5f68 6f74 3a20 626f 6f6c 203d 2046  ne_hot: bool = F
-0000eac0: 616c 7365 2920 2d3e 2027 5469 6d65 5365  alse) -> 'TimeSe
+0000e4d0: 2020 2020 2020 2020 6469 6d73 3d73 656c          dims=sel
+0000e4e0: 662e 5f78 612e 6469 6d73 2c0a 2020 2020  f._xa.dims,.    
+0000e4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e500: 2020 2020 2020 2020 2020 636f 6f72 6473            coords
+0000e510: 3d7b 7365 6c66 2e5f 7469 6d65 5f64 696d  ={self._time_dim
+0000e520: 3a20 7365 6c66 2e5f 7469 6d65 5f69 6e64  : self._time_ind
+0000e530: 6578 2e61 7070 656e 6428 6f74 6865 722e  ex.append(other.
+0000e540: 7469 6d65 5f69 6e64 6578 292c 0a20 2020  time_index),.   
+0000e550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e570: 2020 2044 494d 535b 315d 3a20 7365 6c66     DIMS[1]: self
+0000e580: 2e63 6f6d 706f 6e65 6e74 737d 290a 0a20  .components}).. 
+0000e590: 2020 2020 2020 2023 206e 6577 5f78 6120         # new_xa 
+0000e5a0: 3d20 7872 2e63 6f6e 6361 7428 6f62 6a73  = xr.concat(objs
+0000e5b0: 3d5b 7365 6c66 2e5f 7861 2c20 6f74 6865  =[self._xa, othe
+0000e5c0: 725f 7861 5d2c 2064 696d 3d73 7472 2873  r_xa], dim=str(s
+0000e5d0: 656c 662e 5f74 696d 655f 6469 6d29 290a  elf._time_dim)).
+0000e5e0: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+0000e5f0: 656c 662e 5f68 6173 5f64 6174 6574 696d  elf._has_datetim
+0000e600: 655f 696e 6465 783a 0a20 2020 2020 2020  e_index:.       
+0000e610: 2020 2020 206e 6577 5f78 6120 3d20 6e65       new_xa = ne
+0000e620: 775f 7861 2e72 6573 6574 5f69 6e64 6578  w_xa.reset_index
+0000e630: 2864 696d 735f 6f72 5f6c 6576 656c 733d  (dims_or_levels=
+0000e640: 6e65 775f 7861 2e64 696d 735b 305d 290a  new_xa.dims[0]).
+0000e650: 0a20 2020 2020 2020 2023 2054 4f44 4f3a  .        # TODO:
+0000e660: 2066 696c 6c5f 6d69 7373 696e 675f 6461   fill_missing_da
+0000e670: 7465 7320 7461 6b65 7320 6120 7065 7266  tes takes a perf
+0000e680: 6f72 6d61 6e63 6520 6869 743b 2064 6f20  ormance hit; do 
+0000e690: 7765 206e 6565 6420 6974 2068 6572 650a  we need it here.
+0000e6a0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+0000e6b0: 696d 6553 6572 6965 732e 6672 6f6d 5f78  imeSeries.from_x
+0000e6c0: 6172 7261 7928 6e65 775f 7861 2c20 6669  array(new_xa, fi
+0000e6d0: 6c6c 5f6d 6973 7369 6e67 5f64 6174 6573  ll_missing_dates
+0000e6e0: 3d54 7275 652c 2066 7265 713d 7365 6c66  =True, freq=self
+0000e6f0: 2e5f 6672 6571 5f73 7472 290a 0a20 2020  ._freq_str)..   
+0000e700: 2064 6566 2061 7070 656e 645f 7661 6c75   def append_valu
+0000e710: 6573 2873 656c 662c 2076 616c 7565 733a  es(self, values:
+0000e720: 206e 702e 6e64 6172 7261 7929 202d 3e20   np.ndarray) -> 
+0000e730: 2754 696d 6553 6572 6965 7327 3a0a 2020  'TimeSeries':.  
+0000e740: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000e750: 2020 4170 7065 6e64 7320 7661 6c75 6573    Appends values
+0000e760: 2074 6f20 6375 7272 656e 7420 5469 6d65   to current Time
+0000e770: 5365 7269 6573 2c20 746f 2074 6865 2067  Series, to the g
+0000e780: 6976 656e 2069 6e64 6963 6573 2e0a 0a20  iven indices... 
+0000e790: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+0000e7a0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0000e7b0: 2d2d 2d2d 0a20 2020 2020 2020 2076 616c  ----.        val
+0000e7c0: 7565 730a 2020 2020 2020 2020 2020 2020  ues.            
+0000e7d0: 416e 2061 7272 6179 2077 6974 6820 7468  An array with th
+0000e7e0: 6520 7661 6c75 6573 2074 6f20 6170 7065  e values to appe
+0000e7f0: 6e64 2e0a 0a20 2020 2020 2020 2052 6574  nd...        Ret
+0000e800: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+0000e810: 2d2d 2d2d 0a20 2020 2020 2020 2054 696d  ----.        Tim
+0000e820: 6553 6572 6965 730a 2020 2020 2020 2020  eSeries.        
+0000e830: 2020 2020 4120 6e65 7720 5469 6d65 5365      A new TimeSe
+0000e840: 7269 6573 2077 6974 6820 7468 6520 6e65  ries with the ne
+0000e850: 7720 7661 6c75 6573 2061 7070 656e 6465  w values appende
+0000e860: 640a 2020 2020 2020 2020 2222 220a 0a20  d.        """.. 
+0000e870: 2020 2020 2020 2023 2054 4f44 4f20 7465         # TODO te
+0000e880: 7374 0a20 2020 2020 2020 2069 6620 7365  st.        if se
+0000e890: 6c66 2e5f 6861 735f 6461 7465 7469 6d65  lf._has_datetime
+0000e8a0: 5f69 6e64 6578 3a0a 2020 2020 2020 2020  _index:.        
+0000e8b0: 2020 2020 6964 7820 3d20 7064 2e44 6174      idx = pd.Dat
+0000e8c0: 6574 696d 6549 6e64 6578 285b 7365 6c66  etimeIndex([self
+0000e8d0: 2e65 6e64 5f74 696d 6528 2920 2b20 6920  .end_time() + i 
+0000e8e0: 2a20 7365 6c66 2e5f 6672 6571 2066 6f72  * self._freq for
+0000e8f0: 2069 2069 6e20 7261 6e67 6528 312c 206c   i in range(1, l
+0000e900: 656e 2876 616c 7565 7329 2b31 295d 2c20  en(values)+1)], 
+0000e910: 6672 6571 3d73 656c 662e 5f66 7265 7129  freq=self._freq)
+0000e920: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0000e930: 2020 2020 2020 2020 2020 2069 6478 203d             idx =
+0000e940: 2070 642e 5261 6e67 6549 6e64 6578 286c   pd.RangeIndex(l
+0000e950: 656e 2873 656c 6629 2c20 6c65 6e28 7365  en(self), len(se
+0000e960: 6c66 292b 6c65 6e28 7661 6c75 6573 292c  lf)+len(values),
+0000e970: 2031 290a 0a20 2020 2020 2020 2072 6574   1)..        ret
+0000e980: 7572 6e20 7365 6c66 2e61 7070 656e 6428  urn self.append(
+0000e990: 5469 6d65 5365 7269 6573 2e66 726f 6d5f  TimeSeries.from_
+0000e9a0: 7469 6d65 735f 616e 645f 7661 6c75 6573  times_and_values
+0000e9b0: 2876 616c 7565 733d 7661 6c75 6573 2c0a  (values=values,.
+0000e9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9f0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+0000ea00: 733d 6964 782c 0a20 2020 2020 2020 2020  s=idx,.         
+0000ea10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea40: 2020 2066 696c 6c5f 6d69 7373 696e 675f     fill_missing_
+0000ea50: 6461 7465 733d 4661 6c73 6529 290a 0a20  dates=False)).. 
+0000ea60: 2020 2064 6566 2075 7064 6174 6528 7365     def update(se
+0000ea70: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
+0000ea80: 2020 2069 6e64 6578 3a20 7064 2e44 6174     index: pd.Dat
+0000ea90: 6574 696d 6549 6e64 6578 2c0a 2020 2020  etimeIndex,.    
+0000eaa0: 2020 2020 2020 2020 2020 2076 616c 7565             value
+0000eab0: 733a 206e 702e 6e64 6172 7261 7920 3d20  s: np.ndarray = 
+0000eac0: 4e6f 6e65 2920 2d3e 2027 5469 6d65 5365  None) -> 'TimeSe
 0000ead0: 7269 6573 273a 0a20 2020 2020 2020 2022  ries':.        "
-0000eae0: 2222 0a20 2020 2020 2020 2052 6574 7572  "".        Retur
-0000eaf0: 6e73 2061 206e 6577 2054 696d 6553 6572  ns a new TimeSer
-0000eb00: 6965 7320 696e 7374 616e 6365 2077 6974  ies instance wit
-0000eb10: 6820 6f6e 6520 286f 7220 6d6f 7265 2920  h one (or more) 
-0000eb20: 6164 6469 7469 6f6e 616c 2063 6f6d 706f  additional compo
-0000eb30: 6e65 6e74 2873 2920 7468 6174 2063 6f6e  nent(s) that con
-0000eb40: 7461 696e 2061 6e20 6174 7472 6962 7574  tain an attribut
-0000eb50: 650a 2020 2020 2020 2020 6f66 2074 6865  e.        of the
-0000eb60: 2074 696d 6520 696e 6465 7820 6f66 2074   time index of t
-0000eb70: 6865 2063 7572 7265 6e74 2073 6572 6965  he current serie
-0000eb80: 7320 7370 6563 6966 6965 6420 7769 7468  s specified with
-0000eb90: 2060 6174 7472 6962 7574 6560 2c20 7375   `attribute`, su
-0000eba0: 6368 2061 7320 2777 6565 6b64 6179 272c  ch as 'weekday',
-0000ebb0: 2027 6461 7927 206f 7220 276d 6f6e 7468   'day' or 'month
-0000ebc0: 272e 0a0a 2020 2020 2020 2020 5468 6973  '...        This
-0000ebd0: 2077 6f72 6b73 206f 6e6c 7920 666f 7220   works only for 
-0000ebe0: 6465 7465 726d 696e 6973 7469 6320 7469  deterministic ti
-0000ebf0: 6d65 2073 6572 6965 7320 2869 2e65 2e2c  me series (i.e.,
-0000ec00: 206d 6164 6520 6f66 2031 2073 616d 706c   made of 1 sampl
-0000ec10: 6529 2e0a 0a20 2020 2020 2020 2050 6172  e)...        Par
-0000ec20: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-0000ec30: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-0000ec40: 2020 2061 7474 7269 6275 7465 0a20 2020     attribute.   
-0000ec50: 2020 2020 2020 2020 2041 2070 642e 4461           A pd.Da
-0000ec60: 7461 7469 6d65 496e 6465 7820 6174 7472  tatimeIndex attr
-0000ec70: 6962 7574 6520 7768 6963 6820 7769 6c6c  ibute which will
-0000ec80: 2073 6572 7665 2061 7320 7468 6520 6261   serve as the ba
-0000ec90: 7369 7320 6f66 2074 6865 206e 6577 2063  sis of the new c
-0000eca0: 6f6c 756d 6e28 7329 2e0a 2020 2020 2020  olumn(s)..      
-0000ecb0: 2020 6f6e 655f 686f 740a 2020 2020 2020    one_hot.      
-0000ecc0: 2020 2020 2020 426f 6f6c 6561 6e20 7661        Boolean va
-0000ecd0: 6c75 6520 696e 6469 6361 7469 6e67 2077  lue indicating w
-0000ece0: 6865 7468 6572 2074 6f20 6164 6420 7468  hether to add th
-0000ecf0: 6520 7370 6563 6966 6965 6420 6174 7472  e specified attr
-0000ed00: 6962 7574 6520 6173 2061 206f 6e65 2068  ibute as a one h
-0000ed10: 6f74 2065 6e63 6f64 696e 670a 2020 2020  ot encoding.    
-0000ed20: 2020 2020 2020 2020 2872 6573 756c 7473          (results
-0000ed30: 2069 6e20 6d6f 7265 2063 6f6c 756d 6e73   in more columns
-0000ed40: 292e 0a0a 2020 2020 2020 2020 5265 7475  )...        Retu
-0000ed50: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-0000ed60: 2d2d 2d0a 2020 2020 2020 2020 5469 6d65  ---.        Time
-0000ed70: 5365 7269 6573 0a20 2020 2020 2020 2020  Series.         
-0000ed80: 2020 204e 6577 2054 696d 6553 6572 6965     New TimeSerie
-0000ed90: 7320 696e 7374 616e 6365 2065 6e68 616e  s instance enhan
-0000eda0: 6365 6420 6279 2060 6174 7472 6962 7574  ced by `attribut
-0000edb0: 6560 2e0a 2020 2020 2020 2020 2222 220a  e`..        """.
-0000edc0: 2020 2020 2020 2020 7365 6c66 2e5f 6173          self._as
-0000edd0: 7365 7274 5f64 6574 6572 6d69 6e69 7374  sert_determinist
-0000ede0: 6963 2829 0a20 2020 2020 2020 2066 726f  ic().        fro
-0000edf0: 6d20 2e75 7469 6c73 2069 6d70 6f72 7420  m .utils import 
-0000ee00: 7469 6d65 7365 7269 6573 5f67 656e 6572  timeseries_gener
-0000ee10: 6174 696f 6e20 6173 2074 670a 2020 2020  ation as tg.    
-0000ee20: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0000ee30: 7374 6163 6b28 7467 2e64 6174 6574 696d  stack(tg.datetim
-0000ee40: 655f 6174 7472 6962 7574 655f 7469 6d65  e_attribute_time
-0000ee50: 7365 7269 6573 2873 656c 662e 7469 6d65  series(self.time
-0000ee60: 5f69 6e64 6578 2c20 6174 7472 6962 7574  _index, attribut
-0000ee70: 652c 206f 6e65 5f68 6f74 2929 0a0a 2020  e, one_hot))..  
-0000ee80: 2020 6465 6620 6164 645f 686f 6c69 6461    def add_holida
-0000ee90: 7973 2873 656c 662c 0a20 2020 2020 2020  ys(self,.       
-0000eea0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000eeb0: 756e 7472 795f 636f 6465 3a20 7374 722c  untry_code: str,
-0000eec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000eed0: 2020 2020 2020 7072 6f76 3a20 7374 7220        prov: str 
-0000eee0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000eef0: 2020 2020 2020 2020 2020 2020 2073 7461               sta
-0000ef00: 7465 3a20 7374 7220 3d20 4e6f 6e65 2920  te: str = None) 
-0000ef10: 2d3e 2027 5469 6d65 5365 7269 6573 273a  -> 'TimeSeries':
-0000ef20: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000ef30: 2020 2020 2041 6464 7320 6120 6269 6e61       Adds a bina
-0000ef40: 7279 2075 6e69 7661 7269 6174 6520 636f  ry univariate co
-0000ef50: 6d70 6f6e 656e 7420 746f 2074 6865 2063  mponent to the c
-0000ef60: 7572 7265 6e74 2073 6572 6965 7320 7468  urrent series th
-0000ef70: 6174 2065 7175 616c 7320 3120 6174 2065  at equals 1 at e
-0000ef80: 7665 7279 2069 6e64 6578 2074 6861 740a  very index that.
-0000ef90: 2020 2020 2020 2020 636f 7272 6573 706f          correspo
-0000efa0: 6e64 7320 746f 2073 656c 6563 7465 6420  nds to selected 
-0000efb0: 636f 756e 7472 7927 7320 686f 6c69 6461  country's holida
-0000efc0: 792c 2061 6e64 2030 206f 7468 6572 7769  y, and 0 otherwi
-0000efd0: 7365 2e20 5468 6520 6672 6571 7565 6e63  se. The frequenc
-0000efe0: 7920 6f66 2074 6865 2054 696d 6553 6572  y of the TimeSer
-0000eff0: 6965 7320 6973 2064 6169 6c79 2e0a 0a20  ies is daily... 
-0000f000: 2020 2020 2020 2041 7661 696c 6162 6c65         Available
-0000f010: 2063 6f75 6e74 7269 6573 2063 616e 2062   countries can b
-0000f020: 6520 666f 756e 6420 6068 6572 6520 3c68  e found `here <h
-0000f030: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-0000f040: 6d2f 6472 2d70 726f 6469 6779 2f70 7974  m/dr-prodigy/pyt
-0000f050: 686f 6e2d 686f 6c69 6461 7973 2361 7661  hon-holidays#ava
-0000f060: 696c 6162 6c65 2d63 6f75 6e74 7269 6573  ilable-countries
-0000f070: 3e60 5f2e 0a0a 2020 2020 2020 2020 5468  >`_...        Th
-0000f080: 6973 2077 6f72 6b73 206f 6e6c 7920 666f  is works only fo
-0000f090: 7220 6465 7465 726d 696e 6973 7469 6320  r deterministic 
-0000f0a0: 7469 6d65 2073 6572 6965 7320 2869 2e65  time series (i.e
-0000f0b0: 2e2c 206d 6164 6520 6f66 2031 2073 616d  ., made of 1 sam
-0000f0c0: 706c 6529 2e0a 0a20 2020 2020 2020 2050  ple)...        P
-0000f0d0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-0000f0e0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-0000f0f0: 2020 2020 2063 6f75 6e74 7279 5f63 6f64       country_cod
-0000f100: 650a 2020 2020 2020 2020 2020 2020 5468  e.            Th
-0000f110: 6520 636f 756e 7472 7920 4953 4f20 636f  e country ISO co
-0000f120: 6465 0a20 2020 2020 2020 2070 726f 760a  de.        prov.
-0000f130: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-0000f140: 7072 6f76 696e 6365 0a20 2020 2020 2020  province.       
-0000f150: 2073 7461 7465 0a20 2020 2020 2020 2020   state.         
-0000f160: 2020 2054 6865 2073 7461 7465 0a0a 2020     The state..  
-0000f170: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
-0000f180: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-0000f190: 2020 2020 2020 5469 6d65 5365 7269 6573        TimeSeries
-0000f1a0: 0a20 2020 2020 2020 2020 2020 2041 206e  .            A n
-0000f1b0: 6577 2054 696d 6553 6572 6965 7320 696e  ew TimeSeries in
-0000f1c0: 7374 616e 6365 2c20 656e 6861 6e63 6564  stance, enhanced
-0000f1d0: 2077 6974 6820 6269 6e61 7279 2068 6f6c   with binary hol
-0000f1e0: 6964 6179 2063 6f6d 706f 6e65 6e74 2e0a  iday component..
-0000f1f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000f200: 2020 2020 7365 6c66 2e5f 6173 7365 7274      self._assert
-0000f210: 5f64 6574 6572 6d69 6e69 7374 6963 2829  _deterministic()
-0000f220: 0a20 2020 2020 2020 2066 726f 6d20 2e75  .        from .u
-0000f230: 7469 6c73 2069 6d70 6f72 7420 7469 6d65  tils import time
-0000f240: 7365 7269 6573 5f67 656e 6572 6174 696f  series_generatio
-0000f250: 6e20 6173 2074 670a 2020 2020 2020 2020  n as tg.        
-0000f260: 7265 7475 726e 2073 656c 662e 7374 6163  return self.stac
-0000f270: 6b28 7467 2e68 6f6c 6964 6179 735f 7469  k(tg.holidays_ti
-0000f280: 6d65 7365 7269 6573 2873 656c 662e 7469  meseries(self.ti
-0000f290: 6d65 5f69 6e64 6578 2c20 636f 756e 7472  me_index, countr
-0000f2a0: 795f 636f 6465 2c20 7072 6f76 2c20 7374  y_code, prov, st
-0000f2b0: 6174 6529 290a 0a20 2020 2064 6566 2072  ate))..    def r
-0000f2c0: 6573 616d 706c 6528 7365 6c66 2c20 6672  esample(self, fr
-0000f2d0: 6571 3a20 7374 722c 206d 6574 686f 643a  eq: str, method:
-0000f2e0: 2073 7472 203d 2027 7061 6427 2920 2d3e   str = 'pad') ->
-0000f2f0: 2027 5469 6d65 5365 7269 6573 273a 0a20   'TimeSeries':. 
-0000f300: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000f310: 2020 2043 7265 6174 6573 2061 6e20 7265     Creates an re
-0000f320: 696e 6465 7865 6420 7469 6d65 2073 6572  indexed time ser
-0000f330: 6965 7320 7769 7468 2061 2067 6976 656e  ies with a given
-0000f340: 2066 7265 7175 656e 6379 2e0a 2020 2020   frequency..    
-0000f350: 2020 2020 5072 6f76 6964 6564 206d 6574      Provided met
-0000f360: 686f 6420 6973 2075 7365 6420 746f 2066  hod is used to f
-0000f370: 696c 6c20 686f 6c65 7320 696e 2072 6569  ill holes in rei
-0000f380: 6e64 6578 6564 2054 696d 6553 6572 6965  ndexed TimeSerie
-0000f390: 732c 2062 7920 6465 6661 756c 7420 2770  s, by default 'p
-0000f3a0: 6164 272e 0a0a 2020 2020 2020 2020 5061  ad'...        Pa
-0000f3b0: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-0000f3c0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-0000f3d0: 2020 2020 6672 6571 0a20 2020 2020 2020      freq.       
-0000f3e0: 2020 2020 2054 6865 206e 6577 2074 696d       The new tim
-0000f3f0: 6520 6469 6666 6572 656e 6365 2062 6574  e difference bet
-0000f400: 7765 656e 2074 776f 2061 646a 6163 656e  ween two adjacen
-0000f410: 7420 656e 7472 6965 7320 696e 2074 6865  t entries in the
-0000f420: 2072 6574 7572 6e65 6420 5469 6d65 5365   returned TimeSe
-0000f430: 7269 6573 2e0a 2020 2020 2020 2020 2020  ries..          
-0000f440: 2020 4120 4461 7465 4f66 6673 6574 2061    A DateOffset a
-0000f450: 6c69 6173 2069 7320 6578 7065 6374 6564  lias is expected
-0000f460: 2e0a 2020 2020 2020 2020 6d65 7468 6f64  ..        method
-0000f470: 3a0a 2020 2020 2020 2020 2020 2020 4d65  :.            Me
-0000f480: 7468 6f64 2074 6f20 6669 6c6c 2068 6f6c  thod to fill hol
-0000f490: 6573 2069 6e20 7265 696e 6465 7865 6420  es in reindexed 
-0000f4a0: 5469 6d65 5365 7269 6573 2028 6e6f 7465  TimeSeries (note
-0000f4b0: 2074 6869 7320 646f 6573 206e 6f74 2066   this does not f
-0000f4c0: 696c 6c20 4e61 4e73 2074 6861 7420 616c  ill NaNs that al
-0000f4d0: 7265 6164 7920 7765 7265 2070 7265 7365  ready were prese
-0000f4e0: 6e74 293a 0a0a 2020 2020 2020 2020 2020  nt):..          
-0000f4f0: 2020 e280 9870 6164 e280 993a 2070 726f    ...pad...: pro
-0000f500: 7061 6761 7465 206c 6173 7420 7661 6c69  pagate last vali
-0000f510: 6420 6f62 7365 7276 6174 696f 6e20 666f  d observation fo
-0000f520: 7277 6172 6420 746f 206e 6578 7420 7661  rward to next va
-0000f530: 6c69 640a 0a20 2020 2020 2020 2020 2020  lid..           
-0000f540: 20e2 8098 6261 636b 6669 6c6c e280 993a   ...backfill...:
-0000f550: 2075 7365 204e 4558 5420 7661 6c69 6420   use NEXT valid 
-0000f560: 6f62 7365 7276 6174 696f 6e20 746f 2066  observation to f
-0000f570: 696c 6c2e 0a20 2020 2020 2020 2052 6574  ill..        Ret
-0000f580: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-0000f590: 2d2d 2d2d 0a20 2020 2020 2020 2054 696d  ----.        Tim
-0000f5a0: 6553 6572 6965 730a 2020 2020 2020 2020  eSeries.        
-0000f5b0: 2020 2020 4120 7265 696e 6465 7865 6420      A reindexed 
-0000f5c0: 5469 6d65 5365 7269 6573 2077 6974 6820  TimeSeries with 
-0000f5d0: 6769 7665 6e20 6672 6571 7565 6e63 792e  given frequency.
-0000f5e0: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-0000f5f0: 2020 2020 2020 7265 7361 6d70 6c65 203d        resample =
-0000f600: 2073 656c 662e 5f78 612e 7265 7361 6d70   self._xa.resamp
-0000f610: 6c65 287b 7365 6c66 2e5f 7469 6d65 5f64  le({self._time_d
-0000f620: 696d 3a20 6672 6571 7d29 0a0a 2020 2020  im: freq})..    
-0000f630: 2020 2020 2320 544f 444f 3a20 6368 6563      # TODO: chec
-0000f640: 6b0a 2020 2020 2020 2020 6966 206d 6574  k.        if met
-0000f650: 686f 6420 3d3d 2027 7061 6427 3a0a 2020  hod == 'pad':.  
-0000f660: 2020 2020 2020 2020 2020 6e65 775f 7861            new_xa
-0000f670: 203d 2072 6573 616d 706c 652e 7061 6428   = resample.pad(
-0000f680: 290a 2020 2020 2020 2020 656c 6966 206d  ).        elif m
-0000f690: 6574 686f 6420 3d3d 2027 6266 696c 6c27  ethod == 'bfill'
-0000f6a0: 3a0a 2020 2020 2020 2020 2020 2020 6e65  :.            ne
-0000f6b0: 775f 7861 203d 2072 6573 616d 706c 652e  w_xa = resample.
-0000f6c0: 6261 636b 6669 6c6c 2829 0a20 2020 2020  backfill().     
-0000f6d0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000f6e0: 2020 2020 2072 6169 7365 5f6c 6f67 2856       raise_log(V
-0000f6f0: 616c 7565 4572 726f 7228 2755 6e6b 6e6f  alueError('Unkno
-0000f700: 776e 206d 6574 686f 643a 207b 7d27 2e66  wn method: {}'.f
-0000f710: 6f72 6d61 7428 6d65 7468 6f64 2929 2c20  ormat(method)), 
-0000f720: 6c6f 6767 6572 290a 2020 2020 2020 2020  logger).        
-0000f730: 7265 7475 726e 2054 696d 6553 6572 6965  return TimeSerie
-0000f740: 7328 6e65 775f 7861 290a 0a20 2020 2064  s(new_xa)..    d
-0000f750: 6566 2069 735f 7769 7468 696e 5f72 616e  ef is_within_ran
-0000f760: 6765 2873 656c 662c 2074 733a 2055 6e69  ge(self, ts: Uni
-0000f770: 6f6e 5b70 642e 5469 6d65 7374 616d 702c  on[pd.Timestamp,
-0000f780: 2069 6e74 5d29 202d 3e20 626f 6f6c 3a0a   int]) -> bool:.
-0000f790: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000f7a0: 2020 2020 4368 6563 6b20 7768 6574 6865      Check whethe
-0000f7b0: 7220 6120 6769 7665 6e20 7469 6d65 7374  r a given timest
-0000f7c0: 616d 7020 6f72 2069 6e74 6567 6572 2069  amp or integer i
-0000f7d0: 7320 7769 7468 696e 6720 7468 6520 7469  s withing the ti
-0000f7e0: 6d65 2069 6e74 6572 7661 6c20 6f66 2074  me interval of t
-0000f7f0: 6869 7320 7469 6d65 2073 6572 6965 732e  his time series.
-0000f800: 0a20 2020 2020 2020 2049 6620 6120 7469  .        If a ti
-0000f810: 6d65 7374 616d 7020 6973 2070 726f 7669  mestamp is provi
-0000f820: 6465 642c 2069 7420 646f 6573 206e 6f74  ded, it does not
-0000f830: 206e 6565 6420 746f 2062 6520 616e 2065   need to be an e
-0000f840: 6c65 6d65 6e74 206f 6620 7468 6520 7469  lement of the ti
-0000f850: 6d65 2069 6e64 6578 206f 6620 7468 6520  me index of the 
-0000f860: 7365 7269 6573 2e0a 0a20 2020 2020 2020  series...       
-0000f870: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-0000f880: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-0000f890: 2020 2020 2020 2074 730a 2020 2020 2020         ts.      
-0000f8a0: 2020 2020 2020 5468 6520 6070 616e 6461        The `panda
-0000f8b0: 732e 5469 6d65 7374 616d 7060 2028 6966  s.Timestamp` (if
-0000f8c0: 2069 6e64 6578 6564 2077 6974 6820 4461   indexed with Da
-0000f8d0: 7465 7469 6d65 496e 6465 7829 206f 7220  tetimeIndex) or 
-0000f8e0: 696e 7465 6765 7220 2869 6620 696e 6465  integer (if inde
-0000f8f0: 7865 6420 7769 7468 2052 616e 6765 496e  xed with RangeIn
-0000f900: 6465 7829 2074 6f20 6368 6563 6b2e 0a0a  dex) to check...
-0000f910: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-0000f920: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-0000f930: 2020 2020 2020 2020 626f 6f6c 0a20 2020          bool.   
-0000f940: 2020 2020 2020 2020 2057 6865 7468 6572           Whether
-0000f950: 2060 7473 6020 6973 2063 6f6e 7461 696e   `ts` is contain
-0000f960: 6564 2077 6974 6869 6e20 7468 6520 696e  ed within the in
-0000f970: 7465 7276 616c 206f 6620 7468 6973 2074  terval of this t
-0000f980: 696d 6520 7365 7269 6573 2e0a 2020 2020  ime series..    
-0000f990: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000f9a0: 7265 7475 726e 2073 656c 662e 7469 6d65  return self.time
-0000f9b0: 5f69 6e64 6578 5b30 5d20 3c3d 2074 7320  _index[0] <= ts 
-0000f9c0: 3c3d 2073 656c 662e 7469 6d65 5f69 6e64  <= self.time_ind
-0000f9d0: 6578 5b2d 315d 0a0a 2020 2020 6465 6620  ex[-1]..    def 
-0000f9e0: 6d61 7028 7365 6c66 2c0a 2020 2020 2020  map(self,.      
-0000f9f0: 2020 2020 2020 666e 3a20 556e 696f 6e5b        fn: Union[
-0000fa00: 4361 6c6c 6162 6c65 5b5b 6e70 2e6e 756d  Callable[[np.num
-0000fa10: 6265 725d 2c20 6e70 2e6e 756d 6265 725d  ber], np.number]
-0000fa20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000fa30: 2020 2020 2020 2020 4361 6c6c 6162 6c65          Callable
-0000fa40: 5b5b 556e 696f 6e5b 7064 2e54 696d 6573  [[Union[pd.Times
-0000fa50: 7461 6d70 2c20 696e 745d 2c20 6e70 2e6e  tamp, int], np.n
-0000fa60: 756d 6265 725d 2c20 6e70 2e6e 756d 6265  umber], np.numbe
-0000fa70: 725d 5d29 202d 3e20 2754 696d 6553 6572  r]]) -> 'TimeSer
-0000fa80: 6965 7327 3a20 2023 206e 6f71 613a 2045  ies':  # noqa: E
-0000fa90: 3530 310a 2020 2020 2020 2020 2222 220a  501.        """.
-0000faa0: 2020 2020 2020 2020 4170 706c 6965 7320          Applies 
-0000fab0: 7468 6520 6675 6e63 7469 6f6e 2060 666e  the function `fn
-0000fac0: 6020 656c 656d 656e 7477 6973 6520 746f  ` elementwise to
-0000fad0: 2061 6c6c 2076 616c 7565 7320 696e 2074   all values in t
-0000fae0: 6869 7320 5469 6d65 5365 7269 6573 2e0a  his TimeSeries..
-0000faf0: 2020 2020 2020 2020 5265 7475 726e 7320          Returns 
-0000fb00: 6120 6e65 7720 5469 6d65 5365 7269 6573  a new TimeSeries
-0000fb10: 2069 6e73 7461 6e63 652e 2049 6620 6066   instance. If `f
-0000fb20: 6e60 2074 616b 6573 2031 2061 7267 756d  n` takes 1 argum
-0000fb30: 656e 7420 6974 2069 7320 7369 6d70 6c79  ent it is simply
-0000fb40: 2061 7070 6c69 6564 2065 6c65 6d65 6e74   applied element
-0000fb50: 7769 7365 2e0a 2020 2020 2020 2020 4966  wise..        If
-0000fb60: 2069 7420 7461 6b65 7320 3220 6172 6775   it takes 2 argu
-0000fb70: 6d65 6e74 732c 2069 7420 6973 2061 7070  ments, it is app
-0000fb80: 6c69 6564 2065 6c65 6d65 6e74 7769 7365  lied elementwise
-0000fb90: 206f 6e20 7468 6520 2874 696d 6573 7461   on the (timesta
-0000fba0: 6d70 2c20 7661 6c75 6529 2074 7570 6c65  mp, value) tuple
-0000fbb0: 732e 0a0a 2020 2020 2020 2020 4174 2074  s...        At t
-0000fbc0: 6865 206d 6f6d 656e 7420 7468 6973 2066  he moment this f
-0000fbd0: 756e 6374 696f 6e20 776f 726b 7320 6f6e  unction works on
-0000fbe0: 6c79 206f 6e20 6465 7465 726d 696e 6973  ly on determinis
-0000fbf0: 7469 6320 7469 6d65 2073 6572 6965 7320  tic time series 
-0000fc00: 2869 2e65 2e2c 206d 6164 6520 6f66 2031  (i.e., made of 1
-0000fc10: 2073 616d 706c 6529 2e0a 0a20 2020 2020   sample)...     
-0000fc20: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-0000fc30: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-0000fc40: 0a20 2020 2020 2020 2066 6e0a 2020 2020  .        fn.    
-0000fc50: 2020 2020 2020 2020 4569 7468 6572 2061          Either a
-0000fc60: 2066 756e 6374 696f 6e20 7768 6963 6820   function which 
-0000fc70: 7461 6b65 7320 6120 7661 6c75 6520 616e  takes a value an
-0000fc80: 6420 7265 7475 726e 7320 6120 7661 6c75  d returns a valu
-0000fc90: 6520 6965 2e20 6066 2878 2920 3d20 7960  e ie. `f(x) = y`
-0000fca0: 0a20 2020 2020 2020 2020 2020 204f 7220  .            Or 
-0000fcb0: 6120 6675 6e63 7469 6f6e 2077 6869 6368  a function which
-0000fcc0: 2074 616b 6573 2061 2076 616c 7565 2061   takes a value a
-0000fcd0: 6e64 2069 7473 2074 696d 6573 7461 6d70  nd its timestamp
-0000fce0: 2061 6e64 2072 6574 7572 6e73 2061 2076   and returns a v
-0000fcf0: 616c 7565 2069 652e 2060 6628 7469 6d65  alue ie. `f(time
-0000fd00: 7374 616d 702c 2078 2920 3d20 7960 0a20  stamp, x) = y`. 
-0000fd10: 2020 2020 2020 2020 2020 2054 6865 2074             The t
-0000fd20: 7970 6520 6f66 2060 7469 6d65 7374 616d  ype of `timestam
-0000fd30: 7060 2069 7320 6569 7468 6572 2060 7064  p` is either `pd
-0000fd40: 2e54 696d 6573 7461 6d70 6020 2869 6620  .Timestamp` (if 
-0000fd50: 7468 6520 7365 7269 6573 2069 7320 696e  the series is in
-0000fd60: 6465 7865 6420 7769 7468 2061 2044 6174  dexed with a Dat
-0000fd70: 6574 696d 6549 6e64 6578 292c 0a20 2020  etimeIndex),.   
-0000fd80: 2020 2020 2020 2020 206f 7220 616e 2069           or an i
-0000fd90: 6e74 6567 6572 206f 7468 6572 7769 7365  nteger otherwise
-0000fda0: 2028 6966 2074 6865 2073 6572 6965 7320   (if the series 
-0000fdb0: 6973 2069 6e64 6578 6564 2077 6974 6820  is indexed with 
-0000fdc0: 6120 5261 6e67 6549 6e64 6578 292e 0a0a  a RangeIndex)...
-0000fdd0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-0000fde0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-0000fdf0: 2020 2020 2020 2020 5469 6d65 5365 7269          TimeSeri
-0000fe00: 6573 0a20 2020 2020 2020 2020 2020 2041  es.            A
-0000fe10: 206e 6577 2054 696d 6553 6572 6965 7320   new TimeSeries 
-0000fe20: 696e 7374 616e 6365 0a20 2020 2020 2020  instance.       
-0000fe30: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
-0000fe40: 6e6f 7420 6973 696e 7374 616e 6365 2866  not isinstance(f
-0000fe50: 6e2c 2043 616c 6c61 626c 6529 3a0a 2020  n, Callable):.  
-0000fe60: 2020 2020 2020 2020 2020 7261 6973 655f            raise_
-0000fe70: 6c6f 6728 5479 7065 4572 726f 7228 2266  log(TypeError("f
-0000fe80: 6e20 7368 6f75 6c64 2062 6520 6361 6c6c  n should be call
-0000fe90: 6162 6c65 2229 2c20 6c6f 6767 6572 290a  able"), logger).
-0000fea0: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-0000feb0: 7374 616e 6365 2866 6e2c 206e 702e 7566  stance(fn, np.uf
-0000fec0: 756e 6329 3a0a 2020 2020 2020 2020 2020  unc):.          
-0000fed0: 2020 6966 2066 6e2e 6e69 6e20 3d3d 2031    if fn.nin == 1
-0000fee0: 2061 6e64 2066 6e2e 6e6f 7574 203d 3d20   and fn.nout == 
-0000fef0: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
-0000ff00: 2020 206e 756d 5f61 7267 7320 3d20 310a     num_args = 1.
-0000ff10: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-0000ff20: 2066 6e2e 6e69 6e20 3d3d 2032 2061 6e64   fn.nin == 2 and
-0000ff30: 2066 6e2e 6e6f 7574 203d 3d20 313a 0a20   fn.nout == 1:. 
-0000ff40: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000ff50: 756d 5f61 7267 7320 3d20 320a 2020 2020  um_args = 2.    
-0000ff60: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000ff70: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-0000ff80: 6973 655f 6c6f 6728 5661 6c75 6545 7272  ise_log(ValueErr
-0000ff90: 6f72 2822 666e 206d 7573 7420 6861 7665  or("fn must have
-0000ffa0: 2065 6974 6865 7220 6f6e 6520 6f72 2074   either one or t
-0000ffb0: 776f 2061 7267 756d 656e 7473 2061 6e64  wo arguments and
-0000ffc0: 2072 6574 7572 6e20 6120 7369 6e67 6c65   return a single
-0000ffd0: 2076 616c 7565 2229 2c20 6c6f 6767 6572   value"), logger
-0000ffe0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-0000fff0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00010000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010010: 206e 756d 5f61 7267 7320 3d20 6c65 6e28   num_args = len(
-00010020: 7369 676e 6174 7572 6528 666e 292e 7061  signature(fn).pa
-00010030: 7261 6d65 7465 7273 290a 2020 2020 2020  rameters).      
-00010040: 2020 2020 2020 6578 6365 7074 2056 616c        except Val
-00010050: 7565 4572 726f 723a 0a20 2020 2020 2020  ueError:.       
-00010060: 2020 2020 2020 2020 2072 6169 7365 5f6c           raise_l
-00010070: 6f67 2856 616c 7565 4572 726f 7228 2269  og(ValueError("i
-00010080: 6e73 7065 6374 2e73 6967 6e61 7475 7265  nspect.signature
-00010090: 2866 6e29 2066 6169 6c65 642e 2054 7279  (fn) failed. Try
-000100a0: 2077 7261 7070 696e 6720 666e 2069 6e20   wrapping fn in 
-000100b0: 6120 6c61 6d62 6461 2c20 652e 672e 206c  a lambda, e.g. l
-000100c0: 616d 6264 6120 783a 2066 6e28 7829 2229  ambda x: fn(x)")
-000100d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000100e0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-000100f0: 6572 290a 0a20 2020 2020 2020 2069 6620  er)..        if 
-00010100: 6e75 6d5f 6172 6773 203d 3d20 313a 2020  num_args == 1:  
-00010110: 2320 7369 6d70 6c65 206d 6170 2066 756e  # simple map fun
-00010120: 6374 696f 6e20 6628 7829 0a20 2020 2020  ction f(x).     
-00010130: 2020 2020 2020 2064 6620 3d20 7365 6c66         df = self
-00010140: 2e70 645f 6461 7461 6672 616d 6528 292e  .pd_dataframe().
-00010150: 6170 706c 796d 6170 2866 6e29 0a20 2020  applymap(fn).   
-00010160: 2020 2020 2065 6c69 6620 6e75 6d5f 6172       elif num_ar
-00010170: 6773 203d 3d20 323a 2020 2320 6d61 7020  gs == 2:  # map 
-00010180: 6675 6e63 7469 6f6e 2075 7365 7320 7469  function uses ti
-00010190: 6d65 7374 616d 7020 6628 7469 6d65 7374  mestamp f(timest
-000101a0: 616d 702c 2078 290a 2020 2020 2020 2020  amp, x).        
-000101b0: 2020 2020 6465 6620 6170 706c 795f 666e      def apply_fn
-000101c0: 5f77 7261 7070 6572 2872 6f77 293a 0a20  _wrapper(row):. 
-000101d0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000101e0: 696d 6573 7461 6d70 203d 2072 6f77 2e6e  imestamp = row.n
-000101f0: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
-00010200: 2020 2020 7265 7475 726e 2072 6f77 2e6d      return row.m
-00010210: 6170 286c 616d 6264 6120 783a 2066 6e28  ap(lambda x: fn(
-00010220: 7469 6d65 7374 616d 702c 2078 2929 0a20  timestamp, x)). 
-00010230: 2020 2020 2020 2020 2020 2064 6620 3d20             df = 
-00010240: 7365 6c66 2e70 645f 6461 7461 6672 616d  self.pd_datafram
-00010250: 6528 292e 6170 706c 7928 6170 706c 795f  e().apply(apply_
-00010260: 666e 5f77 7261 7070 6572 2c20 6178 6973  fn_wrapper, axis
-00010270: 3d31 290a 2020 2020 2020 2020 656c 7365  =1).        else
-00010280: 3a0a 2020 2020 2020 2020 2020 2020 6466  :.            df
-00010290: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-000102a0: 2020 2020 7261 6973 655f 6c6f 6728 5661      raise_log(Va
-000102b0: 6c75 6545 7272 6f72 2822 666e 206d 7573  lueError("fn mus
-000102c0: 7420 6861 7665 2065 6974 6865 7220 6f6e  t have either on
-000102d0: 6520 6f72 2074 776f 2061 7267 756d 656e  e or two argumen
-000102e0: 7473 2229 2c20 6c6f 6767 6572 290a 0a20  ts"), logger).. 
-000102f0: 2020 2020 2020 2072 6574 7572 6e20 5469         return Ti
-00010300: 6d65 5365 7269 6573 2e66 726f 6d5f 6461  meSeries.from_da
-00010310: 7461 6672 616d 6528 6466 290a 0a20 2020  taframe(df)..   
-00010320: 2064 6566 2074 6f5f 6a73 6f6e 2873 656c   def to_json(sel
-00010330: 6629 202d 3e20 7374 723a 0a20 2020 2020  f) -> str:.     
-00010340: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
-00010350: 6f6e 7665 7274 7320 7468 6520 6054 696d  onverts the `Tim
-00010360: 6553 6572 6965 7360 206f 626a 6563 7420  eSeries` object 
-00010370: 746f 2061 204a 534f 4e20 5374 7269 6e67  to a JSON String
-00010380: 0a0a 2020 2020 2020 2020 4174 2074 6865  ..        At the
-00010390: 206d 6f6d 656e 7420 7468 6973 2066 756e   moment this fun
-000103a0: 6374 696f 6e20 776f 726b 7320 6f6e 6c79  ction works only
-000103b0: 206f 6e20 6465 7465 726d 696e 6973 7469   on deterministi
-000103c0: 6320 7469 6d65 2073 6572 6965 7320 2869  c time series (i
-000103d0: 2e65 2e2c 206d 6164 6520 6f66 2031 2073  .e., made of 1 s
-000103e0: 616d 706c 6529 2e0a 0a20 2020 2020 2020  ample)...       
-000103f0: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-00010400: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-00010410: 2073 7472 0a20 2020 2020 2020 2020 2020   str.           
-00010420: 2041 204a 534f 4e20 5374 7269 6e67 2072   A JSON String r
-00010430: 6570 7265 7365 6e74 696e 6720 7468 6520  epresenting the 
-00010440: 7469 6d65 2073 6572 6965 730a 2020 2020  time series.    
-00010450: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00010460: 7265 7475 726e 2073 656c 662e 7064 5f64  return self.pd_d
-00010470: 6174 6166 7261 6d65 2829 2e74 6f5f 6a73  ataframe().to_js
-00010480: 6f6e 286f 7269 656e 743d 2773 706c 6974  on(orient='split
-00010490: 272c 2064 6174 655f 666f 726d 6174 3d27  ', date_format='
-000104a0: 6973 6f27 290a 0a20 2020 2064 6566 2070  iso')..    def p
-000104b0: 6c6f 7428 7365 6c66 2c0a 2020 2020 2020  lot(self,.      
-000104c0: 2020 2020 2020 206e 6577 5f70 6c6f 743a         new_plot:
-000104d0: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
-000104e0: 2020 2020 2020 2020 2020 2020 6365 6e74              cent
-000104f0: 7261 6c5f 7175 616e 7469 6c65 3a20 556e  ral_quantile: Un
-00010500: 696f 6e5b 666c 6f61 742c 2073 7472 5d20  ion[float, str] 
-00010510: 3d20 302e 352c 0a20 2020 2020 2020 2020  = 0.5,.         
-00010520: 2020 2020 6c6f 775f 7175 616e 7469 6c65      low_quantile
-00010530: 3a20 4f70 7469 6f6e 616c 5b66 6c6f 6174  : Optional[float
-00010540: 5d20 3d20 302e 3035 2c0a 2020 2020 2020  ] = 0.05,.      
-00010550: 2020 2020 2020 2068 6967 685f 7175 616e         high_quan
-00010560: 7469 6c65 3a20 4f70 7469 6f6e 616c 5b66  tile: Optional[f
-00010570: 6c6f 6174 5d20 3d20 302e 3935 2c0a 2020  loat] = 0.95,.  
-00010580: 2020 2020 2020 2020 2020 202a 6172 6773             *args
-00010590: 2c0a 2020 2020 2020 2020 2020 2020 202a  ,.             *
-000105a0: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
-000105b0: 2020 2222 220a 2020 2020 2020 2020 4120    """.        A 
-000105c0: 7772 6170 7065 7220 6d65 7468 6f64 2061  wrapper method a
-000105d0: 726f 756e 6420 6078 6172 7261 792e 4461  round `xarray.Da
-000105e0: 7461 4172 7261 792e 706c 6f74 2829 602e  taArray.plot()`.
-000105f0: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00010600: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-00010610: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00010620: 6e65 775f 706c 6f74 0a20 2020 2020 2020  new_plot.       
-00010630: 2020 2020 2077 6865 7468 6572 2074 6f20       whether to 
-00010640: 7370 6177 6e20 6120 6e65 7720 4669 6775  spawn a new Figu
-00010650: 7265 0a20 2020 2020 2020 2063 656e 7472  re.        centr
-00010660: 616c 5f71 7561 6e74 696c 650a 2020 2020  al_quantile.    
-00010670: 2020 2020 2020 2020 5468 6520 7175 616e          The quan
-00010680: 7469 6c65 2028 6265 7477 6565 6e20 3020  tile (between 0 
-00010690: 616e 6420 3129 2074 6f20 706c 6f74 2061  and 1) to plot a
-000106a0: 7320 6120 2263 656e 7472 616c 2220 7661  s a "central" va
-000106b0: 6c75 652c 2069 6620 7468 6520 7365 7269  lue, if the seri
-000106c0: 6573 2069 7320 7374 6f63 6861 7374 6963  es is stochastic
-000106d0: 2028 692e 652e 2c20 6966 0a20 2020 2020   (i.e., if.     
-000106e0: 2020 2020 2020 2069 7420 6861 7320 6d75         it has mu
-000106f0: 6c74 6970 6c65 2073 616d 706c 6573 292e  ltiple samples).
-00010700: 2054 6869 7320 7769 6c6c 2062 6520 6170   This will be ap
-00010710: 706c 6965 6420 6f6e 2065 6163 6820 636f  plied on each co
-00010720: 6d70 6f6e 656e 7420 7365 7061 7261 7465  mponent separate
-00010730: 6c79 2028 692e 652e 2c20 746f 2064 6973  ly (i.e., to dis
-00010740: 706c 6179 2071 7561 6e74 696c 6573 0a20  play quantiles. 
-00010750: 2020 2020 2020 2020 2020 206f 6620 7468             of th
-00010760: 6520 636f 6d70 6f6e 656e 7473 2720 6d61  e components' ma
-00010770: 7267 696e 616c 2064 6973 7472 6962 7574  rginal distribut
-00010780: 696f 6e73 292e 2046 6f72 2069 6e73 7461  ions). For insta
-00010790: 6e63 652c 2073 6574 7469 6e67 2060 6365  nce, setting `ce
-000107a0: 6e74 7261 6c5f 7175 616e 7469 6c65 3d30  ntral_quantile=0
-000107b0: 2e35 6020 7769 6c6c 2070 6c6f 7420 7468  .5` will plot th
-000107c0: 650a 2020 2020 2020 2020 2020 2020 6d65  e.            me
-000107d0: 6469 616e 206f 6620 6561 6368 2063 6f6d  dian of each com
-000107e0: 706f 6e65 6e74 2e20 6063 656e 7472 616c  ponent. `central
-000107f0: 5f71 7561 6e74 696c 6560 2063 616e 2061  _quantile` can a
-00010800: 6c73 6f20 6265 2073 6574 2074 6f20 276d  lso be set to 'm
-00010810: 6561 6e27 2e0a 2020 2020 2020 2020 6c6f  ean'..        lo
-00010820: 775f 7175 616e 7469 6c65 0a20 2020 2020  w_quantile.     
-00010830: 2020 2020 2020 2054 6865 2071 7561 6e74         The quant
-00010840: 696c 6520 746f 2075 7365 2066 6f72 2074  ile to use for t
-00010850: 6865 206c 6f77 6572 2062 6f75 6e64 206f  he lower bound o
-00010860: 6620 7468 6520 706c 6f74 7465 6420 636f  f the plotted co
-00010870: 6e66 6964 656e 6365 2069 6e74 6572 7661  nfidence interva
-00010880: 6c2e 2053 696d 696c 6172 2074 6f20 6063  l. Similar to `c
-00010890: 656e 7472 616c 5f71 7561 6e74 696c 6560  entral_quantile`
-000108a0: 2c0a 2020 2020 2020 2020 2020 2020 7468  ,.            th
-000108b0: 6973 2069 7320 6170 706c 6965 6420 746f  is is applied to
-000108c0: 2065 6163 6820 636f 6d70 6f6e 656e 7420   each component 
-000108d0: 7365 7061 7261 7465 6c79 2028 692e 652e  separately (i.e.
-000108e0: 2c20 6469 7370 6c61 7969 6e67 206d 6172  , displaying mar
-000108f0: 6769 6e61 6c20 6469 7374 7269 6275 7469  ginal distributi
-00010900: 6f6e 7329 2e20 4e6f 2063 6f6e 6669 6465  ons). No confide
-00010910: 6e63 650a 2020 2020 2020 2020 2020 2020  nce.            
-00010920: 696e 7465 7276 616c 2069 7320 7368 6f77  interval is show
-00010930: 6e20 6966 2060 636f 6e66 6964 656e 6365  n if `confidence
-00010940: 5f6c 6f77 5f71 7561 6e74 696c 6560 2069  _low_quantile` i
-00010950: 7320 4e6f 6e65 2028 6465 6661 756c 7420  s None (default 
-00010960: 302e 3035 292e 0a20 2020 2020 2020 2068  0.05)..        h
-00010970: 6967 685f 7175 616e 7469 6c65 0a20 2020  igh_quantile.   
-00010980: 2020 2020 2020 2020 2054 6865 2071 7561           The qua
-00010990: 6e74 696c 6520 746f 2075 7365 2066 6f72  ntile to use for
-000109a0: 2074 6865 2075 7070 6572 2062 6f75 6e64   the upper bound
-000109b0: 206f 6620 7468 6520 706c 6f74 7465 6420   of the plotted 
-000109c0: 636f 6e66 6964 656e 6365 2069 6e74 6572  confidence inter
-000109d0: 7661 6c2e 2053 696d 696c 6172 2074 6f20  val. Similar to 
-000109e0: 6063 656e 7472 616c 5f71 7561 6e74 696c  `central_quantil
-000109f0: 6560 2c0a 2020 2020 2020 2020 2020 2020  e`,.            
-00010a00: 7468 6973 2069 7320 6170 706c 6965 6420  this is applied 
-00010a10: 746f 2065 6163 6820 636f 6d70 6f6e 656e  to each componen
-00010a20: 7420 7365 7061 7261 7465 6c79 2028 692e  t separately (i.
-00010a30: 652e 2c20 6469 7370 6c61 7969 6e67 206d  e., displaying m
-00010a40: 6172 6769 6e61 6c20 6469 7374 7269 6275  arginal distribu
-00010a50: 7469 6f6e 7329 2e20 4e6f 2063 6f6e 6669  tions). No confi
-00010a60: 6465 6e63 650a 2020 2020 2020 2020 2020  dence.          
-00010a70: 2020 696e 7465 7276 616c 2069 7320 7368    interval is sh
-00010a80: 6f77 6e20 6966 2060 6869 6768 5f71 7561  own if `high_qua
-00010a90: 6e74 696c 6560 2069 7320 4e6f 6e65 2028  ntile` is None (
-00010aa0: 6465 6661 756c 7420 302e 3935 292e 0a20  default 0.95).. 
-00010ab0: 2020 2020 2020 2061 7267 730a 2020 2020         args.    
-00010ac0: 2020 2020 2020 2020 736f 6d65 2070 6f73          some pos
-00010ad0: 6974 696f 6e61 6c20 6172 6775 6d65 6e74  itional argument
-00010ae0: 7320 666f 7220 7468 6520 6070 6c6f 7428  s for the `plot(
-00010af0: 2960 206d 6574 686f 640a 2020 2020 2020  )` method.      
-00010b00: 2020 6b77 6172 6773 0a20 2020 2020 2020    kwargs.       
-00010b10: 2020 2020 2073 6f6d 6520 6b65 7977 6f72       some keywor
-00010b20: 6420 6172 6775 6d65 6e74 7320 666f 7220  d arguments for 
-00010b30: 7468 6520 6070 6c6f 7428 2960 206d 6574  the `plot()` met
-00010b40: 686f 640a 2020 2020 2020 2020 2222 220a  hod.        """.
-00010b50: 2020 2020 2020 2020 616c 7068 615f 636f          alpha_co
-00010b60: 6e66 6964 656e 6365 5f69 6e74 766c 7320  nfidence_intvls 
-00010b70: 3d20 302e 3235 0a0a 2020 2020 2020 2020  = 0.25..        
-00010b80: 6966 2063 656e 7472 616c 5f71 7561 6e74  if central_quant
-00010b90: 696c 6520 213d 2027 6d65 616e 273a 0a20  ile != 'mean':. 
-00010ba0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00010bb0: 5f69 665f 6e6f 7428 6973 696e 7374 616e  _if_not(isinstan
-00010bc0: 6365 2863 656e 7472 616c 5f71 7561 6e74  ce(central_quant
-00010bd0: 696c 652c 2066 6c6f 6174 2920 616e 6420  ile, float) and 
-00010be0: 302e 203c 3d20 6365 6e74 7261 6c5f 7175  0. <= central_qu
-00010bf0: 616e 7469 6c65 203c 3d20 312e 2c0a 2020  antile <= 1.,.  
-00010c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c10: 2020 2020 2020 2027 6365 6e74 7261 6c5f         'central_
-00010c20: 7175 616e 7469 6c65 206d 7573 7420 6265  quantile must be
-00010c30: 2065 6974 6865 7220 226d 6561 6e22 2c20   either "mean", 
-00010c40: 6f72 2061 2066 6c6f 6174 2062 6574 7765  or a float betwe
-00010c50: 656e 2030 2061 6e64 2031 2e27 2c0a 2020  en 0 and 1.',.  
-00010c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c70: 2020 2020 2020 206c 6f67 6765 7229 0a0a         logger)..
-00010c80: 2020 2020 2020 2020 6966 2068 6967 685f          if high_
-00010c90: 7175 616e 7469 6c65 2069 7320 6e6f 7420  quantile is not 
-00010ca0: 4e6f 6e65 2061 6e64 206c 6f77 5f71 7561  None and low_qua
-00010cb0: 6e74 696c 6520 6973 206e 6f74 204e 6f6e  ntile is not Non
-00010cc0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00010cd0: 6169 7365 5f69 665f 6e6f 7428 302e 203c  aise_if_not(0. <
-00010ce0: 3d20 6c6f 775f 7175 616e 7469 6c65 203c  = low_quantile <
-00010cf0: 3d20 312e 2061 6e64 2030 2e20 3c3d 2068  = 1. and 0. <= h
-00010d00: 6967 685f 7175 616e 7469 6c65 203c 3d20  igh_quantile <= 
-00010d10: 312e 2c0a 2020 2020 2020 2020 2020 2020  1.,.            
-00010d20: 2020 2020 2020 2020 2020 2020 2027 636f               'co
-00010d30: 6e66 6964 656e 6365 2069 6e74 6572 7661  nfidence interva
-00010d40: 6c20 6c6f 7720 616e 6420 6869 6768 2071  l low and high q
-00010d50: 7561 6e74 696c 6573 206d 7573 7420 6265  uantiles must be
-00010d60: 2062 6574 7765 656e 2030 2061 6e64 2031   between 0 and 1
-00010d70: 2e27 2c0a 2020 2020 2020 2020 2020 2020  .',.            
-00010d80: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-00010d90: 6765 7229 0a0a 2020 2020 2020 2020 6669  ger)..        fi
-00010da0: 6720 3d20 2870 6c74 2e66 6967 7572 6528  g = (plt.figure(
-00010db0: 2920 6966 206e 6577 5f70 6c6f 7420 656c  ) if new_plot el
-00010dc0: 7365 2028 6b77 6172 6773 5b27 6669 6775  se (kwargs['figu
-00010dd0: 7265 275d 2069 6620 2766 6967 7572 6527  re'] if 'figure'
-00010de0: 2069 6e20 6b77 6172 6773 2065 6c73 6520   in kwargs else 
-00010df0: 706c 742e 6763 6628 2929 290a 2020 2020  plt.gcf())).    
-00010e00: 2020 2020 6b77 6172 6773 5b27 6669 6775      kwargs['figu
-00010e10: 7265 275d 203d 2066 6967 0a20 2020 2020  re'] = fig.     
-00010e20: 2020 206c 6162 656c 203d 206b 7761 7267     label = kwarg
-00010e30: 735b 276c 6162 656c 275d 2069 6620 276c  s['label'] if 'l
-00010e40: 6162 656c 2720 696e 206b 7761 7267 7320  abel' in kwargs 
-00010e50: 656c 7365 2027 270a 0a20 2020 2020 2020  else ''..       
-00010e60: 2069 6620 276c 7727 206e 6f74 2069 6e20   if 'lw' not in 
-00010e70: 6b77 6172 6773 3a0a 2020 2020 2020 2020  kwargs:.        
-00010e80: 2020 2020 6b77 6172 6773 5b27 6c77 275d      kwargs['lw']
-00010e90: 203d 2032 0a0a 2020 2020 2020 2020 6966   = 2..        if
-00010ea0: 2073 656c 662e 6e5f 636f 6d70 6f6e 656e   self.n_componen
-00010eb0: 7473 203e 2031 303a 0a20 2020 2020 2020  ts > 10:.       
-00010ec0: 2020 2020 206c 6f67 6765 722e 7761 726e       logger.warn
-00010ed0: 2827 4e75 6d62 6572 206f 6620 636f 6d70  ('Number of comp
-00010ee0: 6f6e 656e 7473 2069 7320 6c61 7267 6572  onents is larger
-00010ef0: 2074 6861 6e20 3130 2028 7b7d 292e 2050   than 10 ({}). P
-00010f00: 6c6f 7474 696e 6720 6f6e 6c79 2074 6865  lotting only the
-00010f10: 2066 6972 7374 2031 3020 636f 6d70 6f6e   first 10 compon
-00010f20: 656e 7473 2e27 2e66 6f72 6d61 7428 0a20  ents.'.format(. 
-00010f30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00010f40: 656c 662e 6e5f 636f 6d70 6f6e 656e 7473  elf.n_components
-00010f50: 0a20 2020 2020 2020 2020 2020 2029 290a  .            )).
-00010f60: 0a20 2020 2020 2020 2066 6f72 2069 2c20  .        for i, 
-00010f70: 6320 696e 2065 6e75 6d65 7261 7465 2873  c in enumerate(s
-00010f80: 656c 662e 5f78 612e 636f 6d70 6f6e 656e  elf._xa.componen
-00010f90: 745b 3a31 305d 293a 0a20 2020 2020 2020  t[:10]):.       
-00010fa0: 2020 2020 2063 6f6d 705f 6e61 6d65 203d       comp_name =
-00010fb0: 2073 7472 2863 2e76 616c 7565 7329 0a0a   str(c.values)..
-00010fc0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00010fd0: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
-00010fe0: 2020 2020 2020 6b77 6172 6773 5b27 6669        kwargs['fi
-00010ff0: 6775 7265 275d 203d 2070 6c74 2e67 6366  gure'] = plt.gcf
-00011000: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
-00011010: 636f 6d70 203d 2073 656c 662e 5f78 612e  comp = self._xa.
-00011020: 7365 6c28 636f 6d70 6f6e 656e 743d 6329  sel(component=c)
-00011030: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00011040: 2063 6f6d 702e 7361 6d70 6c65 2e73 697a   comp.sample.siz
-00011050: 6520 3e20 313a 0a20 2020 2020 2020 2020  e > 1:.         
-00011060: 2020 2020 2020 2069 6620 6365 6e74 7261         if centra
-00011070: 6c5f 7175 616e 7469 6c65 203d 3d20 276d  l_quantile == 'm
-00011080: 6561 6e27 3a0a 2020 2020 2020 2020 2020  ean':.          
-00011090: 2020 2020 2020 2020 2020 6365 6e74 7261            centra
-000110a0: 6c5f 7365 7269 6573 203d 2063 6f6d 702e  l_series = comp.
-000110b0: 6d65 616e 2864 696d 3d44 494d 535b 325d  mean(dim=DIMS[2]
-000110c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000110d0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000110e0: 2020 2020 2020 2020 2020 2020 6365 6e74              cent
-000110f0: 7261 6c5f 7365 7269 6573 203d 2063 6f6d  ral_series = com
-00011100: 702e 7175 616e 7469 6c65 2871 3d63 656e  p.quantile(q=cen
-00011110: 7472 616c 5f71 7561 6e74 696c 652c 2064  tral_quantile, d
-00011120: 696d 3d44 494d 535b 325d 290a 2020 2020  im=DIMS[2]).    
-00011130: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00011140: 2020 2020 2020 2020 2020 2020 2020 6365                ce
-00011150: 6e74 7261 6c5f 7365 7269 6573 203d 2063  ntral_series = c
-00011160: 6f6d 702e 6d65 616e 2864 696d 3d44 494d  omp.mean(dim=DIM
-00011170: 535b 325d 290a 0a20 2020 2020 2020 2020  S[2])..         
-00011180: 2020 2023 2074 656d 706f 7261 7269 6c79     # temporarily
-00011190: 2073 6574 2061 6c70 6861 2074 6f20 3120   set alpha to 1 
-000111a0: 746f 2070 6c6f 7420 7468 6520 6365 6e74  to plot the cent
-000111b0: 7261 6c20 7661 6c75 6520 2874 6869 7320  ral value (this 
-000111c0: 7761 7920 616c 7068 6120 696d 7061 6374  way alpha impact
-000111d0: 7320 6f6e 6c79 2074 6865 2063 6f6e 6669  s only the confi
-000111e0: 6465 6e63 6520 696e 7476 6c73 290a 2020  dence intvls).  
-000111f0: 2020 2020 2020 2020 2020 616c 7068 6120            alpha 
-00011200: 3d20 6b77 6172 6773 5b27 616c 7068 6127  = kwargs['alpha'
-00011210: 5d20 6966 2027 616c 7068 6127 2069 6e20  ] if 'alpha' in 
-00011220: 6b77 6172 6773 2065 6c73 6520 4e6f 6e65  kwargs else None
-00011230: 0a20 2020 2020 2020 2020 2020 206b 7761  .            kwa
-00011240: 7267 735b 2761 6c70 6861 275d 203d 2031  rgs['alpha'] = 1
-00011250: 0a0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
-00011260: 6265 6c5f 746f 5f75 7365 203d 2028 6c61  bel_to_use = (la
-00011270: 6265 6c20 2b20 2827 5f27 202b 2073 7472  bel + ('_' + str
-00011280: 2869 2920 6966 206c 656e 2873 656c 662e  (i) if len(self.
-00011290: 636f 6d70 6f6e 656e 7473 2920 3e20 3120  components) > 1 
-000112a0: 656c 7365 2027 2729 2920 6966 206c 6162  else '')) if lab
-000112b0: 656c 2021 3d20 2727 205c 0a20 2020 2020  el != '' \.     
-000112c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112d0: 2020 2020 2020 656c 7365 2027 2720 2b20        else '' + 
-000112e0: 7374 7228 636f 6d70 5f6e 616d 6529 0a20  str(comp_name). 
-000112f0: 2020 2020 2020 2020 2020 206b 7761 7267             kwarg
-00011300: 735b 276c 6162 656c 275d 203d 206c 6162  s['label'] = lab
-00011310: 656c 5f74 6f5f 7573 650a 0a20 2020 2020  el_to_use..     
-00011320: 2020 2020 2020 2070 203d 2063 656e 7472         p = centr
-00011330: 616c 5f73 6572 6965 732e 706c 6f74 282a  al_series.plot(*
-00011340: 6172 6773 2c20 2a2a 6b77 6172 6773 290a  args, **kwargs).
-00011350: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
-00011360: 725f 7573 6564 203d 2070 5b30 5d2e 6765  r_used = p[0].ge
-00011370: 745f 636f 6c6f 7228 290a 2020 2020 2020  t_color().      
-00011380: 2020 2020 2020 6b77 6172 6773 5b27 616c        kwargs['al
-00011390: 7068 6127 5d20 3d20 616c 7068 6120 6966  pha'] = alpha if
-000113a0: 2061 6c70 6861 2069 7320 6e6f 7420 4e6f   alpha is not No
-000113b0: 6e65 2065 6c73 6520 616c 7068 615f 636f  ne else alpha_co
-000113c0: 6e66 6964 656e 6365 5f69 6e74 766c 730a  nfidence_intvls.
-000113d0: 0a20 2020 2020 2020 2020 2020 2023 204f  .            # O
-000113e0: 7074 696f 6e61 6c6c 7920 7368 6f77 2063  ptionally show c
-000113f0: 6f6e 6669 6465 6e63 6520 696e 7465 7276  onfidence interv
-00011400: 616c 730a 2020 2020 2020 2020 2020 2020  als.            
-00011410: 6966 2063 6f6d 702e 7361 6d70 6c65 2e73  if comp.sample.s
-00011420: 697a 6520 3e20 3120 616e 6420 6c6f 775f  ize > 1 and low_
-00011430: 7175 616e 7469 6c65 2069 7320 6e6f 7420  quantile is not 
-00011440: 4e6f 6e65 2061 6e64 2068 6967 685f 7175  None and high_qu
-00011450: 616e 7469 6c65 2069 7320 6e6f 7420 4e6f  antile is not No
-00011460: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00011470: 2020 2020 2020 2020 6c6f 775f 7365 7269          low_seri
-00011480: 6573 203d 2063 6f6d 702e 7175 616e 7469  es = comp.quanti
-00011490: 6c65 2871 3d6c 6f77 5f71 7561 6e74 696c  le(q=low_quantil
-000114a0: 652c 2064 696d 3d44 494d 535b 325d 290a  e, dim=DIMS[2]).
-000114b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114c0: 2020 2020 6869 6768 5f73 6572 6965 7320      high_series 
-000114d0: 3d20 636f 6d70 2e71 7561 6e74 696c 6528  = comp.quantile(
-000114e0: 713d 6869 6768 5f71 7561 6e74 696c 652c  q=high_quantile,
-000114f0: 2064 696d 3d44 494d 535b 325d 290a 2020   dim=DIMS[2]).  
-00011500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011510: 2020 706c 742e 6669 6c6c 5f62 6574 7765    plt.fill_betwe
-00011520: 656e 2873 656c 662e 7469 6d65 5f69 6e64  en(self.time_ind
-00011530: 6578 2c20 6c6f 775f 7365 7269 6573 2c20  ex, low_series, 
-00011540: 6869 6768 5f73 6572 6965 732c 2063 6f6c  high_series, col
-00011550: 6f72 3d63 6f6c 6f72 5f75 7365 642c 0a20  or=color_used,. 
-00011560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011580: 2020 2020 616c 7068 613d 2861 6c70 6861      alpha=(alpha
-00011590: 5f63 6f6e 6669 6465 6e63 655f 696e 7476  _confidence_intv
-000115a0: 6c73 2069 6620 2761 6c70 6861 2720 6e6f  ls if 'alpha' no
-000115b0: 7420 696e 206b 7761 7267 7320 656c 7365  t in kwargs else
-000115c0: 206b 7761 7267 735b 2761 6c70 6861 275d   kwargs['alpha']
-000115d0: 2929 0a0a 2020 2020 2020 2020 706c 742e  ))..        plt.
-000115e0: 6c65 6765 6e64 2829 0a20 2020 2020 2020  legend().       
-000115f0: 2070 6c74 2e74 6974 6c65 2873 656c 662e   plt.title(self.
-00011600: 5f78 612e 6e61 6d65 293b 0a0a 2020 2020  _xa.name);..    
-00011610: 2222 220a 2020 2020 5369 6d70 6c65 2073  """.    Simple s
-00011620: 7461 7469 7374 6963 732e 2041 7420 7468  tatistics. At th
-00011630: 6520 6d6f 6d65 6e74 2074 6865 7365 2077  e moment these w
-00011640: 6f72 6b20 6f6e 6c79 206f 6e20 6465 7465  ork only on dete
-00011650: 726d 696e 6973 7469 6320 7365 7269 6573  rministic series
-00011660: 2c20 616e 6420 6172 6520 7772 6170 7065  , and are wrappe
-00011670: 6420 6172 6f75 6e64 2050 616e 6461 732e  d around Pandas.
-00011680: 0a20 2020 2022 2222 0a0a 2020 2020 6465  .    """..    de
-00011690: 6620 6d65 616e 2873 656c 662c 2061 7869  f mean(self, axi
-000116a0: 733d 4e6f 6e65 2c20 736b 6970 6e61 3d4e  s=None, skipna=N
-000116b0: 6f6e 652c 206c 6576 656c 3d4e 6f6e 652c  one, level=None,
-000116c0: 206e 756d 6572 6963 5f6f 6e6c 793d 4e6f   numeric_only=No
-000116d0: 6e65 2c20 2a2a 6b77 6172 6773 2920 2d3e  ne, **kwargs) ->
-000116e0: 2066 6c6f 6174 3a0a 2020 2020 2020 2020   float:.        
-000116f0: 7265 7475 726e 2073 656c 662e 7064 5f64  return self.pd_d
-00011700: 6174 6166 7261 6d65 2863 6f70 793d 4661  ataframe(copy=Fa
-00011710: 6c73 6529 2e6d 6561 6e28 6178 6973 2c20  lse).mean(axis, 
-00011720: 736b 6970 6e61 2c20 6c65 7665 6c2c 206e  skipna, level, n
-00011730: 756d 6572 6963 5f6f 6e6c 792c 202a 2a6b  umeric_only, **k
-00011740: 7761 7267 7329 0a0a 2020 2020 6465 6620  wargs)..    def 
-00011750: 7661 7228 7365 6c66 2c20 6178 6973 3d4e  var(self, axis=N
-00011760: 6f6e 652c 2073 6b69 706e 613d 4e6f 6e65  one, skipna=None
-00011770: 2c20 6c65 7665 6c3d 4e6f 6e65 2c20 6464  , level=None, dd
-00011780: 6f66 3d31 2c20 6e75 6d65 7269 635f 6f6e  of=1, numeric_on
-00011790: 6c79 3d4e 6f6e 652c 202a 2a6b 7761 7267  ly=None, **kwarg
-000117a0: 7329 202d 3e20 666c 6f61 743a 0a20 2020  s) -> float:.   
-000117b0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000117c0: 2e70 645f 6461 7461 6672 616d 6528 636f  .pd_dataframe(co
-000117d0: 7079 3d46 616c 7365 292e 7661 7228 6178  py=False).var(ax
-000117e0: 6973 2c20 736b 6970 6e61 2c20 6c65 7665  is, skipna, leve
-000117f0: 6c2c 2064 646f 662c 206e 756d 6572 6963  l, ddof, numeric
-00011800: 5f6f 6e6c 792c 202a 2a6b 7761 7267 7329  _only, **kwargs)
-00011810: 0a0a 2020 2020 6465 6620 7374 6428 7365  ..    def std(se
-00011820: 6c66 2c20 6178 6973 3d4e 6f6e 652c 2073  lf, axis=None, s
-00011830: 6b69 706e 613d 4e6f 6e65 2c20 6c65 7665  kipna=None, leve
-00011840: 6c3d 4e6f 6e65 2c20 6464 6f66 3d31 2c20  l=None, ddof=1, 
-00011850: 6e75 6d65 7269 635f 6f6e 6c79 3d4e 6f6e  numeric_only=Non
-00011860: 652c 202a 2a6b 7761 7267 7329 202d 3e20  e, **kwargs) -> 
-00011870: 666c 6f61 743a 0a20 2020 2020 2020 2072  float:.        r
-00011880: 6574 7572 6e20 7365 6c66 2e70 645f 6461  eturn self.pd_da
-00011890: 7461 6672 616d 6528 636f 7079 3d46 616c  taframe(copy=Fal
-000118a0: 7365 292e 7374 6428 6178 6973 2c20 736b  se).std(axis, sk
-000118b0: 6970 6e61 2c20 6c65 7665 6c2c 2064 646f  ipna, level, ddo
-000118c0: 662c 206e 756d 6572 6963 5f6f 6e6c 792c  f, numeric_only,
-000118d0: 202a 2a6b 7761 7267 7329 0a0a 2020 2020   **kwargs)..    
-000118e0: 6465 6620 736b 6577 2873 656c 662c 2061  def skew(self, a
-000118f0: 7869 733d 4e6f 6e65 2c20 736b 6970 6e61  xis=None, skipna
-00011900: 3d4e 6f6e 652c 206c 6576 656c 3d4e 6f6e  =None, level=Non
-00011910: 652c 206e 756d 6572 6963 5f6f 6e6c 793d  e, numeric_only=
-00011920: 4e6f 6e65 2c20 2a2a 6b77 6172 6773 2920  None, **kwargs) 
-00011930: 2d3e 2066 6c6f 6174 3a0a 2020 2020 2020  -> float:.      
-00011940: 2020 7265 7475 726e 2073 656c 662e 7064    return self.pd
-00011950: 5f64 6174 6166 7261 6d65 2863 6f70 793d  _dataframe(copy=
-00011960: 4661 6c73 6529 2e73 6b65 7728 6178 6973  False).skew(axis
-00011970: 2c20 736b 6970 6e61 2c20 6c65 7665 6c2c  , skipna, level,
-00011980: 206e 756d 6572 6963 5f6f 6e6c 792c 202a   numeric_only, *
-00011990: 2a6b 7761 7267 7329 0a0a 2020 2020 6465  *kwargs)..    de
-000119a0: 6620 6b75 7274 6f73 6973 2873 656c 662c  f kurtosis(self,
-000119b0: 2061 7869 733d 4e6f 6e65 2c20 736b 6970   axis=None, skip
-000119c0: 6e61 3d4e 6f6e 652c 206c 6576 656c 3d4e  na=None, level=N
-000119d0: 6f6e 652c 206e 756d 6572 6963 5f6f 6e6c  one, numeric_onl
-000119e0: 793d 4e6f 6e65 2c20 2a2a 6b77 6172 6773  y=None, **kwargs
-000119f0: 2920 2d3e 2066 6c6f 6174 3a0a 2020 2020  ) -> float:.    
-00011a00: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00011a10: 7064 5f64 6174 6166 7261 6d65 2863 6f70  pd_dataframe(cop
-00011a20: 793d 4661 6c73 6529 2e6b 7572 746f 7369  y=False).kurtosi
-00011a30: 7328 6178 6973 2c20 736b 6970 6e61 2c20  s(axis, skipna, 
-00011a40: 6c65 7665 6c2c 206e 756d 6572 6963 5f6f  level, numeric_o
-00011a50: 6e6c 792c 202a 2a6b 7761 7267 7329 0a0a  nly, **kwargs)..
-00011a60: 2020 2020 6465 6620 6d69 6e28 7365 6c66      def min(self
-00011a70: 2c20 6178 6973 3d4e 6f6e 652c 2073 6b69  , axis=None, ski
-00011a80: 706e 613d 4e6f 6e65 2c20 6c65 7665 6c3d  pna=None, level=
-00011a90: 4e6f 6e65 2c20 6e75 6d65 7269 635f 6f6e  None, numeric_on
-00011aa0: 6c79 3d4e 6f6e 652c 202a 2a6b 7761 7267  ly=None, **kwarg
-00011ab0: 7329 202d 3e20 666c 6f61 743a 0a20 2020  s) -> float:.   
-00011ac0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00011ad0: 2e70 645f 6461 7461 6672 616d 6528 636f  .pd_dataframe(co
-00011ae0: 7079 3d46 616c 7365 292e 6d69 6e28 6178  py=False).min(ax
-00011af0: 6973 2c20 736b 6970 6e61 2c20 6c65 7665  is, skipna, leve
-00011b00: 6c2c 206e 756d 6572 6963 5f6f 6e6c 792c  l, numeric_only,
-00011b10: 202a 2a6b 7761 7267 7329 0a0a 2020 2020   **kwargs)..    
-00011b20: 6465 6620 6d61 7828 7365 6c66 2c20 6178  def max(self, ax
-00011b30: 6973 3d4e 6f6e 652c 2073 6b69 706e 613d  is=None, skipna=
-00011b40: 4e6f 6e65 2c20 6c65 7665 6c3d 4e6f 6e65  None, level=None
-00011b50: 2c20 6e75 6d65 7269 635f 6f6e 6c79 3d4e  , numeric_only=N
-00011b60: 6f6e 652c 202a 2a6b 7761 7267 7329 202d  one, **kwargs) -
-00011b70: 3e20 666c 6f61 743a 0a20 2020 2020 2020  > float:.       
-00011b80: 2072 6574 7572 6e20 7365 6c66 2e70 645f   return self.pd_
-00011b90: 6461 7461 6672 616d 6528 636f 7079 3d46  dataframe(copy=F
-00011ba0: 616c 7365 292e 6d61 7828 6178 6973 2c20  alse).max(axis, 
-00011bb0: 736b 6970 6e61 2c20 6c65 7665 6c2c 206e  skipna, level, n
-00011bc0: 756d 6572 6963 5f6f 6e6c 792c 202a 2a6b  umeric_only, **k
-00011bd0: 7761 7267 7329 0a0a 2020 2020 6465 6620  wargs)..    def 
-00011be0: 7375 6d28 7365 6c66 2c20 6178 6973 3d4e  sum(self, axis=N
-00011bf0: 6f6e 652c 2073 6b69 706e 613d 4e6f 6e65  one, skipna=None
-00011c00: 2c20 6c65 7665 6c3d 4e6f 6e65 2c20 6e75  , level=None, nu
-00011c10: 6d65 7269 635f 6f6e 6c79 3d4e 6f6e 652c  meric_only=None,
-00011c20: 206d 696e 5f63 6f75 6e74 3d30 2c20 2a2a   min_count=0, **
-00011c30: 6b77 6172 6773 2920 2d3e 2066 6c6f 6174  kwargs) -> float
-00011c40: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00011c50: 2073 656c 662e 7064 5f64 6174 6166 7261   self.pd_datafra
-00011c60: 6d65 2863 6f70 793d 4661 6c73 6529 2e73  me(copy=False).s
-00011c70: 756d 2861 7869 732c 2073 6b69 706e 612c  um(axis, skipna,
-00011c80: 206c 6576 656c 2c20 6e75 6d65 7269 635f   level, numeric_
-00011c90: 6f6e 6c79 2c20 6d69 6e5f 636f 756e 742c  only, min_count,
-00011ca0: 202a 2a6b 7761 7267 7329 0a0a 2020 2020   **kwargs)..    
-00011cb0: 6465 6620 6d65 6469 616e 2873 656c 662c  def median(self,
-00011cc0: 2061 7869 733d 4e6f 6e65 2c20 736b 6970   axis=None, skip
-00011cd0: 6e61 3d4e 6f6e 652c 206c 6576 656c 3d4e  na=None, level=N
-00011ce0: 6f6e 652c 206e 756d 6572 6963 5f6f 6e6c  one, numeric_onl
-00011cf0: 793d 4e6f 6e65 2c20 2a2a 6b77 6172 6773  y=None, **kwargs
-00011d00: 2920 2d3e 2066 6c6f 6174 3a0a 2020 2020  ) -> float:.    
-00011d10: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00011d20: 7064 5f64 6174 6166 7261 6d65 2863 6f70  pd_dataframe(cop
-00011d30: 793d 4661 6c73 6529 2e6d 6564 6961 6e28  y=False).median(
-00011d40: 6178 6973 2c20 736b 6970 6e61 2c20 6c65  axis, skipna, le
-00011d50: 7665 6c2c 206e 756d 6572 6963 5f6f 6e6c  vel, numeric_onl
-00011d60: 792c 202a 2a6b 7761 7267 7329 0a0a 2020  y, **kwargs)..  
-00011d70: 2020 6465 6620 6175 746f 636f 7272 2873    def autocorr(s
-00011d80: 656c 662c 206c 6167 3d31 2920 2d3e 2066  elf, lag=1) -> f
-00011d90: 6c6f 6174 3a0a 2020 2020 2020 2020 7265  loat:.        re
-00011da0: 7475 726e 2073 656c 662e 7064 5f64 6174  turn self.pd_dat
-00011db0: 6166 7261 6d65 2863 6f70 793d 4661 6c73  aframe(copy=Fals
-00011dc0: 6529 2e61 7574 6f63 6f72 7228 6c61 6729  e).autocorr(lag)
-00011dd0: 0a0a 2020 2020 6465 6620 6465 7363 7269  ..    def descri
-00011de0: 6265 2873 656c 662c 2070 6572 6365 6e74  be(self, percent
-00011df0: 696c 6573 3d4e 6f6e 652c 2069 6e63 6c75  iles=None, inclu
-00011e00: 6465 3d4e 6f6e 652c 2065 7863 6c75 6465  de=None, exclude
-00011e10: 3d4e 6f6e 6529 202d 3e20 7064 2e44 6174  =None) -> pd.Dat
-00011e20: 6146 7261 6d65 3a0a 2020 2020 2020 2020  aFrame:.        
-00011e30: 7265 7475 726e 2073 656c 662e 7064 5f64  return self.pd_d
-00011e40: 6174 6166 7261 6d65 2863 6f70 793d 4661  ataframe(copy=Fa
-00011e50: 6c73 6529 2e64 6573 6372 6962 6528 7065  lse).describe(pe
-00011e60: 7263 656e 7469 6c65 732c 2069 6e63 6c75  rcentiles, inclu
-00011e70: 6465 2c20 6578 636c 7564 6529 0a0a 2020  de, exclude)..  
-00011e80: 2020 2222 220a 2020 2020 4475 6e64 6572    """.    Dunder
-00011e90: 206d 6574 686f 6473 0a20 2020 2022 2222   methods.    """
-00011ea0: 0a0a 2020 2020 230a 2020 2020 6465 6620  ..    #.    def 
-00011eb0: 5f63 6f6d 6269 6e65 5f61 7272 6179 7328  _combine_arrays(
-00011ec0: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-00011ed0: 2020 2020 2020 2020 2020 2020 2020 6f74                ot
-00011ee0: 6865 723a 2055 6e69 6f6e 5b27 5469 6d65  her: Union['Time
-00011ef0: 5365 7269 6573 272c 2078 722e 4461 7461  Series', xr.Data
-00011f00: 4172 7261 792c 206e 702e 6e64 6172 7261  Array, np.ndarra
-00011f10: 795d 2c0a 2020 2020 2020 2020 2020 2020  y],.            
-00011f20: 2020 2020 2020 2020 2020 2020 636f 6d62              comb
-00011f30: 696e 655f 666e 3a20 4361 6c6c 6162 6c65  ine_fn: Callable
-00011f40: 5b5b 6e70 2e6e 6461 7272 6179 2c20 6e70  [[np.ndarray, np
-00011f50: 2e6e 6461 7272 6179 5d2c 206e 702e 6e64  .ndarray], np.nd
-00011f60: 6172 7261 795d 2920 2d3e 2027 5469 6d65  array]) -> 'Time
-00011f70: 5365 7269 6573 273a 0a20 2020 2020 2020  Series':.       
-00011f80: 2022 2222 0a20 2020 2020 2020 2054 6869   """.        Thi
-00011f90: 7320 6973 2061 2068 656c 7065 7220 6675  s is a helper fu
-00011fa0: 6e63 7469 6f6e 2074 6861 7420 616c 6c6f  nction that allo
-00011fb0: 7773 2075 7320 746f 2063 6f6d 6269 6e65  ws us to combine
-00011fc0: 2074 6869 7320 7365 7269 6573 2077 6974   this series wit
-00011fd0: 6820 616e 6f74 6865 7220 6f6e 652c 0a20  h another one,. 
-00011fe0: 2020 2020 2020 2064 6972 6563 746c 7920         directly 
-00011ff0: 6170 706c 7969 6e67 2061 6e20 6f70 6572  applying an oper
-00012000: 6174 696f 6e20 6f6e 2074 6865 6972 2075  ation on their u
-00012010: 6e64 6572 6c79 696e 6720 6e75 6d70 7920  nderlying numpy 
-00012020: 6172 7261 7973 2e0a 2020 2020 2020 2020  arrays..        
-00012030: 2222 220a 0a20 2020 2020 2020 2069 6620  """..        if 
-00012040: 6973 696e 7374 616e 6365 286f 7468 6572  isinstance(other
-00012050: 2c20 5469 6d65 5365 7269 6573 293a 0a20  , TimeSeries):. 
-00012060: 2020 2020 2020 2020 2020 206f 7468 6572             other
-00012070: 5f76 616c 7320 3d20 6f74 6865 722e 6461  _vals = other.da
-00012080: 7461 5f61 7272 6179 2863 6f70 793d 4661  ta_array(copy=Fa
-00012090: 6c73 6529 2e76 616c 7565 730a 2020 2020  lse).values.    
-000120a0: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
-000120b0: 6e63 6528 6f74 6865 722c 2078 722e 4461  nce(other, xr.Da
-000120c0: 7461 4172 7261 7929 3a0a 2020 2020 2020  taArray):.      
-000120d0: 2020 2020 2020 6f74 6865 725f 7661 6c73        other_vals
-000120e0: 203d 206f 7468 6572 2e76 616c 7565 730a   = other.values.
-000120f0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00012100: 2020 2020 2020 2020 2020 6f74 6865 725f            other_
-00012110: 7661 6c73 203d 206f 7468 6572 0a0a 2020  vals = other..  
-00012120: 2020 2020 2020 7261 6973 655f 6966 5f6e        raise_if_n
-00012130: 6f74 2873 656c 662e 5f78 612e 7661 6c75  ot(self._xa.valu
-00012140: 6573 2e73 6861 7065 203d 3d20 6f74 6865  es.shape == othe
-00012150: 725f 7661 6c73 2e73 6861 7065 2c20 2741  r_vals.shape, 'A
-00012160: 7474 656d 7074 6564 2074 6f20 7065 7266  ttempted to perf
-00012170: 6f72 6d20 6f70 6572 6174 696f 6e20 6f6e  orm operation on
-00012180: 2074 776f 2054 696d 6553 6572 6965 7320   two TimeSeries 
-00012190: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-000121a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121d0: 2020 276f 6620 756e 6571 7561 6c20 7368    'of unequal sh
-000121e0: 6170 6573 2e27 2c20 6c6f 6767 6572 290a  apes.', logger).
-000121f0: 2020 2020 2020 2020 6e65 775f 7861 203d          new_xa =
-00012200: 2073 656c 662e 5f78 612e 636f 7079 2829   self._xa.copy()
-00012210: 0a20 2020 2020 2020 206e 6577 5f78 612e  .        new_xa.
-00012220: 7661 6c75 6573 203d 2063 6f6d 6269 6e65  values = combine
-00012230: 5f66 6e28 6e65 775f 7861 2e76 616c 7565  _fn(new_xa.value
-00012240: 732c 206f 7468 6572 5f76 616c 7329 0a20  s, other_vals). 
-00012250: 2020 2020 2020 2072 6574 7572 6e20 5469         return Ti
-00012260: 6d65 5365 7269 6573 286e 6577 5f78 6129  meSeries(new_xa)
-00012270: 0a0a 2020 2020 6465 6620 5f5f 6571 5f5f  ..    def __eq__
-00012280: 2873 656c 662c 206f 7468 6572 293a 0a20  (self, other):. 
-00012290: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-000122a0: 616e 6365 286f 7468 6572 2c20 5469 6d65  ance(other, Time
-000122b0: 5365 7269 6573 293a 0a20 2020 2020 2020  Series):.       
-000122c0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000122d0: 2e5f 7861 2e65 7175 616c 7328 6f74 6865  ._xa.equals(othe
-000122e0: 722e 6461 7461 5f61 7272 6179 2863 6f70  r.data_array(cop
-000122f0: 793d 4661 6c73 6529 290a 2020 2020 2020  y=False)).      
-00012300: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
-00012310: 2020 2020 6465 6620 5f5f 6e65 5f5f 2873      def __ne__(s
-00012320: 656c 662c 206f 7468 6572 293a 0a20 2020  elf, other):.   
-00012330: 2020 2020 2072 6574 7572 6e20 6e6f 7420       return not 
-00012340: 7365 6c66 2e5f 5f65 715f 5f28 6f74 6865  self.__eq__(othe
-00012350: 7229 0a0a 2020 2020 6465 6620 5f5f 6c65  r)..    def __le
-00012360: 6e5f 5f28 7365 6c66 293a 0a20 2020 2020  n__(self):.     
-00012370: 2020 2072 6574 7572 6e20 6c65 6e28 7365     return len(se
-00012380: 6c66 2e5f 7861 290a 0a20 2020 2064 6566  lf._xa)..    def
-00012390: 205f 5f61 6464 5f5f 2873 656c 662c 206f   __add__(self, o
-000123a0: 7468 6572 293a 0a20 2020 2020 2020 2069  ther):.        i
-000123b0: 6620 6973 696e 7374 616e 6365 286f 7468  f isinstance(oth
-000123c0: 6572 2c20 2869 6e74 2c20 666c 6f61 742c  er, (int, float,
-000123d0: 206e 702e 696e 7465 6765 7229 293a 0a20   np.integer)):. 
-000123e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000123f0: 6e20 5469 6d65 5365 7269 6573 2873 656c  n TimeSeries(sel
-00012400: 662e 5f78 6120 2b20 6f74 6865 7229 0a20  f._xa + other). 
-00012410: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
-00012420: 7374 616e 6365 286f 7468 6572 2c20 2854  stance(other, (T
-00012430: 696d 6553 6572 6965 732c 2078 722e 4461  imeSeries, xr.Da
-00012440: 7461 4172 7261 792c 206e 702e 6e64 6172  taArray, np.ndar
-00012450: 7261 7929 293a 0a20 2020 2020 2020 2020  ray)):.         
-00012460: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00012470: 636f 6d62 696e 655f 6172 7261 7973 286f  combine_arrays(o
-00012480: 7468 6572 2c20 6c61 6d62 6461 2073 312c  ther, lambda s1,
-00012490: 2073 323a 2073 3120 2b20 7332 290a 2020   s2: s1 + s2).  
-000124a0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000124b0: 2020 2020 2020 2020 7261 6973 655f 6c6f          raise_lo
-000124c0: 6728 5479 7065 4572 726f 7228 2775 6e73  g(TypeError('uns
-000124d0: 7570 706f 7274 6564 206f 7065 7261 6e64  upported operand
-000124e0: 2074 7970 6528 7329 2066 6f72 202b 206f   type(s) for + o
-000124f0: 7220 6164 6428 293a 205c 277b 7d5c 2720  r add(): \'{}\' 
-00012500: 616e 6420 5c27 7b7d 5c27 2e27 0a20 2020  and \'{}\'.'.   
-00012510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012520: 2020 2020 2020 2020 2020 2020 202e 666f               .fo
-00012530: 726d 6174 2874 7970 6528 7365 6c66 292e  rmat(type(self).
-00012540: 5f5f 6e61 6d65 5f5f 2c20 7479 7065 286f  __name__, type(o
-00012550: 7468 6572 292e 5f5f 6e61 6d65 5f5f 2929  ther).__name__))
-00012560: 2c20 6c6f 6767 6572 290a 0a20 2020 2064  , logger)..    d
-00012570: 6566 205f 5f72 6164 645f 5f28 7365 6c66  ef __radd__(self
-00012580: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
-00012590: 2020 7265 7475 726e 2073 656c 6620 2b20    return self + 
-000125a0: 6f74 6865 720a 0a20 2020 2064 6566 205f  other..    def _
-000125b0: 5f73 7562 5f5f 2873 656c 662c 206f 7468  _sub__(self, oth
-000125c0: 6572 293a 0a20 2020 2020 2020 2069 6620  er):.        if 
-000125d0: 6973 696e 7374 616e 6365 286f 7468 6572  isinstance(other
-000125e0: 2c20 2869 6e74 2c20 666c 6f61 742c 206e  , (int, float, n
-000125f0: 702e 696e 7465 6765 7229 293a 0a20 2020  p.integer)):.   
-00012600: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00012610: 5469 6d65 5365 7269 6573 2873 656c 662e  TimeSeries(self.
-00012620: 5f78 6120 2d20 6f74 6865 7229 0a20 2020  _xa - other).   
-00012630: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
-00012640: 616e 6365 286f 7468 6572 2c20 2854 696d  ance(other, (Tim
-00012650: 6553 6572 6965 732c 2078 722e 4461 7461  eSeries, xr.Data
-00012660: 4172 7261 792c 206e 702e 6e64 6172 7261  Array, np.ndarra
-00012670: 7929 293a 0a20 2020 2020 2020 2020 2020  y)):.           
-00012680: 2072 6574 7572 6e20 7365 6c66 2e5f 636f   return self._co
-00012690: 6d62 696e 655f 6172 7261 7973 286f 7468  mbine_arrays(oth
-000126a0: 6572 2c20 6c61 6d62 6461 2073 312c 2073  er, lambda s1, s
-000126b0: 323a 2073 3120 2d20 7332 290a 2020 2020  2: s1 - s2).    
-000126c0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000126d0: 2020 2020 2020 7261 6973 655f 6c6f 6728        raise_log(
-000126e0: 5479 7065 4572 726f 7228 2775 6e73 7570  TypeError('unsup
-000126f0: 706f 7274 6564 206f 7065 7261 6e64 2074  ported operand t
-00012700: 7970 6528 7329 2066 6f72 202d 206f 7220  ype(s) for - or 
-00012710: 7375 6228 293a 205c 277b 7d5c 2720 616e  sub(): \'{}\' an
-00012720: 6420 5c27 7b7d 5c27 2e27 0a20 2020 2020  d \'{}\'.'.     
-00012730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012740: 2020 2020 2020 2020 2020 202e 666f 726d             .form
-00012750: 6174 2874 7970 6528 7365 6c66 292e 5f5f  at(type(self).__
-00012760: 6e61 6d65 5f5f 2c20 7479 7065 286f 7468  name__, type(oth
-00012770: 6572 292e 5f5f 6e61 6d65 5f5f 2929 2c20  er).__name__)), 
-00012780: 6c6f 6767 6572 290a 0a20 2020 2064 6566  logger)..    def
-00012790: 205f 5f72 7375 625f 5f28 7365 6c66 2c20   __rsub__(self, 
-000127a0: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
-000127b0: 7265 7475 726e 206f 7468 6572 202b 2028  return other + (
-000127c0: 2d73 656c 6629 0a0a 2020 2020 6465 6620  -self)..    def 
-000127d0: 5f5f 6d75 6c5f 5f28 7365 6c66 2c20 6f74  __mul__(self, ot
-000127e0: 6865 7229 3a0a 2020 2020 2020 2020 6966  her):.        if
-000127f0: 2069 7369 6e73 7461 6e63 6528 6f74 6865   isinstance(othe
-00012800: 722c 2028 696e 742c 2066 6c6f 6174 2c20  r, (int, float, 
-00012810: 6e70 2e69 6e74 6567 6572 2929 3a0a 2020  np.integer)):.  
-00012820: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00012830: 2054 696d 6553 6572 6965 7328 7365 6c66   TimeSeries(self
-00012840: 2e5f 7861 202a 206f 7468 6572 290a 2020  ._xa * other).  
-00012850: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
-00012860: 7461 6e63 6528 6f74 6865 722c 2028 5469  tance(other, (Ti
-00012870: 6d65 5365 7269 6573 2c20 7872 2e44 6174  meSeries, xr.Dat
-00012880: 6141 7272 6179 2c20 6e70 2e6e 6461 7272  aArray, np.ndarr
-00012890: 6179 2929 3a0a 2020 2020 2020 2020 2020  ay)):.          
-000128a0: 2020 7265 7475 726e 2073 656c 662e 5f63    return self._c
-000128b0: 6f6d 6269 6e65 5f61 7272 6179 7328 6f74  ombine_arrays(ot
-000128c0: 6865 722c 206c 616d 6264 6120 7331 2c20  her, lambda s1, 
-000128d0: 7332 3a20 7331 202a 2073 3229 0a20 2020  s2: s1 * s2).   
-000128e0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000128f0: 2020 2020 2020 2072 6169 7365 5f6c 6f67         raise_log
-00012900: 2854 7970 6545 7272 6f72 2827 756e 7375  (TypeError('unsu
-00012910: 7070 6f72 7465 6420 6f70 6572 616e 6420  pported operand 
-00012920: 7479 7065 2873 2920 666f 7220 2a20 6f72  type(s) for * or
-00012930: 206d 756c 2829 3a20 5c27 7b7d 5c27 2061   mul(): \'{}\' a
-00012940: 6e64 205c 277b 7d5c 272e 270a 2020 2020  nd \'{}\'.'.    
-00012950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012960: 2020 2020 2020 2020 2020 2020 2e66 6f72              .for
-00012970: 6d61 7428 7479 7065 2873 656c 6629 2e5f  mat(type(self)._
-00012980: 5f6e 616d 655f 5f2c 2074 7970 6528 6f74  _name__, type(ot
-00012990: 6865 7229 2e5f 5f6e 616d 655f 5f29 292c  her).__name__)),
-000129a0: 206c 6f67 6765 7229 0a0a 2020 2020 6465   logger)..    de
-000129b0: 6620 5f5f 726d 756c 5f5f 2873 656c 662c  f __rmul__(self,
-000129c0: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
-000129d0: 2072 6574 7572 6e20 7365 6c66 202a 206f   return self * o
-000129e0: 7468 6572 0a0a 2020 2020 6465 6620 5f5f  ther..    def __
-000129f0: 706f 775f 5f28 7365 6c66 2c20 6e29 3a0a  pow__(self, n):.
-00012a00: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-00012a10: 7461 6e63 6528 6e2c 2028 696e 742c 2066  tance(n, (int, f
-00012a20: 6c6f 6174 2c20 6e70 2e69 6e74 6567 6572  loat, np.integer
-00012a30: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-00012a40: 7261 6973 655f 6966 286e 203c 2030 2c20  raise_if(n < 0, 
-00012a50: 2741 7474 656d 7074 6564 2074 6f20 7261  'Attempted to ra
-00012a60: 6973 6520 6120 7365 7269 6573 2074 6f20  ise a series to 
-00012a70: 6120 6e65 6761 7469 7665 2070 6f77 6572  a negative power
-00012a80: 2e27 2c20 6c6f 6767 6572 290a 2020 2020  .', logger).    
-00012a90: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-00012aa0: 696d 6553 6572 6965 7328 7365 6c66 2e5f  imeSeries(self._
-00012ab0: 7861 202a 2a20 666c 6f61 7428 6e29 290a  xa ** float(n)).
-00012ac0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-00012ad0: 7461 6e63 6528 6e2c 2028 5469 6d65 5365  tance(n, (TimeSe
-00012ae0: 7269 6573 2c20 7872 2e44 6174 6141 7272  ries, xr.DataArr
-00012af0: 6179 2c20 6e70 2e6e 6461 7272 6179 2929  ay, np.ndarray))
-00012b00: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00012b10: 7475 726e 2073 656c 662e 5f63 6f6d 6269  turn self._combi
-00012b20: 6e65 5f61 7272 6179 7328 6e2c 206c 616d  ne_arrays(n, lam
-00012b30: 6264 6120 7331 2c20 7332 3a20 7331 202a  bda s1, s2: s1 *
-00012b40: 2a20 7332 2920 2023 2065 6c65 6d65 6e74  * s2)  # element
-00012b50: 7769 7365 2070 6f77 6572 0a20 2020 2020  wise power.     
-00012b60: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00012b70: 2020 2020 2072 6169 7365 5f6c 6f67 2854       raise_log(T
-00012b80: 7970 6545 7272 6f72 2827 756e 7375 7070  ypeError('unsupp
-00012b90: 6f72 7465 6420 6f70 6572 616e 6420 7479  orted operand ty
-00012ba0: 7065 2873 2920 666f 7220 2a2a 206f 7220  pe(s) for ** or 
-00012bb0: 706f 7728 293a 205c 277b 7d5c 2720 616e  pow(): \'{}\' an
-00012bc0: 6420 5c27 7b7d 5c27 2e27 0a20 2020 2020  d \'{}\'.'.     
-00012bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012be0: 2020 2020 2020 2020 2020 202e 666f 726d             .form
-00012bf0: 6174 2874 7970 6528 7365 6c66 292e 5f5f  at(type(self).__
-00012c00: 6e61 6d65 5f5f 2c20 7479 7065 286e 292e  name__, type(n).
-00012c10: 5f5f 6e61 6d65 5f5f 2929 2c20 6c6f 6767  __name__)), logg
-00012c20: 6572 290a 0a20 2020 2064 6566 205f 5f74  er)..    def __t
-00012c30: 7275 6564 6976 5f5f 2873 656c 662c 206f  ruediv__(self, o
-00012c40: 7468 6572 293a 0a20 2020 2020 2020 2069  ther):.        i
-00012c50: 6620 6973 696e 7374 616e 6365 286f 7468  f isinstance(oth
-00012c60: 6572 2c20 2869 6e74 2c20 666c 6f61 742c  er, (int, float,
-00012c70: 206e 702e 696e 7465 6765 7229 293a 0a20   np.integer)):. 
-00012c80: 2020 2020 2020 2020 2020 2069 6620 6f74             if ot
-00012c90: 6865 7220 3d3d 2030 3a0a 2020 2020 2020  her == 0:.      
-00012ca0: 2020 2020 2020 2020 2020 7261 6973 655f            raise_
-00012cb0: 6c6f 6728 5a65 726f 4469 7669 7369 6f6e  log(ZeroDivision
-00012cc0: 4572 726f 7228 2743 616e 6e6f 7420 6469  Error('Cannot di
-00012cd0: 7669 6465 2062 7920 302e 2729 2c20 6c6f  vide by 0.'), lo
-00012ce0: 6767 6572 290a 2020 2020 2020 2020 2020  gger).          
-00012cf0: 2020 7265 7475 726e 2054 696d 6553 6572    return TimeSer
-00012d00: 6965 7328 7365 6c66 2e5f 7861 202f 206f  ies(self._xa / o
-00012d10: 7468 6572 290a 2020 2020 2020 2020 656c  ther).        el
-00012d20: 6966 2069 7369 6e73 7461 6e63 6528 6f74  if isinstance(ot
-00012d30: 6865 722c 2028 5469 6d65 5365 7269 6573  her, (TimeSeries
-00012d40: 2c20 7872 2e44 6174 6141 7272 6179 2c20  , xr.DataArray, 
-00012d50: 6e70 2e6e 6461 7272 6179 2929 3a0a 2020  np.ndarray)):.  
-00012d60: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00012d70: 2028 6f74 6865 722e 616c 6c5f 7661 6c75   (other.all_valu
-00012d80: 6573 2829 2021 3d20 3029 2e61 6c6c 2829  es() != 0).all()
-00012d90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012da0: 2020 7261 6973 655f 6c6f 6728 5a65 726f    raise_log(Zero
-00012db0: 4469 7669 7369 6f6e 4572 726f 7228 2743  DivisionError('C
-00012dc0: 616e 6e6f 7420 6469 7669 6465 2062 7920  annot divide by 
-00012dd0: 6120 5469 6d65 5365 7269 6573 2077 6974  a TimeSeries wit
-00012de0: 6820 6120 7661 6c75 6520 302e 2729 2c20  h a value 0.'), 
-00012df0: 6c6f 6767 6572 290a 2020 2020 2020 2020  logger).        
-00012e00: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00012e10: 5f63 6f6d 6269 6e65 5f61 7272 6179 7328  _combine_arrays(
-00012e20: 6f74 6865 722c 206c 616d 6264 6120 7331  other, lambda s1
-00012e30: 2c20 7332 3a20 7331 202f 2073 3229 0a20  , s2: s1 / s2). 
-00012e40: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00012e50: 2020 2020 2020 2020 2072 6169 7365 5f6c           raise_l
-00012e60: 6f67 2854 7970 6545 7272 6f72 2827 756e  og(TypeError('un
-00012e70: 7375 7070 6f72 7465 6420 6f70 6572 616e  supported operan
-00012e80: 6420 7479 7065 2873 2920 666f 7220 2f20  d type(s) for / 
-00012e90: 6f72 2074 7275 6564 6976 2829 3a20 5c27  or truediv(): \'
-00012ea0: 7b7d 5c27 2061 6e64 205c 277b 7d5c 272e  {}\' and \'{}\'.
-00012eb0: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-00012ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ed0: 2020 2e66 6f72 6d61 7428 7479 7065 2873    .format(type(s
-00012ee0: 656c 6629 2e5f 5f6e 616d 655f 5f2c 2074  elf).__name__, t
-00012ef0: 7970 6528 6f74 6865 7229 2e5f 5f6e 616d  ype(other).__nam
-00012f00: 655f 5f29 292c 206c 6f67 6765 7229 0a0a  e__)), logger)..
-00012f10: 2020 2020 6465 6620 5f5f 7274 7275 6564      def __rtrued
-00012f20: 6976 5f5f 2873 656c 662c 206e 293a 0a20  iv__(self, n):. 
-00012f30: 2020 2020 2020 2072 6574 7572 6e20 6e20         return n 
-00012f40: 2a20 2873 656c 6620 2a2a 2028 2d31 2929  * (self ** (-1))
-00012f50: 0a0a 2020 2020 6465 6620 5f5f 6162 735f  ..    def __abs_
-00012f60: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
-00012f70: 2072 6574 7572 6e20 5469 6d65 5365 7269   return TimeSeri
-00012f80: 6573 2861 6273 2873 656c 662e 5f78 6129  es(abs(self._xa)
-00012f90: 290a 0a20 2020 2064 6566 205f 5f6e 6567  )..    def __neg
-00012fa0: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
-00012fb0: 2020 7265 7475 726e 2054 696d 6553 6572    return TimeSer
-00012fc0: 6965 7328 2d73 656c 662e 5f78 6129 0a0a  ies(-self._xa)..
-00012fd0: 2020 2020 6465 6620 5f5f 636f 6e74 6169      def __contai
-00012fe0: 6e73 5f5f 2873 656c 662c 2074 733a 2055  ns__(self, ts: U
-00012ff0: 6e69 6f6e 5b69 6e74 2c20 7064 2e54 696d  nion[int, pd.Tim
-00013000: 6573 7461 6d70 5d29 202d 3e20 626f 6f6c  estamp]) -> bool
-00013010: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00013020: 2074 7320 696e 2073 656c 662e 7469 6d65   ts in self.time
-00013030: 5f69 6e64 6578 0a0a 2020 2020 6465 6620  _index..    def 
-00013040: 5f5f 726f 756e 645f 5f28 7365 6c66 2c20  __round__(self, 
-00013050: 6e3d 4e6f 6e65 293a 0a20 2020 2020 2020  n=None):.       
-00013060: 2072 6574 7572 6e20 5469 6d65 5365 7269   return TimeSeri
-00013070: 6573 2873 656c 662e 5f78 612e 726f 756e  es(self._xa.roun
-00013080: 6428 6e29 290a 0a20 2020 2064 6566 205f  d(n))..    def _
-00013090: 5f6c 745f 5f28 7365 6c66 2c20 6f74 6865  _lt__(self, othe
-000130a0: 7229 202d 3e20 7872 2e44 6174 6141 7272  r) -> xr.DataArr
-000130b0: 6179 3a0a 2020 2020 2020 2020 6966 2069  ay:.        if i
-000130c0: 7369 6e73 7461 6e63 6528 6f74 6865 722c  sinstance(other,
-000130d0: 2028 696e 742c 2066 6c6f 6174 2c20 6e70   (int, float, np
-000130e0: 2e69 6e74 6567 6572 2c20 6e70 2e6e 6461  .integer, np.nda
-000130f0: 7272 6179 2c20 7872 2e44 6174 6141 7272  rray, xr.DataArr
-00013100: 6179 2929 3a0a 2020 2020 2020 2020 2020  ay)):.          
-00013110: 2020 7365 7269 6573 203d 2073 656c 662e    series = self.
-00013120: 5f78 6120 3c20 6f74 6865 720a 2020 2020  _xa < other.    
-00013130: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
-00013140: 6e63 6528 6f74 6865 722c 2054 696d 6553  nce(other, TimeS
-00013150: 6572 6965 7329 3a0a 2020 2020 2020 2020  eries):.        
-00013160: 2020 2020 7365 7269 6573 203d 2073 656c      series = sel
-00013170: 662e 5f78 6120 3c20 6f74 6865 722e 6461  f._xa < other.da
-00013180: 7461 5f61 7272 6179 2863 6f70 793d 4661  ta_array(copy=Fa
-00013190: 6c73 6529 0a20 2020 2020 2020 2065 6c73  lse).        els
-000131a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000131b0: 6169 7365 5f6c 6f67 2854 7970 6545 7272  aise_log(TypeErr
-000131c0: 6f72 2827 756e 7375 7070 6f72 7465 6420  or('unsupported 
-000131d0: 6f70 6572 616e 6420 7479 7065 2873 2920  operand type(s) 
-000131e0: 666f 7220 3c20 3a20 5c27 7b7d 5c27 2061  for < : \'{}\' a
-000131f0: 6e64 205c 277b 7d5c 272e 270a 2020 2020  nd \'{}\'.'.    
-00013200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013210: 2020 2020 2020 2020 2020 2020 2e66 6f72              .for
-00013220: 6d61 7428 7479 7065 2873 656c 6629 2e5f  mat(type(self)._
-00013230: 5f6e 616d 655f 5f2c 2074 7970 6528 6f74  _name__, type(ot
-00013240: 6865 7229 2e5f 5f6e 616d 655f 5f29 292c  her).__name__)),
-00013250: 206c 6f67 6765 7229 0a20 2020 2020 2020   logger).       
-00013260: 2072 6574 7572 6e20 7365 7269 6573 2020   return series  
-00013270: 2320 4e6f 7465 3a20 7765 2072 6574 7572  # Note: we retur
-00013280: 6e20 6120 4461 7461 4172 7261 790a 0a20  n a DataArray.. 
-00013290: 2020 2064 6566 205f 5f67 745f 5f28 7365     def __gt__(se
-000132a0: 6c66 2c20 6f74 6865 7229 202d 3e20 7872  lf, other) -> xr
-000132b0: 2e44 6174 6141 7272 6179 3a0a 2020 2020  .DataArray:.    
-000132c0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-000132d0: 6528 6f74 6865 722c 2028 696e 742c 2066  e(other, (int, f
-000132e0: 6c6f 6174 2c20 6e70 2e69 6e74 6567 6572  loat, np.integer
-000132f0: 2c20 6e70 2e6e 6461 7272 6179 2c20 7872  , np.ndarray, xr
-00013300: 2e44 6174 6141 7272 6179 2929 3a0a 2020  .DataArray)):.  
-00013310: 2020 2020 2020 2020 2020 7365 7269 6573            series
-00013320: 203d 2073 656c 662e 5f78 6120 3e20 6f74   = self._xa > ot
-00013330: 6865 720a 2020 2020 2020 2020 656c 6966  her.        elif
-00013340: 2069 7369 6e73 7461 6e63 6528 6f74 6865   isinstance(othe
-00013350: 722c 2054 696d 6553 6572 6965 7329 3a0a  r, TimeSeries):.
-00013360: 2020 2020 2020 2020 2020 2020 7365 7269              seri
-00013370: 6573 203d 2073 656c 662e 5f78 6120 3e20  es = self._xa > 
-00013380: 6f74 6865 722e 6461 7461 5f61 7272 6179  other.data_array
-00013390: 2863 6f70 793d 4661 6c73 6529 0a20 2020  (copy=False).   
-000133a0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000133b0: 2020 2020 2020 2073 6572 6965 7320 3d20         series = 
-000133c0: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-000133d0: 2072 6169 7365 5f6c 6f67 2854 7970 6545   raise_log(TypeE
-000133e0: 7272 6f72 2827 756e 7375 7070 6f72 7465  rror('unsupporte
-000133f0: 6420 6f70 6572 616e 6420 7479 7065 2873  d operand type(s
-00013400: 2920 666f 7220 3c20 3a20 5c27 7b7d 5c27  ) for < : \'{}\'
-00013410: 2061 6e64 205c 277b 7d5c 272e 270a 2020   and \'{}\'.'.  
-00013420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013430: 2020 2020 2020 2020 2020 2020 2020 2e66                .f
-00013440: 6f72 6d61 7428 7479 7065 2873 656c 6629  ormat(type(self)
-00013450: 2e5f 5f6e 616d 655f 5f2c 2074 7970 6528  .__name__, type(
-00013460: 6f74 6865 7229 2e5f 5f6e 616d 655f 5f29  other).__name__)
-00013470: 292c 206c 6f67 6765 7229 0a20 2020 2020  ), logger).     
-00013480: 2020 2072 6574 7572 6e20 7365 7269 6573     return series
-00013490: 2020 2320 4e6f 7465 3a20 7765 2072 6574    # Note: we ret
-000134a0: 7572 6e20 6120 4461 7461 4172 7261 790a  urn a DataArray.
-000134b0: 0a20 2020 2064 6566 205f 5f6c 655f 5f28  .    def __le__(
-000134c0: 7365 6c66 2c20 6f74 6865 7229 202d 3e20  self, other) -> 
-000134d0: 7872 2e44 6174 6141 7272 6179 3a0a 2020  xr.DataArray:.  
-000134e0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-000134f0: 6e63 6528 6f74 6865 722c 2028 696e 742c  nce(other, (int,
-00013500: 2066 6c6f 6174 2c20 6e70 2e69 6e74 6567   float, np.integ
-00013510: 6572 2c20 6e70 2e6e 6461 7272 6179 2c20  er, np.ndarray, 
-00013520: 7872 2e44 6174 6141 7272 6179 2929 3a0a  xr.DataArray)):.
-00013530: 2020 2020 2020 2020 2020 2020 7365 7269              seri
-00013540: 6573 203d 2073 656c 662e 5f78 6120 3c3d  es = self._xa <=
-00013550: 206f 7468 6572 0a20 2020 2020 2020 2065   other.        e
-00013560: 6c69 6620 6973 696e 7374 616e 6365 286f  lif isinstance(o
-00013570: 7468 6572 2c20 5469 6d65 5365 7269 6573  ther, TimeSeries
-00013580: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-00013590: 6572 6965 7320 3d20 7365 6c66 2e5f 7861  eries = self._xa
-000135a0: 203c 3d20 6f74 6865 722e 6461 7461 5f61   <= other.data_a
-000135b0: 7272 6179 2863 6f70 793d 4661 6c73 6529  rray(copy=False)
-000135c0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-000135d0: 2020 2020 2020 2020 2020 2073 6572 6965             serie
-000135e0: 7320 3d20 4e6f 6e65 0a20 2020 2020 2020  s = None.       
-000135f0: 2020 2020 2072 6169 7365 5f6c 6f67 2854       raise_log(T
-00013600: 7970 6545 7272 6f72 2827 756e 7375 7070  ypeError('unsupp
-00013610: 6f72 7465 6420 6f70 6572 616e 6420 7479  orted operand ty
-00013620: 7065 2873 2920 666f 7220 3c20 3a20 5c27  pe(s) for < : \'
-00013630: 7b7d 5c27 2061 6e64 205c 277b 7d5c 272e  {}\' and \'{}\'.
-00013640: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-00013650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013660: 2020 2e66 6f72 6d61 7428 7479 7065 2873    .format(type(s
-00013670: 656c 6629 2e5f 5f6e 616d 655f 5f2c 2074  elf).__name__, t
-00013680: 7970 6528 6f74 6865 7229 2e5f 5f6e 616d  ype(other).__nam
-00013690: 655f 5f29 292c 206c 6f67 6765 7229 0a20  e__)), logger). 
-000136a0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000136b0: 7269 6573 2020 2320 4e6f 7465 3a20 7765  ries  # Note: we
-000136c0: 2072 6574 7572 6e20 6120 4461 7461 4172   return a DataAr
-000136d0: 7261 790a 0a20 2020 2064 6566 205f 5f67  ray..    def __g
-000136e0: 655f 5f28 7365 6c66 2c20 6f74 6865 7229  e__(self, other)
-000136f0: 202d 3e20 7872 2e44 6174 6141 7272 6179   -> xr.DataArray
-00013700: 3a0a 2020 2020 2020 2020 6966 2069 7369  :.        if isi
-00013710: 6e73 7461 6e63 6528 6f74 6865 722c 2028  nstance(other, (
-00013720: 696e 742c 2066 6c6f 6174 2c20 6e70 2e69  int, float, np.i
-00013730: 6e74 6567 6572 2c20 6e70 2e6e 6461 7272  nteger, np.ndarr
-00013740: 6179 2c20 7872 2e44 6174 6141 7272 6179  ay, xr.DataArray
-00013750: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-00013760: 7365 7269 6573 203d 2073 656c 662e 5f78  series = self._x
-00013770: 6120 3e3d 206f 7468 6572 0a20 2020 2020  a >= other.     
-00013780: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
-00013790: 6365 286f 7468 6572 2c20 5469 6d65 5365  ce(other, TimeSe
-000137a0: 7269 6573 293a 0a20 2020 2020 2020 2020  ries):.         
-000137b0: 2020 2073 6572 6965 7320 3d20 7365 6c66     series = self
-000137c0: 2e5f 7861 203e 3d20 6f74 6865 722e 6461  ._xa >= other.da
-000137d0: 7461 5f61 7272 6179 2863 6f70 793d 4661  ta_array(copy=Fa
-000137e0: 6c73 6529 0a20 2020 2020 2020 2065 6c73  lse).        els
-000137f0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00013800: 6572 6965 7320 3d20 4e6f 6e65 0a20 2020  eries = None.   
-00013810: 2020 2020 2020 2020 2072 6169 7365 5f6c           raise_l
-00013820: 6f67 2854 7970 6545 7272 6f72 2827 756e  og(TypeError('un
-00013830: 7375 7070 6f72 7465 6420 6f70 6572 616e  supported operan
-00013840: 6420 7479 7065 2873 2920 666f 7220 3c20  d type(s) for < 
-00013850: 3a20 5c27 7b7d 5c27 2061 6e64 205c 277b  : \'{}\' and \'{
-00013860: 7d5c 272e 270a 2020 2020 2020 2020 2020  }\'.'.          
-00013870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013880: 2020 2020 2020 2e66 6f72 6d61 7428 7479        .format(ty
-00013890: 7065 2873 656c 6629 2e5f 5f6e 616d 655f  pe(self).__name_
-000138a0: 5f2c 2074 7970 6528 6f74 6865 7229 2e5f  _, type(other)._
-000138b0: 5f6e 616d 655f 5f29 292c 206c 6f67 6765  _name__)), logge
-000138c0: 7229 0a20 2020 2020 2020 2072 6574 7572  r).        retur
-000138d0: 6e20 7365 7269 6573 2020 2320 4e6f 7465  n series  # Note
-000138e0: 3a20 7765 2072 6574 7572 6e20 6120 4461  : we return a Da
-000138f0: 7461 4172 7261 790a 0a20 2020 2064 6566  taArray..    def
-00013900: 205f 5f73 7472 5f5f 2873 656c 6629 3a0a   __str__(self):.
-00013910: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00013920: 7472 2873 656c 662e 5f78 6129 2e72 6570  tr(self._xa).rep
-00013930: 6c61 6365 2827 7861 7272 6179 2e44 6174  lace('xarray.Dat
-00013940: 6141 7272 6179 272c 2027 5469 6d65 5365  aArray', 'TimeSe
-00013950: 7269 6573 2028 4461 7461 4172 7261 7929  ries (DataArray)
-00013960: 2729 0a0a 2020 2020 6465 6620 5f5f 7265  ')..    def __re
-00013970: 7072 5f5f 2873 656c 6629 3a0a 2020 2020  pr__(self):.    
-00013980: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00013990: 5f78 612e 5f5f 7265 7072 5f5f 2829 2e72  _xa.__repr__().r
-000139a0: 6570 6c61 6365 2827 7861 7272 6179 2e44  eplace('xarray.D
-000139b0: 6174 6141 7272 6179 272c 2027 5469 6d65  ataArray', 'Time
-000139c0: 5365 7269 6573 2028 4461 7461 4172 7261  Series (DataArra
-000139d0: 7929 2729 0a0a 2020 2020 6465 6620 5f72  y)')..    def _r
-000139e0: 6570 725f 6874 6d6c 5f28 7365 6c66 293a  epr_html_(self):
-000139f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00013a00: 7365 6c66 2e5f 7861 2e5f 7265 7072 5f68  self._xa._repr_h
-00013a10: 746d 6c5f 2829 2e72 6570 6c61 6365 2827  tml_().replace('
-00013a20: 7861 7272 6179 2e44 6174 6141 7272 6179  xarray.DataArray
-00013a30: 272c 2027 5469 6d65 5365 7269 6573 2028  ', 'TimeSeries (
-00013a40: 4461 7461 4172 7261 7929 2729 0a0a 2020  DataArray)')..  
-00013a50: 2020 6465 6620 5f5f 636f 7079 5f5f 2873    def __copy__(s
-00013a60: 656c 662c 2064 6565 703a 2062 6f6f 6c20  elf, deep: bool 
-00013a70: 3d20 5472 7565 293a 0a20 2020 2020 2020  = True):.       
-00013a80: 2072 6574 7572 6e20 7365 6c66 2e63 6f70   return self.cop
-00013a90: 7928 290a 0a20 2020 2064 6566 205f 5f64  y()..    def __d
-00013aa0: 6565 7063 6f70 795f 5f28 7365 6c66 293a  eepcopy__(self):
-00013ab0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00013ac0: 5469 6d65 5365 7269 6573 2873 656c 662e  TimeSeries(self.
-00013ad0: 5f78 612e 636f 7079 2829 290a 0a20 2020  _xa.copy())..   
-00013ae0: 2064 6566 205f 5f67 6574 6974 656d 5f5f   def __getitem__
-00013af0: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
-00013b00: 2020 2020 2020 2020 2020 206b 6579 3a20             key: 
-00013b10: 556e 696f 6e5b 7064 2e44 6174 6574 696d  Union[pd.Datetim
-00013b20: 6549 6e64 6578 2c0a 2020 2020 2020 2020  eIndex,.        
-00013b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b40: 2020 2020 2020 2070 642e 5261 6e67 6549         pd.RangeI
-00013b50: 6e64 6578 2c0a 2020 2020 2020 2020 2020  ndex,.          
-00013b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b70: 2020 2020 204c 6973 745b 7374 725d 2c0a       List[str],.
-00013b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b90: 2020 2020 2020 2020 2020 2020 2020 204c                 L
-00013ba0: 6973 745b 696e 745d 2c0a 2020 2020 2020  ist[int],.      
-00013bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013bc0: 2020 2020 2020 2020 204c 6973 745b 7064           List[pd
-00013bd0: 2e54 696d 6573 7461 6d70 5d2c 0a20 2020  .Timestamp],.   
-00013be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013bf0: 2020 2020 2020 2020 2020 2020 7374 722c              str,
-00013c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c20: 696e 742c 0a20 2020 2020 2020 2020 2020  int,.           
-00013c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c40: 2020 2020 7064 2e54 696d 6573 7461 6d70      pd.Timestamp
-00013c50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00013c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c70: 2041 6e79 5d29 202d 3e20 2754 696d 6553   Any]) -> 'TimeS
-00013c80: 6572 6965 7327 3a0a 2020 2020 2020 2020  eries':.        
-00013c90: 2222 2241 6c6c 6f77 2069 6e64 6578 696e  """Allow indexin
-00013ca0: 6720 6f6e 2064 6172 7473 2054 696d 6553  g on darts TimeS
-00013cb0: 6572 6965 732e 0a0a 2020 2020 2020 2020  eries...        
-00013cc0: 5468 6520 7375 7070 6f72 7465 6420 696e  The supported in
-00013cd0: 6465 7820 7479 7065 7320 6172 6520 7468  dex types are th
-00013ce0: 6520 666f 6c6c 6f77 696e 6720 6261 7365  e following base
-00013cf0: 2074 7970 6573 2061 7320 6120 7369 6e67   types as a sing
-00013d00: 6c65 2076 616c 7565 2c20 6120 6c69 7374  le value, a list
-00013d10: 206f 7220 6120 736c 6963 653a 0a20 2020   or a slice:.   
-00013d20: 2020 2020 202d 2070 642e 5469 6d65 7374       - pd.Timest
-00013d30: 616d 7020 2d3e 2072 6574 7572 6e20 6120  amp -> return a 
-00013d40: 5469 6d65 5365 7269 6573 2063 6f72 7265  TimeSeries corre
-00013d50: 7370 6f6e 6469 6e67 2074 6f20 7468 6520  sponding to the 
-00013d60: 7661 6c75 6528 7329 2061 7420 7468 6520  value(s) at the 
-00013d70: 6769 7665 6e20 7469 6d65 7374 616d 7028  given timestamp(
-00013d80: 7329 2e0a 2020 2020 2020 2020 2d20 7374  s)..        - st
-00013d90: 7220 2d3e 2072 6574 7572 6e20 6120 5469  r -> return a Ti
-00013da0: 6d65 5365 7269 6573 2069 6e63 6c75 6469  meSeries includi
-00013db0: 6e67 2074 6865 2063 6f6c 756d 6e28 7329  ng the column(s)
-00013dc0: 2028 636f 6d70 6f6e 656e 7473 2920 7370   (components) sp
-00013dd0: 6563 6966 6965 6420 6173 2073 7472 2e0a  ecified as str..
-00013de0: 2020 2020 2020 2020 2d20 696e 7420 2d3e          - int ->
-00013df0: 2072 6574 7572 6e20 6120 5469 6d65 5365   return a TimeSe
-00013e00: 7269 6573 2077 6974 6820 7468 6520 7661  ries with the va
-00013e10: 6c75 6528 7329 2061 7420 7468 6520 6769  lue(s) at the gi
-00013e20: 7665 6e20 726f 7720 2874 696d 6529 2069  ven row (time) i
-00013e30: 6e64 6578 2e0a 0a20 2020 2020 2020 2060  ndex...        `
-00013e40: 7064 2e44 6174 6574 696d 6549 6e64 6578  pd.DatetimeIndex
-00013e50: 6020 616e 6420 6070 642e 5261 6e67 6549  ` and `pd.RangeI
-00013e60: 6e64 6578 6020 6172 6520 616c 736f 2073  ndex` are also s
-00013e70: 7570 706f 7274 6564 2061 6e64 2077 696c  upported and wil
-00013e80: 6c20 7265 7475 726e 2074 6865 2063 6f72  l return the cor
-00013e90: 7265 7370 6f6e 6469 6e67 2076 616c 7565  responding value
-00013ea0: 2873 290a 2020 2020 2020 2020 6174 2074  (s).        at t
-00013eb0: 6865 2070 726f 7669 6465 6420 7469 6d65  he provided time
-00013ec0: 2069 6e64 6963 6573 2e0a 0a20 2020 2020   indices...     
-00013ed0: 2020 202e 2e20 7761 726e 696e 673a 3a0a     .. warning::.
-00013ee0: 2020 2020 2020 2020 2020 2020 736c 6963              slic
-00013ef0: 6573 2075 7365 2070 616e 6461 7320 636f  es use pandas co
-00013f00: 6e76 656e 7469 6f6e 206f 6620 696e 636c  nvention of incl
-00013f10: 7564 696e 6720 626f 7468 2065 6e64 7320  uding both ends 
-00013f20: 6f66 2074 6865 2073 6c69 6365 2e0a 2020  of the slice..  
-00013f30: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00013f40: 2020 6465 6620 5f63 6865 636b 5f64 7428    def _check_dt(
-00013f50: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-00013f60: 6169 7365 5f69 665f 6e6f 7428 7365 6c66  aise_if_not(self
-00013f70: 2e5f 6861 735f 6461 7465 7469 6d65 5f69  ._has_datetime_i
-00013f80: 6e64 6578 2c20 2741 7474 656d 7074 6564  ndex, 'Attempted
-00013f90: 2069 6e64 6578 696e 6720 6120 7365 7269   indexing a seri
-00013fa0: 6573 2077 6974 6820 6120 4461 7465 7469  es with a Dateti
-00013fb0: 6d65 496e 6465 7820 6f72 2061 2074 696d  meIndex or a tim
-00013fc0: 6573 7461 6d70 2c20 270a 2020 2020 2020  estamp, '.      
-00013fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ff0: 2020 2020 2020 2020 2020 2020 2027 6275               'bu
-00014000: 7420 7468 6520 7365 7269 6573 2075 7365  t the series use
-00014010: 7320 6120 5261 6e67 6549 6e64 6578 2e27  s a RangeIndex.'
-00014020: 2c20 6c6f 6767 6572 290a 0a20 2020 2020  , logger)..     
-00014030: 2020 2064 6566 205f 6368 6563 6b5f 7261     def _check_ra
-00014040: 6e67 6528 293a 0a20 2020 2020 2020 2020  nge():.         
-00014050: 2020 2072 6169 7365 5f69 6628 7365 6c66     raise_if(self
-00014060: 2e5f 6861 735f 6461 7465 7469 6d65 5f69  ._has_datetime_i
-00014070: 6e64 6578 2c20 2741 7474 656d 7074 6564  ndex, 'Attempted
-00014080: 2069 6e64 6578 696e 6720 6120 7365 7269   indexing a seri
-00014090: 6573 2077 6974 6820 6120 5261 6e67 6549  es with a RangeI
-000140a0: 6e64 6578 2c20 270a 2020 2020 2020 2020  ndex, '.        
-000140b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140d0: 2020 2020 2020 2027 6275 7420 7468 6520         'but the 
-000140e0: 7365 7269 6573 2075 7365 7320 6120 4461  series uses a Da
-000140f0: 7465 7469 6d65 496e 6465 782e 272c 206c  tetimeIndex.', l
-00014100: 6f67 6765 7229 0a0a 2020 2020 2020 2020  ogger)..        
-00014110: 6465 6620 5f73 6574 5f66 7265 715f 696e  def _set_freq_in
-00014120: 5f78 6128 7861 5f3a 2078 722e 4461 7461  _xa(xa_: xr.Data
-00014130: 4172 7261 7929 3a0a 2020 2020 2020 2020  Array):.        
-00014140: 2020 2020 2320 6d75 7461 7465 7320 7468      # mutates th
-00014150: 6520 4461 7461 4172 7261 7920 746f 206d  e DataArray to m
-00014160: 616b 6520 7375 7265 2069 7420 636f 6e74  ake sure it cont
-00014170: 6169 6e73 2074 6865 2066 7265 710a 2020  ains the freq.  
-00014180: 2020 2020 2020 2020 2020 696e 6665 7272            inferr
-00014190: 6564 5f66 7265 7120 3d20 7861 5f2e 6765  ed_freq = xa_.ge
-000141a0: 745f 696e 6465 7828 7365 6c66 2e5f 7469  t_index(self._ti
-000141b0: 6d65 5f64 696d 292e 696e 6665 7272 6564  me_dim).inferred
-000141c0: 5f66 7265 710a 2020 2020 2020 2020 2020  _freq.          
-000141d0: 2020 6966 2069 6e66 6572 7265 645f 6672    if inferred_fr
-000141e0: 6571 2069 7320 6e6f 7420 4e6f 6e65 3a0a  eq is not None:.
-000141f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014200: 7861 5f2e 6765 745f 696e 6465 7828 7365  xa_.get_index(se
-00014210: 6c66 2e5f 7469 6d65 5f64 696d 292e 6672  lf._time_dim).fr
-00014220: 6571 203d 2074 6f5f 6f66 6673 6574 2869  eq = to_offset(i
-00014230: 6e66 6572 7265 645f 6672 6571 290a 2020  nferred_freq).  
-00014240: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00014250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014260: 7861 5f2e 6765 745f 696e 6465 7828 7365  xa_.get_index(se
-00014270: 6c66 2e5f 7469 6d65 5f64 696d 292e 6672  lf._time_dim).fr
-00014280: 6571 203d 2073 656c 662e 5f66 7265 710a  eq = self._freq.
-00014290: 0a20 2020 2020 2020 2023 2068 616e 646c  .        # handl
-000142a0: 6520 4461 7465 7469 6d65 496e 6465 7820  e DatetimeIndex 
-000142b0: 616e 6420 5261 6e67 6549 6e64 6578 3a0a  and RangeIndex:.
-000142c0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-000142d0: 7461 6e63 6528 6b65 792c 2070 642e 4461  tance(key, pd.Da
-000142e0: 7465 7469 6d65 496e 6465 7829 3a0a 2020  tetimeIndex):.  
-000142f0: 2020 2020 2020 2020 2020 5f63 6865 636b            _check
-00014300: 5f64 7428 290a 2020 2020 2020 2020 2020  _dt().          
-00014310: 2020 7861 5f20 3d20 7365 6c66 2e5f 7861    xa_ = self._xa
-00014320: 2e73 656c 287b 7365 6c66 2e5f 7469 6d65  .sel({self._time
-00014330: 5f64 696d 3a20 6b65 797d 290a 0a20 2020  _dim: key})..   
-00014340: 2020 2020 2020 2020 2023 2069 6e64 6578           # index
-00014350: 696e 6720 6d61 7920 6469 7363 6172 6420  ing may discard 
-00014360: 7468 6520 6672 6571 2073 6f20 7765 2072  the freq so we r
-00014370: 6573 746f 7265 2069 742e 2e2e 0a20 2020  estore it....   
-00014380: 2020 2020 2020 2020 2023 2054 4f44 4f3a           # TODO:
-00014390: 2075 6e69 742d 7465 7374 2074 6869 730a   unit-test this.
-000143a0: 2020 2020 2020 2020 2020 2020 5f73 6574              _set
-000143b0: 5f66 7265 715f 696e 5f78 6128 7861 5f29  _freq_in_xa(xa_)
-000143c0: 0a0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-000143d0: 7475 726e 2054 696d 6553 6572 6965 7328  turn TimeSeries(
-000143e0: 7861 5f29 0a20 2020 2020 2020 2065 6c69  xa_).        eli
-000143f0: 6620 6973 696e 7374 616e 6365 286b 6579  f isinstance(key
-00014400: 2c20 7064 2e52 616e 6765 496e 6465 7829  , pd.RangeIndex)
-00014410: 3a0a 2020 2020 2020 2020 2020 2020 5f63  :.            _c
-00014420: 6865 636b 5f72 616e 6765 2829 0a20 2020  heck_range().   
-00014430: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00014440: 5469 6d65 5365 7269 6573 2873 656c 662e  TimeSeries(self.
-00014450: 5f78 612e 7365 6c28 7b73 656c 662e 5f74  _xa.sel({self._t
-00014460: 696d 655f 6469 6d3a 206b 6579 7d29 290a  ime_dim: key})).
-00014470: 0a20 2020 2020 2020 2023 2068 616e 646c  .        # handl
-00014480: 6520 736c 6963 6573 3a0a 2020 2020 2020  e slices:.      
-00014490: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
-000144a0: 6528 6b65 792c 2073 6c69 6365 293a 0a20  e(key, slice):. 
-000144b0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-000144c0: 696e 7374 616e 6365 286b 6579 2e73 7461  instance(key.sta
-000144d0: 7274 2c20 7374 7229 206f 7220 6973 696e  rt, str) or isin
-000144e0: 7374 616e 6365 286b 6579 2e73 746f 702c  stance(key.stop,
-000144f0: 2073 7472 293a 0a20 2020 2020 2020 2020   str):.         
-00014500: 2020 2020 2020 2072 6574 7572 6e20 5469         return Ti
-00014510: 6d65 5365 7269 6573 2873 656c 662e 5f78  meSeries(self._x
-00014520: 612e 7365 6c28 7b44 494d 535b 315d 3a20  a.sel({DIMS[1]: 
-00014530: 6b65 797d 2929 0a20 2020 2020 2020 2020  key})).         
-00014540: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
-00014550: 6365 286b 6579 2e73 7461 7274 2c20 696e  ce(key.start, in
-00014560: 7429 206f 7220 6973 696e 7374 616e 6365  t) or isinstance
-00014570: 286b 6579 2e73 746f 702c 2069 6e74 293a  (key.stop, int):
-00014580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014590: 2072 6574 7572 6e20 5469 6d65 5365 7269   return TimeSeri
-000145a0: 6573 2873 656c 662e 5f78 612e 6973 656c  es(self._xa.isel
-000145b0: 287b 7365 6c66 2e5f 7469 6d65 5f64 696d  ({self._time_dim
-000145c0: 3a20 6b65 797d 2929 0a20 2020 2020 2020  : key})).       
-000145d0: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
-000145e0: 616e 6365 286b 6579 2e73 7461 7274 2c20  ance(key.start, 
-000145f0: 7064 2e54 696d 6573 7461 6d70 2920 6f72  pd.Timestamp) or
-00014600: 2069 7369 6e73 7461 6e63 6528 6b65 792e   isinstance(key.
-00014610: 7374 6f70 2c20 7064 2e54 696d 6573 7461  stop, pd.Timesta
-00014620: 6d70 293a 0a20 2020 2020 2020 2020 2020  mp):.           
-00014630: 2020 2020 205f 6368 6563 6b5f 6474 2829       _check_dt()
-00014640: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014650: 2020 2320 696e 6465 7869 6e67 206d 6179    # indexing may
-00014660: 2064 6973 6361 7264 2074 6865 2066 7265   discard the fre
-00014670: 7120 736f 2077 6520 7265 7374 6f72 6520  q so we restore 
-00014680: 6974 2e2e 2e0a 2020 2020 2020 2020 2020  it....          
-00014690: 2020 2020 2020 7861 5f20 3d20 7365 6c66        xa_ = self
-000146a0: 2e5f 7861 2e73 656c 287b 7365 6c66 2e5f  ._xa.sel({self._
-000146b0: 7469 6d65 5f64 696d 3a20 6b65 797d 290a  time_dim: key}).
-000146c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146d0: 5f73 6574 5f66 7265 715f 696e 5f78 6128  _set_freq_in_xa(
-000146e0: 7861 5f29 0a20 2020 2020 2020 2020 2020  xa_).           
-000146f0: 2020 2020 2072 6574 7572 6e20 5469 6d65       return Time
-00014700: 5365 7269 6573 2878 615f 290a 0a20 2020  Series(xa_)..   
-00014710: 2020 2020 2023 2068 616e 646c 6520 7369       # handle si
-00014720: 6d70 6c65 2074 7970 6573 3a0a 2020 2020  mple types:.    
-00014730: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
-00014740: 6e63 6528 6b65 792c 2073 7472 293a 0a20  nce(key, str):. 
-00014750: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00014760: 6e20 5469 6d65 5365 7269 6573 2873 656c  n TimeSeries(sel
-00014770: 662e 5f78 612e 7365 6c28 7b44 494d 535b  f._xa.sel({DIMS[
-00014780: 315d 3a20 5b6b 6579 5d7d 2929 2020 2320  1]: [key]}))  # 
-00014790: 6861 7665 2074 6f20 7075 7420 6b65 7920  have to put key 
-000147a0: 696e 2061 206c 6973 7420 6e6f 7420 746f  in a list not to
-000147b0: 2064 726f 7020 7468 6520 6469 6d65 6e73   drop the dimens
-000147c0: 696f 6e0a 2020 2020 2020 2020 656c 6966  ion.        elif
-000147d0: 2069 7369 6e73 7461 6e63 6528 6b65 792c   isinstance(key,
-000147e0: 2069 6e74 293a 0a20 2020 2020 2020 2020   int):.         
-000147f0: 2020 2072 6574 7572 6e20 5469 6d65 5365     return TimeSe
-00014800: 7269 6573 2873 656c 662e 5f78 612e 6973  ries(self._xa.is
-00014810: 656c 287b 7365 6c66 2e5f 7469 6d65 5f64  el({self._time_d
-00014820: 696d 3a20 5b6b 6579 5d7d 2929 0a20 2020  im: [key]})).   
-00014830: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
-00014840: 616e 6365 286b 6579 2c20 7064 2e54 696d  ance(key, pd.Tim
-00014850: 6573 7461 6d70 293a 0a20 2020 2020 2020  estamp):.       
-00014860: 2020 2020 205f 6368 6563 6b5f 6474 2829       _check_dt()
-00014870: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00014880: 696e 6465 7869 6e67 206d 6179 2064 6973  indexing may dis
-00014890: 6361 7264 2074 6865 2066 7265 7120 736f  card the freq so
-000148a0: 2077 6520 7265 7374 6f72 6520 6974 2e2e   we restore it..
-000148b0: 2e0a 2020 2020 2020 2020 2020 2020 7861  ..            xa
-000148c0: 5f20 3d20 7365 6c66 2e5f 7861 2e73 656c  _ = self._xa.sel
-000148d0: 287b 7365 6c66 2e5f 7469 6d65 5f64 696d  ({self._time_dim
-000148e0: 3a20 5b6b 6579 5d7d 290a 2020 2020 2020  : [key]}).      
-000148f0: 2020 2020 2020 5f73 6574 5f66 7265 715f        _set_freq_
-00014900: 696e 5f78 6128 7861 5f29 0a20 2020 2020  in_xa(xa_).     
-00014910: 2020 2020 2020 2072 6574 7572 6e20 5469         return Ti
-00014920: 6d65 5365 7269 6573 2878 615f 290a 0a20  meSeries(xa_).. 
-00014930: 2020 2020 2020 2023 2068 616e 646c 6520         # handle 
-00014940: 6c69 7374 733a 0a20 2020 2020 2020 2069  lists:.        i
-00014950: 6620 6973 696e 7374 616e 6365 286b 6579  f isinstance(key
-00014960: 2c20 6c69 7374 293a 0a20 2020 2020 2020  , list):.       
-00014970: 2020 2020 2069 6620 616c 6c28 6973 696e       if all(isin
-00014980: 7374 616e 6365 2873 2c20 7374 7229 2066  stance(s, str) f
-00014990: 6f72 2073 2069 6e20 6b65 7929 3a0a 2020  or s in key):.  
-000149a0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000149b0: 7768 656e 2073 7472 696e 6728 7329 2061  when string(s) a
-000149c0: 7265 2070 726f 7669 6465 642c 2077 6520  re provided, we 
-000149d0: 636f 6e73 6964 6572 2069 7420 6173 2028  consider it as (
-000149e0: 6120 6c69 7374 206f 6629 2063 6f6d 706f  a list of) compo
-000149f0: 6e65 6e74 2873 290a 2020 2020 2020 2020  nent(s).        
-00014a00: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-00014a10: 696d 6553 6572 6965 7328 7365 6c66 2e5f  imeSeries(self._
-00014a20: 7861 2e73 656c 287b 4449 4d53 5b31 5d3a  xa.sel({DIMS[1]:
-00014a30: 206b 6579 7d29 290a 2020 2020 2020 2020   key})).        
-00014a40: 2020 2020 656c 6966 2061 6c6c 2869 7369      elif all(isi
-00014a50: 6e73 7461 6e63 6528 692c 2069 6e74 2920  nstance(i, int) 
-00014a60: 666f 7220 6920 696e 206b 6579 293a 0a20  for i in key):. 
-00014a70: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00014a80: 6574 7572 6e20 5469 6d65 5365 7269 6573  eturn TimeSeries
-00014a90: 2873 656c 662e 5f78 612e 6973 656c 287b  (self._xa.isel({
-00014aa0: 7365 6c66 2e5f 7469 6d65 5f64 696d 3a20  self._time_dim: 
-00014ab0: 6b65 797d 2929 0a20 2020 2020 2020 2020  key})).         
-00014ac0: 2020 2065 6c69 6620 616c 6c28 6973 696e     elif all(isin
-00014ad0: 7374 616e 6365 2874 2c20 7064 2e54 696d  stance(t, pd.Tim
-00014ae0: 6573 7461 6d70 2920 666f 7220 7420 696e  estamp) for t in
-00014af0: 206b 6579 293a 0a20 2020 2020 2020 2020   key):.         
-00014b00: 2020 2020 2020 205f 6368 6563 6b5f 6474         _check_dt
-00014b10: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
-00014b20: 2020 2020 2320 696e 6465 7869 6e67 206d      # indexing m
-00014b30: 6179 2064 6973 6361 7264 2074 6865 2066  ay discard the f
-00014b40: 7265 7120 736f 2077 6520 7265 7374 6f72  req so we restor
-00014b50: 6520 6974 2e2e 2e0a 2020 2020 2020 2020  e it....        
-00014b60: 2020 2020 2020 2020 7861 5f20 3d20 7365          xa_ = se
-00014b70: 6c66 2e5f 7861 2e73 656c 287b 7365 6c66  lf._xa.sel({self
-00014b80: 2e5f 7469 6d65 5f64 696d 3a20 6b65 797d  ._time_dim: key}
-00014b90: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00014ba0: 2020 5f73 6574 5f66 7265 715f 696e 5f78    _set_freq_in_x
-00014bb0: 6128 7861 5f29 0a20 2020 2020 2020 2020  a(xa_).         
-00014bc0: 2020 2020 2020 2072 6574 7572 6e20 5469         return Ti
-00014bd0: 6d65 5365 7269 6573 2878 615f 290a 0a20  meSeries(xa_).. 
-00014be0: 2020 2020 2020 2072 6169 7365 5f6c 6f67         raise_log
-00014bf0: 2849 6e64 6578 4572 726f 7228 2254 6865  (IndexError("The
-00014c00: 2074 7970 6520 6f66 2079 6f75 7220 696e   type of your in
-00014c10: 6465 7820 7761 7320 6e6f 7420 6d61 7463  dex was not matc
-00014c20: 6865 642e 2229 2c20 6c6f 6767 6572 290a  hed."), logger).
+0000eae0: 2222 0a20 2020 2020 2020 2055 7064 6174  "".        Updat
+0000eaf0: 6573 2074 6865 2054 696d 6553 6572 6965  es the TimeSerie
+0000eb00: 7320 7769 7468 2074 6865 206e 6577 2076  s with the new v
+0000eb10: 616c 7565 7320 7072 6f76 6964 6564 2e0a  alues provided..
+0000eb20: 2020 2020 2020 2020 4966 2069 6e64 6963          If indic
+0000eb30: 6573 2061 7265 206e 6f74 2069 6e20 6f72  es are not in or
+0000eb40: 6967 696e 616c 2054 696d 6553 6572 6965  iginal TimeSerie
+0000eb50: 732c 2074 6865 7920 7769 6c6c 2062 6520  s, they will be 
+0000eb60: 6469 7363 6172 6465 642e 0a20 2020 2020  discarded..     
+0000eb70: 2020 2055 7365 2060 6e75 6d70 792e 6e61     Use `numpy.na
+0000eb80: 6e60 2074 6f20 6967 6e6f 7265 2061 2073  n` to ignore a s
+0000eb90: 7065 6369 6669 6320 696e 6465 7820 696e  pecific index in
+0000eba0: 2061 2073 6572 6965 732e 0a0a 2020 2020   a series...    
+0000ebb0: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+0000ebc0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+0000ebd0: 2d0a 2020 2020 2020 2020 696e 6465 780a  -.        index.
+0000ebe0: 2020 2020 2020 2020 2020 2020 4120 6070              A `p
+0000ebf0: 616e 6461 732e 4461 7465 5469 6d65 496e  andas.DateTimeIn
+0000ec00: 6465 7860 2063 6f6e 7461 696e 696e 6720  dex` containing 
+0000ec10: 7468 6520 696e 6469 6365 7320 746f 2072  the indices to r
+0000ec20: 6570 6c61 6365 2e0a 2020 2020 2020 2020  eplace..        
+0000ec30: 7661 6c75 6573 0a20 2020 2020 2020 2020  values.         
+0000ec40: 2020 2041 6e20 6172 7261 7920 636f 6e74     An array cont
+0000ec50: 6169 6e69 6e67 2074 6865 2076 616c 7565  aining the value
+0000ec60: 7320 746f 2072 6570 6c61 6365 2028 6f70  s to replace (op
+0000ec70: 7469 6f6e 616c 292e 0a0a 2020 2020 2020  tional)...      
+0000ec80: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+0000ec90: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+0000eca0: 2020 5469 6d65 5365 7269 6573 0a20 2020    TimeSeries.   
+0000ecb0: 2020 2020 2020 2020 2041 206e 6577 2054           A new T
+0000ecc0: 696d 6553 6572 6965 7320 7769 7468 2075  imeSeries with u
+0000ecd0: 7064 6174 6564 2076 616c 7565 732e 0a20  pdated values.. 
+0000ece0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000ecf0: 2020 2023 2054 4f44 4f3a 2049 2064 6f6e     # TODO: I don
+0000ed00: 2774 2074 6869 6e6b 2074 6869 7320 6973  't think this is
+0000ed10: 206e 6565 6465 642e 2e2e 2070 726f 6261   needed... proba
+0000ed20: 626c 7920 6265 7474 6572 2074 6f20 6a75  bly better to ju
+0000ed30: 7374 2063 7265 6174 6520 6120 6e65 7720  st create a new 
+0000ed40: 5469 6d65 5365 7269 6573 0a20 2020 2020  TimeSeries.     
+0000ed50: 2020 2072 6169 7365 204e 6f74 496d 706c     raise NotImpl
+0000ed60: 656d 656e 7465 6445 7272 6f72 2827 5469  ementedError('Ti
+0000ed70: 6d65 5365 7269 6573 2e75 7064 6174 6528  meSeries.update(
+0000ed80: 2920 6973 206e 6f74 2073 7570 706f 7274  ) is not support
+0000ed90: 6564 2061 6e79 6d6f 7265 2e27 290a 0a20  ed anymore.').. 
+0000eda0: 2020 2064 6566 2073 7461 636b 2873 656c     def stack(sel
+0000edb0: 662c 206f 7468 6572 3a20 2754 696d 6553  f, other: 'TimeS
+0000edc0: 6572 6965 7327 2920 2d3e 2027 5469 6d65  eries') -> 'Time
+0000edd0: 5365 7269 6573 273a 0a20 2020 2020 2020  Series':.       
+0000ede0: 2022 2222 0a20 2020 2020 2020 2053 7461   """.        Sta
+0000edf0: 636b 7320 616e 6f74 6865 7220 756e 6976  cks another univ
+0000ee00: 6172 6961 7465 206f 7220 6d75 6c74 6976  ariate or multiv
+0000ee10: 6172 6961 7465 2054 696d 6553 6572 6965  ariate TimeSerie
+0000ee20: 7320 7769 7468 2074 6865 2073 616d 6520  s with the same 
+0000ee30: 7469 6d65 2069 6e64 6578 206f 6e20 746f  time index on to
+0000ee40: 7020 6f66 0a20 2020 2020 2020 2074 6865  p of.        the
+0000ee50: 2063 7572 7265 6e74 206f 6e65 2028 616c   current one (al
+0000ee60: 6f6e 6720 7468 6520 636f 6d70 6f6e 656e  ong the componen
+0000ee70: 7420 6178 6973 292c 2061 6e64 2072 6574  t axis), and ret
+0000ee80: 7572 6e73 2074 6865 206e 6577 6c79 2066  urns the newly f
+0000ee90: 6f72 6d65 6420 6d75 6c74 6976 6172 6961  ormed multivaria
+0000eea0: 7465 2054 696d 6553 6572 6965 7320 7468  te TimeSeries th
+0000eeb0: 6174 2069 6e63 6c75 6465 730a 2020 2020  at includes.    
+0000eec0: 2020 2020 616c 6c20 7468 6520 636f 6d70      all the comp
+0000eed0: 6f6e 656e 7473 206f 6620 6073 656c 6660  onents of `self`
+0000eee0: 2061 6e64 206f 6620 606f 7468 6572 602e   and of `other`.
+0000eef0: 0a0a 2020 2020 2020 2020 5468 6520 7265  ..        The re
+0000ef00: 7375 6c74 696e 6720 5469 6d65 5365 7269  sulting TimeSeri
+0000ef10: 6573 2077 696c 6c20 6861 7665 2074 6865  es will have the
+0000ef20: 2073 616d 6520 6e61 6d65 2066 6f72 2069   same name for i
+0000ef30: 7473 2074 696d 6520 6469 6d65 6e73 696f  ts time dimensio
+0000ef40: 6e20 6173 2074 6869 7320 5469 6d65 5365  n as this TimeSe
+0000ef50: 7269 6573 2c20 616e 6420 7468 650a 2020  ries, and the.  
+0000ef60: 2020 2020 2020 7361 6d65 206e 756d 6265        same numbe
+0000ef70: 7220 6f66 2073 616d 706c 6573 2e0a 0a20  r of samples... 
+0000ef80: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+0000ef90: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0000efa0: 2d2d 2d2d 0a20 2020 2020 2020 206f 7468  ----.        oth
+0000efb0: 6572 0a20 2020 2020 2020 2020 2020 2041  er.            A
+0000efc0: 2054 696d 6553 6572 6965 7320 696e 7374   TimeSeries inst
+0000efd0: 616e 6365 2077 6974 6820 7468 6520 7361  ance with the sa
+0000efe0: 6d65 2069 6e64 6578 2061 6e64 2074 6865  me index and the
+0000eff0: 2073 616d 6520 6e75 6d62 6572 206f 6620   same number of 
+0000f000: 7361 6d70 6c65 7320 6173 2074 6865 2063  samples as the c
+0000f010: 7572 7265 6e74 206f 6e65 2e0a 0a20 2020  urrent one...   
+0000f020: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+0000f030: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+0000f040: 2020 2020 2054 696d 6553 6572 6965 730a       TimeSeries.
+0000f050: 2020 2020 2020 2020 2020 2020 4120 6e65              A ne
+0000f060: 7720 6d75 6c74 6976 6172 6961 7465 2054  w multivariate T
+0000f070: 696d 6553 6572 6965 7320 696e 7374 616e  imeSeries instan
+0000f080: 6365 2e0a 2020 2020 2020 2020 2222 220a  ce..        """.
+0000f090: 2020 2020 2020 2020 7261 6973 655f 6966          raise_if
+0000f0a0: 5f6e 6f74 2873 656c 662e 6861 735f 7361  _not(self.has_sa
+0000f0b0: 6d65 5f74 696d 655f 6173 286f 7468 6572  me_time_as(other
+0000f0c0: 292c 2027 5468 6520 696e 6469 6365 7320  ), 'The indices 
+0000f0d0: 6f66 2074 6865 2074 776f 2054 696d 6553  of the two TimeS
+0000f0e0: 6572 6965 7320 696e 7374 616e 6365 7320  eries instances 
+0000f0f0: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+0000f100: 2020 2020 2020 2027 6d75 7374 2062 6520         'must be 
+0000f110: 6571 7561 6c27 2c20 6c6f 6767 6572 290a  equal', logger).
+0000f120: 2020 2020 2020 2020 7261 6973 655f 6966          raise_if
+0000f130: 5f6e 6f74 2873 656c 662e 6e5f 7361 6d70  _not(self.n_samp
+0000f140: 6c65 7320 3d3d 206f 7468 6572 2e6e 5f73  les == other.n_s
+0000f150: 616d 706c 6573 2c20 2754 776f 2073 6572  amples, 'Two ser
+0000f160: 6965 7320 6361 6e20 6265 2073 7461 636b  ies can be stack
+0000f170: 6564 206f 6e6c 7920 6966 2074 6865 7920  ed only if they 
+0000f180: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+0000f190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f1b0: 2020 2020 2020 2020 2020 2768 6176 6520            'have 
+0000f1c0: 7468 6520 7361 6d65 206e 756d 6265 7220  the same number 
+0000f1d0: 6f66 2073 616d 706c 6573 2e27 2c20 6c6f  of samples.', lo
+0000f1e0: 6767 6572 290a 0a20 2020 2020 2020 206f  gger)..        o
+0000f1f0: 7468 6572 5f78 6120 3d20 6f74 6865 722e  ther_xa = other.
+0000f200: 6461 7461 5f61 7272 6179 2863 6f70 793d  data_array(copy=
+0000f210: 4661 6c73 6529 0a20 2020 2020 2020 2069  False).        i
+0000f220: 6620 6f74 6865 725f 7861 2e64 696d 735b  f other_xa.dims[
+0000f230: 305d 2021 3d20 7365 6c66 2e5f 7469 6d65  0] != self._time
+0000f240: 5f64 696d 3a0a 2020 2020 2020 2020 2020  _dim:.          
+0000f250: 2020 6e65 775f 6f74 6865 725f 7861 203d    new_other_xa =
+0000f260: 2078 722e 4461 7461 4172 7261 7928 6f74   xr.DataArray(ot
+0000f270: 6865 725f 7861 2e76 616c 7565 732c 0a20  her_xa.values,. 
+0000f280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f2a0: 2020 2020 2020 2064 696d 733d 7365 6c66         dims=self
+0000f2b0: 2e5f 7861 2e64 696d 732c 0a20 2020 2020  ._xa.dims,.     
+0000f2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f2e0: 2020 2063 6f6f 7264 733d 7b73 656c 662e     coords={self.
+0000f2f0: 5f74 696d 655f 6469 6d3a 2073 656c 662e  _time_dim: self.
+0000f300: 5f74 696d 655f 696e 6465 782c 2044 494d  _time_index, DIM
+0000f310: 535b 315d 3a20 6f74 6865 722e 636f 6d70  S[1]: other.comp
+0000f320: 6f6e 656e 7473 7d29 0a20 2020 2020 2020  onents}).       
+0000f330: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000f340: 2020 206e 6577 5f6f 7468 6572 5f78 6120     new_other_xa 
+0000f350: 3d20 6f74 6865 725f 7861 0a0a 2020 2020  = other_xa..    
+0000f360: 2020 2020 6e65 775f 7861 203d 2078 722e      new_xa = xr.
+0000f370: 636f 6e63 6174 2828 7365 6c66 2e5f 7861  concat((self._xa
+0000f380: 2c20 6e65 775f 6f74 6865 725f 7861 292c  , new_other_xa),
+0000f390: 2064 696d 3d44 494d 535b 315d 290a 0a20   dim=DIMS[1]).. 
+0000f3a0: 2020 2020 2020 2023 2077 6520 6361 6c6c         # we call
+0000f3b0: 2074 6865 2066 6163 746f 7279 206d 6574   the factory met
+0000f3c0: 686f 6420 6865 7265 2074 6f20 6469 7361  hod here to disa
+0000f3d0: 6d62 6967 7561 7465 2063 6f6c 756d 6e20  mbiguate column 
+0000f3e0: 6e61 6d65 7320 6966 206e 6565 6465 642e  names if needed.
+0000f3f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000f400: 5469 6d65 5365 7269 6573 2e66 726f 6d5f  TimeSeries.from_
+0000f410: 7861 7272 6179 286e 6577 5f78 612c 2066  xarray(new_xa, f
+0000f420: 696c 6c5f 6d69 7373 696e 675f 6461 7465  ill_missing_date
+0000f430: 733d 4661 6c73 6529 0a0a 2020 2020 6465  s=False)..    de
+0000f440: 6620 756e 6976 6172 6961 7465 5f63 6f6d  f univariate_com
+0000f450: 706f 6e65 6e74 2873 656c 662c 2069 6e64  ponent(self, ind
+0000f460: 6578 3a20 556e 696f 6e5b 7374 722c 2069  ex: Union[str, i
+0000f470: 6e74 5d29 202d 3e20 2754 696d 6553 6572  nt]) -> 'TimeSer
+0000f480: 6965 7327 3a0a 2020 2020 2020 2020 2222  ies':.        ""
+0000f490: 220a 2020 2020 2020 2020 5265 7472 6965  ".        Retrie
+0000f4a0: 7665 7320 6f6e 6520 6f66 2074 6865 2063  ves one of the c
+0000f4b0: 6f6d 706f 6e65 6e74 7320 6f66 2074 6865  omponents of the
+0000f4c0: 2063 7572 7265 6e74 2054 696d 6553 6572   current TimeSer
+0000f4d0: 6965 7320 696e 7374 616e 6365 0a20 2020  ies instance.   
+0000f4e0: 2020 2020 2061 6e64 2072 6574 7572 6e73       and returns
+0000f4f0: 2069 7420 6173 206e 6577 2075 6e69 7661   it as new univa
+0000f500: 7269 6174 6520 5469 6d65 5365 7269 6573  riate TimeSeries
+0000f510: 2069 6e73 7461 6e63 652e 0a0a 2020 2020   instance...    
+0000f520: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+0000f530: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+0000f540: 2d0a 2020 2020 2020 2020 696e 6465 780a  -.        index.
+0000f550: 2020 2020 2020 2020 2020 2020 416e 207a              An z
+0000f560: 6572 6f2d 696e 6465 7865 6420 696e 7465  ero-indexed inte
+0000f570: 6765 7220 696e 6469 6361 7469 6e67 2077  ger indicating w
+0000f580: 6869 6368 2063 6f6d 706f 6e65 6e74 2074  hich component t
+0000f590: 6f20 7265 7472 6965 7665 2e20 4966 2063  o retrieve. If c
+0000f5a0: 6f6d 706f 6e65 6e74 7320 6861 7665 206e  omponents have n
+0000f5b0: 616d 6573 2c0a 2020 2020 2020 2020 2020  ames,.          
+0000f5c0: 2020 7468 6973 2063 616e 2062 6520 6120    this can be a 
+0000f5d0: 7374 7269 6e67 2077 6974 6820 7468 6520  string with the 
+0000f5e0: 636f 6d70 6f6e 656e 7427 7320 6e61 6d65  component's name
+0000f5f0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+0000f600: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+0000f610: 2d2d 0a20 2020 2020 2020 2054 696d 6553  --.        TimeS
+0000f620: 6572 6965 730a 2020 2020 2020 2020 2020  eries.          
+0000f630: 2020 4120 6e65 7720 756e 6976 6172 6961    A new univaria
+0000f640: 7465 2054 696d 6553 6572 6965 7320 696e  te TimeSeries in
+0000f650: 7374 616e 6365 2e0a 2020 2020 2020 2020  stance..        
+0000f660: 2222 220a 2020 2020 2020 2020 6966 2069  """.        if i
+0000f670: 7369 6e73 7461 6e63 6528 696e 6465 782c  sinstance(index,
+0000f680: 2069 6e74 293a 0a20 2020 2020 2020 2020   int):.         
+0000f690: 2020 206e 6577 5f78 6120 3d20 7365 6c66     new_xa = self
+0000f6a0: 2e5f 7861 2e69 7365 6c28 636f 6d70 6f6e  ._xa.isel(compon
+0000f6b0: 656e 743d 696e 6465 7829 2e65 7870 616e  ent=index).expan
+0000f6c0: 645f 6469 6d73 2844 494d 535b 315d 2c20  d_dims(DIMS[1], 
+0000f6d0: 6178 6973 3d31 290a 2020 2020 2020 2020  axis=1).        
+0000f6e0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000f6f0: 2020 6e65 775f 7861 203d 2073 656c 662e    new_xa = self.
+0000f700: 5f78 612e 7365 6c28 636f 6d70 6f6e 656e  _xa.sel(componen
+0000f710: 743d 696e 6465 7829 2e65 7870 616e 645f  t=index).expand_
+0000f720: 6469 6d73 2844 494d 535b 315d 2c20 6178  dims(DIMS[1], ax
+0000f730: 6973 3d31 290a 2020 2020 2020 2020 7265  is=1).        re
+0000f740: 7475 726e 2054 696d 6553 6572 6965 7328  turn TimeSeries(
+0000f750: 6e65 775f 7861 290a 0a20 2020 2064 6566  new_xa)..    def
+0000f760: 2061 6464 5f64 6174 6574 696d 655f 6174   add_datetime_at
+0000f770: 7472 6962 7574 6528 7365 6c66 2c20 6174  tribute(self, at
+0000f780: 7472 6962 7574 652c 206f 6e65 5f68 6f74  tribute, one_hot
+0000f790: 3a20 626f 6f6c 203d 2046 616c 7365 2920  : bool = False) 
+0000f7a0: 2d3e 2027 5469 6d65 5365 7269 6573 273a  -> 'TimeSeries':
+0000f7b0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000f7c0: 2020 2020 2052 6574 7572 6e73 2061 206e       Returns a n
+0000f7d0: 6577 2054 696d 6553 6572 6965 7320 696e  ew TimeSeries in
+0000f7e0: 7374 616e 6365 2077 6974 6820 6f6e 6520  stance with one 
+0000f7f0: 286f 7220 6d6f 7265 2920 6164 6469 7469  (or more) additi
+0000f800: 6f6e 616c 2063 6f6d 706f 6e65 6e74 2873  onal component(s
+0000f810: 2920 7468 6174 2063 6f6e 7461 696e 2061  ) that contain a
+0000f820: 6e20 6174 7472 6962 7574 650a 2020 2020  n attribute.    
+0000f830: 2020 2020 6f66 2074 6865 2074 696d 6520      of the time 
+0000f840: 696e 6465 7820 6f66 2074 6865 2063 7572  index of the cur
+0000f850: 7265 6e74 2073 6572 6965 7320 7370 6563  rent series spec
+0000f860: 6966 6965 6420 7769 7468 2060 6174 7472  ified with `attr
+0000f870: 6962 7574 6560 2c20 7375 6368 2061 7320  ibute`, such as 
+0000f880: 2777 6565 6b64 6179 272c 2027 6461 7927  'weekday', 'day'
+0000f890: 206f 7220 276d 6f6e 7468 272e 0a0a 2020   or 'month'...  
+0000f8a0: 2020 2020 2020 5468 6973 2077 6f72 6b73        This works
+0000f8b0: 206f 6e6c 7920 666f 7220 6465 7465 726d   only for determ
+0000f8c0: 696e 6973 7469 6320 7469 6d65 2073 6572  inistic time ser
+0000f8d0: 6965 7320 2869 2e65 2e2c 206d 6164 6520  ies (i.e., made 
+0000f8e0: 6f66 2031 2073 616d 706c 6529 2e0a 0a20  of 1 sample)... 
+0000f8f0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+0000f900: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0000f910: 2d2d 2d2d 0a20 2020 2020 2020 2061 7474  ----.        att
+0000f920: 7269 6275 7465 0a20 2020 2020 2020 2020  ribute.         
+0000f930: 2020 2041 2070 642e 4461 7461 7469 6d65     A pd.Datatime
+0000f940: 496e 6465 7820 6174 7472 6962 7574 6520  Index attribute 
+0000f950: 7768 6963 6820 7769 6c6c 2073 6572 7665  which will serve
+0000f960: 2061 7320 7468 6520 6261 7369 7320 6f66   as the basis of
+0000f970: 2074 6865 206e 6577 2063 6f6c 756d 6e28   the new column(
+0000f980: 7329 2e0a 2020 2020 2020 2020 6f6e 655f  s)..        one_
+0000f990: 686f 740a 2020 2020 2020 2020 2020 2020  hot.            
+0000f9a0: 426f 6f6c 6561 6e20 7661 6c75 6520 696e  Boolean value in
+0000f9b0: 6469 6361 7469 6e67 2077 6865 7468 6572  dicating whether
+0000f9c0: 2074 6f20 6164 6420 7468 6520 7370 6563   to add the spec
+0000f9d0: 6966 6965 6420 6174 7472 6962 7574 6520  ified attribute 
+0000f9e0: 6173 2061 206f 6e65 2068 6f74 2065 6e63  as a one hot enc
+0000f9f0: 6f64 696e 670a 2020 2020 2020 2020 2020  oding.          
+0000fa00: 2020 2872 6573 756c 7473 2069 6e20 6d6f    (results in mo
+0000fa10: 7265 2063 6f6c 756d 6e73 292e 0a0a 2020  re columns)...  
+0000fa20: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
+0000fa30: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
+0000fa40: 2020 2020 2020 5469 6d65 5365 7269 6573        TimeSeries
+0000fa50: 0a20 2020 2020 2020 2020 2020 204e 6577  .            New
+0000fa60: 2054 696d 6553 6572 6965 7320 696e 7374   TimeSeries inst
+0000fa70: 616e 6365 2065 6e68 616e 6365 6420 6279  ance enhanced by
+0000fa80: 2060 6174 7472 6962 7574 6560 2e0a 2020   `attribute`..  
+0000fa90: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000faa0: 2020 7365 6c66 2e5f 6173 7365 7274 5f64    self._assert_d
+0000fab0: 6574 6572 6d69 6e69 7374 6963 2829 0a20  eterministic(). 
+0000fac0: 2020 2020 2020 2066 726f 6d20 2e75 7469         from .uti
+0000fad0: 6c73 2069 6d70 6f72 7420 7469 6d65 7365  ls import timese
+0000fae0: 7269 6573 5f67 656e 6572 6174 696f 6e20  ries_generation 
+0000faf0: 6173 2074 670a 2020 2020 2020 2020 7265  as tg.        re
+0000fb00: 7475 726e 2073 656c 662e 7374 6163 6b28  turn self.stack(
+0000fb10: 7467 2e64 6174 6574 696d 655f 6174 7472  tg.datetime_attr
+0000fb20: 6962 7574 655f 7469 6d65 7365 7269 6573  ibute_timeseries
+0000fb30: 2873 656c 662e 7469 6d65 5f69 6e64 6578  (self.time_index
+0000fb40: 2c20 6174 7472 6962 7574 652c 206f 6e65  , attribute, one
+0000fb50: 5f68 6f74 2929 0a0a 2020 2020 6465 6620  _hot))..    def 
+0000fb60: 6164 645f 686f 6c69 6461 7973 2873 656c  add_holidays(sel
+0000fb70: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
+0000fb80: 2020 2020 2020 2020 636f 756e 7472 795f          country_
+0000fb90: 636f 6465 3a20 7374 722c 0a20 2020 2020  code: str,.     
+0000fba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fbb0: 7072 6f76 3a20 7374 7220 3d20 4e6f 6e65  prov: str = None
+0000fbc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000fbd0: 2020 2020 2020 2073 7461 7465 3a20 7374         state: st
+0000fbe0: 7220 3d20 4e6f 6e65 2920 2d3e 2027 5469  r = None) -> 'Ti
+0000fbf0: 6d65 5365 7269 6573 273a 0a20 2020 2020  meSeries':.     
+0000fc00: 2020 2022 2222 0a20 2020 2020 2020 2041     """.        A
+0000fc10: 6464 7320 6120 6269 6e61 7279 2075 6e69  dds a binary uni
+0000fc20: 7661 7269 6174 6520 636f 6d70 6f6e 656e  variate componen
+0000fc30: 7420 746f 2074 6865 2063 7572 7265 6e74  t to the current
+0000fc40: 2073 6572 6965 7320 7468 6174 2065 7175   series that equ
+0000fc50: 616c 7320 3120 6174 2065 7665 7279 2069  als 1 at every i
+0000fc60: 6e64 6578 2074 6861 740a 2020 2020 2020  ndex that.      
+0000fc70: 2020 636f 7272 6573 706f 6e64 7320 746f    corresponds to
+0000fc80: 2073 656c 6563 7465 6420 636f 756e 7472   selected countr
+0000fc90: 7927 7320 686f 6c69 6461 792c 2061 6e64  y's holiday, and
+0000fca0: 2030 206f 7468 6572 7769 7365 2e20 5468   0 otherwise. Th
+0000fcb0: 6520 6672 6571 7565 6e63 7920 6f66 2074  e frequency of t
+0000fcc0: 6865 2054 696d 6553 6572 6965 7320 6973  he TimeSeries is
+0000fcd0: 2064 6169 6c79 2e0a 0a20 2020 2020 2020   daily...       
+0000fce0: 2041 7661 696c 6162 6c65 2063 6f75 6e74   Available count
+0000fcf0: 7269 6573 2063 616e 2062 6520 666f 756e  ries can be foun
+0000fd00: 6420 6068 6572 6520 3c68 7474 7073 3a2f  d `here <https:/
+0000fd10: 2f67 6974 6875 622e 636f 6d2f 6472 2d70  /github.com/dr-p
+0000fd20: 726f 6469 6779 2f70 7974 686f 6e2d 686f  rodigy/python-ho
+0000fd30: 6c69 6461 7973 2361 7661 696c 6162 6c65  lidays#available
+0000fd40: 2d63 6f75 6e74 7269 6573 3e60 5f2e 0a0a  -countries>`_...
+0000fd50: 2020 2020 2020 2020 5468 6973 2077 6f72          This wor
+0000fd60: 6b73 206f 6e6c 7920 666f 7220 6465 7465  ks only for dete
+0000fd70: 726d 696e 6973 7469 6320 7469 6d65 2073  rministic time s
+0000fd80: 6572 6965 7320 2869 2e65 2e2c 206d 6164  eries (i.e., mad
+0000fd90: 6520 6f66 2031 2073 616d 706c 6529 2e0a  e of 1 sample)..
+0000fda0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+0000fdb0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+0000fdc0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2063  ------.        c
+0000fdd0: 6f75 6e74 7279 5f63 6f64 650a 2020 2020  ountry_code.    
+0000fde0: 2020 2020 2020 2020 5468 6520 636f 756e          The coun
+0000fdf0: 7472 7920 4953 4f20 636f 6465 0a20 2020  try ISO code.   
+0000fe00: 2020 2020 2070 726f 760a 2020 2020 2020       prov.      
+0000fe10: 2020 2020 2020 5468 6520 7072 6f76 696e        The provin
+0000fe20: 6365 0a20 2020 2020 2020 2073 7461 7465  ce.        state
+0000fe30: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+0000fe40: 2073 7461 7465 0a0a 2020 2020 2020 2020   state..        
+0000fe50: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+0000fe60: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+0000fe70: 5469 6d65 5365 7269 6573 0a20 2020 2020  TimeSeries.     
+0000fe80: 2020 2020 2020 2041 206e 6577 2054 696d         A new Tim
+0000fe90: 6553 6572 6965 7320 696e 7374 616e 6365  eSeries instance
+0000fea0: 2c20 656e 6861 6e63 6564 2077 6974 6820  , enhanced with 
+0000feb0: 6269 6e61 7279 2068 6f6c 6964 6179 2063  binary holiday c
+0000fec0: 6f6d 706f 6e65 6e74 2e0a 2020 2020 2020  omponent..      
+0000fed0: 2020 2222 220a 2020 2020 2020 2020 7365    """.        se
+0000fee0: 6c66 2e5f 6173 7365 7274 5f64 6574 6572  lf._assert_deter
+0000fef0: 6d69 6e69 7374 6963 2829 0a20 2020 2020  ministic().     
+0000ff00: 2020 2066 726f 6d20 2e75 7469 6c73 2069     from .utils i
+0000ff10: 6d70 6f72 7420 7469 6d65 7365 7269 6573  mport timeseries
+0000ff20: 5f67 656e 6572 6174 696f 6e20 6173 2074  _generation as t
+0000ff30: 670a 2020 2020 2020 2020 7265 7475 726e  g.        return
+0000ff40: 2073 656c 662e 7374 6163 6b28 7467 2e68   self.stack(tg.h
+0000ff50: 6f6c 6964 6179 735f 7469 6d65 7365 7269  olidays_timeseri
+0000ff60: 6573 2873 656c 662e 7469 6d65 5f69 6e64  es(self.time_ind
+0000ff70: 6578 2c20 636f 756e 7472 795f 636f 6465  ex, country_code
+0000ff80: 2c20 7072 6f76 2c20 7374 6174 6529 290a  , prov, state)).
+0000ff90: 0a20 2020 2064 6566 2072 6573 616d 706c  .    def resampl
+0000ffa0: 6528 7365 6c66 2c20 6672 6571 3a20 7374  e(self, freq: st
+0000ffb0: 722c 206d 6574 686f 643a 2073 7472 203d  r, method: str =
+0000ffc0: 2027 7061 6427 2920 2d3e 2027 5469 6d65   'pad') -> 'Time
+0000ffd0: 5365 7269 6573 273a 0a20 2020 2020 2020  Series':.       
+0000ffe0: 2022 2222 0a20 2020 2020 2020 2043 7265   """.        Cre
+0000fff0: 6174 6573 2061 6e20 7265 696e 6465 7865  ates an reindexe
+00010000: 6420 7469 6d65 2073 6572 6965 7320 7769  d time series wi
+00010010: 7468 2061 2067 6976 656e 2066 7265 7175  th a given frequ
+00010020: 656e 6379 2e0a 2020 2020 2020 2020 5072  ency..        Pr
+00010030: 6f76 6964 6564 206d 6574 686f 6420 6973  ovided method is
+00010040: 2075 7365 6420 746f 2066 696c 6c20 686f   used to fill ho
+00010050: 6c65 7320 696e 2072 6569 6e64 6578 6564  les in reindexed
+00010060: 2054 696d 6553 6572 6965 732c 2062 7920   TimeSeries, by 
+00010070: 6465 6661 756c 7420 2770 6164 272e 0a0a  default 'pad'...
+00010080: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00010090: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+000100a0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6672  -----.        fr
+000100b0: 6571 0a20 2020 2020 2020 2020 2020 2054  eq.            T
+000100c0: 6865 206e 6577 2074 696d 6520 6469 6666  he new time diff
+000100d0: 6572 656e 6365 2062 6574 7765 656e 2074  erence between t
+000100e0: 776f 2061 646a 6163 656e 7420 656e 7472  wo adjacent entr
+000100f0: 6965 7320 696e 2074 6865 2072 6574 7572  ies in the retur
+00010100: 6e65 6420 5469 6d65 5365 7269 6573 2e0a  ned TimeSeries..
+00010110: 2020 2020 2020 2020 2020 2020 4120 4461              A Da
+00010120: 7465 4f66 6673 6574 2061 6c69 6173 2069  teOffset alias i
+00010130: 7320 6578 7065 6374 6564 2e0a 2020 2020  s expected..    
+00010140: 2020 2020 6d65 7468 6f64 3a0a 2020 2020      method:.    
+00010150: 2020 2020 2020 2020 4d65 7468 6f64 2074          Method t
+00010160: 6f20 6669 6c6c 2068 6f6c 6573 2069 6e20  o fill holes in 
+00010170: 7265 696e 6465 7865 6420 5469 6d65 5365  reindexed TimeSe
+00010180: 7269 6573 2028 6e6f 7465 2074 6869 7320  ries (note this 
+00010190: 646f 6573 206e 6f74 2066 696c 6c20 4e61  does not fill Na
+000101a0: 4e73 2074 6861 7420 616c 7265 6164 7920  Ns that already 
+000101b0: 7765 7265 2070 7265 7365 6e74 293a 0a0a  were present):..
+000101c0: 2020 2020 2020 2020 2020 2020 e280 9870              ...p
+000101d0: 6164 e280 993a 2070 726f 7061 6761 7465  ad...: propagate
+000101e0: 206c 6173 7420 7661 6c69 6420 6f62 7365   last valid obse
+000101f0: 7276 6174 696f 6e20 666f 7277 6172 6420  rvation forward 
+00010200: 746f 206e 6578 7420 7661 6c69 640a 0a20  to next valid.. 
+00010210: 2020 2020 2020 2020 2020 20e2 8098 6261             ...ba
+00010220: 636b 6669 6c6c e280 993a 2075 7365 204e  ckfill...: use N
+00010230: 4558 5420 7661 6c69 6420 6f62 7365 7276  EXT valid observ
+00010240: 6174 696f 6e20 746f 2066 696c 6c2e 0a20  ation to fill.. 
+00010250: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
+00010260: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
+00010270: 2020 2020 2020 2054 696d 6553 6572 6965         TimeSerie
+00010280: 730a 2020 2020 2020 2020 2020 2020 4120  s.            A 
+00010290: 7265 696e 6465 7865 6420 5469 6d65 5365  reindexed TimeSe
+000102a0: 7269 6573 2077 6974 6820 6769 7665 6e20  ries with given 
+000102b0: 6672 6571 7565 6e63 792e 0a20 2020 2020  frequency..     
+000102c0: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+000102d0: 7265 7361 6d70 6c65 203d 2073 656c 662e  resample = self.
+000102e0: 5f78 612e 7265 7361 6d70 6c65 287b 7365  _xa.resample({se
+000102f0: 6c66 2e5f 7469 6d65 5f64 696d 3a20 6672  lf._time_dim: fr
+00010300: 6571 7d29 0a0a 2020 2020 2020 2020 2320  eq})..        # 
+00010310: 544f 444f 3a20 6368 6563 6b0a 2020 2020  TODO: check.    
+00010320: 2020 2020 6966 206d 6574 686f 6420 3d3d      if method ==
+00010330: 2027 7061 6427 3a0a 2020 2020 2020 2020   'pad':.        
+00010340: 2020 2020 6e65 775f 7861 203d 2072 6573      new_xa = res
+00010350: 616d 706c 652e 7061 6428 290a 2020 2020  ample.pad().    
+00010360: 2020 2020 656c 6966 206d 6574 686f 6420      elif method 
+00010370: 3d3d 2027 6266 696c 6c27 3a0a 2020 2020  == 'bfill':.    
+00010380: 2020 2020 2020 2020 6e65 775f 7861 203d          new_xa =
+00010390: 2072 6573 616d 706c 652e 6261 636b 6669   resample.backfi
+000103a0: 6c6c 2829 0a20 2020 2020 2020 2065 6c73  ll().        els
+000103b0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000103c0: 6169 7365 5f6c 6f67 2856 616c 7565 4572  aise_log(ValueEr
+000103d0: 726f 7228 2755 6e6b 6e6f 776e 206d 6574  ror('Unknown met
+000103e0: 686f 643a 207b 7d27 2e66 6f72 6d61 7428  hod: {}'.format(
+000103f0: 6d65 7468 6f64 2929 2c20 6c6f 6767 6572  method)), logger
+00010400: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00010410: 2054 696d 6553 6572 6965 7328 6e65 775f   TimeSeries(new_
+00010420: 7861 290a 0a20 2020 2064 6566 2069 735f  xa)..    def is_
+00010430: 7769 7468 696e 5f72 616e 6765 2873 656c  within_range(sel
+00010440: 662c 2074 733a 2055 6e69 6f6e 5b70 642e  f, ts: Union[pd.
+00010450: 5469 6d65 7374 616d 702c 2069 6e74 5d29  Timestamp, int])
+00010460: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
+00010470: 2020 2222 220a 2020 2020 2020 2020 4368    """.        Ch
+00010480: 6563 6b20 7768 6574 6865 7220 6120 6769  eck whether a gi
+00010490: 7665 6e20 7469 6d65 7374 616d 7020 6f72  ven timestamp or
+000104a0: 2069 6e74 6567 6572 2069 7320 7769 7468   integer is with
+000104b0: 696e 6720 7468 6520 7469 6d65 2069 6e74  ing the time int
+000104c0: 6572 7661 6c20 6f66 2074 6869 7320 7469  erval of this ti
+000104d0: 6d65 2073 6572 6965 732e 0a20 2020 2020  me series..     
+000104e0: 2020 2049 6620 6120 7469 6d65 7374 616d     If a timestam
+000104f0: 7020 6973 2070 726f 7669 6465 642c 2069  p is provided, i
+00010500: 7420 646f 6573 206e 6f74 206e 6565 6420  t does not need 
+00010510: 746f 2062 6520 616e 2065 6c65 6d65 6e74  to be an element
+00010520: 206f 6620 7468 6520 7469 6d65 2069 6e64   of the time ind
+00010530: 6578 206f 6620 7468 6520 7365 7269 6573  ex of the series
+00010540: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+00010550: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+00010560: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00010570: 2074 730a 2020 2020 2020 2020 2020 2020   ts.            
+00010580: 5468 6520 6070 616e 6461 732e 5469 6d65  The `pandas.Time
+00010590: 7374 616d 7060 2028 6966 2069 6e64 6578  stamp` (if index
+000105a0: 6564 2077 6974 6820 4461 7465 7469 6d65  ed with Datetime
+000105b0: 496e 6465 7829 206f 7220 696e 7465 6765  Index) or intege
+000105c0: 7220 2869 6620 696e 6465 7865 6420 7769  r (if indexed wi
+000105d0: 7468 2049 6e74 3634 496e 6465 7829 2074  th Int64Index) t
+000105e0: 6f20 6368 6563 6b2e 0a0a 2020 2020 2020  o check...      
+000105f0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+00010600: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+00010610: 2020 626f 6f6c 0a20 2020 2020 2020 2020    bool.         
+00010620: 2020 2057 6865 7468 6572 2060 7473 6020     Whether `ts` 
+00010630: 6973 2063 6f6e 7461 696e 6564 2077 6974  is contained wit
+00010640: 6869 6e20 7468 6520 696e 7465 7276 616c  hin the interval
+00010650: 206f 6620 7468 6973 2074 696d 6520 7365   of this time se
+00010660: 7269 6573 2e0a 2020 2020 2020 2020 2222  ries..        ""
+00010670: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+00010680: 2073 656c 662e 7469 6d65 5f69 6e64 6578   self.time_index
+00010690: 5b30 5d20 3c3d 2074 7320 3c3d 2073 656c  [0] <= ts <= sel
+000106a0: 662e 7469 6d65 5f69 6e64 6578 5b2d 315d  f.time_index[-1]
+000106b0: 0a0a 2020 2020 6465 6620 6d61 7028 7365  ..    def map(se
+000106c0: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
+000106d0: 666e 3a20 556e 696f 6e5b 4361 6c6c 6162  fn: Union[Callab
+000106e0: 6c65 5b5b 6e70 2e6e 756d 6265 725d 2c20  le[[np.number], 
+000106f0: 6e70 2e6e 756d 6265 725d 2c0a 2020 2020  np.number],.    
+00010700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010710: 2020 4361 6c6c 6162 6c65 5b5b 556e 696f    Callable[[Unio
+00010720: 6e5b 7064 2e54 696d 6573 7461 6d70 2c20  n[pd.Timestamp, 
+00010730: 696e 745d 2c20 6e70 2e6e 756d 6265 725d  int], np.number]
+00010740: 2c20 6e70 2e6e 756d 6265 725d 5d29 202d  , np.number]]) -
+00010750: 3e20 2754 696d 6553 6572 6965 7327 3a20  > 'TimeSeries': 
+00010760: 2023 206e 6f71 613a 2045 3530 310a 2020   # noqa: E501.  
+00010770: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00010780: 2020 4170 706c 6965 7320 7468 6520 6675    Applies the fu
+00010790: 6e63 7469 6f6e 2060 666e 6020 656c 656d  nction `fn` elem
+000107a0: 656e 7477 6973 6520 746f 2061 6c6c 2076  entwise to all v
+000107b0: 616c 7565 7320 696e 2074 6869 7320 5469  alues in this Ti
+000107c0: 6d65 5365 7269 6573 2e0a 2020 2020 2020  meSeries..      
+000107d0: 2020 5265 7475 726e 7320 6120 6e65 7720    Returns a new 
+000107e0: 5469 6d65 5365 7269 6573 2069 6e73 7461  TimeSeries insta
+000107f0: 6e63 652e 2049 6620 6066 6e60 2074 616b  nce. If `fn` tak
+00010800: 6573 2031 2061 7267 756d 656e 7420 6974  es 1 argument it
+00010810: 2069 7320 7369 6d70 6c79 2061 7070 6c69   is simply appli
+00010820: 6564 2065 6c65 6d65 6e74 7769 7365 2e0a  ed elementwise..
+00010830: 2020 2020 2020 2020 4966 2069 7420 7461          If it ta
+00010840: 6b65 7320 3220 6172 6775 6d65 6e74 732c  kes 2 arguments,
+00010850: 2069 7420 6973 2061 7070 6c69 6564 2065   it is applied e
+00010860: 6c65 6d65 6e74 7769 7365 206f 6e20 7468  lementwise on th
+00010870: 6520 2874 696d 6573 7461 6d70 2c20 7661  e (timestamp, va
+00010880: 6c75 6529 2074 7570 6c65 732e 0a0a 2020  lue) tuples...  
+00010890: 2020 2020 2020 4174 2074 6865 206d 6f6d        At the mom
+000108a0: 656e 7420 7468 6973 2066 756e 6374 696f  ent this functio
+000108b0: 6e20 776f 726b 7320 6f6e 6c79 206f 6e20  n works only on 
+000108c0: 6465 7465 726d 696e 6973 7469 6320 7469  deterministic ti
+000108d0: 6d65 2073 6572 6965 7320 2869 2e65 2e2c  me series (i.e.,
+000108e0: 206d 6164 6520 6f66 2031 2073 616d 706c   made of 1 sampl
+000108f0: 6529 2e0a 0a20 2020 2020 2020 2050 6172  e)...        Par
+00010900: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+00010910: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00010920: 2020 2066 6e0a 2020 2020 2020 2020 2020     fn.          
+00010930: 2020 4569 7468 6572 2061 2066 756e 6374    Either a funct
+00010940: 696f 6e20 7768 6963 6820 7461 6b65 7320  ion which takes 
+00010950: 6120 7661 6c75 6520 616e 6420 7265 7475  a value and retu
+00010960: 726e 7320 6120 7661 6c75 6520 6965 2e20  rns a value ie. 
+00010970: 6066 2878 2920 3d20 7960 0a20 2020 2020  `f(x) = y`.     
+00010980: 2020 2020 2020 204f 7220 6120 6675 6e63         Or a func
+00010990: 7469 6f6e 2077 6869 6368 2074 616b 6573  tion which takes
+000109a0: 2061 2076 616c 7565 2061 6e64 2069 7473   a value and its
+000109b0: 2074 696d 6573 7461 6d70 2061 6e64 2072   timestamp and r
+000109c0: 6574 7572 6e73 2061 2076 616c 7565 2069  eturns a value i
+000109d0: 652e 2060 6628 7469 6d65 7374 616d 702c  e. `f(timestamp,
+000109e0: 2078 2920 3d20 7960 0a20 2020 2020 2020   x) = y`.       
+000109f0: 2020 2020 2054 6865 2074 7970 6520 6f66       The type of
+00010a00: 2060 7469 6d65 7374 616d 7060 2069 7320   `timestamp` is 
+00010a10: 6569 7468 6572 2060 7064 2e54 696d 6573  either `pd.Times
+00010a20: 7461 6d70 6020 2869 6620 7468 6520 7365  tamp` (if the se
+00010a30: 7269 6573 2069 7320 696e 6465 7865 6420  ries is indexed 
+00010a40: 7769 7468 2061 2044 6174 6574 696d 6549  with a DatetimeI
+00010a50: 6e64 6578 292c 0a20 2020 2020 2020 2020  ndex),.         
+00010a60: 2020 206f 7220 616e 2069 6e74 6567 6572     or an integer
+00010a70: 206f 7468 6572 7769 7365 2028 6966 2074   otherwise (if t
+00010a80: 6865 2073 6572 6965 7320 6973 2069 6e64  he series is ind
+00010a90: 6578 6564 2077 6974 6820 616e 2049 6e74  exed with an Int
+00010aa0: 3634 496e 6465 7829 2e0a 0a20 2020 2020  64Index)...     
+00010ab0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+00010ac0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+00010ad0: 2020 2054 696d 6553 6572 6965 730a 2020     TimeSeries.  
+00010ae0: 2020 2020 2020 2020 2020 4120 6e65 7720            A new 
+00010af0: 5469 6d65 5365 7269 6573 2069 6e73 7461  TimeSeries insta
+00010b00: 6e63 650a 2020 2020 2020 2020 2222 220a  nce.        """.
+00010b10: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
+00010b20: 7369 6e73 7461 6e63 6528 666e 2c20 4361  sinstance(fn, Ca
+00010b30: 6c6c 6162 6c65 293a 0a20 2020 2020 2020  llable):.       
+00010b40: 2020 2020 2072 6169 7365 5f6c 6f67 2854       raise_log(T
+00010b50: 7970 6545 7272 6f72 2822 666e 2073 686f  ypeError("fn sho
+00010b60: 756c 6420 6265 2063 616c 6c61 626c 6522  uld be callable"
+00010b70: 292c 206c 6f67 6765 7229 0a0a 2020 2020  ), logger)..    
+00010b80: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00010b90: 6528 666e 2c20 6e70 2e75 6675 6e63 293a  e(fn, np.ufunc):
+00010ba0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00010bb0: 666e 2e6e 696e 203d 3d20 3120 616e 6420  fn.nin == 1 and 
+00010bc0: 666e 2e6e 6f75 7420 3d3d 2031 3a0a 2020  fn.nout == 1:.  
+00010bd0: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
+00010be0: 6d5f 6172 6773 203d 2031 0a20 2020 2020  m_args = 1.     
+00010bf0: 2020 2020 2020 2065 6c69 6620 666e 2e6e         elif fn.n
+00010c00: 696e 203d 3d20 3220 616e 6420 666e 2e6e  in == 2 and fn.n
+00010c10: 6f75 7420 3d3d 2031 3a0a 2020 2020 2020  out == 1:.      
+00010c20: 2020 2020 2020 2020 2020 6e75 6d5f 6172            num_ar
+00010c30: 6773 203d 2032 0a20 2020 2020 2020 2020  gs = 2.         
+00010c40: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00010c50: 2020 2020 2020 2020 2072 6169 7365 5f6c           raise_l
+00010c60: 6f67 2856 616c 7565 4572 726f 7228 2266  og(ValueError("f
+00010c70: 6e20 6d75 7374 2068 6176 6520 6569 7468  n must have eith
+00010c80: 6572 206f 6e65 206f 7220 7477 6f20 6172  er one or two ar
+00010c90: 6775 6d65 6e74 7320 616e 6420 7265 7475  guments and retu
+00010ca0: 726e 2061 2073 696e 676c 6520 7661 6c75  rn a single valu
+00010cb0: 6522 292c 206c 6f67 6765 7229 0a20 2020  e"), logger).   
+00010cc0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00010cd0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00010ce0: 2020 2020 2020 2020 2020 2020 6e75 6d5f              num_
+00010cf0: 6172 6773 203d 206c 656e 2873 6967 6e61  args = len(signa
+00010d00: 7475 7265 2866 6e29 2e70 6172 616d 6574  ture(fn).paramet
+00010d10: 6572 7329 0a20 2020 2020 2020 2020 2020  ers).           
+00010d20: 2065 7863 6570 7420 5661 6c75 6545 7272   except ValueErr
+00010d30: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
+00010d40: 2020 2020 7261 6973 655f 6c6f 6728 5661      raise_log(Va
+00010d50: 6c75 6545 7272 6f72 2822 696e 7370 6563  lueError("inspec
+00010d60: 742e 7369 676e 6174 7572 6528 666e 2920  t.signature(fn) 
+00010d70: 6661 696c 6564 2e20 5472 7920 7772 6170  failed. Try wrap
+00010d80: 7069 6e67 2066 6e20 696e 2061 206c 616d  ping fn in a lam
+00010d90: 6264 612c 2065 2e67 2e20 6c61 6d62 6461  bda, e.g. lambda
+00010da0: 2078 3a20 666e 2878 2922 292c 0a20 2020   x: fn(x)"),.   
+00010db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010dc0: 2020 2020 2020 206c 6f67 6765 7229 0a0a         logger)..
+00010dd0: 2020 2020 2020 2020 6966 206e 756d 5f61          if num_a
+00010de0: 7267 7320 3d3d 2031 3a20 2023 2073 696d  rgs == 1:  # sim
+00010df0: 706c 6520 6d61 7020 6675 6e63 7469 6f6e  ple map function
+00010e00: 2066 2878 290a 2020 2020 2020 2020 2020   f(x).          
+00010e10: 2020 6466 203d 2073 656c 662e 7064 5f64    df = self.pd_d
+00010e20: 6174 6166 7261 6d65 2829 2e61 7070 6c79  ataframe().apply
+00010e30: 6d61 7028 666e 290a 2020 2020 2020 2020  map(fn).        
+00010e40: 656c 6966 206e 756d 5f61 7267 7320 3d3d  elif num_args ==
+00010e50: 2032 3a20 2023 206d 6170 2066 756e 6374   2:  # map funct
+00010e60: 696f 6e20 7573 6573 2074 696d 6573 7461  ion uses timesta
+00010e70: 6d70 2066 2874 696d 6573 7461 6d70 2c20  mp f(timestamp, 
+00010e80: 7829 0a20 2020 2020 2020 2020 2020 2064  x).            d
+00010e90: 6566 2061 7070 6c79 5f66 6e5f 7772 6170  ef apply_fn_wrap
+00010ea0: 7065 7228 726f 7729 3a0a 2020 2020 2020  per(row):.      
+00010eb0: 2020 2020 2020 2020 2020 7469 6d65 7374            timest
+00010ec0: 616d 7020 3d20 726f 772e 6e61 6d65 0a20  amp = row.name. 
+00010ed0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00010ee0: 6574 7572 6e20 726f 772e 6d61 7028 6c61  eturn row.map(la
+00010ef0: 6d62 6461 2078 3a20 666e 2874 696d 6573  mbda x: fn(times
+00010f00: 7461 6d70 2c20 7829 290a 2020 2020 2020  tamp, x)).      
+00010f10: 2020 2020 2020 6466 203d 2073 656c 662e        df = self.
+00010f20: 7064 5f64 6174 6166 7261 6d65 2829 2e61  pd_dataframe().a
+00010f30: 7070 6c79 2861 7070 6c79 5f66 6e5f 7772  pply(apply_fn_wr
+00010f40: 6170 7065 722c 2061 7869 733d 3129 0a20  apper, axis=1). 
+00010f50: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00010f60: 2020 2020 2020 2020 2064 6620 3d20 4e6f           df = No
+00010f70: 6e65 0a20 2020 2020 2020 2020 2020 2072  ne.            r
+00010f80: 6169 7365 5f6c 6f67 2856 616c 7565 4572  aise_log(ValueEr
+00010f90: 726f 7228 2266 6e20 6d75 7374 2068 6176  ror("fn must hav
+00010fa0: 6520 6569 7468 6572 206f 6e65 206f 7220  e either one or 
+00010fb0: 7477 6f20 6172 6775 6d65 6e74 7322 292c  two arguments"),
+00010fc0: 206c 6f67 6765 7229 0a0a 2020 2020 2020   logger)..      
+00010fd0: 2020 7265 7475 726e 2054 696d 6553 6572    return TimeSer
+00010fe0: 6965 732e 6672 6f6d 5f64 6174 6166 7261  ies.from_datafra
+00010ff0: 6d65 2864 6629 0a0a 2020 2020 6465 6620  me(df)..    def 
+00011000: 746f 5f6a 736f 6e28 7365 6c66 2920 2d3e  to_json(self) ->
+00011010: 2073 7472 3a0a 2020 2020 2020 2020 2222   str:.        ""
+00011020: 220a 2020 2020 2020 2020 436f 6e76 6572  ".        Conver
+00011030: 7473 2074 6865 2060 5469 6d65 5365 7269  ts the `TimeSeri
+00011040: 6573 6020 6f62 6a65 6374 2074 6f20 6120  es` object to a 
+00011050: 4a53 4f4e 2053 7472 696e 670a 0a20 2020  JSON String..   
+00011060: 2020 2020 2041 7420 7468 6520 6d6f 6d65       At the mome
+00011070: 6e74 2074 6869 7320 6675 6e63 7469 6f6e  nt this function
+00011080: 2077 6f72 6b73 206f 6e6c 7920 6f6e 2064   works only on d
+00011090: 6574 6572 6d69 6e69 7374 6963 2074 696d  eterministic tim
+000110a0: 6520 7365 7269 6573 2028 692e 652e 2c20  e series (i.e., 
+000110b0: 6d61 6465 206f 6620 3120 7361 6d70 6c65  made of 1 sample
+000110c0: 292e 0a0a 2020 2020 2020 2020 5265 7475  )...        Retu
+000110d0: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
+000110e0: 2d2d 2d0a 2020 2020 2020 2020 7374 720a  ---.        str.
+000110f0: 2020 2020 2020 2020 2020 2020 4120 4a53              A JS
+00011100: 4f4e 2053 7472 696e 6720 7265 7072 6573  ON String repres
+00011110: 656e 7469 6e67 2074 6865 2074 696d 6520  enting the time 
+00011120: 7365 7269 6573 0a20 2020 2020 2020 2022  series.        "
+00011130: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+00011140: 6e20 7365 6c66 2e70 645f 6461 7461 6672  n self.pd_datafr
+00011150: 616d 6528 292e 746f 5f6a 736f 6e28 6f72  ame().to_json(or
+00011160: 6965 6e74 3d27 7370 6c69 7427 2c20 6461  ient='split', da
+00011170: 7465 5f66 6f72 6d61 743d 2769 736f 2729  te_format='iso')
+00011180: 0a0a 2020 2020 6465 6620 706c 6f74 2873  ..    def plot(s
+00011190: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+000111a0: 2020 6e65 775f 706c 6f74 3a20 626f 6f6c    new_plot: bool
+000111b0: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
+000111c0: 2020 2020 2020 2063 656e 7472 616c 5f71         central_q
+000111d0: 7561 6e74 696c 653a 2055 6e69 6f6e 5b66  uantile: Union[f
+000111e0: 6c6f 6174 2c20 7374 725d 203d 2030 2e35  loat, str] = 0.5
+000111f0: 2c0a 2020 2020 2020 2020 2020 2020 206c  ,.             l
+00011200: 6f77 5f71 7561 6e74 696c 653a 204f 7074  ow_quantile: Opt
+00011210: 696f 6e61 6c5b 666c 6f61 745d 203d 2030  ional[float] = 0
+00011220: 2e30 352c 0a20 2020 2020 2020 2020 2020  .05,.           
+00011230: 2020 6869 6768 5f71 7561 6e74 696c 653a    high_quantile:
+00011240: 204f 7074 696f 6e61 6c5b 666c 6f61 745d   Optional[float]
+00011250: 203d 2030 2e39 352c 0a20 2020 2020 2020   = 0.95,.       
+00011260: 2020 2020 2020 2a61 7267 732c 0a20 2020        *args,.   
+00011270: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
+00011280: 6773 293a 0a20 2020 2020 2020 2022 2222  gs):.        """
+00011290: 0a20 2020 2020 2020 2041 2077 7261 7070  .        A wrapp
+000112a0: 6572 206d 6574 686f 6420 6172 6f75 6e64  er method around
+000112b0: 2060 7861 7272 6179 2e44 6174 6141 7272   `xarray.DataArr
+000112c0: 6179 2e70 6c6f 7428 2960 2e0a 0a20 2020  ay.plot()`...   
+000112d0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+000112e0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+000112f0: 2d2d 0a20 2020 2020 2020 206e 6577 5f70  --.        new_p
+00011300: 6c6f 740a 2020 2020 2020 2020 2020 2020  lot.            
+00011310: 7768 6574 6865 7220 746f 2073 7061 776e  whether to spawn
+00011320: 2061 206e 6577 2046 6967 7572 650a 2020   a new Figure.  
+00011330: 2020 2020 2020 6365 6e74 7261 6c5f 7175        central_qu
+00011340: 616e 7469 6c65 0a20 2020 2020 2020 2020  antile.         
+00011350: 2020 2054 6865 2071 7561 6e74 696c 6520     The quantile 
+00011360: 2862 6574 7765 656e 2030 2061 6e64 2031  (between 0 and 1
+00011370: 2920 746f 2070 6c6f 7420 6173 2061 2022  ) to plot as a "
+00011380: 6365 6e74 7261 6c22 2076 616c 7565 2c20  central" value, 
+00011390: 6966 2074 6865 2073 6572 6965 7320 6973  if the series is
+000113a0: 2073 746f 6368 6173 7469 6320 2869 2e65   stochastic (i.e
+000113b0: 2e2c 2069 660a 2020 2020 2020 2020 2020  ., if.          
+000113c0: 2020 6974 2068 6173 206d 756c 7469 706c    it has multipl
+000113d0: 6520 7361 6d70 6c65 7329 2e20 5468 6973  e samples). This
+000113e0: 2077 696c 6c20 6265 2061 7070 6c69 6564   will be applied
+000113f0: 206f 6e20 6561 6368 2063 6f6d 706f 6e65   on each compone
+00011400: 6e74 2073 6570 6172 6174 656c 7920 2869  nt separately (i
+00011410: 2e65 2e2c 2074 6f20 6469 7370 6c61 7920  .e., to display 
+00011420: 7175 616e 7469 6c65 730a 2020 2020 2020  quantiles.      
+00011430: 2020 2020 2020 6f66 2074 6865 2063 6f6d        of the com
+00011440: 706f 6e65 6e74 7327 206d 6172 6769 6e61  ponents' margina
+00011450: 6c20 6469 7374 7269 6275 7469 6f6e 7329  l distributions)
+00011460: 2e20 466f 7220 696e 7374 616e 6365 2c20  . For instance, 
+00011470: 7365 7474 696e 6720 6063 656e 7472 616c  setting `central
+00011480: 5f71 7561 6e74 696c 653d 302e 3560 2077  _quantile=0.5` w
+00011490: 696c 6c20 706c 6f74 2074 6865 0a20 2020  ill plot the.   
+000114a0: 2020 2020 2020 2020 206d 6564 6961 6e20           median 
+000114b0: 6f66 2065 6163 6820 636f 6d70 6f6e 656e  of each componen
+000114c0: 742e 2060 6365 6e74 7261 6c5f 7175 616e  t. `central_quan
+000114d0: 7469 6c65 6020 6361 6e20 616c 736f 2062  tile` can also b
+000114e0: 6520 7365 7420 746f 2027 6d65 616e 272e  e set to 'mean'.
+000114f0: 0a20 2020 2020 2020 206c 6f77 5f71 7561  .        low_qua
+00011500: 6e74 696c 650a 2020 2020 2020 2020 2020  ntile.          
+00011510: 2020 5468 6520 7175 616e 7469 6c65 2074    The quantile t
+00011520: 6f20 7573 6520 666f 7220 7468 6520 6c6f  o use for the lo
+00011530: 7765 7220 626f 756e 6420 6f66 2074 6865  wer bound of the
+00011540: 2070 6c6f 7474 6564 2063 6f6e 6669 6465   plotted confide
+00011550: 6e63 6520 696e 7465 7276 616c 2e20 5369  nce interval. Si
+00011560: 6d69 6c61 7220 746f 2060 6365 6e74 7261  milar to `centra
+00011570: 6c5f 7175 616e 7469 6c65 602c 0a20 2020  l_quantile`,.   
+00011580: 2020 2020 2020 2020 2074 6869 7320 6973           this is
+00011590: 2061 7070 6c69 6564 2074 6f20 6561 6368   applied to each
+000115a0: 2063 6f6d 706f 6e65 6e74 2073 6570 6172   component separ
+000115b0: 6174 656c 7920 2869 2e65 2e2c 2064 6973  ately (i.e., dis
+000115c0: 706c 6179 696e 6720 6d61 7267 696e 616c  playing marginal
+000115d0: 2064 6973 7472 6962 7574 696f 6e73 292e   distributions).
+000115e0: 204e 6f20 636f 6e66 6964 656e 6365 0a20   No confidence. 
+000115f0: 2020 2020 2020 2020 2020 2069 6e74 6572             inter
+00011600: 7661 6c20 6973 2073 686f 776e 2069 6620  val is shown if 
+00011610: 6063 6f6e 6669 6465 6e63 655f 6c6f 775f  `confidence_low_
+00011620: 7175 616e 7469 6c65 6020 6973 204e 6f6e  quantile` is Non
+00011630: 6520 2864 6566 6175 6c74 2030 2e30 3529  e (default 0.05)
+00011640: 2e0a 2020 2020 2020 2020 6869 6768 5f71  ..        high_q
+00011650: 7561 6e74 696c 650a 2020 2020 2020 2020  uantile.        
+00011660: 2020 2020 5468 6520 7175 616e 7469 6c65      The quantile
+00011670: 2074 6f20 7573 6520 666f 7220 7468 6520   to use for the 
+00011680: 7570 7065 7220 626f 756e 6420 6f66 2074  upper bound of t
+00011690: 6865 2070 6c6f 7474 6564 2063 6f6e 6669  he plotted confi
+000116a0: 6465 6e63 6520 696e 7465 7276 616c 2e20  dence interval. 
+000116b0: 5369 6d69 6c61 7220 746f 2060 6365 6e74  Similar to `cent
+000116c0: 7261 6c5f 7175 616e 7469 6c65 602c 0a20  ral_quantile`,. 
+000116d0: 2020 2020 2020 2020 2020 2074 6869 7320             this 
+000116e0: 6973 2061 7070 6c69 6564 2074 6f20 6561  is applied to ea
+000116f0: 6368 2063 6f6d 706f 6e65 6e74 2073 6570  ch component sep
+00011700: 6172 6174 656c 7920 2869 2e65 2e2c 2064  arately (i.e., d
+00011710: 6973 706c 6179 696e 6720 6d61 7267 696e  isplaying margin
+00011720: 616c 2064 6973 7472 6962 7574 696f 6e73  al distributions
+00011730: 292e 204e 6f20 636f 6e66 6964 656e 6365  ). No confidence
+00011740: 0a20 2020 2020 2020 2020 2020 2069 6e74  .            int
+00011750: 6572 7661 6c20 6973 2073 686f 776e 2069  erval is shown i
+00011760: 6620 6068 6967 685f 7175 616e 7469 6c65  f `high_quantile
+00011770: 6020 6973 204e 6f6e 6520 2864 6566 6175  ` is None (defau
+00011780: 6c74 2030 2e39 3529 2e0a 2020 2020 2020  lt 0.95)..      
+00011790: 2020 6172 6773 0a20 2020 2020 2020 2020    args.         
+000117a0: 2020 2073 6f6d 6520 706f 7369 7469 6f6e     some position
+000117b0: 616c 2061 7267 756d 656e 7473 2066 6f72  al arguments for
+000117c0: 2074 6865 2060 706c 6f74 2829 6020 6d65   the `plot()` me
+000117d0: 7468 6f64 0a20 2020 2020 2020 206b 7761  thod.        kwa
+000117e0: 7267 730a 2020 2020 2020 2020 2020 2020  rgs.            
+000117f0: 736f 6d65 206b 6579 776f 7264 2061 7267  some keyword arg
+00011800: 756d 656e 7473 2066 6f72 2074 6865 2060  uments for the `
+00011810: 706c 6f74 2829 6020 6d65 7468 6f64 0a20  plot()` method. 
+00011820: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00011830: 2020 2061 6c70 6861 5f63 6f6e 6669 6465     alpha_confide
+00011840: 6e63 655f 696e 7476 6c73 203d 2030 2e32  nce_intvls = 0.2
+00011850: 350a 0a20 2020 2020 2020 2069 6620 6365  5..        if ce
+00011860: 6e74 7261 6c5f 7175 616e 7469 6c65 2021  ntral_quantile !
+00011870: 3d20 276d 6561 6e27 3a0a 2020 2020 2020  = 'mean':.      
+00011880: 2020 2020 2020 7261 6973 655f 6966 5f6e        raise_if_n
+00011890: 6f74 2869 7369 6e73 7461 6e63 6528 6365  ot(isinstance(ce
+000118a0: 6e74 7261 6c5f 7175 616e 7469 6c65 2c20  ntral_quantile, 
+000118b0: 666c 6f61 7429 2061 6e64 2030 2e20 3c3d  float) and 0. <=
+000118c0: 2063 656e 7472 616c 5f71 7561 6e74 696c   central_quantil
+000118d0: 6520 3c3d 2031 2e2c 0a20 2020 2020 2020  e <= 1.,.       
+000118e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000118f0: 2020 2763 656e 7472 616c 5f71 7561 6e74    'central_quant
+00011900: 696c 6520 6d75 7374 2062 6520 6569 7468  ile must be eith
+00011910: 6572 2022 6d65 616e 222c 206f 7220 6120  er "mean", or a 
+00011920: 666c 6f61 7420 6265 7477 6565 6e20 3020  float between 0 
+00011930: 616e 6420 312e 272c 0a20 2020 2020 2020  and 1.',.       
+00011940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011950: 2020 6c6f 6767 6572 290a 0a20 2020 2020    logger)..     
+00011960: 2020 2069 6620 6869 6768 5f71 7561 6e74     if high_quant
+00011970: 696c 6520 6973 206e 6f74 204e 6f6e 6520  ile is not None 
+00011980: 616e 6420 6c6f 775f 7175 616e 7469 6c65  and low_quantile
+00011990: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000119a0: 2020 2020 2020 2020 2020 7261 6973 655f            raise_
+000119b0: 6966 5f6e 6f74 2830 2e20 3c3d 206c 6f77  if_not(0. <= low
+000119c0: 5f71 7561 6e74 696c 6520 3c3d 2031 2e20  _quantile <= 1. 
+000119d0: 616e 6420 302e 203c 3d20 6869 6768 5f71  and 0. <= high_q
+000119e0: 7561 6e74 696c 6520 3c3d 2031 2e2c 0a20  uantile <= 1.,. 
+000119f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a00: 2020 2020 2020 2020 2763 6f6e 6669 6465          'confide
+00011a10: 6e63 6520 696e 7465 7276 616c 206c 6f77  nce interval low
+00011a20: 2061 6e64 2068 6967 6820 7175 616e 7469   and high quanti
+00011a30: 6c65 7320 6d75 7374 2062 6520 6265 7477  les must be betw
+00011a40: 6565 6e20 3020 616e 6420 312e 272c 0a20  een 0 and 1.',. 
+00011a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a60: 2020 2020 2020 2020 6c6f 6767 6572 290a          logger).
+00011a70: 0a20 2020 2020 2020 2066 6967 203d 2028  .        fig = (
+00011a80: 706c 742e 6669 6775 7265 2829 2069 6620  plt.figure() if 
+00011a90: 6e65 775f 706c 6f74 2065 6c73 6520 286b  new_plot else (k
+00011aa0: 7761 7267 735b 2766 6967 7572 6527 5d20  wargs['figure'] 
+00011ab0: 6966 2027 6669 6775 7265 2720 696e 206b  if 'figure' in k
+00011ac0: 7761 7267 7320 656c 7365 2070 6c74 2e67  wargs else plt.g
+00011ad0: 6366 2829 2929 0a20 2020 2020 2020 206b  cf())).        k
+00011ae0: 7761 7267 735b 2766 6967 7572 6527 5d20  wargs['figure'] 
+00011af0: 3d20 6669 670a 2020 2020 2020 2020 6c61  = fig.        la
+00011b00: 6265 6c20 3d20 6b77 6172 6773 5b27 6c61  bel = kwargs['la
+00011b10: 6265 6c27 5d20 6966 2027 6c61 6265 6c27  bel'] if 'label'
+00011b20: 2069 6e20 6b77 6172 6773 2065 6c73 6520   in kwargs else 
+00011b30: 2727 0a0a 2020 2020 2020 2020 6966 2027  ''..        if '
+00011b40: 6c77 2720 6e6f 7420 696e 206b 7761 7267  lw' not in kwarg
+00011b50: 733a 0a20 2020 2020 2020 2020 2020 206b  s:.            k
+00011b60: 7761 7267 735b 276c 7727 5d20 3d20 320a  wargs['lw'] = 2.
+00011b70: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00011b80: 2e6e 5f63 6f6d 706f 6e65 6e74 7320 3e20  .n_components > 
+00011b90: 3130 3a0a 2020 2020 2020 2020 2020 2020  10:.            
+00011ba0: 6c6f 6767 6572 2e77 6172 6e28 274e 756d  logger.warn('Num
+00011bb0: 6265 7220 6f66 2063 6f6d 706f 6e65 6e74  ber of component
+00011bc0: 7320 6973 206c 6172 6765 7220 7468 616e  s is larger than
+00011bd0: 2031 3020 287b 7d29 2e20 506c 6f74 7469   10 ({}). Plotti
+00011be0: 6e67 206f 6e6c 7920 7468 6520 6669 7273  ng only the firs
+00011bf0: 7420 3130 2063 6f6d 706f 6e65 6e74 732e  t 10 components.
+00011c00: 272e 666f 726d 6174 280a 2020 2020 2020  '.format(.      
+00011c10: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00011c20: 5f63 6f6d 706f 6e65 6e74 730a 2020 2020  _components.    
+00011c30: 2020 2020 2020 2020 2929 0a0a 2020 2020          ))..    
+00011c40: 2020 2020 666f 7220 692c 2063 2069 6e20      for i, c in 
+00011c50: 656e 756d 6572 6174 6528 7365 6c66 2e5f  enumerate(self._
+00011c60: 7861 2e63 6f6d 706f 6e65 6e74 5b3a 3130  xa.component[:10
+00011c70: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
+00011c80: 636f 6d70 5f6e 616d 6520 3d20 7374 7228  comp_name = str(
+00011c90: 632e 7661 6c75 6573 290a 0a20 2020 2020  c.values)..     
+00011ca0: 2020 2020 2020 2069 6620 6920 3e20 303a         if i > 0:
+00011cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011cc0: 206b 7761 7267 735b 2766 6967 7572 6527   kwargs['figure'
+00011cd0: 5d20 3d20 706c 742e 6763 6628 290a 0a20  ] = plt.gcf().. 
+00011ce0: 2020 2020 2020 2020 2020 2063 6f6d 7020             comp 
+00011cf0: 3d20 7365 6c66 2e5f 7861 2e73 656c 2863  = self._xa.sel(c
+00011d00: 6f6d 706f 6e65 6e74 3d63 290a 0a20 2020  omponent=c)..   
+00011d10: 2020 2020 2020 2020 2069 6620 636f 6d70           if comp
+00011d20: 2e73 616d 706c 652e 7369 7a65 203e 2031  .sample.size > 1
+00011d30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00011d40: 2020 6966 2063 656e 7472 616c 5f71 7561    if central_qua
+00011d50: 6e74 696c 6520 3d3d 2027 6d65 616e 273a  ntile == 'mean':
+00011d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011d70: 2020 2020 2063 656e 7472 616c 5f73 6572       central_ser
+00011d80: 6965 7320 3d20 636f 6d70 2e6d 6561 6e28  ies = comp.mean(
+00011d90: 6469 6d3d 4449 4d53 5b32 5d29 0a20 2020  dim=DIMS[2]).   
+00011da0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00011db0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00011dc0: 2020 2020 2020 2063 656e 7472 616c 5f73         central_s
+00011dd0: 6572 6965 7320 3d20 636f 6d70 2e71 7561  eries = comp.qua
+00011de0: 6e74 696c 6528 713d 6365 6e74 7261 6c5f  ntile(q=central_
+00011df0: 7175 616e 7469 6c65 2c20 6469 6d3d 4449  quantile, dim=DI
+00011e00: 4d53 5b32 5d29 0a20 2020 2020 2020 2020  MS[2]).         
+00011e10: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00011e20: 2020 2020 2020 2020 2063 656e 7472 616c           central
+00011e30: 5f73 6572 6965 7320 3d20 636f 6d70 2e6d  _series = comp.m
+00011e40: 6561 6e28 6469 6d3d 4449 4d53 5b32 5d29  ean(dim=DIMS[2])
+00011e50: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00011e60: 7465 6d70 6f72 6172 696c 7920 7365 7420  temporarily set 
+00011e70: 616c 7068 6120 746f 2031 2074 6f20 706c  alpha to 1 to pl
+00011e80: 6f74 2074 6865 2063 656e 7472 616c 2076  ot the central v
+00011e90: 616c 7565 2028 7468 6973 2077 6179 2061  alue (this way a
+00011ea0: 6c70 6861 2069 6d70 6163 7473 206f 6e6c  lpha impacts onl
+00011eb0: 7920 7468 6520 636f 6e66 6964 656e 6365  y the confidence
+00011ec0: 2069 6e74 766c 7329 0a20 2020 2020 2020   intvls).       
+00011ed0: 2020 2020 2061 6c70 6861 203d 206b 7761       alpha = kwa
+00011ee0: 7267 735b 2761 6c70 6861 275d 2069 6620  rgs['alpha'] if 
+00011ef0: 2761 6c70 6861 2720 696e 206b 7761 7267  'alpha' in kwarg
+00011f00: 7320 656c 7365 204e 6f6e 650a 2020 2020  s else None.    
+00011f10: 2020 2020 2020 2020 6b77 6172 6773 5b27          kwargs['
+00011f20: 616c 7068 6127 5d20 3d20 310a 0a20 2020  alpha'] = 1..   
+00011f30: 2020 2020 2020 2020 206c 6162 656c 5f74           label_t
+00011f40: 6f5f 7573 6520 3d20 286c 6162 656c 202b  o_use = (label +
+00011f50: 2028 275f 2720 2b20 7374 7228 6929 2069   ('_' + str(i) i
+00011f60: 6620 6c65 6e28 7365 6c66 2e63 6f6d 706f  f len(self.compo
+00011f70: 6e65 6e74 7329 203e 2031 2065 6c73 6520  nents) > 1 else 
+00011f80: 2727 2929 2069 6620 6c61 6265 6c20 213d  '')) if label !=
+00011f90: 2027 2720 5c0a 2020 2020 2020 2020 2020   '' \.          
+00011fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011fb0: 2065 6c73 6520 2727 202b 2073 7472 2863   else '' + str(c
+00011fc0: 6f6d 705f 6e61 6d65 290a 2020 2020 2020  omp_name).      
+00011fd0: 2020 2020 2020 6b77 6172 6773 5b27 6c61        kwargs['la
+00011fe0: 6265 6c27 5d20 3d20 6c61 6265 6c5f 746f  bel'] = label_to
+00011ff0: 5f75 7365 0a0a 2020 2020 2020 2020 2020  _use..          
+00012000: 2020 7020 3d20 6365 6e74 7261 6c5f 7365    p = central_se
+00012010: 7269 6573 2e70 6c6f 7428 2a61 7267 732c  ries.plot(*args,
+00012020: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
+00012030: 2020 2020 2020 2063 6f6c 6f72 5f75 7365         color_use
+00012040: 6420 3d20 705b 305d 2e67 6574 5f63 6f6c  d = p[0].get_col
+00012050: 6f72 2829 0a20 2020 2020 2020 2020 2020  or().           
+00012060: 206b 7761 7267 735b 2761 6c70 6861 275d   kwargs['alpha']
+00012070: 203d 2061 6c70 6861 2069 6620 616c 7068   = alpha if alph
+00012080: 6120 6973 206e 6f74 204e 6f6e 6520 656c  a is not None el
+00012090: 7365 2061 6c70 6861 5f63 6f6e 6669 6465  se alpha_confide
+000120a0: 6e63 655f 696e 7476 6c73 0a0a 2020 2020  nce_intvls..    
+000120b0: 2020 2020 2020 2020 2320 4f70 7469 6f6e          # Option
+000120c0: 616c 6c79 2073 686f 7720 636f 6e66 6964  ally show confid
+000120d0: 656e 6365 2069 6e74 6572 7661 6c73 0a20  ence intervals. 
+000120e0: 2020 2020 2020 2020 2020 2069 6620 636f             if co
+000120f0: 6d70 2e73 616d 706c 652e 7369 7a65 203e  mp.sample.size >
+00012100: 2031 2061 6e64 206c 6f77 5f71 7561 6e74   1 and low_quant
+00012110: 696c 6520 6973 206e 6f74 204e 6f6e 6520  ile is not None 
+00012120: 616e 6420 6869 6768 5f71 7561 6e74 696c  and high_quantil
+00012130: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+00012140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012150: 2020 206c 6f77 5f73 6572 6965 7320 3d20     low_series = 
+00012160: 636f 6d70 2e71 7561 6e74 696c 6528 713d  comp.quantile(q=
+00012170: 6c6f 775f 7175 616e 7469 6c65 2c20 6469  low_quantile, di
+00012180: 6d3d 4449 4d53 5b32 5d29 0a20 2020 2020  m=DIMS[2]).     
+00012190: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+000121a0: 6967 685f 7365 7269 6573 203d 2063 6f6d  igh_series = com
+000121b0: 702e 7175 616e 7469 6c65 2871 3d68 6967  p.quantile(q=hig
+000121c0: 685f 7175 616e 7469 6c65 2c20 6469 6d3d  h_quantile, dim=
+000121d0: 4449 4d53 5b32 5d29 0a20 2020 2020 2020  DIMS[2]).       
+000121e0: 2020 2020 2020 2020 2020 2020 2070 6c74               plt
+000121f0: 2e66 696c 6c5f 6265 7477 6565 6e28 7365  .fill_between(se
+00012200: 6c66 2e74 696d 655f 696e 6465 782c 206c  lf.time_index, l
+00012210: 6f77 5f73 6572 6965 732c 2068 6967 685f  ow_series, high_
+00012220: 7365 7269 6573 2c20 636f 6c6f 723d 636f  series, color=co
+00012230: 6c6f 725f 7573 6564 2c0a 2020 2020 2020  lor_used,.      
+00012240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012250: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00012260: 6c70 6861 3d28 616c 7068 615f 636f 6e66  lpha=(alpha_conf
+00012270: 6964 656e 6365 5f69 6e74 766c 7320 6966  idence_intvls if
+00012280: 2027 616c 7068 6127 206e 6f74 2069 6e20   'alpha' not in 
+00012290: 6b77 6172 6773 2065 6c73 6520 6b77 6172  kwargs else kwar
+000122a0: 6773 5b27 616c 7068 6127 5d29 290a 0a20  gs['alpha'])).. 
+000122b0: 2020 2020 2020 2070 6c74 2e6c 6567 656e         plt.legen
+000122c0: 6428 290a 2020 2020 2020 2020 706c 742e  d().        plt.
+000122d0: 7469 746c 6528 7365 6c66 2e5f 7861 2e6e  title(self._xa.n
+000122e0: 616d 6529 3b0a 0a20 2020 2022 2222 0a20  ame);..    """. 
+000122f0: 2020 2053 696d 706c 6520 7374 6174 6973     Simple statis
+00012300: 7469 6373 2e20 4174 2074 6865 206d 6f6d  tics. At the mom
+00012310: 656e 7420 7468 6573 6520 776f 726b 206f  ent these work o
+00012320: 6e6c 7920 6f6e 2064 6574 6572 6d69 6e69  nly on determini
+00012330: 7374 6963 2073 6572 6965 732c 2061 6e64  stic series, and
+00012340: 2061 7265 2077 7261 7070 6564 2061 726f   are wrapped aro
+00012350: 756e 6420 5061 6e64 6173 2e0a 2020 2020  und Pandas..    
+00012360: 2222 220a 0a20 2020 2064 6566 206d 6561  """..    def mea
+00012370: 6e28 7365 6c66 2c20 6178 6973 3d4e 6f6e  n(self, axis=Non
+00012380: 652c 2073 6b69 706e 613d 4e6f 6e65 2c20  e, skipna=None, 
+00012390: 6c65 7665 6c3d 4e6f 6e65 2c20 6e75 6d65  level=None, nume
+000123a0: 7269 635f 6f6e 6c79 3d4e 6f6e 652c 202a  ric_only=None, *
+000123b0: 2a6b 7761 7267 7329 202d 3e20 666c 6f61  *kwargs) -> floa
+000123c0: 743a 0a20 2020 2020 2020 2072 6574 7572  t:.        retur
+000123d0: 6e20 7365 6c66 2e70 645f 6461 7461 6672  n self.pd_datafr
+000123e0: 616d 6528 636f 7079 3d46 616c 7365 292e  ame(copy=False).
+000123f0: 6d65 616e 2861 7869 732c 2073 6b69 706e  mean(axis, skipn
+00012400: 612c 206c 6576 656c 2c20 6e75 6d65 7269  a, level, numeri
+00012410: 635f 6f6e 6c79 2c20 2a2a 6b77 6172 6773  c_only, **kwargs
+00012420: 290a 0a20 2020 2064 6566 2076 6172 2873  )..    def var(s
+00012430: 656c 662c 2061 7869 733d 4e6f 6e65 2c20  elf, axis=None, 
+00012440: 736b 6970 6e61 3d4e 6f6e 652c 206c 6576  skipna=None, lev
+00012450: 656c 3d4e 6f6e 652c 2064 646f 663d 312c  el=None, ddof=1,
+00012460: 206e 756d 6572 6963 5f6f 6e6c 793d 4e6f   numeric_only=No
+00012470: 6e65 2c20 2a2a 6b77 6172 6773 2920 2d3e  ne, **kwargs) ->
+00012480: 2066 6c6f 6174 3a0a 2020 2020 2020 2020   float:.        
+00012490: 7265 7475 726e 2073 656c 662e 7064 5f64  return self.pd_d
+000124a0: 6174 6166 7261 6d65 2863 6f70 793d 4661  ataframe(copy=Fa
+000124b0: 6c73 6529 2e76 6172 2861 7869 732c 2073  lse).var(axis, s
+000124c0: 6b69 706e 612c 206c 6576 656c 2c20 6464  kipna, level, dd
+000124d0: 6f66 2c20 6e75 6d65 7269 635f 6f6e 6c79  of, numeric_only
+000124e0: 2c20 2a2a 6b77 6172 6773 290a 0a20 2020  , **kwargs)..   
+000124f0: 2064 6566 2073 7464 2873 656c 662c 2061   def std(self, a
+00012500: 7869 733d 4e6f 6e65 2c20 736b 6970 6e61  xis=None, skipna
+00012510: 3d4e 6f6e 652c 206c 6576 656c 3d4e 6f6e  =None, level=Non
+00012520: 652c 2064 646f 663d 312c 206e 756d 6572  e, ddof=1, numer
+00012530: 6963 5f6f 6e6c 793d 4e6f 6e65 2c20 2a2a  ic_only=None, **
+00012540: 6b77 6172 6773 2920 2d3e 2066 6c6f 6174  kwargs) -> float
+00012550: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00012560: 2073 656c 662e 7064 5f64 6174 6166 7261   self.pd_datafra
+00012570: 6d65 2863 6f70 793d 4661 6c73 6529 2e73  me(copy=False).s
+00012580: 7464 2861 7869 732c 2073 6b69 706e 612c  td(axis, skipna,
+00012590: 206c 6576 656c 2c20 6464 6f66 2c20 6e75   level, ddof, nu
+000125a0: 6d65 7269 635f 6f6e 6c79 2c20 2a2a 6b77  meric_only, **kw
+000125b0: 6172 6773 290a 0a20 2020 2064 6566 2073  args)..    def s
+000125c0: 6b65 7728 7365 6c66 2c20 6178 6973 3d4e  kew(self, axis=N
+000125d0: 6f6e 652c 2073 6b69 706e 613d 4e6f 6e65  one, skipna=None
+000125e0: 2c20 6c65 7665 6c3d 4e6f 6e65 2c20 6e75  , level=None, nu
+000125f0: 6d65 7269 635f 6f6e 6c79 3d4e 6f6e 652c  meric_only=None,
+00012600: 202a 2a6b 7761 7267 7329 202d 3e20 666c   **kwargs) -> fl
+00012610: 6f61 743a 0a20 2020 2020 2020 2072 6574  oat:.        ret
+00012620: 7572 6e20 7365 6c66 2e70 645f 6461 7461  urn self.pd_data
+00012630: 6672 616d 6528 636f 7079 3d46 616c 7365  frame(copy=False
+00012640: 292e 736b 6577 2861 7869 732c 2073 6b69  ).skew(axis, ski
+00012650: 706e 612c 206c 6576 656c 2c20 6e75 6d65  pna, level, nume
+00012660: 7269 635f 6f6e 6c79 2c20 2a2a 6b77 6172  ric_only, **kwar
+00012670: 6773 290a 0a20 2020 2064 6566 206b 7572  gs)..    def kur
+00012680: 746f 7369 7328 7365 6c66 2c20 6178 6973  tosis(self, axis
+00012690: 3d4e 6f6e 652c 2073 6b69 706e 613d 4e6f  =None, skipna=No
+000126a0: 6e65 2c20 6c65 7665 6c3d 4e6f 6e65 2c20  ne, level=None, 
+000126b0: 6e75 6d65 7269 635f 6f6e 6c79 3d4e 6f6e  numeric_only=Non
+000126c0: 652c 202a 2a6b 7761 7267 7329 202d 3e20  e, **kwargs) -> 
+000126d0: 666c 6f61 743a 0a20 2020 2020 2020 2072  float:.        r
+000126e0: 6574 7572 6e20 7365 6c66 2e70 645f 6461  eturn self.pd_da
+000126f0: 7461 6672 616d 6528 636f 7079 3d46 616c  taframe(copy=Fal
+00012700: 7365 292e 6b75 7274 6f73 6973 2861 7869  se).kurtosis(axi
+00012710: 732c 2073 6b69 706e 612c 206c 6576 656c  s, skipna, level
+00012720: 2c20 6e75 6d65 7269 635f 6f6e 6c79 2c20  , numeric_only, 
+00012730: 2a2a 6b77 6172 6773 290a 0a20 2020 2064  **kwargs)..    d
+00012740: 6566 206d 696e 2873 656c 662c 2061 7869  ef min(self, axi
+00012750: 733d 4e6f 6e65 2c20 736b 6970 6e61 3d4e  s=None, skipna=N
+00012760: 6f6e 652c 206c 6576 656c 3d4e 6f6e 652c  one, level=None,
+00012770: 206e 756d 6572 6963 5f6f 6e6c 793d 4e6f   numeric_only=No
+00012780: 6e65 2c20 2a2a 6b77 6172 6773 2920 2d3e  ne, **kwargs) ->
+00012790: 2066 6c6f 6174 3a0a 2020 2020 2020 2020   float:.        
+000127a0: 7265 7475 726e 2073 656c 662e 7064 5f64  return self.pd_d
+000127b0: 6174 6166 7261 6d65 2863 6f70 793d 4661  ataframe(copy=Fa
+000127c0: 6c73 6529 2e6d 696e 2861 7869 732c 2073  lse).min(axis, s
+000127d0: 6b69 706e 612c 206c 6576 656c 2c20 6e75  kipna, level, nu
+000127e0: 6d65 7269 635f 6f6e 6c79 2c20 2a2a 6b77  meric_only, **kw
+000127f0: 6172 6773 290a 0a20 2020 2064 6566 206d  args)..    def m
+00012800: 6178 2873 656c 662c 2061 7869 733d 4e6f  ax(self, axis=No
+00012810: 6e65 2c20 736b 6970 6e61 3d4e 6f6e 652c  ne, skipna=None,
+00012820: 206c 6576 656c 3d4e 6f6e 652c 206e 756d   level=None, num
+00012830: 6572 6963 5f6f 6e6c 793d 4e6f 6e65 2c20  eric_only=None, 
+00012840: 2a2a 6b77 6172 6773 2920 2d3e 2066 6c6f  **kwargs) -> flo
+00012850: 6174 3a0a 2020 2020 2020 2020 7265 7475  at:.        retu
+00012860: 726e 2073 656c 662e 7064 5f64 6174 6166  rn self.pd_dataf
+00012870: 7261 6d65 2863 6f70 793d 4661 6c73 6529  rame(copy=False)
+00012880: 2e6d 6178 2861 7869 732c 2073 6b69 706e  .max(axis, skipn
+00012890: 612c 206c 6576 656c 2c20 6e75 6d65 7269  a, level, numeri
+000128a0: 635f 6f6e 6c79 2c20 2a2a 6b77 6172 6773  c_only, **kwargs
+000128b0: 290a 0a20 2020 2064 6566 2073 756d 2873  )..    def sum(s
+000128c0: 656c 662c 2061 7869 733d 4e6f 6e65 2c20  elf, axis=None, 
+000128d0: 736b 6970 6e61 3d4e 6f6e 652c 206c 6576  skipna=None, lev
+000128e0: 656c 3d4e 6f6e 652c 206e 756d 6572 6963  el=None, numeric
+000128f0: 5f6f 6e6c 793d 4e6f 6e65 2c20 6d69 6e5f  _only=None, min_
+00012900: 636f 756e 743d 302c 202a 2a6b 7761 7267  count=0, **kwarg
+00012910: 7329 202d 3e20 666c 6f61 743a 0a20 2020  s) -> float:.   
+00012920: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00012930: 2e70 645f 6461 7461 6672 616d 6528 636f  .pd_dataframe(co
+00012940: 7079 3d46 616c 7365 292e 7375 6d28 6178  py=False).sum(ax
+00012950: 6973 2c20 736b 6970 6e61 2c20 6c65 7665  is, skipna, leve
+00012960: 6c2c 206e 756d 6572 6963 5f6f 6e6c 792c  l, numeric_only,
+00012970: 206d 696e 5f63 6f75 6e74 2c20 2a2a 6b77   min_count, **kw
+00012980: 6172 6773 290a 0a20 2020 2064 6566 206d  args)..    def m
+00012990: 6564 6961 6e28 7365 6c66 2c20 6178 6973  edian(self, axis
+000129a0: 3d4e 6f6e 652c 2073 6b69 706e 613d 4e6f  =None, skipna=No
+000129b0: 6e65 2c20 6c65 7665 6c3d 4e6f 6e65 2c20  ne, level=None, 
+000129c0: 6e75 6d65 7269 635f 6f6e 6c79 3d4e 6f6e  numeric_only=Non
+000129d0: 652c 202a 2a6b 7761 7267 7329 202d 3e20  e, **kwargs) -> 
+000129e0: 666c 6f61 743a 0a20 2020 2020 2020 2072  float:.        r
+000129f0: 6574 7572 6e20 7365 6c66 2e70 645f 6461  eturn self.pd_da
+00012a00: 7461 6672 616d 6528 636f 7079 3d46 616c  taframe(copy=Fal
+00012a10: 7365 292e 6d65 6469 616e 2861 7869 732c  se).median(axis,
+00012a20: 2073 6b69 706e 612c 206c 6576 656c 2c20   skipna, level, 
+00012a30: 6e75 6d65 7269 635f 6f6e 6c79 2c20 2a2a  numeric_only, **
+00012a40: 6b77 6172 6773 290a 0a20 2020 2064 6566  kwargs)..    def
+00012a50: 2061 7574 6f63 6f72 7228 7365 6c66 2c20   autocorr(self, 
+00012a60: 6c61 673d 3129 202d 3e20 666c 6f61 743a  lag=1) -> float:
+00012a70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00012a80: 7365 6c66 2e70 645f 6461 7461 6672 616d  self.pd_datafram
+00012a90: 6528 636f 7079 3d46 616c 7365 292e 6175  e(copy=False).au
+00012aa0: 746f 636f 7272 286c 6167 290a 0a20 2020  tocorr(lag)..   
+00012ab0: 2064 6566 2064 6573 6372 6962 6528 7365   def describe(se
+00012ac0: 6c66 2c20 7065 7263 656e 7469 6c65 733d  lf, percentiles=
+00012ad0: 4e6f 6e65 2c20 696e 636c 7564 653d 4e6f  None, include=No
+00012ae0: 6e65 2c20 6578 636c 7564 653d 4e6f 6e65  ne, exclude=None
+00012af0: 2920 2d3e 2070 642e 4461 7461 4672 616d  ) -> pd.DataFram
+00012b00: 653a 0a20 2020 2020 2020 2072 6574 7572  e:.        retur
+00012b10: 6e20 7365 6c66 2e70 645f 6461 7461 6672  n self.pd_datafr
+00012b20: 616d 6528 636f 7079 3d46 616c 7365 292e  ame(copy=False).
+00012b30: 6465 7363 7269 6265 2870 6572 6365 6e74  describe(percent
+00012b40: 696c 6573 2c20 696e 636c 7564 652c 2065  iles, include, e
+00012b50: 7863 6c75 6465 290a 0a20 2020 2022 2222  xclude)..    """
+00012b60: 0a20 2020 2044 756e 6465 7220 6d65 7468  .    Dunder meth
+00012b70: 6f64 730a 2020 2020 2222 220a 0a20 2020  ods.    """..   
+00012b80: 2023 0a20 2020 2064 6566 205f 636f 6d62   #.    def _comb
+00012b90: 696e 655f 6172 7261 7973 2873 656c 662c  ine_arrays(self,
+00012ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012bb0: 2020 2020 2020 2020 206f 7468 6572 3a20           other: 
+00012bc0: 556e 696f 6e5b 2754 696d 6553 6572 6965  Union['TimeSerie
+00012bd0: 7327 2c20 7872 2e44 6174 6141 7272 6179  s', xr.DataArray
+00012be0: 2c20 6e70 2e6e 6461 7272 6179 5d2c 0a20  , np.ndarray],. 
+00012bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c00: 2020 2020 2020 2063 6f6d 6269 6e65 5f66         combine_f
+00012c10: 6e3a 2043 616c 6c61 626c 655b 5b6e 702e  n: Callable[[np.
+00012c20: 6e64 6172 7261 792c 206e 702e 6e64 6172  ndarray, np.ndar
+00012c30: 7261 795d 2c20 6e70 2e6e 6461 7272 6179  ray], np.ndarray
+00012c40: 5d29 202d 3e20 2754 696d 6553 6572 6965  ]) -> 'TimeSerie
+00012c50: 7327 3a0a 2020 2020 2020 2020 2222 220a  s':.        """.
+00012c60: 2020 2020 2020 2020 5468 6973 2069 7320          This is 
+00012c70: 6120 6865 6c70 6572 2066 756e 6374 696f  a helper functio
+00012c80: 6e20 7468 6174 2061 6c6c 6f77 7320 7573  n that allows us
+00012c90: 2074 6f20 636f 6d62 696e 6520 7468 6973   to combine this
+00012ca0: 2073 6572 6965 7320 7769 7468 2061 6e6f   series with ano
+00012cb0: 7468 6572 206f 6e65 2c0a 2020 2020 2020  ther one,.      
+00012cc0: 2020 6469 7265 6374 6c79 2061 7070 6c79    directly apply
+00012cd0: 696e 6720 616e 206f 7065 7261 7469 6f6e  ing an operation
+00012ce0: 206f 6e20 7468 6569 7220 756e 6465 726c   on their underl
+00012cf0: 7969 6e67 206e 756d 7079 2061 7272 6179  ying numpy array
+00012d00: 732e 0a20 2020 2020 2020 2022 2222 0a0a  s..        """..
+00012d10: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00012d20: 7461 6e63 6528 6f74 6865 722c 2054 696d  tance(other, Tim
+00012d30: 6553 6572 6965 7329 3a0a 2020 2020 2020  eSeries):.      
+00012d40: 2020 2020 2020 6f74 6865 725f 7661 6c73        other_vals
+00012d50: 203d 206f 7468 6572 2e64 6174 615f 6172   = other.data_ar
+00012d60: 7261 7928 636f 7079 3d46 616c 7365 292e  ray(copy=False).
+00012d70: 7661 6c75 6573 0a20 2020 2020 2020 2065  values.        e
+00012d80: 6c69 6620 6973 696e 7374 616e 6365 286f  lif isinstance(o
+00012d90: 7468 6572 2c20 7872 2e44 6174 6141 7272  ther, xr.DataArr
+00012da0: 6179 293a 0a20 2020 2020 2020 2020 2020  ay):.           
+00012db0: 206f 7468 6572 5f76 616c 7320 3d20 6f74   other_vals = ot
+00012dc0: 6865 722e 7661 6c75 6573 0a20 2020 2020  her.values.     
+00012dd0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00012de0: 2020 2020 206f 7468 6572 5f76 616c 7320       other_vals 
+00012df0: 3d20 6f74 6865 720a 0a20 2020 2020 2020  = other..       
+00012e00: 2072 6169 7365 5f69 665f 6e6f 7428 7365   raise_if_not(se
+00012e10: 6c66 2e5f 7861 2e76 616c 7565 732e 7368  lf._xa.values.sh
+00012e20: 6170 6520 3d3d 206f 7468 6572 5f76 616c  ape == other_val
+00012e30: 732e 7368 6170 652c 2027 4174 7465 6d70  s.shape, 'Attemp
+00012e40: 7465 6420 746f 2070 6572 666f 726d 206f  ted to perform o
+00012e50: 7065 7261 7469 6f6e 206f 6e20 7477 6f20  peration on two 
+00012e60: 5469 6d65 5365 7269 6573 2027 0a20 2020  TimeSeries '.   
+00012e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ea0: 2020 2020 2020 2020 2020 2020 2027 6f66               'of
+00012eb0: 2075 6e65 7175 616c 2073 6861 7065 732e   unequal shapes.
+00012ec0: 272c 206c 6f67 6765 7229 0a20 2020 2020  ', logger).     
+00012ed0: 2020 206e 6577 5f78 6120 3d20 7365 6c66     new_xa = self
+00012ee0: 2e5f 7861 2e63 6f70 7928 290a 2020 2020  ._xa.copy().    
+00012ef0: 2020 2020 6e65 775f 7861 2e76 616c 7565      new_xa.value
+00012f00: 7320 3d20 636f 6d62 696e 655f 666e 286e  s = combine_fn(n
+00012f10: 6577 5f78 612e 7661 6c75 6573 2c20 6f74  ew_xa.values, ot
+00012f20: 6865 725f 7661 6c73 290a 2020 2020 2020  her_vals).      
+00012f30: 2020 7265 7475 726e 2054 696d 6553 6572    return TimeSer
+00012f40: 6965 7328 6e65 775f 7861 290a 0a20 2020  ies(new_xa)..   
+00012f50: 2064 6566 205f 5f65 715f 5f28 7365 6c66   def __eq__(self
+00012f60: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
+00012f70: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+00012f80: 6f74 6865 722c 2054 696d 6553 6572 6965  other, TimeSerie
+00012f90: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00012fa0: 7265 7475 726e 2073 656c 662e 5f78 612e  return self._xa.
+00012fb0: 6571 7561 6c73 286f 7468 6572 2e64 6174  equals(other.dat
+00012fc0: 615f 6172 7261 7928 636f 7079 3d46 616c  a_array(copy=Fal
+00012fd0: 7365 2929 0a20 2020 2020 2020 2072 6574  se)).        ret
+00012fe0: 7572 6e20 4661 6c73 650a 0a20 2020 2064  urn False..    d
+00012ff0: 6566 205f 5f6e 655f 5f28 7365 6c66 2c20  ef __ne__(self, 
+00013000: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
+00013010: 7265 7475 726e 206e 6f74 2073 656c 662e  return not self.
+00013020: 5f5f 6571 5f5f 286f 7468 6572 290a 0a20  __eq__(other).. 
+00013030: 2020 2064 6566 205f 5f6c 656e 5f5f 2873     def __len__(s
+00013040: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
+00013050: 7475 726e 206c 656e 2873 656c 662e 5f78  turn len(self._x
+00013060: 6129 0a0a 2020 2020 6465 6620 5f5f 6164  a)..    def __ad
+00013070: 645f 5f28 7365 6c66 2c20 6f74 6865 7229  d__(self, other)
+00013080: 3a0a 2020 2020 2020 2020 6966 2069 7369  :.        if isi
+00013090: 6e73 7461 6e63 6528 6f74 6865 722c 2028  nstance(other, (
+000130a0: 696e 742c 2066 6c6f 6174 2c20 6e70 2e69  int, float, np.i
+000130b0: 6e74 6567 6572 2929 3a0a 2020 2020 2020  nteger)):.      
+000130c0: 2020 2020 2020 7265 7475 726e 2054 696d        return Tim
+000130d0: 6553 6572 6965 7328 7365 6c66 2e5f 7861  eSeries(self._xa
+000130e0: 202b 206f 7468 6572 290a 2020 2020 2020   + other).      
+000130f0: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
+00013100: 6528 6f74 6865 722c 2028 5469 6d65 5365  e(other, (TimeSe
+00013110: 7269 6573 2c20 7872 2e44 6174 6141 7272  ries, xr.DataArr
+00013120: 6179 2c20 6e70 2e6e 6461 7272 6179 2929  ay, np.ndarray))
+00013130: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00013140: 7475 726e 2073 656c 662e 5f63 6f6d 6269  turn self._combi
+00013150: 6e65 5f61 7272 6179 7328 6f74 6865 722c  ne_arrays(other,
+00013160: 206c 616d 6264 6120 7331 2c20 7332 3a20   lambda s1, s2: 
+00013170: 7331 202b 2073 3229 0a20 2020 2020 2020  s1 + s2).       
+00013180: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00013190: 2020 2072 6169 7365 5f6c 6f67 2854 7970     raise_log(Typ
+000131a0: 6545 7272 6f72 2827 756e 7375 7070 6f72  eError('unsuppor
+000131b0: 7465 6420 6f70 6572 616e 6420 7479 7065  ted operand type
+000131c0: 2873 2920 666f 7220 2b20 6f72 2061 6464  (s) for + or add
+000131d0: 2829 3a20 5c27 7b7d 5c27 2061 6e64 205c  (): \'{}\' and \
+000131e0: 277b 7d5c 272e 270a 2020 2020 2020 2020  '{}\'.'.        
+000131f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013200: 2020 2020 2020 2020 2e66 6f72 6d61 7428          .format(
+00013210: 7479 7065 2873 656c 6629 2e5f 5f6e 616d  type(self).__nam
+00013220: 655f 5f2c 2074 7970 6528 6f74 6865 7229  e__, type(other)
+00013230: 2e5f 5f6e 616d 655f 5f29 292c 206c 6f67  .__name__)), log
+00013240: 6765 7229 0a0a 2020 2020 6465 6620 5f5f  ger)..    def __
+00013250: 7261 6464 5f5f 2873 656c 662c 206f 7468  radd__(self, oth
+00013260: 6572 293a 0a20 2020 2020 2020 2072 6574  er):.        ret
+00013270: 7572 6e20 7365 6c66 202b 206f 7468 6572  urn self + other
+00013280: 0a0a 2020 2020 6465 6620 5f5f 7375 625f  ..    def __sub_
+00013290: 5f28 7365 6c66 2c20 6f74 6865 7229 3a0a  _(self, other):.
+000132a0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+000132b0: 7461 6e63 6528 6f74 6865 722c 2028 696e  tance(other, (in
+000132c0: 742c 2066 6c6f 6174 2c20 6e70 2e69 6e74  t, float, np.int
+000132d0: 6567 6572 2929 3a0a 2020 2020 2020 2020  eger)):.        
+000132e0: 2020 2020 7265 7475 726e 2054 696d 6553      return TimeS
+000132f0: 6572 6965 7328 7365 6c66 2e5f 7861 202d  eries(self._xa -
+00013300: 206f 7468 6572 290a 2020 2020 2020 2020   other).        
+00013310: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
+00013320: 6f74 6865 722c 2028 5469 6d65 5365 7269  other, (TimeSeri
+00013330: 6573 2c20 7872 2e44 6174 6141 7272 6179  es, xr.DataArray
+00013340: 2c20 6e70 2e6e 6461 7272 6179 2929 3a0a  , np.ndarray)):.
+00013350: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00013360: 726e 2073 656c 662e 5f63 6f6d 6269 6e65  rn self._combine
+00013370: 5f61 7272 6179 7328 6f74 6865 722c 206c  _arrays(other, l
+00013380: 616d 6264 6120 7331 2c20 7332 3a20 7331  ambda s1, s2: s1
+00013390: 202d 2073 3229 0a20 2020 2020 2020 2065   - s2).        e
+000133a0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000133b0: 2072 6169 7365 5f6c 6f67 2854 7970 6545   raise_log(TypeE
+000133c0: 7272 6f72 2827 756e 7375 7070 6f72 7465  rror('unsupporte
+000133d0: 6420 6f70 6572 616e 6420 7479 7065 2873  d operand type(s
+000133e0: 2920 666f 7220 2d20 6f72 2073 7562 2829  ) for - or sub()
+000133f0: 3a20 5c27 7b7d 5c27 2061 6e64 205c 277b  : \'{}\' and \'{
+00013400: 7d5c 272e 270a 2020 2020 2020 2020 2020  }\'.'.          
+00013410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013420: 2020 2020 2020 2e66 6f72 6d61 7428 7479        .format(ty
+00013430: 7065 2873 656c 6629 2e5f 5f6e 616d 655f  pe(self).__name_
+00013440: 5f2c 2074 7970 6528 6f74 6865 7229 2e5f  _, type(other)._
+00013450: 5f6e 616d 655f 5f29 292c 206c 6f67 6765  _name__)), logge
+00013460: 7229 0a0a 2020 2020 6465 6620 5f5f 7273  r)..    def __rs
+00013470: 7562 5f5f 2873 656c 662c 206f 7468 6572  ub__(self, other
+00013480: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+00013490: 6e20 6f74 6865 7220 2b20 282d 7365 6c66  n other + (-self
+000134a0: 290a 0a20 2020 2064 6566 205f 5f6d 756c  )..    def __mul
+000134b0: 5f5f 2873 656c 662c 206f 7468 6572 293a  __(self, other):
+000134c0: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+000134d0: 7374 616e 6365 286f 7468 6572 2c20 2869  stance(other, (i
+000134e0: 6e74 2c20 666c 6f61 742c 206e 702e 696e  nt, float, np.in
+000134f0: 7465 6765 7229 293a 0a20 2020 2020 2020  teger)):.       
+00013500: 2020 2020 2072 6574 7572 6e20 5469 6d65       return Time
+00013510: 5365 7269 6573 2873 656c 662e 5f78 6120  Series(self._xa 
+00013520: 2a20 6f74 6865 7229 0a20 2020 2020 2020  * other).       
+00013530: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+00013540: 286f 7468 6572 2c20 2854 696d 6553 6572  (other, (TimeSer
+00013550: 6965 732c 2078 722e 4461 7461 4172 7261  ies, xr.DataArra
+00013560: 792c 206e 702e 6e64 6172 7261 7929 293a  y, np.ndarray)):
+00013570: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00013580: 7572 6e20 7365 6c66 2e5f 636f 6d62 696e  urn self._combin
+00013590: 655f 6172 7261 7973 286f 7468 6572 2c20  e_arrays(other, 
+000135a0: 6c61 6d62 6461 2073 312c 2073 323a 2073  lambda s1, s2: s
+000135b0: 3120 2a20 7332 290a 2020 2020 2020 2020  1 * s2).        
+000135c0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000135d0: 2020 7261 6973 655f 6c6f 6728 5479 7065    raise_log(Type
+000135e0: 4572 726f 7228 2775 6e73 7570 706f 7274  Error('unsupport
+000135f0: 6564 206f 7065 7261 6e64 2074 7970 6528  ed operand type(
+00013600: 7329 2066 6f72 202a 206f 7220 6d75 6c28  s) for * or mul(
+00013610: 293a 205c 277b 7d5c 2720 616e 6420 5c27  ): \'{}\' and \'
+00013620: 7b7d 5c27 2e27 0a20 2020 2020 2020 2020  {}\'.'.         
+00013630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013640: 2020 2020 2020 202e 666f 726d 6174 2874         .format(t
+00013650: 7970 6528 7365 6c66 292e 5f5f 6e61 6d65  ype(self).__name
+00013660: 5f5f 2c20 7479 7065 286f 7468 6572 292e  __, type(other).
+00013670: 5f5f 6e61 6d65 5f5f 2929 2c20 6c6f 6767  __name__)), logg
+00013680: 6572 290a 0a20 2020 2064 6566 205f 5f72  er)..    def __r
+00013690: 6d75 6c5f 5f28 7365 6c66 2c20 6f74 6865  mul__(self, othe
+000136a0: 7229 3a0a 2020 2020 2020 2020 7265 7475  r):.        retu
+000136b0: 726e 2073 656c 6620 2a20 6f74 6865 720a  rn self * other.
+000136c0: 0a20 2020 2064 6566 205f 5f70 6f77 5f5f  .    def __pow__
+000136d0: 2873 656c 662c 206e 293a 0a20 2020 2020  (self, n):.     
+000136e0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+000136f0: 286e 2c20 2869 6e74 2c20 666c 6f61 742c  (n, (int, float,
+00013700: 206e 702e 696e 7465 6765 7229 293a 0a20   np.integer)):. 
+00013710: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00013720: 5f69 6628 6e20 3c20 302c 2027 4174 7465  _if(n < 0, 'Atte
+00013730: 6d70 7465 6420 746f 2072 6169 7365 2061  mpted to raise a
+00013740: 2073 6572 6965 7320 746f 2061 206e 6567   series to a neg
+00013750: 6174 6976 6520 706f 7765 722e 272c 206c  ative power.', l
+00013760: 6f67 6765 7229 0a20 2020 2020 2020 2020  ogger).         
+00013770: 2020 2072 6574 7572 6e20 5469 6d65 5365     return TimeSe
+00013780: 7269 6573 2873 656c 662e 5f78 6120 2a2a  ries(self._xa **
+00013790: 2066 6c6f 6174 286e 2929 0a20 2020 2020   float(n)).     
+000137a0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+000137b0: 286e 2c20 2854 696d 6553 6572 6965 732c  (n, (TimeSeries,
+000137c0: 2078 722e 4461 7461 4172 7261 792c 206e   xr.DataArray, n
+000137d0: 702e 6e64 6172 7261 7929 293a 0a20 2020  p.ndarray)):.   
+000137e0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000137f0: 7365 6c66 2e5f 636f 6d62 696e 655f 6172  self._combine_ar
+00013800: 7261 7973 286e 2c20 6c61 6d62 6461 2073  rays(n, lambda s
+00013810: 312c 2073 323a 2073 3120 2a2a 2073 3229  1, s2: s1 ** s2)
+00013820: 2020 2320 656c 656d 656e 7477 6973 6520    # elementwise 
+00013830: 706f 7765 720a 2020 2020 2020 2020 656c  power.        el
+00013840: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00013850: 7261 6973 655f 6c6f 6728 5479 7065 4572  raise_log(TypeEr
+00013860: 726f 7228 2775 6e73 7570 706f 7274 6564  ror('unsupported
+00013870: 206f 7065 7261 6e64 2074 7970 6528 7329   operand type(s)
+00013880: 2066 6f72 202a 2a20 6f72 2070 6f77 2829   for ** or pow()
+00013890: 3a20 5c27 7b7d 5c27 2061 6e64 205c 277b  : \'{}\' and \'{
+000138a0: 7d5c 272e 270a 2020 2020 2020 2020 2020  }\'.'.          
+000138b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000138c0: 2020 2020 2020 2e66 6f72 6d61 7428 7479        .format(ty
+000138d0: 7065 2873 656c 6629 2e5f 5f6e 616d 655f  pe(self).__name_
+000138e0: 5f2c 2074 7970 6528 6e29 2e5f 5f6e 616d  _, type(n).__nam
+000138f0: 655f 5f29 292c 206c 6f67 6765 7229 0a0a  e__)), logger)..
+00013900: 2020 2020 6465 6620 5f5f 7472 7565 6469      def __truedi
+00013910: 765f 5f28 7365 6c66 2c20 6f74 6865 7229  v__(self, other)
+00013920: 3a0a 2020 2020 2020 2020 6966 2069 7369  :.        if isi
+00013930: 6e73 7461 6e63 6528 6f74 6865 722c 2028  nstance(other, (
+00013940: 696e 742c 2066 6c6f 6174 2c20 6e70 2e69  int, float, np.i
+00013950: 6e74 6567 6572 2929 3a0a 2020 2020 2020  nteger)):.      
+00013960: 2020 2020 2020 6966 206f 7468 6572 203d        if other =
+00013970: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+00013980: 2020 2020 2072 6169 7365 5f6c 6f67 285a       raise_log(Z
+00013990: 6572 6f44 6976 6973 696f 6e45 7272 6f72  eroDivisionError
+000139a0: 2827 4361 6e6e 6f74 2064 6976 6964 6520  ('Cannot divide 
+000139b0: 6279 2030 2e27 292c 206c 6f67 6765 7229  by 0.'), logger)
+000139c0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000139d0: 7572 6e20 5469 6d65 5365 7269 6573 2873  urn TimeSeries(s
+000139e0: 656c 662e 5f78 6120 2f20 6f74 6865 7229  elf._xa / other)
+000139f0: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
+00013a00: 696e 7374 616e 6365 286f 7468 6572 2c20  instance(other, 
+00013a10: 2854 696d 6553 6572 6965 732c 2078 722e  (TimeSeries, xr.
+00013a20: 4461 7461 4172 7261 792c 206e 702e 6e64  DataArray, np.nd
+00013a30: 6172 7261 7929 293a 0a20 2020 2020 2020  array)):.       
+00013a40: 2020 2020 2069 6620 6e6f 7420 286f 7468       if not (oth
+00013a50: 6572 2e61 6c6c 5f76 616c 7565 7328 2920  er.all_values() 
+00013a60: 213d 2030 292e 616c 6c28 293a 0a20 2020  != 0).all():.   
+00013a70: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00013a80: 7365 5f6c 6f67 285a 6572 6f44 6976 6973  se_log(ZeroDivis
+00013a90: 696f 6e45 7272 6f72 2827 4361 6e6e 6f74  ionError('Cannot
+00013aa0: 2064 6976 6964 6520 6279 2061 2054 696d   divide by a Tim
+00013ab0: 6553 6572 6965 7320 7769 7468 2061 2076  eSeries with a v
+00013ac0: 616c 7565 2030 2e27 292c 206c 6f67 6765  alue 0.'), logge
+00013ad0: 7229 0a20 2020 2020 2020 2020 2020 2072  r).            r
+00013ae0: 6574 7572 6e20 7365 6c66 2e5f 636f 6d62  eturn self._comb
+00013af0: 696e 655f 6172 7261 7973 286f 7468 6572  ine_arrays(other
+00013b00: 2c20 6c61 6d62 6461 2073 312c 2073 323a  , lambda s1, s2:
+00013b10: 2073 3120 2f20 7332 290a 2020 2020 2020   s1 / s2).      
+00013b20: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00013b30: 2020 2020 7261 6973 655f 6c6f 6728 5479      raise_log(Ty
+00013b40: 7065 4572 726f 7228 2775 6e73 7570 706f  peError('unsuppo
+00013b50: 7274 6564 206f 7065 7261 6e64 2074 7970  rted operand typ
+00013b60: 6528 7329 2066 6f72 202f 206f 7220 7472  e(s) for / or tr
+00013b70: 7565 6469 7628 293a 205c 277b 7d5c 2720  uediv(): \'{}\' 
+00013b80: 616e 6420 5c27 7b7d 5c27 2e27 0a20 2020  and \'{}\'.'.   
+00013b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ba0: 2020 2020 2020 2020 2020 2020 202e 666f               .fo
+00013bb0: 726d 6174 2874 7970 6528 7365 6c66 292e  rmat(type(self).
+00013bc0: 5f5f 6e61 6d65 5f5f 2c20 7479 7065 286f  __name__, type(o
+00013bd0: 7468 6572 292e 5f5f 6e61 6d65 5f5f 2929  ther).__name__))
+00013be0: 2c20 6c6f 6767 6572 290a 0a20 2020 2064  , logger)..    d
+00013bf0: 6566 205f 5f72 7472 7565 6469 765f 5f28  ef __rtruediv__(
+00013c00: 7365 6c66 2c20 6e29 3a0a 2020 2020 2020  self, n):.      
+00013c10: 2020 7265 7475 726e 206e 202a 2028 7365    return n * (se
+00013c20: 6c66 202a 2a20 282d 3129 290a 0a20 2020  lf ** (-1))..   
+00013c30: 2064 6566 205f 5f61 6273 5f5f 2873 656c   def __abs__(sel
+00013c40: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
+00013c50: 726e 2054 696d 6553 6572 6965 7328 6162  rn TimeSeries(ab
+00013c60: 7328 7365 6c66 2e5f 7861 2929 0a0a 2020  s(self._xa))..  
+00013c70: 2020 6465 6620 5f5f 6e65 675f 5f28 7365    def __neg__(se
+00013c80: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
+00013c90: 7572 6e20 5469 6d65 5365 7269 6573 282d  urn TimeSeries(-
+00013ca0: 7365 6c66 2e5f 7861 290a 0a20 2020 2064  self._xa)..    d
+00013cb0: 6566 205f 5f63 6f6e 7461 696e 735f 5f28  ef __contains__(
+00013cc0: 7365 6c66 2c20 7473 3a20 556e 696f 6e5b  self, ts: Union[
+00013cd0: 696e 742c 2070 642e 5469 6d65 7374 616d  int, pd.Timestam
+00013ce0: 705d 2920 2d3e 2062 6f6f 6c3a 0a20 2020  p]) -> bool:.   
+00013cf0: 2020 2020 2072 6574 7572 6e20 7473 2069       return ts i
+00013d00: 6e20 7365 6c66 2e74 696d 655f 696e 6465  n self.time_inde
+00013d10: 780a 0a20 2020 2064 6566 205f 5f72 6f75  x..    def __rou
+00013d20: 6e64 5f5f 2873 656c 662c 206e 3d4e 6f6e  nd__(self, n=Non
+00013d30: 6529 3a0a 2020 2020 2020 2020 7265 7475  e):.        retu
+00013d40: 726e 2054 696d 6553 6572 6965 7328 7365  rn TimeSeries(se
+00013d50: 6c66 2e5f 7861 2e72 6f75 6e64 286e 2929  lf._xa.round(n))
+00013d60: 0a0a 2020 2020 6465 6620 5f5f 6c74 5f5f  ..    def __lt__
+00013d70: 2873 656c 662c 206f 7468 6572 2920 2d3e  (self, other) ->
+00013d80: 2078 722e 4461 7461 4172 7261 793a 0a20   xr.DataArray:. 
+00013d90: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00013da0: 616e 6365 286f 7468 6572 2c20 2869 6e74  ance(other, (int
+00013db0: 2c20 666c 6f61 742c 206e 702e 696e 7465  , float, np.inte
+00013dc0: 6765 722c 206e 702e 6e64 6172 7261 792c  ger, np.ndarray,
+00013dd0: 2078 722e 4461 7461 4172 7261 7929 293a   xr.DataArray)):
+00013de0: 0a20 2020 2020 2020 2020 2020 2073 6572  .            ser
+00013df0: 6965 7320 3d20 7365 6c66 2e5f 7861 203c  ies = self._xa <
+00013e00: 206f 7468 6572 0a20 2020 2020 2020 2065   other.        e
+00013e10: 6c69 6620 6973 696e 7374 616e 6365 286f  lif isinstance(o
+00013e20: 7468 6572 2c20 5469 6d65 5365 7269 6573  ther, TimeSeries
+00013e30: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+00013e40: 6572 6965 7320 3d20 7365 6c66 2e5f 7861  eries = self._xa
+00013e50: 203c 206f 7468 6572 2e64 6174 615f 6172   < other.data_ar
+00013e60: 7261 7928 636f 7079 3d46 616c 7365 290a  ray(copy=False).
+00013e70: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00013e80: 2020 2020 2020 2020 2020 7261 6973 655f            raise_
+00013e90: 6c6f 6728 5479 7065 4572 726f 7228 2775  log(TypeError('u
+00013ea0: 6e73 7570 706f 7274 6564 206f 7065 7261  nsupported opera
+00013eb0: 6e64 2074 7970 6528 7329 2066 6f72 203c  nd type(s) for <
+00013ec0: 203a 205c 277b 7d5c 2720 616e 6420 5c27   : \'{}\' and \'
+00013ed0: 7b7d 5c27 2e27 0a20 2020 2020 2020 2020  {}\'.'.         
+00013ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ef0: 2020 2020 2020 202e 666f 726d 6174 2874         .format(t
+00013f00: 7970 6528 7365 6c66 292e 5f5f 6e61 6d65  ype(self).__name
+00013f10: 5f5f 2c20 7479 7065 286f 7468 6572 292e  __, type(other).
+00013f20: 5f5f 6e61 6d65 5f5f 2929 2c20 6c6f 6767  __name__)), logg
+00013f30: 6572 290a 2020 2020 2020 2020 7265 7475  er).        retu
+00013f40: 726e 2073 6572 6965 7320 2023 204e 6f74  rn series  # Not
+00013f50: 653a 2077 6520 7265 7475 726e 2061 2044  e: we return a D
+00013f60: 6174 6141 7272 6179 0a0a 2020 2020 6465  ataArray..    de
+00013f70: 6620 5f5f 6774 5f5f 2873 656c 662c 206f  f __gt__(self, o
+00013f80: 7468 6572 2920 2d3e 2078 722e 4461 7461  ther) -> xr.Data
+00013f90: 4172 7261 793a 0a20 2020 2020 2020 2069  Array:.        i
+00013fa0: 6620 6973 696e 7374 616e 6365 286f 7468  f isinstance(oth
+00013fb0: 6572 2c20 2869 6e74 2c20 666c 6f61 742c  er, (int, float,
+00013fc0: 206e 702e 696e 7465 6765 722c 206e 702e   np.integer, np.
+00013fd0: 6e64 6172 7261 792c 2078 722e 4461 7461  ndarray, xr.Data
+00013fe0: 4172 7261 7929 293a 0a20 2020 2020 2020  Array)):.       
+00013ff0: 2020 2020 2073 6572 6965 7320 3d20 7365       series = se
+00014000: 6c66 2e5f 7861 203e 206f 7468 6572 0a20  lf._xa > other. 
+00014010: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
+00014020: 7374 616e 6365 286f 7468 6572 2c20 5469  stance(other, Ti
+00014030: 6d65 5365 7269 6573 293a 0a20 2020 2020  meSeries):.     
+00014040: 2020 2020 2020 2073 6572 6965 7320 3d20         series = 
+00014050: 7365 6c66 2e5f 7861 203e 206f 7468 6572  self._xa > other
+00014060: 2e64 6174 615f 6172 7261 7928 636f 7079  .data_array(copy
+00014070: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
+00014080: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00014090: 2020 7365 7269 6573 203d 204e 6f6e 650a    series = None.
+000140a0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+000140b0: 655f 6c6f 6728 5479 7065 4572 726f 7228  e_log(TypeError(
+000140c0: 2775 6e73 7570 706f 7274 6564 206f 7065  'unsupported ope
+000140d0: 7261 6e64 2074 7970 6528 7329 2066 6f72  rand type(s) for
+000140e0: 203c 203a 205c 277b 7d5c 2720 616e 6420   < : \'{}\' and 
+000140f0: 5c27 7b7d 5c27 2e27 0a20 2020 2020 2020  \'{}\'.'.       
+00014100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014110: 2020 2020 2020 2020 202e 666f 726d 6174           .format
+00014120: 2874 7970 6528 7365 6c66 292e 5f5f 6e61  (type(self).__na
+00014130: 6d65 5f5f 2c20 7479 7065 286f 7468 6572  me__, type(other
+00014140: 292e 5f5f 6e61 6d65 5f5f 2929 2c20 6c6f  ).__name__)), lo
+00014150: 6767 6572 290a 2020 2020 2020 2020 7265  gger).        re
+00014160: 7475 726e 2073 6572 6965 7320 2023 204e  turn series  # N
+00014170: 6f74 653a 2077 6520 7265 7475 726e 2061  ote: we return a
+00014180: 2044 6174 6141 7272 6179 0a0a 2020 2020   DataArray..    
+00014190: 6465 6620 5f5f 6c65 5f5f 2873 656c 662c  def __le__(self,
+000141a0: 206f 7468 6572 2920 2d3e 2078 722e 4461   other) -> xr.Da
+000141b0: 7461 4172 7261 793a 0a20 2020 2020 2020  taArray:.       
+000141c0: 2069 6620 6973 696e 7374 616e 6365 286f   if isinstance(o
+000141d0: 7468 6572 2c20 2869 6e74 2c20 666c 6f61  ther, (int, floa
+000141e0: 742c 206e 702e 696e 7465 6765 722c 206e  t, np.integer, n
+000141f0: 702e 6e64 6172 7261 792c 2078 722e 4461  p.ndarray, xr.Da
+00014200: 7461 4172 7261 7929 293a 0a20 2020 2020  taArray)):.     
+00014210: 2020 2020 2020 2073 6572 6965 7320 3d20         series = 
+00014220: 7365 6c66 2e5f 7861 203c 3d20 6f74 6865  self._xa <= othe
+00014230: 720a 2020 2020 2020 2020 656c 6966 2069  r.        elif i
+00014240: 7369 6e73 7461 6e63 6528 6f74 6865 722c  sinstance(other,
+00014250: 2054 696d 6553 6572 6965 7329 3a0a 2020   TimeSeries):.  
+00014260: 2020 2020 2020 2020 2020 7365 7269 6573            series
+00014270: 203d 2073 656c 662e 5f78 6120 3c3d 206f   = self._xa <= o
+00014280: 7468 6572 2e64 6174 615f 6172 7261 7928  ther.data_array(
+00014290: 636f 7079 3d46 616c 7365 290a 2020 2020  copy=False).    
+000142a0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000142b0: 2020 2020 2020 7365 7269 6573 203d 204e        series = N
+000142c0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+000142d0: 7261 6973 655f 6c6f 6728 5479 7065 4572  raise_log(TypeEr
+000142e0: 726f 7228 2775 6e73 7570 706f 7274 6564  ror('unsupported
+000142f0: 206f 7065 7261 6e64 2074 7970 6528 7329   operand type(s)
+00014300: 2066 6f72 203c 203a 205c 277b 7d5c 2720   for < : \'{}\' 
+00014310: 616e 6420 5c27 7b7d 5c27 2e27 0a20 2020  and \'{}\'.'.   
+00014320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014330: 2020 2020 2020 2020 2020 2020 202e 666f               .fo
+00014340: 726d 6174 2874 7970 6528 7365 6c66 292e  rmat(type(self).
+00014350: 5f5f 6e61 6d65 5f5f 2c20 7479 7065 286f  __name__, type(o
+00014360: 7468 6572 292e 5f5f 6e61 6d65 5f5f 2929  ther).__name__))
+00014370: 2c20 6c6f 6767 6572 290a 2020 2020 2020  , logger).      
+00014380: 2020 7265 7475 726e 2073 6572 6965 7320    return series 
+00014390: 2023 204e 6f74 653a 2077 6520 7265 7475   # Note: we retu
+000143a0: 726e 2061 2044 6174 6141 7272 6179 0a0a  rn a DataArray..
+000143b0: 2020 2020 6465 6620 5f5f 6765 5f5f 2873      def __ge__(s
+000143c0: 656c 662c 206f 7468 6572 2920 2d3e 2078  elf, other) -> x
+000143d0: 722e 4461 7461 4172 7261 793a 0a20 2020  r.DataArray:.   
+000143e0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+000143f0: 6365 286f 7468 6572 2c20 2869 6e74 2c20  ce(other, (int, 
+00014400: 666c 6f61 742c 206e 702e 696e 7465 6765  float, np.intege
+00014410: 722c 206e 702e 6e64 6172 7261 792c 2078  r, np.ndarray, x
+00014420: 722e 4461 7461 4172 7261 7929 293a 0a20  r.DataArray)):. 
+00014430: 2020 2020 2020 2020 2020 2073 6572 6965             serie
+00014440: 7320 3d20 7365 6c66 2e5f 7861 203e 3d20  s = self._xa >= 
+00014450: 6f74 6865 720a 2020 2020 2020 2020 656c  other.        el
+00014460: 6966 2069 7369 6e73 7461 6e63 6528 6f74  if isinstance(ot
+00014470: 6865 722c 2054 696d 6553 6572 6965 7329  her, TimeSeries)
+00014480: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00014490: 7269 6573 203d 2073 656c 662e 5f78 6120  ries = self._xa 
+000144a0: 3e3d 206f 7468 6572 2e64 6174 615f 6172  >= other.data_ar
+000144b0: 7261 7928 636f 7079 3d46 616c 7365 290a  ray(copy=False).
+000144c0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000144d0: 2020 2020 2020 2020 2020 7365 7269 6573            series
+000144e0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+000144f0: 2020 2020 7261 6973 655f 6c6f 6728 5479      raise_log(Ty
+00014500: 7065 4572 726f 7228 2775 6e73 7570 706f  peError('unsuppo
+00014510: 7274 6564 206f 7065 7261 6e64 2074 7970  rted operand typ
+00014520: 6528 7329 2066 6f72 203c 203a 205c 277b  e(s) for < : \'{
+00014530: 7d5c 2720 616e 6420 5c27 7b7d 5c27 2e27  }\' and \'{}\'.'
+00014540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014560: 202e 666f 726d 6174 2874 7970 6528 7365   .format(type(se
+00014570: 6c66 292e 5f5f 6e61 6d65 5f5f 2c20 7479  lf).__name__, ty
+00014580: 7065 286f 7468 6572 292e 5f5f 6e61 6d65  pe(other).__name
+00014590: 5f5f 2929 2c20 6c6f 6767 6572 290a 2020  __)), logger).  
+000145a0: 2020 2020 2020 7265 7475 726e 2073 6572        return ser
+000145b0: 6965 7320 2023 204e 6f74 653a 2077 6520  ies  # Note: we 
+000145c0: 7265 7475 726e 2061 2044 6174 6141 7272  return a DataArr
+000145d0: 6179 0a0a 2020 2020 6465 6620 5f5f 7374  ay..    def __st
+000145e0: 725f 5f28 7365 6c66 293a 0a20 2020 2020  r__(self):.     
+000145f0: 2020 2072 6574 7572 6e20 7374 7228 7365     return str(se
+00014600: 6c66 2e5f 7861 292e 7265 706c 6163 6528  lf._xa).replace(
+00014610: 2778 6172 7261 792e 4461 7461 4172 7261  'xarray.DataArra
+00014620: 7927 2c20 2754 696d 6553 6572 6965 7320  y', 'TimeSeries 
+00014630: 2844 6174 6141 7272 6179 2927 290a 0a20  (DataArray)').. 
+00014640: 2020 2064 6566 205f 5f72 6570 725f 5f28     def __repr__(
+00014650: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
+00014660: 6574 7572 6e20 7365 6c66 2e5f 7861 2e5f  eturn self._xa._
+00014670: 5f72 6570 725f 5f28 292e 7265 706c 6163  _repr__().replac
+00014680: 6528 2778 6172 7261 792e 4461 7461 4172  e('xarray.DataAr
+00014690: 7261 7927 2c20 2754 696d 6553 6572 6965  ray', 'TimeSerie
+000146a0: 7320 2844 6174 6141 7272 6179 2927 290a  s (DataArray)').
+000146b0: 0a20 2020 2064 6566 205f 7265 7072 5f68  .    def _repr_h
+000146c0: 746d 6c5f 2873 656c 6629 3a0a 2020 2020  tml_(self):.    
+000146d0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000146e0: 5f78 612e 5f72 6570 725f 6874 6d6c 5f28  _xa._repr_html_(
+000146f0: 292e 7265 706c 6163 6528 2778 6172 7261  ).replace('xarra
+00014700: 792e 4461 7461 4172 7261 7927 2c20 2754  y.DataArray', 'T
+00014710: 696d 6553 6572 6965 7320 2844 6174 6141  imeSeries (DataA
+00014720: 7272 6179 2927 290a 0a20 2020 2064 6566  rray)')..    def
+00014730: 205f 5f63 6f70 795f 5f28 7365 6c66 2c20   __copy__(self, 
+00014740: 6465 6570 3a20 626f 6f6c 203d 2054 7275  deep: bool = Tru
+00014750: 6529 3a0a 2020 2020 2020 2020 7265 7475  e):.        retu
+00014760: 726e 2073 656c 662e 636f 7079 2829 0a0a  rn self.copy()..
+00014770: 2020 2020 6465 6620 5f5f 6465 6570 636f      def __deepco
+00014780: 7079 5f5f 2873 656c 6629 3a0a 2020 2020  py__(self):.    
+00014790: 2020 2020 7265 7475 726e 2054 696d 6553      return TimeS
+000147a0: 6572 6965 7328 7365 6c66 2e5f 7861 2e63  eries(self._xa.c
+000147b0: 6f70 7928 2929 0a0a 2020 2020 6465 6620  opy())..    def 
+000147c0: 5f5f 6765 7469 7465 6d5f 5f28 7365 6c66  __getitem__(self
+000147d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000147e0: 2020 2020 2020 6b65 793a 2055 6e69 6f6e        key: Union
+000147f0: 5b70 642e 4461 7465 7469 6d65 496e 6465  [pd.DatetimeInde
+00014800: 782c 0a20 2020 2020 2020 2020 2020 2020  x,.             
+00014810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014820: 2020 7064 2e49 6e74 3634 496e 6465 782c    pd.Int64Index,
+00014830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014850: 4c69 7374 5b73 7472 5d2c 0a20 2020 2020  List[str],.     
+00014860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014870: 2020 2020 2020 2020 2020 4c69 7374 5b69            List[i
+00014880: 6e74 5d2c 0a20 2020 2020 2020 2020 2020  nt],.           
+00014890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000148a0: 2020 2020 4c69 7374 5b70 642e 5469 6d65      List[pd.Time
+000148b0: 7374 616d 705d 2c0a 2020 2020 2020 2020  stamp],.        
+000148c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000148d0: 2020 2020 2020 2073 7472 2c0a 2020 2020         str,.    
+000148e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000148f0: 2020 2020 2020 2020 2020 2069 6e74 2c0a             int,.
+00014900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014910: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00014920: 642e 5469 6d65 7374 616d 702c 0a20 2020  d.Timestamp,.   
+00014930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014940: 2020 2020 2020 2020 2020 2020 416e 795d              Any]
+00014950: 2920 2d3e 2027 5469 6d65 5365 7269 6573  ) -> 'TimeSeries
+00014960: 273a 0a20 2020 2020 2020 2022 2222 416c  ':.        """Al
+00014970: 6c6f 7720 696e 6465 7869 6e67 206f 6e20  low indexing on 
+00014980: 6461 7274 7320 5469 6d65 5365 7269 6573  darts TimeSeries
+00014990: 2e0a 0a20 2020 2020 2020 2054 6865 2073  ...        The s
+000149a0: 7570 706f 7274 6564 2069 6e64 6578 2074  upported index t
+000149b0: 7970 6573 2061 7265 2074 6865 2066 6f6c  ypes are the fol
+000149c0: 6c6f 7769 6e67 2062 6173 6520 7479 7065  lowing base type
+000149d0: 7320 6173 2061 2073 696e 676c 6520 7661  s as a single va
+000149e0: 6c75 652c 2061 206c 6973 7420 6f72 2061  lue, a list or a
+000149f0: 2073 6c69 6365 3a0a 2020 2020 2020 2020   slice:.        
+00014a00: 2d20 7064 2e54 696d 6573 7461 6d70 202d  - pd.Timestamp -
+00014a10: 3e20 7265 7475 726e 2061 2054 696d 6553  > return a TimeS
+00014a20: 6572 6965 7320 636f 7272 6573 706f 6e64  eries correspond
+00014a30: 696e 6720 746f 2074 6865 2076 616c 7565  ing to the value
+00014a40: 2873 2920 6174 2074 6865 2067 6976 656e  (s) at the given
+00014a50: 2074 696d 6573 7461 6d70 2873 292e 0a20   timestamp(s).. 
+00014a60: 2020 2020 2020 202d 2073 7472 202d 3e20         - str -> 
+00014a70: 7265 7475 726e 2061 2054 696d 6553 6572  return a TimeSer
+00014a80: 6965 7320 696e 636c 7564 696e 6720 7468  ies including th
+00014a90: 6520 636f 6c75 6d6e 2873 2920 2863 6f6d  e column(s) (com
+00014aa0: 706f 6e65 6e74 7329 2073 7065 6369 6669  ponents) specifi
+00014ab0: 6564 2061 7320 7374 722e 0a20 2020 2020  ed as str..     
+00014ac0: 2020 202d 2069 6e74 202d 3e20 7265 7475     - int -> retu
+00014ad0: 726e 2061 2054 696d 6553 6572 6965 7320  rn a TimeSeries 
+00014ae0: 7769 7468 2074 6865 2076 616c 7565 2873  with the value(s
+00014af0: 2920 6174 2074 6865 2067 6976 656e 2072  ) at the given r
+00014b00: 6f77 2028 7469 6d65 2920 696e 6465 782e  ow (time) index.
+00014b10: 0a0a 2020 2020 2020 2020 6070 642e 4461  ..        `pd.Da
+00014b20: 7465 7469 6d65 496e 6465 7860 2061 6e64  tetimeIndex` and
+00014b30: 2060 7064 2e49 6e74 3634 496e 6465 7860   `pd.Int64Index`
+00014b40: 2061 7265 2061 6c73 6f20 7375 7070 6f72   are also suppor
+00014b50: 7465 6420 616e 6420 7769 6c6c 2072 6574  ted and will ret
+00014b60: 7572 6e20 7468 6520 636f 7272 6573 706f  urn the correspo
+00014b70: 6e64 696e 6720 7661 6c75 6528 7329 0a20  nding value(s). 
+00014b80: 2020 2020 2020 2061 7420 7468 6520 7072         at the pr
+00014b90: 6f76 6964 6564 2074 696d 6520 696e 6469  ovided time indi
+00014ba0: 6365 732e 0a0a 2020 2020 2020 2020 2e2e  ces...        ..
+00014bb0: 2077 6172 6e69 6e67 3a3a 0a20 2020 2020   warning::.     
+00014bc0: 2020 2020 2020 2073 6c69 6365 7320 7573         slices us
+00014bd0: 6520 7061 6e64 6173 2063 6f6e 7665 6e74  e pandas convent
+00014be0: 696f 6e20 6f66 2069 6e63 6c75 6469 6e67  ion of including
+00014bf0: 2062 6f74 6820 656e 6473 206f 6620 7468   both ends of th
+00014c00: 6520 736c 6963 652e 0a20 2020 2020 2020  e slice..       
+00014c10: 2022 2222 0a20 2020 2020 2020 2064 6566   """.        def
+00014c20: 205f 6368 6563 6b5f 6474 2829 3a0a 2020   _check_dt():.  
+00014c30: 2020 2020 2020 2020 2020 7261 6973 655f            raise_
+00014c40: 6966 5f6e 6f74 2873 656c 662e 5f68 6173  if_not(self._has
+00014c50: 5f64 6174 6574 696d 655f 696e 6465 782c  _datetime_index,
+00014c60: 2027 4174 7465 6d70 7465 6420 696e 6465   'Attempted inde
+00014c70: 7869 6e67 2061 2073 6572 6965 7320 7769  xing a series wi
+00014c80: 7468 2061 2044 6174 6574 696d 6549 6e64  th a DatetimeInd
+00014c90: 6578 206f 7220 6120 7469 6d65 7374 616d  ex or a timestam
+00014ca0: 702c 2027 0a20 2020 2020 2020 2020 2020  p, '.           
+00014cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014cd0: 2020 2020 2020 2020 2762 7574 2074 6865          'but the
+00014ce0: 2073 6572 6965 7320 7573 6573 2061 6e20   series uses an 
+00014cf0: 496e 7436 3449 6e64 6578 2e27 2c20 6c6f  Int64Index.', lo
+00014d00: 6767 6572 290a 0a20 2020 2020 2020 2064  gger)..        d
+00014d10: 6566 205f 6368 6563 6b5f 7261 6e67 6528  ef _check_range(
+00014d20: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+00014d30: 6169 7365 5f69 6628 7365 6c66 2e5f 6861  aise_if(self._ha
+00014d40: 735f 6461 7465 7469 6d65 5f69 6e64 6578  s_datetime_index
+00014d50: 2c20 2741 7474 656d 7074 6564 2069 6e64  , 'Attempted ind
+00014d60: 6578 696e 6720 6120 7365 7269 6573 2077  exing a series w
+00014d70: 6974 6820 616e 2049 6e74 3634 496e 6465  ith an Int64Inde
+00014d80: 782c 2027 0a20 2020 2020 2020 2020 2020  x, '.           
+00014d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014db0: 2020 2020 2762 7574 2074 6865 2073 6572      'but the ser
+00014dc0: 6965 7320 7573 6573 2061 2044 6174 6574  ies uses a Datet
+00014dd0: 696d 6549 6e64 6578 2e27 2c20 6c6f 6767  imeIndex.', logg
+00014de0: 6572 290a 0a20 2020 2020 2020 2064 6566  er)..        def
+00014df0: 205f 7365 745f 6672 6571 5f69 6e5f 7861   _set_freq_in_xa
+00014e00: 2878 615f 3a20 7872 2e44 6174 6141 7272  (xa_: xr.DataArr
+00014e10: 6179 293a 0a20 2020 2020 2020 2020 2020  ay):.           
+00014e20: 2023 206d 7574 6174 6573 2074 6865 2044   # mutates the D
+00014e30: 6174 6141 7272 6179 2074 6f20 6d61 6b65  ataArray to make
+00014e40: 2073 7572 6520 6974 2063 6f6e 7461 696e   sure it contain
+00014e50: 7320 7468 6520 6672 6571 0a20 2020 2020  s the freq.     
+00014e60: 2020 2020 2020 2069 6e66 6572 7265 645f         inferred_
+00014e70: 6672 6571 203d 2078 615f 2e67 6574 5f69  freq = xa_.get_i
+00014e80: 6e64 6578 2873 656c 662e 5f74 696d 655f  ndex(self._time_
+00014e90: 6469 6d29 2e69 6e66 6572 7265 645f 6672  dim).inferred_fr
+00014ea0: 6571 0a20 2020 2020 2020 2020 2020 2069  eq.            i
+00014eb0: 6620 696e 6665 7272 6564 5f66 7265 7120  f inferred_freq 
+00014ec0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00014ed0: 2020 2020 2020 2020 2020 2020 2078 615f               xa_
+00014ee0: 2e67 6574 5f69 6e64 6578 2873 656c 662e  .get_index(self.
+00014ef0: 5f74 696d 655f 6469 6d29 2e66 7265 7120  _time_dim).freq 
+00014f00: 3d20 746f 5f6f 6666 7365 7428 696e 6665  = to_offset(infe
+00014f10: 7272 6564 5f66 7265 7129 0a20 2020 2020  rred_freq).     
+00014f20: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00014f30: 2020 2020 2020 2020 2020 2020 2078 615f               xa_
+00014f40: 2e67 6574 5f69 6e64 6578 2873 656c 662e  .get_index(self.
+00014f50: 5f74 696d 655f 6469 6d29 2e66 7265 7120  _time_dim).freq 
+00014f60: 3d20 7365 6c66 2e5f 6672 6571 0a0a 2020  = self._freq..  
+00014f70: 2020 2020 2020 2320 6861 6e64 6c65 2044        # handle D
+00014f80: 6174 6574 696d 6549 6e64 6578 2061 6e64  atetimeIndex and
+00014f90: 2049 6e74 3634 496e 6465 783a 0a20 2020   Int64Index:.   
+00014fa0: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00014fb0: 6365 286b 6579 2c20 7064 2e44 6174 6574  ce(key, pd.Datet
+00014fc0: 696d 6549 6e64 6578 293a 0a20 2020 2020  imeIndex):.     
+00014fd0: 2020 2020 2020 205f 6368 6563 6b5f 6474         _check_dt
+00014fe0: 2829 0a20 2020 2020 2020 2020 2020 2078  ().            x
+00014ff0: 615f 203d 2073 656c 662e 5f78 612e 7365  a_ = self._xa.se
+00015000: 6c28 7b73 656c 662e 5f74 696d 655f 6469  l({self._time_di
+00015010: 6d3a 206b 6579 7d29 0a0a 2020 2020 2020  m: key})..      
+00015020: 2020 2020 2020 2320 696e 6465 7869 6e67        # indexing
+00015030: 206d 6179 2064 6973 6361 7264 2074 6865   may discard the
+00015040: 2066 7265 7120 736f 2077 6520 7265 7374   freq so we rest
+00015050: 6f72 6520 6974 2e2e 2e0a 2020 2020 2020  ore it....      
+00015060: 2020 2020 2020 2320 544f 444f 3a20 756e        # TODO: un
+00015070: 6974 2d74 6573 7420 7468 6973 0a20 2020  it-test this.   
+00015080: 2020 2020 2020 2020 205f 7365 745f 6672           _set_fr
+00015090: 6571 5f69 6e5f 7861 2878 615f 290a 0a20  eq_in_xa(xa_).. 
+000150a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000150b0: 6e20 5469 6d65 5365 7269 6573 2878 615f  n TimeSeries(xa_
+000150c0: 290a 2020 2020 2020 2020 656c 6966 2069  ).        elif i
+000150d0: 7369 6e73 7461 6e63 6528 6b65 792c 2070  sinstance(key, p
+000150e0: 642e 496e 7436 3449 6e64 6578 293a 0a20  d.Int64Index):. 
+000150f0: 2020 2020 2020 2020 2020 205f 6368 6563             _chec
+00015100: 6b5f 7261 6e67 6528 290a 2020 2020 2020  k_range().      
+00015110: 2020 2020 2020 7265 7475 726e 2054 696d        return Tim
+00015120: 6553 6572 6965 7328 7365 6c66 2e5f 7861  eSeries(self._xa
+00015130: 2e73 656c 287b 7365 6c66 2e5f 7469 6d65  .sel({self._time
+00015140: 5f64 696d 3a20 6b65 797d 2929 0a0a 2020  _dim: key}))..  
+00015150: 2020 2020 2020 2320 6861 6e64 6c65 2073        # handle s
+00015160: 6c69 6365 733a 0a20 2020 2020 2020 2065  lices:.        e
+00015170: 6c69 6620 6973 696e 7374 616e 6365 286b  lif isinstance(k
+00015180: 6579 2c20 736c 6963 6529 3a0a 2020 2020  ey, slice):.    
+00015190: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+000151a0: 7461 6e63 6528 6b65 792e 7374 6172 742c  tance(key.start,
+000151b0: 2073 7472 2920 6f72 2069 7369 6e73 7461   str) or isinsta
+000151c0: 6e63 6528 6b65 792e 7374 6f70 2c20 7374  nce(key.stop, st
+000151d0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+000151e0: 2020 2020 7265 7475 726e 2054 696d 6553      return TimeS
+000151f0: 6572 6965 7328 7365 6c66 2e5f 7861 2e73  eries(self._xa.s
+00015200: 656c 287b 4449 4d53 5b31 5d3a 206b 6579  el({DIMS[1]: key
+00015210: 7d29 290a 2020 2020 2020 2020 2020 2020  })).            
+00015220: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
+00015230: 6b65 792e 7374 6172 742c 2028 696e 742c  key.start, (int,
+00015240: 206e 702e 696e 7436 3429 2920 6f72 2069   np.int64)) or i
+00015250: 7369 6e73 7461 6e63 6528 6b65 792e 7374  sinstance(key.st
+00015260: 6f70 2c20 2869 6e74 2c20 6e70 2e69 6e74  op, (int, np.int
+00015270: 3634 2929 3a0a 2020 2020 2020 2020 2020  64)):.          
+00015280: 2020 2020 2020 7265 7475 726e 2054 696d        return Tim
+00015290: 6553 6572 6965 7328 7365 6c66 2e5f 7861  eSeries(self._xa
+000152a0: 2e69 7365 6c28 7b73 656c 662e 5f74 696d  .isel({self._tim
+000152b0: 655f 6469 6d3a 206b 6579 7d29 290a 2020  e_dim: key})).  
+000152c0: 2020 2020 2020 2020 2020 656c 6966 2069            elif i
+000152d0: 7369 6e73 7461 6e63 6528 6b65 792e 7374  sinstance(key.st
+000152e0: 6172 742c 2070 642e 5469 6d65 7374 616d  art, pd.Timestam
+000152f0: 7029 206f 7220 6973 696e 7374 616e 6365  p) or isinstance
+00015300: 286b 6579 2e73 746f 702c 2070 642e 5469  (key.stop, pd.Ti
+00015310: 6d65 7374 616d 7029 3a0a 2020 2020 2020  mestamp):.      
+00015320: 2020 2020 2020 2020 2020 5f63 6865 636b            _check
+00015330: 5f64 7428 290a 0a20 2020 2020 2020 2020  _dt()..         
+00015340: 2020 2020 2020 2023 2069 6e64 6578 696e         # indexin
+00015350: 6720 6d61 7920 6469 7363 6172 6420 7468  g may discard th
+00015360: 6520 6672 6571 2073 6f20 7765 2072 6573  e freq so we res
+00015370: 746f 7265 2069 742e 2e2e 0a20 2020 2020  tore it....     
+00015380: 2020 2020 2020 2020 2020 2078 615f 203d             xa_ =
+00015390: 2073 656c 662e 5f78 612e 7365 6c28 7b73   self._xa.sel({s
+000153a0: 656c 662e 5f74 696d 655f 6469 6d3a 206b  elf._time_dim: k
+000153b0: 6579 7d29 0a20 2020 2020 2020 2020 2020  ey}).           
+000153c0: 2020 2020 205f 7365 745f 6672 6571 5f69       _set_freq_i
+000153d0: 6e5f 7861 2878 615f 290a 2020 2020 2020  n_xa(xa_).      
+000153e0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000153f0: 2054 696d 6553 6572 6965 7328 7861 5f29   TimeSeries(xa_)
+00015400: 0a0a 2020 2020 2020 2020 2320 6861 6e64  ..        # hand
+00015410: 6c65 2073 696d 706c 6520 7479 7065 733a  le simple types:
+00015420: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
+00015430: 696e 7374 616e 6365 286b 6579 2c20 7374  instance(key, st
+00015440: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00015450: 7265 7475 726e 2054 696d 6553 6572 6965  return TimeSerie
+00015460: 7328 7365 6c66 2e5f 7861 2e73 656c 287b  s(self._xa.sel({
+00015470: 4449 4d53 5b31 5d3a 205b 6b65 795d 7d29  DIMS[1]: [key]})
+00015480: 2920 2023 2068 6176 6520 746f 2070 7574  )  # have to put
+00015490: 206b 6579 2069 6e20 6120 6c69 7374 206e   key in a list n
+000154a0: 6f74 2074 6f20 6472 6f70 2074 6865 2064  ot to drop the d
+000154b0: 696d 656e 7369 6f6e 0a20 2020 2020 2020  imension.       
+000154c0: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+000154d0: 286b 6579 2c20 2869 6e74 2c20 6e70 2e69  (key, (int, np.i
+000154e0: 6e74 3634 2929 3a0a 2020 2020 2020 2020  nt64)):.        
+000154f0: 2020 2020 7265 7475 726e 2054 696d 6553      return TimeS
+00015500: 6572 6965 7328 7365 6c66 2e5f 7861 2e69  eries(self._xa.i
+00015510: 7365 6c28 7b73 656c 662e 5f74 696d 655f  sel({self._time_
+00015520: 6469 6d3a 205b 6b65 795d 7d29 290a 2020  dim: [key]})).  
+00015530: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
+00015540: 7461 6e63 6528 6b65 792c 2070 642e 5469  tance(key, pd.Ti
+00015550: 6d65 7374 616d 7029 3a0a 2020 2020 2020  mestamp):.      
+00015560: 2020 2020 2020 5f63 6865 636b 5f64 7428        _check_dt(
+00015570: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
+00015580: 2069 6e64 6578 696e 6720 6d61 7920 6469   indexing may di
+00015590: 7363 6172 6420 7468 6520 6672 6571 2073  scard the freq s
+000155a0: 6f20 7765 2072 6573 746f 7265 2069 742e  o we restore it.
+000155b0: 2e2e 0a20 2020 2020 2020 2020 2020 2078  ...            x
+000155c0: 615f 203d 2073 656c 662e 5f78 612e 7365  a_ = self._xa.se
+000155d0: 6c28 7b73 656c 662e 5f74 696d 655f 6469  l({self._time_di
+000155e0: 6d3a 205b 6b65 795d 7d29 0a20 2020 2020  m: [key]}).     
+000155f0: 2020 2020 2020 205f 7365 745f 6672 6571         _set_freq
+00015600: 5f69 6e5f 7861 2878 615f 290a 2020 2020  _in_xa(xa_).    
+00015610: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+00015620: 696d 6553 6572 6965 7328 7861 5f29 0a0a  imeSeries(xa_)..
+00015630: 2020 2020 2020 2020 2320 6861 6e64 6c65          # handle
+00015640: 206c 6973 7473 3a0a 2020 2020 2020 2020   lists:.        
+00015650: 6966 2069 7369 6e73 7461 6e63 6528 6b65  if isinstance(ke
+00015660: 792c 206c 6973 7429 3a0a 2020 2020 2020  y, list):.      
+00015670: 2020 2020 2020 6966 2061 6c6c 2869 7369        if all(isi
+00015680: 6e73 7461 6e63 6528 732c 2073 7472 2920  nstance(s, str) 
+00015690: 666f 7220 7320 696e 206b 6579 293a 0a20  for s in key):. 
+000156a0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000156b0: 2077 6865 6e20 7374 7269 6e67 2873 2920   when string(s) 
+000156c0: 6172 6520 7072 6f76 6964 6564 2c20 7765  are provided, we
+000156d0: 2063 6f6e 7369 6465 7220 6974 2061 7320   consider it as 
+000156e0: 2861 206c 6973 7420 6f66 2920 636f 6d70  (a list of) comp
+000156f0: 6f6e 656e 7428 7329 0a20 2020 2020 2020  onent(s).       
+00015700: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00015710: 5469 6d65 5365 7269 6573 2873 656c 662e  TimeSeries(self.
+00015720: 5f78 612e 7365 6c28 7b44 494d 535b 315d  _xa.sel({DIMS[1]
+00015730: 3a20 6b65 797d 2929 0a20 2020 2020 2020  : key})).       
+00015740: 2020 2020 2065 6c69 6620 616c 6c28 6973       elif all(is
+00015750: 696e 7374 616e 6365 2869 2c20 2869 6e74  instance(i, (int
+00015760: 2c20 6e70 2e69 6e74 3634 2929 2066 6f72  , np.int64)) for
+00015770: 2069 2069 6e20 6b65 7929 3a0a 2020 2020   i in key):.    
+00015780: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00015790: 726e 2054 696d 6553 6572 6965 7328 7365  rn TimeSeries(se
+000157a0: 6c66 2e5f 7861 2e69 7365 6c28 7b73 656c  lf._xa.isel({sel
+000157b0: 662e 5f74 696d 655f 6469 6d3a 206b 6579  f._time_dim: key
+000157c0: 7d29 290a 2020 2020 2020 2020 2020 2020  })).            
+000157d0: 656c 6966 2061 6c6c 2869 7369 6e73 7461  elif all(isinsta
+000157e0: 6e63 6528 742c 2070 642e 5469 6d65 7374  nce(t, pd.Timest
+000157f0: 616d 7029 2066 6f72 2074 2069 6e20 6b65  amp) for t in ke
+00015800: 7929 3a0a 2020 2020 2020 2020 2020 2020  y):.            
+00015810: 2020 2020 5f63 6865 636b 5f64 7428 290a      _check_dt().
+00015820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015830: 2023 2069 6e64 6578 696e 6720 6d61 7920   # indexing may 
+00015840: 6469 7363 6172 6420 7468 6520 6672 6571  discard the freq
+00015850: 2073 6f20 7765 2072 6573 746f 7265 2069   so we restore i
+00015860: 742e 2e2e 0a20 2020 2020 2020 2020 2020  t....           
+00015870: 2020 2020 2078 615f 203d 2073 656c 662e       xa_ = self.
+00015880: 5f78 612e 7365 6c28 7b73 656c 662e 5f74  _xa.sel({self._t
+00015890: 696d 655f 6469 6d3a 206b 6579 7d29 0a20  ime_dim: key}). 
+000158a0: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+000158b0: 7365 745f 6672 6571 5f69 6e5f 7861 2878  set_freq_in_xa(x
+000158c0: 615f 290a 2020 2020 2020 2020 2020 2020  a_).            
+000158d0: 2020 2020 7265 7475 726e 2054 696d 6553      return TimeS
+000158e0: 6572 6965 7328 7861 5f29 0a0a 2020 2020  eries(xa_)..    
+000158f0: 2020 2020 7261 6973 655f 6c6f 6728 496e      raise_log(In
+00015900: 6465 7845 7272 6f72 2822 5468 6520 7479  dexError("The ty
+00015910: 7065 206f 6620 796f 7572 2069 6e64 6578  pe of your index
+00015920: 2077 6173 206e 6f74 206d 6174 6368 6564   was not matched
+00015930: 2e22 292c 206c 6f67 6765 7229 0a         ."), logger).
```

### Comparing `darts-0.9.0/darts/utils/data/horizon_based_dataset.py` & `darts-0.9.1/darts/utils/data/horizon_based_dataset.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/utils/data/sequential_dataset.py` & `darts-0.9.1/darts/utils/data/sequential_dataset.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/utils/data/shifted_dataset.py` & `darts-0.9.1/darts/utils/data/shifted_dataset.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/utils/data/simple_inference_dataset.py` & `darts-0.9.1/darts/utils/data/simple_inference_dataset.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/utils/data/timeseries_dataset.py` & `darts-0.9.1/darts/utils/data/timeseries_dataset.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/utils/likelihood_models.py` & `darts-0.9.1/darts/utils/likelihood_models.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/utils/missing_values.py` & `darts-0.9.1/darts/utils/missing_values.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/utils/model_selection.py` & `darts-0.9.1/darts/utils/model_selection.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/utils/statistics.py` & `darts-0.9.1/darts/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/utils/timeseries_generation.py` & `darts-0.9.1/darts/utils/timeseries_generation.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/utils/torch.py` & `darts-0.9.1/darts/utils/torch.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/darts/utils/utils.py` & `darts-0.9.1/darts/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Additional util functions
 -------------------------
 """
 import pandas as pd
+import numpy as np
 
 from ..timeseries import TimeSeries
 from ..logging import raise_log, get_logger, raise_if_not, raise_if
 from typing import List, Callable, TypeVar, Iterator, Tuple
 from IPython import get_ipython
 from tqdm import tqdm
 from tqdm.notebook import tqdm as tqdm_notebook
@@ -182,15 +183,15 @@
     # check start parameter
     if hasattr(n, 'start'):
         if isinstance(n.start, float):
             raise_if_not(0.0 <= n.start < 1.0, '`start` should be between 0.0 and 1.0.', logger)
         elif isinstance(n.start, pd.Timestamp):
             raise_if(n.start not in series, '`start` timestamp must be an entry in the time series\' time index')
             raise_if(n.start == series.end_time(), '`start` timestamp is the last timestamp of the series', logger)
-        elif isinstance(n.start, int):
+        elif isinstance(n.start, (int, np.int64)):
             raise_if_not(n.start >= 0, logger)
             raise_if(n.start > len(series), '`start` index should be smaller than length of the series', logger)
         else:
             raise_log(TypeError("`start` needs to be either `float`, `int` or `pd.Timestamp`"), logger)
 
     start = series.get_timestamp_at_point(n.start)
```

### Comparing `darts-0.9.0/darts.egg-info/PKG-INFO` & `darts-0.9.1/darts.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darts
-Version: 0.9.0
+Version: 0.9.1
 Summary: A python library for easy manipulation and forecasting of time series.
 Home-page: https://unit8co.github.io/darts/
 Maintainer: Unit8 SA
 Maintainer-email: darts@unit8.co
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/unit8co/darts/issues
 Project-URL: Documentation, https://unit8co.github.io/darts/
@@ -139,30 +139,29 @@
 inferences of the underlying states/values.
 
 ## Forecasting Models
 Here's a breakdown of the forecasting models currently implemented in Darts. We are constantly working
 on bringing more models and features.
 
 Model | Univariate | Multivariate | Probabilistic | Multiple-series training | Past-observed covariates support | Future-known covariates support
---- | --- | --- | --- | --- | --- | --- |
-`ARIMA` | x | | x | | | |
-`VARIMA` | x | x | | | | |
-`AutoARIMA` | x | | | | | |
-`ExponentialSmoothing` | x | | x | | | |
-`Theta` and `FourTheta` | x | | | | | |
-`Prophet` | x | | | | | |
-`FFT` (Fast Fourier Transform) | x | | | | | |
-Regression Models (incl `RandomForest` and `LinearRegressionModel`) | x | | | | | |
-`RNNModel` (incl. LSTM and GRU); equivalent to DeepAR in its probabilistic version | x | x | x | x | x | x |
-`BlockRNNModel` (incl. LSTM and GRU) | x | x | | x | x | (x) |
-`NBEATSModel` | x | x | | x | x | (x) |
-`TCNModel` | x | x | x | x | x | (x) |
-`TransformerModel` | x | x | | x | x | (x) |
-Naive Baselines | x | | | | | |
-
+--- | --- | --- | --- | --- | --- | ---
+`ARIMA` | x | | x | | |
+`VARIMA` | x | x | | | |
+`AutoARIMA` | x | | | | |
+`ExponentialSmoothing` | x | | x | | |
+`Theta` and `FourTheta` | x | | | | |
+`Prophet` | x | | | | |
+`FFT` (Fast Fourier Transform) | x | | | | |
+Regression Models (incl `RandomForest` and `LinearRegressionModel`) | x | | | | |
+`RNNModel` (incl. LSTM and GRU); equivalent to DeepAR in its probabilistic version | x | x | x | x | x | x
+`BlockRNNModel` (incl. LSTM and GRU) | x | x | | x | x | ( x )
+`NBEATSModel` | x | x | | x | x | ( x )
+`TCNModel` | x | x | x | x | x | ( x )
+`TransformerModel` | x | x | | x | x | ( x )
+Naive Baselines | x | | | | |
 
 ## Contribute
 
 The development is ongoing, and there are many new features that we want to add.
 We welcome pull requests and issues on GitHub.
 
 Before working on a contribution (a new feature or a fix), [**check our contribution guidelines**](CONTRIBUTE.md).
@@ -172,20 +171,20 @@
 
 If what you want to tell us is not a suitable github issue, feel free to send us an email at <a href="mailto:darts@unit8.co">darts@unit8.co</a> for darts related matters or <a href="mailto:info@unit8.co">info@unit8.co</a> for any other inquiries.
 
 ## Installation Guide
 
 ### Preconditions
 
-Some of the models depend on `fbprophet` and `torch`, which have non-Python dependencies.
+Some of the models depend on `prophet` and `torch`, which have non-Python dependencies.
 A Conda environment is thus recommended because it will handle all of those in one go.
 
 The following steps assume running inside a conda environment.
 If that's not possible, first follow the official instructions to install
-[fbprophet](https://facebook.github.io/prophet/docs/installation.html#python)
+[prophet](https://facebook.github.io/prophet/docs/installation.html#python)
 and [torch](https://pytorch.org/get-started/locally/), then skip to
 [Install darts](#install-darts)
 
 To create a conda environment for Python 3.7
 (after installing [conda](https://docs.conda.io/en/latest/miniconda.html)):
 
     conda create --name <env-name> python=3.7
@@ -193,30 +192,30 @@
 Don't forget to activate your virtual environment
 
     conda activate <env-name>
 
 
 #### MAC
 
-    conda install -c conda-forge -c pytorch pip fbprophet pytorch
+    conda install -c conda-forge -c pytorch pip prophet pytorch
 
 #### Linux and Windows
 
-    conda install -c conda-forge -c pytorch pip fbprophet pytorch cpuonly
+    conda install -c conda-forge -c pytorch pip prophet pytorch cpuonly
 
 ### Install darts
 
 Install Darts with all available models: `pip install darts`.
 
 As some models have relatively heavy (or non-Python) dependencies,
 we also maintain the `u8darts` package, which provides the following alternate lighter install options:
 
 * Install core only (without neural networks, Prophet or AutoARIMA): `pip install u8darts`
 * Install core + neural networks (PyTorch): `pip install 'u8darts[torch]'`
-* Install core + Facebook Prophet: `pip install 'u8darts[fbprophet]'`
+* Install core + Facebook Prophet: `pip install 'u8darts[prophet]'`
 * Install core + AutoARIMA: `pip install 'u8darts[pmdarima]'`
 
 ### Running the examples only, without installing:
 
 If the conda setup is causing too many problems, we also provide a Docker image with everything set up for you and ready-to-use Python notebooks with demo examples.
 To run the example notebooks without installing our libraries natively on your machine, you can use our Docker image:
 ```bash
@@ -240,15 +239,15 @@
 alternatively you can run
 ```bash
 ./gradlew unitTest_all # to run only unittests
 ./gradlew coverageTest # to run coverage
 ./gradlew lint         # to run linter
 ```
 
-To run the tests for specific flavours of the library, replace `_all` with `_core`, `_fbprophet`, `_pmdarima` or `_torch`.
+To run the tests for specific flavours of the library, replace `_all` with `_core`, `_prophet`, `_pmdarima` or `_torch`.
 
 ### Documentation
 
 To build documantation locally just run
 ```bash
 ./gradlew buildDocs
 ```
```

### Comparing `darts-0.9.0/darts.egg-info/SOURCES.txt` & `darts-0.9.1/darts.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 MANIFEST.in
 README.md
 build.gradle
 coverage.sh
 gradlew
 gradlew.bat
 make_dists.sh
+pyproject.toml
 settings.gradle
 setup.cfg
 setup.py
 setup_u8darts.py
 .github/CODEOWNERS
 .github/pull_request_template.md
 .github/ISSUE_TEMPLATE/bug_report.md
@@ -152,14 +153,17 @@
 examples/02-multi-time-series-and-covariates.ipynb
 examples/03-data-processing.ipynb
 examples/04-FFT-examples.ipynb
 examples/05-RNN-examples.ipynb
 examples/06-TCN-examples.ipynb
 examples/07-Transformer-examples.ipynb
 examples/08-NBEATS-examples.ipynb
+examples/09-DeepAR-examples.ipynb
+examples/10-DeepTCN-examples.ipynb
+examples/future-covariates-example.ipynb
 examples/M4_competition/M4_competition_benchmark.ipynb
 examples/M4_competition/M4_metrics.py
 examples/M4_competition/create_ts.py
 examples/M4_competition/download_data_M4.py
 examples/M4_competition/evaluate_arima.py
 examples/M4_competition/evaluate_baselines.py
 examples/M4_competition/evaluate_ensembling.py
@@ -175,13 +179,13 @@
 examples/utils/__init__.py
 examples/utils/utils.py
 gradle/wrapper/gradle-wrapper.jar
 gradle/wrapper/gradle-wrapper.properties
 requirements/core.txt
 requirements/dev-all.txt
 requirements/dev.txt
-requirements/fbprophet.txt
 requirements/pmdarima.txt
+requirements/prophet.txt
 requirements/release.txt
 requirements/torch.txt
 static/images/darts-logo-trim.png
 static/images/example.png
```

### Comparing `darts-0.9.0/datasets/AirPassengers.csv` & `darts-0.9.1/datasets/AirPassengers.csv`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/datasets/ausbeer.csv` & `darts-0.9.1/datasets/ausbeer.csv`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/datasets/energy_dataset.csv` & `darts-0.9.1/datasets/energy_dataset.csv`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/datasets/gasrate_co2.csv` & `darts-0.9.1/datasets/gasrate_co2.csv`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/datasets/heart_rate.csv` & `darts-0.9.1/datasets/heart_rate.csv`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/datasets/ice_cream_heater.csv` & `darts-0.9.1/datasets/ice_cream_heater.csv`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/datasets/monthly-milk-incomplete.csv` & `darts-0.9.1/datasets/monthly-milk-incomplete.csv`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/datasets/monthly-milk.csv` & `darts-0.9.1/datasets/monthly-milk.csv`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/datasets/monthly-sunspots.csv` & `darts-0.9.1/datasets/monthly-sunspots.csv`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/datasets/taylor.csv` & `darts-0.9.1/datasets/taylor.csv`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/datasets/temps.csv` & `darts-0.9.1/datasets/temps.csv`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/datasets/us_gasoline.csv` & `darts-0.9.1/datasets/us_gasoline.csv`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/datasets/wineind.csv` & `darts-0.9.1/datasets/wineind.csv`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/datasets/woolyrnq.csv` & `darts-0.9.1/datasets/woolyrnq.csv`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/docs/Makefile` & `darts-0.9.1/docs/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 .PHONY: help Makefile
 
 generate:
 	@sphinx-apidoc -e -f --templatedir templates -o "$(SOURCEDIR)/generated_api" ../darts ../darts/logging.py ../darts/tests/*
 
 readme:
-	@m2r ../README.md; mv ../README.rst "$(SOURCEDIR)"
+	@m2r2 ../README.md; mv ../README.rst "$(SOURCEDIR)"
 
 copy-examples:
 	@cp -r ../examples "$(SOURCEDIR)/examples"
 
 clean:
 	@rm -rf ./build
 	@rm -rf ./source/examples
```

### Comparing `darts-0.9.0/docs/source/conf.py` & `darts-0.9.1/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 # -- Project information -----------------------------------------------------
 
 project = 'darts'
 copyright = '2021, Unit8 SA'
 author = 'Unit8 SA'
-version = '0.9.0'
+version = '0.9.1'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
@@ -35,15 +35,15 @@
     'sphinx.ext.viewcode',
     'sphinx.ext.todo',
     'sphinx_automodapi.automodapi',
     'sphinx.ext.graphviz',
     'sphinx.ext.napoleon',
     'sphinx.ext.githubpages',
     'nbsphinx',
-    'm2r'
+    'm2r2'
 ]
 
 autodoc_default_options = {
     'inherited-members': None,
     'show-inheritance': None,
     'exclude-members': 'TimeSeriesTorchDataset'
 }
```

### Comparing `darts-0.9.0/docs/source/examples.rst` & `darts-0.9.1/docs/source/examples.rst`

 * *Files 8% similar despite different names*

```diff
@@ -64,26 +64,66 @@
 You will find below an example Jupyter notebook showcasing the usage of the TCN model
 
 .. toctree::
    :maxdepth: 1
 
    examples/06-TCN-examples.ipynb
 
-Transformer Model Examples
-==========================
+Transformer Model
+=================
 
 You will find below an example Jupyter notebook showcasing the usage of the Transformer model
 
 .. toctree::
    :maxdepth: 1
 
    examples/07-Transformer-examples.ipynb
 
-N-BEATS Model Examples
-==========================
+N-BEATS Model
+=============
 
 You will find below an example Jupyter notebook showcasing the usage of the N-BEATS model
 
 .. toctree::
    :maxdepth: 1
 
    examples/08-NBEATS-examples.ipynb
+
+DeepAR Model
+============
+
+You will find below an example Jupyter notebook showcasing the usage of the DeepAR model
+
+.. toctree::
+   :maxdepth: 1
+
+   examples/09-DeepAR-examples.ipynb
+
+DeepTCN Model
+=============
+
+You will find below an example Jupyter notebook showcasing the usage of the DeepTCN model
+
+.. toctree::
+   :maxdepth: 1
+
+   examples/10-DeepTCN-examples.ipynb
+
+Kalman Filter Model
+===================
+
+You will find below an example Jupyter notebook showcasing the usage of the Kalman filter model
+
+.. toctree::
+   :maxdepth: 1
+
+   examples/11-Kalman-filter-examples.ipynb
+
+Gaussian Process Filter Model
+=============================
+
+You will find below an example Jupyter notebook showcasing the usage of the Gaussian Process filter model
+
+.. toctree::
+   :maxdepth: 1
+
+   examples/12-GP-filter-examples.ipynb
```

### Comparing `darts-0.9.0/docs/source/static/darts-logo-trim.png` & `darts-0.9.1/docs/source/static/darts-logo-trim.png`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/docs/templates/package.rst_t` & `darts-0.9.1/docs/templates/package.rst_t`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/examples/01-darts-intro.ipynb` & `darts-0.9.1/examples/01-darts-intro.ipynb`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/examples/02-multi-time-series-and-covariates.ipynb` & `darts-0.9.1/examples/02-multi-time-series-and-covariates.ipynb`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/examples/03-data-processing.ipynb` & `darts-0.9.1/examples/03-data-processing.ipynb`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/examples/04-FFT-examples.ipynb` & `darts-0.9.1/examples/04-FFT-examples.ipynb`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/examples/05-RNN-examples.ipynb` & `darts-0.9.1/examples/05-RNN-examples.ipynb`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/examples/06-TCN-examples.ipynb` & `darts-0.9.1/examples/06-TCN-examples.ipynb`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/examples/07-Transformer-examples.ipynb` & `darts-0.9.1/examples/07-Transformer-examples.ipynb`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/examples/08-NBEATS-examples.ipynb` & `darts-0.9.1/examples/08-NBEATS-examples.ipynb`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/examples/M4_competition/M4_competition_benchmark.ipynb` & `darts-0.9.1/examples/M4_competition/M4_competition_benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/examples/M4_competition/M4_metrics.py` & `darts-0.9.1/examples/M4_competition/M4_metrics.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/examples/M4_competition/create_ts.py` & `darts-0.9.1/examples/M4_competition/create_ts.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/examples/M4_competition/download_data_M4.py` & `darts-0.9.1/examples/M4_competition/download_data_M4.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/examples/M4_competition/evaluate_arima.py` & `darts-0.9.1/examples/M4_competition/evaluate_arima.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/examples/M4_competition/evaluate_baselines.py` & `darts-0.9.1/examples/M4_competition/evaluate_baselines.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/examples/M4_competition/evaluate_ensembling.py` & `darts-0.9.1/examples/M4_competition/evaluate_ensembling.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/examples/M4_competition/evaluate_fft.py` & `darts-0.9.1/examples/M4_competition/evaluate_fft.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/examples/M4_competition/evaluate_groe_R.py` & `darts-0.9.1/examples/M4_competition/evaluate_groe_R.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/examples/M4_competition/evaluate_naive2_with_R.py` & `darts-0.9.1/examples/M4_competition/evaluate_naive2_with_R.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/examples/M4_competition/evaluate_prophet.py` & `darts-0.9.1/examples/M4_competition/evaluate_prophet.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/examples/M4_competition/evaluate_theta_methods.py` & `darts-0.9.1/examples/M4_competition/evaluate_theta_methods.py`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/examples/static/images/global_io.png` & `darts-0.9.1/examples/static/images/global_io.png`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/examples/static/images/global_io_covs.png` & `darts-0.9.1/examples/static/images/global_io_covs.png`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/examples/static/images/seq_dataset_multi_ts.png` & `darts-0.9.1/examples/static/images/seq_dataset_multi_ts.png`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/examples/static/images/seq_dataset_one_ts.png` & `darts-0.9.1/examples/static/images/seq_dataset_one_ts.png`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/gradle/wrapper/gradle-wrapper.jar` & `darts-0.9.1/gradle/wrapper/gradle-wrapper.jar`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/gradlew` & `darts-0.9.1/gradlew`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/gradlew.bat` & `darts-0.9.1/gradlew.bat`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/setup.py` & `darts-0.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 def read_requirements(path):
     return list(Path(path).read_text().splitlines())
 
 
 base_reqs = read_requirements('requirements/core.txt')
 pmdarima_reqs = read_requirements('requirements/pmdarima.txt')
 torch_reqs = read_requirements('requirements/torch.txt')
-fbprophet_reqs = read_requirements('requirements/fbprophet.txt')
+prophet_reqs = read_requirements('requirements/prophet.txt')
 
-all_reqs = base_reqs + pmdarima_reqs + torch_reqs + fbprophet_reqs
+all_reqs = base_reqs + pmdarima_reqs + torch_reqs + prophet_reqs
 
 with open("README.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
 
 URL = 'https://unit8co.github.io/darts/'
 
@@ -25,15 +25,15 @@
     'Documentation': URL,
     'Source Code': 'https://github.com/unit8co/darts'
 }
 
 
 setup(
       name='darts',
-      version="0.9.0",
+      version="0.9.1",
       description='A python library for easy manipulation and forecasting of time series.',
       long_description=LONG_DESCRIPTION,
       long_description_content_type="text/markdown",
       project_urls=PROJECT_URLS,
       url=URL,
       maintainer='Unit8 SA',
       maintainer_email='darts@unit8.co',
```

### Comparing `darts-0.9.0/setup_u8darts.py` & `darts-0.9.1/setup_u8darts.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 def read_requirements(path):
     return list(Path(path).read_text().splitlines())
 
 
 base_reqs = read_requirements('requirements/core.txt')
 pmdarima_reqs = read_requirements('requirements/pmdarima.txt')
 torch_reqs = read_requirements('requirements/torch.txt')
-fbprophet_reqs = read_requirements('requirements/fbprophet.txt')
+prophet_reqs = read_requirements('requirements/prophet.txt')
 
-all_reqs = base_reqs + pmdarima_reqs + torch_reqs + fbprophet_reqs
+all_reqs = base_reqs + pmdarima_reqs + torch_reqs + prophet_reqs
 
 with open("README.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
 
 URL = 'https://unit8co.github.io/darts/'
 
@@ -25,30 +25,30 @@
     'Documentation': URL,
     'Source Code': 'https://github.com/unit8co/darts'
 }
 
 
 setup(
       name='u8darts',
-      version="0.9.0",
+      version="0.9.1",
       description='A python library for easy manipulation and forecasting of time series.',
       long_description=LONG_DESCRIPTION,
       long_description_content_type="text/markdown",
       project_urls=PROJECT_URLS,
       url=URL,
       maintainer='Unit8 SA',
       maintainer_email='darts@unit8.co',
       license='Apache License 2.0',
       packages=find_packages(),
       install_requires=base_reqs,
       extras_require={
             'all': all_reqs,
             'pmdarima': pmdarima_reqs,
             'torch': torch_reqs,
-            'fbprophet': fbprophet_reqs,
+            'prophet': prophet_reqs,
       },
       package_data={
           'darts': ['py.typed'],
       },
       zip_safe=False,
       python_requires='>=3.7',
       classifiers=[
```

### Comparing `darts-0.9.0/static/images/darts-logo-trim.png` & `darts-0.9.1/static/images/darts-logo-trim.png`

 * *Files identical despite different names*

### Comparing `darts-0.9.0/static/images/example.png` & `darts-0.9.1/static/images/example.png`

 * *Files identical despite different names*

