# Comparing `tmp/rysk_client-0.2.8.tar.gz` & `tmp/rysk_client-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rysk_client-0.2.8.tar", max compression
+gzip compressed data, was "rysk_client-0.2.9.tar", max compression
```

## Comparing `rysk_client-0.2.8.tar` & `rysk_client-0.2.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    45006 2023-07-18 12:52:22.898416 rysk_client-0.2.8/README.md
--rw-r--r--   0        0        0      726 2023-07-18 12:52:22.902416 rysk_client-0.2.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/__init__.py
--rw-r--r--   0        0        0     9029 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/cli.py
--rw-r--r--   0        0        0    24651 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/client.py
--rw-r--r--   0        0        0      974 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/beyond_pricer/__init__.py
--rw-r--r--   0        0        0    35992 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/beyond_pricer/build/beyond_pricer.json
--rw-r--r--   0        0        0    13187 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.py
--rw-r--r--   0        0        0      527 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.yaml
--rw-r--r--   0        0        0      971 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/d_h_v_lens/__init__.py
--rw-r--r--   0        0        0    35311 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/d_h_v_lens/build/d_h_v_lens.json
--rw-r--r--   0        0        0     6580 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.py
--rw-r--r--   0        0        0      601 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.yaml
--rw-r--r--   0        0        0      968 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/o_token/__init__.py
--rw-r--r--   0        0        0    15813 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/o_token/build/o_token.json
--rw-r--r--   0        0        0     8845 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/o_token/contract.py
--rw-r--r--   0        0        0      509 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/o_token/contract.yaml
--rw-r--r--   0        0        0      976 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/option_exchange/__init__.py
--rw-r--r--   0        0        0    38053 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/option_exchange/build/option_exchange.json
--rw-r--r--   0        0        0    11285 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/option_exchange/contract.py
--rw-r--r--   0        0        0      533 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/option_exchange/contract.yaml
--rw-r--r--   0        0        0      976 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/opyn_controller/__init__.py
--rw-r--r--   0        0        0    42143 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/opyn_controller/build/opyn_controller.json
--rw-r--r--   0        0        0    13308 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/opyn_controller/contract.py
--rw-r--r--   0        0        0      533 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/opyn_controller/contract.yaml
--rw-r--r--   0        0        0      981 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/opyn_option_registry/__init__.py
--rw-r--r--   0        0        0    38232 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/opyn_option_registry/build/opyn_option_registry.json
--rw-r--r--   0        0        0    10787 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.py
--rw-r--r--   0        0        0      547 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.yaml
--rw-r--r--   0        0        0      965 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/usdc/__init__.py
--rw-r--r--   0        0        0    11137 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/usdc/build/usdc.json
--rw-r--r--   0        0        0     6104 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/usdc/contract.py
--rw-r--r--   0        0        0      580 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/usdc/contract.yaml
--rw-r--r--   0        0        0      979 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/user_position_lens/__init__.py
--rw-r--r--   0        0        0     2515 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/user_position_lens/build/user_position_lens.json
--rw-r--r--   0        0        0     4220 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/user_position_lens/contract.py
--rw-r--r--   0        0        0      541 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/user_position_lens/contract.yaml
--rw-r--r--   0        0        0      965 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/weth/__init__.py
--rw-r--r--   0        0        0    15880 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/weth/build/weth.json
--rw-r--r--   0        0        0     6490 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/weth/contract.py
--rw-r--r--   0        0        0      580 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/weth/contract.yaml
--rw-r--r--   0        0        0      488 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/packages/packages.json
--rw-r--r--   0        0        0      690 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/src/action_type.py
--rw-r--r--   0        0        0     1142 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/src/collateral.py
--rw-r--r--   0        0        0     5480 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/src/constants.py
--rw-r--r--   0        0        0      212 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/src/crypto.py
--rw-r--r--   0        0        0      185 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/src/exceptions.py
--rw-r--r--   0        0        0     9777 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/src/operation_factory.py
--rw-r--r--   0        0        0      507 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/src/order.py
--rw-r--r--   0        0        0      182 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/src/order_side.py
--rw-r--r--   0        0        0     4538 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/src/pnl_calculator.py
--rw-r--r--   0        0        0      517 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/src/position.py
--rw-r--r--   0        0        0     1114 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/src/position_manager.py
--rw-r--r--   0        0        0      193 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/src/position_side.py
--rw-r--r--   0        0        0     9137 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/src/rysk_option_market.py
--rw-r--r--   0        0        0     3253 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/src/subgraph.py
--rw-r--r--   0        0        0     3443 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/src/utils.py
--rw-r--r--   0        0        0    13973 2023-07-18 12:52:22.902416 rysk_client-0.2.8/rysk_client/web3_client.py
--rw-r--r--   0        0        0    45624 1970-01-01 00:00:00.000000 rysk_client-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    45006 2023-08-03 17:15:37.735755 rysk_client-0.2.9/README.md
+-rw-r--r--   0        0        0      726 2023-08-03 17:15:37.739755 rysk_client-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/__init__.py
+-rw-r--r--   0        0        0     9029 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/cli.py
+-rw-r--r--   0        0        0    25058 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/client.py
+-rw-r--r--   0        0        0      974 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/beyond_pricer/__init__.py
+-rw-r--r--   0        0        0    35992 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/beyond_pricer/build/beyond_pricer.json
+-rw-r--r--   0        0        0    13187 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.py
+-rw-r--r--   0        0        0      527 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.yaml
+-rw-r--r--   0        0        0      971 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/d_h_v_lens/__init__.py
+-rw-r--r--   0        0        0    35311 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/d_h_v_lens/build/d_h_v_lens.json
+-rw-r--r--   0        0        0     6580 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.py
+-rw-r--r--   0        0        0      601 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.yaml
+-rw-r--r--   0        0        0      968 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/o_token/__init__.py
+-rw-r--r--   0        0        0    15813 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/o_token/build/o_token.json
+-rw-r--r--   0        0        0     8845 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/o_token/contract.py
+-rw-r--r--   0        0        0      509 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/o_token/contract.yaml
+-rw-r--r--   0        0        0      976 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/option_exchange/__init__.py
+-rw-r--r--   0        0        0    38053 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/option_exchange/build/option_exchange.json
+-rw-r--r--   0        0        0    11285 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/option_exchange/contract.py
+-rw-r--r--   0        0        0      533 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/option_exchange/contract.yaml
+-rw-r--r--   0        0        0      976 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/opyn_controller/__init__.py
+-rw-r--r--   0        0        0    42143 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/opyn_controller/build/opyn_controller.json
+-rw-r--r--   0        0        0    13308 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/opyn_controller/contract.py
+-rw-r--r--   0        0        0      533 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/opyn_controller/contract.yaml
+-rw-r--r--   0        0        0      981 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/opyn_option_registry/__init__.py
+-rw-r--r--   0        0        0    38232 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/opyn_option_registry/build/opyn_option_registry.json
+-rw-r--r--   0        0        0    10787 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.py
+-rw-r--r--   0        0        0      547 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.yaml
+-rw-r--r--   0        0        0      965 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/usdc/__init__.py
+-rw-r--r--   0        0        0    11137 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/usdc/build/usdc.json
+-rw-r--r--   0        0        0     6104 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/usdc/contract.py
+-rw-r--r--   0        0        0      580 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/usdc/contract.yaml
+-rw-r--r--   0        0        0      979 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/user_position_lens/__init__.py
+-rw-r--r--   0        0        0     2515 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/user_position_lens/build/user_position_lens.json
+-rw-r--r--   0        0        0     4220 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/user_position_lens/contract.py
+-rw-r--r--   0        0        0      541 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/user_position_lens/contract.yaml
+-rw-r--r--   0        0        0      965 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/weth/__init__.py
+-rw-r--r--   0        0        0    15880 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/weth/build/weth.json
+-rw-r--r--   0        0        0     6490 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/weth/contract.py
+-rw-r--r--   0        0        0      580 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/weth/contract.yaml
+-rw-r--r--   0        0        0      488 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/packages/packages.json
+-rw-r--r--   0        0        0      690 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/src/action_type.py
+-rw-r--r--   0        0        0     1142 2023-08-03 17:15:37.739755 rysk_client-0.2.9/rysk_client/src/collateral.py
+-rw-r--r--   0        0        0     5480 2023-08-03 17:15:37.743755 rysk_client-0.2.9/rysk_client/src/constants.py
+-rw-r--r--   0        0        0      212 2023-08-03 17:15:37.743755 rysk_client-0.2.9/rysk_client/src/crypto.py
+-rw-r--r--   0        0        0      185 2023-08-03 17:15:37.743755 rysk_client-0.2.9/rysk_client/src/exceptions.py
+-rw-r--r--   0        0        0     8922 2023-08-03 17:15:37.743755 rysk_client-0.2.9/rysk_client/src/operation_factory.py
+-rw-r--r--   0        0        0      507 2023-08-03 17:15:37.743755 rysk_client-0.2.9/rysk_client/src/order.py
+-rw-r--r--   0        0        0      182 2023-08-03 17:15:37.743755 rysk_client-0.2.9/rysk_client/src/order_side.py
+-rw-r--r--   0        0        0     4538 2023-08-03 17:15:37.743755 rysk_client-0.2.9/rysk_client/src/pnl_calculator.py
+-rw-r--r--   0        0        0      517 2023-08-03 17:15:37.743755 rysk_client-0.2.9/rysk_client/src/position.py
+-rw-r--r--   0        0        0     1114 2023-08-03 17:15:37.743755 rysk_client-0.2.9/rysk_client/src/position_manager.py
+-rw-r--r--   0        0        0      193 2023-08-03 17:15:37.743755 rysk_client-0.2.9/rysk_client/src/position_side.py
+-rw-r--r--   0        0        0     9137 2023-08-03 17:15:37.743755 rysk_client-0.2.9/rysk_client/src/rysk_option_market.py
+-rw-r--r--   0        0        0     3253 2023-08-03 17:15:37.743755 rysk_client-0.2.9/rysk_client/src/subgraph.py
+-rw-r--r--   0        0        0     3443 2023-08-03 17:15:37.743755 rysk_client-0.2.9/rysk_client/src/utils.py
+-rw-r--r--   0        0        0    13812 2023-08-03 17:15:37.743755 rysk_client-0.2.9/rysk_client/web3_client.py
+-rw-r--r--   0        0        0    45624 1970-01-01 00:00:00.000000 rysk_client-0.2.9/PKG-INFO
```

### Comparing `rysk_client-0.2.8/README.md` & `rysk_client-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/pyproject.toml` & `rysk_client-0.2.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rysk_client"
-version = "0.2.8"
+version = "0.2.9"
 description = ""
 authors = ["8baller <8ball030@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "rysk_client", from = "." },
 ]
```

### Comparing `rysk_client-0.2.8/rysk_client/cli.py` & `rysk_client-0.2.9/rysk_client/cli.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/client.py` & `rysk_client-0.2.9/rysk_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -444,36 +444,38 @@
             self._logger.info("Fetching Tickers.")
             self.fetch_tickers()
         _amount = amount * WETH_MULTIPLIER
 
         rysk_option_market = self.get_market(market)
         if rysk_option_market.is_put:
             rysk_option_market.collateral = self.collateral_factory.USDC
+            # we need to approve the collateral
             amount_to_approve = int(
-                self._option_chain.current_price
-                * amount
-                * (1 + ALLOWED_SLIPPAGE)
-                * WETH_MULTIPLIER
+                rysk_option_market.strike / WETH_MULTIPLIER * amount * USDC_MULTIPLIER
             )
             contract = self.web3_client.usdc
+            collateral_asset = "usdc"
+
         else:
             rysk_option_market.collateral = self.collateral_factory.WETH
             amount_to_approve = int(_amount * (1 + ALLOWED_SLIPPAGE))
             contract = self.web3_client.settlement_weth
         series = self.market_factory.to_series(rysk_option_market)
 
         acceptable_premium = self.web3_client.get_options_prices(
             series,
             dhv_exposure=rysk_option_market.dhv,
             amount=_amount,
             side=OrderSide.SELL.value,
             collateral=collateral_asset,
         )
 
-        self._logger.info(f"Acceptable premium: ${acceptable_premium:.2f}")
+        self._logger.info(
+            f"Acceptable premium: ${acceptable_premium / USDC_MULTIPLIER:.2f}"
+        )
 
         user_vaults = self.web3_client.fetch_user_vaults(self._crypto.address)
         otoken_id = self.web3_client.get_otoken(series)
         self._logger.info(f"Option Otoken id is {otoken_id}")
 
         issue_new_vault = False
         if otoken_id not in set(i[1] for i in user_vaults):
@@ -522,15 +524,15 @@
         operate_tuple = self.operation_factory.sell(
             int(acceptable_premium * 0.95),
             owner_address=self._crypto.address,  # pylint: disable=E1120
             exchange_address=self.web3_client.option_exchange.address,
             otoken_address=otoken_address,
             amount=int(_amount),
             vault_id=int(vault_id),
-            collateral=int(_amount),
+            collateral_amount=int(amount_to_approve),
             rysk_option_market=rysk_option_market,
             issue_new_vault=issue_new_vault,
         )
         return self.web3_client._operate(  # pylint: disable=protected-access
             operate_tuple, self.web3_client.option_exchange
         )
 
@@ -583,15 +585,15 @@
         otoken_address = self.web3_client.get_otoken(series)
         if size is None:
             _amount = self.web3_client.get_otoken_balance(otoken_address) * 10**10
         else:
             _amount = size * WETH_MULTIPLIER
         if _market.name not in self.active_markets:
             raise ValueError(f"{market} is not an active market...")
-        acceptable_premium = int(_market.ask * (1 - ALLOWED_SLIPPAGE))
+        acceptable_premium = int(_market.ask * (1 - ALLOWED_SLIPPAGE) * size)
         # we check the approval
         otoken_contract = self.web3_client.get_otoken_contract(otoken_address)
 
         # we get the balance
         balance = self.web3_client.get_otoken_balance(otoken_address)
 
         self._logger.info(f"Balance for {market} is {balance / 10**8}")
@@ -656,17 +658,24 @@
         positions = [f for f in user_vaults if f[1] == otoken_id]
         if len(positions) == 0:
             raise ValueError(f"Nothing to close for {market}...")
         if len(positions) > 1:
             raise ValueError(f"Multiple positions for {market}...")
         vault_id = positions[0][0]
 
+        if rysk_option_market.is_put:
+            # here we retrieve how much collateral we get for the amount of options
+            # we basically need strike * amount
+            strike = rysk_option_market.strike / WETH_MULTIPLIER
+            collateral_amount = int(strike * size * USDC_MULTIPLIER)
+        else:
+            collateral_amount = int(_amount)
+
         txn = self.web3_client.close_short(
             acceptable_premium=acceptable_premium,
             amount=int(_amount),
             otoken_address=self.web3_client.web3.toChecksumAddress(otoken_address),
             collateral_asset=rysk_option_market.collateral,
-            collateral_amount=int(_amount),
+            collateral_amount=collateral_amount,
             vault_id=vault_id,
-            rysk_option_market=rysk_option_market,
         )
         return self._sign_and_submit(txn)
```

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/beyond_pricer/__init__.py` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/beyond_pricer/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/beyond_pricer/build/beyond_pricer.json` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/beyond_pricer/build/beyond_pricer.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.py` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.yaml` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/d_h_v_lens/__init__.py` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/d_h_v_lens/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/d_h_v_lens/build/d_h_v_lens.json` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/d_h_v_lens/build/d_h_v_lens.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.py` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.yaml` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/o_token/__init__.py` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/o_token/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/o_token/build/o_token.json` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/o_token/build/o_token.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/o_token/contract.py` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/o_token/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/option_exchange/__init__.py` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/option_exchange/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/option_exchange/build/option_exchange.json` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/option_exchange/build/option_exchange.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/option_exchange/contract.py` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/option_exchange/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/option_exchange/contract.yaml` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/option_exchange/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/opyn_controller/__init__.py` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/opyn_controller/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/opyn_controller/build/opyn_controller.json` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/opyn_controller/build/opyn_controller.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/opyn_controller/contract.py` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/opyn_controller/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/opyn_controller/contract.yaml` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/opyn_controller/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/opyn_option_registry/__init__.py` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/opyn_option_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/opyn_option_registry/build/opyn_option_registry.json` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/opyn_option_registry/build/opyn_option_registry.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.py` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.yaml` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/usdc/__init__.py` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/usdc/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/usdc/build/usdc.json` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/usdc/build/usdc.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/usdc/contract.py` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/usdc/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/usdc/contract.yaml` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/usdc/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/user_position_lens/__init__.py` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/user_position_lens/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/user_position_lens/build/user_position_lens.json` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/user_position_lens/build/user_position_lens.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/user_position_lens/contract.py` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/user_position_lens/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/user_position_lens/contract.yaml` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/user_position_lens/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/weth/__init__.py` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/weth/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/weth/build/weth.json` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/weth/build/weth.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/weth/contract.py` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/weth/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/packages/eightballer/contracts/weth/contract.yaml` & `rysk_client-0.2.9/rysk_client/packages/eightballer/contracts/weth/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/src/action_type.py` & `rysk_client-0.2.9/rysk_client/src/action_type.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/src/collateral.py` & `rysk_client-0.2.9/rysk_client/src/collateral.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/src/constants.py` & `rysk_client-0.2.9/rysk_client/src/constants.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/src/operation_factory.py` & `rysk_client-0.2.9/rysk_client/src/operation_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from dataclasses import dataclass
 from enum import Enum
 
 from rysk_client.src.action_type import ActionType, RyskActionType
 from rysk_client.src.collateral import CollateralFactory
 from rysk_client.src.constants import (EMPTY_SERIES, NULL_ADDRESS, NULL_DATA,
-                                       WETH_MULTIPLIER, Chain)
+                                       Chain)
 from rysk_client.src.rysk_option_market import MarketFactory, RyskOptionMarket
 from rysk_client.src.utils import from_wei_to_opyn
 
 
 class OperationType(Enum):
     """Distinguish between operations for the rysk and opyn contracts."""
 
@@ -85,15 +85,15 @@
     ):
         """Create the operation to buy an option."""
         return [
             {
                 "operation": OperationType.RYSK_ACTION.value,
                 "operationQueue": [
                     {
-                        "actionType": RyskActionType.CLOSE_OPTION.value,
+                        "actionType": RyskActionType.SELL_OPTION.value,
                         "owner": NULL_ADDRESS,
                         "secondAddress": owner_address,
                         "asset": otoken_address,
                         "vaultId": 0,
                         "amount": amount,
                         "optionSeries": EMPTY_SERIES,
                         "indexOrAcceptablePremium": acceptable_premium,
@@ -107,30 +107,23 @@
         self,
         acceptable_premium: int,
         owner_address: str,
         exchange_address: str,
         otoken_address: str,
         amount: int,
         vault_id: int,
-        collateral: int,
+        collateral_amount: int,
         rysk_option_market: RyskOptionMarket,
         issue_new_vault: bool = False,
     ):
         """Create the operation to sell an option."""
         if rysk_option_market.is_put:
-            # here we retrieve how much collateral we get for the amount of options
-            # we basically need strike * amount
-            eth = collateral / WETH_MULTIPLIER
-            strike = rysk_option_market.strike / WETH_MULTIPLIER
-            _amount = from_wei_to_opyn(amount) / 1e2
-            collateral_amount = int(eth * strike * _amount)
             collateral = self.collateral_factory.USDC
 
         else:
-            collateral_amount = amount
             collateral = self.collateral_factory.WETH
 
         required_data = [
             {
                 "actionType": ActionType.DEPOSIT_COLLATERAL.value,
                 "owner": owner_address,
                 "secondAddress": exchange_address,
@@ -205,26 +198,18 @@
         acceptable_premium: int,
         owner_address: str,
         otoken_address: str,
         amount: int,
         collateral_amount: int,
         collateral_asset: str,
         vault_id: int,
-        rysk_option_market: RyskOptionMarket,
     ):
         """
         Create the operation to close a short options
         """
-        if rysk_option_market.is_put:
-            # here we retrieve how much collateral we get for the amount of options
-            # we basically need strike * amount
-            eth = collateral_amount / WETH_MULTIPLIER
-            strike = rysk_option_market.strike / WETH_MULTIPLIER
-            _amount = from_wei_to_opyn(amount) / 1e2
-            collateral_amount = int(eth * strike * _amount)
 
         tx_data = [
             {
                 "operation": OperationType.RYSK_ACTION.value,
                 "operationQueue": [
                     {
                         "actionType": RyskActionType.BUY_OPTION.value,
```

### Comparing `rysk_client-0.2.8/rysk_client/src/pnl_calculator.py` & `rysk_client-0.2.9/rysk_client/src/pnl_calculator.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/src/position.py` & `rysk_client-0.2.9/rysk_client/src/position.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/src/position_manager.py` & `rysk_client-0.2.9/rysk_client/src/position_manager.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/src/rysk_option_market.py` & `rysk_client-0.2.9/rysk_client/src/rysk_option_market.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/src/subgraph.py` & `rysk_client-0.2.9/rysk_client/src/subgraph.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/src/utils.py` & `rysk_client-0.2.9/rysk_client/src/utils.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.8/rysk_client/web3_client.py` & `rysk_client-0.2.9/rysk_client/web3_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from rysk_client.src.collateral import CollateralFactory
 from rysk_client.src.constants import (ARBITRUM_GOERLI, NULL_ADDRESS,
                                        NULL_DATA, Chain)
 from rysk_client.src.crypto import EthCrypto
 from rysk_client.src.operation_factory import OperationFactory
 from rysk_client.src.order import Order
 from rysk_client.src.order_side import OrderSide
-from rysk_client.src.rysk_option_market import RyskOptionMarket
 from rysk_client.src.utils import (get_contract, get_logger, get_web3,
                                    print_operate_tuple)
 
 
 class Balances(Enum):
     """
     Class to represent the balances of an address.
@@ -370,28 +369,26 @@
         self,
         acceptable_premium: int,
         amount: int,
         otoken_address: str,
         collateral_amount: int,
         collateral_asset: str,
         vault_id: int,
-        rysk_option_market: RyskOptionMarket,
     ):
         """
         Build the transaction to close a short position.
         """
         operate_tuple = self._operation_factory.close_short(
             acceptable_premium=acceptable_premium,
             owner_address=self._crypto.address,  # type: ignore
             otoken_address=self.web3.toChecksumAddress(otoken_address),
             amount=int(amount),
             collateral_amount=int(collateral_amount),
             collateral_asset=collateral_asset,
             vault_id=vault_id,
-            rysk_option_market=rysk_option_market,
         )
         return self._operate(operate_tuple, self.option_exchange)
 
     def _operate(
         self,
         operate_tuple: List[Dict[str, Any]],
         contract: Contract,
```

### Comparing `rysk_client-0.2.8/PKG-INFO` & `rysk_client-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rysk-client
-Version: 0.2.8
+Version: 0.2.9
 Summary: 
 Author: 8baller
 Author-email: 8ball030@gmail.com
 Requires-Python: >=3.8,<=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

