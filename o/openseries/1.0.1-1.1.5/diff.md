# Comparing `tmp/openseries-1.0.1-py3-none-any.whl.zip` & `tmp/openseries-1.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,16 @@
-Zip file size: 53979 bytes, number of entries: 15
+Zip file size: 54748 bytes, number of entries: 14
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 openseries/__init__.py
--rw-r--r--  2.0 unx     9970 b- defN 80-Jan-01 00:00 openseries/datefixer.py
--rw-r--r--  2.0 unx   115141 b- defN 80-Jan-01 00:00 openseries/frame.py
--rw-r--r--  2.0 unx     1119 b- defN 80-Jan-01 00:00 openseries/load_plotly.py
+-rw-r--r--  2.0 unx    10168 b- defN 80-Jan-01 00:00 openseries/datefixer.py
+-rw-r--r--  2.0 unx   116260 b- defN 80-Jan-01 00:00 openseries/frame.py
+-rw-r--r--  2.0 unx     1180 b- defN 80-Jan-01 00:00 openseries/load_plotly.py
 -rw-r--r--  2.0 unx      178 b- defN 80-Jan-01 00:00 openseries/plotly_captor_logo.json
 -rw-r--r--  2.0 unx     1429 b- defN 80-Jan-01 00:00 openseries/plotly_layouts.json
--rw-r--r--  2.0 unx     4404 b- defN 80-Jan-01 00:00 openseries/risk.py
--rw-r--r--  2.0 unx    84385 b- defN 80-Jan-01 00:00 openseries/series.py
--rw-r--r--  2.0 unx    13878 b- defN 80-Jan-01 00:00 openseries/sim_price.py
--rw-r--r--  2.0 unx    14673 b- defN 80-Jan-01 00:00 openseries/stoch_processes.py
--rw-r--r--  2.0 unx     6698 b- defN 80-Jan-01 00:00 openseries/types.py
--rw-r--r--  2.0 unx     1521 b- defN 80-Jan-01 00:00 openseries-1.0.1.dist-info/LICENSE.md
--rw-r--r--  2.0 unx    47927 b- defN 80-Jan-01 00:00 openseries-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 openseries-1.0.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1200 b- defN 16-Jan-01 00:00 openseries-1.0.1.dist-info/RECORD
-15 files, 302611 bytes uncompressed, 52019 bytes compressed:  82.8%
+-rw-r--r--  2.0 unx     4456 b- defN 80-Jan-01 00:00 openseries/risk.py
+-rw-r--r--  2.0 unx    85198 b- defN 80-Jan-01 00:00 openseries/series.py
+-rw-r--r--  2.0 unx    37088 b- defN 80-Jan-01 00:00 openseries/simulation.py
+-rw-r--r--  2.0 unx     5767 b- defN 80-Jan-01 00:00 openseries/types.py
+-rw-r--r--  2.0 unx     1521 b- defN 80-Jan-01 00:00 openseries-1.1.5.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx    47610 b- defN 80-Jan-01 00:00 openseries-1.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 openseries-1.1.5.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1115 b- defN 16-Jan-01 00:00 openseries-1.1.5.dist-info/RECORD
+14 files, 312058 bytes uncompressed, 52920 bytes compressed:  83.0%
```

## zipnote {}

```diff
@@ -18,29 +18,26 @@
 
 Filename: openseries/risk.py
 Comment: 
 
 Filename: openseries/series.py
 Comment: 
 
-Filename: openseries/sim_price.py
-Comment: 
-
-Filename: openseries/stoch_processes.py
+Filename: openseries/simulation.py
 Comment: 
 
 Filename: openseries/types.py
 Comment: 
 
-Filename: openseries-1.0.1.dist-info/LICENSE.md
+Filename: openseries-1.1.5.dist-info/LICENSE.md
 Comment: 
 
-Filename: openseries-1.0.1.dist-info/METADATA
+Filename: openseries-1.1.5.dist-info/METADATA
 Comment: 
 
-Filename: openseries-1.0.1.dist-info/WHEEL
+Filename: openseries-1.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: openseries-1.0.1.dist-info/RECORD
+Filename: openseries-1.1.5.dist-info/RECORD
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
+from typing import Dict, List, Optional, Union
 from dateutil.relativedelta import relativedelta
 from holidays import country_holidays, list_supported_countries
 from numpy import array, busdaycalendar, datetime64, is_busday, where, timedelta64
 from pandas import date_range, Timestamp
 from pandas.tseries.offsets import CustomBusinessDay
 
+from openseries.types import CountriesType
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
@@ -53,15 +56,16 @@
         staging = country_holidays(country=countries, years=years)
         if custom_holidays is not None:
             staging.update(custom_holidays)
         hols = array(sorted(staging.keys()), dtype="datetime64[D]")
     elif isinstance(countries, list) and all(
         country in list_supported_countries() for country in countries
     ):
-        countryholidays: List[dt.date | str] = []
+        country: str
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
@@ -1,20 +1,21 @@
 """
 Defining the OpenFrame class
 """
+from __future__ import annotations
 from copy import deepcopy
 import datetime as dt
 from functools import reduce
 from logging import warning
 from math import ceil
 from os import path
 from pathlib import Path
 from random import choices
 from string import ascii_letters
-from typing import cast, Dict, List, Tuple, Union
+from typing import cast, Dict, List, Optional, Tuple, Type, TypeVar, Union
 from dateutil.relativedelta import relativedelta
 from ffn.core import calc_mean_var_weights, calc_inv_vol_weights, calc_erc_weights
 from numpy import cov, cumprod, log, sqrt
 from openpyxl import Workbook
 from openpyxl.utils.dataframe import dataframe_to_rows
 from pandas import (
     concat,
@@ -25,25 +26,26 @@
     merge,
     MultiIndex,
     Series,
 )
 from pandas.tseries.offsets import CustomBusinessDay
 from plotly.graph_objs import Figure
 from plotly.offline import plot
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, field_validator
 from scipy.stats import kurtosis, norm, skew
 import statsmodels.api as sm
 
 # noinspection PyProtectedMember
 from statsmodels.regression.linear_model import RegressionResults
 
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
@@ -61,56 +63,52 @@
 from openseries.risk import (
     drawdown_series,
     drawdown_details,
     cvar_down,
     var_down,
 )
 
+TypeOpenFrame = TypeVar("TypeOpenFrame", bound="OpenFrame")
 
-# noinspection PyMethodParameters
-class OpenFrame(BaseModel):
+
+class OpenFrame(BaseModel, arbitrary_types_allowed=True, validate_assignment=True):
     """Object of the class OpenFrame. Subclass of the Pydantic BaseModel
 
     Parameters
     ----------
-    constituents: List[OpenTimeSeries]
+    constituents: List[TypeOpenTimeSeries]
         List of objects of Class OpenTimeSeries
     weights: List[float], optional
         List of weights in float64 format.
 
     Returns
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
+    weights: Optional[List[float]] = None
 
-        arbitrary_types_allowed = True
-        validate_assignment = True
-
-    @validator("constituents")
+    @field_validator("constituents")
+    @classmethod
     def check_labels_unique(
-        cls, tseries: List[OpenTimeSeries]
+        cls: Type[TypeOpenFrame], tseries: List[OpenTimeSeries]
     ) -> List[OpenTimeSeries]:
         """Pydantic validator ensuring that OpenFrame labels are unique"""
         labls = [x.label for x in tseries]
         if len(set(labls)) != len(labls):
             raise ValueError("TimeSeries names/labels must be unique")
         return tseries
 
     def __init__(
-        self: "OpenFrame",
+        self: OpenFrame,
         constituents: List[OpenTimeSeries],
-        weights: List[float] | None = None,
+        weights: Optional[List[float]] = None,
     ) -> None:
         super().__init__(constituents=constituents, weights=weights)
 
         self.constituents = constituents
         self.tsdf = DataFrame(dtype="float64")
         self.weights = weights
 
@@ -118,30 +116,30 @@
             self.tsdf = reduce(
                 lambda left, right: concat([left, right], axis="columns", sort=True),
                 [x.tsdf for x in self.constituents],
             )
         else:
             warning("OpenFrame() was passed an empty list.")
 
-    def from_deepcopy(self: "OpenFrame") -> "OpenFrame":
+    def from_deepcopy(self: TypeOpenFrame) -> TypeOpenFrame:
         """Creates a copy of an OpenFrame object
 
         Returns
         -------
         OpenFrame
             An OpenFrame object
         """
 
         return deepcopy(self)
 
     def to_xlsx(
-        self: "OpenFrame",
+        self: TypeOpenFrame,
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
@@ -172,15 +170,17 @@
         for row in dataframe_to_rows(df=self.tsdf, index=True, header=True):
             wrksheet.append(row)
 
         wrkbook.save(sheetfile)
 
         return sheetfile
 
-    def merge_series(self: "OpenFrame", how: LiteralHowMerge = "outer") -> "OpenFrame":
+    def merge_series(
+        self: TypeOpenFrame, how: LiteralHowMerge = "outer"
+    ) -> TypeOpenFrame:
         """Merges the Pandas Dataframes of the constituent OpenTimeSeries
 
         Parameters
         ----------
         how: LiteralHowMerge, default: "outer"
             The Pandas merge method.
 
@@ -207,15 +207,15 @@
             )
         if how == "inner":
             for xerie in self.constituents:
                 xerie.tsdf = xerie.tsdf.loc[self.tsdf.index]
         return self
 
     def all_properties(
-        self: "OpenFrame", properties: List[LiteralFrameProps] | None = None
+        self: TypeOpenFrame, properties: Optional[List[LiteralFrameProps]] = None
     ) -> DataFrame:
         """Calculates the chosen timeseries properties
 
         Parameters
         ----------
         properties: List[LiteralFrameProps], optional
             The properties to calculate. Defaults to calculating all available.
@@ -232,18 +232,18 @@
             prop_list = [
                 getattr(self, x) for x in OpenFramePropertiesList.allowed_strings
             ]
         results = concat(prop_list, axis="columns").T
         return results
 
     def calc_range(
-        self: "OpenFrame",
-        months_offset: int | None = None,
-        from_dt: dt.date | None = None,
-        to_dt: dt.date | None = None,
+        self: TypeOpenFrame,
+        months_offset: Optional[int] = None,
+        from_dt: Optional[dt.date] = None,
+        to_dt: Optional[dt.date] = None,
     ) -> Tuple[dt.date, dt.date]:
         """Creates user defined date range
 
         Parameters
         ----------
         months_offset: int, optional
             Number of months offset as positive integer. Overrides use of from_date
@@ -291,16 +291,16 @@
                 earlier -= dt.timedelta(days=1)
             while later not in self.tsdf.index.tolist():
                 later += dt.timedelta(days=1)
 
         return earlier, later
 
     def align_index_to_local_cdays(
-        self: "OpenFrame", countries: List[str] | str = "SE"
-    ) -> "OpenFrame":
+        self: TypeOpenFrame, countries: CountriesType = "SE"
+    ) -> TypeOpenFrame:
         """Changes the index of the associated Pandas DataFrame .tsdf to align with
         local calendar business days
 
         Parameters
         ----------
         countries: List[str] | str, default: "SE"
             (List of) country code(s) according to ISO 3166-1 alpha-2
@@ -324,26 +324,26 @@
                 freq=CustomBusinessDay(calendar=calendar),
             )
         ]
         self.tsdf = self.tsdf.reindex(d_range, method=None, copy=False)
         return self
 
     @property
-    def length(self: "OpenFrame") -> int:
+    def length(self: TypeOpenFrame) -> int:
         """
         Returns
         -------
         int
             Number of observations
         """
 
         return len(self.tsdf.index)
 
     @property
-    def lengths_of_items(self: "OpenFrame") -> Series:
+    def lengths_of_items(self: TypeOpenFrame) -> Series:
         """
         Returns
         -------
         Pandas.Series
             Number of observations of all constituents
         """
 
@@ -351,144 +351,144 @@
             data=[self.tsdf.loc[:, d].count() for d in self.tsdf],
             index=self.tsdf.columns,
             name="observations",
             dtype=Int64Dtype(),
         )
 
     @property
-    def item_count(self: "OpenFrame") -> int:
+    def item_count(self: TypeOpenFrame) -> int:
         """
         Returns
         -------
         int
             Number of constituents
         """
 
         return len(self.constituents)
 
     @property
-    def columns_lvl_zero(self: "OpenFrame") -> List[str]:
+    def columns_lvl_zero(self: TypeOpenFrame) -> List[str]:
         """
         Returns
         -------
         List[str]
             Level 0 values of the Pandas.MultiIndex columns in the .tsdf
             Pandas.DataFrame
         """
 
         return list(self.tsdf.columns.get_level_values(0))
 
     @property
-    def columns_lvl_one(self: "OpenFrame") -> List[str]:
+    def columns_lvl_one(self: TypeOpenFrame) -> List[str]:
         """
         Returns
         -------
         List[str]
             Level 1 values of the Pandas.MultiIndex columns in the .tsdf
             Pandas.DataFrame
         """
 
         return list(self.tsdf.columns.get_level_values(1))
 
     @property
-    def first_idx(self: "OpenFrame") -> dt.date:
+    def first_idx(self: TypeOpenFrame) -> dt.date:
         """
         Returns
         -------
         datetime.date
             The first date in the index of the .tsdf Pandas.DataFrame
         """
         return cast(dt.date, self.tsdf.index[0])
 
     @property
-    def first_indices(self: "OpenFrame") -> Series:
+    def first_indices(self: TypeOpenFrame) -> Series:
         """
         Returns
         -------
         Pandas.Series
             The first dates in the timeseries of all constituents
         """
 
         return Series(
             data=[i.first_idx for i in self.constituents],
             index=self.tsdf.columns,
             name="first indices",
         )
 
     @property
-    def last_idx(self: "OpenFrame") -> dt.date:
+    def last_idx(self: TypeOpenFrame) -> dt.date:
         """
         Returns
         -------
         datetime.date
             The last date in the index of the .tsdf Pandas.DataFrame
         """
         return cast(dt.date, self.tsdf.index[-1])
 
     @property
-    def last_indices(self: "OpenFrame") -> Series:
+    def last_indices(self: TypeOpenFrame) -> Series:
         """
         Returns
         -------
         Pandas.Series
             The last dates in the timeseries of all constituents
         """
 
         return Series(
             data=[i.last_idx for i in self.constituents],
             index=self.tsdf.columns,
             name="last indices",
         )
 
     @property
-    def span_of_days(self: "OpenFrame") -> int:
+    def span_of_days(self: TypeOpenFrame) -> int:
         """
         Returns
         -------
         int
             Number of days from the first date to the last
             in the index of the .tsdf Pandas.DataFrame
         """
 
         return (self.last_idx - self.first_idx).days
 
     @property
-    def span_of_days_all(self: "OpenFrame") -> Series:
+    def span_of_days_all(self: TypeOpenFrame) -> Series:
         """
         Number of days from the first date to the last for all items in the frame.
         """
         return Series(
             data=[c.span_of_days for c in self.constituents],
             index=self.tsdf.columns,
             name="span of days",
             dtype=Int64Dtype(),
         )
 
     @property
-    def yearfrac(self: "OpenFrame") -> float:
+    def yearfrac(self: TypeOpenFrame) -> float:
         """
         Returns
         -------
         float
             Length of the index of the .tsdf Pandas.DataFrame expressed in years
             assuming all years have 365.25 days
         """
 
         return self.span_of_days / 365.25
 
     @property
-    def periods_in_a_year(self: "OpenFrame") -> float:
+    def periods_in_a_year(self: TypeOpenFrame) -> float:
         """
         The number of businessdays in an average year for all days in the data.
         Be aware that this is not the same for all constituents.
         """
         return self.length / self.yearfrac
 
     @property
-    def geo_ret(self: "OpenFrame") -> Series:
+    def geo_ret(self: TypeOpenFrame) -> Series:
         """https://www.investopedia.com/terms/c/cagr.asp
 
         Returns
         -------
         Pandas.Series
             Compounded Annual Growth Rate (CAGR)
         """
@@ -500,18 +500,18 @@
         return Series(
             data=(self.tsdf.iloc[-1] / self.tsdf.iloc[0]) ** (1 / self.yearfrac) - 1,
             name="Geometric return",
             dtype="float64",
         )
 
     def geo_ret_func(
-        self: "OpenFrame",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        self: TypeOpenFrame,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> Series:
         """https://www.investopedia.com/terms/c/cagr.asp
 
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
@@ -543,15 +543,15 @@
         return Series(
             data=(self.tsdf.loc[later] / self.tsdf.loc[earlier]) ** (1 / fraction) - 1,
             name="Subset Geometric return",
             dtype="float64",
         )
 
     @property
-    def arithmetic_ret(self: "OpenFrame") -> Series:
+    def arithmetic_ret(self: TypeOpenFrame) -> Series:
         """https://www.investopedia.com/terms/a/arithmeticmean.asp
 
         Returns
         -------
         Pandas.Series
             Annualized arithmetic mean of returns
         """
@@ -559,19 +559,19 @@
         return Series(
             data=self.tsdf.pct_change().mean() * self.periods_in_a_year,
             name="Arithmetic return",
             dtype="float64",
         )
 
     def arithmetic_ret_func(
-        self: "OpenFrame",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
-        periods_in_a_year_fixed: int | None = None,
+        self: TypeOpenFrame,
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
@@ -604,15 +604,15 @@
             .mean()
             * time_factor,
             name="Subset Arithmetic return",
             dtype="float64",
         )
 
     @property
-    def value_ret(self: "OpenFrame") -> Series:
+    def value_ret(self: TypeOpenFrame) -> Series:
         """
         Returns
         -------
         Pandas.Series
             Simple return
         """
 
@@ -624,18 +624,18 @@
         return Series(
             data=self.tsdf.iloc[-1] / self.tsdf.iloc[0] - 1,
             name="Total return",
             dtype="float64",
         )
 
     def value_ret_func(
-        self: "OpenFrame",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        self: TypeOpenFrame,
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
@@ -659,15 +659,15 @@
         return Series(
             data=self.tsdf.loc[later] / self.tsdf.loc[earlier] - 1,
             name="Subset Total return",
             dtype="float64",
         )
 
     def value_ret_calendar_period(
-        self: "OpenFrame", year: int, month: int | None = None
+        self: TypeOpenFrame, year: int, month: Optional[int] = None
     ) -> Series:
         """
         Parameters
         ----------
         year : int
             Calendar year of the period to calculate.
         month : int, optional
@@ -689,15 +689,15 @@
         rtn = rtn.loc[period] + 1
         rtn = rtn.apply(cumprod, axis="index").iloc[-1] - 1
         rtn.name = period
         rtn = rtn.astype("float64")
         return rtn
 
     @property
-    def vol(self: "OpenFrame") -> Series:
+    def vol(self: TypeOpenFrame) -> Series:
         """Based on Pandas .std() which is the equivalent of stdev.s([...])
         in MS Excel \n
         https://www.investopedia.com/terms/v/volatility.asp
 
         Returns
         -------
         Pandas.Series
@@ -707,19 +707,19 @@
         return Series(
             data=self.tsdf.pct_change().std() * sqrt(self.periods_in_a_year),
             name="Volatility",
             dtype="float64",
         )
 
     def vol_func(
-        self: "OpenFrame",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
-        periods_in_a_year_fixed: int | None = None,
+        self: TypeOpenFrame,
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
@@ -754,15 +754,15 @@
             .std()
             * sqrt(time_factor),
             name="Subset Volatility",
             dtype="float64",
         )
 
     @property
-    def downside_deviation(self: "OpenFrame") -> Series:
+    def downside_deviation(self: TypeOpenFrame) -> Series:
         """The standard deviation of returns that are below a Minimum Accepted
         Return of zero.
         It is used to calculate the Sortino Ratio \n
         https://www.investopedia.com/terms/d/downside-deviation.asp
 
         Returns
         -------
@@ -776,20 +776,20 @@
             data=sqrt((dddf[dddf < 0.0] ** 2).sum() / self.length)
             * sqrt(self.periods_in_a_year),
             name="Downside deviation",
             dtype="float64",
         )
 
     def downside_deviation_func(
-        self: "OpenFrame",
+        self: TypeOpenFrame,
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
@@ -834,48 +834,48 @@
         return Series(
             data=sqrt((dddf[dddf < 0.0] ** 2).sum() / how_many) * sqrt(time_factor),
             name="Subset Downside deviation",
             dtype="float64",
         )
 
     @property
-    def ret_vol_ratio(self: "OpenFrame") -> Series:
+    def ret_vol_ratio(self: TypeOpenFrame) -> Series:
         """
         Returns
         -------
         Pandas.Series
             Ratio of the annualized arithmetic mean of returns and annualized
             volatility.
         """
 
         ratio = self.arithmetic_ret / self.vol
         ratio.name = "Return vol ratio"
         ratio = ratio.astype("float64")
         return ratio
 
     def ret_vol_ratio_func(
-        self: "OpenFrame",
-        riskfree_rate: float | None = None,
-        riskfree_column: Tuple[str, ValueType] | int = -1,
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
-        periods_in_a_year_fixed: int | None = None,
+        self: TypeOpenFrame,
+        riskfree_rate: Optional[float] = None,
+        riskfree_column: Union[Tuple[str, ValueType], int] = -1,
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
 
         Parameters
         ----------
         riskfree_rate : float, optional
             The return of the zero volatility asset used to calculate Sharpe ratio
-        riskfree_column : Tuple[str, ValueType] | int, default: -1
+        riskfree_column : Union[Tuple[str, ValueType], int], default: -1
             The return of the zero volatility asset used to calculate Sharpe ratio
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
             and to_date
         from_date : datetime.date, optional
             Specific from date
         to_date : datetime.date, optional
@@ -950,31 +950,31 @@
             data=ratios,
             index=self.tsdf.columns,
             name=f"Sharpe Ratios (rf={riskfree_rate:.2%})",
             dtype="float64",
         )
 
     def jensen_alpha(
-        self: "OpenFrame",
-        asset: Tuple[str, ValueType] | int,
-        market: Tuple[str, ValueType] | int,
+        self: TypeOpenFrame,
+        asset: Union[Tuple[str, ValueType], int],
+        market: Union[Tuple[str, ValueType], int],
         riskfree_rate: float = 0.0,
     ) -> float:
         """The Jensen's measure, or Jensen's alpha, is a risk-adjusted performance
         measure that represents the average return on a portfolio or investment,
         above or below that predicted by the capital asset pricing model (CAPM),
         given the portfolio's or investment's beta and the average market return.
         This metric is also commonly referred to as simply alpha.
         https://www.investopedia.com/terms/j/jensensmeasure.asp
 
         Parameters
         ----------
-        asset: Tuple[str, ValueType] | int
+        asset: Union[Tuple[str, ValueType], int]
             The column of the asset
-        market: Tuple[str, ValueType] | int
+        market: Union[Tuple[str, ValueType], int]
             The column of the market against which Jensen's alpha is measured
         riskfree_rate : float, default: 0.0
             The return of the zero volatility riskfree asset
 
         Returns
         -------
         float
@@ -1065,15 +1065,15 @@
 
         covariance = cov(asset_log, market_log, ddof=1)
         beta = covariance[0, 1] / covariance[1, 1]
 
         return float(asset_cagr - riskfree_rate - beta * (market_cagr - riskfree_rate))
 
     @property
-    def sortino_ratio(self: "OpenFrame") -> Series:
+    def sortino_ratio(self: TypeOpenFrame) -> Series:
         """https://www.investopedia.com/terms/s/sortinoratio.asp
 
         Returns
         -------
         Pandas.Series
             Sortino ratio calculated as the annualized arithmetic mean of returns
             / downside deviation. The ratio implies that the riskfree asset has zero
@@ -1082,33 +1082,33 @@
 
         sortino = self.arithmetic_ret / self.downside_deviation
         sortino.name = "Sortino ratio"
         sortino = sortino.astype("float64")
         return sortino
 
     def sortino_ratio_func(
-        self: "OpenFrame",
-        riskfree_rate: float | None = None,
-        riskfree_column: Tuple[str, ValueType] | int = -1,
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
-        periods_in_a_year_fixed: int | None = None,
+        self: TypeOpenFrame,
+        riskfree_rate: Optional[float] = None,
+        riskfree_column: Union[Tuple[str, ValueType], int] = -1,
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
 
         Parameters
         ----------
         riskfree_rate : float, optional
             The return of the zero volatility asset
-        riskfree_column : Tuple[str, ValueType] | int, default: -1
+        riskfree_column : Union[Tuple[str, ValueType], int], default: -1
             The return of the zero volatility asset used to calculate Sharpe ratio
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
             and to_date
         from_date : datetime.date, optional
             Specific from date
         to_date : datetime.date, optional
@@ -1190,15 +1190,15 @@
             data=ratios,
             index=self.tsdf.columns,
             name=f"Sortino Ratios (rf={riskfree_rate:.2%},mar=0.0%)",
             dtype="float64",
         )
 
     @property
-    def z_score(self: "OpenFrame") -> Series:
+    def z_score(self: TypeOpenFrame) -> Series:
         """https://www.investopedia.com/terms/z/zscore.asp
 
         Returns
         -------
         float
             Z-score as (last return - mean return) / standard deviation of returns.
         """
@@ -1207,18 +1207,18 @@
         return Series(
             data=(zscframe.iloc[-1] - zscframe.mean()) / zscframe.std(),
             name="Z-score",
             dtype="float64",
         )
 
     def z_score_func(
-        self: "OpenFrame",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        self: TypeOpenFrame,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> Series:
         """https://www.investopedia.com/terms/z/zscore.asp
 
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
@@ -1239,15 +1239,15 @@
         return Series(
             data=(zscframe.iloc[-1] - zscframe.mean()) / zscframe.std(),
             name="Subset Z-score",
             dtype="float64",
         )
 
     @property
-    def max_drawdown(self: "OpenFrame") -> Series:
+    def max_drawdown(self: TypeOpenFrame) -> Series:
         """https://www.investopedia.com/terms/m/maximum-drawdown-mdd.asp
 
         Returns
         -------
         Pandas.Series
             Maximum drawdown without any limit on date range
         """
@@ -1255,15 +1255,15 @@
         return Series(
             data=(self.tsdf / self.tsdf.expanding(min_periods=1).max()).min() - 1,
             name="Max drawdown",
             dtype="float64",
         )
 
     @property
-    def max_drawdown_date(self: "OpenFrame") -> Series:
+    def max_drawdown_date(self: TypeOpenFrame) -> Series:
         """https://www.investopedia.com/terms/m/maximum-drawdown-mdd.asp
 
         Returns
         -------
         Pandas.Series
             Date when the maximum drawdown occurred
         """
@@ -1272,52 +1272,55 @@
         return Series(
             data=md_dates,
             index=self.tsdf.columns,
             name="Max drawdown dates",
         )
 
     def max_drawdown_func(
-        self: "OpenFrame",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        self: TypeOpenFrame,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
+        min_periods: int = 1,
     ) -> Series:
         """https://www.investopedia.com/terms/m/maximum-drawdown-mdd.asp
 
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
             and to_date
         from_date : datetime.date, optional
             Specific from date
         to_date : datetime.date, optional
             Specific to date
+        min_periods: int, default: 1
+            Smallest number of observations to use to find the maximum drawdown
 
         Returns
         -------
         Pandas.Series
             Maximum drawdown without any limit on date range
         """
 
         earlier, later = self.calc_range(months_from_last, from_date, to_date)
         return Series(
             data=(
                 self.tsdf.loc[cast(int, earlier) : cast(int, later)]
                 / self.tsdf.loc[cast(int, earlier) : cast(int, later)]
-                .expanding(min_periods=1)
+                .expanding(min_periods=min_periods)
                 .max()
             ).min()
             - 1,
             name="Subset Max drawdown",
             dtype="float64",
         )
 
     @property
-    def max_drawdown_cal_year(self: "OpenFrame") -> Series:
+    def max_drawdown_cal_year(self: TypeOpenFrame) -> Series:
         """https://www.investopedia.com/terms/m/maximum-drawdown-mdd.asp
 
         Returns
         -------
         Pandas.Series
             Maximum drawdown in a single calendar year.
         """
@@ -1331,26 +1334,26 @@
             .min()
         )
         mxdwn.name = "Max drawdown in cal yr"
         mxdwn = mxdwn.astype("float64")
         return mxdwn
 
     @property
-    def worst(self: "OpenFrame") -> Series:
+    def worst(self: TypeOpenFrame) -> Series:
         """
         Returns
         -------
         Pandas.Series
             Most negative percentage change
         """
 
         return Series(data=self.tsdf.pct_change().min(), name="Worst", dtype="float64")
 
     @property
-    def worst_month(self: "OpenFrame") -> Series:
+    def worst_month(self: TypeOpenFrame) -> Series:
         """
         Returns
         -------
         Pandas.Series
             Most negative month
         """
 
@@ -1359,19 +1362,19 @@
         return Series(
             data=wdf.resample("BM").last().pct_change().min(),
             name="Worst month",
             dtype="float64",
         )
 
     def worst_func(
-        self: "OpenFrame",
+        self: TypeOpenFrame,
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
@@ -1396,33 +1399,33 @@
             .sum()
             .min(),
             name=f"Subset Worst {observations}day period",
             dtype="float64",
         )
 
     @property
-    def positive_share(self: "OpenFrame") -> Series:
+    def positive_share(self: TypeOpenFrame) -> Series:
         """
         Returns
         -------
         Pandas.Series
             The share of percentage changes that are greater than zero
         """
         pos = self.tsdf.pct_change()[1:][self.tsdf.pct_change()[1:] > 0.0].count()
         tot = self.tsdf.pct_change()[1:].count()
         answer = pos / tot
         answer.name = "Positive share"
         answer = answer.astype("float64")
         return answer
 
     def positive_share_func(
-        self: "OpenFrame",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        self: TypeOpenFrame,
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
@@ -1453,15 +1456,15 @@
         )
         answer = pos / tot
         answer.name = "Positive share"
         answer = answer.astype("float64")
         return answer
 
     @property
-    def skew(self: "OpenFrame") -> Series:
+    def skew(self: TypeOpenFrame) -> Series:
         """https://www.investopedia.com/terms/s/skewness.asp
 
         Returns
         -------
         Pandas.Series
             Skew of the return distribution
         """
@@ -1470,18 +1473,18 @@
             data=skew(self.tsdf.pct_change().values, bias=True, nan_policy="omit"),
             index=self.tsdf.columns,
             name="Skew",
             dtype="float64",
         )
 
     def skew_func(
-        self: "OpenFrame",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        self: TypeOpenFrame,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> Series:
         """https://www.investopedia.com/terms/s/skewness.asp
 
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
@@ -1509,15 +1512,15 @@
             ),
             index=self.tsdf.columns,
             name="Subset Skew",
             dtype="float64",
         )
 
     @property
-    def kurtosis(self: "OpenFrame") -> Series:
+    def kurtosis(self: TypeOpenFrame) -> Series:
         """https://www.investopedia.com/terms/k/kurtosis.asp
 
         Returns
         -------
         Pandas.Series
             Kurtosis of the return distribution
         """
@@ -1528,18 +1531,18 @@
             ),
             index=self.tsdf.columns,
             name="Kurtosis",
             dtype="float64",
         )
 
     def kurtosis_func(
-        self: "OpenFrame",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        self: TypeOpenFrame,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> Series:
         """https://www.investopedia.com/terms/k/kurtosis.asp
 
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
@@ -1566,15 +1569,15 @@
             ),
             index=self.tsdf.columns,
             name="Subset Kurtosis",
             dtype="float64",
         )
 
     @property
-    def cvar_down(self: "OpenFrame") -> Series:
+    def cvar_down(self: TypeOpenFrame) -> Series:
         """https://www.investopedia.com/terms/c/conditional_value_at_risk.asp
 
         Returns
         -------
         Pandas.Series
             Downside 95% Conditional Value At Risk "CVaR"
         """
@@ -1592,19 +1595,19 @@
             data=var_list,
             index=self.tsdf.columns,
             name=f"CVaR {level:.1%}",
             dtype="float64",
         )
 
     def cvar_down_func(
-        self: "OpenFrame",
+        self: TypeOpenFrame,
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
@@ -1636,15 +1639,15 @@
             data=var_list,
             index=self.tsdf.columns,
             name=f"CVaR {level:.1%}",
             dtype="float64",
         )
 
     @property
-    def var_down(self: "OpenFrame") -> Series:
+    def var_down(self: TypeOpenFrame) -> Series:
         """Downside 95% Value At Risk, "VaR". The equivalent of
         percentile.inc([...], 1-level) over returns in MS Excel \n
         https://www.investopedia.com/terms/v/var.asp
 
         Returns
         -------
         Pandas.Series
@@ -1657,19 +1660,19 @@
                 1 - level, interpolation=interpolation
             ),
             name=f"VaR {level:.1%}",
             dtype="float64",
         )
 
     def var_down_func(
-        self: "OpenFrame",
+        self: TypeOpenFrame,
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
@@ -1699,15 +1702,15 @@
             .pct_change()
             .quantile(1 - level, interpolation=interpolation),
             name=f"VaR {level:.1%}",
             dtype="float64",
         )
 
     @property
-    def vol_from_var(self: "OpenFrame") -> Series:
+    def vol_from_var(self: TypeOpenFrame) -> Series:
         """
         Returns
         -------
         Pandas.Series
             Implied annualized volatility from the Downside 95% VaR using the
             assumption that returns are normally distributed.
         """
@@ -1719,22 +1722,22 @@
             / norm.ppf(level)
         )
         return Series(
             data=imp_vol, name=f"Imp vol from VaR {level:.0%}", dtype="float64"
         )
 
     def vol_from_var_func(
-        self: "OpenFrame",
+        self: TypeOpenFrame,
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
@@ -1790,25 +1793,25 @@
                 / norm.ppf(level)
             )
         return Series(
             data=imp_vol, name=f"Subset Imp vol from VaR {level:.0%}", dtype="float64"
         )
 
     def target_weight_from_var(
-        self: "OpenFrame",
+        self: TypeOpenFrame,
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
@@ -1853,30 +1856,30 @@
         vfv = vfv.apply(
             lambda x: max(min_leverage_local, min(target_vol / x, max_leverage_local))
         )
         return Series(
             data=vfv, name=f"Weight from target vol {target_vol:.1%}", dtype="float64"
         )
 
-    def value_to_ret(self: "OpenFrame") -> "OpenFrame":
+    def value_to_ret(self: TypeOpenFrame) -> TypeOpenFrame:
         """
         Returns
         -------
         OpenFrame
             The returns of the values in the series
         """
 
         self.tsdf = self.tsdf.pct_change()
         self.tsdf.iloc[0] = 0
         new_labels = [ValueType.RTRN] * self.item_count
         arrays = [self.tsdf.columns.get_level_values(0), new_labels]
         self.tsdf.columns = MultiIndex.from_arrays(arrays)
         return self
 
-    def value_to_diff(self: "OpenFrame", periods: int = 1) -> "OpenFrame":
+    def value_to_diff(self: TypeOpenFrame, periods: int = 1) -> TypeOpenFrame:
         """Converts valueseries to series of their period differences
 
         Parameters
         ----------
         periods: int, default: 1
             The number of periods between observations over which difference
             is calculated
@@ -1890,28 +1893,28 @@
         self.tsdf = self.tsdf.diff(periods=periods)
         self.tsdf.iloc[0] = 0
         new_labels = [ValueType.RTRN] * self.item_count
         arrays = [self.tsdf.columns.get_level_values(0), new_labels]
         self.tsdf.columns = MultiIndex.from_arrays(arrays)
         return self
 
-    def value_to_log(self: "OpenFrame") -> "OpenFrame":
+    def value_to_log(self: TypeOpenFrame) -> TypeOpenFrame:
         """Converts a valueseries into logarithmic return series \n
         Equivalent to LN(value[t] / value[t=0]) in MS Excel
 
         Returns
         -------
         OpenFrame
             An OpenFrame object
         """
 
         self.tsdf = log(self.tsdf / self.tsdf.iloc[0])
         return self
 
-    def to_cumret(self: "OpenFrame") -> "OpenFrame":
+    def to_cumret(self: TypeOpenFrame) -> TypeOpenFrame:
         """Converts returnseries into cumulative valueseries
 
         Returns
         -------
         OpenFrame
             An OpenFrame object
         """
@@ -1924,16 +1927,16 @@
         self.tsdf = self.tsdf.apply(cumprod, axis="index") / self.tsdf.iloc[0]
         new_labels = [ValueType.PRICE] * self.item_count
         arrays = [self.tsdf.columns.get_level_values(0), new_labels]
         self.tsdf.columns = MultiIndex.from_arrays(arrays)
         return self
 
     def resample(
-        self: "OpenFrame", freq: Union[LiteralBizDayFreq, str] = "BM"
-    ) -> "OpenFrame":
+        self: TypeOpenFrame, freq: Union[LiteralBizDayFreq, str] = "BM"
+    ) -> TypeOpenFrame:
         """Resamples the timeseries frequency
 
         Parameters
         ----------
         freq: Union[LiteralBizDayFreq, str], default "BM"
             The date offset string that sets the resampled frequency
             Examples are "7D", "B", "M", "BM", "Q", "BQ", "A", "BA"
@@ -1953,20 +1956,20 @@
             xerie.tsdf.index = [
                 dejt.date() for dejt in DatetimeIndex(xerie.tsdf.index)
             ]
 
         return self
 
     def resample_to_business_period_ends(
-        self: "OpenFrame",
+        self: TypeOpenFrame,
         freq: LiteralBizDayFreq = "BM",
-        countries: List[str] | str = "SE",
+        countries: CountriesType = "SE",
         convention: LiteralPandasResampleConvention = "end",
         method: LiteralPandasReindexMethod = "nearest",
-    ) -> "OpenFrame":
+    ) -> TypeOpenFrame:
         """Resamples timeseries frequency to the business calendar
         month end dates of each period while leaving any stubs
         in place. Stubs will be aligned to the shortest stub
 
         Parameters
         ----------
         freq: LiteralBizDayFreq, default BM
@@ -2022,56 +2025,62 @@
         self.tsdf = self.tsdf.reindex([d.date() for d in dates], method=method)
         for xerie in self.constituents:
             xerie.tsdf = xerie.tsdf.reindex(
                 [dejt.date() for dejt in dates], method=method
             )
         return self
 
-    def to_drawdown_series(self: "OpenFrame") -> "OpenFrame":
+    def to_drawdown_series(self: TypeOpenFrame) -> TypeOpenFrame:
         """Converts the timeseries into a drawdown series
 
         Returns
         -------
         OpenFrame
             An OpenFrame object
         """
 
         for serie in self.tsdf:
             self.tsdf.loc[:, serie] = drawdown_series(self.tsdf.loc[:, serie])
         return self
 
-    def drawdown_details(self: "OpenFrame") -> DataFrame:
-        """
+    def drawdown_details(self: TypeOpenFrame, min_periods: int = 1) -> DataFrame:
+        """Calculates 'Max Drawdown', 'Start of drawdown', 'Date of bottom',
+        'Days from start to bottom', & 'Average fall per day'
+
+        Parameters
+        ----------
+        min_periods: int, default: 1
+            Smallest number of observations to use to find the maximum drawdown
+
         Returns
         -------
         Pandas.DataFrame
-            Calculates 'Max Drawdown', 'Start of drawdown', 'Date of bottom',
-            'Days from start to bottom', & 'Average fall per day'
+            Drawdown details
         """
 
         mxdwndf = DataFrame()
         for i in self.constituents:
             tmpdf = i.tsdf.copy()
             tmpdf.index = DatetimeIndex(tmpdf.index)
-            ddown = drawdown_details(tmpdf)
+            ddown = drawdown_details(prices=tmpdf, min_periods=min_periods)
             ddown.name = i.label
             mxdwndf = concat([mxdwndf, ddown], axis="columns")
         return mxdwndf
 
     def ewma_risk(
-        self: "OpenFrame",
+        self: TypeOpenFrame,
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
@@ -2179,18 +2188,18 @@
         return DataFrame(
             index=cols + [corr_label],
             columns=data.index,
             data=[raw_one, raw_two, raw_corr],
         ).T
 
     def rolling_vol(
-        self: "OpenFrame",
+        self: TypeOpenFrame,
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
@@ -2216,15 +2225,15 @@
         )
         voldf = voldf.dropna().to_frame()
         voldf.columns = [[vol_label], ["Rolling volatility"]]
 
         return voldf
 
     def rolling_return(
-        self: "OpenFrame", column: int, observations: int = 21
+        self: TypeOpenFrame, column: int, observations: int = 21
     ) -> DataFrame:
         """
         Parameters
         ----------
         column: int
             Position as integer of column to calculate
         observations: int, default: 21
@@ -2245,15 +2254,15 @@
         )
         retdf = retdf.dropna().to_frame()
         retdf.columns = [[ret_label], ["Rolling returns"]]
 
         return retdf
 
     def rolling_cvar_down(
-        self: "OpenFrame", column: int, level: float = 0.95, observations: int = 252
+        self: TypeOpenFrame, column: int, level: float = 0.95, observations: int = 252
     ) -> DataFrame:
         """
         Parameters
         ----------
         column: int
             Position as integer of column to calculate
         level: float, default: 0.95
@@ -2275,15 +2284,15 @@
         )
         cvardf = cvardf.dropna().to_frame()
         cvardf.columns = [[cvar_label], ["Rolling CVaR"]]
 
         return cvardf
 
     def rolling_var_down(
-        self: "OpenFrame",
+        self: TypeOpenFrame,
         column: int,
         level: float = 0.95,
         interpolation: LiteralQuantileInterp = "lower",
         observations: int = 252,
     ) -> DataFrame:
         """
         Parameters
@@ -2311,16 +2320,16 @@
         )
         vardf = vardf.dropna().to_frame()
         vardf.columns = [[var_label], ["Rolling VaR"]]
 
         return vardf
 
     def value_nan_handle(
-        self: "OpenFrame", method: LiteralNanMethod = "fill"
-    ) -> "OpenFrame":
+        self: TypeOpenFrame, method: LiteralNanMethod = "fill"
+    ) -> TypeOpenFrame:
         """Handling of missing values in a valueseries
 
         Parameters
         ----------
         method: LiteralNanMethod, default: "fill"
             Method used to handle NaN. Either fill with last known or drop
 
@@ -2337,16 +2346,16 @@
         if method == "fill":
             self.tsdf.fillna(method="pad", inplace=True)
         else:
             self.tsdf.dropna(inplace=True)
         return self
 
     def return_nan_handle(
-        self: "OpenFrame", method: LiteralNanMethod = "fill"
-    ) -> "OpenFrame":
+        self: TypeOpenFrame, method: LiteralNanMethod = "fill"
+    ) -> TypeOpenFrame:
         """Handling of missing values in a returnseries
 
         Parameters
         ----------
         method: LiteralNanMethod, default: "fill"
             Method used to handle NaN. Either fill with zero or drop
 
@@ -2363,28 +2372,30 @@
         if method == "fill":
             self.tsdf.fillna(value=0.0, inplace=True)
         else:
             self.tsdf.dropna(inplace=True)
         return self
 
     @property
-    def correl_matrix(self: "OpenFrame") -> DataFrame:
+    def correl_matrix(self: TypeOpenFrame) -> DataFrame:
         """
         Returns
         -------
         Pandas.DataFrame
             Correlation matrix
         """
         corr_matrix = self.tsdf.pct_change().corr(method="pearson", min_periods=1)
         corr_matrix.columns = corr_matrix.columns.droplevel(level=1)
         corr_matrix.index = corr_matrix.index.droplevel(level=1)
         corr_matrix.index.name = "Correlation"
         return corr_matrix
 
-    def add_timeseries(self: "OpenFrame", new_series: OpenTimeSeries) -> "OpenFrame":
+    def add_timeseries(
+        self: TypeOpenFrame, new_series: OpenTimeSeries
+    ) -> TypeOpenFrame:
         """
         Parameters
         ----------
         new_series: OpenTimeSeries
             The timeseries to add
 
         Returns
@@ -2392,15 +2403,15 @@
         OpenFrame
             An OpenFrame object
         """
         self.constituents += [new_series]
         self.tsdf = concat([self.tsdf, new_series.tsdf], axis="columns", sort=True)
         return self
 
-    def delete_timeseries(self: "OpenFrame", lvl_zero_item: str) -> "OpenFrame":
+    def delete_timeseries(self: TypeOpenFrame, lvl_zero_item: str) -> TypeOpenFrame:
         """
         Parameters
         ----------
         lvl_zero_item: str
             The .tsdf column level 0 value of the timeseries to delete
 
         Returns
@@ -2420,20 +2431,20 @@
             self.constituents = [
                 item for item in self.constituents if item.label != lvl_zero_item
             ]
         self.tsdf.drop(lvl_zero_item, axis="columns", level=0, inplace=True)
         return self
 
     def trunc_frame(
-        self: "OpenFrame",
-        start_cut: dt.date | None = None,
-        end_cut: dt.date | None = None,
+        self: TypeOpenFrame,
+        start_cut: Optional[dt.date] = None,
+        end_cut: Optional[dt.date] = None,
         before: bool = True,
         after: bool = True,
-    ) -> "OpenFrame":
+    ) -> TypeOpenFrame:
         """Truncates DataFrame such that all timeseries have the same time span
 
         Parameters
         ----------
         start_cut: datetime.date, optional
             New first date
         end_cut: datetime.date, optional
@@ -2473,15 +2484,15 @@
                 f"One or more constituents still not truncated to same "
                 f"end dates.\n"
                 f"{self.tsdf.tail()}"
             )
         return self
 
     def relative(
-        self: "OpenFrame",
+        self: TypeOpenFrame,
         long_column: int = 0,
         short_column: int = 1,
         base_zero: bool = True,
     ) -> None:
         """Calculates cumulative relative return between two series.
         A new series is added to the frame.
 
@@ -2507,28 +2518,28 @@
             )
         else:
             self.tsdf[rel_label, ValueType.RELRTRN] = (
                 1.0 + self.tsdf.iloc[:, long_column] - self.tsdf.iloc[:, short_column]
             )
 
     def tracking_error_func(
-        self: "OpenFrame",
-        base_column: Tuple[str, ValueType] | int = -1,
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
-        periods_in_a_year_fixed: int | None = None,
+        self: TypeOpenFrame,
+        base_column: Union[Tuple[str, ValueType], int] = -1,
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
-        base_column: Tuple[str, ValueType] | int, default: -1
+        base_column: Union[Tuple[str, ValueType], int], default: -1
             Column of timeseries that is the denominator in the ratio.
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
             and to_date
         from_date : datetime.date, optional
             Specific from date
         to_date : datetime.date, optional
@@ -2584,29 +2595,29 @@
             data=terrors,
             index=self.tsdf.columns,
             name=f"Tracking Errors vs {short_label}",
             dtype="float64",
         )
 
     def info_ratio_func(
-        self: "OpenFrame",
-        base_column: Tuple[str, ValueType] | int = -1,
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
-        periods_in_a_year_fixed: int | None = None,
+        self: TypeOpenFrame,
+        base_column: Union[Tuple[str, ValueType], int] = -1,
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
         ----------
-        base_column: Tuple[str, ValueType] | int, default: -1
+        base_column: Union[Tuple[str, ValueType], int], default: -1
             Column of timeseries that is the denominator in the ratio.
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
             and to_date
         from_date : datetime.date, optional
             Specific from date
         to_date : datetime.date, optional
@@ -2663,36 +2674,36 @@
             data=ratios,
             index=self.tsdf.columns,
             name=f"Info Ratios vs {short_label}",
             dtype="float64",
         )
 
     def capture_ratio_func(
-        self: "OpenFrame",
+        self: TypeOpenFrame,
         ratio: LiteralCaptureRatio,
-        base_column: Tuple[str, ValueType] | int = -1,
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
-        periods_in_a_year_fixed: int | None = None,
+        base_column: Union[Tuple[str, ValueType], int] = -1,
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
         Finance Education (Vol 2 Winter 2013).
         https://www.economics-finance.org/jefe/volume12-2/11ArticleCox.pdf
 
         Parameters
         ----------
         ratio: LiteralCaptureRatio
             The ratio to calculate
-        base_column: Tuple[str, ValueType] | int, default: -1
+        base_column: Union[Tuple[str, ValueType], int], default: -1
             Column of timeseries that is the denominator in the ratio.
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
             and to_date
         from_date : datetime.date, optional
             Specific from date
         to_date : datetime.date, optional
@@ -2831,26 +2842,26 @@
             data=ratios,
             index=self.tsdf.columns,
             name=resultname,
             dtype="float64",
         )
 
     def beta(
-        self: "OpenFrame",
-        asset: Tuple[str, ValueType] | int,
-        market: Tuple[str, ValueType] | int,
+        self: TypeOpenFrame,
+        asset: Union[Tuple[str, ValueType], int],
+        market: Union[Tuple[str, ValueType], int],
     ) -> float:
         """https://www.investopedia.com/terms/b/beta.asp
         Calculates Beta as Co-variance of asset & market divided by Variance of market
 
         Parameters
         ----------
-        asset: Tuple[str, ValueType] | int
+        asset: Union[Tuple[str, ValueType], int]
             The column of the asset
-        market: Tuple[str, ValueType] | int
+        market: Union[Tuple[str, ValueType], int]
             The column of the market against which Beta is measured
 
         Returns
         -------
         float
             Beta as Co-variance of x & y divided by Variance of x
         """
@@ -2898,30 +2909,30 @@
 
         covariance = cov(y_value, x_value, ddof=1)
         beta = covariance[0, 1] / covariance[1, 1]
 
         return float(beta)
 
     def ord_least_squares_fit(
-        self: "OpenFrame",
-        y_column: Tuple[str, ValueType] | int,
-        x_column: Tuple[str, ValueType] | int,
+        self: TypeOpenFrame,
+        y_column: Union[Tuple[str, ValueType], int],
+        x_column: Union[Tuple[str, ValueType], int],
         fitted_series: bool = True,
         method: LiteralOlsFitMethod = "pinv",
         cov_type: LiteralOlsFitCovType = "nonrobust",
     ) -> RegressionResults:
         """https://www.statsmodels.org/stable/examples/notebooks/generated/ols.html
         Performs a linear regression and adds a new column with a fitted line
         using Ordinary Least Squares fit
 
         Parameters
         ----------
-        y_column: Tuple[str, ValueType] | int
+        y_column: Union[Tuple[str, ValueType], int]
             The column level values of the dependent variable y
-        x_column: Tuple[str, ValueType] | int
+        x_column: Union[Tuple[str, ValueType], int]
             The column level values of the exogenous variable x
         fitted_series: bool, default: True
             If True the fit is added as a new column in the .tsdf Pandas.DataFrame
         method: LiteralOlsFitMethod, default: pinv
             Method to solve least squares problem
         cov_type: LiteralOlsFitCovType, default: nonrobust
             Covariance estimator
@@ -2957,26 +2968,26 @@
         results = sm.OLS(y_value, x_value).fit(method=method, cov_type=cov_type)
         if fitted_series:
             self.tsdf[y_label, x_label] = results.predict(x_value)
 
         return results
 
     def make_portfolio(
-        self: "OpenFrame",
+        self: TypeOpenFrame,
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
@@ -3052,19 +3063,19 @@
                 raise NotImplementedError("Weight strategy not implemented")
         portfolio = dframe.dot(self.weights)
         portfolio = portfolio.add(1.0).cumprod().to_frame()
         portfolio.columns = [[name], [ValueType.PRICE]]
         return portfolio
 
     def rolling_info_ratio(
-        self: "OpenFrame",
+        self: TypeOpenFrame,
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
@@ -3108,15 +3119,15 @@
 
         ratiodf = (retdf.iloc[:, 0] / voldf.iloc[:, 0]).to_frame()
         ratiodf.columns = [[ratio_label], ["Information Ratio"]]
 
         return ratiodf
 
     def rolling_beta(
-        self: "OpenFrame",
+        self: TypeOpenFrame,
         asset_column: int = 0,
         market_column: int = 1,
         observations: int = 21,
     ) -> DataFrame:
         """https://www.investopedia.com/terms/b/beta.asp
         Calculates Beta as Co-variance of asset & market divided by Variance of market
 
@@ -3149,15 +3160,15 @@
         rollbeta = rollbeta.to_frame()
         rollbeta.index = rollbeta.index.droplevel(level=1)
         rollbeta.columns = [[beta_label], ["Beta"]]
 
         return rollbeta
 
     def rolling_corr(
-        self: "OpenFrame",
+        self: TypeOpenFrame,
         first_column: int = 0,
         second_column: int = 1,
         observations: int = 21,
     ) -> DataFrame:
         """Calculates correlation between two series. The period with
         at least the given number of observations is the first period calculated.
 
@@ -3189,20 +3200,20 @@
         )
         corrdf = corrdf.dropna().to_frame()
         corrdf.columns = [[corr_label], ["Rolling correlation"]]
 
         return corrdf
 
     def plot_series(
-        self: "OpenFrame",
+        self: TypeOpenFrame,
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
 
@@ -3293,20 +3304,20 @@
             config=fig["config"],
             output_type=output_type,
         )
 
         return figure, plotfile
 
     def plot_bars(
-        self: "OpenFrame",
+        self: TypeOpenFrame,
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

## openseries/load_plotly.py

```diff
@@ -1,28 +1,30 @@
 """
 Function to load plotly layout and configuration from local json file
 """
 from json import load
 from os.path import abspath, dirname, join
-from typing import Dict, List, Tuple
+from typing import Dict, List, Tuple, Union
 
 
 def load_plotly_dict(
     responsive: bool = True,
 ) -> Tuple[
     Dict[
         str,
-        str
-        | int
-        | float
-        | bool
-        | List[str]
-        | Dict[str, str | int | float | bool | List[str]],
+        Union[
+            str,
+            int,
+            float,
+            bool,
+            List[str],
+            Dict[str, Union[str, int, float, bool, List[str]]],
+        ],
     ],
-    Dict[str, str | float],
+    Dict[str, Union[str, float]],
 ]:
     """Function to load the plotly defaults
 
     Parameters
     ----------
     responsive : bool
```

## openseries/risk.py

```diff
@@ -2,30 +2,32 @@
 Value-at-Risk, Conditional-Value-at-Risk and drawdown functions.
 
 Source:
 https://github.com/pmorissette/ffn/blob/master/ffn/core.py
 """
 import datetime as dt
 from math import ceil
-from typing import cast, List
+from typing import cast, List, Union
 from numpy import (
     Inf,
     isnan,
     maximum,
     mean,
     nan_to_num,
     quantile,
     sort,
 )
 from pandas import DataFrame, Series
 
 from openseries.types import LiteralQuantileInterp
 
 
-def cvar_down(data: DataFrame | Series | List[float], level: float = 0.95) -> float:
+def cvar_down(
+    data: Union[DataFrame, Series, List[float]], level: float = 0.95
+) -> float:
     """https://www.investopedia.com/terms/c/conditional_value_at_risk.asp
 
     Parameters
     ----------
     data: DataFrame | Series | List[float]
         The data to perform the calculation over
     level: float, default: 0.95
@@ -43,15 +45,15 @@
         clean = nan_to_num(data)
     ret = clean[1:] / clean[:-1] - 1
     array = sort(ret)
     return cast(float, mean(array[: int(ceil(len(array) * (1 - level)))]))
 
 
 def var_down(
-    data: DataFrame | Series | List[float],
+    data: Union[DataFrame, Series, List[float]],
     level: float = 0.95,
     interpolation: LiteralQuantileInterp = "lower",
 ) -> float:
     """Downside Value At Risk, "VaR". The equivalent of
     percentile.inc([...], 1-level) over returns in MS Excel \n
     https://www.investopedia.com/terms/v/var.asp
 
@@ -74,15 +76,15 @@
         clean = nan_to_num(data.iloc[:, 0])
     else:
         clean = nan_to_num(data)
     ret = clean[1:] / clean[:-1] - 1
     return cast(float, quantile(ret, 1 - level, method=interpolation))
 
 
-def drawdown_series(prices: DataFrame | Series) -> DataFrame | Series:
+def drawdown_series(prices: Union[DataFrame, Series]) -> Union[DataFrame, Series]:
     """Calculates https://www.investopedia.com/terms/d/drawdown.asp
     This returns a series representing a drawdown. When the price is at all-time
     highs, the drawdown is 0. However, when prices are below high watermarks,
     the drawdown series = current / hwm - 1 The max drawdown can be obtained by
     simply calling .min() on the result (since the drawdown series is negative)
     Method ignores all gaps of NaN's in the price series.
 
@@ -92,51 +94,49 @@
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
 
 
-def drawdown_details(prices: DataFrame | Series) -> Series:
+def drawdown_details(prices: Union[DataFrame, Series], min_periods: int = 1) -> Series:
     """Details of the maximum drawdown
 
     Parameters
     ----------
     prices: DataFrame | Series
         A timeserie of dates and values
+    min_periods: int, default: 1
+        Smallest number of observations to use to find the maximum drawdown
 
     Returns
     -------
     Series
         Max Drawdown
         Start of drawdown
         Date of bottom
         Days from start to bottom
         Average fall per day
     """
 
-    mdd_date = (prices / prices.expanding(min_periods=1).max()).idxmin().values[0]
+    mdd_date = (
+        (prices / prices.expanding(min_periods=min_periods).max()).idxmin().values[0]
+    )
     mdate = dt.datetime.strptime(str(mdd_date)[:10], "%Y-%m-%d").date()
-    maxdown = ((prices / prices.expanding(min_periods=1).max()).min() - 1).iloc[0]
+    maxdown = (
+        (prices / prices.expanding(min_periods=min_periods).max()).min() - 1
+    ).iloc[0]
     ddata = prices.copy()
     drwdwn = drawdown_series(ddata).loc[: cast(int, mdate)]
     drwdwn.sort_index(ascending=False, inplace=True)
     sdate = drwdwn[drwdwn == 0.0].idxmax().values[0]
     sdate = dt.datetime.strptime(str(sdate)[:10], "%Y-%m-%d").date()
     duration = (mdate - sdate).days
     ret_per_day = maxdown / duration
```

## openseries/series.py

```diff
@@ -1,56 +1,58 @@
 """
 Defining the OpenTimeSeries class
 """
+from __future__ import annotations
 from copy import deepcopy
 import datetime as dt
 from enum import Enum
 from json import dump
 from math import ceil
 from os import path
 from pathlib import Path
 from re import compile as re_compile
-from typing import Any, cast, Dict, List, Tuple, TypeVar, Union
+from typing import Any, cast, Dict, List, Optional, Tuple, Type, TypeVar, Union
 from numpy import (
     array,
     cumprod,
-    dtype,
+    float64,
     insert,
     isnan,
     log,
-    ndarray,
     sqrt,
     square,
 )
+from numpy.typing import NDArray
 from dateutil.relativedelta import relativedelta
 from openpyxl import Workbook
 from openpyxl.utils.dataframe import dataframe_to_rows
 from pandas import (
     concat,
     DataFrame,
     DatetimeIndex,
     date_range,
     MultiIndex,
     Series,
 )
 from pandas.tseries.offsets import CustomBusinessDay
 from plotly.graph_objs import Figure
 from plotly.offline import plot
-from pydantic import BaseModel, constr, conlist, validator
+from pydantic import BaseModel, field_validator, model_validator
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
+    CountriesType,
+    CurrencyStringType,
+    DatabaseIdStringType,
+    DateListType,
+    ValueListType,
     LiteralQuantileInterp,
     LiteralBizDayFreq,
     LiteralPandasResampleConvention,
     LiteralPandasReindexMethod,
     LiteralNanMethod,
     LiteralLinePlotMode,
     LiteralBarPlotMode,
@@ -61,14 +63,16 @@
 from openseries.risk import (
     cvar_down,
     var_down,
     drawdown_series,
     drawdown_details,
 )
 
+TypeOpenTimeSeries = TypeVar("TypeOpenTimeSeries", bound="OpenTimeSeries")
+
 
 def check_if_none(item: Any) -> bool:
     """Function to check if a variable is None or equivalent
 
     Parameters
     ----------
     item : Any
@@ -126,109 +130,108 @@
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
+    values: ValueListType
     local_ccy: bool
     tsdf: DataFrame
+    currency: CurrencyStringType
+    domestic: CurrencyStringType = "SEK"
+    countries: CountriesType = "SE"
+    isin: Optional[str] = None
+    label: Optional[str] = None
 
-    class Config:
-        """Configurations for the OpenTimeSeries class"""
-
-        arbitrary_types_allowed = True
-        validate_assignment = True
-
-    @validator("isin")
-    def check_isincode(cls, isin_code: str) -> str:
+    @field_validator("isin")
+    @classmethod
+    def check_isincode(cls: Type[TypeOpenTimeSeries], isin_code: str) -> str:
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
+    def check_dates_unique(self) -> OpenTimeSeries:
+        """Pydantic validator to ensure that the dates are unique"""
+        dates_list_length = len(self.dates)
+        dates_set_length = len(set(self.dates))
+        if dates_list_length != dates_set_length:
+            raise ValueError("Dates are not unique")
+        return self
+
     @classmethod
     def setup_class(
-        cls, domestic_ccy: str = "SEK", countries: List[str] | str = "SE"
+        cls: Type[TypeOpenTimeSeries],
+        domestic_ccy: CurrencyStringType = "SEK",
+        countries: CountriesType = "SE",
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
@@ -259,24 +262,25 @@
             )
 
         cls.domestic = domestic_ccy
         cls.countries = countries
 
     @classmethod
     def from_arrays(
-        cls,
+        cls: Type[TypeOpenTimeSeries],
         name: str,
-        dates: List[str],
-        values: List[float],
+        dates: DateListType,
+        values: ValueListType,
         valuetype: ValueType = ValueType.PRICE,
-        timeseries_id: str = "",
-        instrument_id: str = "",
-        baseccy: str = "SEK",
+        timeseries_id: DatabaseIdStringType = "",
+        instrument_id: DatabaseIdStringType = "",
+        isin: Optional[str] = None,
+        baseccy: CurrencyStringType = "SEK",
         local_ccy: bool = True,
-    ) -> "OpenTimeSeries":
+    ) -> TypeOpenTimeSeries:
         """Creates a timeseries from a Pandas DataFrame or Series
 
         Parameters
         ----------
         name: str
             string identifier of the timeseries and/or instrument
         dates: List[str]
@@ -285,16 +289,18 @@
             Array of values
         valuetype : ValueType, default: ValueType.PRICE
             Identifies if the series is a series of values or returns
         timeseries_id : str
             Database identifier of the timeseries
         instrument_id: str
             Database identifier of the instrument associated with the timeseries
+        isin : str, optional
+            ISO 6166 identifier code of the associated instrument
         baseccy : str, default: "SEK"
-            The currency of the timeseries
+            ISO 4217 currency code of the timeseries
         local_ccy: bool, default: True
             Boolean flag indicating if timeseries is in local currency
 
         Returns
         -------
         OpenTimeSeries
             An OpenTimeSeries object
@@ -304,45 +310,46 @@
             name=name,
             label=name,
             dates=dates,
             values=values,
             valuetype=valuetype,
             timeseriesId=timeseries_id,
             instrumentId=instrument_id,
+            isin=isin,
             currency=baseccy,
             local_ccy=local_ccy,
             tsdf=DataFrame(
                 data=values,
                 index=[dejt.date() for dejt in DatetimeIndex(dates)],
                 columns=[[name], [valuetype]],
                 dtype="float64",
             ),
         )
 
     @classmethod
     def from_df(
-        cls,
-        dframe: DataFrame | Series,
+        cls: Type[TypeOpenTimeSeries],
+        dframe: Union[DataFrame, Series],
         column_nmbr: int = 0,
         valuetype: ValueType = ValueType.PRICE,
-        baseccy: str = "SEK",
+        baseccy: CurrencyStringType = "SEK",
         local_ccy: bool = True,
-    ) -> "OpenTimeSeries":
+    ) -> TypeOpenTimeSeries:
         """Creates a timeseries from a Pandas DataFrame or Series
 
         Parameters
         ----------
         dframe: DataFrame | Series
             Pandas DataFrame or Series
         column_nmbr : int, default: 0
             Using iloc[:, column_nmbr] to pick column
         valuetype : ValueType, default: ValueType.PRICE
             Identifies if the series is a series of values or returns
         baseccy : str, default: "SEK"
-            The currency of the timeseries
+            ISO 4217 currency code of the timeseries
         local_ccy: bool, default: True
             Boolean flag indicating if timeseries is in local currency
 
         Returns
         -------
         OpenTimeSeries
             An OpenTimeSeries object
@@ -397,24 +404,24 @@
                 columns=[[label], [valuetype]],
                 dtype="float64",
             ),
         )
 
     @classmethod
     def from_fixed_rate(
-        cls,
+        cls: Type[TypeOpenTimeSeries],
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
-    ) -> "OpenTimeSeries":
+    ) -> TypeOpenTimeSeries:
         """Creates a timeseries from values accruing with a given fixed rate return
 
         Providing a date_range of type Pandas DatetimeIndex takes priority over
         providing a combination of days and an end date.
 
         Parameters
         ----------
@@ -475,30 +482,30 @@
                 data=arr,
                 index=[d.date() for d in DatetimeIndex(d_range)],
                 columns=[[label], [valuetype]],
                 dtype="float64",
             ),
         )
 
-    def from_deepcopy(self: "OpenTimeSeries") -> "OpenTimeSeries":
+    def from_deepcopy(self: TypeOpenTimeSeries) -> TypeOpenTimeSeries:
         """Creates a copy of an OpenTimeSeries object
 
         Returns
         -------
         OpenTimeSeries
             An OpenTimeSeries object
         """
 
         return deepcopy(self)
 
     def to_xlsx(
-        self: "OpenTimeSeries",
+        self: TypeOpenTimeSeries,
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
@@ -530,16 +537,16 @@
             wrksheet.append(row)
 
         wrkbook.save(sheetfile)
 
         return sheetfile
 
     def to_json(
-        self: "OpenTimeSeries", filename: str, directory: str | None = None
-    ) -> Dict[str, str | bool | ValueType | List[str] | List[float]]:
+        self: TypeOpenTimeSeries, filename: str, directory: Optional[str] = None
+    ) -> Dict[str, Union[str, bool, ValueType, List[str], List[float]]]:
         """Dumps timeseries data into a json file
 
         The label and tsdf parameters are deleted before the json file is saved
 
         Parameters
         ----------
         filename: str
@@ -561,15 +568,15 @@
             data.pop(item)
 
         with open(path.join(directory, filename), "w", encoding="utf-8") as jsonfile:
             dump(data, jsonfile, indent=2, sort_keys=False)
 
         return data
 
-    def pandas_df(self: "OpenTimeSeries") -> "OpenTimeSeries":
+    def pandas_df(self: TypeOpenTimeSeries) -> TypeOpenTimeSeries:
         """Sets the .tsdf parameter as a Pandas DataFrame from the .dates and
         .values lists
 
         Returns
         -------
         OpenTimeSeries
             An OpenTimeSeries object
@@ -584,18 +591,18 @@
 
         dframe.sort_index(inplace=True)
         self.tsdf = dframe
 
         return self
 
     def calc_range(
-        self: "OpenTimeSeries",
-        months_offset: int | None = None,
-        from_dt: dt.date | None = None,
-        to_dt: dt.date | None = None,
+        self: TypeOpenTimeSeries,
+        months_offset: Optional[int] = None,
+        from_dt: Optional[dt.date] = None,
+        to_dt: Optional[dt.date] = None,
     ) -> Tuple[dt.date, dt.date]:
         """Creates user defined date range
 
         Parameters
         ----------
         months_offset: int, optional
             Number of months offset as positive integer. Overrides use of from_date
@@ -645,15 +652,15 @@
                     earlier -= dt.timedelta(days=1)
             if later is not None:
                 while later not in self.tsdf.index.tolist():
                     later += dt.timedelta(days=1)
 
         return earlier, later
 
-    def align_index_to_local_cdays(self: "OpenTimeSeries") -> "OpenTimeSeries":
+    def align_index_to_local_cdays(self: TypeOpenTimeSeries) -> TypeOpenTimeSeries:
         """Changes the index of the associated Pandas DataFrame .tsdf to align with
         local calendar business days
 
         Returns
         -------
         OpenTimeSeries
             An OpenTimeSeries object
@@ -673,15 +680,15 @@
         ]
 
         self.tsdf = self.tsdf.reindex(d_range, method=None, copy=False)
 
         return self
 
     def all_properties(
-        self: "OpenTimeSeries", properties: List[LiteralSeriesProps] | None = None
+        self: TypeOpenTimeSeries, properties: Optional[List[LiteralSeriesProps]] = None
     ) -> DataFrame:
         """Calculates the chosen timeseries properties
 
         Parameters
         ----------
         properties: List[LiteralSeriesProps], optional
             The properties to calculate. Defaults to calculating all available.
@@ -699,82 +706,82 @@
 
         props = OpenTimeSeriesPropertiesList(*properties)
         pdf = DataFrame.from_dict({x: getattr(self, x) for x in props}, orient="index")
         pdf.columns = self.tsdf.columns
         return pdf
 
     @property
-    def length(self: "OpenTimeSeries") -> int:
+    def length(self: TypeOpenTimeSeries) -> int:
         """
         Returns
         -------
         int
             Number of observations
         """
 
         return len(self.tsdf.index)
 
     @property
-    def first_idx(self: "OpenTimeSeries") -> dt.date:
+    def first_idx(self: TypeOpenTimeSeries) -> dt.date:
         """
         Returns
         -------
         datetime.date
             The first date in the timeseries
         """
 
         return cast(dt.date, self.tsdf.index[0])
 
     @property
-    def last_idx(self: "OpenTimeSeries") -> dt.date:
+    def last_idx(self: TypeOpenTimeSeries) -> dt.date:
         """
         Returns
         -------
         datetime.date
             The last date in the timeseries
         """
 
         return cast(dt.date, self.tsdf.index[-1])
 
     @property
-    def span_of_days(self: "OpenTimeSeries") -> int:
+    def span_of_days(self: TypeOpenTimeSeries) -> int:
         """
         Returns
         -------
         int
             Number of days from the first date to the last
         """
 
         return (self.last_idx - self.first_idx).days
 
     @property
-    def yearfrac(self: "OpenTimeSeries") -> float:
+    def yearfrac(self: TypeOpenTimeSeries) -> float:
         """
         Returns
         -------
         float
             Length of the timeseries expressed in years assuming all years
             have 365.25 days
         """
 
         return self.span_of_days / 365.25
 
     @property
-    def periods_in_a_year(self: "OpenTimeSeries") -> float:
+    def periods_in_a_year(self: TypeOpenTimeSeries) -> float:
         """
         Returns
         -------
         float
             The average number of observations per year
         """
 
         return self.length / self.yearfrac
 
     @property
-    def geo_ret(self: "OpenTimeSeries") -> float:
+    def geo_ret(self: TypeOpenTimeSeries) -> float:
         """https://www.investopedia.com/terms/c/cagr.asp
 
         Returns
         -------
         float
             Compounded Annual Growth Rate (CAGR)
         """
@@ -794,18 +801,18 @@
                 / self.tsdf.loc[self.first_idx, self.tsdf.columns.values[0]]
             )
             ** (1 / self.yearfrac)
             - 1,
         )
 
     def geo_ret_func(
-        self: "OpenTimeSeries",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        self: TypeOpenTimeSeries,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> float:
         """https://www.investopedia.com/terms/c/cagr.asp
 
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
@@ -842,31 +849,31 @@
                 / self.tsdf.loc[earlier, self.tsdf.columns.values[0]]
             )
             ** (1 / fraction)
             - 1,
         )
 
     @property
-    def arithmetic_ret(self: "OpenTimeSeries") -> float:
+    def arithmetic_ret(self: TypeOpenTimeSeries) -> float:
         """https://www.investopedia.com/terms/a/arithmeticmean.asp
 
         Returns
         -------
         float
             Annualized arithmetic mean of returns
         """
 
         return float((self.tsdf.pct_change().mean() * self.periods_in_a_year).iloc[0])
 
     def arithmetic_ret_func(
-        self: "OpenTimeSeries",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
-        periods_in_a_year_fixed: int | None = None,
+        self: TypeOpenTimeSeries,
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
@@ -901,15 +908,15 @@
                 .pct_change()
                 .mean()
                 * time_factor
             ).iloc[0],
         )
 
     @property
-    def value_ret(self: "OpenTimeSeries") -> float:
+    def value_ret(self: TypeOpenTimeSeries) -> float:
         """
         Returns
         -------
         float
             Simple return
         """
 
@@ -917,18 +924,18 @@
             raise ValueError(
                 "Simple Return cannot be calculated due to an initial value being "
                 "zero."
             )
         return float((self.tsdf.iloc[-1] / self.tsdf.iloc[0] - 1).iloc[0])
 
     def value_ret_func(
-        self: "OpenTimeSeries",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        self: TypeOpenTimeSeries,
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
@@ -948,15 +955,15 @@
             raise ValueError(
                 "Simple Return cannot be calculated due to an initial value being "
                 "zero."
             )
         return float((self.tsdf.loc[later] / self.tsdf.loc[earlier] - 1).iloc[0])
 
     def value_ret_calendar_period(
-        self: "OpenTimeSeries", year: int, month: int | None = None
+        self: TypeOpenTimeSeries, year: int, month: Optional[int] = None
     ) -> float:
         """
         Parameters
         ----------
         year : int
             Calendar year of the period to calculate.
         month : int, optional
@@ -975,15 +982,15 @@
         else:
             period = "-".join([str(year), str(month).zfill(2)])
         rtn = caldf.copy().pct_change()
         rtn = rtn.loc[period] + 1
         return float((rtn.apply(cumprod, axis="index").iloc[-1] - 1).iloc[0])
 
     @property
-    def vol(self: "OpenTimeSeries") -> float:
+    def vol(self: TypeOpenTimeSeries) -> float:
         """Based on Pandas .std() which is the equivalent of stdev.s([...])
         in MS Excel \n
         https://www.investopedia.com/terms/v/volatility.asp
 
         Returns
         -------
         float
@@ -992,19 +999,19 @@
 
         return cast(
             float,
             (self.tsdf.pct_change().std() * sqrt(self.periods_in_a_year)).iloc[0],
         )
 
     def vol_func(
-        self: "OpenTimeSeries",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
-        periods_in_a_year_fixed: int | None = None,
+        self: TypeOpenTimeSeries,
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
@@ -1039,15 +1046,15 @@
             (
                 self.tsdf.loc[cast(int, earlier) : cast(int, later)].pct_change().std()
                 * sqrt(time_factor)
             ).iloc[0],
         )
 
     @property
-    def downside_deviation(self: "OpenTimeSeries") -> float:
+    def downside_deviation(self: TypeOpenTimeSeries) -> float:
         """The standard deviation of returns that are below a Minimum Accepted
         Return of zero.
         It is used to calculate the Sortino Ratio \n
         https://www.investopedia.com/terms/d/downside-deviation.asp
 
         Returns
         -------
@@ -1060,20 +1067,20 @@
         return cast(
             float,
             sqrt((dddf[dddf.values < 0.0].values ** 2).sum() / self.length)
             * sqrt(self.periods_in_a_year),
         )
 
     def downside_deviation_func(
-        self: "OpenTimeSeries",
+        self: TypeOpenTimeSeries,
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
@@ -1120,29 +1127,29 @@
         return cast(
             float,
             sqrt((dddf[dddf.values < 0.0].values ** 2).sum() / how_many)
             * sqrt(time_factor),
         )
 
     @property
-    def ret_vol_ratio(self: "OpenTimeSeries") -> float:
+    def ret_vol_ratio(self: TypeOpenTimeSeries) -> float:
         """
         Returns
         -------
         float
             Ratio of the annualized arithmetic mean of returns and annualized
             volatility.
         """
         return self.arithmetic_ret / self.vol
 
     def ret_vol_ratio_func(
-        self: "OpenTimeSeries",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        self: TypeOpenTimeSeries,
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
@@ -1169,33 +1176,33 @@
 
         return (
             self.arithmetic_ret_func(months_from_last, from_date, to_date)
             - riskfree_rate
         ) / self.vol_func(months_from_last, from_date, to_date)
 
     @property
-    def sortino_ratio(self: "OpenTimeSeries") -> float:
+    def sortino_ratio(self: TypeOpenTimeSeries) -> float:
         """https://www.investopedia.com/terms/s/sortinoratio.asp
 
         Returns
         -------
         float
         Pandas.Series
             Sortino ratio calculated as the annualized arithmetic mean of returns
             / downside deviation. The ratio implies that the riskfree asset has zero
             volatility, and a minimum acceptable return of zero.
         """
 
         return self.arithmetic_ret / self.downside_deviation
 
     def sortino_ratio_func(
-        self: "OpenTimeSeries",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        self: TypeOpenTimeSeries,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
         riskfree_rate: float = 0.0,
     ) -> float:
         """The Sortino ratio calculated as ( asset return - risk free return )
         / downside deviation. The ratio implies that the riskfree asset has
         zero volatility. \n
         https://www.investopedia.com/terms/s/sortinoratio.asp
 
@@ -1226,15 +1233,15 @@
             min_accepted_return=0.0,
             months_from_last=months_from_last,
             from_date=from_date,
             to_date=to_date,
         )
 
     @property
-    def z_score(self: "OpenTimeSeries") -> float:
+    def z_score(self: TypeOpenTimeSeries) -> float:
         """https://www.investopedia.com/terms/z/zscore.asp
 
         Returns
         -------
         float
             Z-score as (last return - mean return) / standard deviation of returns.
         """
@@ -1244,18 +1251,18 @@
             (
                 (self.tsdf.pct_change().iloc[-1] - self.tsdf.pct_change().mean())
                 / self.tsdf.pct_change().std()
             ).iloc[0],
         )
 
     def z_score_func(
-        self: "OpenTimeSeries",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        self: TypeOpenTimeSeries,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> float:
         """https://www.investopedia.com/terms/z/zscore.asp
 
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
@@ -1272,83 +1279,85 @@
         """
 
         earlier, later = self.calc_range(months_from_last, from_date, to_date)
         part = self.tsdf.loc[cast(int, earlier) : cast(int, later)].pct_change().copy()
         return float(((part.iloc[-1] - part.mean()) / part.std()).iloc[0])
 
     @property
-    def max_drawdown(self: "OpenTimeSeries") -> float:
+    def max_drawdown(self: TypeOpenTimeSeries) -> float:
         """https://www.investopedia.com/terms/m/maximum-drawdown-mdd.asp
 
         Returns
         -------
         float
             Maximum drawdown without any limit on date range
         """
 
         return cast(
             float,
             ((self.tsdf / self.tsdf.expanding(min_periods=1).max()).min() - 1).iloc[0],
         )
 
     @property
-    def max_drawdown_date(self: "OpenTimeSeries") -> dt.date:
+    def max_drawdown_date(self: TypeOpenTimeSeries) -> dt.date:
         """https://www.investopedia.com/terms/m/maximum-drawdown-mdd.asp
 
         Returns
         -------
         datetime.date
             Date when the maximum drawdown occurred
         """
 
         mdddf = self.tsdf.copy()
         mdddf.index = DatetimeIndex(mdddf.index)
         mdd_date = (mdddf / mdddf.expanding(min_periods=1).max()).idxmin().values[0]
         return dt.datetime.strptime(str(mdd_date)[:10], "%Y-%m-%d").date()
 
     def max_drawdown_func(
-        self: "OpenTimeSeries",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        self: TypeOpenTimeSeries,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
+        min_periods: int = 1,
     ) -> float:
         """https://www.investopedia.com/terms/m/maximum-drawdown-mdd.asp
 
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
             and to_date
         from_date : datetime.date, optional
             Specific from date
         to_date : datetime.date, optional
             Specific to date
+        min_periods: int, default: 1
 
         Returns
         -------
         float
             Maximum drawdown without any limit on date range
         """
 
         earlier, later = self.calc_range(months_from_last, from_date, to_date)
         return cast(
             float,
             (
                 (
                     self.tsdf.loc[cast(int, earlier) : cast(int, later)]
                     / self.tsdf.loc[cast(int, earlier) : cast(int, later)]
-                    .expanding(min_periods=1)
+                    .expanding(min_periods=min_periods)
                     .max()
                 ).min()
                 - 1
             ).iloc[0],
         )
 
     @property
-    def max_drawdown_cal_year(self: "OpenTimeSeries") -> float:
+    def max_drawdown_cal_year(self: TypeOpenTimeSeries) -> float:
         """https://www.investopedia.com/terms/m/maximum-drawdown-mdd.asp
 
         Returns
         -------
         float
             Maximum drawdown in a single calendar year.
         """
@@ -1359,43 +1368,43 @@
                 self.tsdf.groupby(years)
                 .apply(lambda x: (x / x.expanding(min_periods=1).max()).min() - 1)
                 .min()
             ).iloc[0],
         )
 
     @property
-    def worst(self: "OpenTimeSeries") -> float:
+    def worst(self: TypeOpenTimeSeries) -> float:
         """
         Returns
         -------
         float
             Most negative percentage change
         """
 
         return float((self.tsdf.pct_change().min()).iloc[0])
 
     @property
-    def worst_month(self: "OpenTimeSeries") -> float:
+    def worst_month(self: TypeOpenTimeSeries) -> float:
         """
         Returns
         -------
         float
             Most negative month
         """
 
         resdf = self.tsdf.copy()
         resdf.index = DatetimeIndex(resdf.index)
         return float((resdf.resample("BM").last().pct_change().min()).iloc[0])
 
     def worst_func(
-        self: "OpenTimeSeries",
+        self: TypeOpenTimeSeries,
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
@@ -1422,32 +1431,32 @@
                 .rolling(observations, min_periods=observations)
                 .sum()
                 .min()
             ).iloc[0],
         )
 
     @property
-    def positive_share(self: "OpenTimeSeries") -> float:
+    def positive_share(self: TypeOpenTimeSeries) -> float:
         """
         Returns
         -------
         float
             The share of percentage changes that are greater than zero
         """
         pos = self.tsdf.pct_change()[1:][
             self.tsdf.pct_change()[1:].values >= 0.0
         ].count()
         tot = self.tsdf.pct_change()[1:].count()
         return float((pos / tot).iloc[0])
 
     def positive_share_func(
-        self: "OpenTimeSeries",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        self: TypeOpenTimeSeries,
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
@@ -1469,33 +1478,33 @@
             (
                 period[period.pct_change().ge(0.0)].count()
                 / period.pct_change().count()
             ).iloc[0],
         )
 
     @property
-    def skew(self: "OpenTimeSeries") -> float:
+    def skew(self: TypeOpenTimeSeries) -> float:
         """https://www.investopedia.com/terms/s/skewness.asp
 
         Returns
         -------
         float
             Skew of the return distribution
         """
 
         return cast(
             float,
             skew(a=self.tsdf.pct_change().values, bias=True, nan_policy="omit")[0],
         )
 
     def skew_func(
-        self: "OpenTimeSeries",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        self: TypeOpenTimeSeries,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> float:
         """https://www.investopedia.com/terms/s/skewness.asp
 
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
@@ -1518,15 +1527,15 @@
                 self.tsdf.loc[cast(int, earlier) : cast(int, later)].pct_change(),
                 bias=True,
                 nan_policy="omit",
             )[0],
         )
 
     @property
-    def kurtosis(self: "OpenTimeSeries") -> float:
+    def kurtosis(self: TypeOpenTimeSeries) -> float:
         """https://www.investopedia.com/terms/k/kurtosis.asp
 
         Returns
         -------
         float
             Kurtosis of the return distribution
         """
@@ -1537,18 +1546,18 @@
                 fisher=True,
                 bias=True,
                 nan_policy="omit",
             )[0],
         )
 
     def kurtosis_func(
-        self: "OpenTimeSeries",
-        months_from_last: int | None = None,
-        from_date: dt.date | None = None,
-        to_date: dt.date | None = None,
+        self: TypeOpenTimeSeries,
+        months_from_last: Optional[int] = None,
+        from_date: Optional[dt.date] = None,
+        to_date: Optional[dt.date] = None,
     ) -> float:
         """https://www.investopedia.com/terms/k/kurtosis.asp
 
         Parameters
         ----------
         months_from_last : int, optional
             number of months offset as positive integer. Overrides use of from_date
@@ -1573,15 +1582,15 @@
                 fisher=True,
                 bias=True,
                 nan_policy="omit",
             )[0],
         )
 
     @property
-    def cvar_down(self: "OpenTimeSeries") -> float:
+    def cvar_down(self: TypeOpenTimeSeries) -> float:
         """https://www.investopedia.com/terms/c/conditional_value_at_risk.asp
 
         Returns
         -------
         float
             Downside Conditional 95% Value At Risk "CVaR"
         """
@@ -1595,19 +1604,19 @@
                 .sort_values()
                 .iloc[: int(ceil((1 - level) * items))]
                 .mean()
             ),
         )
 
     def cvar_down_func(
-        self: "OpenTimeSeries",
+        self: TypeOpenTimeSeries,
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
@@ -1643,15 +1652,15 @@
                 .sort_values()
                 .iloc[: int(ceil((1 - level) * how_many))]
                 .mean()
             ),
         )
 
     @property
-    def var_down(self: "OpenTimeSeries") -> float:
+    def var_down(self: TypeOpenTimeSeries) -> float:
         """Downside 95% Value At Risk, "VaR". The equivalent of
         percentile.inc([...], 1-level) over returns in MS Excel \n
         https://www.investopedia.com/terms/v/var.asp
 
         Returns
         -------
         float
@@ -1665,19 +1674,19 @@
                 self.tsdf.pct_change()
                 .quantile(1 - level, interpolation=interpolation)
                 .iloc[0]
             ),
         )
 
     def var_down_func(
-        self: "OpenTimeSeries",
+        self: TypeOpenTimeSeries,
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
@@ -1708,15 +1717,15 @@
                 self.tsdf.loc[cast(int, earlier) : cast(int, later)]
                 .pct_change()
                 .quantile(q=1 - level, interpolation=interpolation)
             ).iloc[0],
         )
 
     @property
-    def vol_from_var(self: "OpenTimeSeries") -> float:
+    def vol_from_var(self: TypeOpenTimeSeries) -> float:
         """
         Returns
         -------
         float
             Implied annualized volatility from the Downside 95% VaR using the
             assumption that returns are normally distributed.
         """
@@ -1728,22 +1737,22 @@
                 -sqrt(self.periods_in_a_year)
                 * self.var_down_func(level, interpolation=interpolation)
                 / norm.ppf(level)
             ),
         )
 
     def vol_from_var_func(
-        self: "OpenTimeSeries",
+        self: TypeOpenTimeSeries,
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
@@ -1811,25 +1820,25 @@
                     level, months_from_last, from_date, to_date, interpolation
                 )
                 / norm.ppf(level)
             ),
         )
 
     def target_weight_from_var(
-        self: "OpenTimeSeries",
+        self: TypeOpenTimeSeries,
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
@@ -1875,29 +1884,31 @@
                     drift_adjust=drift_adjust,
                     periods_in_a_year_fixed=periods_in_a_year_fixed,
                 ),
                 max_leverage_local,
             ),
         )
 
-    def value_to_ret(self: "OpenTimeSeries") -> "OpenTimeSeries":
+    def value_to_ret(self: TypeOpenTimeSeries) -> TypeOpenTimeSeries:
         """
         Returns
         -------
         OpenTimeSeries
             The returns of the values in the series
         """
 
         self.tsdf = self.tsdf.pct_change()
         self.tsdf.iloc[0] = 0
         self.valuetype = ValueType.RTRN
         self.tsdf.columns = [[self.label], [self.valuetype]]
         return self
 
-    def value_to_diff(self: "OpenTimeSeries", periods: int = 1) -> "OpenTimeSeries":
+    def value_to_diff(
+        self: TypeOpenTimeSeries, periods: int = 1
+    ) -> TypeOpenTimeSeries:
         """Converts a valueseries to a series of its period differences
 
         Parameters
         ----------
         periods: int, default: 1
             The number of periods between observations over which difference
             is calculated
@@ -1910,50 +1921,51 @@
 
         self.tsdf = self.tsdf.diff(periods=periods)
         self.tsdf.iloc[0] = 0
         self.valuetype = ValueType.RTRN
         self.tsdf.columns = [[self.label], [self.valuetype]]
         return self
 
-    def value_to_log(self: "OpenTimeSeries") -> "OpenTimeSeries":
+    def value_to_log(self: TypeOpenTimeSeries) -> TypeOpenTimeSeries:
         """Converts a valueseries into logarithmic return series \n
         Equivalent to LN(value[t] / value[t=0]) in MS Excel
 
         Returns
         -------
         OpenTimeSeries
             An OpenTimeSeries object
         """
 
         self.tsdf = log(self.tsdf / self.tsdf.iloc[0])
         return self
 
-    def to_cumret(self: "OpenTimeSeries") -> "OpenTimeSeries":
+    def to_cumret(self: TypeOpenTimeSeries) -> TypeOpenTimeSeries:
         """Converts a returnseries into a cumulative valueseries
 
         Returns
         -------
         OpenTimeSeries
             An OpenTimeSeries object
         """
         if not any(
-            x == ValueType.RTRN for x in self.tsdf.columns.get_level_values(1).values
+            x == ValueType.RTRN
+            for x in cast(MultiIndex, self.tsdf.columns).get_level_values(1).values
         ):
             self.value_to_ret()
 
         self.tsdf = self.tsdf.add(1.0)
         self.tsdf = self.tsdf.cumprod(axis=0) / self.tsdf.iloc[0]
         self.valuetype = ValueType.PRICE
         self.tsdf.columns = [[self.label], [self.valuetype]]
 
         return self
 
     def from_1d_rate_to_cumret(
-        self: "OpenTimeSeries", days_in_year: int = 365, divider: float = 1.0
-    ) -> "OpenTimeSeries":
+        self: TypeOpenTimeSeries, days_in_year: int = 365, divider: float = 1.0
+    ) -> TypeOpenTimeSeries:
         """Converts a series of 1-day rates into a cumulative valueseries
 
         Parameters
         ----------
         days_in_year: int, default 365
             Calendar days per year used as divisor
         divider: float, default 100.0
@@ -1974,16 +1986,16 @@
         self.values = list(arr)
         self.valuetype = ValueType.PRICE
         self.pandas_df()
 
         return self
 
     def resample(
-        self: "OpenTimeSeries", freq: Union[LiteralBizDayFreq, str] = "BM"
-    ) -> "OpenTimeSeries":
+        self: TypeOpenTimeSeries, freq: Union[LiteralBizDayFreq, str] = "BM"
+    ) -> TypeOpenTimeSeries:
         """Resamples the timeseries frequency
 
         Parameters
         ----------
         freq: Union[LiteralBizDayFreq, str], default "BM"
             The date offset string that sets the resampled frequency
             Examples are "7D", "B", "M", "BM", "Q", "BQ", "A", "BA"
@@ -1996,19 +2008,19 @@
 
         self.tsdf.index = DatetimeIndex(self.tsdf.index)
         self.tsdf = self.tsdf.resample(freq).last()
         self.tsdf.index = [d.date() for d in DatetimeIndex(self.tsdf.index)]
         return self
 
     def resample_to_business_period_ends(
-        self: "OpenTimeSeries",
+        self: TypeOpenTimeSeries,
         freq: LiteralBizDayFreq = "BM",
         convention: LiteralPandasResampleConvention = "end",
         method: LiteralPandasReindexMethod = "nearest",
-    ) -> "OpenTimeSeries":
+    ) -> TypeOpenTimeSeries:
         """Resamples timeseries frequency to the business calendar
         month end dates of each period while leaving any stubs
         in place
 
         Parameters
         ----------
         freq: LiteralBizDayFreq, default BM
@@ -2057,50 +2069,50 @@
             ]
             + [self.tsdf.index[-1]]
         )
         dates = dates.drop_duplicates()
         self.tsdf = self.tsdf.reindex([d.date() for d in dates], method=method)
         return self
 
-    def to_drawdown_series(self: "OpenTimeSeries") -> "OpenTimeSeries":
+    def to_drawdown_series(self: TypeOpenTimeSeries) -> TypeOpenTimeSeries:
         """Converts the timeseries into a drawdown series
 
         Returns
         -------
         OpenTimeSeries
             An OpenTimeSeries object
         """
 
         self.tsdf = drawdown_series(self.tsdf)
         self.tsdf.columns = [[self.label], ["Drawdowns"]]
 
         return self
 
-    def drawdown_details(self: "OpenTimeSeries") -> DataFrame:
+    def drawdown_details(self: TypeOpenTimeSeries) -> DataFrame:
         """
         Returns
         -------
         Pandas.DataFrame
             Calculates 'Max Drawdown', 'Start of drawdown', 'Date of bottom',
             'Days from start to bottom', & 'Average fall per day'
         """
 
         dddf = self.tsdf.copy()
         dddf.index = DatetimeIndex(dddf.index)
         return drawdown_details(dddf).to_frame()
 
     def ewma_vol_func(
-        self: "OpenTimeSeries",
+        self: TypeOpenTimeSeries,
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
@@ -2160,17 +2172,17 @@
             )
 
         data.loc[:, (self.label, ValueType.EWMA)] = rawdata
 
         return data.loc[:, (self.label, ValueType.EWMA)]
 
     def rolling_vol(
-        self: "OpenTimeSeries",
+        self: TypeOpenTimeSeries,
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
@@ -2191,15 +2203,15 @@
             time_factor
         )
         voldf.dropna(inplace=True)
         voldf.columns = [[self.label], ["Rolling volatility"]]
 
         return voldf
 
-    def rolling_return(self: "OpenTimeSeries", observations: int = 21) -> DataFrame:
+    def rolling_return(self: TypeOpenTimeSeries, observations: int = 21) -> DataFrame:
         """
         Parameters
         ----------
         observations: int, default: 21
             Number of observations in the overlapping window.
 
         Returns
@@ -2214,15 +2226,15 @@
             .sum()
         )
         retdf.columns = [[self.label], ["Rolling returns"]]
 
         return retdf.dropna()
 
     def rolling_cvar_down(
-        self: "OpenTimeSeries", level: float = 0.95, observations: int = 252
+        self: TypeOpenTimeSeries, level: float = 0.95, observations: int = 252
     ) -> DataFrame:
         """
         Parameters
         ----------
         level: float, default: 0.95
             The sought Conditional Value At Risk level
         observations: int, default: 252
@@ -2239,15 +2251,15 @@
         )
         cvardf = cvardf.dropna()
         cvardf.columns = [[self.label], ["Rolling CVaR"]]
 
         return cvardf
 
     def rolling_var_down(
-        self: "OpenTimeSeries",
+        self: TypeOpenTimeSeries,
         level: float = 0.95,
         observations: int = 252,
         interpolation: LiteralQuantileInterp = "lower",
     ) -> DataFrame:
         """
         Parameters
         ----------
@@ -2269,16 +2281,16 @@
         )
         vardf = vardf.dropna()
         vardf.columns = [[self.label], ["Rolling VaR"]]
 
         return vardf
 
     def value_nan_handle(
-        self: "OpenTimeSeries", method: LiteralNanMethod = "fill"
-    ) -> "OpenTimeSeries":
+        self: TypeOpenTimeSeries, method: LiteralNanMethod = "fill"
+    ) -> TypeOpenTimeSeries:
         """Handling of missing values in a valueseries
 
         Parameters
         ----------
         method: LiteralNanMethod, default: "fill"
             Method used to handle NaN. Either fill with last known or drop
 
@@ -2295,16 +2307,16 @@
         if method == "fill":
             self.tsdf.fillna(method="ffill", inplace=True)
         else:
             self.tsdf.dropna(inplace=True)
         return self
 
     def return_nan_handle(
-        self: "OpenTimeSeries", method: LiteralNanMethod = "fill"
-    ) -> "OpenTimeSeries":
+        self: TypeOpenTimeSeries, method: LiteralNanMethod = "fill"
+    ) -> TypeOpenTimeSeries:
         """Handling of missing values in a returnseries
 
         Parameters
         ----------
         method: LiteralNanMethod, default: "fill"
             Method used to handle NaN. Either fill with zero or drop
 
@@ -2321,16 +2333,16 @@
         if method == "fill":
             self.tsdf.fillna(value=0.0, inplace=True)
         else:
             self.tsdf.dropna(inplace=True)
         return self
 
     def running_adjustment(
-        self: "OpenTimeSeries", adjustment: float, days_in_year: int = 365
-    ) -> "OpenTimeSeries":
+        self: TypeOpenTimeSeries, adjustment: float, days_in_year: int = 365
+    ) -> TypeOpenTimeSeries:
         """Adds (+) or subtracts (-) a fee from the timeseries return
 
         Parameters
         ----------
         adjustment: float
             Fee to add or subtract
         days_in_year: int, default: 365
@@ -2340,15 +2352,16 @@
         Returns
         -------
         OpenTimeSeries
             An OpenTimeSeries object
         """
         values: List[float]
         if any(
-            x == ValueType.RTRN for x in self.tsdf.columns.get_level_values(1).values
+            x == ValueType.RTRN
+            for x in cast(MultiIndex, self.tsdf.columns).get_level_values(1).values
         ):
             ra_df = self.tsdf.copy()
             values = [1.0]
             returns_input = True
         else:
             values = [self.tsdf.iloc[0, 0]]
             ra_df = self.tsdf.pct_change().copy()
@@ -2371,19 +2384,19 @@
         self.tsdf.columns = [[self.label], [self.valuetype]]
         self.tsdf.index = [d.date() for d in DatetimeIndex(self.tsdf.index)]
         if returns_input:
             self.value_to_ret()
         return self
 
     def set_new_label(
-        self: "OpenTimeSeries",
-        lvl_zero: str | None = None,
-        lvl_one: ValueType | None = None,
+        self: TypeOpenTimeSeries,
+        lvl_zero: Optional[str] = None,
+        lvl_one: Optional[ValueType] = None,
         delete_lvl_one: bool = False,
-    ) -> "OpenTimeSeries":
+    ) -> TypeOpenTimeSeries:
         """Sets the column labels of the .tsdf Pandas Dataframe associated
         with the timeseries
 
         Parameters
         ----------
         lvl_zero: str, optional
             New level zero label
@@ -2412,18 +2425,18 @@
             self.tsdf.columns = MultiIndex.from_arrays([[lvl_zero], [lvl_one]])
             self.label, self.valuetype = lvl_zero, cast(ValueType, lvl_one)
         if delete_lvl_one:
             self.tsdf.columns = self.tsdf.columns.droplevel(level=1)
         return self
 
     def plot_series(
-        self: "OpenTimeSeries",
+        self: TypeOpenTimeSeries,
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
 
@@ -2504,18 +2517,18 @@
             config=fig["config"],
             output_type=output_type,
         )
 
         return figure, plotfile
 
     def plot_bars(
-        self: "OpenTimeSeries",
+        self: TypeOpenTimeSeries,
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
@@ -2571,36 +2584,33 @@
             config=fig["config"],
             output_type=output_type,
         )
 
         return figure, plotfile
 
 
-TypeOpenTimeSeries = TypeVar("TypeOpenTimeSeries", bound=OpenTimeSeries)
-
-
 def timeseries_chain(
-    front: Union[TypeOpenTimeSeries, type(OpenTimeSeries)],
-    back: Union[TypeOpenTimeSeries, type(OpenTimeSeries)],
+    front: TypeOpenTimeSeries,
+    back: TypeOpenTimeSeries,
     old_fee: float = 0.0,
 ) -> Union[TypeOpenTimeSeries, OpenTimeSeries]:
     """Chain two timeseries together
 
     Parameters
     ----------
-    front: Union[TypeOpenTimeSeries, type(OpenTimeSeries)]
+    front: TypeOpenTimeSeries
         Earlier series to chain with
-    back: Union[TypeOpenTimeSeries, type(OpenTimeSeries)]
+    back: TypeOpenTimeSeries
         Later series to chain with
     old_fee: bool, default: False
         Fee to apply to earlier series
 
     Returns
     -------
-    Union[TypeOpenTimeSeries, OpenTimeSeries]
+    TypeOpenTimeSeries
         An OpenTimeSeries object or a subclass thereof
     """
     old = front.from_deepcopy()
     old.running_adjustment(old_fee)
     olddf = old.tsdf.copy()
     new = back.from_deepcopy()
     idx = 0
@@ -2615,15 +2625,15 @@
         first = new.tsdf.index[idx]
         if first > olddf.index[-1]:
             raise ValueError("Failed to find a matching date between series")
 
     dates: List[str] = [x.strftime("%Y-%m-%d") for x in olddf.index if x < first]
     values = array([x[0] for x in old.tsdf.values][: len(dates)])
     values = cast(
-        ndarray[Any, dtype[Any]],
+        NDArray[float64],
         list(values * new.tsdf.iloc[:, 0].loc[first] / olddf.iloc[:, 0].loc[first]),
     )
 
     dates.extend([x.strftime("%Y-%m-%d") for x in new.tsdf.index])
     values += [x[0] for x in new.tsdf.values]
 
     if back.__class__.__subclasscheck__(OpenTimeSeries):
```

## openseries/types.py

```diff
@@ -1,17 +1,52 @@
 """
 Declaring types used throughout the project
 """
-from typing import Literal, List
-from pydantic import BaseModel
+from typing import Annotated, Literal, List, Union
+from pydantic import confloat, conint, conlist, constr, StringConstraints
 
-COUNTRYPATTERN = r"^[A-Z]{2}$"
-CURRENCYPATTERN = r"^[A-Z]{3}$"
-DATEPATTERN = r"^\d{4}-(0[1-9]|1[0-2])-(0[1-9]|[12]\d|3[01])$"
-DATABASEIDPATTERN = r"^([0-9a-f]{24})?$"
+CountryStringType = Annotated[
+    str,
+    StringConstraints(
+        pattern=r"^[A-Z]{2}$", to_upper=True, min_length=2, max_length=2, strict=True
+    ),
+]
+CountryListType = conlist(
+    constr(
+        pattern=r"^[A-Z]{2}$", to_upper=True, min_length=2, max_length=2, strict=True
+    ),
+    min_length=1,
+)
+CountriesType = Union[CountryListType, CountryStringType]  # type: ignore[valid-type]
+
+CurrencyStringType = Annotated[
+    str,
+    StringConstraints(
+        pattern=r"^[A-Z]{3}$", to_upper=True, min_length=3, max_length=3, strict=True
+    ),
+]
+
+DateListType = Annotated[
+    List[str],
+    conlist(
+        constr(pattern=r"^\d{4}-(0[1-9]|1[0-2])-(0[1-9]|[12]\d|3[01])$"), min_length=2
+    ),
+]
+
+ValueListType = Annotated[List[float], conlist(float, min_length=2)]
+
+DatabaseIdStringType = Annotated[str, StringConstraints(pattern=r"^([0-9a-f]{24})?$")]
+
+DaysInYearType = Annotated[int, conint(strict=True, ge=1, le=366)]
+
+TradingDaysType = Annotated[int, conint(strict=True, gt=1)]
+
+SimCountType = Annotated[int, conint(strict=True, ge=1)]
+
+VolatilityType = Annotated[float, confloat(strict=True, gt=0.0)]
 
 LiteralLinePlotMode = Literal[
     "lines",
     "markers",
     "lines+markers",
     "lines+text",
     "markers+text",
@@ -185,67 +220,7 @@
             if item not in self.allowed_strings:
                 raise ValueError(
                     f"Invalid string: {item}. Allowed strings: {self.allowed_strings}"
                 )
             if item in seen:
                 raise ValueError(f"Duplicate string: {item}")
             seen.add(item)
-
-
-class ModelParameters(BaseModel):
-    """Object of the class ModelParameters. Subclass of the Pydantic BaseModel
-
-    Parameters
-    ----------
-    all_s0: float
-        Starting asset value
-    all_time: float
-        Amount of time to simulate for
-    all_delta: float
-        Delta, the rate of time e.g. 1/252 = daily, 1/12 = monthly
-    all_sigma: float
-        Volatility of the stochastic processes
-    all_r0: float, default: 0.0
-        Starting interest rate value
-    gbm_mu: float
-        Annual drift factor for geometric brownian motion
-    jumps_lamda: float, default: 0.0
-        Probability of a jump happening at each point in time
-    jumps_sigma: float, default: 0.0
-        Volatility of the jump size
-    jumps_mu: float, default: 0.0
-        Average jump size
-    cir_a: float, default: 0.0
-        Rate of mean reversion for Cox Ingersoll Ross
-    cir_mu: float, default: 0.0
-        Long run average interest rate for Cox Ingersoll Ross
-    cir_rho: float, default: 0.0
-        Correlation between the wiener processes of the Heston model
-    ou_a: float, default: 0.0
-        Rate of mean reversion for Ornstein Uhlenbeck
-    ou_mu: float, default: 0.0
-        Long run average interest rate for Ornstein Uhlenbeck
-    heston_a: float, default: 0.0
-        Rate of mean reversion for volatility in the Heston model
-    heston_mu: float, default: 0.0
-        Long run average volatility for the Heston model
-    heston_vol0: float, default: 0.0
-        Starting volatility value for the Heston vol model
-    """
-
-    all_s0: float
-    all_time: int
-    all_delta: float
-    all_sigma: float
-    gbm_mu: float
-    jumps_lamda: float = 0.0
-    jumps_sigma: float = 0.0
-    jumps_mu: float = 0.0
-    cir_a: float = 0.0
-    cir_mu: float = 0.0
-    all_r0: float = 0.0
-    cir_rho: float = 0.0
-    ou_a: float = 0.0
-    ou_mu: float = 0.0
-    heston_a: float = 0.0
-    heston_mu: float = 0.0
-    heston_vol0: float = 0.0
```

## Comparing `openseries-1.0.1.dist-info/LICENSE.md` & `openseries-1.1.5.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `openseries-1.0.1.dist-info/METADATA` & `openseries-1.1.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: openseries
-Version: 1.0.1
+Version: 1.1.5
 Summary: Package for simple financial time series analysis.
 Home-page: https://github.com/CaptorAB/OpenSeries
 License: BSD-3-Clause
 Keywords: python,python3,plotly,pandas,finance,fintech,data-science,timeseries,timeseries-data,timeseries-analysis,investment,investment-analysis,investing
 Author: Martin Karrin
 Author-email: martin.karrin@captor.se
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pydantic
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
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
 
@@ -64,18 +65,15 @@
 
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
@@ -121,18 +119,22 @@
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
@@ -198,26 +200,24 @@
 | [series.py](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/series.py)                             | Defines the class _OpenTimeSeries_ for managing and analyzing a single timeseries. The module also defines a function `timeseries_chain` that can be used to chain two timeseries objects together. |
 | [frame.py](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/frame.py)                               | Defines the class _OpenFrame_ for managing a group of timeseries, and e.g. calculate a portfolio timeseries from a rebalancing strategy between timeseries.                                         |
 | [datefixer.py](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/datefixer.py)                       | Date utilities. Please read the docstring of each function for its description.                                                                                                                     |
 | [load_plotly.py](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/load_plotly.py)                   | Functions to load [Plotly](https://plotly.com/python/) default layout and configuration from local json file.                                                                                       |
 | [plotly_layouts.json](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/plotly_layouts.json)         | [Plotly](https://plotly.com/python/) defaults used in the `plot_bars` and `plot_series` methods.                                                                                                    |
 | [plotly_captor_logo.json](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/plotly_captor_logo.json) | JSON with a link to the Captor logo used in the `plot_bars` and `plot_series` methods.                                                                                                              |
 | [risk.py](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/risk.py)                                 | Functions used to calculate VaR, CVaR and drawdowns.                                                                                                                                                |
-| [sim_price.py](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/sim_price.py)                       | Simulates OpenTimeSeries from different stochastic processes.                                                                                                                                       |
-| [stoch_processes.py](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/stoch_processes.py)           | Generates stochastic processes used in the `sim_price.py` module.                                                                                                                                   |
+| [simulation.py](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/simulation.py)                     | Simulates OpenTimeSeries from different stochastic processes.                                                                                                                                       |
 | [types.py](https://github.com/CaptorAB/OpenSeries/blob/master/openseries/types.py)                               | Contains all bespoke typing.                                                                                                                                                                        |
 
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

## Comparing `openseries-1.0.1.dist-info/RECORD` & `openseries-1.1.5.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 openseries/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-openseries/datefixer.py,sha256=h4zshiUkJmRmbBgiCCVulxVUa2SO1dRdJMAKLMxE-tc,9970
-openseries/frame.py,sha256=p0xHGTEe6eUlakoxgAldwXjquTSfyvXMektdsYEgJnI,115141
-openseries/load_plotly.py,sha256=DfpacL-aL5z-W0Cw7FL4YtDSbgeSI8Q-8DO6940wiJc,1119
+openseries/datefixer.py,sha256=AiTgkeGD8DMksNRsctp-tk9pSckUd6NoZBaRgBAM9oY,10168
+openseries/frame.py,sha256=GPMDtu5yOP5Ec0NSD6QjUARqVPVbJIhRFlugYRoXZlM,116260
+openseries/load_plotly.py,sha256=DSeLRNjMAlLYrYjD7zXCcKr0ilJLrmUqpPyqywqbbbU,1180
 openseries/plotly_captor_logo.json,sha256=pGMuPVu4cEO3ZsCH1wU03hxqbIQkHFNoJUs1k1WK89Y,178
 openseries/plotly_layouts.json,sha256=xhrMOqW8LXb4QMtPiNBGdkPX518OHThiIJ68jpQk524,1429
-openseries/risk.py,sha256=_NJd8V-6pMx8pTodW-QpGKlmCDbCn4TsEjieKnCkIxU,4404
-openseries/series.py,sha256=Xw7ppt2bCVspkjYIqZKcMNfVIlrsmrnV7XWtp99qxrg,84385
-openseries/sim_price.py,sha256=dWzmj22nq4TW4BZBwP8Ajtid_g322No6D_m7t5bT8No,13878
-openseries/stoch_processes.py,sha256=6O4C_nC2iBseWggvDDC2gTpTqS5fI5nfjSRpccaazLE,14673
-openseries/types.py,sha256=t5xeqoD-e9fm0aU5I9chbzLcZ-MHmb9-jInCz3NrIfk,6698
-openseries-1.0.1.dist-info/LICENSE.md,sha256=NJjeq3wyB7EnnHLmsdK1EK6zT00T1eB3FgAmHAPT_vM,1521
-openseries-1.0.1.dist-info/METADATA,sha256=PTN4E6RKx3YEmLLohbkKawOJZJPsbrE4B-wjRUxiWwM,47927
-openseries-1.0.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-openseries-1.0.1.dist-info/RECORD,,
+openseries/risk.py,sha256=T678SgRCuxKh49pF38DlivtQfXjG1NZ8fR2ff5PrLZw,4456
+openseries/series.py,sha256=ymSvN9NRwP8PAcvFIAXe-f9IWtXn4HyBVMI5XLrRFg0,85198
+openseries/simulation.py,sha256=-C7h5YS2a5JAK7aJS6oqrDrtMwxwTXR5b2jLS70K21Y,37088
+openseries/types.py,sha256=sBW0XvpPSJKhp6bloMZ9htkrPM-0fre4vku9B7Yq1_s,5767
+openseries-1.1.5.dist-info/LICENSE.md,sha256=NJjeq3wyB7EnnHLmsdK1EK6zT00T1eB3FgAmHAPT_vM,1521
+openseries-1.1.5.dist-info/METADATA,sha256=J85a7iUFPDTIR5zkCqt8BDpyWo5mJfzc8FSXxfX8kvg,47610
+openseries-1.1.5.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+openseries-1.1.5.dist-info/RECORD,,
```

