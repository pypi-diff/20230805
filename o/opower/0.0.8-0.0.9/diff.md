# Comparing `tmp/opower-0.0.8.tar.gz` & `tmp/opower-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opower-0.0.8.tar", last modified: Sun Jun  4 05:53:19 2023, max compression
+gzip compressed data, was "opower-0.0.9.tar", last modified: Sat Jun 10 07:00:40 2023, max compression
```

## Comparing `opower-0.0.8.tar` & `opower-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:53:19.625353 opower-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-04 05:53:10.000000 opower-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-04 05:53:19.625353 opower-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-04 05:53:10.000000 opower-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-04 05:53:10.000000 opower-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-04 05:53:19.625353 opower-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:53:19.621353 opower-0.0.8/src/
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-06-04 05:53:10.000000 opower-0.0.8/src/demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:53:19.621353 opower-0.0.8/src/opower/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-04 05:53:10.000000 opower-0.0.8/src/opower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-04 05:53:10.000000 opower-0.0.8/src/opower/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-06-04 05:53:10.000000 opower-0.0.8/src/opower/opower.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:53:19.625353 opower-0.0.8/src/opower/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-04 05:53:10.000000 opower-0.0.8/src/opower/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-04 05:53:10.000000 opower-0.0.8/src/opower/utilities/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-04 05:53:10.000000 opower-0.0.8/src/opower/utilities/pge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-04 05:53:10.000000 opower-0.0.8/src/opower/utilities/pse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:53:19.625353 opower-0.0.8/src/opower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-04 05:53:19.000000 opower-0.0.8/src/opower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-04 05:53:19.000000 opower-0.0.8/src/opower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 05:53:19.000000 opower-0.0.8/src/opower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-04 05:53:19.000000 opower-0.0.8/src/opower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 05:53:19.000000 opower-0.0.8/src/opower.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:53:19.625353 opower-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-04 05:53:10.000000 opower-0.0.8/tests/test_opower.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:00:40.203860 opower-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-10 07:00:28.000000 opower-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-10 07:00:40.203860 opower-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-10 07:00:28.000000 opower-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-10 07:00:28.000000 opower-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-10 07:00:40.203860 opower-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:00:40.199860 opower-0.0.9/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-06-10 07:00:28.000000 opower-0.0.9/src/demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:00:40.203860 opower-0.0.9/src/opower/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-10 07:00:28.000000 opower-0.0.9/src/opower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-10 07:00:28.000000 opower-0.0.9/src/opower/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-06-10 07:00:28.000000 opower-0.0.9/src/opower/opower.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:00:40.203860 opower-0.0.9/src/opower/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-10 07:00:28.000000 opower-0.0.9/src/opower/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-10 07:00:28.000000 opower-0.0.9/src/opower/utilities/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-10 07:00:28.000000 opower-0.0.9/src/opower/utilities/pge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-10 07:00:28.000000 opower-0.0.9/src/opower/utilities/pse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:00:40.203860 opower-0.0.9/src/opower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-10 07:00:40.000000 opower-0.0.9/src/opower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-10 07:00:40.000000 opower-0.0.9/src/opower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 07:00:40.000000 opower-0.0.9/src/opower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-10 07:00:40.000000 opower-0.0.9/src/opower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-10 07:00:40.000000 opower-0.0.9/src/opower.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:00:40.203860 opower-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-10 07:00:28.000000 opower-0.0.9/tests/test_opower.py
```

### Comparing `opower-0.0.8/LICENSE` & `opower-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `opower-0.0.8/PKG-INFO` & `opower-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opower
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python library for getting historical and forecasted usage/cost from utilities that use opower.com such as PG&E
 Author-email: tronikos <tronikos@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/tronikos/opower
 Project-URL: Bug Tracker, https://github.com/tronikos/opower/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `opower-0.0.8/README.md` & `opower-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `opower-0.0.8/pyproject.toml` & `opower-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "opower"
-version = "0.0.8"
+version = "0.0.9"
 license = {text = "Apache-2.0"}
 authors = [
     { name="tronikos", email="tronikos@gmail.com" },
 ]
 description = "A Python library for getting historical and forecasted usage/cost from utilities that use opower.com such as PG&E"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `opower-0.0.8/src/demo.py` & `opower-0.0.9/src/demo.py`

 * *Files identical despite different names*

### Comparing `opower-0.0.8/src/opower/__init__.py` & `opower-0.0.9/src/opower/__init__.py`

 * *Files identical despite different names*

### Comparing `opower-0.0.8/src/opower/opower.py` & `opower-0.0.9/src/opower/opower.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,17 +52,25 @@
 
     def __str__(self):
         """Return the value of the enum."""
         return self.value
 
 
 @dataclasses.dataclass
+class Customer:
+    """Data about a customer."""
+
+    uuid: str
+
+
+@dataclasses.dataclass
 class Account:
     """Data about an account."""
 
+    customer: Customer
     uuid: str
     utility_account_id: str
     meter_type: MeterType
 
 
 @dataclasses.dataclass
 class Forecast:
@@ -141,15 +149,15 @@
         """Initialize."""
         self.session = session
         self.session._default_headers = CIMultiDict({"User-Agent": "Mozilla/5.0"})
         self.session._raise_for_status = True
         self.utility: type[UtilityBase] = _select_utility(utility)
         self.username = username
         self.password = password
-        self.customer = None
+        self.customers = []
 
     async def async_login(self) -> None:
         """Login to the utility website and authorize opower.com for access.
 
         :raises InvalidAuth: if login information is incorrect
         :raises CannotConnect: if we receive any HTTP error
         """
@@ -177,93 +185,80 @@
         action_url, hidden_inputs = _get_form_action_url_and_hidden_inputs(result)
         assert set(hidden_inputs.keys()) == {"opentoken"}
 
         # Pass it back to the utility website.
         async with self.session.post(action_url, data=hidden_inputs) as resp:
             pass
 
-    async def async_get_accounts(self) -> list[Account]:
-        """Get a list of accounts for the signed in user.
-
-        Typically one account for electricity and one for gas.
-        """
-        customer = await self._async_get_customer()
-        accounts = []
-        for account in customer["utilityAccounts"]:
-            accounts.append(
-                Account(
-                    uuid=account["uuid"],
-                    utility_account_id=account["preferredUtilityAccountId"],
-                    meter_type=MeterType(account["meterType"]),
-                )
-            )
-        return accounts
-
     async def async_get_forecast(self) -> list[Forecast]:
         """Get current and forecasted usage and cost for the current monthly bill.
 
         One forecast for each account, typically one for electricity, one for gas.
         """
-        customer = await self._async_get_customer()
-        customer_uuid = customer["uuid"]
-        url = (
-            "https://"
-            f"{self.utility.subdomain()}"
-            ".opower.com/ei/edge/apis/bill-forecast-cws-v1/cws/"
-            f"{self.utility.subdomain()}"
-            "/customers/"
-            f"{customer_uuid}"
-            "/combined-forecast"
-        )
-        _LOGGER.debug("Fetching: %s", url)
-        async with self.session.get(url) as resp:
-            result = await resp.json()
-            if DEBUG_LOG_RESPONSE:
-                _LOGGER.debug("Fetched: %s", json.dumps(result, indent=2))
         forecasts = []
-        for forecast in result["accountForecasts"]:
-            forecasts.append(
-                Forecast(
-                    account=Account(
-                        uuid=forecast["accountUuids"][0],
-                        utility_account_id=str(forecast["preferredUtilityAccountId"]),
-                        meter_type=MeterType(forecast["meterType"]),
-                    ),
-                    start_date=date.fromisoformat(forecast["startDate"]),
-                    end_date=date.fromisoformat(forecast["endDate"]),
-                    current_date=date.fromisoformat(forecast["currentDate"]),
-                    unit_of_measure=UnitOfMeasure(forecast["unitOfMeasure"]),
-                    usage_to_date=float(forecast.get("usageToDate", 0)),
-                    cost_to_date=float(forecast.get("costToDate", 0)),
-                    forecasted_usage=float(forecast.get("forecastedUsage", 0)),
-                    forecasted_cost=float(forecast.get("forecastedCost", 0)),
-                    typical_usage=float(forecast.get("typicalUsage", 0)),
-                    typical_cost=float(forecast.get("typicalCost", 0)),
-                )
+        for customer in await self._async_get_customers():
+            url = (
+                "https://"
+                f"{self.utility.subdomain()}"
+                ".opower.com/ei/edge/apis/bill-forecast-cws-v1/cws/"
+                f"{self.utility.subdomain()}"
+                "/customers/"
+                f"{customer.uuid}"
+                "/combined-forecast"
             )
+            _LOGGER.debug("Fetching: %s", url)
+            async with self.session.get(url) as resp:
+                result = await resp.json()
+                if DEBUG_LOG_RESPONSE:
+                    _LOGGER.debug("Fetched: %s", json.dumps(result, indent=2))
+            for forecast in result["accountForecasts"]:
+                forecasts.append(
+                    Forecast(
+                        account=Account(
+                            customer=customer,
+                            uuid=forecast["accountUuids"][0],
+                            utility_account_id=str(
+                                forecast["preferredUtilityAccountId"]
+                            ),
+                            meter_type=MeterType(forecast["meterType"]),
+                        ),
+                        start_date=date.fromisoformat(forecast["startDate"]),
+                        end_date=date.fromisoformat(forecast["endDate"]),
+                        current_date=date.fromisoformat(forecast["currentDate"]),
+                        unit_of_measure=UnitOfMeasure(forecast["unitOfMeasure"]),
+                        usage_to_date=float(forecast.get("usageToDate", 0)),
+                        cost_to_date=float(forecast.get("costToDate", 0)),
+                        forecasted_usage=float(forecast.get("forecastedUsage", 0)),
+                        forecasted_cost=float(forecast.get("forecastedCost", 0)),
+                        typical_usage=float(forecast.get("typicalUsage", 0)),
+                        typical_cost=float(forecast.get("typicalCost", 0)),
+                    )
+                )
         return forecasts
 
-    async def _async_get_customer(self):
-        """Get information about the current customer."""
-        # Cache the customer data
-        if not self.customer:
-            async with self.session.get(
+    async def _async_get_customers(self) -> list[Customer]:
+        """Get customers associated to the user."""
+        # Cache the customers
+        if not self.customers:
+            url = (
                 "https://"
                 f"{self.utility.subdomain()}"
                 ".opower.com/ei/edge/apis/multi-account-v1/cws/"
                 f"{self.utility.subdomain()}"
-                # Alternative to get multiple accounts:
-                # /customers?offset=0&batchSize=100&addressFilter=
-                "/customers/current"
-            ) as resp:
-                self.customer = await resp.json()
+                "/customers?offset=0&batchSize=100&addressFilter="
+            )
+            _LOGGER.debug("Fetching: %s", url)
+            async with self.session.get(url) as resp:
+                result = await resp.json()
                 if DEBUG_LOG_RESPONSE:
-                    _LOGGER.debug("Fetched: %s", json.dumps(self.customer, indent=2))
-        assert self.customer
-        return self.customer
+                    _LOGGER.debug("Fetched: %s", json.dumps(result, indent=2))
+            for customer in result["customers"]:
+                self.customers.append(Customer(uuid=customer["uuid"]))
+        assert self.customers
+        return self.customers
 
     async def async_get_cost_reads(
         self,
         account: Account,
         aggregate_type: AggregateType,
         start_date: datetime | None = None,
         end_date: datetime | None = None,
@@ -276,15 +271,15 @@
         url = (
             "https://"
             f"{self.utility.subdomain()}"
             ".opower.com/ei/edge/apis/DataBrowser-v1/cws/cost/utilityAccount/"
             f"{account.uuid}"
         )
         reads = await self._async_get_dated_data(
-            url, aggregate_type, start_date, end_date
+            account.customer, url, aggregate_type, start_date, end_date
         )
         result = []
         for read in reads:
             result.append(
                 CostRead(
                     start_time=datetime.fromisoformat(read["startTime"]),
                     end_time=datetime.fromisoformat(read["endTime"]),
@@ -318,39 +313,40 @@
             ".opower.com/ei/edge/apis/DataBrowser-v1/cws/utilities/"
             f"{self.utility.subdomain()}"
             "/utilityAccounts/"
             f"{account.uuid}"
             "/reads"
         )
         reads = await self._async_get_dated_data(
-            url, aggregate_type, start_date, end_date
+            account.customer, url, aggregate_type, start_date, end_date
         )
         result = []
         for read in reads:
             result.append(
                 UsageRead(
                     start_time=datetime.fromisoformat(read["startTime"]),
                     end_time=datetime.fromisoformat(read["endTime"]),
                     consumption=read["consumption"]["value"],
                 )
             )
         return result
 
     async def _async_get_dated_data(
         self,
+        customer: Customer,
         url: str,
         aggregate_type: AggregateType,
         start_date: datetime | None = None,
         end_date: datetime | None = None,
     ) -> list[Any]:
         """Wrap _async_fetch by breaking requests for big date ranges to smaller ones to satisfy opower imposed limits."""
         if start_date is None:
             if aggregate_type == AggregateType.BILL:
                 return await self._async_fetch(
-                    url, aggregate_type, start_date, end_date
+                    customer, url, aggregate_type, start_date, end_date
                 )
             raise ValueError("start_date is required unless aggregate_type=BILL")
         if end_date is None:
             raise ValueError("end_date is required unless aggregate_type=BILL")
 
         start = arrow.get(start_date.date(), self.utility.timezone())
         end = arrow.get(end_date.date(), self.utility.timezone()).shift(days=1)
@@ -368,40 +364,46 @@
         req_end = end
         while True:
             req_start = start
             if max_request_days is not None:
                 req_start = max(start, req_end.shift(days=-max_request_days))
             if req_start >= req_end:
                 return result
-            reads = await self._async_fetch(url, aggregate_type, req_start, req_end)
+            reads = await self._async_fetch(
+                customer, url, aggregate_type, req_start, req_end
+            )
             if not reads:
                 return result
             result = reads + result
             req_end = req_start.shift(days=-1)
 
     async def _async_fetch(
         self,
+        customer: Customer,
         url: str,
         aggregate_type: AggregateType,
         start_date: datetime | arrow.Arrow | None = None,
         end_date: datetime | arrow.Arrow | None = None,
     ) -> list[Any]:
         convert_to_date = "/cws/utilities/" in url
         params = {"aggregateType": aggregate_type.value}
+        headers = {
+            "Opower-Selected-Entities": f'["urn:opower:customer:uuid:{customer.uuid}"]'
+        }
         if start_date:
             params["startDate"] = (
                 start_date.date() if convert_to_date else start_date
             ).isoformat()
         if end_date:
             params["endDate"] = (
                 end_date.date() if convert_to_date else end_date
             ).isoformat()
         _LOGGER.debug("Fetching: %s?%s", url, urlencode(params))
         try:
-            async with self.session.get(url, params=params) as resp:
+            async with self.session.get(url, params=params, headers=headers) as resp:
                 result = await resp.json()
                 if DEBUG_LOG_RESPONSE:
                     _LOGGER.debug("Fetched: %s", json.dumps(result, indent=2))
                 return result["reads"]
         except ClientResponseError as err:
             # Ignore server errors for BILL requests
             # that can happen if end_date is before account activation
```

### Comparing `opower-0.0.8/src/opower/utilities/base.py` & `opower-0.0.9/src/opower/utilities/base.py`

 * *Files identical despite different names*

### Comparing `opower-0.0.8/src/opower/utilities/pge.py` & `opower-0.0.9/src/opower/utilities/pge.py`

 * *Files identical despite different names*

### Comparing `opower-0.0.8/src/opower/utilities/pse.py` & `opower-0.0.9/src/opower/utilities/pse.py`

 * *Files identical despite different names*

### Comparing `opower-0.0.8/src/opower.egg-info/PKG-INFO` & `opower-0.0.9/src/opower.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opower
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python library for getting historical and forecasted usage/cost from utilities that use opower.com such as PG&E
 Author-email: tronikos <tronikos@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/tronikos/opower
 Project-URL: Bug Tracker, https://github.com/tronikos/opower/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

