# Comparing `tmp/investos-0.1.6.tar.gz` & `tmp/investos-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "investos-0.1.6.tar", max compression
+gzip compressed data, was "investos-0.1.7.tar", max compression
```

## Comparing `investos-0.1.6.tar` & `investos-0.1.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    20869 2023-04-03 18:29:49.638655 investos-0.1.6/LICENSE
--rw-r--r--   0        0        0     1904 2023-07-24 00:26:14.040338 investos-0.1.6/README.md
--rw-r--r--   0        0        0       49 2023-08-01 18:00:06.636074 investos-0.1.6/investos/__init__.py
--rw-r--r--   0        0        0      238 2023-07-21 18:30:51.315697 investos-0.1.6/investos/portfolio/__init__.py
--rw-r--r--   0        0        0      337 2023-07-21 18:30:51.315827 investos-0.1.6/investos/portfolio/constraint_model/__init__.py
--rw-r--r--   0        0        0      466 2023-07-21 18:30:51.315953 investos-0.1.6/investos/portfolio/constraint_model/base_constraint.py
--rw-r--r--   0        0        0     1331 2023-07-21 18:30:51.316077 investos-0.1.6/investos/portfolio/constraint_model/leverage_constraint.py
--rw-r--r--   0        0        0     2579 2023-07-21 18:30:51.316202 investos-0.1.6/investos/portfolio/constraint_model/long_constraint.py
--rw-r--r--   0        0        0     1411 2023-07-21 18:30:51.316360 investos-0.1.6/investos/portfolio/constraint_model/trade_constraint.py
--rw-r--r--   0        0        0     2361 2023-07-21 18:30:51.316520 investos-0.1.6/investos/portfolio/constraint_model/weight_constraint.py
--rw-r--r--   0        0        0    13295 2023-07-21 18:30:51.316723 investos-0.1.6/investos/portfolio/controller.py
--rw-r--r--   0        0        0      168 2023-07-21 18:30:51.316851 investos-0.1.6/investos/portfolio/cost_model/__init__.py
--rw-r--r--   0        0        0     1851 2023-07-21 18:30:51.316976 investos-0.1.6/investos/portfolio/cost_model/base_cost.py
--rw-r--r--   0        0        0     2121 2023-07-21 18:30:51.317101 investos-0.1.6/investos/portfolio/cost_model/holding_cost.py
--rw-r--r--   0        0        0     4076 2023-07-21 18:30:51.317232 investos-0.1.6/investos/portfolio/cost_model/trading_cost.py
--rw-r--r--   0        0        0      159 2023-07-25 18:27:16.735028 investos-0.1.6/investos/portfolio/result/__init__.py
--rw-r--r--   0        0        0    12627 2023-07-26 06:37:12.033358 investos-0.1.6/investos/portfolio/result/base_result.py
--rw-r--r--   0        0        0      260 2023-07-21 18:30:51.317663 investos-0.1.6/investos/portfolio/result/forecast_result.py
--rw-r--r--   0        0        0     4551 2023-08-01 17:55:15.170620 investos-0.1.6/investos/portfolio/result/save_result.py
--rw-r--r--   0        0        0     1300 2023-08-01 18:45:00.404371 investos-0.1.6/investos/portfolio/result/weights_result.py
--rw-r--r--   0        0        0      115 2023-07-19 05:16:44.134721 investos-0.1.6/investos/portfolio/risk_model/__init__.py
--rw-r--r--   0        0        0     1307 2023-07-21 18:30:51.317920 investos-0.1.6/investos/portfolio/risk_model/base_risk.py
--rw-r--r--   0        0        0     2599 2023-07-21 18:30:51.318049 investos-0.1.6/investos/portfolio/risk_model/stat_factor_risk.py
--rw-r--r--   0        0        0      160 2023-07-19 05:16:44.135700 investos-0.1.6/investos/portfolio/strategy/__init__.py
--rw-r--r--   0        0        0     1275 2023-07-21 18:30:51.318176 investos-0.1.6/investos/portfolio/strategy/base_strategy.py
--rw-r--r--   0        0        0     3991 2023-07-21 18:30:51.318305 investos-0.1.6/investos/portfolio/strategy/rank_long_short.py
--rw-r--r--   0        0        0     4040 2023-07-21 18:30:51.318476 investos-0.1.6/investos/portfolio/strategy/spo.py
--rw-r--r--   0        0        0     2215 2023-07-21 18:30:51.318602 investos-0.1.6/investos/util.py
--rw-r--r--   0        0        0     2287 2023-08-01 17:59:36.224378 investos-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3388 1970-01-01 00:00:00.000000 investos-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    20869 2023-04-03 18:29:49.638655 investos-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1904 2023-07-24 00:26:14.040338 investos-0.1.7/README.md
+-rw-r--r--   0        0        0       49 2023-08-04 22:46:09.490600 investos-0.1.7/investos/__init__.py
+-rw-r--r--   0        0        0      238 2023-07-21 18:30:51.315697 investos-0.1.7/investos/portfolio/__init__.py
+-rw-r--r--   0        0        0      337 2023-07-21 18:30:51.315827 investos-0.1.7/investos/portfolio/constraint_model/__init__.py
+-rw-r--r--   0        0        0      643 2023-08-04 22:43:26.796814 investos-0.1.7/investos/portfolio/constraint_model/base_constraint.py
+-rw-r--r--   0        0        0     1331 2023-07-21 18:30:51.316077 investos-0.1.7/investos/portfolio/constraint_model/leverage_constraint.py
+-rw-r--r--   0        0        0     2579 2023-07-21 18:30:51.316202 investos-0.1.7/investos/portfolio/constraint_model/long_constraint.py
+-rw-r--r--   0        0        0     1411 2023-07-21 18:30:51.316360 investos-0.1.7/investos/portfolio/constraint_model/trade_constraint.py
+-rw-r--r--   0        0        0     2361 2023-07-21 18:30:51.316520 investos-0.1.7/investos/portfolio/constraint_model/weight_constraint.py
+-rw-r--r--   0        0        0    13295 2023-07-21 18:30:51.316723 investos-0.1.7/investos/portfolio/controller.py
+-rw-r--r--   0        0        0      168 2023-07-21 18:30:51.316851 investos-0.1.7/investos/portfolio/cost_model/__init__.py
+-rw-r--r--   0        0        0     2115 2023-08-04 22:43:26.797112 investos-0.1.7/investos/portfolio/cost_model/base_cost.py
+-rw-r--r--   0        0        0     2121 2023-07-21 18:30:51.317101 investos-0.1.7/investos/portfolio/cost_model/holding_cost.py
+-rw-r--r--   0        0        0     4076 2023-07-21 18:30:51.317232 investos-0.1.7/investos/portfolio/cost_model/trading_cost.py
+-rw-r--r--   0        0        0      159 2023-07-25 18:27:16.735028 investos-0.1.7/investos/portfolio/result/__init__.py
+-rw-r--r--   0        0        0    12627 2023-07-26 06:37:12.033358 investos-0.1.7/investos/portfolio/result/base_result.py
+-rw-r--r--   0        0        0      260 2023-07-21 18:30:51.317663 investos-0.1.7/investos/portfolio/result/forecast_result.py
+-rw-r--r--   0        0        0     4675 2023-08-04 22:44:09.283379 investos-0.1.7/investos/portfolio/result/save_result.py
+-rw-r--r--   0        0        0     1300 2023-08-03 16:22:31.837257 investos-0.1.7/investos/portfolio/result/weights_result.py
+-rw-r--r--   0        0        0      115 2023-07-19 05:16:44.134721 investos-0.1.7/investos/portfolio/risk_model/__init__.py
+-rw-r--r--   0        0        0     1307 2023-07-21 18:30:51.317920 investos-0.1.7/investos/portfolio/risk_model/base_risk.py
+-rw-r--r--   0        0        0     2599 2023-07-21 18:30:51.318049 investos-0.1.7/investos/portfolio/risk_model/stat_factor_risk.py
+-rw-r--r--   0        0        0      160 2023-07-19 05:16:44.135700 investos-0.1.7/investos/portfolio/strategy/__init__.py
+-rw-r--r--   0        0        0     1839 2023-08-04 22:43:26.797362 investos-0.1.7/investos/portfolio/strategy/base_strategy.py
+-rw-r--r--   0        0        0     3991 2023-07-21 18:30:51.318305 investos-0.1.7/investos/portfolio/strategy/rank_long_short.py
+-rw-r--r--   0        0        0     4040 2023-07-21 18:30:51.318476 investos-0.1.7/investos/portfolio/strategy/spo.py
+-rw-r--r--   0        0        0     2215 2023-07-21 18:30:51.318602 investos-0.1.7/investos/util.py
+-rw-r--r--   0        0        0     2287 2023-08-04 22:45:31.281796 investos-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3388 1970-01-01 00:00:00.000000 investos-0.1.7/PKG-INFO
```

### Comparing `investos-0.1.6/LICENSE` & `investos-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `investos-0.1.6/README.md` & `investos-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `investos-0.1.6/investos/portfolio/constraint_model/leverage_constraint.py` & `investos-0.1.7/investos/portfolio/constraint_model/leverage_constraint.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.6/investos/portfolio/constraint_model/long_constraint.py` & `investos-0.1.7/investos/portfolio/constraint_model/long_constraint.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.6/investos/portfolio/constraint_model/trade_constraint.py` & `investos-0.1.7/investos/portfolio/constraint_model/trade_constraint.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.6/investos/portfolio/constraint_model/weight_constraint.py` & `investos-0.1.7/investos/portfolio/constraint_model/weight_constraint.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.6/investos/portfolio/controller.py` & `investos-0.1.7/investos/portfolio/controller.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.6/investos/portfolio/cost_model/base_cost.py` & `investos-0.1.7/investos/portfolio/cost_model/base_cost.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,7 +37,17 @@
         newobj = copy.copy(self)
         newobj.gamma *= other
         return newobj
 
     def __rmul__(self, other):
         """Read the gamma parameter as a multiplication; so you can change self.gamma without setting it directly as: gamma * BaseCost()"""
         return self.__mul__(other)
+
+    def metadata_dict(self):
+        metadata_dict = {}
+
+        metadata_dict["gamma"] = self.gamma
+
+        if getattr(self, "price_movement_sensitivity", None):
+            metadata_dict["price_movement_sensitivity"] = self.limit
+
+        return metadata_dict
```

### Comparing `investos-0.1.6/investos/portfolio/cost_model/holding_cost.py` & `investos-0.1.7/investos/portfolio/cost_model/holding_cost.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.6/investos/portfolio/cost_model/trading_cost.py` & `investos-0.1.7/investos/portfolio/cost_model/trading_cost.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.6/investos/portfolio/result/base_result.py` & `investos-0.1.7/investos/portfolio/result/base_result.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.6/investos/portfolio/result/save_result.py` & `investos-0.1.7/investos/portfolio/result/save_result.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,42 +5,44 @@
     def save(
         self,
         description,
         api_key,
         api_endpoint="https://app.forecastos.com/api/v1",
         tags=[],
         team_ids=[],
+        strategy=None,
     ):
         self.api_key = api_key
         self.api_endpoint = api_endpoint
         self.request_headers = {
             "Authorization": f"Bearer {self.api_key}",
             "Content-Type": "application/json",
         }
         self.tags = tags
         self.team_ids = team_ids
 
-        self.save_backtest(description)
+        self.save_backtest(description, strategy)
         self.save_backtest_charts()
 
-    def save_backtest(self, description):
+    def save_backtest(self, description, strategy):
         json_body = {
             "backtest": {
                 "description": description,
                 "performance_summary": {
                     "total_return": self.total_return,
                     "annualized_return": self.annualized_return,
                     "annualized_excess_return": self.annualized_excess_return,
                     "sharpe_ratio": self.sharpe_ratio,
                     "max_drawdown": self.max_drawdown,
                     "annual_turnover": self.annual_turnover,
                 },
                 "portfolio_id": None,
                 "tags": self.tags,
                 "team_ids": self.team_ids,
+                "portfolio_construction": strategy and strategy.metadata_dict(),
             }
         }
 
         response = requests.post(
             f"{self.api_endpoint}/backtests",
             headers=self.request_headers,
             json=json_body,
```

### Comparing `investos-0.1.6/investos/portfolio/result/weights_result.py` & `investos-0.1.7/investos/portfolio/result/weights_result.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.6/investos/portfolio/risk_model/base_risk.py` & `investos-0.1.7/investos/portfolio/risk_model/base_risk.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.6/investos/portfolio/risk_model/stat_factor_risk.py` & `investos-0.1.7/investos/portfolio/risk_model/stat_factor_risk.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.6/investos/portfolio/strategy/base_strategy.py` & `investos-0.1.7/investos/portfolio/strategy/base_strategy.py`

 * *Files 24% similar despite different names*

```diff
@@ -31,7 +31,22 @@
         ----------
         holdings : pandas.Series
             Holdings at beginning of period `t`.
         t : datetime.datetime
             The datetime for associated holdings `holdings`.
         """
         raise NotImplementedError
+
+    def metadata_dict(self):
+        return {
+            "strategy": self.__class__.__name__,
+            "risk_model": self.risk_model
+            and {self.risk_model.__class__.__name__: self.risk_model.metadata_dict()},
+            "constraint_models": {
+                el.__class__.__name__: el.metadata_dict() for el in self.constraints
+            },
+            "cost_models": {
+                el.__class__.__name__: el.metadata_dict()
+                for el in self.costs
+                if "Risk" not in el.__class__.__name__
+            },
+        }
```

### Comparing `investos-0.1.6/investos/portfolio/strategy/rank_long_short.py` & `investos-0.1.7/investos/portfolio/strategy/rank_long_short.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.6/investos/portfolio/strategy/spo.py` & `investos-0.1.7/investos/portfolio/strategy/spo.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.6/investos/util.py` & `investos-0.1.7/investos/util.py`

 * *Files identical despite different names*

### Comparing `investos-0.1.6/pyproject.toml` & `investos-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "investos"
-version = "0.1.6"
+version = "0.1.7"
 description = "For investors who want to focus on generating alpha"
 authors = ["Charlie Reese"]
 license = "Creative Commons Attribution-NonCommercial-ShareAlike (CC-BY-NC-SA)"
 readme = "README.md"
 packages = [{include = "investos"}]
 homepage = "https://investos.io/"
 repository = "https://github.com/charliereese/investos"
```

### Comparing `investos-0.1.6/PKG-INFO` & `investos-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: investos
-Version: 0.1.6
+Version: 0.1.7
 Summary: For investors who want to focus on generating alpha
 Home-page: https://investos.io/
 License: Creative Commons Attribution-NonCommercial-ShareAlike (CC-BY-NC-SA)
 Keywords: investing,alpha,backtesting,portfolio,optimization
 Author: Charlie Reese
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

