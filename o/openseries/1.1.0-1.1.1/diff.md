# Comparing `tmp/openseries-1.1.0-py3-none-any.whl.zip` & `tmp/openseries-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 54059 bytes, number of entries: 15
+Zip file size: 54599 bytes, number of entries: 15
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 openseries/__init__.py
--rw-r--r--  2.0 unx     9970 b- defN 80-Jan-01 00:00 openseries/datefixer.py
--rw-r--r--  2.0 unx   115113 b- defN 80-Jan-01 00:00 openseries/frame.py
+-rw-r--r--  2.0 unx    10224 b- defN 80-Jan-01 00:00 openseries/datefixer.py
+-rw-r--r--  2.0 unx   115343 b- defN 80-Jan-01 00:00 openseries/frame.py
 -rw-r--r--  2.0 unx     1119 b- defN 80-Jan-01 00:00 openseries/load_plotly.py
 -rw-r--r--  2.0 unx      178 b- defN 80-Jan-01 00:00 openseries/plotly_captor_logo.json
 -rw-r--r--  2.0 unx     1429 b- defN 80-Jan-01 00:00 openseries/plotly_layouts.json
--rw-r--r--  2.0 unx     4404 b- defN 80-Jan-01 00:00 openseries/risk.py
--rw-r--r--  2.0 unx    84308 b- defN 80-Jan-01 00:00 openseries/series.py
--rw-r--r--  2.0 unx    13822 b- defN 80-Jan-01 00:00 openseries/sim_price.py
--rw-r--r--  2.0 unx    14673 b- defN 80-Jan-01 00:00 openseries/stoch_processes.py
--rw-r--r--  2.0 unx     7082 b- defN 80-Jan-01 00:00 openseries/types.py
--rw-r--r--  2.0 unx     1521 b- defN 80-Jan-01 00:00 openseries-1.1.0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx    47925 b- defN 80-Jan-01 00:00 openseries-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 openseries-1.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1200 b- defN 16-Jan-01 00:00 openseries-1.1.0.dist-info/RECORD
-15 files, 302832 bytes uncompressed, 52099 bytes compressed:  82.8%
+-rw-r--r--  2.0 unx     4234 b- defN 80-Jan-01 00:00 openseries/risk.py
+-rw-r--r--  2.0 unx    84592 b- defN 80-Jan-01 00:00 openseries/series.py
+-rw-r--r--  2.0 unx    15521 b- defN 80-Jan-01 00:00 openseries/sim_price.py
+-rw-r--r--  2.0 unx    14719 b- defN 80-Jan-01 00:00 openseries/stoch_processes.py
+-rw-r--r--  2.0 unx     7235 b- defN 80-Jan-01 00:00 openseries/types.py
+-rw-r--r--  2.0 unx     1521 b- defN 80-Jan-01 00:00 openseries-1.1.1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx    47876 b- defN 80-Jan-01 00:00 openseries-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 openseries-1.1.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1201 b- defN 16-Jan-01 00:00 openseries-1.1.1.dist-info/RECORD
+15 files, 305280 bytes uncompressed, 52639 bytes compressed:  82.8%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: openseries/stoch_processes.py
 Comment: 
 
 Filename: openseries/types.py
 Comment: 
 
-Filename: openseries-1.1.0.dist-info/LICENSE.md
+Filename: openseries-1.1.1.dist-info/LICENSE.md
 Comment: 
 
-Filename: openseries-1.1.0.dist-info/METADATA
+Filename: openseries-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: openseries-1.1.0.dist-info/WHEEL
+Filename: openseries-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: openseries-1.1.0.dist-info/RECORD
+Filename: openseries-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openseries/datefixer.py

```diff
@@ -1,29 +1,32 @@
 """
 Date related utilities
 """
 import datetime as dt
-from typing import Dict, List, Union
+from typing import cast, Dict, List, Optional, Union
 from dateutil.relativedelta import relativedelta
 from holidays import country_holidays, list_supported_countries
 from numpy import array, busdaycalendar, datetime64, is_busday, where, timedelta64
 from pandas import date_range, Timestamp
 from pandas.tseries.offsets import CustomBusinessDay
 
+from openseries.types import CountryStringType, CountriesType
+
 
 def holiday_calendar(
     startyear: int,
     endyear: int,
-    countries: List[str] | str = "SE",
-    custom_holidays: Union[
-        Dict[Union[dt.date, dt.datetime, str, float, int], str],
-        List[Union[dt.date, dt.datetime, str, float, int]],
-        Union[dt.date, dt.datetime, str, float, int],
-    ]
-    | None = None,
+    countries: CountriesType = "SE",
+    custom_holidays: Optional[
+        Union[
+            Dict[Union[dt.date, dt.datetime, str, float, int], str],
+            List[Union[dt.date, dt.datetime, str, float, int]],
+            Union[dt.date, dt.datetime, str, float, int],
+        ]
+    ] = None,
 ) -> busdaycalendar:
     """Function to generate a business calendar
 
     Parameters
     ----------
     startyear: int
         First year in date range generated
@@ -51,17 +54,18 @@
 
     if isinstance(countries, str) and countries in list_supported_countries():
         staging = country_holidays(country=countries, years=years)
         if custom_holidays is not None:
             staging.update(custom_holidays)
         hols = array(sorted(staging.keys()), dtype="datetime64[D]")
     elif isinstance(countries, list) and all(
-        country in list_supported_countries() for country in countries
+        country in list_supported_countries() for country in cast(List[str], countries)
     ):
-        countryholidays: List[dt.date | str] = []
+        country: CountryStringType
+        countryholidays: List[Union[dt.date, str]] = []
         for i, country in enumerate(countries):
             staging = country_holidays(country=country, years=years)
             if i == 0 and custom_holidays is not None:
                 staging.update(custom_holidays)
             countryholidays += list(staging)
         hols = array(sorted(list(set(countryholidays))), dtype="datetime64[D]")
     else:
@@ -70,15 +74,15 @@
             "of string country codes according to ISO 3166-1 alpha-2."
         )
 
     return busdaycalendar(holidays=hols)
 
 
 def date_fix(
-    fixerdate: str | dt.date | dt.datetime | datetime64 | Timestamp,
+    fixerdate: Union[str, dt.date, dt.datetime, datetime64, Timestamp],
 ) -> dt.date:
     """Function to parse from different date formats into datetime.date
 
     Parameters
     ----------
     fixerdate: str | datetime.date | datetime.datetime |
     numpy.datetime64 | pandas.Timestamp
@@ -104,25 +108,26 @@
     raise TypeError(
         f"Unknown date format {str(fixerdate)} of "
         f"type {str(type(fixerdate))} encountered"
     )
 
 
 def date_offset_foll(
-    raw_date: str | dt.date | dt.datetime | datetime64 | Timestamp,
+    raw_date: Union[str, dt.date, dt.datetime, datetime64, Timestamp],
     months_offset: int = 12,
     adjust: bool = False,
     following: bool = True,
-    countries: str | List[str] = "SE",
-    custom_holidays: Union[
-        Dict[Union[dt.date, dt.datetime, str, float, int], str],
-        List[Union[dt.date, dt.datetime, str, float, int]],
-        Union[dt.date, dt.datetime, str, float, int],
-    ]
-    | None = None,
+    countries: CountriesType = "SE",
+    custom_holidays: Optional[
+        Union[
+            Dict[Union[dt.date, dt.datetime, str, float, int], str],
+            List[Union[dt.date, dt.datetime, str, float, int]],
+            Union[dt.date, dt.datetime, str, float, int],
+        ]
+    ] = None,
 ) -> dt.date:
     """Function to offset dates according to a given calendar
 
     Parameters
     ----------
     raw_date: str | datetime.date | datetime.datetime | numpy.datetime64 |
     pandas.Timestamp
@@ -170,22 +175,23 @@
         while not is_busday(dates=new_date, busdaycal=calendar):
             new_date += day_delta
 
     return new_date
 
 
 def get_previous_business_day_before_today(
-    today: dt.date | None = None,
-    countries: str | List[str] = "SE",
-    custom_holidays: Union[
-        Dict[Union[dt.date, dt.datetime, str, float, int], str],
-        List[Union[dt.date, dt.datetime, str, float, int]],
-        Union[dt.date, dt.datetime, str, float, int],
-    ]
-    | None = None,
+    today: Optional[dt.date] = None,
+    countries: CountriesType = "SE",
+    custom_holidays: Optional[
+        Union[
+            Dict[Union[dt.date, dt.datetime, str, float, int], str],
+            List[Union[dt.date, dt.datetime, str, float, int]],
+            Union[dt.date, dt.datetime, str, float, int],
+        ]
+    ] = None,
 ) -> dt.date:
     """Function to bump backwards to find the previous business day before today
 
     Parameters
     ----------
     today: datetime.date, optional
         Manual input of the day from where the previous business day is found
@@ -216,21 +222,22 @@
         following=False,
     )
 
 
 def offset_business_days(
     ddate: dt.date,
     days: int,
-    countries: List[str] | str = "SE",
-    custom_holidays: Union[
-        Dict[Union[dt.date, dt.datetime, str, float, int], str],
-        List[Union[dt.date, dt.datetime, str, float, int]],
-        Union[dt.date, dt.datetime, str, float, int],
-    ]
-    | None = None,
+    countries: CountriesType = "SE",
+    custom_holidays: Optional[
+        Union[
+            Dict[Union[dt.date, dt.datetime, str, float, int], str],
+            List[Union[dt.date, dt.datetime, str, float, int]],
+            Union[dt.date, dt.datetime, str, float, int],
+        ]
+    ] = None,
 ) -> dt.date:
     """Function to bump a date by business days instead of calendar days.
     It first adjusts to a valid business day and then bumps with given
     number of business days from there
 
     Parameters
     ----------
```

## openseries/frame.py

```diff
@@ -6,15 +6,15 @@
 from functools import reduce
 from logging import warning
 from math import ceil
 from os import path
 from pathlib import Path
 from random import choices
 from string import ascii_letters
-from typing import cast, Dict, List, Tuple, Union
+from typing import cast, Dict, List, Optional, Tuple, Union
 from dateutil.relativedelta import relativedelta
 from ffn.core import calc_mean_var_weights, calc_inv_vol_weights, calc_erc_weights
 from numpy import cov, cumprod, log, sqrt
 from openpyxl import Workbook
 from openpyxl.utils.dataframe import dataframe_to_rows
 from pandas import (
     concat,
@@ -25,26 +25,24 @@
     merge,
     MultiIndex,
     Series,
 )
 from pandas.tseries.offsets import CustomBusinessDay
 from plotly.graph_objs import Figure
 from plotly.offline import plot
-from pydantic import field_validator, ConfigDict, BaseModel
-
+from pydantic import BaseModel, field_validator
 from scipy.stats import kurtosis, norm, skew
 import statsmodels.api as sm
-
-# noinspection PyProtectedMember
-from statsmodels.regression.linear_model import RegressionResults
+from statsmodels.base.model import LikelihoodModelResults
 
 from openseries.series import OpenTimeSeries, ValueType, ewma_calc
 from openseries.datefixer import date_offset_foll, holiday_calendar
 from openseries.load_plotly import load_plotly_dict
 from openseries.types import (
+    CountriesType,
     LiteralHowMerge,
     LiteralQuantileInterp,
     LiteralBizDayFreq,
     LiteralPandasResampleConvention,
     LiteralPandasReindexMethod,
     LiteralNanMethod,
     LiteralCaptureRatio,
@@ -63,16 +61,15 @@
     drawdown_series,
     drawdown_details,
     cvar_down,
     var_down,
 )
 
 
-# noinspection PyMethodParameters
-class OpenFrame(BaseModel):
+class OpenFrame(BaseModel, arbitrary_types_allowed=True, validate_assignment=True):
     """Object of the class OpenFrame. Subclass of the Pydantic BaseModel
 
     Parameters
     ----------
     constituents: List[OpenTimeSeries]
         List of objects of Class OpenTimeSeries
     weights: List[float], optional
@@ -82,32 +79,31 @@
     -------
     OpenFrame
         Object of the class OpenFrame
     """
 
     constituents: List[OpenTimeSeries]
     tsdf: DataFrame = DataFrame()
-    weights: None | List[float] = None
-
-    model_config = ConfigDict(arbitrary_types_allowed=True, validate_assignment=True)
+    weights: Optional[List[float]] = None
 
     @field_validator("constituents")
+    @classmethod
     def check_labels_unique(
         cls, tseries: List[OpenTimeSeries]
     ) -> List[OpenTimeSeries]:
         """Pydantic validator ensuring that OpenFrame labels are unique"""
         labls = [x.label for x in tseries]
         if len(set(labls)) != len(labls):
             raise ValueError("TimeSeries names/labels must be unique")
         return tseries
 
     def __init__(
         self: "OpenFrame",
         constituents: List[OpenTimeSeries],
-        weights: List[float] | None = None,
+        weights: Optional[List[float]] = None,
     ) -> None:
         super().__init__(constituents=constituents, weights=weights)
 
         self.constituents = constituents
         self.tsdf = DataFrame(dtype="float64")
         self.weights = weights
 
@@ -129,16 +125,16 @@
         """
 
         return deepcopy(self)
 
     def to_xlsx(
         self: "OpenFrame",
         filename: str,
-        sheet_title: str | None = None,
-        directory: str | None = None,
+        sheet_title: Optional[str] = None,
+        directory: Optional[str] = None,
     ) -> str:
         """Saves the data in the .tsdf DataFrame to an Excel spreadsheet file
 
         Parameters
         ----------
         filename: str
             Filename that should include .xlsx
@@ -204,15 +200,15 @@
             )
         if how == "inner":
             for xerie in self.constituents:
                 xerie.tsdf = xerie.tsdf.loc[self.tsdf.index]
         return self
 
     def all_properties(
-        self: "OpenFrame", properties: List[LiteralFrameProps] | None = None
+        self: "OpenFrame", properties: Optional[List[LiteralFrameProps]] = None
     ) -> DataFrame:
         """Calculates the chosen timeseries properties
 
         Parameters
         ----------
         properties: List[LiteralFrameProps], optional
             The properties to calculate. Defaults to calculating all available.
@@ -230,17 +226,17 @@
                 getattr(self, x) for x in OpenFramePropertiesList.allowed_strings
             ]
         results = concat(prop_list, axis="columns").T
         return results
 
     def calc_range(
         self: "OpenFrame",
-        months_offset: int | None = None,
-        from_dt: dt.date | None = None,
-        to_dt: dt.date | None = None,
+        months_offset: Optional[int] = None,
+        from_dt: Optional[dt.date] = None,
+        to_dt: Optional[dt.date] = None,
     ) -> Tuple[dt.date, dt.date]:
         """Creates user defined date range
 
         Parameters
         ----------
         months_offset: int, optional
             Number of months offset as positive integer. Overrides use of from_date
@@ -288,15 +284,15 @@
                 earlier -= dt.timedelta(days=1)
             while later not in self.tsdf.index.tolist():
                 later += dt.timedelta(days=1)
 
         return earlier, later
 
     def align_index_to_local_cdays(
-        self: "OpenFrame", countries: List[str] | str = "SE"
+        self: "OpenFrame", countries: CountriesType = "SE"
     ) -> "OpenFrame":
         """Changes the index of the associated Pandas DataFrame .tsdf to align with
         local calendar business days
 
         Parameters
         ----------
         countries: List[str] | str, default: "SE"
@@ -498,17 +494,17 @@
             data=(self.tsdf.iloc[-1] / self.tsdf.iloc[0]) ** (1 / self.yearfrac) - 1,
             name="Geometric return",
             dtype="float64",
         )
 
     def geo_ret_func(
         self: "OpenFrame",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> Series:
         """https://www.investopedia.com/terms/c/cagr.asp
 
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
@@ -557,18 +553,18 @@
             data=self.tsdf.pct_change().mean() * self.periods_in_a_year,
             name="Arithmetic return",
             dtype="float64",
         )
 
     def arithmetic_ret_func(
         self: "OpenFrame",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
-        periods_in_a_year_fixed: int | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
+        periods_in_a_year_fixed: Optional[int] = None,
     ) -> Series:
         """https://www.investopedia.com/terms/a/arithmeticmean.asp
 
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
@@ -622,17 +618,17 @@
             data=self.tsdf.iloc[-1] / self.tsdf.iloc[0] - 1,
             name="Total return",
             dtype="float64",
         )
 
     def value_ret_func(
         self: "OpenFrame",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> Series:
         """
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
             and to_date
@@ -656,15 +652,15 @@
         return Series(
             data=self.tsdf.loc[later] / self.tsdf.loc[earlier] - 1,
             name="Subset Total return",
             dtype="float64",
         )
 
     def value_ret_calendar_period(
-        self: "OpenFrame", year: int, month: int | None = None
+        self: "OpenFrame", year: int, month: Optional[int] = None
     ) -> Series:
         """
         Parameters
         ----------
         year : int
             Calendar year of the period to calculate.
         month : int, optional
@@ -705,18 +701,18 @@
             data=self.tsdf.pct_change().std() * sqrt(self.periods_in_a_year),
             name="Volatility",
             dtype="float64",
         )
 
     def vol_func(
         self: "OpenFrame",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
-        periods_in_a_year_fixed: int | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
+        periods_in_a_year_fixed: Optional[int] = None,
     ) -> Series:
         """Based on Pandas .std() which is the equivalent of stdev.s([...])
         in MS Excel \n
         https://www.investopedia.com/terms/v/volatility.asp
 
         Parameters
         ----------
@@ -775,18 +771,18 @@
             name="Downside deviation",
             dtype="float64",
         )
 
     def downside_deviation_func(
         self: "OpenFrame",
         min_accepted_return: float = 0.0,
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
-        periods_in_a_year_fixed: int | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
+        periods_in_a_year_fixed: Optional[int] = None,
     ) -> Series:
         """The standard deviation of returns that are below a Minimum Accepted
         Return of zero.
         It is used to calculate the Sortino Ratio \n
         https://www.investopedia.com/terms/d/downside-deviation.asp
 
         Parameters
@@ -847,20 +843,20 @@
         ratio = self.arithmetic_ret / self.vol
         ratio.name = "Return vol ratio"
         ratio = ratio.astype("float64")
         return ratio
 
     def ret_vol_ratio_func(
         self: "OpenFrame",
-        riskfree_rate: float | None = None,
+        riskfree_rate: Optional[float] = None,
         riskfree_column: Tuple[str, ValueType] | int = -1,
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
-        periods_in_a_year_fixed: int | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
+        periods_in_a_year_fixed: Optional[int] = None,
     ) -> Series:
         """The ratio of annualized arithmetic mean of returns and annualized
         volatility or, if riskfree return provided, Sharpe ratio calculated
         as ( geometric return - risk-free return ) / volatility. The latter ratio
         implies that the riskfree asset has zero volatility. \n
         https://www.investopedia.com/terms/s/sharperatio.asp
 
@@ -1080,20 +1076,20 @@
         sortino = self.arithmetic_ret / self.downside_deviation
         sortino.name = "Sortino ratio"
         sortino = sortino.astype("float64")
         return sortino
 
     def sortino_ratio_func(
         self: "OpenFrame",
-        riskfree_rate: float | None = None,
+        riskfree_rate: Optional[float] = None,
         riskfree_column: Tuple[str, ValueType] | int = -1,
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
-        periods_in_a_year_fixed: int | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
+        periods_in_a_year_fixed: Optional[int] = None,
     ) -> Series:
         """The Sortino ratio calculated as ( return - risk free return )
         / downside deviation. The ratio implies that the riskfree asset has zero
         volatility, and a minimum acceptable return of zero. The ratio is
         calculated using the annualized arithmetic mean of returns. \n
         https://www.investopedia.com/terms/s/sortinoratio.asp
 
@@ -1205,17 +1201,17 @@
             data=(zscframe.iloc[-1] - zscframe.mean()) / zscframe.std(),
             name="Z-score",
             dtype="float64",
         )
 
     def z_score_func(
         self: "OpenFrame",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> Series:
         """https://www.investopedia.com/terms/z/zscore.asp
 
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
@@ -1270,17 +1266,17 @@
             data=md_dates,
             index=self.tsdf.columns,
             name="Max drawdown dates",
         )
 
     def max_drawdown_func(
         self: "OpenFrame",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> Series:
         """https://www.investopedia.com/terms/m/maximum-drawdown-mdd.asp
 
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
@@ -1358,17 +1354,17 @@
             name="Worst month",
             dtype="float64",
         )
 
     def worst_func(
         self: "OpenFrame",
         observations: int = 1,
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> Series:
         """
         Parameters
         ----------
         observations: int, default: 1
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
@@ -1409,17 +1405,17 @@
         answer = pos / tot
         answer.name = "Positive share"
         answer = answer.astype("float64")
         return answer
 
     def positive_share_func(
         self: "OpenFrame",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> Series:
         """
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
             and to_date
@@ -1468,17 +1464,17 @@
             index=self.tsdf.columns,
             name="Skew",
             dtype="float64",
         )
 
     def skew_func(
         self: "OpenFrame",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> Series:
         """https://www.investopedia.com/terms/s/skewness.asp
 
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
@@ -1526,17 +1522,17 @@
             index=self.tsdf.columns,
             name="Kurtosis",
             dtype="float64",
         )
 
     def kurtosis_func(
         self: "OpenFrame",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> Series:
         """https://www.investopedia.com/terms/k/kurtosis.asp
 
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
@@ -1591,17 +1587,17 @@
             name=f"CVaR {level:.1%}",
             dtype="float64",
         )
 
     def cvar_down_func(
         self: "OpenFrame",
         level: float = 0.95,
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> Series:
         """https://www.investopedia.com/terms/c/conditional_value_at_risk.asp
 
         Parameters
         ----------
         level: float, default: 0.95
             The sought CVaR level
@@ -1656,17 +1652,17 @@
             name=f"VaR {level:.1%}",
             dtype="float64",
         )
 
     def var_down_func(
         self: "OpenFrame",
         level: float = 0.95,
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
         interpolation: LiteralQuantileInterp = "lower",
     ) -> Series:
         """https://www.investopedia.com/terms/v/var.asp
         Downside Value At Risk, "VaR". The equivalent of
         percentile.inc([...], 1-level) over returns in MS Excel.
 
         Parameters
@@ -1718,20 +1714,20 @@
         return Series(
             data=imp_vol, name=f"Imp vol from VaR {level:.0%}", dtype="float64"
         )
 
     def vol_from_var_func(
         self: "OpenFrame",
         level: float = 0.95,
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
         interpolation: LiteralQuantileInterp = "lower",
         drift_adjust: bool = False,
-        periods_in_a_year_fixed: int | None = None,
+        periods_in_a_year_fixed: Optional[int] = None,
     ) -> Series:
         """
         Parameters
         ----------
 
         level: float, default: 0.95
             The sought VaR level
@@ -1792,20 +1788,20 @@
 
     def target_weight_from_var(
         self: "OpenFrame",
         target_vol: float = 0.175,
         min_leverage_local: float = 0.0,
         max_leverage_local: float = 99999.0,
         level: float = 0.95,
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
         interpolation: LiteralQuantileInterp = "lower",
         drift_adjust: bool = False,
-        periods_in_a_year_fixed: int | None = None,
+        periods_in_a_year_fixed: Optional[int] = None,
     ) -> Series:
         """A position weight multiplier from the ratio between a VaR implied
         volatility and a given target volatility. Multiplier = 1.0 -> target met
 
         Parameters
         ----------
         target_vol: float, default: 0.175
@@ -1952,15 +1948,15 @@
             ]
 
         return self
 
     def resample_to_business_period_ends(
         self: "OpenFrame",
         freq: LiteralBizDayFreq = "BM",
-        countries: List[str] | str = "SE",
+        countries: CountriesType = "SE",
         convention: LiteralPandasResampleConvention = "end",
         method: LiteralPandasReindexMethod = "nearest",
     ) -> "OpenFrame":
         """Resamples timeseries frequency to the business calendar
         month end dates of each period while leaving any stubs
         in place. Stubs will be aligned to the shortest stub
 
@@ -2057,18 +2053,18 @@
     def ewma_risk(
         self: "OpenFrame",
         lmbda: float = 0.94,
         day_chunk: int = 11,
         dlta_degr_freedms: int = 0,
         first_column: int = 0,
         second_column: int = 1,
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
-        periods_in_a_year_fixed: int | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
+        periods_in_a_year_fixed: Optional[int] = None,
     ) -> DataFrame:
         """Exponentially Weighted Moving Average Model for Volatilities and
         Correlation.
         https://www.investopedia.com/articles/07/ewma.asp
 
         Parameters
         ----------
@@ -2179,15 +2175,15 @@
             data=[raw_one, raw_two, raw_corr],
         ).T
 
     def rolling_vol(
         self: "OpenFrame",
         column: int,
         observations: int = 21,
-        periods_in_a_year_fixed: int | None = None,
+        periods_in_a_year_fixed: Optional[int] = None,
     ) -> DataFrame:
         """
         Parameters
         ----------
         column: int
             Position as integer of column to calculate
         observations: int, default: 21
@@ -2418,16 +2414,16 @@
                 item for item in self.constituents if item.label != lvl_zero_item
             ]
         self.tsdf.drop(lvl_zero_item, axis="columns", level=0, inplace=True)
         return self
 
     def trunc_frame(
         self: "OpenFrame",
-        start_cut: dt.date | None = None,
-        end_cut: dt.date | None = None,
+        start_cut: Optional[dt.date] = None,
+        end_cut: Optional[dt.date] = None,
         before: bool = True,
         after: bool = True,
     ) -> "OpenFrame":
         """Truncates DataFrame such that all timeseries have the same time span
 
         Parameters
         ----------
@@ -2506,18 +2502,18 @@
             self.tsdf[rel_label, ValueType.RELRTRN] = (
                 1.0 + self.tsdf.iloc[:, long_column] - self.tsdf.iloc[:, short_column]
             )
 
     def tracking_error_func(
         self: "OpenFrame",
         base_column: Tuple[str, ValueType] | int = -1,
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
-        periods_in_a_year_fixed: int | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
+        periods_in_a_year_fixed: Optional[int] = None,
     ) -> Series:
         """Calculates the Tracking Error which is the standard deviation of the
         difference between the fund and its index returns. \n
         https://www.investopedia.com/terms/t/trackingerror.asp
 
         Parameters
         ----------
@@ -2583,18 +2579,18 @@
             name=f"Tracking Errors vs {short_label}",
             dtype="float64",
         )
 
     def info_ratio_func(
         self: "OpenFrame",
         base_column: Tuple[str, ValueType] | int = -1,
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
-        periods_in_a_year_fixed: int | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
+        periods_in_a_year_fixed: Optional[int] = None,
     ) -> Series:
         """The Information Ratio equals ( fund return less index return ) divided
         by the Tracking Error. And the Tracking Error is the standard deviation of
         the difference between the fund and its index returns.
         The ratio is calculated using the annualized arithmetic mean of returns.
 
         Parameters
@@ -2663,18 +2659,18 @@
             dtype="float64",
         )
 
     def capture_ratio_func(
         self: "OpenFrame",
         ratio: LiteralCaptureRatio,
         base_column: Tuple[str, ValueType] | int = -1,
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
-        periods_in_a_year_fixed: int | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
+        periods_in_a_year_fixed: Optional[int] = None,
     ) -> Series:
         """The Up (Down) Capture Ratio is calculated by dividing the CAGR
         of the asset during periods that the benchmark returns are positive (negative)
         by the CAGR of the benchmark during the same periods.
         CaptureRatio.BOTH is the Up ratio divided by the Down ratio.
         Source: 'Capture Ratios: A Popular Method of Measuring Portfolio Performance
         in Practice', Don R. Cox and Delbert C. Goff, Journal of Economics and
@@ -2901,15 +2897,15 @@
     def ord_least_squares_fit(
         self: "OpenFrame",
         y_column: Tuple[str, ValueType] | int,
         x_column: Tuple[str, ValueType] | int,
         fitted_series: bool = True,
         method: LiteralOlsFitMethod = "pinv",
         cov_type: LiteralOlsFitCovType = "nonrobust",
-    ) -> RegressionResults:
+    ) -> LikelihoodModelResults:
         """https://www.statsmodels.org/stable/examples/notebooks/generated/ols.html
         Performs a linear regression and adds a new column with a fitted line
         using Ordinary Least Squares fit
 
         Parameters
         ----------
         y_column: Tuple[str, ValueType] | int
@@ -2956,24 +2952,24 @@
             self.tsdf[y_label, x_label] = results.predict(x_value)
 
         return results
 
     def make_portfolio(
         self: "OpenFrame",
         name: str,
-        weight_strat: LiteralPortfolioWeightings | None = None,
-        initial_weights: List[float] | None = None,
-        risk_weights: List[float] | None = None,
+        weight_strat: Optional[LiteralPortfolioWeightings] = None,
+        initial_weights: Optional[List[float]] = None,
+        risk_weights: Optional[List[float]] = None,
         risk_parity_method: LiteralRiskParityMethod = "ccd",
         maximum_iterations: int = 100,
         tolerance: float = 1e-8,
         weight_bounds: Tuple[float, float] = (0.0, 1.0),
         riskfree: float = 0.0,
         covar_method: LiteralCovMethod = "ledoit-wolf",
-        options: Dict[str, int] | None = None,
+        options: Optional[Dict[str, int]] = None,
     ) -> DataFrame:
         """Calculates a basket timeseries based on the supplied weights
 
         Parameters
         ----------
         name: str
             Name of the basket timeseries
@@ -3053,15 +3049,15 @@
         return portfolio
 
     def rolling_info_ratio(
         self: "OpenFrame",
         long_column: int = 0,
         short_column: int = 1,
         observations: int = 21,
-        periods_in_a_year_fixed: int | None = None,
+        periods_in_a_year_fixed: Optional[int] = None,
     ) -> DataFrame:
         """The Information Ratio equals ( fund return less index return ) divided by
         the Tracking Error. And the Tracking Error is the standard deviation of the
         difference between the fund and its index returns.
 
         Parameters
         ----------
@@ -3188,18 +3184,18 @@
         corrdf.columns = [[corr_label], ["Rolling correlation"]]
 
         return corrdf
 
     def plot_series(
         self: "OpenFrame",
         mode: LiteralLinePlotMode = "lines",
-        tick_fmt: str | None = None,
-        filename: str | None = None,
-        directory: str | None = None,
-        labels: List[str] | None = None,
+        tick_fmt: Optional[str] = None,
+        filename: Optional[str] = None,
+        directory: Optional[str] = None,
+        labels: Optional[List[str]] = None,
         auto_open: bool = True,
         add_logo: bool = True,
         show_last: bool = False,
         output_type: LiteralPlotlyOutput = "file",
     ) -> Tuple[Figure, str]:
         """Creates a Plotly Figure
 
@@ -3292,18 +3288,18 @@
         )
 
         return figure, plotfile
 
     def plot_bars(
         self: "OpenFrame",
         mode: LiteralBarPlotMode = "group",
-        tick_fmt: str | None = None,
-        filename: str | None = None,
-        directory: str | None = None,
-        labels: List[str] | None = None,
+        tick_fmt: Optional[str] = None,
+        filename: Optional[str] = None,
+        directory: Optional[str] = None,
+        labels: Optional[List[str]] = None,
         auto_open: bool = True,
         add_logo: bool = True,
         output_type: LiteralPlotlyOutput = "file",
     ) -> Tuple[Figure, str]:
         """Creates a Plotly Bar Figure
 
         Parameters
```

## openseries/risk.py

```diff
@@ -92,25 +92,17 @@
         A timeserie of dates and values
 
     Returns
     -------
     DataFrame | Series
         A drawdown timeserie
     """
-
-    # make a copy so that we don't modify original data
     drawdown = prices.copy()
-
-    # Fill NaN's with previous values
     drawdown = drawdown.fillna(method="ffill")
-
-    # Ignore problems with NaN's in the beginning
     drawdown[isnan(drawdown)] = -Inf
-
-    # Rolling maximum
     roll_max = maximum.accumulate(drawdown)
     drawdown = drawdown / roll_max - 1.0
     return drawdown
 
 
 def drawdown_details(prices: DataFrame | Series) -> Series:
     """Details of the maximum drawdown
```

## openseries/series.py

```diff
@@ -39,15 +39,15 @@
 from scipy.stats import kurtosis, norm, skew
 from stdnum import isin as isincode
 from stdnum.exceptions import InvalidChecksum
 
 from openseries.datefixer import date_offset_foll, date_fix, holiday_calendar
 from openseries.load_plotly import load_plotly_dict
 from openseries.types import (
-    CountryStringType,
+    CountriesType,
     CurrencyStringType,
     DatabaseIdStringType,
     DateListType,
     LiteralQuantileInterp,
     LiteralBizDayFreq,
     LiteralPandasResampleConvention,
     LiteralPandasReindexMethod,
@@ -177,15 +177,15 @@
     valuetype: ValueType
     dates: DateListType
     values: conlist(float, min_length=2)
     local_ccy: bool
     tsdf: DataFrame
     currency: CurrencyStringType
     domestic: CurrencyStringType = "SEK"
-    countries: CountryStringType = "SE"
+    countries: CountriesType = "SE"
     isin: Optional[str] = None
     label: Optional[str] = None
 
     @field_validator("isin")
     @classmethod
     def check_isincode(cls, isin_code: str) -> str:
         """Pydantic validator to ensure that the ISIN code is valid if provided"""
@@ -205,15 +205,15 @@
         dates_set_length = len(set(self.dates))
         if dates_list_length != dates_set_length:
             raise ValueError("Dates are not unique")
         return self
 
     @classmethod
     def setup_class(
-        cls, domestic_ccy: str = "SEK", countries: List[str] | str = "SE"
+        cls, domestic_ccy: CurrencyStringType = "SEK", countries: CountriesType = "SE"
     ) -> None:
         """Sets the domestic currency and calendar of the user.
 
         Parameters
         ----------
         domestic_ccy : str, default: "SEK"
             Currency code according to ISO 4217
@@ -263,15 +263,15 @@
         cls,
         name: str,
         dates: List[str],
         values: List[float],
         valuetype: ValueType = ValueType.PRICE,
         timeseries_id: str = "",
         instrument_id: str = "",
-        baseccy: str = "SEK",
+        baseccy: CurrencyStringType = "SEK",
         local_ccy: bool = True,
     ) -> "OpenTimeSeries":
         """Creates a timeseries from a Pandas DataFrame or Series
 
         Parameters
         ----------
         name: str
@@ -317,15 +317,15 @@
 
     @classmethod
     def from_df(
         cls,
         dframe: DataFrame | Series,
         column_nmbr: int = 0,
         valuetype: ValueType = ValueType.PRICE,
-        baseccy: str = "SEK",
+        baseccy: CurrencyStringType = "SEK",
         local_ccy: bool = True,
     ) -> "OpenTimeSeries":
         """Creates a timeseries from a Pandas DataFrame or Series
 
         Parameters
         ----------
         dframe: DataFrame | Series
@@ -396,20 +396,20 @@
             ),
         )
 
     @classmethod
     def from_fixed_rate(
         cls,
         rate: float,
-        d_range: DatetimeIndex | None = None,
-        days: int | None = None,
-        end_dt: dt.date | None = None,
+        d_range: Optional[DatetimeIndex] = None,
+        days: Optional[int] = None,
+        end_dt: Optional[dt.date] = None,
         label: str = "Series",
         valuetype: ValueType = ValueType.PRICE,
-        baseccy: str = "SEK",
+        baseccy: CurrencyStringType = "SEK",
         local_ccy: bool = True,
     ) -> "OpenTimeSeries":
         """Creates a timeseries from values accruing with a given fixed rate return
 
         Providing a date_range of type Pandas DatetimeIndex takes priority over
         providing a combination of days and an end date.
 
@@ -486,16 +486,16 @@
         """
 
         return deepcopy(self)
 
     def to_xlsx(
         self: "OpenTimeSeries",
         filename: str,
-        sheet_title: str | None = None,
-        directory: str | None = None,
+        sheet_title: Optional[str] = None,
+        directory: Optional[str] = None,
     ) -> str:
         """Saves the data in the .tsdf DataFrame to an Excel spreadsheet file
 
         Parameters
         ----------
         filename: str
             Filename that should include .xlsx
@@ -527,15 +527,15 @@
             wrksheet.append(row)
 
         wrkbook.save(sheetfile)
 
         return sheetfile
 
     def to_json(
-        self: "OpenTimeSeries", filename: str, directory: str | None = None
+        self: "OpenTimeSeries", filename: str, directory: Optional[str] = None
     ) -> Dict[str, str | bool | ValueType | List[str] | List[float]]:
         """Dumps timeseries data into a json file
 
         The label and tsdf parameters are deleted before the json file is saved
 
         Parameters
         ----------
@@ -582,17 +582,17 @@
         dframe.sort_index(inplace=True)
         self.tsdf = dframe
 
         return self
 
     def calc_range(
         self: "OpenTimeSeries",
-        months_offset: int | None = None,
-        from_dt: dt.date | None = None,
-        to_dt: dt.date | None = None,
+        months_offset: Optional[int] = None,
+        from_dt: Optional[dt.date] = None,
+        to_dt: Optional[dt.date] = None,
     ) -> Tuple[dt.date, dt.date]:
         """Creates user defined date range
 
         Parameters
         ----------
         months_offset: int, optional
             Number of months offset as positive integer. Overrides use of from_date
@@ -670,15 +670,15 @@
         ]
 
         self.tsdf = self.tsdf.reindex(d_range, method=None, copy=False)
 
         return self
 
     def all_properties(
-        self: "OpenTimeSeries", properties: List[LiteralSeriesProps] | None = None
+        self: "OpenTimeSeries", properties: Optional[List[LiteralSeriesProps]] = None
     ) -> DataFrame:
         """Calculates the chosen timeseries properties
 
         Parameters
         ----------
         properties: List[LiteralSeriesProps], optional
             The properties to calculate. Defaults to calculating all available.
@@ -792,17 +792,17 @@
             )
             ** (1 / self.yearfrac)
             - 1,
         )
 
     def geo_ret_func(
         self: "OpenTimeSeries",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> float:
         """https://www.investopedia.com/terms/c/cagr.asp
 
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
@@ -852,18 +852,18 @@
             Annualized arithmetic mean of returns
         """
 
         return float((self.tsdf.pct_change().mean() * self.periods_in_a_year).iloc[0])
 
     def arithmetic_ret_func(
         self: "OpenTimeSeries",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
-        periods_in_a_year_fixed: int | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
+        periods_in_a_year_fixed: Optional[int] = None,
     ) -> float:
         """https://www.investopedia.com/terms/a/arithmeticmean.asp
 
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
@@ -915,17 +915,17 @@
                 "Simple Return cannot be calculated due to an initial value being "
                 "zero."
             )
         return float((self.tsdf.iloc[-1] / self.tsdf.iloc[0] - 1).iloc[0])
 
     def value_ret_func(
         self: "OpenTimeSeries",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> float:
         """
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
             and to_date
@@ -945,15 +945,15 @@
             raise ValueError(
                 "Simple Return cannot be calculated due to an initial value being "
                 "zero."
             )
         return float((self.tsdf.loc[later] / self.tsdf.loc[earlier] - 1).iloc[0])
 
     def value_ret_calendar_period(
-        self: "OpenTimeSeries", year: int, month: int | None = None
+        self: "OpenTimeSeries", year: int, month: Optional[int] = None
     ) -> float:
         """
         Parameters
         ----------
         year : int
             Calendar year of the period to calculate.
         month : int, optional
@@ -990,18 +990,18 @@
         return cast(
             float,
             (self.tsdf.pct_change().std() * sqrt(self.periods_in_a_year)).iloc[0],
         )
 
     def vol_func(
         self: "OpenTimeSeries",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
-        periods_in_a_year_fixed: int | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
+        periods_in_a_year_fixed: Optional[int] = None,
     ) -> float:
         """Based on Pandas .std() which is the equivalent of stdev.s([...])
         in MS Excel \n
         https://www.investopedia.com/terms/v/volatility.asp
 
         Parameters
         ----------
@@ -1059,18 +1059,18 @@
             sqrt((dddf[dddf.values < 0.0].values ** 2).sum() / self.length)
             * sqrt(self.periods_in_a_year),
         )
 
     def downside_deviation_func(
         self: "OpenTimeSeries",
         min_accepted_return: float = 0.0,
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
-        periods_in_a_year_fixed: int | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
+        periods_in_a_year_fixed: Optional[int] = None,
     ) -> float:
         """The standard deviation of returns that are below a Minimum Accepted
         Return of zero.
         It is used to calculate the Sortino Ratio \n
         https://www.investopedia.com/terms/d/downside-deviation.asp
 
         Parameters
@@ -1129,17 +1129,17 @@
             Ratio of the annualized arithmetic mean of returns and annualized
             volatility.
         """
         return self.arithmetic_ret / self.vol
 
     def ret_vol_ratio_func(
         self: "OpenTimeSeries",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
         riskfree_rate: float = 0.0,
     ) -> float:
         """The ratio of annualized arithmetic mean of returns and annualized
         volatility or, if risk-free return provided, Sharpe ratio calculated
         as ( geometric return - risk-free return ) / volatility. The latter ratio
         implies that the riskfree asset has zero volatility. \n
         https://www.investopedia.com/terms/s/sharperatio.asp
@@ -1182,17 +1182,17 @@
             volatility, and a minimum acceptable return of zero.
         """
 
         return self.arithmetic_ret / self.downside_deviation
 
     def sortino_ratio_func(
         self: "OpenTimeSeries",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
         riskfree_rate: float = 0.0,
     ) -> float:
         """The Sortino ratio calculated as ( asset return - risk free return )
         / downside deviation. The ratio implies that the riskfree asset has
         zero volatility. \n
         https://www.investopedia.com/terms/s/sortinoratio.asp
 
@@ -1242,17 +1242,17 @@
                 (self.tsdf.pct_change().iloc[-1] - self.tsdf.pct_change().mean())
                 / self.tsdf.pct_change().std()
             ).iloc[0],
         )
 
     def z_score_func(
         self: "OpenTimeSeries",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> float:
         """https://www.investopedia.com/terms/z/zscore.asp
 
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
@@ -1300,17 +1300,17 @@
         mdddf = self.tsdf.copy()
         mdddf.index = DatetimeIndex(mdddf.index)
         mdd_date = (mdddf / mdddf.expanding(min_periods=1).max()).idxmin().values[0]
         return dt.datetime.strptime(str(mdd_date)[:10], "%Y-%m-%d").date()
 
     def max_drawdown_func(
         self: "OpenTimeSeries",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> float:
         """https://www.investopedia.com/terms/m/maximum-drawdown-mdd.asp
 
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
@@ -1382,17 +1382,17 @@
         resdf = self.tsdf.copy()
         resdf.index = DatetimeIndex(resdf.index)
         return float((resdf.resample("BM").last().pct_change().min()).iloc[0])
 
     def worst_func(
         self: "OpenTimeSeries",
         observations: int = 1,
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> float:
         """
         Parameters
         ----------
         observations: int, default: 1
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
@@ -1434,17 +1434,17 @@
             self.tsdf.pct_change()[1:].values >= 0.0
         ].count()
         tot = self.tsdf.pct_change()[1:].count()
         return float((pos / tot).iloc[0])
 
     def positive_share_func(
         self: "OpenTimeSeries",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> float:
         """
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
             and to_date
@@ -1482,17 +1482,17 @@
         return cast(
             float,
             skew(a=self.tsdf.pct_change().values, bias=True, nan_policy="omit")[0],
         )
 
     def skew_func(
         self: "OpenTimeSeries",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> float:
         """https://www.investopedia.com/terms/s/skewness.asp
 
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
@@ -1535,17 +1535,17 @@
                 bias=True,
                 nan_policy="omit",
             )[0],
         )
 
     def kurtosis_func(
         self: "OpenTimeSeries",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> float:
         """https://www.investopedia.com/terms/k/kurtosis.asp
 
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
@@ -1594,17 +1594,17 @@
                 .mean()
             ),
         )
 
     def cvar_down_func(
         self: "OpenTimeSeries",
         level: float = 0.95,
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> float:
         """https://www.investopedia.com/terms/c/conditional_value_at_risk.asp
 
         Parameters
         ----------
         level: float, default: 0.95
             The sought CVaR level
@@ -1664,17 +1664,17 @@
                 .iloc[0]
             ),
         )
 
     def var_down_func(
         self: "OpenTimeSeries",
         level: float = 0.95,
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
         interpolation: LiteralQuantileInterp = "lower",
     ) -> float:
         """https://www.investopedia.com/terms/v/var.asp
         Downside Value At Risk, "VaR". The equivalent of
         percentile.inc([...], 1-level) over returns in MS Excel.
 
         Parameters
@@ -1727,20 +1727,20 @@
                 / norm.ppf(level)
             ),
         )
 
     def vol_from_var_func(
         self: "OpenTimeSeries",
         level: float = 0.95,
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
         interpolation: LiteralQuantileInterp = "lower",
         drift_adjust: bool = False,
-        periods_in_a_year_fixed: int | None = None,
+        periods_in_a_year_fixed: Optional[int] = None,
     ) -> float:
         """
         Parameters
         ----------
 
         level: float, default: 0.95
             The sought VaR level
@@ -1813,20 +1813,20 @@
 
     def target_weight_from_var(
         self: "OpenTimeSeries",
         target_vol: float = 0.175,
         min_leverage_local: float = 0.0,
         max_leverage_local: float = 99999.0,
         level: float = 0.95,
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
         interpolation: LiteralQuantileInterp = "lower",
         drift_adjust: bool = False,
-        periods_in_a_year_fixed: int | None = None,
+        periods_in_a_year_fixed: Optional[int] = None,
     ) -> float:
         """A position weight multiplier from the ratio between a VaR implied
         volatility and a given target volatility. Multiplier = 1.0 -> target met
 
         Parameters
         ----------
         target_vol: float, default: 0.175
@@ -2086,18 +2086,18 @@
         return drawdown_details(dddf).to_frame()
 
     def ewma_vol_func(
         self: "OpenTimeSeries",
         lmbda: float = 0.94,
         day_chunk: int = 11,
         dlta_degr_freedms: int = 0,
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
-        periods_in_a_year_fixed: int | None = None,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
+        periods_in_a_year_fixed: Optional[int] = None,
     ) -> Series:
         """Exponentially Weighted Moving Average Model for Volatility.
         https://www.investopedia.com/articles/07/ewma.asp
 
         Parameters
         ----------
         lmbda: float, default: 0.94
@@ -2159,15 +2159,15 @@
         data.loc[:, (self.label, ValueType.EWMA)] = rawdata
 
         return data.loc[:, (self.label, ValueType.EWMA)]
 
     def rolling_vol(
         self: "OpenTimeSeries",
         observations: int = 21,
-        periods_in_a_year_fixed: int | None = None,
+        periods_in_a_year_fixed: Optional[int] = None,
     ) -> DataFrame:
         """
         Parameters
         ----------
         observations: int, default: 21
             Number of observations in the overlapping window.
         periods_in_a_year_fixed : int, optional
@@ -2369,16 +2369,16 @@
         self.tsdf.index = [d.date() for d in DatetimeIndex(self.tsdf.index)]
         if returns_input:
             self.value_to_ret()
         return self
 
     def set_new_label(
         self: "OpenTimeSeries",
-        lvl_zero: str | None = None,
-        lvl_one: ValueType | None = None,
+        lvl_zero: Optional[str] = None,
+        lvl_one: Optional[ValueType] = None,
         delete_lvl_one: bool = False,
     ) -> "OpenTimeSeries":
         """Sets the column labels of the .tsdf Pandas Dataframe associated
         with the timeseries
 
         Parameters
         ----------
@@ -2411,16 +2411,16 @@
         if delete_lvl_one:
             self.tsdf.columns = self.tsdf.columns.droplevel(level=1)
         return self
 
     def plot_series(
         self: "OpenTimeSeries",
         mode: LiteralLinePlotMode = "lines",
-        tick_fmt: str | None = None,
-        directory: str | None = None,
+        tick_fmt: Optional[str] = None,
+        directory: Optional[str] = None,
         auto_open: bool = True,
         add_logo: bool = True,
         show_last: bool = False,
         output_type: LiteralPlotlyOutput = "file",
     ) -> Tuple[Figure, str]:
         """Creates a Plotly Figure
 
@@ -2503,16 +2503,16 @@
         )
 
         return figure, plotfile
 
     def plot_bars(
         self: "OpenTimeSeries",
         mode: LiteralBarPlotMode = "group",
-        tick_fmt: str | None = None,
-        directory: str | None = None,
+        tick_fmt: Optional[str] = None,
+        directory: Optional[str] = None,
         auto_open: bool = True,
         add_logo: bool = True,
         output_type: LiteralPlotlyOutput = "file",
     ) -> Tuple[Figure, str]:
         """Creates a Plotly Bar Figure
 
         Parameters
```

## openseries/sim_price.py

```diff
@@ -1,16 +1,21 @@
 """
 Defining the ReturnSimulation class which simulates returns based on
 stochastic processes generated using the stoch_process.py module.
 """
-from typing import cast
+import datetime as dt
+from typing import cast, Tuple
 from numpy import insert, random, sqrt
-from pandas import DataFrame
+from pandas import DataFrame, date_range
+from pandas.tseries.offsets import CustomBusinessDay
 from pydantic import ConfigDict, BaseModel
 
+from openseries.datefixer import holiday_calendar
+from openseries.frame import OpenFrame
+from openseries.series import OpenTimeSeries, ValueType
 from openseries.stoch_processes import (
     ModelParameters,
     geometric_brownian_motion_log_returns,
     geometric_brownian_motion_jump_diffusion_levels,
     heston_model_levels,
 )
 
@@ -439,7 +444,54 @@
             number_of_sims=number_of_sims,
             trading_days=trading_days,
             trading_days_in_year=trading_days_in_year,
             mean_annual_return=mean_annual_return,
             mean_annual_vol=mean_annual_vol,
             dframe=DataFrame(data=daily_returns),
         )
+
+
+def make_simulated_data_from_merton_jump_gbm() -> Tuple[OpenTimeSeries, OpenFrame]:
+    """Creates OpenTimeSeries and OpenFrame based on a
+    Merton Jump-Diffusion model simulation
+
+    Returns
+    -------
+    Tuple[OpenTimeSeries, OpenFrame]
+        Objects based on a simulation
+    """
+    OpenTimeSeries.setup_class()
+
+    sim = ReturnSimulation.from_merton_jump_gbm(
+        number_of_sims=5,
+        trading_days=2512,
+        mean_annual_return=0.05,
+        mean_annual_vol=0.1,
+        jumps_lamda=0.00125,
+        jumps_sigma=0.001,
+        jumps_mu=-0.2,
+        seed=71,
+    )
+    end = dt.date(2019, 6, 30)
+    startyear = 2009
+    calendar = holiday_calendar(
+        startyear=startyear, endyear=end.year, countries=OpenTimeSeries.countries
+    )
+    d_range = [
+        d.date()
+        for d in date_range(
+            periods=sim.trading_days,
+            end=end,
+            freq=CustomBusinessDay(calendar=calendar),
+        )
+    ]
+    sdf = sim.dframe.iloc[0].T.to_frame()
+    sdf.index = d_range
+    sdf.columns = [["Asset"], [ValueType.RTRN]]
+    series = OpenTimeSeries.from_df(sdf, valuetype=ValueType.RTRN).to_cumret()
+    tslist = []
+    for item in range(sim.number_of_sims):
+        sdf = sim.dframe.iloc[item].T.to_frame()
+        sdf.index = d_range
+        sdf.columns = [[f"Asset_{item}"], [ValueType.RTRN]]
+        tslist.append(OpenTimeSeries.from_df(sdf, valuetype=ValueType.RTRN))
+    return series, OpenFrame(tslist)
```

## openseries/stoch_processes.py

```diff
@@ -12,15 +12,15 @@
 - The Heston Stochastic Volatility Model
 - Cox Ingersoll Ross
 - Ornstein Uhlenbeck
 
 """
 from math import log, sqrt
 from math import pow as mathpow
-from typing import Any, List, Tuple
+from typing import Any, List, Optional, Tuple
 from numpy import add, array, dtype, ndarray, exp, float64
 import numpy.random as nrand
 
 from openseries.types import ModelParameters
 
 __all__ = [
     "ModelParameters",
@@ -59,15 +59,15 @@
     for rtn in range(1, len(returns)):
         # Add the price at t-1 * return at t
         price_sequence.append(price_sequence[rtn - 1] * returns[rtn - 1])
     return array(price_sequence)
 
 
 def brownian_motion_log_returns(
-    param: ModelParameters, seed: int | None = None
+    param: ModelParameters, seed: Optional[int] = None
 ) -> ndarray[Any, dtype[float64]]:
     """This method returns a Wiener process. The Wiener process is also called
     Brownian motion. For more information about the Wiener process check out
     the Wikipedia page: http://en.wikipedia.org/wiki/Wiener_process
 
     Parameters
     ----------
@@ -86,15 +86,15 @@
         nrand.seed(seed)
 
     sqrt_delta_sigma = sqrt(param.all_delta) * param.all_sigma
     return nrand.normal(loc=0, scale=sqrt_delta_sigma, size=param.all_time)
 
 
 def brownian_motion_levels(
-    param: ModelParameters, seed: int | None = None
+    param: ModelParameters, seed: Optional[int] = None
 ) -> ndarray[Any, dtype[float64]]:
     """Delivers a price sequence whose returns evolve according to a brownian motion
 
     Parameters
     ----------
     param: ModelParameters
         Model input
@@ -107,15 +107,15 @@
         Price sequence which follows a brownian motion
     """
 
     return convert_to_prices(param, brownian_motion_log_returns(param, seed=seed))
 
 
 def geometric_brownian_motion_log_returns(
-    param: ModelParameters, seed: int | None = None
+    param: ModelParameters, seed: Optional[int] = None
 ) -> ndarray[Any, dtype[float64]]:
     """This method constructs a sequence of log returns which, when
     exponentiated, produce a random Geometric Brownian Motion (GBM).
     GBM is the stochastic process underlying the Black Scholes
     options pricing formula
 
     Parameters
@@ -135,15 +135,15 @@
     sigma_pow_mu_delta = (
         param.gbm_mu - 0.5 * mathpow(param.all_sigma, 2.0)
     ) * param.all_delta
     return wiener_process + sigma_pow_mu_delta
 
 
 def geometric_brownian_motion_levels(
-    param: ModelParameters, seed: int | None = None
+    param: ModelParameters, seed: Optional[int] = None
 ) -> ndarray[Any, dtype[float64]]:
     """Prices for an asset which evolves according to a geometric brownian motion
 
     Parameters
     ----------
     param: ModelParameters
         Model input
@@ -158,15 +158,15 @@
 
     return convert_to_prices(
         param, geometric_brownian_motion_log_returns(param, seed=seed)
     )
 
 
 def jump_diffusion_process(
-    param: ModelParameters, seed: int | None = None
+    param: ModelParameters, seed: Optional[int] = None
 ) -> ndarray[Any, dtype[float64]]:
     """This method produces a sequence of Jump Sizes which represent a jump
     diffusion process. These jumps are combined with a geometric brownian
     motion (log returns) to produce the Merton model
 
     Parameters
     ----------
@@ -200,15 +200,15 @@
                 jump_sizes[j] += nrand.normal(param.jumps_mu, param.jumps_sigma)
                 break
         time += 1
     return array(jump_sizes)
 
 
 def geometric_brownian_motion_jump_diffusion_log_returns(
-    param: ModelParameters, seed: int | None = None
+    param: ModelParameters, seed: Optional[int] = None
 ) -> ndarray[Any, dtype[float64]]:
     """This method constructs combines a geometric brownian motion process
     (log returns) with a jump diffusion process (log returns) to produce a
     sequence of gbm jump returns
 
     Parameters
     ----------
@@ -225,15 +225,15 @@
 
     jump_diffusion = jump_diffusion_process(param, seed=seed)
     geometric_brownian_motion = geometric_brownian_motion_log_returns(param, seed=seed)
     return add(jump_diffusion, geometric_brownian_motion)
 
 
 def geometric_brownian_motion_jump_diffusion_levels(
-    param: ModelParameters, seed: int | None = None
+    param: ModelParameters, seed: Optional[int] = None
 ) -> ndarray[Any, dtype[float64]]:
     """Converts returns generated with a Geometric Brownian Motion process
     with jumps into prices
 
     Parameters
     ----------
     param: ModelParameters
@@ -252,15 +252,15 @@
         geometric_brownian_motion_jump_diffusion_log_returns(param, seed=seed),
     )
 
 
 def heston_construct_correlated_path(
     param: ModelParameters,
     brownian_motion_one: ndarray[Any, dtype[float64]],
-    seed: int | None = None,
+    seed: Optional[int] = None,
 ) -> Tuple[ndarray[Any, dtype[float64]], ndarray[Any, dtype[float64]]]:
     """This method is a simplified version of the Cholesky decomposition method for
     just two assets. It does not make use of matrix algebra and is therefore quite
     easy to implement
 
     Parameters
     ----------
@@ -287,15 +287,15 @@
         term_one = param.cir_rho * brownian_motion_one[npath]
         term_two = sqrt(1 - mathpow(param.cir_rho, 2.0)) * nrand.normal(0, sqrt_delta)
         brownian_motion_two.append(term_one + term_two)
     return array(brownian_motion_one), array(brownian_motion_two)
 
 
 def cox_ingersoll_ross_heston(
-    param: ModelParameters, seed: int | None = None
+    param: ModelParameters, seed: Optional[int] = None
 ) -> Tuple[ndarray[Any, dtype[float64]], ndarray[Any, dtype[float64]]]:
     """This method returns the rate levels of a mean-reverting Cox Ingersoll Ross
     process. It is used to model interest rates as well as stochastic
     volatility in the Heston model. Because the returns between the underlying
     and the stochastic volatility should be correlated we pass a correlated
     Brownian motion process into the method from which the interest rate levels
     are constructed. The other correlated process is used in the Heston model
@@ -334,15 +334,15 @@
             * brownian_motion_volatility[hpath - 1]
         )
         volatilities.append(max(volatilities[-1], 0.05) + drift + randomness)
     return array(brownian_motion_volatility), array(volatilities)
 
 
 def heston_model_levels(
-    param: ModelParameters, seed: int | None = None
+    param: ModelParameters, seed: Optional[int] = None
 ) -> Tuple[ndarray[Any, dtype[float64]], ndarray[Any, dtype[float64]]]:
     """The Heston model is the geometric brownian motion model with stochastic
     volatility. This stochastic volatility is given by the Cox Ingersoll Ross
     process. Step one on this method is to construct two correlated
     GBM processes. One is used for the underlying asset prices and the other
     is used for the stochastic volatility levels
     Get two correlated brownian motion sequences for the volatility parameter
@@ -378,15 +378,15 @@
         heston_market_price_levels.append(
             heston_market_price_levels[hpath - 1] + drift + vol
         )
     return array(heston_market_price_levels), array(cir_process)
 
 
 def cox_ingersoll_ross_levels(
-    param: ModelParameters, seed: int | None = None
+    param: ModelParameters, seed: Optional[int] = None
 ) -> ndarray[Any, dtype[float64]]:
     """This method returns the rate levels of a mean-reverting Cox Ingersoll Ross
     process. It is used to model interest rates as well as stochastic
     volatility in the Heston model. Because the returns between the underlying
     and the stochastic volatility should be correlated we pass a correlated
     Brownian motion process into the method from which the interest rate levels
     are constructed. The other correlated process is used in the Heston model
@@ -413,15 +413,15 @@
         drift = cir_mean_rev * (cir_avg_ir - levels[hpath - 1]) * param.all_delta
         randomness = sqrt(levels[hpath - 1]) * brownian_motion[hpath - 1]
         levels.append(levels[hpath - 1] + drift + randomness)
     return array(levels)
 
 
 def ornstein_uhlenbeck_levels(
-    param: ModelParameters, seed: int | None = None
+    param: ModelParameters, seed: Optional[int] = None
 ) -> ndarray[Any, dtype[float64]]:
     """This method returns the rate levels of a mean-reverting
     Ornstein Uhlenbeck process
 
     Parameters
     ----------
     param: ModelParameters
```

## openseries/types.py

```diff
@@ -1,22 +1,18 @@
 """
 Declaring types used throughout the project
 """
-from typing import Literal, List
+from typing import Literal, List, TypeAlias, Union
 from pydantic import BaseModel, conlist, constr
 
 
-CountryStringType = conlist(
-    constr(
-        pattern=r"^[A-Z]{2}$", to_upper=True, min_length=2, max_length=2, strict=True
-    ),
-    min_length=1,
-) | constr(
+CountryStringType = constr(
     pattern=r"^[A-Z]{2}$", to_upper=True, min_length=2, max_length=2, strict=True
 )
+CountriesType = Union[conlist(CountryStringType, min_length=1), CountryStringType]
 
 CurrencyStringType = constr(
     pattern=r"^[A-Z]{3}$", to_upper=True, min_length=3, max_length=3, strict=True
 )
 
 DateListType = conlist(
     constr(pattern=r"^\d{4}-(0[1-9]|1[0-2])-(0[1-9]|[12]\d|3[01])$"), min_length=2
@@ -28,43 +24,47 @@
     "lines",
     "markers",
     "lines+markers",
     "lines+text",
     "markers+text",
     "lines+markers+text",
 ]
-LiteralHowMerge = Literal["outer", "inner"]
-LiteralQuantileInterp = Literal["linear", "lower", "higher", "midpoint", "nearest"]
-LiteralBizDayFreq = Literal["BM", "BQ", "BA"]
-LiteralPandasResampleConvention = Literal["start", "s", "end", "e"]
-LiteralPandasReindexMethod = Literal[
+LiteralHowMerge: TypeAlias = Literal["outer", "inner"]
+LiteralQuantileInterp: TypeAlias = Literal[
+    "linear", "lower", "higher", "midpoint", "nearest"
+]
+LiteralBizDayFreq: TypeAlias = Literal["BM", "BQ", "BA"]
+LiteralPandasResampleConvention: TypeAlias = Literal["start", "s", "end", "e"]
+LiteralPandasReindexMethod: TypeAlias = Literal[
     None, "pad", "ffill", "backfill", "bfill", "nearest"
 ]
-LiteralNanMethod = Literal["fill", "drop"]
-LiteralCaptureRatio = Literal["up", "down", "both"]
-LiteralBarPlotMode = Literal["stack", "group", "overlay", "relative"]
-LiteralPlotlyOutput = Literal["file", "div"]
-LiteralOlsFitMethod = Literal["pinv", "qr"]
-LiteralPortfolioWeightings = Literal["eq_weights", "eq_risk", "inv_vol", "mean_var"]
-LiteralCovMethod = Literal["ledoit-wolf", "standard"]
-LiteralRiskParityMethod = Literal["ccd", "slsqp"]
-LiteralOlsFitCovType = Literal[
+LiteralNanMethod: TypeAlias = Literal["fill", "drop"]
+LiteralCaptureRatio: TypeAlias = Literal["up", "down", "both"]
+LiteralBarPlotMode: TypeAlias = Literal["stack", "group", "overlay", "relative"]
+LiteralPlotlyOutput: TypeAlias = Literal["file", "div"]
+LiteralOlsFitMethod: TypeAlias = Literal["pinv", "qr"]
+LiteralPortfolioWeightings: TypeAlias = Literal[
+    "eq_weights", "eq_risk", "inv_vol", "mean_var"
+]
+LiteralCovMethod: TypeAlias = Literal["ledoit-wolf", "standard"]
+LiteralRiskParityMethod: TypeAlias = Literal["ccd", "slsqp"]
+LiteralOlsFitCovType: TypeAlias = Literal[
     "nonrobust",
     "fixed scale",
     "HC0",
     "HC1",
     "HC2",
     "HC3",
     "HAC",
     "hac-panel",
     "hac-groupsum",
     "cluster",
 ]
 
-LiteralSeriesProps = Literal[
+LiteralSeriesProps: TypeAlias = Literal[
     "value_ret",
     "geo_ret",
     "arithmetic_ret",
     "vol",
     "downside_deviation",
     "ret_vol_ratio",
     "sortino_ratio",
@@ -83,15 +83,15 @@
     "first_idx",
     "last_idx",
     "length",
     "span_of_days",
     "yearfrac",
     "periods_in_a_year",
 ]
-LiteralFrameProps = Literal[
+LiteralFrameProps: TypeAlias = Literal[
     "value_ret",
     "geo_ret",
     "arithmetic_ret",
     "vol",
     "downside_deviation",
     "ret_vol_ratio",
     "sortino_ratio",
```

## Comparing `openseries-1.1.0.dist-info/LICENSE.md` & `openseries-1.1.1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `openseries-1.1.0.dist-info/METADATA` & `openseries-1.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openseries
-Version: 1.1.0
+Version: 1.1.1
 Summary: Package for simple financial time series analysis.
 Home-page: https://github.com/CaptorAB/OpenSeries
 License: BSD-3-Clause
 Keywords: python,python3,plotly,pandas,finance,fintech,data-science,timeseries,timeseries-data,timeseries-analysis,investment,investment-analysis,investing
 Author: Martin Karrin
 Author-email: martin.karrin@captor.se
 Requires-Python: >=3.10,<3.12
@@ -64,18 +64,15 @@
 
 An overview of an OpenTimeSeries object is shown in the below example. It shows how to
 create an object from a constructing classmethod. The design aligns with how we within
 our fund company's code base have a subclass of OpenTimeSeries with class methods
 for our different data sources. Combined with some additional tools it allows us to
 efficiently present investment cases to clients.
 
-The OpenTimeSeries and OpenFrame classes are both subclasses of
-the [Pydantic BaseModel](https://docs.pydantic.dev/usage/models/).
-
-To make use of some tools available in the [Pandas](https://pandas.pydata.org/) library
+To make use of the tools available in the [Pandas](https://pandas.pydata.org/) library
 the [OpenTimeSeries](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/series.py)
 and [OpenFrame](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/frame.py)
 classes have an attribute `tsdf`
 which is a DataFrame constructed from the raw data in the lists `dates` and `values`.
 
 ```python
 from openseries.series import OpenTimeSeries
@@ -121,18 +118,22 @@
 ### Usage example on Jupyter Nbviewer
 
 [![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.org/github/karrmagadgeteer2/NoteBook/blob/master/openseriesnotebook.ipynb)
 
 
 ## Development Instructions
 
-These instructions assume that you
-have a compatible Python version installed on your machine and that you are OK
-to install this project in a virtual environment. If not, feel free to do it your
-own way.
+These instructions assume that you have a compatible Python version installed on
+your machine and that you are OK to install this project in a virtual environment.
+If not, feel free to do it your own way.
+
+The OpenTimeSeries and OpenFrame classes are both subclasses of
+the [Pydantic BaseModel](https://docs.pydantic.dev/usage/models/). Please refer to its documentation for information
+on any attributes or methods inherited from this model.
+
 
 ### Windows Powershell
 
 ```powershell
 git clone https://github.com/CaptorAB/OpenSeries.git
 cd OpenSeries
 ./make.ps1 -task make
@@ -209,15 +210,14 @@
 ### Class methods used to construct objects.
 
 | Method            | Applies to                    | Description                                                                                        |
 |:------------------|:------------------------------|:---------------------------------------------------------------------------------------------------|
 | `from_arrays`     | `OpenTimeSeries`              | Class method to create an OpenTimeSeries object from a list of date strings and a list of values.  |
 | `from_df`         | `OpenTimeSeries`              | Class method to create an OpenTimeSeries object from a pandas.DataFrame or pandas.Series.          |
 | `from_fixed_rate` | `OpenTimeSeries`              | Class method to create an OpenTimeSeries object from a fixed rate, number of days and an end date. |
-| `parse_obj`       | `OpenTimeSeries`              | A method inherited from the Pydantic BaseModel to construct an object from a `dict`.               |
 | `from_deepcopy`   | `OpenTimeSeries`, `OpenFrame` | Creates a copy of an OpenTimeSeries object.                                                        |
 
 ### Non-numerical or "helper" properties that apply only to the [OpenTimeSeries](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/series.py) class.
 
 | Property       | type            | Applies to       | Description                                                                                                                                  |
 |:---------------|:----------------|:-----------------|:---------------------------------------------------------------------------------------------------------------------------------------------|
 | `timeseriesId` | `str`           | `OpenTimeSeries` | Placeholder for database identifier for the timeseries. Can be left as empty string.                                                         |
```

## Comparing `openseries-1.1.0.dist-info/RECORD` & `openseries-1.1.1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 openseries/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-openseries/datefixer.py,sha256=h4zshiUkJmRmbBgiCCVulxVUa2SO1dRdJMAKLMxE-tc,9970
-openseries/frame.py,sha256=nHRVfYRYPDIV32W6KCMEaJ7d9wG1qWMaeK_6JwfHnOM,115113
+openseries/datefixer.py,sha256=oNDIIQgm2vYxLIVS2kow1SMPn1KcZTjgwgVJfPcccTU,10224
+openseries/frame.py,sha256=bhPaWvzZQcKW7P93U1VT6mKMjydV2cfuJiigai1_nEs,115343
 openseries/load_plotly.py,sha256=DfpacL-aL5z-W0Cw7FL4YtDSbgeSI8Q-8DO6940wiJc,1119
 openseries/plotly_captor_logo.json,sha256=pGMuPVu4cEO3ZsCH1wU03hxqbIQkHFNoJUs1k1WK89Y,178
 openseries/plotly_layouts.json,sha256=xhrMOqW8LXb4QMtPiNBGdkPX518OHThiIJ68jpQk524,1429
-openseries/risk.py,sha256=_NJd8V-6pMx8pTodW-QpGKlmCDbCn4TsEjieKnCkIxU,4404
-openseries/series.py,sha256=ytojrTbUtgi6Pmh4DbJd_SFIDP-A4xJE2BLaShStwqs,84308
-openseries/sim_price.py,sha256=2UQKJ9p2_0A10PbxadP5EhjeC9LRBP7IsoQdwQBKHNA,13822
-openseries/stoch_processes.py,sha256=6O4C_nC2iBseWggvDDC2gTpTqS5fI5nfjSRpccaazLE,14673
-openseries/types.py,sha256=wz-G8BrlB4NjxDpcJUwYO5PhEjfKI52uoO53k3VkJEQ,7082
-openseries-1.1.0.dist-info/LICENSE.md,sha256=NJjeq3wyB7EnnHLmsdK1EK6zT00T1eB3FgAmHAPT_vM,1521
-openseries-1.1.0.dist-info/METADATA,sha256=l7BJzQc--wMAzmYRy2mjo1Gq3bI8VaeZu9YAmJn-z3s,47925
-openseries-1.1.0.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-openseries-1.1.0.dist-info/RECORD,,
+openseries/risk.py,sha256=rAb2Mcd--pS77BgtyFz22QxUmeMS3zICyZ2NhyyQo3M,4234
+openseries/series.py,sha256=moqaN9CMx23xPLPK9ZGu9NzxJy0esZUYq-kpRy-At8A,84592
+openseries/sim_price.py,sha256=7_0NUbx01-d_BmvHnbmDfuCyB5my3Zn9utbu39jDPnc,15521
+openseries/stoch_processes.py,sha256=0s8W-jPaUMkRau7InmSkRgqyoKIbvL4CgoJajPJoQ30,14719
+openseries/types.py,sha256=HqkEf5AcmlbCBnBsjrWnKoG_iV07A39Bu49wA4vFhS0,7235
+openseries-1.1.1.dist-info/LICENSE.md,sha256=NJjeq3wyB7EnnHLmsdK1EK6zT00T1eB3FgAmHAPT_vM,1521
+openseries-1.1.1.dist-info/METADATA,sha256=wRNQc3e8ufp8EDHuFcdigKErnk2mRVMfa_LwbqfpjAk,47876
+openseries-1.1.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+openseries-1.1.1.dist-info/RECORD,,
```

