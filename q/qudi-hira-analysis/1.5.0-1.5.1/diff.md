# Comparing `tmp/qudi_hira_analysis-1.5.0.tar.gz` & `tmp/qudi_hira_analysis-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qudi_hira_analysis-1.5.0.tar", max compression
+gzip compressed data, was "qudi_hira_analysis-1.5.1.tar", max compression
```

## Comparing `qudi_hira_analysis-1.5.0.tar` & `qudi_hira_analysis-1.5.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1069 2023-02-26 15:52:31.954729 qudi_hira_analysis-1.5.0/LICENSE
--rw-r--r--   0        0        0    16332 2023-08-04 06:47:03.161233 qudi_hira_analysis-1.5.0/README.md
--rw-r--r--   0        0        0      928 2023-08-01 00:09:02.716972 qudi_hira_analysis-1.5.0/pyproject.toml
--rw-r--r--   0        0        0      223 2023-07-31 23:15:03.175697 qudi_hira_analysis-1.5.0/qudi_hira_analysis/__init__.py
--rw-r--r--   0        0        0    17870 2023-08-04 06:41:24.509443 qudi_hira_analysis-1.5.0/qudi_hira_analysis/analysis_logic.py
--rw-r--r--   0        0        0    13763 2023-07-31 20:44:03.798915 qudi_hira_analysis-1.5.0/qudi_hira_analysis/data_handler.py
--rw-r--r--   0        0        0        0 2023-03-05 21:19:20.710018 qudi_hira_analysis-1.5.0/qudi_hira_analysis/fitmethods/__init__.py
--rw-r--r--   0        0        0     1936 2023-03-05 21:19:20.710848 qudi_hira_analysis-1.5.0/qudi_hira_analysis/fitmethods/antibunchingmethods.py
--rw-r--r--   0        0        0    24480 2023-03-05 21:19:20.711380 qudi_hira_analysis-1.5.0/qudi_hira_analysis/fitmethods/decaylikemethods.py
--rw-r--r--   0        0        0    40854 2023-03-05 21:19:20.711692 qudi_hira_analysis-1.5.0/qudi_hira_analysis/fitmethods/gaussianlikemethods.py
--rw-r--r--   0        0        0    23135 2023-05-04 17:12:59.439365 qudi_hira_analysis-1.5.0/qudi_hira_analysis/fitmethods/generalmethods.py
--rw-r--r--   0        0        0     5848 2023-03-05 21:19:20.712252 qudi_hira_analysis-1.5.0/qudi_hira_analysis/fitmethods/hyperbolicsaturationmethods.py
--rw-r--r--   0        0        0    10577 2023-03-05 21:19:20.712412 qudi_hira_analysis-1.5.0/qudi_hira_analysis/fitmethods/linearmethods.py
--rw-r--r--   0        0        0    41793 2023-08-01 01:02:54.235988 qudi_hira_analysis-1.5.0/qudi_hira_analysis/fitmethods/lorentzianlikemethods.py
--rw-r--r--   0        0        0    16450 2023-03-05 21:19:20.712885 qudi_hira_analysis-1.5.0/qudi_hira_analysis/fitmethods/poissonianlikemethods.py
--rw-r--r--   0        0        0   106110 2023-03-05 21:19:20.713199 qudi_hira_analysis-1.5.0/qudi_hira_analysis/fitmethods/sinemethods.py
--rw-r--r--   0        0        0     1792 2023-04-12 17:43:42.063526 qudi_hira_analysis-1.5.0/qudi_hira_analysis/helper_functions.py
--rw-r--r--   0        0        0    13657 2023-05-04 17:12:59.439937 qudi_hira_analysis-1.5.0/qudi_hira_analysis/io_handler.py
--rw-r--r--   0        0        0     7597 2023-08-01 00:07:31.606918 qudi_hira_analysis-1.5.0/qudi_hira_analysis/measurement_dataclass.py
--rw-r--r--   0        0        0    18711 2023-05-04 17:12:59.440573 qudi_hira_analysis-1.5.0/qudi_hira_analysis/qudi_fit_logic.py
--rw-r--r--   0        0        0    23800 2023-08-04 05:01:38.724738 qudi_hira_analysis-1.5.0/qudi_hira_analysis/raster_odmr_fitting.py
--rw-r--r--   0        0        0    17330 1970-01-01 00:00:00.000000 qudi_hira_analysis-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-02-26 15:52:31.954729 qudi_hira_analysis-1.5.1/LICENSE
+-rw-r--r--   0        0        0     6054 2023-08-04 12:05:24.320963 qudi_hira_analysis-1.5.1/README.md
+-rw-r--r--   0        0        0     1073 2023-08-04 12:16:16.253433 qudi_hira_analysis-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     7338 2023-08-04 12:07:18.173457 qudi_hira_analysis-1.5.1/qudi_hira_analysis/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-05 21:19:20.710018 qudi_hira_analysis-1.5.1/qudi_hira_analysis/_fitmethods/__init__.py
+-rw-r--r--   0        0        0     1936 2023-03-05 21:19:20.710848 qudi_hira_analysis-1.5.1/qudi_hira_analysis/_fitmethods/antibunchingmethods.py
+-rw-r--r--   0        0        0    24480 2023-03-05 21:19:20.711380 qudi_hira_analysis-1.5.1/qudi_hira_analysis/_fitmethods/decaylikemethods.py
+-rw-r--r--   0        0        0    40854 2023-03-05 21:19:20.711692 qudi_hira_analysis-1.5.1/qudi_hira_analysis/_fitmethods/gaussianlikemethods.py
+-rw-r--r--   0        0        0    23135 2023-05-04 17:12:59.439365 qudi_hira_analysis-1.5.1/qudi_hira_analysis/_fitmethods/generalmethods.py
+-rw-r--r--   0        0        0     5848 2023-03-05 21:19:20.712252 qudi_hira_analysis-1.5.1/qudi_hira_analysis/_fitmethods/hyperbolicsaturationmethods.py
+-rw-r--r--   0        0        0    10577 2023-03-05 21:19:20.712412 qudi_hira_analysis-1.5.1/qudi_hira_analysis/_fitmethods/linearmethods.py
+-rw-r--r--   0        0        0    41793 2023-08-01 01:02:54.235988 qudi_hira_analysis-1.5.1/qudi_hira_analysis/_fitmethods/lorentzianlikemethods.py
+-rw-r--r--   0        0        0    16450 2023-03-05 21:19:20.712885 qudi_hira_analysis-1.5.1/qudi_hira_analysis/_fitmethods/poissonianlikemethods.py
+-rw-r--r--   0        0        0   106110 2023-03-05 21:19:20.713199 qudi_hira_analysis-1.5.1/qudi_hira_analysis/_fitmethods/sinemethods.py
+-rw-r--r--   0        0        0    18714 2023-08-04 10:10:24.333159 qudi_hira_analysis-1.5.1/qudi_hira_analysis/_qudi_fit_logic.py
+-rw-r--r--   0        0        0    23800 2023-08-04 05:01:38.724738 qudi_hira_analysis-1.5.1/qudi_hira_analysis/_raster_odmr_fitting.py
+-rw-r--r--   0        0        0    19014 2023-08-04 10:04:17.749129 qudi_hira_analysis-1.5.1/qudi_hira_analysis/analysis_logic.py
+-rw-r--r--   0        0        0    13445 2023-08-04 09:39:52.243740 qudi_hira_analysis-1.5.1/qudi_hira_analysis/data_handler.py
+-rw-r--r--   0        0        0     1792 2023-04-12 17:43:42.063526 qudi_hira_analysis-1.5.1/qudi_hira_analysis/helper_functions.py
+-rw-r--r--   0        0        0    15592 2023-08-04 09:58:04.128172 qudi_hira_analysis-1.5.1/qudi_hira_analysis/io_handler.py
+-rw-r--r--   0        0        0     7960 2023-08-04 09:41:43.896562 qudi_hira_analysis-1.5.1/qudi_hira_analysis/measurement_dataclass.py
+-rw-r--r--   0        0        0     7149 1970-01-01 00:00:00.000000 qudi_hira_analysis-1.5.1/PKG-INFO
```

### Comparing `qudi_hira_analysis-1.5.0/LICENSE` & `qudi_hira_analysis-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.5.0/pyproject.toml` & `qudi_hira_analysis-1.5.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [tool.poetry]
 name = "qudi-hira-analysis"
-version = "1.5.0"
+version = "1.5.1"
 repository = "https://github.com/dineshpinto/qudi-hira-analysis"
 homepage = "https://github.com/dineshpinto/qudi-hira-analysis"
+documentation = "https://dineshpinto.github.io/qudi-hira-analysis/qudi_hira_analysis/"
 keywords = ["python", "qubit", "analysis", "nv centers", "photon timetrace"]
 description = "A Python toolkit to analzye photon timetrace data from qubit sensors"
 authors = ["dineshpinto <annual.fallout_0z@icloud.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "qudi_hira_analysis" }]
 
@@ -26,10 +27,14 @@
 jupyterlab = "^3.6.2"
 notebook = "^6.5.4"
 
 
 [tool.poetry.group.test.dependencies]
 coverage = "^7.2.5"
 
+
+[tool.poetry.group.docs.dependencies]
+pdoc3 = "^0.10.0"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `qudi_hira_analysis-1.5.0/qudi_hira_analysis/analysis_logic.py` & `qudi_hira_analysis-1.5.1/qudi_hira_analysis/analysis_logic.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,25 +7,30 @@
 from typing import Tuple, TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
 from joblib import Parallel, delayed, cpu_count
 from tqdm import tqdm
 
-import qudi_hira_analysis.raster_odmr_fitting as rof
-from qudi_hira_analysis.qudi_fit_logic import FitLogic
+import qudi_hira_analysis._raster_odmr_fitting as rof
+from qudi_hira_analysis._qudi_fit_logic import FitLogic
 
 if TYPE_CHECKING:
     from lmfit.model import ModelResult, Parameter
     from .measurement_dataclass import MeasurementDataclass
 
 logging.basicConfig(format='%(name)s :: %(levelname)s :: %(message)s', level=logging.INFO)
 
 
 class FitMethodsAndEstimators:
+    """
+        Class for storing fit methods and estimators.
+        Fit methods are stored as tuples of (method, estimator)
+        where method is the name of the fit method and estimator is the name of the estimator.
+    """
     # Fit methods with corresponding estimators
     antibunching: tuple = ("antibunching", "dip")
     hyperbolicsaturation: tuple = ("hyperbolicsaturation", "generic")
     lorentzian: tuple = ("lorentzian", "dip")
     lorentziandouble: tuple = ("lorentziandouble", "dip")
     sineexponentialdecay: tuple = ("sineexponentialdecay", "generic")
     decayexponential: tuple = ("decayexponential", "generic")
@@ -44,57 +49,31 @@
     sinetriple: tuple = ("sinetriple", "generic")
     sinetriplewithexpdecay: tuple = ("sinetriplewithexpdecay", "generic")
     sinetriplewiththreeexpdecay: tuple = ("sinetriplewiththreeexpdecay", "generic")
     twoDgaussian: tuple = ("twoDgaussian", "generic")
 
 
 class AnalysisLogic(FitLogic):
+    """
+        Class for performing analysis on measurement data
+    """
     fit_function = FitMethodsAndEstimators
 
     def __init__(self):
         super().__init__()
         self.log = logging.getLogger(__name__)
 
     def _perform_fit(
             self,
             x: np.ndarray,
             y: np.ndarray,
             fit_function: str,
             estimator: str,
             parameters: list[Parameter] = None,
             dims: str = "1d") -> Tuple[np.ndarray, np.ndarray, ModelResult]:
-        """
-        Fits available:
-            | Dimension | Fit                           |
-            |-----------|-------------------------------|
-            | 1d        | decayexponential              |
-            |           | biexponential                 |
-            |           | decayexponentialstretched     |
-            |           | gaussian                      |
-            |           | gaussiandouble                |
-            |           | gaussianlinearoffset          |
-            |           | hyperbolicsaturation          |
-            |           | linear                        |
-            |           | lorentzian                    |
-            |           | lorentziandouble              |
-            |           | lorentziantriple              |
-            |           | sine                          |
-            |           | sinedouble                    |
-            |           | sinedoublewithexpdecay        |
-            |           | sinedoublewithtwoexpdecay     |
-            |           | sineexponentialdecay          |
-            |           | sinestretchedexponentialdecay |
-            |           | sinetriple                    |
-            |           | sinetriplewithexpdecay        |
-            |           | sinetriplewiththreeexpdecay   |
-            | 2d        | twoDgaussian                  |
-        Estimators:
-            - generic
-            - dip
-        """
         fit = {dims: {'default': {'fit_function': fit_function, 'estimator': estimator}}}
         user_fit = self.validate_load_fits(fit)
 
         if parameters:
             user_fit[dims]["default"]["parameters"].add_many(*parameters)
 
         use_settings = {}
@@ -118,51 +97,79 @@
             self,
             x: str | np.ndarray | pd.Series,
             y: str | np.ndarray | pd.Series,
             fit_function: FitMethodsAndEstimators,
             data: pd.DataFrame = None,
             parameters: list[Parameter] = None
     ) -> Tuple[np.ndarray, np.ndarray, ModelResult]:
+        """
+        Args:
+            x: x data
+            y: y data
+            fit_function: fit function to use
+            data: pandas DataFrame containing x and y data
+            parameters: list of parameters to use in fit
+
+        Returns:
+            x_fit: x data of fit
+            y_fit: y data of fit
+            result: result of fit
+
+        """
         if "twoD" in fit_function[0]:
-            dims = "2d"
+            dims: str = "2d"
         else:
-            dims = "1d"
+            dims: str = "1d"
 
         if data is None:
             if isinstance(x, pd.Series) or isinstance(x, pd.Index):
-                x = x.to_numpy()
+                x: np.ndarray = x.to_numpy()
             if isinstance(y, pd.Series):
-                y = y.to_numpy()
+                y: np.ndarray = y.to_numpy()
         elif isinstance(data, pd.DataFrame):
-            x = data[x].to_numpy()
-            y = data[y].to_numpy()
+            x: np.ndarray = data[x].to_numpy()
+            y: np.ndarray = data[y].to_numpy()
         else:
             raise TypeError("Data must be a pandas DataFrame or None")
 
         return self._perform_fit(
             x=x,
             y=y,
             fit_function=fit_function[0],
             estimator=fit_function[1],
             parameters=parameters,
             dims=dims
         )
 
     def get_all_fits(self) -> Tuple[list, list]:
-        one_d_fits = list(self.fit_list['1d'].keys())
-        two_d_fits = list(self.fit_list['2d'].keys())
+        one_d_fits: list = list(self.fit_list['1d'].keys())
+        two_d_fits: list = list(self.fit_list['2d'].keys())
         self.log.info(f"1d fits: {one_d_fits}\n2d fits: {two_d_fits}")
         return one_d_fits, two_d_fits
 
     @staticmethod
     def analyse_mean(
             laser_data: np.ndarray,
             signal_start: float = 100e-9,
             signal_end: float = 300e-9,
-            bin_width: float = 1e-9) -> Tuple[np.ndarray, np.ndarray]:
+            bin_width: float = 1e-9
+    ) -> Tuple[np.ndarray, np.ndarray]:
+        """
+        Calculate the mean of the signal window.
+
+        Args:
+            laser_data: 2D array of laser data
+            signal_start: start of the signal window in seconds
+            signal_end: end of the signal window in seconds
+            bin_width: width of a bin in seconds
+
+        Returns:
+            np.ndarray: mean of the signal window
+            np.ndarray: measurement error
+        """
         # Get number of lasers
         num_of_lasers = laser_data.shape[0]
 
         if not isinstance(bin_width, float):
             return np.zeros(num_of_lasers), np.zeros(num_of_lasers)
 
         # Convert the times in seconds to bins (i.e. array indices)
@@ -195,17 +202,27 @@
             laser_data: np.ndarray,
             signal_start: float = 100e-9,
             signal_end: float = 300e-9,
             norm_start: float = 1000e-9,
             norm_end: float = 2000e-9,
             bin_width: float = 1e-9) -> Tuple[np.ndarray, np.ndarray]:
         """
-        This method takes the mean of the signal window.
-        It then does not divide by the background window to normalize
-        but rather substracts the background window to generate the output.
+        Subtracts the mean of the signal window from the mean of the reference window.
+
+        Args:
+            laser_data: 2D array of laser data
+            signal_start: start of the signal window in seconds
+            signal_end: end of the signal window in seconds
+            norm_start: start of the reference window in seconds
+            norm_end: end of the reference window in seconds
+            bin_width: width of a bin in seconds
+
+        Returns:
+            np.ndarray: referenced mean of the signal window
+            np.ndarray: measurement error
         """
         # Get number of lasers
         num_of_lasers = laser_data.shape[0]
 
         if not isinstance(bin_width, float):
             return np.zeros(num_of_lasers), np.zeros(num_of_lasers)
 
@@ -241,15 +258,31 @@
     @staticmethod
     def analyse_mean_norm(
             laser_data: np.ndarray,
             signal_start: float = 100e-9,
             signal_end: float = 300e-9,
             norm_start: float = 1000e-9,
             norm_end=2000e-9,
-            bin_width: float = 1e-9) -> Tuple[np.ndarray, np.ndarray]:
+            bin_width: float = 1e-9
+    ) -> Tuple[np.ndarray, np.ndarray]:
+        """
+        Divides the mean of the signal window from the mean of the reference window.
+
+        Args:
+            laser_data: 2D array of laser data
+            signal_start: start of the signal window in seconds
+            signal_end: end of the signal window in seconds
+            norm_start: start of the reference window in seconds
+            norm_end: end of the reference window in seconds
+            bin_width: width of a bin in seconds
+
+        Returns:
+            np.ndarray: normalized mean of the signal window
+            np.ndarray: measurement error
+        """
         # Get number of lasers
         num_of_lasers = laser_data.shape[0]
 
         if not isinstance(bin_width, float):
             return np.zeros(num_of_lasers), np.zeros(num_of_lasers)
 
         # Convert the times in seconds to bins (i.e. array indices)
@@ -285,15 +318,15 @@
                 # calculate with respect to gaussian error 'evolution'
                 error_data[ii] = signal_data[ii] * np.sqrt(1 / signal_sum + 1 / reference_sum)
             else:
                 error_data[ii] = 0.0
 
         return signal_data, error_data
 
-    def optimize_hyperparameters(
+    def optimize_raster_odmr_params(
             self,
             measurements: dict[str, MeasurementDataclass],
             num_samples: int = 10,
             num_params: int = 3,
     ) -> Tuple[float, Tuple[float, float, float]]:
         """
         This method optimizes the hyperparameters of the ODMR analysis.
@@ -302,72 +335,74 @@
 
         Args:
             measurements: A dictionary of measurements to optimize the hyperparameters for.
             num_params: The number of parameters to optimize.
             num_samples: The number of measurements to sample.
 
         Returns:
-            The optimal hyperparameters.
+            float: The highest minimum r2 value
+            tuple: Optimized hyperparameters.
         """
-        r2_threshs = np.around(np.linspace(start=0.9, stop=0.99, num=num_params), decimals=2)
-        thresh_fracs = np.around(np.linspace(start=0.5, stop=0.9, num=num_params), decimals=1)
-        sigma_thresh_fracs = np.around(np.linspace(start=0.1, stop=0.2, num=num_params), decimals=1)
+        r2_threshs: np.ndarray = np.around(np.linspace(start=0.9, stop=0.99, num=num_params), decimals=2)
+        thresh_fracs: np.ndarray = np.around(np.linspace(start=0.5, stop=0.9, num=num_params), decimals=1)
+        sigma_thresh_fracs: np.ndarray = np.around(np.linspace(start=0.1, stop=0.2, num=num_params), decimals=1)
 
-        odmr_sample = {}
+        odmr_sample: dict = {}
         for k, v in random.sample(sorted(measurements.items()), k=num_samples):
             odmr_sample[k] = v
 
-        highest_min_r2 = 0
-        optimal_params = (0, 0, 0)
+        highest_min_r2: float = 0
+        optimal_params: Tuple[float, float, float] = (0, 0, 0)
 
         for idx, (r2_thresh, thresh_frac, sigma_thresh_frac) in enumerate(
                 product(r2_threshs, thresh_fracs, sigma_thresh_fracs)):
-            odmr_sample = self.raster_odmr_fitting(
+            odmr_sample = self.fit_raster_odmr(
                 odmr_sample,
                 r2_thresh=r2_thresh,
                 thresh_frac=thresh_frac,
                 sigma_thresh_frac=sigma_thresh_frac,
                 min_thresh=0.01,
                 progress_bar=False
             )
 
-            r2s = np.zeros(len(odmr_sample))
+            r2s: np.ndarray = np.zeros(len(odmr_sample))
             for _idx, odmr in enumerate(odmr_sample.values()):
                 r2s[_idx] = odmr.fit_model.rsquared
-            min_r2 = np.min(r2s)
+            min_r2: float = np.min(r2s)
 
             if highest_min_r2 < min_r2:
                 highest_min_r2 = min_r2
                 optimal_params = (r2_thresh, thresh_frac, sigma_thresh_frac)
 
         return highest_min_r2, optimal_params
 
     @staticmethod
-    def raster_odmr_fitting(
+    def fit_raster_odmr(
             odmr_measurements: dict[str, MeasurementDataclass],
             r2_thresh: float = 0.95,
             thresh_frac: float = 0.5,
             sigma_thresh_frac: float = 0.15,
             min_thresh: float = 0.01,
             extract_pixel_from_filename: bool = True,
             progress_bar: bool = True
     ) -> dict[str, MeasurementDataclass]:
         """
         Fit a list of ODMR data to single and double Lorentzian functions
 
         Args:
             odmr_measurements: List of ODMR data in MeasurementDataclasses
             r2_thresh: R^2 Threshold below which a double lorentzian is fitted instead of a single lorentzian
-            thresh_frac:
-            min_thresh:
-            sigma_thresh_frac:
+            thresh_frac: Threshold fraction for the peak finding
+            min_thresh: Minimum threshold for the peak finding
+            sigma_thresh_frac: Change in threshold fraction for the peak finding
             extract_pixel_from_filename: Extract `(row, col)` (in this format) from filename
             progress_bar: Show progress bar
+
         Returns:
-            List of ODMR data with fit, fit model and pixels in MeasurementDataclass
+            dict: ODMR data with fit, fit model and pixels in MeasurementDataclass
         """
 
         model1, base_params1 = rof.make_lorentzian_model()
         model2, base_params2 = rof.make_lorentziandouble_model()
 
         # Generate arguments for the parallel fitting
         args = []
@@ -406,17 +441,24 @@
             if extract_pixel_from_filename:
                 row, col = map(int, re.findall(r'(?<=\().*?(?=\))', odmr.filename)[0].split(","))
                 odmr.xy_position = (row, col)
 
         return odmr_measurements
 
     @staticmethod
-    def pixel_average_nan(orig_image: np.ndarray) -> np.ndarray:
-        """ Average a nan pixel to its surrounding 8 points """
-        image = orig_image.copy()
+    def average_raster_odmr_pixels(orig_image: np.ndarray) -> np.ndarray:
+        """ Average a NaN pixel to its surrounding pixels.
+
+        Args:
+            orig_image: Image with NaN pixels
+
+        Returns:
+            Image with NaN pixels replaced by the average of its surrounding pixels
+        """
+        image: np.ndarray = orig_image.copy()
         for row, col in np.argwhere(np.isnan(image)):
             if row == 0:
                 pixel_avg = np.nanmean(image[row + 1:row + 2, col - 1:col + 2])
             elif row == image.shape[0] - 1:
                 pixel_avg = np.nanmean(image[row - 1:row, col - 1:col + 2])
             elif col == 0:
                 pixel_avg = np.nanmean(image[row - 1:row + 2, col + 1:col + 2])
```

### Comparing `qudi_hira_analysis-1.5.0/qudi_hira_analysis/data_handler.py` & `qudi_hira_analysis-1.5.1/qudi_hira_analysis/data_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,32 +72,27 @@
         )
 
 
 class DataHandler(DataLoader, AnalysisLogic):
     """
     Handles automated data searching and extraction into dataclasses.
 
-    Parameters
-    ----------
-        data_folder: pathlib.Path
-            Path to the data folder.
-        figure_folder: pathlib.Path
-            Path to the figure folder.
-        measurement_folder: str or pathlib.Path
-            Path to the measurement folder.
-
-    Examples
-    --------
-    Create an instance of the DataHandler class:
-
-    >>> dh = DataHandler(
-    >>>     data_folder=Path('C:\\'', 'Data'),
-    >>>     figure_folder=Path('C:\\'', 'QudiHiraAnalysis'),
-    >>>     measurement_folder=Path('20230101_Bakeout'),
-    >>> )
+    Parameters:
+        data_folder: Path to the data folder.
+        figure_folder: Path to the figure folder.
+        measurement_folder: Path to the measurement folder.
+
+    Examples:
+        Create an instance of the DataHandler class:
+
+        >>> dh = DataHandler(
+        >>>     data_folder=Path('C:\\'', 'Data'),
+        >>>     figure_folder=Path('C:\\'', 'QudiHiraAnalysis'),
+        >>>     measurement_folder=Path('20230101_Bakeout'),
+        >>> )
     """
 
     def __init__(
             self,
             data_folder: Path,
             figure_folder: Path,
             measurement_folder: Path = Path(),
@@ -166,15 +161,15 @@
             print(line)
 
     def figure_folder_tree(self):
         """ Print a tree of the figure folder. """
         for line in self.__tree(self.figure_folder_path):
             print(line)
 
-    def get_measurement_filepaths(
+    def _get_measurement_filepaths(
             self,
             measurement: str,
             extension: str,
             exclude_str: str | None = None
     ) -> list[Path]:
         """
         List all measurement files for a single measurement type, regardless of date
@@ -200,16 +195,16 @@
     ) -> dict[str: MeasurementDataclass]:
 
         if pulsed:
             filtered_filepaths = []
             timestamps = set()
 
             # Get set of unique timestamps containing pulsed_measurement_str
-            for filepath in self.get_measurement_filepaths(measurement=measurement_str, extension=extension,
-                                                           exclude_str="image_1.dat"):
+            for filepath in self._get_measurement_filepaths(measurement=measurement_str, extension=extension,
+                                                            exclude_str="image_1.dat"):
                 filename = filepath.name
                 if measurement_str in filename:
                     timestamps.add(filename[:16])
                     filtered_filepaths.append(filepath)
 
             pulsed_measurement_data: dict[str: MeasurementDataclass] = {}
 
@@ -249,21 +244,21 @@
                 exclude_str = None
             else:
                 loaders = self.default_qudi_loader
                 exclude_str = None
 
             measurement_data: dict[str: MeasurementDataclass] = {}
 
-            for filepath in self.get_measurement_filepaths(measurement_str, extension, exclude_str):
+            for filepath in self._get_measurement_filepaths(measurement_str, extension, exclude_str):
                 ts = filepath.name[:16]
                 measurement_data[ts] = (
                     MeasurementDataclass(
                         filepath=filepath,
                         timestamp=datetime.datetime.strptime(ts, self.timestamp_format_str),
-                        loaders=loaders
+                        _loaders=loaders
                     )
                 )
             return measurement_data
 
     def __load_standard_measurements_into_dataclass(
             self,
             measurement_str: str,
@@ -292,77 +287,64 @@
         elif extension == ".001":
             loaders = self.bruker_spm_loader
             exclude_str = None
         else:
             loaders = self.default_qudi_loader
             exclude_str = None
 
-        for filepath in self.get_measurement_filepaths(measurement_str, extension, exclude_str):
+        for filepath in self._get_measurement_filepaths(measurement_str, extension, exclude_str):
             timestamp = datetime.datetime.fromtimestamp(filepath.stat().st_mtime)
             self.log.warning("Extracting timestamp from file modified time, may not be accurate.")
             ts = datetime.datetime.strftime(timestamp, self.timestamp_format_str)
             measurement_list[ts] = (
                 MeasurementDataclass(
                     filepath=filepath,
                     timestamp=timestamp,
-                    loaders=loaders
+                    _loaders=loaders
                 )
             )
         return measurement_list
 
     def load_measurements(
             self,
             measurement_str: str,
             qudi: bool = True,
             pulsed: bool = False,
             extension: str = ".dat"
     ) -> dict[str: MeasurementDataclass]:
         """
         Lazy load all measurements of a given type into a dictionary of dataclasses.
 
-        Parameters
-        ----------
-            measurement_str: str
-                The name of the measurement type to load e.g. t1, t2,
-                confocal etc. Recursively searches through the path
-                defined by data_folder and measurement_folder
-            qudi: bool
-                Whether the measurement is a qudi measurement
-                (default: False).
-            pulsed: bool
-                Whether the measurement is a pulsed measurement
-                (default: False).
-            extension: str
-                The file extension of the measurement files.
-                (default: .dat)
+        Args:
+            measurement_str: The name of the measurement type to load e.g. t1, t2, confocal etc. Recursively searches through the path defined by data_folder and measurement_folder
+            qudi: Whether the measurement is a qudi measurement (default: False).
+            pulsed: Whether the measurement is a pulsed measurement (default: False).
+            extension: The file extension of the measurement files (default: .dat).
 
-        Returns
-        -------
-            measurement_list: dict[str: MeasurementDataclass]
-                A dictionary of dataclasses containing the measurement data.
+        Returns:
+            dict: A dictionary of dataclasses containing the measurement data.
 
-        Examples
-        --------
-        `dh` is an instance of the `DataHandler` class.
+        Examples:
+            `dh` is an instance of the `DataHandler` class.
 
-        Load all T1 measurements:
+            Load all T1 measurements:
 
-        >>> dh.load_measurements(measurement_str="ODMR", pulsed=True)
+            >>> dh.load_measurements(measurement_str="ODMR", pulsed=True)
 
-        Load all confocal data:
+            Load all confocal data:
 
-        >>> dh.load_measurements(measurement_str="Confocal")
+            >>> dh.load_measurements(measurement_str="Confocal")
 
-        Load all temperature monitoring data:
+            Load all temperature monitoring data:
 
-        >>> dh.load_measurements(measurement_str="Temperature")
+            >>> dh.load_measurements(measurement_str="Temperature")
 
-        Load all pressure monitoring data:
+            Load all pressure monitoring data:
 
-        >>> dh.load_measurements(measurement_str="Pressure")
+            >>> dh.load_measurements(measurement_str="Pressure")
         """
 
         measurement_str = measurement_str.lower()
         if qudi:
             return self.__load_qudi_measurements_into_dataclass(measurement_str, pulsed=pulsed, extension=".dat")
         else:
             return self.__load_standard_measurements_into_dataclass(measurement_str, extension=extension)
```

### Comparing `qudi_hira_analysis-1.5.0/qudi_hira_analysis/fitmethods/antibunchingmethods.py` & `qudi_hira_analysis-1.5.1/qudi_hira_analysis/_fitmethods/antibunchingmethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.5.0/qudi_hira_analysis/fitmethods/decaylikemethods.py` & `qudi_hira_analysis-1.5.1/qudi_hira_analysis/_fitmethods/decaylikemethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.5.0/qudi_hira_analysis/fitmethods/gaussianlikemethods.py` & `qudi_hira_analysis-1.5.1/qudi_hira_analysis/_fitmethods/gaussianlikemethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.5.0/qudi_hira_analysis/fitmethods/generalmethods.py` & `qudi_hira_analysis-1.5.1/qudi_hira_analysis/_fitmethods/generalmethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.5.0/qudi_hira_analysis/fitmethods/hyperbolicsaturationmethods.py` & `qudi_hira_analysis-1.5.1/qudi_hira_analysis/_fitmethods/hyperbolicsaturationmethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.5.0/qudi_hira_analysis/fitmethods/linearmethods.py` & `qudi_hira_analysis-1.5.1/qudi_hira_analysis/_fitmethods/linearmethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.5.0/qudi_hira_analysis/fitmethods/lorentzianlikemethods.py` & `qudi_hira_analysis-1.5.1/qudi_hira_analysis/_fitmethods/lorentzianlikemethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.5.0/qudi_hira_analysis/fitmethods/poissonianlikemethods.py` & `qudi_hira_analysis-1.5.1/qudi_hira_analysis/_fitmethods/poissonianlikemethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.5.0/qudi_hira_analysis/fitmethods/sinemethods.py` & `qudi_hira_analysis-1.5.1/qudi_hira_analysis/_fitmethods/sinemethods.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.5.0/qudi_hira_analysis/helper_functions.py` & `qudi_hira_analysis-1.5.1/qudi_hira_analysis/helper_functions.py`

 * *Files identical despite different names*

### Comparing `qudi_hira_analysis-1.5.0/qudi_hira_analysis/io_handler.py` & `qudi_hira_analysis-1.5.1/qudi_hira_analysis/io_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,59 +18,91 @@
 
     def __init__(self, base_read_path: Path = None, base_write_path: Path = None):
         super().__init__()
         self.base_read_path = base_read_path
         self.base_write_path = base_write_path
 
     @staticmethod
-    def add_base_read_path(func: Callable) -> Callable:
-        """ Decorator to add the base_read_path to the filepath if it is not None """
+    def _add_base_read_path(func: Callable) -> Callable:
+        """
+        Decorator to add the `base_read_path` to the filepath if it is not None
+
+        Args:
+            func: Function to be decorated
+
+        Returns:
+            Decorated function
+        """
 
         @wraps(func)
         def wrapper(self, filepath: Path, **kwargs):
             if self.base_read_path:
                 filepath = self.base_read_path / filepath
             return func(self, filepath, **kwargs)
 
         return wrapper
 
     @staticmethod
-    def add_base_write_path(func: Callable) -> Callable:
-        """ Decorator to add the base_write_path to the filepath if it is not None """
+    def _add_base_write_path(func: Callable) -> Callable:
+        """
+        Decorator to add the `base_write_path` to the filepath if it is not None
+
+        Args:
+            func: Function to be decorated
+
+        Returns:
+            Decorated function
+        """
 
         @wraps(func)
         def wrapper(self, filepath: Path, **kwargs):
             if self.base_write_path:
                 filepath = self.base_write_path / filepath
             filepath.parent.mkdir(exist_ok=True)
             return func(self, filepath, **kwargs)
 
         return wrapper
 
     @staticmethod
-    def check_extension(ext: str) -> Callable:
-        """ Decorator to check the extension of the filepath is correct """
+    def _check_extension(ext: str) -> Callable:
+        """
+        Decorator to check the extension of the filepath is correct
+
+        Args:
+            ext: Extension to check for
+
+        Returns:
+            Decorated function
+        """
 
         def decorator(func: Callable) -> Callable:
+            @wraps(func)
             def wrapper(self, filepath: Path, **kwargs) -> Callable:
                 if filepath.suffix == ext:
                     return func(self, filepath, **kwargs)
                 elif filepath.suffix == "":
                     return func(self, filepath.with_suffix(ext), **kwargs)
                 else:
                     raise IOError(f"Invalid extension '{filepath.suffix}' in '{filepath}', extension should be '{ext}'")
 
             return wrapper
 
         return decorator
 
-    @add_base_read_path
-    @check_extension(".dat")
+    @_add_base_read_path
+    @_check_extension(".dat")
     def read_qudi_parameters(self, filepath: Path) -> dict:
-        """ Extract parameters from a qudi dat file. """
+        """Extract parameters from a qudi dat file.
+
+        Args:
+            filepath: Path to the qudi .dat file
+
+        Returns:
+            Dictionary of parameters
+        """
         params = {}
         with open(filepath) as file:
             for line in file:
                 if line == '#=====\n':
                     break
                 else:
                     # noinspection PyBroadException
@@ -89,37 +121,45 @@
                             datetime_str = datetime.datetime.strptime(timestamp_str, "%d.%m.%Y %Hh%Mmin%Ss").replace(
                                 tzinfo=datetime.timezone.utc)
                             params[label] = datetime_str
                     except Exception as _:
                         pass
         return params
 
-    @add_base_read_path
-    @check_extension(".dat")
+    @_add_base_read_path
+    @_check_extension(".dat")
     def read_into_dataframe(self, filepath: Path) -> pd.DataFrame:
-        """ Read a qudi data file into a pd DataFrame for analysis. """
+        """Read a qudi data file into a pandas DataFrame for analysis.
+
+        Args:
+            filepath: Path to the qudi data file
+
+        Returns:
+            DataFrame containing the data from the qudi data file
+        """
         with open(filepath) as handle:
             # Generate column names for DataFrame by parsing the file
             *_comments, names = itertools.takewhile(lambda line: line.startswith('#'), handle)
             names = names[1:].strip().split("\t")
         return pd.read_csv(filepath, names=names, comment="#", sep="\t")
 
-    @add_base_read_path
+    @_add_base_read_path
     def read_csv(self, filepath: Path, **kwargs) -> pd.DataFrame:
-        """ Read a csv file into a pd DataFrame. """
+        """ Read a csv file into a pandas DataFrame. """
         return pd.read_csv(filepath, **kwargs)
 
-    @add_base_read_path
+    @_add_base_read_path
     def read_excel(self, filepath: Path, **kwargs) -> pd.DataFrame:
-        """ Read a csv file into a pd DataFrame. """
+        """ Read a csv file into a pandas DataFrame. """
         return pd.read_excel(filepath, **kwargs)
 
-    @add_base_read_path
-    @check_extension(".dat")
+    @_add_base_read_path
+    @_check_extension(".dat")
     def read_confocal_into_dataframe(self, filepath: Path) -> pd.DataFrame:
+        """ Read a qudi confocal data file into a pandas DataFrame for analysis. """
         confocal_params = self.read_qudi_parameters(filepath)
         data = self.read_into_ndarray(filepath, delimiter="\t")
         # Use the confocal parameters to generate the index and columns for the DataFrame
         index = np.linspace(
             confocal_params['X image min (m)'],
             confocal_params['X image max (m)'],
             data.shape[0]
@@ -130,59 +170,75 @@
             data.shape[1]
         )
         df = pd.DataFrame(data, index=index, columns=columns)
         # Sort the index to get origin (0, 0) in the lower left corner of the DataFrame
         df.sort_index(axis=0, ascending=False, inplace=True)
         return df
 
-    @add_base_read_path
+    @_add_base_read_path
     def read_into_ndarray(self, filepath: Path, **kwargs) -> np.ndarray:
+        """ Read a file into a numpy ndarray. """
         return np.genfromtxt(filepath, **kwargs)
 
-    @add_base_read_path
+    @_add_base_read_path
     def read_into_ndarray_transposed(self, filepath: Path, **kwargs) -> np.ndarray:
+        """ Read a file into a transposed numpy ndarray. """
         return np.genfromtxt(filepath, **kwargs).T
 
-    @add_base_read_path
-    @check_extension(".pys")
+    @_add_base_read_path
+    @_check_extension(".pys")
     def read_pys(self, filepath: Path) -> dict:
-        """ Loads raw pys data files. Wraps around numpy.load. """
+        """ Read raw .pys data files into a dictionary. """
         byte_dict = np.load(str(filepath), encoding="bytes", allow_pickle=True)
         # Convert byte string keys to normal strings
         return {key.decode('utf8'): byte_dict.get(key) for key in byte_dict.keys()}
 
-    @add_base_read_path
-    @check_extension(".pkl")
+    @_add_base_read_path
+    @_check_extension(".pkl")
     def read_pkl(self, filepath: Path) -> dict:
-        """ Loads processed pickle files for plotting/further analysis. """
+        """ Read pickle files into a dictionary. """
         with open(filepath, 'rb') as f:
             file = pickle.load(f)
         return file
 
-    @add_base_read_path
-    @check_extension(".dat")
+    @_add_base_read_path
+    @_check_extension(".dat")
     def read_nanonis_data(self, filepath: Path) -> pd.DataFrame:
-        """ Extract data from a Nanonis dat file. """
+        """Read data from a Nanonis .dat file.
+
+        Args:
+            filepath: Path to the Nanonis .dat file.
+
+        Returns:
+            DataFrame of data.
+        """
         skip_rows = 0
         with open(filepath) as dat_file:
             for num, line in enumerate(dat_file, 1):
                 if "[DATA]" in line:
                     # Find number of rows to skip when extracting data
                     skip_rows = num
                     break
                 if "#=====" in line:
                     skip_rows = num
                     break
         df = pd.read_table(filepath, sep="\t", skiprows=skip_rows)
         return df
 
-    @add_base_read_path
-    @check_extension(".dat")
+    @_add_base_read_path
+    @_check_extension(".dat")
     def read_nanonis_parameters(self, filepath: Path) -> dict:
-        """ Extract parameters from a Nanonis dat file. """
+        """Read parameters from a Nanonis .dat file.
+
+        Args:
+            filepath: Path to the Nanonis .dat file.
+
+        Returns:
+            Dictionary of parameters.
+        """
         parameters = {}
         with open(filepath) as dat_file:
             for line in dat_file:
                 if line == "\n":
                     # Break when reaching empty line
                     break
                 elif "User" in line or line.split("\t")[0] == "":
@@ -196,45 +252,73 @@
                     except ValueError:
                         pass
                     if "Oscillation Control>" in label:
                         label = label.replace("Oscillation Control>", "")
                     parameters[label] = value
         return parameters
 
-    @add_base_read_path
-    @check_extension(".sxm")
+    @_add_base_read_path
+    @_check_extension(".sxm")
     def read_nanonis_spm_data(self, filepath: Path) -> pySPM.SXM:
-        """ Read a Nanonis SPM data file. """
+        """Read a Nanonis .sxm data file.
+
+        Args:
+            filepath: Path to the .sxm file.
+
+        Returns:
+            pySPM.SXM object containing the data.
+        """
         return pySPM.SXM(filepath)
 
-    @add_base_read_path
-    @check_extension(".001")
+    @_add_base_read_path
+    @_check_extension(".001")
     def read_bruker_spm_data(self, filepath: Path) -> pySPM.Bruker:
-        """ Read a Bruker SPM data file. """
+        """Read a Bruker SPM data file.
+
+        Args:
+            filepath: Path to the .001 file.
+
+        Returns:
+            pySPM.Bruker object containing the data.
+        """
         return pySPM.Bruker(filepath)
 
-    @add_base_read_path
-    @check_extension(".txt")
+    @_add_base_read_path
+    @_check_extension(".txt")
     def read_pfeiffer_data(self, filepath: Path) -> pd.DataFrame:
-        """ Read data stored by Pfeiffer vacuum monitoring software. """
+        """Read data stored by Pfeiffer vacuum monitoring software.
+
+        Args:
+            filepath: Path to the text file.
+
+        Returns:
+            DataFrame containing the data.
+        """
         # Extract rows including the header
         df = pd.read_csv(filepath, sep="\t", skiprows=[0, 2, 3, 4])
         # Combine data and time columns together
         df["Date"] = df["Date"] + " " + df["Time"]
         df = df.drop("Time", axis=1)
         # Infer datetime format and convert to datetime objects
         df["Date"] = pd.to_datetime(df["Date"], infer_datetime_format=True)
         # Set datetime as index
         df = df.set_index("Date", drop=True)
         return df
 
-    @add_base_read_path
-    @check_extension(".xls")
+    @_add_base_read_path
+    @_check_extension(".xls")
     def read_lakeshore_data(self, filepath: Path) -> pd.DataFrame:
-        """ Read data stored by Lakeshore temperature monitor software. """
+        """Read data stored by Lakeshore temperature monitor software.
+
+        Args:
+            filepath: Path to the Excel file.
+
+        Returns:
+            DataFrame containing the data.
+        """
         # Extract only the origin timestamp
         origin = pd.read_excel(filepath, skiprows=1, nrows=1, usecols=[1], header=None)[1][0]
         # Remove any tzinfo to prevent future exceptions in pandas
         origin = origin.replace("CET", "")
         # Parse datetime object from timestamp
         origin = pd.to_datetime(origin)
         # Create DataFrame and drop empty cols
@@ -243,32 +327,47 @@
         # Add datetimes to DataFrame
         df["Datetime"] = pd.to_datetime(df["Time"], unit="ms", origin=origin)
         df = df.drop("Time", axis=1)
         # Set datetime as index
         df = df.set_index("Datetime", drop=True)
         return df
 
-    @add_base_read_path
-    @check_extension(".txt")
+    @_add_base_read_path
+    @_check_extension(".txt")
     def read_oceanoptics_data(self, filepath: str) -> pd.DataFrame:
-        """ Read spectrometer data from OceanOptics spectrometer. """
+        """Read spectrometer data from OceanOptics spectrometer.
+
+        Args:
+            filepath: Path to the data file.
+
+        Returns:
+            DataFrame containing the wavelength and intensity data.
+        """
         df = pd.read_csv(filepath, sep="\t", skiprows=14, names=["wavelength", "intensity"])
         return df
 
     @staticmethod
     def __get_forward_backward_counts(count_rates, num_pixels):
         split_array = np.split(count_rates, 2 * num_pixels)
         # Extract forward scan array as every second element
         forward_counts = np.stack(split_array[::2])
         # Extract backward scan array as every shifted second element
         # Flip scan so that backward and forward scans represent the same data
         backward_counts = np.flip(np.stack(split_array[1::2]), axis=1)
         return forward_counts, backward_counts
 
     def read_pixelscanner_data(self, filepath: Path) -> (pySPM.SPM_image, pySPM.SPM_image):
+        """ Read data from a PixelScanner measurement.
+
+        Args:
+            filepath: Path to the data file.
+
+        Returns:
+            Forward and backward scan data.
+        """
         df = self.read_into_dataframe(filepath)
         num_pixels = int(np.sqrt(len(df) // 2))
 
         if num_pixels ** 2 != len(df) // 2:
             raise ValueError("Number of pixels does not match data length.")
 
         try:
@@ -281,54 +380,56 @@
                 fwd = df["forward (cps)"].to_numpy().reshape(num_pixels, num_pixels)
                 bwd = df["backward (cps)"].to_numpy().reshape(num_pixels, num_pixels)
 
         fwd = pySPM.SPM_image(fwd, channel="Forward", _type="NV-PL")
         bwd = pySPM.SPM_image(bwd, channel="Backward", _type="NV-PL")
         return fwd, bwd
 
-    @add_base_write_path
-    @check_extension(".pkl")
+    @_add_base_write_path
+    @_check_extension(".pkl")
     def save_pkl(self, filepath: Path, obj: object):
-        """ Saves processed pickle files for plotting/further analysis. """
+        """Saves pickle files.
+
+        Args:
+            filepath: Path to the data file.
+            obj: Object to be saved.
+        """
         with open(filepath, 'wb') as f:
             pickle.dump(obj, f)
 
-    @add_base_write_path
-    @check_extension(".pys")
+    @_add_base_write_path
+    @_check_extension(".pys")
     def save_pys(self, filepath: Path, dictionary: dict):
-        """ Saves processed pickle files for plotting/further analysis. """
+        """Saves .pys files.
+
+        Args:
+            filepath: Path to the data file.
+            dictionary: Dictionary to be saved.
+        """
         with open(filepath, 'wb') as f:
             pickle.dump(dictionary, f, 1)
 
-    @add_base_write_path
-    @check_extension(".pys")
+    @_add_base_write_path
+    @_check_extension(".pys")
     def save_df(self, filepath: Path, df: pd.DataFrame):
         """ Save Dataframe as csv. """
         df.to_csv(filepath, sep='\t', encoding='utf-8')
 
-    @add_base_write_path
+    @_add_base_write_path
     def save_figures(self, filepath: Path, fig: plt.Figure, **kwargs):
-        """
-        Saves figures from matplotlib plot data. By default, saves as jpg, png, pdf and svg.
+        """Saves figures from matplotlib plot data.
+
+        By default, saves as jpg, png, pdf and svg.
 
-        Parameters
-        ----------
-        fig : matplotlib.figure.Figure
-            Figure to save.
-        filepath : pathlib.Path
-            Path to save figure to. If called with DataHandler, only the filename is required.
-
-        Keyword Arguments
-        -----------------
-        only_jpg : bool
-            If True, only save as jpg. Default is False.
-        only_pdf : bool
-            If True, only save as pdf. Default is False.
-        **kwargs
-            Keyword arguments passed to fig.savefig().
+        Args:
+            fig: Matplotlib figure to save.
+            filepath: Name of figure to save.
+            only_jpg: If True, only save as jpg (default: False).
+            only_pdf: If True, only save as pdf (default: False).
+            **kwargs: Keyword arguments passed to fig.savefig().
         """
         extensions = None
         if "only_jpg" in kwargs:
             if kwargs.get("only_jpg"):
                 extensions = [".jpg"]
             kwargs.pop("only_jpg", None)
         elif "only_pdf" in kwargs:
```

### Comparing `qudi_hira_analysis-1.5.0/qudi_hira_analysis/measurement_dataclass.py` & `qudi_hira_analysis-1.5.1/qudi_hira_analysis/measurement_dataclass.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     from PIL import Image
 
 logging.basicConfig(format='%(name)s :: %(levelname)s :: %(message)s', level=logging.INFO)
 
 
 @dataclass
 class PulsedMeasurement:
+    """ Dataclass for storing pulsed data and metadata """
     filepath: Path
     loaders: (Callable, Callable) = field(default=None)
     __data: pd.DataFrame = field(default=None)
     __params: dict = field(default=None)
 
     @property
     def data(self) -> pd.DataFrame:
@@ -37,14 +38,15 @@
         if self.__params is None:
             self.__params = self.loaders[1](self.filepath)
         return self.__params
 
 
 @dataclass
 class LaserPulses:
+    """ Dataclass for storing laser pulses data and metadata """
     filepath: Path
     loaders: (Callable, Callable) = field(default=None)
     __data: np.ndarray = field(default=None)
     __params: dict = field(default=None)
 
     @property
     def data(self) -> np.ndarray:
@@ -59,14 +61,15 @@
         if self.__params is None:
             self.__params = self.loaders[1](self.filepath)
         return self.__params
 
 
 @dataclass
 class RawTimetrace:
+    """ Dataclass for storing raw timetrace data and metadata """
     filepath: Path
     loaders: (Callable, Callable) = field(default=None)
     __data: np.ndarray = field(default=None)
     __params: dict = field(default=None)
 
     @property
     def data(self) -> np.ndarray:
@@ -81,31 +84,33 @@
         if self.__params is None:
             self.__params = self.loaders[1](self.filepath)
         return self.__params
 
 
 @dataclass
 class PulsedMeasurementDataclass:
+    """ Dataclass for storing pulsed measurement data and metadata """
     measurement: PulsedMeasurement
     laser_pulses: LaserPulses = field(default=None)
     timetrace: RawTimetrace = field(default=None)
 
     def __post_init__(self):
         self.base_filename = self.measurement.filepath.name.replace("_pulsed_measurement.dat", "")
 
     def show_image(self) -> Image:
         """ Use PIL to open the measurement image saved on the disk """
         return Image.open(str(self.measurement.filepath).replace(".dat", "_fig.png"))
 
 
 @dataclass
 class MeasurementDataclass:
+    """ Dataclass for storing measurement data and metadata """
     timestamp: datetime.datetime
     filepath: Path = field(default=None)
-    loaders: (Callable, Callable) = field(default=None)
+    _loaders: (Callable, Callable) = field(default=None)
     pulsed: PulsedMeasurementDataclass = field(default=None)
     __data: np.ndarray | pd.DataFrame = field(default=None)
     __params: dict = field(default=None)
     _fit_data: pd.DataFrame = field(default=None)
     _fit_model: lmfit.Model = field(default=None)
     _xy_position: Tuple[int, int] = field(default=None)
 
@@ -118,70 +123,71 @@
             self.filename = self.filepath.name
 
     def __repr__(self) -> str:
         return f"Measurement(timestamp='{self.timestamp}', filename='{self.filename}')"
 
     @property
     def data(self) -> np.ndarray | pd.DataFrame:
-        """ Read measurement data from file into suitable data structure """
+        """ Read measurement data from file. """
         if self.pulsed:
             return self.pulsed.measurement.data
         else:
             if self.__data is None:
-                self.__data = self.loaders[0](self.filepath)
+                self.__data = self._loaders[0](self.filepath)
             return self.__data
 
     @property
     def params(self) -> dict:
-        """ Read measurement params from file into dict """
+        """ Read measurement params from file. """
         if self.pulsed:
             return self.pulsed.measurement.params
         else:
             if self.__params is None:
-                self.__params = self.loaders[1](self.filepath)
+                self.__params = self._loaders[1](self.filepath)
             return self.__params
 
     @property
     def fit_data(self) -> pd.DataFrame:
         """ Fit data to a model """
         return self._fit_data
 
     @fit_data.setter
     def fit_data(self, fit_data: pd.DataFrame):
         """ Fit data to a model """
         self._fit_data = fit_data
 
     @property
-    def fit_model(self) -> Image:
+    def fit_model(self) -> lmfit.Model:
+        """ lmfit data model """
         return self._fit_model
 
     @fit_model.setter
     def fit_model(self, fit_model: lmfit.Model):
         self._fit_model = fit_model
 
     @property
     def xy_position(self) -> Tuple[int, int]:
+        """ (row, col) position of measurement in image """
         return self._xy_position
 
     @xy_position.setter
     def xy_position(self, xy_position: Tuple[int, int]):
         self._xy_position = xy_position
 
     def get_param_from_filename(self, unit: str) -> float | None:
         """
         Extract param from filename with format <param><unit>, where param
         is a float or integer and unit is a string. The param can be negative
         with keyword 'minus' or a decimal point with keyword 'point'.
 
         Args:
-            unit: str
-                unit of param to extract, e.g. dBm, mbar, V, etc.
+            unit: unit of param to extract, e.g. dBm, mbar, V etc.
 
-        Returns: float
-            extracted param from filename
+        Returns:
+            Extracted param from filename
 
         Examples:
             filename = "rabi_12dBm"
             >>> get_param_from_filename(unit='dBm')
             12.0
 
             filename = "pixelscan_minus100nm"
```

### Comparing `qudi_hira_analysis-1.5.0/qudi_hira_analysis/qudi_fit_logic.py` & `qudi_hira_analysis-1.5.1/qudi_hira_analysis/_qudi_fit_logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 This file contains the Qudi FitLogic class, which provides all
-fitting methods imported from the files in logic/fitmethods.
+fitting methods imported from the files in logic/_fitmethods.
 
 Qudi is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 Qudi is distributed in the hope that it will be useful,
@@ -51,15 +51,15 @@
 
     def __init__(self):
         super().__init__()
         # locking for thread safety
 
         filenames = []
         # for path in directories:
-        path_list = [os.path.join(os.path.dirname(os.path.realpath(__file__)), 'fitmethods')]
+        path_list = [os.path.join(os.path.dirname(os.path.realpath(__file__)), '_fitmethods')]
         # adding additional path, to be defined in the config
         self.log = logging.getLogger(__name__)
 
         if self._additional_methods_import_path:
             if isinstance(self._additional_methods_import_path, str):
                 self._additional_methods_import_path = [self._additional_methods_import_path]
                 self.log.info('Adding fit methods path: {}'.format(self._additional_methods_import_path))
@@ -85,15 +85,15 @@
 
         # A dictionary containing all fit methods and their estimators.
         self.fit_list = OrderedDict()
         self.fit_list['1d'] = OrderedDict()
         self.fit_list['2d'] = OrderedDict()
         self.fit_list['3d'] = OrderedDict()
 
-        # Go through the fitmethods files and import all methods.
+        # Go through the _fitmethods files and import all methods.
         # Also determine which methods need to be added to the fit_list dictionary
         estimators_for_dict = list()
         models_for_dict = list()
         fits_for_dict = list()
 
         for files in filenames:
             mod = importlib.import_module('{0}'.format(files))
```

### Comparing `qudi_hira_analysis-1.5.0/qudi_hira_analysis/raster_odmr_fitting.py` & `qudi_hira_analysis-1.5.1/qudi_hira_analysis/_raster_odmr_fitting.py`

 * *Files identical despite different names*

