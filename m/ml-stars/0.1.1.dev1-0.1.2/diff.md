# Comparing `tmp/ml-stars-0.1.1.dev1.tar.gz` & `tmp/ml-stars-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-stars-0.1.1.dev1.tar", last modified: Tue May 16 21:58:52 2023, max compression
+gzip compressed data, was "ml-stars-0.1.2.tar", last modified: Fri Aug  4 22:41:42 2023, max compression
```

## Comparing `ml-stars-0.1.1.dev1.tar` & `ml-stars-0.1.2.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.777452 ml-stars-0.1.1.dev1/
--rw-r--r--   0 sarah      (501) staff       (20)      108 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/AUTHORS.rst
--rw-r--r--   0 sarah      (501) staff       (20)     8324 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/CONTRIBUTING.rst
--rw-r--r--   0 sarah      (501) staff       (20)      109 2023-04-18 19:20:35.000000 ml-stars-0.1.1.dev1/HISTORY.md
--rw-r--r--   0 sarah      (501) staff       (20)     1070 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/LICENSE
--rw-r--r--   0 sarah      (501) staff       (20)      299 2023-04-18 19:20:35.000000 ml-stars-0.1.1.dev1/MANIFEST.in
--rw-r--r--   0 sarah      (501) staff       (20)     5275 2023-05-16 21:58:52.777682 ml-stars-0.1.1.dev1/PKG-INFO
--rw-r--r--   0 sarah      (501) staff       (20)     4361 2023-04-18 19:20:35.000000 ml-stars-0.1.1.dev1/README.md
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.670988 ml-stars-0.1.1.dev1/docs/
--rw-r--r--   0 sarah      (501) staff       (20)      608 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/docs/Makefile
--rw-r--r--   0 sarah      (501) staff       (20)     6403 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/docs/conf.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.674231 ml-stars-0.1.1.dev1/docs/developer_guides/
--rw-r--r--   0 sarah      (501) staff       (20)     8504 2023-05-16 18:50:11.000000 ml-stars-0.1.1.dev1/docs/developer_guides/adapters.rst
--rw-r--r--   0 sarah      (501) staff       (20)     7667 2023-05-16 21:56:21.000000 ml-stars-0.1.1.dev1/docs/developer_guides/annotations.rst
--rw-r--r--   0 sarah      (501) staff       (20)     5116 2023-05-16 18:50:11.000000 ml-stars-0.1.1.dev1/docs/developer_guides/contributing.rst
--rw-r--r--   0 sarah      (501) staff       (20)     7925 2023-05-16 18:50:11.000000 ml-stars-0.1.1.dev1/docs/developer_guides/custom.rst
--rw-r--r--   0 sarah      (501) staff       (20)     3414 2023-05-16 21:56:21.000000 ml-stars-0.1.1.dev1/docs/developer_guides/index.rst
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.676652 ml-stars-0.1.1.dev1/docs/getting_started/
--rw-r--r--   0 sarah      (501) staff       (20)     6296 2023-05-16 18:50:11.000000 ml-stars-0.1.1.dev1/docs/getting_started/concepts.rst
--rw-r--r--   0 sarah      (501) staff       (20)      126 2023-05-16 18:50:11.000000 ml-stars-0.1.1.dev1/docs/getting_started/index.rst
--rw-r--r--   0 sarah      (501) staff       (20)     1589 2023-05-16 18:50:11.000000 ml-stars-0.1.1.dev1/docs/getting_started/install.rst
--rw-r--r--   0 sarah      (501) staff       (20)     1920 2023-05-16 18:50:11.000000 ml-stars-0.1.1.dev1/docs/getting_started/quickstart.rst
--rw-r--r--   0 sarah      (501) staff       (20)       29 2023-05-16 18:50:11.000000 ml-stars-0.1.1.dev1/docs/history.rst
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.677263 ml-stars-0.1.1.dev1/docs/images/
--rw-r--r--   0 sarah      (501) staff       (20)    33432 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/docs/images/dai-logo-white-200.png
--rw-r--r--   0 sarah      (501) staff       (20)     1505 2023-05-16 18:50:11.000000 ml-stars-0.1.1.dev1/docs/index.rst
--rw-r--r--   0 sarah      (501) staff       (20)      805 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/docs/make.bat
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.682451 ml-stars-0.1.1.dev1/ml_stars.egg-info/
--rw-r--r--   0 sarah      (501) staff       (20)     5275 2023-05-16 21:58:52.000000 ml-stars-0.1.1.dev1/ml_stars.egg-info/PKG-INFO
--rw-r--r--   0 sarah      (501) staff       (20)     4156 2023-05-16 21:58:52.000000 ml-stars-0.1.1.dev1/ml_stars.egg-info/SOURCES.txt
--rw-r--r--   0 sarah      (501) staff       (20)        1 2023-05-16 21:58:52.000000 ml-stars-0.1.1.dev1/ml_stars.egg-info/dependency_links.txt
--rw-r--r--   0 sarah      (501) staff       (20)       91 2023-05-16 21:58:52.000000 ml-stars-0.1.1.dev1/ml_stars.egg-info/entry_points.txt
--rw-r--r--   0 sarah      (501) staff       (20)        1 2023-05-16 21:58:52.000000 ml-stars-0.1.1.dev1/ml_stars.egg-info/not-zip-safe
--rw-r--r--   0 sarah      (501) staff       (20)      683 2023-05-16 21:58:52.000000 ml-stars-0.1.1.dev1/ml_stars.egg-info/requires.txt
--rw-r--r--   0 sarah      (501) staff       (20)        8 2023-05-16 21:58:52.000000 ml-stars-0.1.1.dev1/ml_stars.egg-info/top_level.txt
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.683611 ml-stars-0.1.1.dev1/mlstars/
--rw-r--r--   0 sarah      (501) staff       (20)      441 2023-05-16 21:58:43.000000 ml-stars-0.1.1.dev1/mlstars/__init__.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.687152 ml-stars-0.1.1.dev1/mlstars/adapters/
--rw-r--r--   0 sarah      (501) staff       (20)        0 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/adapters/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)     4088 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/adapters/keras.py
--rw-r--r--   0 sarah      (501) staff       (20)     3449 2023-05-16 21:56:21.000000 ml-stars-0.1.1.dev1/mlstars/adapters/pandas.py
--rw-r--r--   0 sarah      (501) staff       (20)     1731 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/adapters/statsmodels.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.690023 ml-stars-0.1.1.dev1/mlstars/custom/
--rw-r--r--   0 sarah      (501) staff       (20)        0 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/custom/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)    16626 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/custom/timeseries_anomalies.py
--rw-r--r--   0 sarah      (501) staff       (20)     9471 2023-05-16 21:56:21.000000 ml-stars-0.1.1.dev1/mlstars/custom/timeseries_preprocessing.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.770526 ml-stars-0.1.1.dev1/mlstars/primitives/
--rw-r--r--   0 sarah      (501) staff       (20)     5005 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/keras.Sequential.DoubleLSTMTimeSeriesClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)     4499 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/keras.Sequential.LSTMTimeSeriesClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)     5176 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/keras.Sequential.LSTMTimeSeriesRegressor.json
--rw-r--r--   0 sarah      (501) staff       (20)     1902 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/mlstars.custom.timeseries_anomalies.find_anomalies.json
--rw-r--r--   0 sarah      (501) staff       (20)     1244 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/mlstars.custom.timeseries_anomalies.regression_errors.json
--rw-r--r--   0 sarah      (501) staff       (20)     1173 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/mlstars.custom.timeseries_preprocessing.cutoff_window_sequences.json
--rw-r--r--   0 sarah      (501) staff       (20)      870 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/mlstars.custom.timeseries_preprocessing.intervals_to_mask.json
--rw-r--r--   0 sarah      (501) staff       (20)     2027 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/mlstars.custom.timeseries_preprocessing.rolling_window_sequences.json
--rw-r--r--   0 sarah      (501) staff       (20)     1524 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/mlstars.custom.timeseries_preprocessing.time_segments_aggregate.json
--rw-r--r--   0 sarah      (501) staff       (20)     1099 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/mlstars.custom.timeseries_preprocessing.time_segments_average.json
--rw-r--r--   0 sarah      (501) staff       (20)      847 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/numpy.argmax.json
--rw-r--r--   0 sarah      (501) staff       (20)      821 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/numpy.ravel.json
--rw-r--r--   0 sarah      (501) staff       (20)     1014 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/numpy.reshape.json
--rw-r--r--   0 sarah      (501) staff       (20)     1607 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.append.json
--rw-r--r--   0 sarah      (501) staff       (20)     1621 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.drop.json
--rw-r--r--   0 sarah      (501) staff       (20)     1399 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.drop_duplicates.json
--rw-r--r--   0 sarah      (501) staff       (20)     1579 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.dropna.json
--rw-r--r--   0 sarah      (501) staff       (20)     1738 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.fillna.json
--rw-r--r--   0 sarah      (501) staff       (20)     1686 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.filter.json
--rw-r--r--   0 sarah      (501) staff       (20)      998 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.get.json
--rw-r--r--   0 sarah      (501) staff       (20)     1948 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.join.json
--rw-r--r--   0 sarah      (501) staff       (20)     1521 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.json
--rw-r--r--   0 sarah      (501) staff       (20)      947 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.pop.json
--rw-r--r--   0 sarah      (501) staff       (20)     2273 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.resample.json
--rw-r--r--   0 sarah      (501) staff       (20)     1346 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.select_dtypes.json
--rw-r--r--   0 sarah      (501) staff       (20)     1047 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.set.json
--rw-r--r--   0 sarah      (501) staff       (20)     1817 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.set_index.json
--rw-r--r--   0 sarah      (501) staff       (20)     1346 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.to_numpy.json
--rw-r--r--   0 sarah      (501) staff       (20)     1243 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.unstack.json
--rw-r--r--   0 sarah      (501) staff       (20)     1224 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/pandas.Series.filter.json
--rw-r--r--   0 sarah      (501) staff       (20)     2238 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.decomposition.PCA.json
--rw-r--r--   0 sarah      (501) staff       (20)     1890 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.ensemble.AdaBoostClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)     1914 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.ensemble.AdaBoostRegressor.json
--rw-r--r--   0 sarah      (501) staff       (20)     4782 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.ensemble.GradientBoostingClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)     5015 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.ensemble.GradientBoostingRegressor.json
--rw-r--r--   0 sarah      (501) staff       (20)     2565 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.ensemble.IsolationForest.json
--rw-r--r--   0 sarah      (501) staff       (20)     3721 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.ensemble.RandomForestClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)     3909 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.ensemble.RandomForestRegressor.json
--rw-r--r--   0 sarah      (501) staff       (20)     1765 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.impute.SimpleImputer.json
--rw-r--r--   0 sarah      (501) staff       (20)     5411 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.linear_model.Lasso.json
--rw-r--r--   0 sarah      (501) staff       (20)     2378 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.linear_model.LinearRegression.json
--rw-r--r--   0 sarah      (501) staff       (20)     7498 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.linear_model.LogisticRegression.json
--rw-r--r--   0 sarah      (501) staff       (20)     4365 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.linear_model.Ridge.json
--rw-r--r--   0 sarah      (501) staff       (20)     2459 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.neighbors.KNeighborsClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)     2401 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.neighbors.KNeighborsRegressor.json
--rw-r--r--   0 sarah      (501) staff       (20)     1663 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.preprocessing.MinMaxScaler.json
--rw-r--r--   0 sarah      (501) staff       (20)     1321 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.preprocessing.OneHotEncoder.json
--rw-r--r--   0 sarah      (501) staff       (20)     1262 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.preprocessing.StandardScaler.json
--rw-r--r--   0 sarah      (501) staff       (20)     1366 2023-05-16 21:56:21.000000 ml-stars-0.1.1.dev1/mlstars/primitives/statsmodels.tsa.arima_model.Arima.json
--rw-r--r--   0 sarah      (501) staff       (20)     2226 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/xgboost.XGBClassifier.json
--rw-r--r--   0 sarah      (501) staff       (20)     2220 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/primitives/xgboost.XGBRegressor.json
--rw-r--r--   0 sarah      (501) staff       (20)     2941 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/mlstars/utils.py
--rw-r--r--   0 sarah      (501) staff       (20)      988 2023-05-16 21:58:52.779336 ml-stars-0.1.1.dev1/setup.cfg
--rw-r--r--   0 sarah      (501) staff       (20)     2801 2023-05-16 21:58:43.000000 ml-stars-0.1.1.dev1/setup.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.772229 ml-stars-0.1.1.dev1/tests/
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.774916 ml-stars-0.1.1.dev1/tests/adapters/
--rw-r--r--   0 sarah      (501) staff       (20)     1836 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/tests/adapters/test_keras.py
--rw-r--r--   0 sarah      (501) staff       (20)     5027 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/tests/adapters/test_pandas.py
--rw-r--r--   0 sarah      (501) staff       (20)     1961 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/tests/adapters/test_statsmodels.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-05-16 21:58:52.776696 ml-stars-0.1.1.dev1/tests/custom/
--rw-r--r--   0 sarah      (501) staff       (20)     7362 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/tests/custom/test_timeseries_anomalies.py
--rw-r--r--   0 sarah      (501) staff       (20)    15169 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/tests/custom/test_timeseries_preprocessing.py
--rw-r--r--   0 sarah      (501) staff       (20)      442 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/tests/test_mlstars.py
--rw-r--r--   0 sarah      (501) staff       (20)      217 2023-04-18 19:08:26.000000 ml-stars-0.1.1.dev1/tests/test_utils.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-08-04 22:41:42.504556 ml-stars-0.1.2/
+-rw-r--r--   0 sarah      (501) staff       (20)      108 2023-08-04 22:29:11.000000 ml-stars-0.1.2/AUTHORS.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     8324 2023-08-04 22:29:11.000000 ml-stars-0.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      326 2023-08-04 22:29:11.000000 ml-stars-0.1.2/HISTORY.md
+-rw-r--r--   0 sarah      (501) staff       (20)     1070 2023-08-04 22:29:11.000000 ml-stars-0.1.2/LICENSE
+-rw-r--r--   0 sarah      (501) staff       (20)      299 2023-08-04 22:29:11.000000 ml-stars-0.1.2/MANIFEST.in
+-rw-r--r--   0 sarah      (501) staff       (20)     5545 2023-08-04 22:41:42.504685 ml-stars-0.1.2/PKG-INFO
+-rw-r--r--   0 sarah      (501) staff       (20)     4368 2023-08-04 22:41:35.000000 ml-stars-0.1.2/README.md
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-08-04 22:41:42.477951 ml-stars-0.1.2/docs/
+-rw-r--r--   0 sarah      (501) staff       (20)      608 2023-08-04 22:29:11.000000 ml-stars-0.1.2/docs/Makefile
+-rw-r--r--   0 sarah      (501) staff       (20)     6403 2023-08-04 22:29:11.000000 ml-stars-0.1.2/docs/conf.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-08-04 22:41:42.479479 ml-stars-0.1.2/docs/developer_guides/
+-rw-r--r--   0 sarah      (501) staff       (20)     8504 2023-08-04 22:29:11.000000 ml-stars-0.1.2/docs/developer_guides/adapters.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     7667 2023-08-04 22:29:11.000000 ml-stars-0.1.2/docs/developer_guides/annotations.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     5116 2023-08-04 22:29:11.000000 ml-stars-0.1.2/docs/developer_guides/contributing.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     7925 2023-08-04 22:29:11.000000 ml-stars-0.1.2/docs/developer_guides/custom.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     3414 2023-08-04 22:29:11.000000 ml-stars-0.1.2/docs/developer_guides/index.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-08-04 22:41:42.480831 ml-stars-0.1.2/docs/getting_started/
+-rw-r--r--   0 sarah      (501) staff       (20)     6296 2023-08-04 22:29:11.000000 ml-stars-0.1.2/docs/getting_started/concepts.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      126 2023-08-04 22:29:11.000000 ml-stars-0.1.2/docs/getting_started/index.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     1589 2023-08-04 22:29:11.000000 ml-stars-0.1.2/docs/getting_started/install.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     1920 2023-08-04 22:29:11.000000 ml-stars-0.1.2/docs/getting_started/quickstart.rst
+-rw-r--r--   0 sarah      (501) staff       (20)       29 2023-08-04 22:29:11.000000 ml-stars-0.1.2/docs/history.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-08-04 22:41:42.481124 ml-stars-0.1.2/docs/images/
+-rw-r--r--   0 sarah      (501) staff       (20)    33432 2023-08-04 22:29:11.000000 ml-stars-0.1.2/docs/images/dai-logo-white-200.png
+-rw-r--r--   0 sarah      (501) staff       (20)     1505 2023-08-04 22:29:11.000000 ml-stars-0.1.2/docs/index.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      805 2023-08-04 22:29:11.000000 ml-stars-0.1.2/docs/make.bat
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-08-04 22:41:42.483392 ml-stars-0.1.2/ml_stars.egg-info/
+-rw-r--r--   0 sarah      (501) staff       (20)     5545 2023-08-04 22:41:42.000000 ml-stars-0.1.2/ml_stars.egg-info/PKG-INFO
+-rw-r--r--   0 sarah      (501) staff       (20)     4156 2023-08-04 22:41:42.000000 ml-stars-0.1.2/ml_stars.egg-info/SOURCES.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        1 2023-08-04 22:41:42.000000 ml-stars-0.1.2/ml_stars.egg-info/dependency_links.txt
+-rw-r--r--   0 sarah      (501) staff       (20)       91 2023-08-04 22:41:42.000000 ml-stars-0.1.2/ml_stars.egg-info/entry_points.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        1 2023-08-04 22:41:42.000000 ml-stars-0.1.2/ml_stars.egg-info/not-zip-safe
+-rw-r--r--   0 sarah      (501) staff       (20)      680 2023-08-04 22:41:42.000000 ml-stars-0.1.2/ml_stars.egg-info/requires.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        8 2023-08-04 22:41:42.000000 ml-stars-0.1.2/ml_stars.egg-info/top_level.txt
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-08-04 22:41:42.483986 ml-stars-0.1.2/mlstars/
+-rw-r--r--   0 sarah      (501) staff       (20)      436 2023-08-04 22:41:36.000000 ml-stars-0.1.2/mlstars/__init__.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-08-04 22:41:42.485153 ml-stars-0.1.2/mlstars/adapters/
+-rw-r--r--   0 sarah      (501) staff       (20)        0 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/adapters/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)     4088 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/adapters/keras.py
+-rw-r--r--   0 sarah      (501) staff       (20)     3449 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/adapters/pandas.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1731 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/adapters/statsmodels.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-08-04 22:41:42.486104 ml-stars-0.1.2/mlstars/custom/
+-rw-r--r--   0 sarah      (501) staff       (20)        0 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/custom/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)    16626 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/custom/timeseries_anomalies.py
+-rw-r--r--   0 sarah      (501) staff       (20)     9471 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/custom/timeseries_preprocessing.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-08-04 22:41:42.502126 ml-stars-0.1.2/mlstars/primitives/
+-rw-r--r--   0 sarah      (501) staff       (20)     5005 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/keras.Sequential.DoubleLSTMTimeSeriesClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     4499 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/keras.Sequential.LSTMTimeSeriesClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     5176 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/keras.Sequential.LSTMTimeSeriesRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1902 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/mlstars.custom.timeseries_anomalies.find_anomalies.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1244 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/mlstars.custom.timeseries_anomalies.regression_errors.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1173 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/mlstars.custom.timeseries_preprocessing.cutoff_window_sequences.json
+-rw-r--r--   0 sarah      (501) staff       (20)      870 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/mlstars.custom.timeseries_preprocessing.intervals_to_mask.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2027 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/mlstars.custom.timeseries_preprocessing.rolling_window_sequences.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1524 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/mlstars.custom.timeseries_preprocessing.time_segments_aggregate.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1099 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/mlstars.custom.timeseries_preprocessing.time_segments_average.json
+-rw-r--r--   0 sarah      (501) staff       (20)      847 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/numpy.argmax.json
+-rw-r--r--   0 sarah      (501) staff       (20)      821 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/numpy.ravel.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1014 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/numpy.reshape.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1607 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.append.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1621 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.drop.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1399 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.drop_duplicates.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1579 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.dropna.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1738 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.fillna.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1686 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.filter.json
+-rw-r--r--   0 sarah      (501) staff       (20)      998 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.get.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1948 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.join.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1521 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.json
+-rw-r--r--   0 sarah      (501) staff       (20)      947 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.pop.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2273 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.resample.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1346 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.select_dtypes.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1047 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.set.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1817 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.set_index.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1346 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.to_numpy.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1243 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.unstack.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1224 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/pandas.Series.filter.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2238 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/sklearn.decomposition.PCA.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1890 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/sklearn.ensemble.AdaBoostClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1914 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/sklearn.ensemble.AdaBoostRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     4782 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/sklearn.ensemble.GradientBoostingClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     5015 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/sklearn.ensemble.GradientBoostingRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2565 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/sklearn.ensemble.IsolationForest.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3721 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/sklearn.ensemble.RandomForestClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     3909 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/sklearn.ensemble.RandomForestRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1765 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/sklearn.impute.SimpleImputer.json
+-rw-r--r--   0 sarah      (501) staff       (20)     5411 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/sklearn.linear_model.Lasso.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2378 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/sklearn.linear_model.LinearRegression.json
+-rw-r--r--   0 sarah      (501) staff       (20)     7498 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/sklearn.linear_model.LogisticRegression.json
+-rw-r--r--   0 sarah      (501) staff       (20)     4365 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/sklearn.linear_model.Ridge.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2459 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/sklearn.neighbors.KNeighborsClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2401 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/sklearn.neighbors.KNeighborsRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1663 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/sklearn.preprocessing.MinMaxScaler.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1321 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/sklearn.preprocessing.OneHotEncoder.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1262 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/sklearn.preprocessing.StandardScaler.json
+-rw-r--r--   0 sarah      (501) staff       (20)     1366 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/statsmodels.tsa.arima_model.Arima.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2226 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/xgboost.XGBClassifier.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2220 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/primitives/xgboost.XGBRegressor.json
+-rw-r--r--   0 sarah      (501) staff       (20)     2941 2023-08-04 22:29:11.000000 ml-stars-0.1.2/mlstars/utils.py
+-rw-r--r--   0 sarah      (501) staff       (20)      983 2023-08-04 22:41:42.505489 ml-stars-0.1.2/setup.cfg
+-rw-r--r--   0 sarah      (501) staff       (20)     2843 2023-08-04 22:41:36.000000 ml-stars-0.1.2/setup.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-08-04 22:41:42.502742 ml-stars-0.1.2/tests/
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-08-04 22:41:42.503695 ml-stars-0.1.2/tests/adapters/
+-rw-r--r--   0 sarah      (501) staff       (20)     1836 2023-08-04 22:29:11.000000 ml-stars-0.1.2/tests/adapters/test_keras.py
+-rw-r--r--   0 sarah      (501) staff       (20)     5027 2023-08-04 22:29:11.000000 ml-stars-0.1.2/tests/adapters/test_pandas.py
+-rw-r--r--   0 sarah      (501) staff       (20)     1961 2023-08-04 22:29:11.000000 ml-stars-0.1.2/tests/adapters/test_statsmodels.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-08-04 22:41:42.504308 ml-stars-0.1.2/tests/custom/
+-rw-r--r--   0 sarah      (501) staff       (20)     7362 2023-08-04 22:29:11.000000 ml-stars-0.1.2/tests/custom/test_timeseries_anomalies.py
+-rw-r--r--   0 sarah      (501) staff       (20)    15169 2023-08-04 22:29:11.000000 ml-stars-0.1.2/tests/custom/test_timeseries_preprocessing.py
+-rw-r--r--   0 sarah      (501) staff       (20)      442 2023-08-04 22:29:11.000000 ml-stars-0.1.2/tests/test_mlstars.py
+-rw-r--r--   0 sarah      (501) staff       (20)      217 2023-08-04 22:29:11.000000 ml-stars-0.1.2/tests/test_utils.py
```

### Comparing `ml-stars-0.1.1.dev1/CONTRIBUTING.rst` & `ml-stars-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/LICENSE` & `ml-stars-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/PKG-INFO` & `ml-stars-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: ml-stars
-Version: 0.1.1.dev1
+Version: 0.1.2
 Summary: Primitives and Pipelines for Time Series Data.
 Home-page: https://github.com/sintel-dev/ml-stars
 Author: MIT Data To AI Lab
 Author-email: dailabmit@gmail.com
 License: MIT license
 Keywords: mlstars
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6,<3.9
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.6,<3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 <p align="left">
@@ -51,15 +52,15 @@
 There is also a collection of custom primitives contributed directly to this library, which either
 combine third party tools or implement new functionalities from scratch.
 
 # Installation
 
 ## Requirements
 
-**ml-stars** has been developed and tested on [Python 3.6, 3.7 and 3.8](https://www.python.org/downloads/)
+**ml-stars** has been developed and tested on [Python 3.6, 3.7, 3.8, and 3.9](https://www.python.org/downloads/)
 
 Also, although it is not strictly required, the usage of a
 [virtualenv](https://virtualenv.pypa.io/en/latest/) is highly recommended in order to avoid
 interfering with other software installed in the system where **ml-stars** is run.
 
 ## Install with pip
 
@@ -148,12 +149,19 @@
 
 The data is now in [0, 1] range.
 
 ## What's Next?
 
 Documentation
 
+
 # History
 
-## 0.1.1 - 2023-04-18
+## 0.1.1 - 2023-05-17
+
+* Fix ARIMA adapter [Issue #5](https://github.com/sintel-dev/ml-stars/issues/5) - by @sarahmish
+* Add Documentation [Issue #4](https://github.com/sintel-dev/ml-stars/issues/4) - by @sarahmish
+
+
+## 0.1.0 - 2023-04-18
 
 First official ml-stars release to PyPI: https://pypi.org/project/ml-stars/
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: ml-stars Version: 0.1.1.dev1 Summary: Primitives
-and Pipelines for Time Series Data. Home-page: https://github.com/sintel-dev/
-ml-stars Author: MIT Data To AI Lab Author-email: dailabmit@gmail.com License:
-MIT license Keywords: mlstars Classifier: Development Status :: 2 - Pre-Alpha
+Metadata-Version: 2.1 Name: ml-stars Version: 0.1.2 Summary: Primitives and
+Pipelines for Time Series Data. Home-page: https://github.com/sintel-dev/ml-
+stars Author: MIT Data To AI Lab Author-email: dailabmit@gmail.com License: MIT
+license Keywords: mlstars Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Requires-Python: >=3.6,<3.9 Description-Content-Type:
-text/markdown Provides-Extra: test Provides-Extra: dev License-File: LICENSE
-License-File: AUTHORS.rst
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.6,<3.10 Description-Content-Type: text/markdown Provides-
+Extra: test Provides-Extra: dev License-File: LICENSE License-File: AUTHORS.rst
 [DAI-Lab] An Open Source Project from the Data_to_AI_Lab,_at_MIT
 [![Development Status](https://img.shields.io/badge/Development%20Status-2%20--
 %20Pre--Alpha-yellow)](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-
 +Pre-Alpha) [![PyPi Shield](https://img.shields.io/pypi/v/ml-stars.svg)](https:
 //pypi.python.org/pypi/ml-stars) [![Tests](https://github.com/sintel-dev/ml-
 stars/workflows/Run%20Tests/badge.svg)](https://github.com/sintel-dev/ml-stars/
 actions?query=workflow%3A%22Run+Tests%22+branch%3Amaster) [![Downloads](https:/
@@ -24,15 +24,15 @@
 Development Status: [Pre-Alpha](https://pypi.org/search/
 ?c=Development+Status+%3A%3A+2+-+Pre-Alpha) # Overview This repository contains
 primitive annotations to be used by the MLBlocks library, as well as the
 necessary Python code to make some of them fully compatible with the MLBlocks
 API requirements. There is also a collection of custom primitives contributed
 directly to this library, which either combine third party tools or implement
 new functionalities from scratch. # Installation ## Requirements **ml-stars**
-has been developed and tested on [Python 3.6, 3.7 and 3.8](https://
+has been developed and tested on [Python 3.6, 3.7, 3.8, and 3.9](https://
 www.python.org/downloads/) Also, although it is not strictly required, the
 usage of a [virtualenv](https://virtualenv.pypa.io/en/latest/) is highly
 recommended in order to avoid interfering with other software installed in the
 system where **ml-stars** is run. ## Install with pip The easiest and
 recommended way to install **ml-stars** is using [pip](https://pip.pypa.io/en/
 stable/): ```bash pip install ml-stars ``` This will pull and install the
 latest stable release from [PyPi](https://pypi.org/). If you want to install
@@ -58,9 +58,12 @@
 ```python3 primitive.fit(X=data) ``` ### 4. Produce results Once the pipeline
 is fit, we can process the data by calling the `produce` method of the
 primitive instance and passing agin the `data` as `X`. ```python3 transformed =
 primitive.produce(X=data) transformed ``` After this is done, we can see how
 the transformed data contains the transformed values: ``` array([[0.78571429],
 [0.14285714], [0.28571429], [0. ], [0.42857143], [0.5 ], [0.07142857],
 [0.35714286], [1. ], [0.35714286]]) ``` The data is now in [0, 1] range. ##
-What's Next? Documentation # History ## 0.1.1 - 2023-04-18 First official ml-
-stars release to PyPI: https://pypi.org/project/ml-stars/
+What's Next? Documentation # History ## 0.1.1 - 2023-05-17 * Fix ARIMA adapter
+[Issue #5](https://github.com/sintel-dev/ml-stars/issues/5) - by @sarahmish *
+Add Documentation [Issue #4](https://github.com/sintel-dev/ml-stars/issues/4) -
+by @sarahmish ## 0.1.0 - 2023-04-18 First official ml-stars release to PyPI:
+https://pypi.org/project/ml-stars/
```

### Comparing `ml-stars-0.1.1.dev1/README.md` & `ml-stars-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 There is also a collection of custom primitives contributed directly to this library, which either
 combine third party tools or implement new functionalities from scratch.
 
 # Installation
 
 ## Requirements
 
-**ml-stars** has been developed and tested on [Python 3.6, 3.7 and 3.8](https://www.python.org/downloads/)
+**ml-stars** has been developed and tested on [Python 3.6, 3.7, 3.8, and 3.9](https://www.python.org/downloads/)
 
 Also, although it is not strictly required, the usage of a
 [virtualenv](https://virtualenv.pypa.io/en/latest/) is highly recommended in order to avoid
 interfering with other software installed in the system where **ml-stars** is run.
 
 ## Install with pip
 
@@ -122,8 +122,8 @@
        [0.35714286]])
 ```
 
 The data is now in [0, 1] range.
 
 ## What's Next?
 
-Documentation
+Documentation
```

#### html2text {}

```diff
@@ -13,15 +13,15 @@
 Development Status: [Pre-Alpha](https://pypi.org/search/
 ?c=Development+Status+%3A%3A+2+-+Pre-Alpha) # Overview This repository contains
 primitive annotations to be used by the MLBlocks library, as well as the
 necessary Python code to make some of them fully compatible with the MLBlocks
 API requirements. There is also a collection of custom primitives contributed
 directly to this library, which either combine third party tools or implement
 new functionalities from scratch. # Installation ## Requirements **ml-stars**
-has been developed and tested on [Python 3.6, 3.7 and 3.8](https://
+has been developed and tested on [Python 3.6, 3.7, 3.8, and 3.9](https://
 www.python.org/downloads/) Also, although it is not strictly required, the
 usage of a [virtualenv](https://virtualenv.pypa.io/en/latest/) is highly
 recommended in order to avoid interfering with other software installed in the
 system where **ml-stars** is run. ## Install with pip The easiest and
 recommended way to install **ml-stars** is using [pip](https://pip.pypa.io/en/
 stable/): ```bash pip install ml-stars ``` This will pull and install the
 latest stable release from [PyPi](https://pypi.org/). If you want to install
```

### Comparing `ml-stars-0.1.1.dev1/docs/Makefile` & `ml-stars-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/docs/conf.py` & `ml-stars-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/docs/developer_guides/adapters.rst` & `ml-stars-0.1.2/docs/developer_guides/adapters.rst`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/docs/developer_guides/annotations.rst` & `ml-stars-0.1.2/docs/developer_guides/annotations.rst`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/docs/developer_guides/contributing.rst` & `ml-stars-0.1.2/docs/developer_guides/contributing.rst`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/docs/developer_guides/custom.rst` & `ml-stars-0.1.2/docs/developer_guides/custom.rst`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/docs/developer_guides/index.rst` & `ml-stars-0.1.2/docs/developer_guides/index.rst`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/docs/getting_started/concepts.rst` & `ml-stars-0.1.2/docs/getting_started/concepts.rst`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/docs/getting_started/install.rst` & `ml-stars-0.1.2/docs/getting_started/install.rst`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/docs/getting_started/quickstart.rst` & `ml-stars-0.1.2/docs/getting_started/quickstart.rst`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/docs/images/dai-logo-white-200.png` & `ml-stars-0.1.2/docs/images/dai-logo-white-200.png`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/docs/index.rst` & `ml-stars-0.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/docs/make.bat` & `ml-stars-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/ml_stars.egg-info/PKG-INFO` & `ml-stars-0.1.2/ml_stars.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: ml-stars
-Version: 0.1.1.dev1
+Version: 0.1.2
 Summary: Primitives and Pipelines for Time Series Data.
 Home-page: https://github.com/sintel-dev/ml-stars
 Author: MIT Data To AI Lab
 Author-email: dailabmit@gmail.com
 License: MIT license
 Keywords: mlstars
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6,<3.9
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.6,<3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 <p align="left">
@@ -51,15 +52,15 @@
 There is also a collection of custom primitives contributed directly to this library, which either
 combine third party tools or implement new functionalities from scratch.
 
 # Installation
 
 ## Requirements
 
-**ml-stars** has been developed and tested on [Python 3.6, 3.7 and 3.8](https://www.python.org/downloads/)
+**ml-stars** has been developed and tested on [Python 3.6, 3.7, 3.8, and 3.9](https://www.python.org/downloads/)
 
 Also, although it is not strictly required, the usage of a
 [virtualenv](https://virtualenv.pypa.io/en/latest/) is highly recommended in order to avoid
 interfering with other software installed in the system where **ml-stars** is run.
 
 ## Install with pip
 
@@ -148,12 +149,19 @@
 
 The data is now in [0, 1] range.
 
 ## What's Next?
 
 Documentation
 
+
 # History
 
-## 0.1.1 - 2023-04-18
+## 0.1.1 - 2023-05-17
+
+* Fix ARIMA adapter [Issue #5](https://github.com/sintel-dev/ml-stars/issues/5) - by @sarahmish
+* Add Documentation [Issue #4](https://github.com/sintel-dev/ml-stars/issues/4) - by @sarahmish
+
+
+## 0.1.0 - 2023-04-18
 
 First official ml-stars release to PyPI: https://pypi.org/project/ml-stars/
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: ml-stars Version: 0.1.1.dev1 Summary: Primitives
-and Pipelines for Time Series Data. Home-page: https://github.com/sintel-dev/
-ml-stars Author: MIT Data To AI Lab Author-email: dailabmit@gmail.com License:
-MIT license Keywords: mlstars Classifier: Development Status :: 2 - Pre-Alpha
+Metadata-Version: 2.1 Name: ml-stars Version: 0.1.2 Summary: Primitives and
+Pipelines for Time Series Data. Home-page: https://github.com/sintel-dev/ml-
+stars Author: MIT Data To AI Lab Author-email: dailabmit@gmail.com License: MIT
+license Keywords: mlstars Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Requires-Python: >=3.6,<3.9 Description-Content-Type:
-text/markdown Provides-Extra: test Provides-Extra: dev License-File: LICENSE
-License-File: AUTHORS.rst
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.6,<3.10 Description-Content-Type: text/markdown Provides-
+Extra: test Provides-Extra: dev License-File: LICENSE License-File: AUTHORS.rst
 [DAI-Lab] An Open Source Project from the Data_to_AI_Lab,_at_MIT
 [![Development Status](https://img.shields.io/badge/Development%20Status-2%20--
 %20Pre--Alpha-yellow)](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-
 +Pre-Alpha) [![PyPi Shield](https://img.shields.io/pypi/v/ml-stars.svg)](https:
 //pypi.python.org/pypi/ml-stars) [![Tests](https://github.com/sintel-dev/ml-
 stars/workflows/Run%20Tests/badge.svg)](https://github.com/sintel-dev/ml-stars/
 actions?query=workflow%3A%22Run+Tests%22+branch%3Amaster) [![Downloads](https:/
@@ -24,15 +24,15 @@
 Development Status: [Pre-Alpha](https://pypi.org/search/
 ?c=Development+Status+%3A%3A+2+-+Pre-Alpha) # Overview This repository contains
 primitive annotations to be used by the MLBlocks library, as well as the
 necessary Python code to make some of them fully compatible with the MLBlocks
 API requirements. There is also a collection of custom primitives contributed
 directly to this library, which either combine third party tools or implement
 new functionalities from scratch. # Installation ## Requirements **ml-stars**
-has been developed and tested on [Python 3.6, 3.7 and 3.8](https://
+has been developed and tested on [Python 3.6, 3.7, 3.8, and 3.9](https://
 www.python.org/downloads/) Also, although it is not strictly required, the
 usage of a [virtualenv](https://virtualenv.pypa.io/en/latest/) is highly
 recommended in order to avoid interfering with other software installed in the
 system where **ml-stars** is run. ## Install with pip The easiest and
 recommended way to install **ml-stars** is using [pip](https://pip.pypa.io/en/
 stable/): ```bash pip install ml-stars ``` This will pull and install the
 latest stable release from [PyPi](https://pypi.org/). If you want to install
@@ -58,9 +58,12 @@
 ```python3 primitive.fit(X=data) ``` ### 4. Produce results Once the pipeline
 is fit, we can process the data by calling the `produce` method of the
 primitive instance and passing agin the `data` as `X`. ```python3 transformed =
 primitive.produce(X=data) transformed ``` After this is done, we can see how
 the transformed data contains the transformed values: ``` array([[0.78571429],
 [0.14285714], [0.28571429], [0. ], [0.42857143], [0.5 ], [0.07142857],
 [0.35714286], [1. ], [0.35714286]]) ``` The data is now in [0, 1] range. ##
-What's Next? Documentation # History ## 0.1.1 - 2023-04-18 First official ml-
-stars release to PyPI: https://pypi.org/project/ml-stars/
+What's Next? Documentation # History ## 0.1.1 - 2023-05-17 * Fix ARIMA adapter
+[Issue #5](https://github.com/sintel-dev/ml-stars/issues/5) - by @sarahmish *
+Add Documentation [Issue #4](https://github.com/sintel-dev/ml-stars/issues/4) -
+by @sarahmish ## 0.1.0 - 2023-04-18 First official ml-stars release to PyPI:
+https://pypi.org/project/ml-stars/
```

### Comparing `ml-stars-0.1.1.dev1/ml_stars.egg-info/SOURCES.txt` & `ml-stars-0.1.2/ml_stars.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/ml_stars.egg-info/requires.txt` & `ml-stars-0.1.2/ml_stars.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-Keras<2.5,>=2.4
-mlblocks<0.6,>=0.4
+Keras<2.13,>=2.4
+mlblocks>=0.6
 numpy<1.21.0,>=1.16.0
 pandas<2,>=1
 scikit-learn<1.2,>=0.21
 scipy<2,>=1.1.0
 statsmodels<0.13,>=0.9.0
-tensorflow<2.5,>=2
+tensorflow<2.13,>=2
 xgboost<1,>=0.72.1
 protobuf<4
 
 [dev]
 bumpversion<0.6,>=0.5.3
 pip>=9.0.1
 watchdog<0.11,>=0.8.3
```

### Comparing `ml-stars-0.1.1.dev1/mlstars/adapters/keras.py` & `ml-stars-0.1.2/mlstars/adapters/keras.py`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/adapters/pandas.py` & `ml-stars-0.1.2/mlstars/adapters/pandas.py`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/adapters/statsmodels.py` & `ml-stars-0.1.2/mlstars/adapters/statsmodels.py`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/custom/timeseries_anomalies.py` & `ml-stars-0.1.2/mlstars/custom/timeseries_anomalies.py`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/custom/timeseries_preprocessing.py` & `ml-stars-0.1.2/mlstars/custom/timeseries_preprocessing.py`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/keras.Sequential.DoubleLSTMTimeSeriesClassifier.json` & `ml-stars-0.1.2/mlstars/primitives/keras.Sequential.DoubleLSTMTimeSeriesClassifier.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/keras.Sequential.LSTMTimeSeriesClassifier.json` & `ml-stars-0.1.2/mlstars/primitives/keras.Sequential.LSTMTimeSeriesClassifier.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/keras.Sequential.LSTMTimeSeriesRegressor.json` & `ml-stars-0.1.2/mlstars/primitives/keras.Sequential.LSTMTimeSeriesRegressor.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/mlstars.custom.timeseries_anomalies.find_anomalies.json` & `ml-stars-0.1.2/mlstars/primitives/mlstars.custom.timeseries_anomalies.find_anomalies.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/mlstars.custom.timeseries_anomalies.regression_errors.json` & `ml-stars-0.1.2/mlstars/primitives/mlstars.custom.timeseries_anomalies.regression_errors.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/mlstars.custom.timeseries_preprocessing.cutoff_window_sequences.json` & `ml-stars-0.1.2/mlstars/primitives/mlstars.custom.timeseries_preprocessing.cutoff_window_sequences.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/mlstars.custom.timeseries_preprocessing.intervals_to_mask.json` & `ml-stars-0.1.2/mlstars/primitives/mlstars.custom.timeseries_preprocessing.intervals_to_mask.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/mlstars.custom.timeseries_preprocessing.rolling_window_sequences.json` & `ml-stars-0.1.2/mlstars/primitives/mlstars.custom.timeseries_preprocessing.rolling_window_sequences.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/mlstars.custom.timeseries_preprocessing.time_segments_aggregate.json` & `ml-stars-0.1.2/mlstars/primitives/mlstars.custom.timeseries_preprocessing.time_segments_aggregate.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/mlstars.custom.timeseries_preprocessing.time_segments_average.json` & `ml-stars-0.1.2/mlstars/primitives/mlstars.custom.timeseries_preprocessing.time_segments_average.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/numpy.argmax.json` & `ml-stars-0.1.2/mlstars/primitives/numpy.argmax.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/numpy.ravel.json` & `ml-stars-0.1.2/mlstars/primitives/numpy.ravel.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/numpy.reshape.json` & `ml-stars-0.1.2/mlstars/primitives/numpy.reshape.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.append.json` & `ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.append.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.drop.json` & `ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.drop.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.drop_duplicates.json` & `ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.drop_duplicates.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.dropna.json` & `ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.dropna.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.fillna.json` & `ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.fillna.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.filter.json` & `ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.filter.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.get.json` & `ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.get.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.join.json` & `ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.join.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.json` & `ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.pop.json` & `ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.pop.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.resample.json` & `ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.resample.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.select_dtypes.json` & `ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.select_dtypes.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.set.json` & `ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.set.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.set_index.json` & `ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.set_index.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.to_numpy.json` & `ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.to_numpy.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/pandas.DataFrame.unstack.json` & `ml-stars-0.1.2/mlstars/primitives/pandas.DataFrame.unstack.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/pandas.Series.filter.json` & `ml-stars-0.1.2/mlstars/primitives/pandas.Series.filter.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.decomposition.PCA.json` & `ml-stars-0.1.2/mlstars/primitives/sklearn.decomposition.PCA.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.ensemble.AdaBoostClassifier.json` & `ml-stars-0.1.2/mlstars/primitives/sklearn.ensemble.AdaBoostClassifier.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.ensemble.AdaBoostRegressor.json` & `ml-stars-0.1.2/mlstars/primitives/sklearn.ensemble.AdaBoostRegressor.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.ensemble.GradientBoostingClassifier.json` & `ml-stars-0.1.2/mlstars/primitives/sklearn.ensemble.GradientBoostingClassifier.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.ensemble.GradientBoostingRegressor.json` & `ml-stars-0.1.2/mlstars/primitives/sklearn.ensemble.GradientBoostingRegressor.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.ensemble.IsolationForest.json` & `ml-stars-0.1.2/mlstars/primitives/sklearn.ensemble.IsolationForest.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.ensemble.RandomForestClassifier.json` & `ml-stars-0.1.2/mlstars/primitives/sklearn.ensemble.RandomForestClassifier.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.ensemble.RandomForestRegressor.json` & `ml-stars-0.1.2/mlstars/primitives/sklearn.ensemble.RandomForestRegressor.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.impute.SimpleImputer.json` & `ml-stars-0.1.2/mlstars/primitives/sklearn.impute.SimpleImputer.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.linear_model.Lasso.json` & `ml-stars-0.1.2/mlstars/primitives/sklearn.linear_model.Lasso.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.linear_model.LinearRegression.json` & `ml-stars-0.1.2/mlstars/primitives/sklearn.linear_model.LinearRegression.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.linear_model.LogisticRegression.json` & `ml-stars-0.1.2/mlstars/primitives/sklearn.linear_model.LogisticRegression.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.linear_model.Ridge.json` & `ml-stars-0.1.2/mlstars/primitives/sklearn.linear_model.Ridge.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.neighbors.KNeighborsClassifier.json` & `ml-stars-0.1.2/mlstars/primitives/sklearn.neighbors.KNeighborsClassifier.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.neighbors.KNeighborsRegressor.json` & `ml-stars-0.1.2/mlstars/primitives/sklearn.neighbors.KNeighborsRegressor.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.preprocessing.MinMaxScaler.json` & `ml-stars-0.1.2/mlstars/primitives/sklearn.preprocessing.MinMaxScaler.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.preprocessing.OneHotEncoder.json` & `ml-stars-0.1.2/mlstars/primitives/sklearn.preprocessing.OneHotEncoder.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/sklearn.preprocessing.StandardScaler.json` & `ml-stars-0.1.2/mlstars/primitives/sklearn.preprocessing.StandardScaler.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/statsmodels.tsa.arima_model.Arima.json` & `ml-stars-0.1.2/mlstars/primitives/statsmodels.tsa.arima_model.Arima.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/xgboost.XGBClassifier.json` & `ml-stars-0.1.2/mlstars/primitives/xgboost.XGBClassifier.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/primitives/xgboost.XGBRegressor.json` & `ml-stars-0.1.2/mlstars/primitives/xgboost.XGBRegressor.json`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/mlstars/utils.py` & `ml-stars-0.1.2/mlstars/utils.py`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/setup.cfg` & `ml-stars-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.1.dev1
+current_version = 0.1.2
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `ml-stars-0.1.1.dev1/setup.py` & `ml-stars-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.md', encoding='utf-8') as history_file:
     history = history_file.read()
 
 install_requires = [
-    'Keras>=2.4,<2.5',
-    'mlblocks>=0.4,<0.6',
+    'Keras>=2.4,<2.13',
+    'mlblocks>=0.6',
     'numpy<1.21.0,>=1.16.0',
     'pandas>=1,<2',
     'scikit-learn>=0.21,<1.2',
     'scipy>=1.1.0,<2',
     'statsmodels>=0.9.0,<0.13',
-    'tensorflow>=2,<2.5',
+    'tensorflow>=2,<2.13',
     'xgboost>=0.72.1,<1',
 
     # fix google/protobuf/descriptor
     'protobuf<4',
 ]
 
 setup_requires = [
@@ -78,14 +78,15 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
     ],
     description='Primitives and Pipelines for Time Series Data.',
     entry_points={
         'mlblocks': [
             'primitives=mlstars:MLBLOCKS_PRIMITIVES',
             'pipelines=mlstars:MLBLOCKS_PIPELINES'
         ],
@@ -99,15 +100,15 @@
     license='MIT license',
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     include_package_data=True,
     keywords='mlstars',
     name='ml-stars',
     packages=find_packages(include=['mlstars', 'mlstars.*']),
-    python_requires='>=3.6,<3.9',
+    python_requires='>=3.6,<3.10',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sintel-dev/ml-stars',
-    version='0.1.1.dev1',
+    version='0.1.2',
     zip_safe=False,
 )
```

### Comparing `ml-stars-0.1.1.dev1/tests/adapters/test_keras.py` & `ml-stars-0.1.2/tests/adapters/test_keras.py`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/tests/adapters/test_pandas.py` & `ml-stars-0.1.2/tests/adapters/test_pandas.py`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/tests/adapters/test_statsmodels.py` & `ml-stars-0.1.2/tests/adapters/test_statsmodels.py`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/tests/custom/test_timeseries_anomalies.py` & `ml-stars-0.1.2/tests/custom/test_timeseries_anomalies.py`

 * *Files identical despite different names*

### Comparing `ml-stars-0.1.1.dev1/tests/custom/test_timeseries_preprocessing.py` & `ml-stars-0.1.2/tests/custom/test_timeseries_preprocessing.py`

 * *Files identical despite different names*

