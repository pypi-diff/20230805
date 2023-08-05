# Comparing `tmp/riskmodels-2.1.0.tar.gz` & `tmp/riskmodels-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/riskmodels/riskmodels/dist/tmpa6ybbxji/riskmodels-2.1.0.tar", last modified: Thu Mar 31 21:16:21 2022, max compression
+gzip compressed data, was "/home/runner/work/riskmodels/riskmodels/dist/tmp2nvoexh_/riskmodels-2.2.0.tar", last modified: Tue Apr  5 10:59:15 2022, max compression
```

## Comparing `riskmodels-2.1.0.tar` & `riskmodels-2.2.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 21:16:21.000000 riskmodels-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-03-31 21:16:05.000000 riskmodels-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    14654 2022-03-31 21:16:21.000000 riskmodels-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14183 2022-03-31 21:16:05.000000 riskmodels-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 21:16:21.000000 riskmodels-2.1.0/riskmodels/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-03-31 21:16:11.000000 riskmodels-2.1.0/riskmodels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 21:16:21.000000 riskmodels-2.1.0/riskmodels/adequacy/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-03-31 21:16:05.000000 riskmodels-2.1.0/riskmodels/adequacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16955 2022-03-31 21:16:05.000000 riskmodels-2.1.0/riskmodels/adequacy/acg_models.py
--rw-r--r--   0 runner    (1001) docker     (121)    51153 2022-03-31 21:16:10.000000 riskmodels-2.1.0/riskmodels/adequacy/capacity_models.py
--rw-r--r--   0 runner    (1001) docker     (121)    69654 2022-03-31 21:16:05.000000 riskmodels-2.1.0/riskmodels/bivariate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 21:16:21.000000 riskmodels-2.1.0/riskmodels/c/
--rw-r--r--   0 runner    (1001) docker     (121)    27089 2022-03-31 21:16:05.000000 riskmodels-2.1.0/riskmodels/c/libbivarmargins.c
--rw-r--r--   0 runner    (1001) docker     (121)    11967 2022-03-31 21:16:05.000000 riskmodels-2.1.0/riskmodels/c/libbivarmargins.h
--rw-r--r--   0 runner    (1001) docker     (121)    11293 2022-03-31 21:16:05.000000 riskmodels-2.1.0/riskmodels/c/libtimedependence.c
--rw-r--r--   0 runner    (1001) docker     (121)     5328 2022-03-31 21:16:05.000000 riskmodels-2.1.0/riskmodels/c/libtimedependence.h
--rw-r--r--   0 runner    (1001) docker     (121)    18460 2022-03-31 21:16:05.000000 riskmodels-2.1.0/riskmodels/c/libunivarmargins.c
--rw-r--r--   0 runner    (1001) docker     (121)     7512 2022-03-31 21:16:05.000000 riskmodels-2.1.0/riskmodels/c/libunivarmargins.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 21:16:21.000000 riskmodels-2.1.0/riskmodels/c/mtwist-1.5/
--rw-r--r--   0 runner    (1001) docker     (121)    33254 2022-03-31 21:16:05.000000 riskmodels-2.1.0/riskmodels/c/mtwist-1.5/mtwist.c
--rw-r--r--   0 runner    (1001) docker     (121)    28519 2022-03-31 21:16:05.000000 riskmodels-2.1.0/riskmodels/c/mtwist-1.5/mtwist.h
--rw-r--r--   0 runner    (1001) docker     (121)    19046 2022-03-31 21:16:05.000000 riskmodels-2.1.0/riskmodels/c/mtwist-1.5/randistrs.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 21:16:21.000000 riskmodels-2.1.0/riskmodels/c_build/
--rw-r--r--   0 runner    (1001) docker     (121)     2576 2022-03-31 21:16:09.000000 riskmodels-2.1.0/riskmodels/c_build/build_bivarmargins.py
--rw-r--r--   0 runner    (1001) docker     (121)     1441 2022-03-31 21:16:09.000000 riskmodels-2.1.0/riskmodels/c_build/build_timedependence.py
--rw-r--r--   0 runner    (1001) docker     (121)     1931 2022-03-31 21:16:09.000000 riskmodels-2.1.0/riskmodels/c_build/build_univarmargins.py
--rw-r--r--   0 runner    (1001) docker     (121)    87698 2022-03-31 21:16:11.000000 riskmodels-2.1.0/riskmodels/univariate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 21:16:21.000000 riskmodels-2.1.0/riskmodels/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-03-31 21:16:05.000000 riskmodels-2.1.0/riskmodels/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5934 2022-03-31 21:16:05.000000 riskmodels-2.1.0/riskmodels/utils/adequacy_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (121)    15027 2022-03-31 21:16:05.000000 riskmodels-2.1.0/riskmodels/utils/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (121)    16815 2022-03-31 21:16:05.000000 riskmodels-2.1.0/riskmodels/utils/tmvn.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-31 21:16:21.000000 riskmodels-2.1.0/riskmodels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14654 2022-03-31 21:16:20.000000 riskmodels-2.1.0/riskmodels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      921 2022-03-31 21:16:21.000000 riskmodels-2.1.0/riskmodels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-31 21:16:20.000000 riskmodels-2.1.0/riskmodels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-03-31 21:16:20.000000 riskmodels-2.1.0/riskmodels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-03-31 21:16:21.000000 riskmodels-2.1.0/riskmodels.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-31 21:16:21.000000 riskmodels-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1678 2022-03-31 21:16:05.000000 riskmodels-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 10:59:15.000000 riskmodels-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-04-05 10:58:51.000000 riskmodels-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    14654 2022-04-05 10:59:15.000000 riskmodels-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    14183 2022-04-05 10:58:51.000000 riskmodels-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 10:59:15.000000 riskmodels-2.2.0/riskmodels/
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-04-05 10:59:02.000000 riskmodels-2.2.0/riskmodels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 10:59:15.000000 riskmodels-2.2.0/riskmodels/adequacy/
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2022-04-05 10:58:51.000000 riskmodels-2.2.0/riskmodels/adequacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16955 2022-04-05 10:58:51.000000 riskmodels-2.2.0/riskmodels/adequacy/acg_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)    52181 2022-04-05 10:59:00.000000 riskmodels-2.2.0/riskmodels/adequacy/capacity_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)    69708 2022-04-05 10:58:51.000000 riskmodels-2.2.0/riskmodels/bivariate.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 10:59:15.000000 riskmodels-2.2.0/riskmodels/c/
+-rw-r--r--   0 runner    (1001) docker     (121)    27089 2022-04-05 10:58:51.000000 riskmodels-2.2.0/riskmodels/c/libbivarmargins.c
+-rw-r--r--   0 runner    (1001) docker     (121)    11967 2022-04-05 10:58:51.000000 riskmodels-2.2.0/riskmodels/c/libbivarmargins.h
+-rw-r--r--   0 runner    (1001) docker     (121)    11293 2022-04-05 10:58:51.000000 riskmodels-2.2.0/riskmodels/c/libtimedependence.c
+-rw-r--r--   0 runner    (1001) docker     (121)     5328 2022-04-05 10:58:51.000000 riskmodels-2.2.0/riskmodels/c/libtimedependence.h
+-rw-r--r--   0 runner    (1001) docker     (121)    18460 2022-04-05 10:58:51.000000 riskmodels-2.2.0/riskmodels/c/libunivarmargins.c
+-rw-r--r--   0 runner    (1001) docker     (121)     7512 2022-04-05 10:58:51.000000 riskmodels-2.2.0/riskmodels/c/libunivarmargins.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 10:59:15.000000 riskmodels-2.2.0/riskmodels/c/mtwist-1.5/
+-rw-r--r--   0 runner    (1001) docker     (121)    33254 2022-04-05 10:58:51.000000 riskmodels-2.2.0/riskmodels/c/mtwist-1.5/mtwist.c
+-rw-r--r--   0 runner    (1001) docker     (121)    28519 2022-04-05 10:58:51.000000 riskmodels-2.2.0/riskmodels/c/mtwist-1.5/mtwist.h
+-rw-r--r--   0 runner    (1001) docker     (121)    19046 2022-04-05 10:58:51.000000 riskmodels-2.2.0/riskmodels/c/mtwist-1.5/randistrs.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 10:59:15.000000 riskmodels-2.2.0/riskmodels/c_build/
+-rw-r--r--   0 runner    (1001) docker     (121)     2576 2022-04-05 10:59:00.000000 riskmodels-2.2.0/riskmodels/c_build/build_bivarmargins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1441 2022-04-05 10:59:00.000000 riskmodels-2.2.0/riskmodels/c_build/build_timedependence.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1931 2022-04-05 10:59:00.000000 riskmodels-2.2.0/riskmodels/c_build/build_univarmargins.py
+-rw-r--r--   0 runner    (1001) docker     (121)    87888 2022-04-05 10:59:01.000000 riskmodels-2.2.0/riskmodels/univariate.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 10:59:15.000000 riskmodels-2.2.0/riskmodels/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2022-04-05 10:58:51.000000 riskmodels-2.2.0/riskmodels/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5934 2022-04-05 10:58:51.000000 riskmodels-2.2.0/riskmodels/utils/adequacy_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15027 2022-04-05 10:58:51.000000 riskmodels-2.2.0/riskmodels/utils/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16815 2022-04-05 10:58:51.000000 riskmodels-2.2.0/riskmodels/utils/tmvn.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 10:59:15.000000 riskmodels-2.2.0/riskmodels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    14654 2022-04-05 10:59:14.000000 riskmodels-2.2.0/riskmodels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      921 2022-04-05 10:59:15.000000 riskmodels-2.2.0/riskmodels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-05 10:59:14.000000 riskmodels-2.2.0/riskmodels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-04-05 10:59:14.000000 riskmodels-2.2.0/riskmodels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-04-05 10:59:15.000000 riskmodels-2.2.0/riskmodels.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-05 10:59:15.000000 riskmodels-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1678 2022-04-05 10:58:51.000000 riskmodels-2.2.0/setup.py
```

### Comparing `riskmodels-2.1.0/PKG-INFO` & `riskmodels-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riskmodels
-Version: 2.1.0
+Version: 2.2.0
 Summary: Extreme value models for applications in energy procurement
 Home-page: https://bitbucket.com/nestorsag/phd
 Author: Nestor Sanchez
 Author-email: nestor.sag@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `riskmodels-2.1.0/README.md` & `riskmodels-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `riskmodels-2.1.0/riskmodels/adequacy/acg_models.py` & `riskmodels-2.2.0/riskmodels/adequacy/acg_models.py`

 * *Files identical despite different names*

### Comparing `riskmodels-2.1.0/riskmodels/adequacy/capacity_models.py` & `riskmodels-2.2.0/riskmodels/adequacy/capacity_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,16 +82,16 @@
         demand_data: np.ndarray,
         renewables_data: np.ndarray,
         gen_distributions: t.List[acg_models.NonSequential],
         season_length: int = None,
     ):
         """
         Args:
-            demand_data (np.ndarray): Demand data matrix with two columns
-            renewables_data (np.ndarray): Renewable generation data matrix with two columns
+            demand_data (np.ndarray): Demand data array with two columns
+            renewables_data (np.ndarray): Renewable generation data array with two columns
             gen_distributions (t.List[acg_models.NonSequential]): List of non-sequential ACG objects
             season_length (int, optional): length of peak season. If None, it is set as the length of demand data
 
         """
         gen_distribution = Independent(x=gen_distributions[0], y=gen_distributions[1])
         warnings.warn("Coercing data to integer values.", stacklevel=2)
 
@@ -257,21 +257,25 @@
         self.convgen1 = copy.deepcopy(self.convgen2)
         self.convgen2 = aux
 
         self.gen_distribution = Independent(
             x=self.gen_distribution.y, y=self.gen_distribution.x
         )
 
-    def eeu(self, itc_cap: int = 1000, policy: str = "veto", area: int = 0):
-        """Computes the post-interconnection expected energy unserved.
+    def eeu(self, itc_cap: int = 1000, policy: str = "veto", area: int = 0) -> float:
+        """Computes the post-interconnection expected energy unserved (EEU).
 
         Args:
             itc_cap (int, optional): interconnection capacity
             policy (str, optional): one of 'veto' or 'share'; in a 'veto' policy, areas only export spare available capacity, while in a 'share' policy, capacity shortfalls are shared according to demand proportions across areas. Shortfalls can extend from one area to another by diverting power.
             area (int, optional): Area for which to evaluate eeu; if area=-1, systemwide eeu is returned
+
+        Returns:
+            float: Estimated EEU
+
         """
 
         if area == -1:
             return self.eeu(itc_cap, policy, 0) + self.eeu(itc_cap, policy, 1)
 
         if area == 1:
             self.swap_axes()
@@ -564,29 +568,34 @@
 
 class UnivariateSequential(BaseCapacityModel, BasePydanticModel):
 
     """Univariate model for capacity surplus using a sequential available conventional generation model, implementing Monte Carlo evaluations through map-reduce patterns. Worker instances are of type UnivariateTraces.
 
     Args:
         gen_dir (str): folder with conventional generation data
-        demand (np.ndarray): demand data
-        renewables (np.ndarray): renewables data
+        demand (np.ndarray): one-dimensionsl demand data
+        renewables (np.ndarray): one-dimensional renewables data
         season_length (int): number of timesteps per peak season
         n_cores (int, optional): number of cores to use for map-reduce operations
 
     """
 
     gen_dir: str
     demand: np.ndarray
     renewables: np.ndarray
     season_length: int
     n_cores: t.Optional[int] = 2
 
     _worker_class = UnivariateTraces
 
+    @validator("demand", "renewables", allow_reuse=True)
+    def check_shape_and_order(cls, data):
+        # ensures passed arrays are one-dimensional and follow row-major order
+        return np.ascontiguousarray(data, np.float32).reshape(-1)
+
     class Config:
         arbitrary_types_allowed = True
 
     @classmethod
     def _persist_gen_traces(
         cls, args: t.Tuple[acg_models.Sequential, t.Dict, Path, int]
     ) -> None:
@@ -613,15 +622,15 @@
         renewables: np.ndarray,
         season_length: int,
         n_cores: int = 4,
         burn_in: int = 100,
         seed: int = None,
         compress_files: bool = False,
     ) -> UnivariateSequential:
-        """Generate and persists traces of conventional generation in files, and uses them to instantiate a surplus model. Returns a surplus model ready to perform computations with the generated files.
+        """Generate and persists traces of conventional generation in multiple files, and uses them to instantiate a capacity surplus model. Returns a surplus model ready to perform computations on the generated files.
 
         Args:
             output_dir (str): Output directory for trace files
             n_traces (int): Total number of season traces to simulate
             n_files (int): Number of files to create. Making this a multiple of the available number of cores and ensuring that each file is on the order of 500 MB (~ 125 million floats) is probably optimal.
             gen (acg_models.Sequential): Sequential conventional generation instance.
             demand (np.ndarray): Demand data
@@ -798,19 +807,19 @@
         Returns:
             float: lole estimate
         """
         return self.season_length * self.cdf(
             x=-1e-1
         )  # tiny offset to avoid issues with numerical rounding errors from adding millions of numbers together
 
-    def eeu(self):
-        """Computes the expected energy unserved
+    def eeu(self) -> float:
+        """Computes the expected energy unserved (EEU)
 
         Returns:
-            float: eeu estimate
+            float: estimated EEU
         """
 
         def reducer(mapped):
             n_traces = np.sum([n for _, n in mapped])
             return np.array([n * val for val, n in mapped]).sum() / n_traces
 
         return self.map_reduce(mapper="eeu", reducer=reducer)
@@ -879,23 +888,32 @@
 
 class BivariateSequential(UnivariateSequential):
 
     """Bivariate model for capacity surplus using a sequential available conventional generation model, implementing Monte Carlo evaluations through map-reduce patterns. Worker instances are of type BivariateTraces.
 
     Args:
         gen_dir (str): folder with conventional generation data
-        demand (np.ndarray): demand data
-        renewables (np.ndarray): renewables data
+        demand (np.ndarray): two-dimensional demand array with two columns
+        renewables (np.ndarray): two-dimensional renewables data array with two columns
         season_length (int): number of timesteps per peak season
         n_cores (int, optional): number of cores to use for map-reduce operations
     """
 
     _worker_class = BivariateTraces
     _area_indices = [0, 1]
 
+    @validator("demand", "renewables", allow_reuse=True)
+    def check_shape_and_order(cls, data):
+        # ensures passed arrays are twi-dimensional and follow row-major order
+        if len(data.shape) != 2 or data.shape[1] != 2:
+            raise ValueError(
+                "passed data arrays must be two-dimensional with two columns"
+            )
+        return np.ascontiguousarray(data, np.float32)
+
     @property
     def filedirs(self):
         return [Path(self.gen_dir) / str(area) for area in self._area_indices]
 
     @classmethod
     def init(
         cls,
@@ -906,15 +924,15 @@
         demand: np.ndarray,
         renewables: np.ndarray,
         season_length: int,
         n_cores: int = 4,
         burn_in: int = 100,
         compress_files: bool = False,
     ) -> BivariateSequential:
-        """Generate and persists traces of conventional generation in files, and use them to instantiate a surplus model.
+        """Generate and persists traces of conventional generation in multiple files, and uses them to instantiate a capacity surplus model. Returns a model ready to perform computations on the generated files.
 
         Args:
             output_dir (str): output directory for trace files
             n_traces (int): Total number of traces to simulate; a trace is a sequence of at least one peak season
             n_files (int): Number of files to create. Making this a multiple of the available number of cores and ensuring that each file is on the order of 500 MB (~ 125 million floats) is probably good enough.
             gens (acg_models.Sequential): List of sequential conventional generation instances, one per system.
             demand (np.ndarray): Demand data
@@ -929,15 +947,14 @@
 
 
         """
         for area, gen, univar_demand, univar_renewables in zip(
             cls._area_indices, gens, demand.T, renewables.T
         ):
             out_dir = Path(output_dir) / str(area)
-            print(f"Creating files for area {area}..")
             UnivariateSequential.init(
                 output_dir=str(out_dir),
                 n_traces=n_traces,
                 n_files=n_files,
                 gen=gen,
                 demand=univar_demand,
                 renewables=univar_renewables,
@@ -1059,21 +1076,25 @@
             mapper="cdf",
             reducer=reducer,
             itc_cap=itc_cap,
             policy=policy,
             str_map_kwargs={"x": x},
         )
 
-    def lole(self, itc_cap: float = 1000.0, policy="veto", area: int = 0):
-        """Computes the post-interconnection loss of load expectation.
+    def lole(self, itc_cap: float = 1000.0, policy="veto", area: int = 0) -> float:
+        """Computes the post-interconnection loss of load expectation (LOLE)
 
         Args:
-            itc_cap (int, optional): interconnection capacity
+            itc_cap (float, optional): interconnection capacity
             policy (str, optional): one of 'veto' or 'share'; in a 'veto' policy, areas only export spare available capacity, while in a 'share' policy, exports are market-driven, i.e., by power scarcity at both areas. Shortfalls can extend from one area to another by diverting power.
             area (int, optional): Area for which to evaluate LOLE; if area=-1, system-wide lole is returned
+
+        Returns:
+            float: estimated LOLE
+
         """
         offset = (
             -1e-1
         )  # this avoids numerical issues from adding up millions of numbers in the calculations
         if area in [0, 1]:
             x = np.zeros((2,), dtype=np.float32) + offset  # tiny offset
             x[1 - area] = np.Inf
@@ -1085,21 +1106,24 @@
                 + self.cdf(np.flip(x), itc_cap=itc_cap, policy=policy)
                 - self.cdf(np.minimum(offset, x), itc_cap=itc_cap, policy=policy)
             )
             return self.season_length * prob
         else:
             raise ValueError("area must be in [-1,0,1]")
 
-    def eeu(self, itc_cap: float = 1000.0, policy="veto", area: int = 0):
-        """Computes the post-interconnection expected energy unserved.
+    def eeu(self, itc_cap: float = 1000.0, policy="veto", area: int = 0) -> float:
+        """Computes the post-interconnection expected energy unserved (EEU)
 
         Args:
-            itc_cap (int, optional): interconnection capacity
+            itc_cap (float, optional): interconnection capacity
             policy (str, optional): one of 'veto' or 'share'; in a 'veto' policy, areas only export spare available capacity, while in a 'share' policy, exports are market-driven, i.e., by power scarcity at both areas. Shortfalls can extend from one area to another by diverting power.
             area (int, optional): Area for which to evaluate eeu; if area=-1, systemwide eeu is returned
+
+        Returns:
+            float: estimated EEU
         """
 
         def reducer(mapped):
             n_traces = np.sum([n for _, n in mapped])
             return np.array([n * val for val, n in mapped]).sum() / n_traces
 
         return self.map_reduce(
```

### Comparing `riskmodels-2.1.0/riskmodels/bivariate.py` & `riskmodels-2.2.0/riskmodels/bivariate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1498,14 +1498,15 @@
         """Instantiate an empirical distribution from an n x 2 data matrix
 
         Args:
             data (np.ndarray): observed data
 
 
         """
+        data = np.ascontiguousarray(data, data.dtype)
         if (
             not isinstance(data, np.ndarray)
             or len(data.shape) != 2
             or data.shape[1] != 2
         ):
             raise ValueError("data must be an n x 2 numpy array")
```

### Comparing `riskmodels-2.1.0/riskmodels/c/libbivarmargins.c` & `riskmodels-2.2.0/riskmodels/c/libbivarmargins.c`

 * *Files identical despite different names*

### Comparing `riskmodels-2.1.0/riskmodels/c/libbivarmargins.h` & `riskmodels-2.2.0/riskmodels/c/libbivarmargins.h`

 * *Files identical despite different names*

### Comparing `riskmodels-2.1.0/riskmodels/c/libtimedependence.c` & `riskmodels-2.2.0/riskmodels/c/libtimedependence.c`

 * *Files identical despite different names*

### Comparing `riskmodels-2.1.0/riskmodels/c/libtimedependence.h` & `riskmodels-2.2.0/riskmodels/c/libtimedependence.h`

 * *Files identical despite different names*

### Comparing `riskmodels-2.1.0/riskmodels/c/libunivarmargins.c` & `riskmodels-2.2.0/riskmodels/c/libunivarmargins.c`

 * *Files identical despite different names*

### Comparing `riskmodels-2.1.0/riskmodels/c/libunivarmargins.h` & `riskmodels-2.2.0/riskmodels/c/libunivarmargins.h`

 * *Files identical despite different names*

### Comparing `riskmodels-2.1.0/riskmodels/c/mtwist-1.5/mtwist.c` & `riskmodels-2.2.0/riskmodels/c/mtwist-1.5/mtwist.c`

 * *Files identical despite different names*

### Comparing `riskmodels-2.1.0/riskmodels/c/mtwist-1.5/mtwist.h` & `riskmodels-2.2.0/riskmodels/c/mtwist-1.5/mtwist.h`

 * *Files identical despite different names*

### Comparing `riskmodels-2.1.0/riskmodels/c/mtwist-1.5/randistrs.h` & `riskmodels-2.2.0/riskmodels/c/mtwist-1.5/randistrs.h`

 * *Files identical despite different names*

### Comparing `riskmodels-2.1.0/riskmodels/c_build/build_bivarmargins.py` & `riskmodels-2.2.0/riskmodels/c_build/build_bivarmargins.py`

 * *Files identical despite different names*

### Comparing `riskmodels-2.1.0/riskmodels/c_build/build_timedependence.py` & `riskmodels-2.2.0/riskmodels/c_build/build_timedependence.py`

 * *Files identical despite different names*

### Comparing `riskmodels-2.1.0/riskmodels/c_build/build_univarmargins.py` & `riskmodels-2.2.0/riskmodels/c_build/build_univarmargins.py`

 * *Files identical despite different names*

### Comparing `riskmodels-2.1.0/riskmodels/univariate.py` & `riskmodels-2.2.0/riskmodels/univariate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1584,15 +1584,15 @@
     ) -> t.Union[float, np.ndarray]:
         """Inverse CDF function; it uses linear interpolation.
 
         Args:
             q (t.Union[float, np.ndarray]): probability level
 
         Returns:
-            t.Union[float, np.ndarray]: Linearly interpolated quantile function
+            t.Union[float, np.ndarray]: Evaluations of the (Linearly interpolated) quantile function
 
         """
         is_scalar = isinstance(q, self._allowed_scalar_types)
 
         if is_scalar:
             q = np.array([q])
 
@@ -1633,15 +1633,17 @@
             return 0.0
 
     def std(self, **kwargs):
         return np.sqrt(self.map(lambda x: x - self.mean()).moment(2))
 
     @classmethod
     def from_data(cls, data: np.array):
-
+        if len(data.shape) != 1:
+            warnings.warn("Reshaping input data to one-dimensional array")
+        data = np.ascontiguousarray(data, data.dtype).reshape(-1)
         support, unnorm_pdf = np.unique(data, return_counts=True)
         n = np.sum(unnorm_pdf)
         return cls(support=support, pdf_values=unnorm_pdf / n, data=data)
 
     def plot_mean_residual_life(self, threshold: float) -> matplotlib.figure.Figure:
         """Produces a mean residual life plot for the tail of the distribution above a given threshold
 
@@ -1709,15 +1711,15 @@
                 data, threshold, bin_empirical=isinstance(self, Binned), **kwargs
             )
 
     def map(self, f: t.Callable) -> Empirical:
         """Returns the distribution resulting from an arbitrary transformation
 
         Args:
-            f (t.Callable): Target transformation; it should take a numpy array as input
+            f (t.Callable): function to apply; it should take a numpy array as input
 
         """
         dist_df = pd.DataFrame({"pdf": self.pdf_values, "support": f(self.support)})
         mapped_dist_df = (
             dist_df.groupby("support").sum().reset_index().sort_values("support")
         )
```

### Comparing `riskmodels-2.1.0/riskmodels/utils/adequacy_interfaces.py` & `riskmodels-2.2.0/riskmodels/utils/adequacy_interfaces.py`

 * *Files identical despite different names*

### Comparing `riskmodels-2.1.0/riskmodels/utils/map_reduce.py` & `riskmodels-2.2.0/riskmodels/utils/map_reduce.py`

 * *Files identical despite different names*

### Comparing `riskmodels-2.1.0/riskmodels/utils/tmvn.py` & `riskmodels-2.2.0/riskmodels/utils/tmvn.py`

 * *Files identical despite different names*

### Comparing `riskmodels-2.1.0/riskmodels.egg-info/PKG-INFO` & `riskmodels-2.2.0/riskmodels.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: riskmodels
-Version: 2.1.0
+Version: 2.2.0
 Summary: Extreme value models for applications in energy procurement
 Home-page: https://bitbucket.com/nestorsag/phd
 Author: Nestor Sanchez
 Author-email: nestor.sag@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `riskmodels-2.1.0/riskmodels.egg-info/SOURCES.txt` & `riskmodels-2.2.0/riskmodels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `riskmodels-2.1.0/setup.py` & `riskmodels-2.2.0/setup.py`

 * *Files identical despite different names*

