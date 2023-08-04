# Comparing `tmp/openseries-1.0.1-py3-none-any.whl.zip` & `tmp/openseries-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 53979 bytes, number of entries: 15
+Zip file size: 54059 bytes, number of entries: 15
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 openseries/__init__.py
 -rw-r--r--  2.0 unx     9970 b- defN 80-Jan-01 00:00 openseries/datefixer.py
--rw-r--r--  2.0 unx   115141 b- defN 80-Jan-01 00:00 openseries/frame.py
+-rw-r--r--  2.0 unx   115113 b- defN 80-Jan-01 00:00 openseries/frame.py
 -rw-r--r--  2.0 unx     1119 b- defN 80-Jan-01 00:00 openseries/load_plotly.py
 -rw-r--r--  2.0 unx      178 b- defN 80-Jan-01 00:00 openseries/plotly_captor_logo.json
 -rw-r--r--  2.0 unx     1429 b- defN 80-Jan-01 00:00 openseries/plotly_layouts.json
 -rw-r--r--  2.0 unx     4404 b- defN 80-Jan-01 00:00 openseries/risk.py
--rw-r--r--  2.0 unx    84385 b- defN 80-Jan-01 00:00 openseries/series.py
--rw-r--r--  2.0 unx    13878 b- defN 80-Jan-01 00:00 openseries/sim_price.py
+-rw-r--r--  2.0 unx    84308 b- defN 80-Jan-01 00:00 openseries/series.py
+-rw-r--r--  2.0 unx    13822 b- defN 80-Jan-01 00:00 openseries/sim_price.py
 -rw-r--r--  2.0 unx    14673 b- defN 80-Jan-01 00:00 openseries/stoch_processes.py
--rw-r--r--  2.0 unx     6698 b- defN 80-Jan-01 00:00 openseries/types.py
--rw-r--r--  2.0 unx     1521 b- defN 80-Jan-01 00:00 openseries-1.0.1.dist-info/LICENSE.md
--rw-r--r--  2.0 unx    47927 b- defN 80-Jan-01 00:00 openseries-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 openseries-1.0.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1200 b- defN 16-Jan-01 00:00 openseries-1.0.1.dist-info/RECORD
-15 files, 302611 bytes uncompressed, 52019 bytes compressed:  82.8%
+-rw-r--r--  2.0 unx     7082 b- defN 80-Jan-01 00:00 openseries/types.py
+-rw-r--r--  2.0 unx     1521 b- defN 80-Jan-01 00:00 openseries-1.1.0.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx    47925 b- defN 80-Jan-01 00:00 openseries-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 openseries-1.1.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1200 b- defN 16-Jan-01 00:00 openseries-1.1.0.dist-info/RECORD
+15 files, 302832 bytes uncompressed, 52099 bytes compressed:  82.8%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: openseries/stoch_processes.py
 Comment: 
 
 Filename: openseries/types.py
 Comment: 
 
-Filename: openseries-1.0.1.dist-info/LICENSE.md
+Filename: openseries-1.1.0.dist-info/LICENSE.md
 Comment: 
 
-Filename: openseries-1.0.1.dist-info/METADATA
+Filename: openseries-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: openseries-1.0.1.dist-info/WHEEL
+Filename: openseries-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: openseries-1.0.1.dist-info/RECORD
+Filename: openseries-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openseries/frame.py

```diff
@@ -25,15 +25,16 @@
     merge,
     MultiIndex,
     Series,
 )
 from pandas.tseries.offsets import CustomBusinessDay
 from plotly.graph_objs import Figure
 from plotly.offline import plot
-from pydantic import BaseModel, validator
+from pydantic import field_validator, ConfigDict, BaseModel
+
 from scipy.stats import kurtosis, norm, skew
 import statsmodels.api as sm
 
 # noinspection PyProtectedMember
 from statsmodels.regression.linear_model import RegressionResults
 
 from openseries.series import OpenTimeSeries, ValueType, ewma_calc
@@ -81,23 +82,19 @@
     -------
     OpenFrame
         Object of the class OpenFrame
     """
 
     constituents: List[OpenTimeSeries]
     tsdf: DataFrame = DataFrame()
-    weights: None | List[float]
-
-    class Config:
-        """Configurations for the OpenFrame class"""
+    weights: None | List[float] = None
 
-        arbitrary_types_allowed = True
-        validate_assignment = True
+    model_config = ConfigDict(arbitrary_types_allowed=True, validate_assignment=True)
 
-    @validator("constituents")
+    @field_validator("constituents")
     def check_labels_unique(
         cls, tseries: List[OpenTimeSeries]
     ) -> List[OpenTimeSeries]:
         """Pydantic validator ensuring that OpenFrame labels are unique"""
         labls = [x.label for x in tseries]
         if len(set(labls)) != len(labls):
             raise ValueError("TimeSeries names/labels must be unique")
```

## openseries/series.py

```diff
@@ -5,15 +5,15 @@
 import datetime as dt
 from enum import Enum
 from json import dump
 from math import ceil
 from os import path
 from pathlib import Path
 from re import compile as re_compile
-from typing import Any, cast, Dict, List, Tuple, TypeVar, Union
+from typing import Any, cast, Dict, List, Optional, Tuple, TypeVar, Union
 from numpy import (
     array,
     cumprod,
     dtype,
     insert,
     isnan,
     log,
@@ -31,26 +31,26 @@
     date_range,
     MultiIndex,
     Series,
 )
 from pandas.tseries.offsets import CustomBusinessDay
 from plotly.graph_objs import Figure
 from plotly.offline import plot
-from pydantic import BaseModel, constr, conlist, validator
+from pydantic import BaseModel, conlist, field_validator, model_validator
 from scipy.stats import kurtosis, norm, skew
 from stdnum import isin as isincode
 from stdnum.exceptions import InvalidChecksum
 
 from openseries.datefixer import date_offset_foll, date_fix, holiday_calendar
 from openseries.load_plotly import load_plotly_dict
 from openseries.types import (
-    COUNTRYPATTERN,
-    CURRENCYPATTERN,
-    DATABASEIDPATTERN,
-    DATEPATTERN,
+    CountryStringType,
+    CurrencyStringType,
+    DatabaseIdStringType,
+    DateListType,
     LiteralQuantileInterp,
     LiteralBizDayFreq,
     LiteralPandasResampleConvention,
     LiteralPandasReindexMethod,
     LiteralNanMethod,
     LiteralLinePlotMode,
     LiteralBarPlotMode,
@@ -126,109 +126,106 @@
     ROLLCVAR = "Rolling CVaR"
     ROLLINFORATIO = "Information Ratio"
     ROLLRTRN = "Rolling returns"
     ROLLVAR = "Rolling VaR"
     ROLLVOL = "Rolling volatility"
 
 
-# noinspection PyMethodParameters
-class OpenTimeSeries(BaseModel):
+class OpenTimeSeries(
+    BaseModel,
+    arbitrary_types_allowed=True,
+    validate_assignment=True,
+    revalidate_instances="always",
+    extra="allow",
+):
     """Object of the class OpenTimeSeries. Subclass of the Pydantic BaseModel
 
     Parameters
     ----------
     timeseriesId : str
         Database identifier of the timeseries
     instrumentId: str
         Database identifier of the instrument associated with the timeseries
-    currency : str
-        ISO 4217 currency code of the timeseries
-    dates : List[str]
-        Dates of the individual timeseries items
-        These dates will not be altered by methods
-    domestic : str
-        ISO 4217 currency code of the user's home currency
     name : str
         string identifier of the timeseries and/or instrument
-    isin : str
-        ISO 6166 identifier code of the associated instrument
-    label : str
-        Placeholder for a name of the timeseries
-    countries: list | str, default: "SE"
-        (List of) country code(s) according to ISO 3166-1 alpha-2
     valuetype : ValueType
         Identifies if the series is a series of values or returns
+    dates : List[str]
+        Dates of the individual timeseries items
+        These dates will not be altered by methods
     values : List[float]
         The value or return values of the timeseries items
         These values will not be altered by methods
     local_ccy: bool
         Boolean flag indicating if timeseries is in local currency
     tsdf: pandas.DataFrame
         Pandas object holding dates and values that can be altered via methods
+    currency : str
+        ISO 4217 currency code of the timeseries
+    domestic : str, default: "SEK"
+        ISO 4217 currency code of the user's home currency
+    countries: str, default: "SE"
+        (List of) country code(s) according to ISO 3166-1 alpha-2
+    isin : str, optional
+        ISO 6166 identifier code of the associated instrument
+    label : str, optional
+        Placeholder for a name of the timeseries
     """
 
-    timeseriesId: constr(regex=DATABASEIDPATTERN)
-    instrumentId: constr(regex=DATABASEIDPATTERN)
-    currency: constr(regex=CURRENCYPATTERN, to_upper=True, min_length=3, max_length=3)
-    dates: conlist(
-        item_type=constr(regex=DATEPATTERN),
-        min_items=1,
-        unique_items=True,
-    )
-    domestic: constr(
-        regex=CURRENCYPATTERN, to_upper=True, min_length=3, max_length=3
-    ) = "SEK"
+    timeseriesId: DatabaseIdStringType
+    instrumentId: DatabaseIdStringType
     name: str
-    isin: str | None = None
-    label: str | None = None
-    countries: conlist(
-        item_type=constr(
-            regex=COUNTRYPATTERN, to_upper=True, min_length=2, max_length=2
-        ),
-        min_items=1,
-        unique_items=True,
-    ) | constr(regex=COUNTRYPATTERN, to_upper=True, min_length=2, max_length=2) = "SE"
     valuetype: ValueType
-    values: conlist(item_type=float, min_items=1)
+    dates: DateListType
+    values: conlist(float, min_length=2)
     local_ccy: bool
     tsdf: DataFrame
+    currency: CurrencyStringType
+    domestic: CurrencyStringType = "SEK"
+    countries: CountryStringType = "SE"
+    isin: Optional[str] = None
+    label: Optional[str] = None
 
-    class Config:
-        """Configurations for the OpenTimeSeries class"""
-
-        arbitrary_types_allowed = True
-        validate_assignment = True
-
-    @validator("isin")
+    @field_validator("isin")
+    @classmethod
     def check_isincode(cls, isin_code: str) -> str:
         """Pydantic validator to ensure that the ISIN code is valid if provided"""
         if isin_code:
             try:
                 isincode.validate(isin_code)
             except InvalidChecksum as exc:
                 raise ValueError(
                     "The ISIN code's checksum or check digit is invalid."
                 ) from exc
         return isin_code
 
+    @model_validator(mode="after")
+    def check_dates_unique(self) -> "OpenTimeSeries":
+        """Pydantic validator to ensure that the dates are unique"""
+        dates_list_length = len(self.dates)
+        dates_set_length = len(set(self.dates))
+        if dates_list_length != dates_set_length:
+            raise ValueError("Dates are not unique")
+        return self
+
     @classmethod
     def setup_class(
         cls, domestic_ccy: str = "SEK", countries: List[str] | str = "SE"
     ) -> None:
         """Sets the domestic currency and calendar of the user.
 
         Parameters
         ----------
         domestic_ccy : str, default: "SEK"
             Currency code according to ISO 4217
         countries: List[str] | str, default: "SE"
             (List of) country code(s) according to ISO 3166-1 alpha-2
         """
-        ccy_pattern = re_compile(CURRENCYPATTERN)
-        ctry_pattern = re_compile(COUNTRYPATTERN)
+        ccy_pattern = re_compile(r"^[A-Z]{3}$")
+        ctry_pattern = re_compile(r"^[A-Z]{2}$")
         try:
             ccy_ok = ccy_pattern.match(domestic_ccy)
         except TypeError as exc:
             raise ValueError(
                 "domestic currency must be a code according to ISO 4217"
             ) from exc
         if not ccy_ok:
```

## openseries/sim_price.py

```diff
@@ -1,15 +1,15 @@
 """
 Defining the ReturnSimulation class which simulates returns based on
 stochastic processes generated using the stoch_process.py module.
 """
 from typing import cast
 from numpy import insert, random, sqrt
 from pandas import DataFrame
-from pydantic import BaseModel
+from pydantic import ConfigDict, BaseModel
 
 from openseries.stoch_processes import (
     ModelParameters,
     geometric_brownian_motion_log_returns,
     geometric_brownian_motion_jump_diffusion_levels,
     heston_model_levels,
 )
@@ -36,20 +36,15 @@
 
     number_of_sims: int
     trading_days: int
     trading_days_in_year: int
     mean_annual_return: float
     mean_annual_vol: float
     dframe: DataFrame
-
-    class Config:
-        """Configurations for the ReturnSimulation class"""
-
-        arbitrary_types_allowed = True
-        validate_assignment = True
+    model_config = ConfigDict(arbitrary_types_allowed=True, validate_assignment=True)
 
     @property
     def results(self: "ReturnSimulation") -> DataFrame:
         """
         Returns
         -------
         pandas.DataFrame
```

## openseries/types.py

```diff
@@ -1,17 +1,32 @@
 """
 Declaring types used throughout the project
 """
 from typing import Literal, List
-from pydantic import BaseModel
+from pydantic import BaseModel, conlist, constr
 
-COUNTRYPATTERN = r"^[A-Z]{2}$"
-CURRENCYPATTERN = r"^[A-Z]{3}$"
-DATEPATTERN = r"^\d{4}-(0[1-9]|1[0-2])-(0[1-9]|[12]\d|3[01])$"
-DATABASEIDPATTERN = r"^([0-9a-f]{24})?$"
+
+CountryStringType = conlist(
+    constr(
+        pattern=r"^[A-Z]{2}$", to_upper=True, min_length=2, max_length=2, strict=True
+    ),
+    min_length=1,
+) | constr(
+    pattern=r"^[A-Z]{2}$", to_upper=True, min_length=2, max_length=2, strict=True
+)
+
+CurrencyStringType = constr(
+    pattern=r"^[A-Z]{3}$", to_upper=True, min_length=3, max_length=3, strict=True
+)
+
+DateListType = conlist(
+    constr(pattern=r"^\d{4}-(0[1-9]|1[0-2])-(0[1-9]|[12]\d|3[01])$"), min_length=2
+)
+
+DatabaseIdStringType = constr(pattern=r"^([0-9a-f]{24})?$")
 
 LiteralLinePlotMode = Literal[
     "lines",
     "markers",
     "lines+markers",
     "lines+text",
     "markers+text",
```

## Comparing `openseries-1.0.1.dist-info/LICENSE.md` & `openseries-1.1.0.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `openseries-1.0.1.dist-info/METADATA` & `openseries-1.1.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openseries
-Version: 1.0.1
+Version: 1.1.0
 Summary: Package for simple financial time series analysis.
 Home-page: https://github.com/CaptorAB/OpenSeries
 License: BSD-3-Clause
 Keywords: python,python3,plotly,pandas,finance,fintech,data-science,timeseries,timeseries-data,timeseries-analysis,investment,investment-analysis,investing
 Author: Martin Karrin
 Author-email: martin.karrin@captor.se
 Requires-Python: >=3.10,<3.12
@@ -20,19 +20,19 @@
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Requires-Dist: ffn (>=0.3.7,<0.4.0)
 Requires-Dist: holidays (>=0.18,<0.19)
 Requires-Dist: numpy (>=1.25.1,<2.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: plotly (>=5.15.0,<6.0.0)
-Requires-Dist: pydantic (>=1.10.11,<2.0.0)
+Requires-Dist: pydantic (>=2.1.1,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-stdnum (>=1.18,<2.0)
 Requires-Dist: scipy (>=1.11.1,<2.0.0)
-Requires-Dist: statsmodels (>=0.13.5,<0.14.0)
+Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Project-URL: Repository, https://github.com/CaptorAB/OpenSeries
 Description-Content-Type: text/markdown
 
 <img src="https://sales.captor.se/captor_logo_sv_1600_icketransparent.png" alt="Captor
 Fund Management AB"
 width="81" height="100" align="left" float="right"/><br/>
```

## Comparing `openseries-1.0.1.dist-info/RECORD` & `openseries-1.1.0.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 openseries/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 openseries/datefixer.py,sha256=h4zshiUkJmRmbBgiCCVulxVUa2SO1dRdJMAKLMxE-tc,9970
-openseries/frame.py,sha256=p0xHGTEe6eUlakoxgAldwXjquTSfyvXMektdsYEgJnI,115141
+openseries/frame.py,sha256=nHRVfYRYPDIV32W6KCMEaJ7d9wG1qWMaeK_6JwfHnOM,115113
 openseries/load_plotly.py,sha256=DfpacL-aL5z-W0Cw7FL4YtDSbgeSI8Q-8DO6940wiJc,1119
 openseries/plotly_captor_logo.json,sha256=pGMuPVu4cEO3ZsCH1wU03hxqbIQkHFNoJUs1k1WK89Y,178
 openseries/plotly_layouts.json,sha256=xhrMOqW8LXb4QMtPiNBGdkPX518OHThiIJ68jpQk524,1429
 openseries/risk.py,sha256=_NJd8V-6pMx8pTodW-QpGKlmCDbCn4TsEjieKnCkIxU,4404
-openseries/series.py,sha256=Xw7ppt2bCVspkjYIqZKcMNfVIlrsmrnV7XWtp99qxrg,84385
-openseries/sim_price.py,sha256=dWzmj22nq4TW4BZBwP8Ajtid_g322No6D_m7t5bT8No,13878
+openseries/series.py,sha256=ytojrTbUtgi6Pmh4DbJd_SFIDP-A4xJE2BLaShStwqs,84308
+openseries/sim_price.py,sha256=2UQKJ9p2_0A10PbxadP5EhjeC9LRBP7IsoQdwQBKHNA,13822
 openseries/stoch_processes.py,sha256=6O4C_nC2iBseWggvDDC2gTpTqS5fI5nfjSRpccaazLE,14673
-openseries/types.py,sha256=t5xeqoD-e9fm0aU5I9chbzLcZ-MHmb9-jInCz3NrIfk,6698
-openseries-1.0.1.dist-info/LICENSE.md,sha256=NJjeq3wyB7EnnHLmsdK1EK6zT00T1eB3FgAmHAPT_vM,1521
-openseries-1.0.1.dist-info/METADATA,sha256=PTN4E6RKx3YEmLLohbkKawOJZJPsbrE4B-wjRUxiWwM,47927
-openseries-1.0.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-openseries-1.0.1.dist-info/RECORD,,
+openseries/types.py,sha256=wz-G8BrlB4NjxDpcJUwYO5PhEjfKI52uoO53k3VkJEQ,7082
+openseries-1.1.0.dist-info/LICENSE.md,sha256=NJjeq3wyB7EnnHLmsdK1EK6zT00T1eB3FgAmHAPT_vM,1521
+openseries-1.1.0.dist-info/METADATA,sha256=l7BJzQc--wMAzmYRy2mjo1Gq3bI8VaeZu9YAmJn-z3s,47925
+openseries-1.1.0.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+openseries-1.1.0.dist-info/RECORD,,
```

