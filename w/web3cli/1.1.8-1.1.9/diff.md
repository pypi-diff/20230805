# Comparing `tmp/web3cli-1.1.8.tar.gz` & `tmp/web3cli-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3cli-1.1.8.tar", last modified: Thu Jun 15 13:27:10 2023, max compression
+gzip compressed data, was "web3cli-1.1.9.tar", last modified: Thu Jun 15 15:50:37 2023, max compression
```

## Comparing `web3cli-1.1.8.tar` & `web3cli-1.1.9.tar`

### file list

```diff
@@ -1,176 +1,176 @@
--rw-r--r--   0        0        0     1069 2022-10-24 15:49:55.999119 web3cli-1.1.8/LICENSE
--rw-r--r--   0        0        0    12341 2023-06-12 19:34:10.821303 web3cli-1.1.8/README.md
--rw-r--r--   0        0        0     4057 2023-06-15 13:26:58.567557 web3cli-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     6148 2022-11-13 07:56:22.807127 web3cli-1.1.8/src/web3cli/.DS_Store
--rw-r--r--   0        0        0        0 2022-11-18 22:32:14.016225 web3cli-1.1.8/src/web3cli/__init__.py
--rw-r--r--   0        0        0        0 2022-10-24 15:34:40.198985 web3cli-1.1.8/src/web3cli/controllers/__init__.py
--rw-r--r--   0        0        0     4679 2023-06-10 16:49:18.164306 web3cli-1.1.8/src/web3cli/controllers/abi_controller.py
--rw-r--r--   0        0        0     2049 2023-06-10 16:26:02.765052 web3cli-1.1.8/src/web3cli/controllers/app_key_controller.py
--rw-r--r--   0        0        0     1215 2023-06-10 16:26:21.840704 web3cli-1.1.8/src/web3cli/controllers/base_controller.py
--rw-r--r--   0        0        0     3106 2023-06-10 17:02:35.846994 web3cli-1.1.8/src/web3cli/controllers/call_controller.py
--rw-r--r--   0        0        0     2421 2023-06-10 16:26:42.723101 web3cli-1.1.8/src/web3cli/controllers/config_controller.py
--rw-r--r--   0        0        0     1109 2022-12-17 18:21:46.704206 web3cli-1.1.8/src/web3cli/controllers/controller.py
--rw-r--r--   0        0        0        0 2023-03-25 21:06:13.922427 web3cli-1.1.8/src/web3cli/controllers/crud/__init__.py
--rw-r--r--   0        0        0     2530 2023-06-10 16:49:44.923130 web3cli-1.1.8/src/web3cli/controllers/crud/address_controller.py
--rw-r--r--   0        0        0     4413 2023-06-10 16:50:02.537767 web3cli-1.1.8/src/web3cli/controllers/crud/chain_controller.py
--rw-r--r--   0        0        0     4785 2023-06-10 16:50:16.263301 web3cli-1.1.8/src/web3cli/controllers/crud/contract_controller.py
--rw-r--r--   0        0        0     3035 2023-06-10 16:21:12.060981 web3cli-1.1.8/src/web3cli/controllers/crud/history_controller.py
--rw-r--r--   0        0        0     2972 2023-06-10 16:35:01.955138 web3cli-1.1.8/src/web3cli/controllers/crud/rpc_controller.py
--rw-r--r--   0        0        0     5282 2023-06-10 16:51:30.999842 web3cli-1.1.8/src/web3cli/controllers/crud/signer_controller.py
--rw-r--r--   0        0        0     1390 2023-06-10 16:27:14.395424 web3cli-1.1.8/src/web3cli/controllers/db_controller.py
--rw-r--r--   0        0        0     1010 2023-06-14 09:29:36.678332 web3cli-1.1.8/src/web3cli/controllers/debug_controller.py
--rw-r--r--   0        0        0     1479 2023-06-10 16:29:57.178158 web3cli-1.1.8/src/web3cli/controllers/keyfile_controller.py
--rw-r--r--   0        0        0     4153 2023-06-10 18:07:14.344855 web3cli-1.1.8/src/web3cli/controllers/misc_controller.py
--rw-r--r--   0        0        0     4471 2023-06-10 16:33:44.421618 web3cli-1.1.8/src/web3cli/controllers/replay_controller.py
--rw-r--r--   0        0        0     2403 2023-06-10 16:33:58.579948 web3cli-1.1.8/src/web3cli/controllers/send_controller.py
--rw-r--r--   0        0        0     7346 2023-06-15 13:26:24.428414 web3cli-1.1.8/src/web3cli/controllers/subscribe_controller.py
--rw-r--r--   0        0        0     6878 2023-05-20 18:17:47.046015 web3cli-1.1.8/src/web3cli/controllers/swap_controller.py
--rw-r--r--   0        0        0     7848 2023-06-10 17:57:16.099321 web3cli-1.1.8/src/web3cli/controllers/token_controller.py
--rw-r--r--   0        0        0     2862 2023-05-20 18:17:47.047364 web3cli-1.1.8/src/web3cli/controllers/transact_controller.py
--rw-r--r--   0        0        0     1239 2023-06-10 17:31:55.330976 web3cli-1.1.8/src/web3cli/controllers/tx_controller.py
--rw-r--r--   0        0        0      341 2023-05-20 18:17:47.049010 web3cli-1.1.8/src/web3cli/exceptions.py
--rw-r--r--   0        0        0     1329 2023-06-12 10:20:17.461216 web3cli-1.1.8/src/web3cli/framework/ext_print.py
--rw-r--r--   0        0        0        0 2022-10-24 15:34:40.191413 web3cli-1.1.8/src/web3cli/helpers/__init__.py
--rw-r--r--   0        0        0    18720 2023-06-14 10:16:26.890620 web3cli-1.1.8/src/web3cli/helpers/args.py
--rw-r--r--   0        0        0     2198 2023-05-20 18:17:47.051274 web3cli-1.1.8/src/web3cli/helpers/client_factory.py
--rw-r--r--   0        0        0     1252 2022-12-28 16:44:58.644508 web3cli-1.1.8/src/web3cli/helpers/config.py
--rw-r--r--   0        0        0     2092 2023-05-18 11:14:15.678582 web3cli-1.1.8/src/web3cli/helpers/crypto.py
--rw-r--r--   0        0        0     1228 2023-02-11 17:24:24.959766 web3cli-1.1.8/src/web3cli/helpers/database.py
--rw-r--r--   0        0        0     1776 2023-06-10 18:08:11.403330 web3cli-1.1.8/src/web3cli/helpers/render.py
--rw-r--r--   0        0        0     4548 2023-06-07 12:09:20.814550 web3cli-1.1.8/src/web3cli/helpers/send.py
--rw-r--r--   0        0        0     2178 2023-05-20 18:17:47.053233 web3cli-1.1.8/src/web3cli/helpers/signer.py
--rw-r--r--   0        0        0     1490 2023-06-14 09:30:55.241990 web3cli-1.1.8/src/web3cli/helpers/telegram.py
--rw-r--r--   0        0        0     2132 2023-06-07 12:22:03.729729 web3cli-1.1.8/src/web3cli/helpers/tx.py
--rw-r--r--   0        0        0      435 2023-06-15 13:26:41.473182 web3cli-1.1.8/src/web3cli/helpers/version.py
--rw-r--r--   0        0        0     2595 2023-02-12 21:33:06.910919 web3cli-1.1.8/src/web3cli/hooks.py
--rw-r--r--   0        0        0     7780 2023-06-14 06:02:23.829441 web3cli-1.1.8/src/web3cli/main.py
--rw-r--r--   0        0        0        0 2023-01-29 11:30:42.897043 web3cli-1.1.8/src/web3cli/templates/__init__.py
--rw-r--r--   0        0        0      243 2023-01-29 11:41:03.173746 web3cli-1.1.8/src/web3cli/templates/balance.jinja2
--rw-r--r--   0        0        0      120 2022-11-03 17:39:28.958124 web3cli-1.1.8/src/web3core/__init__.py
--rw-r--r--   0        0        0       72 2023-02-19 11:02:13.393953 web3cli-1.1.8/src/web3core/constants.py
--rw-r--r--   0        0        0       90 2023-01-18 19:29:57.558367 web3cli-1.1.8/src/web3core/db.py
--rw-r--r--   0        0        0     1762 2023-01-18 20:41:45.295870 web3cli-1.1.8/src/web3core/exceptions.py
--rw-r--r--   0        0        0        0 2022-11-03 17:39:28.958845 web3cli-1.1.8/src/web3core/helpers/__init__.py
--rw-r--r--   0        0        0     9448 2023-04-07 18:14:01.618698 web3cli-1.1.8/src/web3core/helpers/abi.py
--rw-r--r--   0        0        0     1148 2023-05-17 09:47:21.910041 web3cli-1.1.8/src/web3core/helpers/blocks.py
--rw-r--r--   0        0        0     3405 2023-05-20 18:17:47.055119 web3cli-1.1.8/src/web3core/helpers/client_factory.py
--rw-r--r--   0        0        0     1060 2022-12-17 18:21:46.707584 web3cli-1.1.8/src/web3core/helpers/crypto.py
--rw-r--r--   0        0        0      714 2023-02-11 17:32:11.986925 web3cli-1.1.8/src/web3core/helpers/database.py
--rw-r--r--   0        0        0     1582 2023-04-07 18:14:01.619156 web3cli-1.1.8/src/web3core/helpers/dex.py
--rw-r--r--   0        0        0      434 2022-12-19 20:01:36.985004 web3cli-1.1.8/src/web3core/helpers/format.py
--rw-r--r--   0        0        0     3460 2023-06-14 08:43:47.711951 web3cli-1.1.8/src/web3core/helpers/misc.py
--rw-r--r--   0        0        0      532 2022-12-16 06:48:29.391730 web3cli-1.1.8/src/web3core/helpers/os.py
--rw-r--r--   0        0        0     1799 2023-06-10 15:39:08.908650 web3cli-1.1.8/src/web3core/helpers/resolve.py
--rw-r--r--   0        0        0      827 2023-06-10 09:19:32.610030 web3cli-1.1.8/src/web3core/helpers/rpc.py
--rw-r--r--   0        0        0     2158 2023-01-14 21:27:16.459461 web3cli-1.1.8/src/web3core/helpers/seed.py
--rw-r--r--   0        0        0      786 2023-06-14 10:04:27.891523 web3cli-1.1.8/src/web3core/helpers/telegram.py
--rw-r--r--   0        0        0     4697 2023-04-07 18:14:01.620145 web3cli-1.1.8/src/web3core/helpers/tx.py
--rw-r--r--   0        0        0      553 2023-06-12 19:19:49.776790 web3cli-1.1.8/src/web3core/helpers/validation.py
--rw-r--r--   0        0        0     1207 2022-12-28 16:44:58.644659 web3cli-1.1.8/src/web3core/helpers/yaml.py
--rw-r--r--   0        0        0      424 2023-01-18 19:29:57.562778 web3cli-1.1.8/src/web3core/models/__init__.py
--rw-r--r--   0        0        0     1790 2023-01-18 19:29:57.563744 web3cli-1.1.8/src/web3core/models/address.py
--rw-r--r--   0        0        0     3433 2023-05-20 18:17:47.055757 web3cli-1.1.8/src/web3core/models/base_model.py
--rw-r--r--   0        0        0     4923 2023-03-25 21:22:51.453293 web3cli-1.1.8/src/web3core/models/chain.py
--rw-r--r--   0        0        0     4262 2023-05-31 08:53:51.850966 web3cli-1.1.8/src/web3core/models/contract.py
--rw-r--r--   0        0        0     1405 2023-05-18 09:25:11.305140 web3cli-1.1.8/src/web3core/models/signer.py
--rw-r--r--   0        0        0     1054 2022-12-28 16:44:59.161817 web3cli-1.1.8/src/web3core/models/timestamps_model.py
--rw-r--r--   0        0        0     2550 2022-12-28 16:44:59.162568 web3cli-1.1.8/src/web3core/models/tx.py
--rw-r--r--   0        0        0     1449 2023-01-18 19:29:57.566552 web3cli-1.1.8/src/web3core/models/types.py
--rw-r--r--   0        0        0       48 2022-11-18 22:43:37.360850 web3cli-1.1.8/src/web3core/seeds/__init__.py
--rw-r--r--   0        0        0     3164 2023-06-08 14:39:52.689918 web3cli-1.1.8/src/web3core/seeds/chain_seeds.py
--rw-r--r--   0        0        0      521 2023-06-08 14:37:27.133219 web3cli-1.1.8/src/web3core/seeds/contract_seeds.py
--rw-r--r--   0        0        0    49489 2023-02-19 09:09:21.024661 web3cli-1.1.8/src/web3core/seeds/contract_type_seeds.py
--rw-r--r--   0        0        0     9720 2023-02-27 16:48:07.675984 web3cli-1.1.8/src/web3core/seeds/contracts/arb_contract_seeds.py
--rw-r--r--   0        0        0     1881 2023-02-27 19:24:54.136969 web3cli-1.1.8/src/web3core/seeds/contracts/avax_contract_seeds.py
--rw-r--r--   0        0        0      867 2023-06-10 15:43:36.615089 web3cli-1.1.8/src/web3core/seeds/contracts/bnb_contract_seeds.py
--rw-r--r--   0        0        0      611 2023-05-25 15:43:35.647237 web3cli-1.1.8/src/web3core/seeds/contracts/era_contract_seeds.py
--rw-r--r--   0        0        0      997 2023-06-08 14:37:20.947238 web3cli-1.1.8/src/web3core/seeds/contracts/erat_contract_seeds.py
--rw-r--r--   0        0        0     1579 2023-02-27 16:48:24.467166 web3cli-1.1.8/src/web3core/seeds/contracts/eth_contract_seeds.py
--rw-r--r--   0        0        0     1183 2023-05-26 15:20:05.535496 web3cli-1.1.8/src/web3core/seeds/contracts/gno_contract_seeds.py
--rw-r--r--   0        0        0     1448 2023-02-19 10:37:03.165028 web3cli-1.1.8/src/web3core/types.py
--rw-r--r--   0        0        0     6148 2023-06-14 09:22:36.471274 web3cli-1.1.8/tests/.DS_Store
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.296564 web3cli-1.1.8/tests/__init__.py
--rw-r--r--   0        0        0    10244 2023-02-28 16:18:44.627516 web3cli-1.1.8/tests/ape/.DS_Store
--rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.934034 web3cli-1.1.8/tests/ape/.build/Factory_IERC20.json
--rw-r--r--   0        0        0      536 2023-04-06 17:43:03.934442 web3cli-1.1.8/tests/ape/.build/Factory_IUniswapV2Callee.json
--rw-r--r--   0        0        0     3605 2023-04-06 17:43:03.935802 web3cli-1.1.8/tests/ape/.build/Factory_IUniswapV2ERC20.json
--rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.936651 web3cli-1.1.8/tests/ape/.build/Factory_IUniswapV2Factory.json
--rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.938968 web3cli-1.1.8/tests/ape/.build/Factory_IUniswapV2Pair.json
--rw-r--r--   0        0        0      862 2023-04-06 17:43:03.939241 web3cli-1.1.8/tests/ape/.build/Factory_Math.json
--rw-r--r--   0        0        0      866 2023-04-06 17:43:03.939527 web3cli-1.1.8/tests/ape/.build/Factory_SafeMath.json
--rw-r--r--   0        0        0      867 2023-04-06 17:43:03.939780 web3cli-1.1.8/tests/ape/.build/Factory_UQ112x112.json
--rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.916870 web3cli-1.1.8/tests/ape/.build/Router_IERC20.json
--rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.917744 web3cli-1.1.8/tests/ape/.build/Router_IUniswapV2Factory.json
--rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.920204 web3cli-1.1.8/tests/ape/.build/Router_IUniswapV2Pair.json
--rw-r--r--   0        0        0     9213 2023-04-06 17:43:03.922797 web3cli-1.1.8/tests/ape/.build/Router_IUniswapV2Router01.json
--rw-r--r--   0        0        0    11845 2023-04-06 17:43:03.926066 web3cli-1.1.8/tests/ape/.build/Router_IUniswapV2Router02.json
--rw-r--r--   0        0        0      683 2023-04-06 17:43:03.926558 web3cli-1.1.8/tests/ape/.build/Router_IWETH.json
--rw-r--r--   0        0        0      872 2023-04-06 17:43:03.926867 web3cli-1.1.8/tests/ape/.build/Router_SafeMath.json
--rw-r--r--   0        0        0      879 2023-04-06 17:43:03.927162 web3cli-1.1.8/tests/ape/.build/Router_TransferHelper.json
--rw-r--r--   0        0        0      881 2023-04-06 17:43:03.927462 web3cli-1.1.8/tests/ape/.build/Router_UniswapV2Library.json
--rw-r--r--   0        0        0    14895 2023-04-06 17:43:03.932635 web3cli-1.1.8/tests/ape/.build/Token.json
--rw-r--r--   0        0        0      791 2023-04-06 17:43:03.932974 web3cli-1.1.8/tests/ape/.build/Token_SafeMath.json
--rw-r--r--   0        0        0    14014 2023-04-06 17:43:03.941015 web3cli-1.1.8/tests/ape/.build/UniswapV2ERC20.json
--rw-r--r--   0        0        0    46097 2023-04-06 17:43:03.942289 web3cli-1.1.8/tests/ape/.build/UniswapV2Factory.json
--rw-r--r--   0        0        0    44784 2023-04-06 17:43:03.944616 web3cli-1.1.8/tests/ape/.build/UniswapV2Pair.json
--rw-r--r--   0        0        0    85730 2023-04-06 17:43:03.931232 web3cli-1.1.8/tests/ape/.build/UniswapV2Router02.json
--rw-r--r--   0        0        0   324962 2023-06-15 13:27:03.206266 web3cli-1.1.8/tests/ape/.build/__local__.json
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.620721 web3cli-1.1.8/tests/ape/__init__.py
--rw-r--r--   0        0        0     6148 2023-02-28 16:18:44.554061 web3cli-1.1.8/tests/ape/contracts/.DS_Store
--rw-r--r--   0        0        0     4101 2023-04-07 18:14:01.621230 web3cli-1.1.8/tests/ape/contracts/token/Token.sol
--rw-r--r--   0        0        0      646 2023-04-07 18:14:01.621775 web3cli-1.1.8/tests/ape/contracts/token/Token_SafeMath.sol
--rw-r--r--   0        0        0     6148 2023-02-28 15:31:57.501753 web3cli-1.1.8/tests/ape/contracts/uniswap/.DS_Store
--rw-r--r--   0        0        0    21725 2023-04-07 18:14:01.622322 web3cli-1.1.8/tests/ape/contracts/uniswap/UniswapV2Factory.sol
--rw-r--r--   0        0        0    34078 2023-04-07 18:14:01.622848 web3cli-1.1.8/tests/ape/contracts/uniswap/UniswapV2Router02.sol
--rw-r--r--   0        0        0      236 2023-04-07 18:14:01.623357 web3cli-1.1.8/tests/ape/scripts/__init__.py
--rw-r--r--   0        0        0      347 2023-04-07 18:14:01.623719 web3cli-1.1.8/tests/ape/scripts/db.py
--rw-r--r--   0        0        0      200 2023-04-07 18:14:01.624050 web3cli-1.1.8/tests/ape/scripts/token.py
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624201 web3cli-1.1.8/tests/ape/tests/__init__.py
--rw-r--r--   0        0        0    13902 2023-04-07 18:14:01.624793 web3cli-1.1.8/tests/ape/tests/fixtures.py
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624997 web3cli-1.1.8/tests/ape/tests/helpers/__init__.py
--rw-r--r--   0        0        0      371 2023-04-07 18:14:01.625481 web3cli-1.1.8/tests/ape/tests/helpers/ape.py
--rw-r--r--   0        0        0      881 2023-04-07 18:14:01.625860 web3cli-1.1.8/tests/ape/tests/helpers/token.py
--rw-r--r--   0        0        0     3790 2023-04-07 18:14:01.626436 web3cli-1.1.8/tests/ape/tests/helpers/uniswap.py
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.626729 web3cli-1.1.8/tests/ape/tests/token/__init__.py
--rw-r--r--   0        0        0     1983 2023-04-07 18:14:01.627373 web3cli-1.1.8/tests/ape/tests/token/test_ape_token_approve.py
--rw-r--r--   0        0        0     2876 2023-04-07 18:14:01.627765 web3cli-1.1.8/tests/ape/tests/token/test_ape_token_transfer.py
--rw-r--r--   0        0        0     6467 2023-04-07 18:14:01.628071 web3cli-1.1.8/tests/ape/tests/token/test_ape_token_transferFrom.py
--rw-r--r--   0        0        0        0 2023-04-07 18:14:01.628193 web3cli-1.1.8/tests/ape/tests/uniswap/__init__.py
--rw-r--r--   0        0        0     4193 2023-04-07 18:14:01.628531 web3cli-1.1.8/tests/ape/tests/uniswap/test_ape_uniswap_v2_add_liquidity.py
--rw-r--r--   0        0        0      794 2023-04-07 18:14:01.628890 web3cli-1.1.8/tests/ape/tests/uniswap/test_ape_uniswap_v2_create_pair.py
--rw-r--r--   0        0        0      487 2023-04-07 18:14:01.629400 web3cli-1.1.8/tests/conftest.py
--rw-r--r--   0        0        0     1130 2023-04-07 12:55:47.114434 web3cli-1.1.8/tests/helper.py
--rw-r--r--   0        0        0     3240 2023-06-08 17:29:54.142209 web3cli-1.1.8/tests/seed.py
--rw-r--r--   0        0        0        0 2022-12-28 17:01:25.438908 web3cli-1.1.8/tests/web3cli/__init__.py
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.297637 web3cli-1.1.8/tests/web3cli/controllers/__init__.py
--rw-r--r--   0        0        0     3754 2023-05-20 18:17:47.056601 web3cli-1.1.8/tests/web3cli/controllers/crud/test_address_controller.py
--rw-r--r--   0        0        0     3510 2023-06-10 17:49:12.472139 web3cli-1.1.8/tests/web3cli/controllers/crud/test_chain_controller.py
--rw-r--r--   0        0        0     8222 2023-05-20 18:17:47.058165 web3cli-1.1.8/tests/web3cli/controllers/crud/test_contract_controller.py
--rw-r--r--   0        0        0     2870 2023-05-20 18:17:47.058996 web3cli-1.1.8/tests/web3cli/controllers/crud/test_history_controller.py
--rw-r--r--   0        0        0     3741 2023-06-10 17:49:22.329714 web3cli-1.1.8/tests/web3cli/controllers/crud/test_rpc_controller.py
--rw-r--r--   0        0        0     4912 2023-06-10 17:49:27.241897 web3cli-1.1.8/tests/web3cli/controllers/crud/test_signer_controller.py
--rw-r--r--   0        0        0     6497 2023-06-10 17:50:24.793662 web3cli-1.1.8/tests/web3cli/controllers/crud/test_token_controller.py
--rw-r--r--   0        0        0     1848 2023-05-18 10:32:19.351291 web3cli-1.1.8/tests/web3cli/controllers/test_appkey_controller.py
--rw-r--r--   0        0        0     6385 2023-06-10 17:54:02.470548 web3cli-1.1.8/tests/web3cli/controllers/test_call_controller.py
--rw-r--r--   0        0        0     1027 2023-06-10 17:47:40.979271 web3cli-1.1.8/tests/web3cli/controllers/test_db_controller.py
--rw-r--r--   0        0        0     1664 2023-06-10 18:03:21.873923 web3cli-1.1.8/tests/web3cli/controllers/test_keyfile_controller.py
--rw-r--r--   0        0        0     5779 2023-06-14 08:57:38.527992 web3cli-1.1.8/tests/web3cli/controllers/test_misc_controller.py
--rw-r--r--   0        0        0     1210 2023-06-07 17:12:04.381111 web3cli-1.1.8/tests/web3cli/controllers/test_replay_controller.py
--rw-r--r--   0        0        0     3415 2023-05-20 18:17:47.063638 web3cli-1.1.8/tests/web3cli/controllers/test_send_controller.py
--rw-r--r--   0        0        0     9593 2023-05-20 18:17:47.064509 web3cli-1.1.8/tests/web3cli/controllers/test_transact_controller.py
--rw-r--r--   0        0        0     1265 2023-06-07 17:10:04.508480 web3cli-1.1.8/tests/web3cli/controllers/test_tx_controller.py
--rw-r--r--   0        0        0     1293 2023-04-07 18:14:01.632176 web3cli-1.1.8/tests/web3cli/fixtures.py
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.303802 web3cli-1.1.8/tests/web3cli/helpers/__init__.py
--rw-r--r--   0        0        0      684 2022-12-28 17:00:06.651527 web3cli-1.1.8/tests/web3cli/helpers/test_crypto_helper.py
--rw-r--r--   0        0        0     1455 2023-02-12 12:11:39.416778 web3cli-1.1.8/tests/web3cli/main.py
--rw-r--r--   0        0        0     1171 2023-02-11 18:15:39.713968 web3cli-1.1.8/tests/web3cli/test_db.py
--rw-r--r--   0        0        0      393 2023-02-11 18:16:36.584225 web3cli-1.1.8/tests/web3cli/test_main.py
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301380 web3cli-1.1.8/tests/web3core/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-18 11:01:18.894137 web3cli-1.1.8/tests/web3core/fixtures.py
--rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301610 web3cli-1.1.8/tests/web3core/helpers/__init__.py
--rw-r--r--   0        0        0     8923 2023-01-28 12:36:51.002666 web3cli-1.1.8/tests/web3core/helpers/test_abi_helper.py
--rw-r--r--   0        0        0      528 2022-12-28 16:44:57.745951 web3cli-1.1.8/tests/web3core/helpers/test_crypto_helper.py
--rw-r--r--   0        0        0     4807 2023-02-19 09:09:21.027684 web3cli-1.1.8/tests/web3core/helpers/test_resolve_address_helper.py
--rw-r--r--   0        0        0     1022 2023-01-29 17:56:31.054122 web3cli-1.1.8/tests/web3core/helpers/test_validation_helper.py
--rw-r--r--   0        0        0     1783 2023-01-14 21:27:16.475375 web3cli-1.1.8/tests/web3core/models/test_contract_model.py
--rw-r--r--   0        0        0    12798 1970-01-01 00:00:00.000000 web3cli-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-10-24 15:49:55.999119 web3cli-1.1.9/LICENSE
+-rw-r--r--   0        0        0    12341 2023-06-12 19:34:10.821303 web3cli-1.1.9/README.md
+-rw-r--r--   0        0        0     4057 2023-06-15 15:50:29.047778 web3cli-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     6148 2022-11-13 07:56:22.807127 web3cli-1.1.9/src/web3cli/.DS_Store
+-rw-r--r--   0        0        0        0 2022-11-18 22:32:14.016225 web3cli-1.1.9/src/web3cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-24 15:34:40.198985 web3cli-1.1.9/src/web3cli/controllers/__init__.py
+-rw-r--r--   0        0        0     4679 2023-06-10 16:49:18.164306 web3cli-1.1.9/src/web3cli/controllers/abi_controller.py
+-rw-r--r--   0        0        0     2049 2023-06-10 16:26:02.765052 web3cli-1.1.9/src/web3cli/controllers/app_key_controller.py
+-rw-r--r--   0        0        0     1215 2023-06-10 16:26:21.840704 web3cli-1.1.9/src/web3cli/controllers/base_controller.py
+-rw-r--r--   0        0        0     3106 2023-06-10 17:02:35.846994 web3cli-1.1.9/src/web3cli/controllers/call_controller.py
+-rw-r--r--   0        0        0     2421 2023-06-10 16:26:42.723101 web3cli-1.1.9/src/web3cli/controllers/config_controller.py
+-rw-r--r--   0        0        0     1109 2022-12-17 18:21:46.704206 web3cli-1.1.9/src/web3cli/controllers/controller.py
+-rw-r--r--   0        0        0        0 2023-03-25 21:06:13.922427 web3cli-1.1.9/src/web3cli/controllers/crud/__init__.py
+-rw-r--r--   0        0        0     2530 2023-06-10 16:49:44.923130 web3cli-1.1.9/src/web3cli/controllers/crud/address_controller.py
+-rw-r--r--   0        0        0     4413 2023-06-10 16:50:02.537767 web3cli-1.1.9/src/web3cli/controllers/crud/chain_controller.py
+-rw-r--r--   0        0        0     4785 2023-06-10 16:50:16.263301 web3cli-1.1.9/src/web3cli/controllers/crud/contract_controller.py
+-rw-r--r--   0        0        0     3035 2023-06-10 16:21:12.060981 web3cli-1.1.9/src/web3cli/controllers/crud/history_controller.py
+-rw-r--r--   0        0        0     2972 2023-06-10 16:35:01.955138 web3cli-1.1.9/src/web3cli/controllers/crud/rpc_controller.py
+-rw-r--r--   0        0        0     5282 2023-06-10 16:51:30.999842 web3cli-1.1.9/src/web3cli/controllers/crud/signer_controller.py
+-rw-r--r--   0        0        0     1390 2023-06-10 16:27:14.395424 web3cli-1.1.9/src/web3cli/controllers/db_controller.py
+-rw-r--r--   0        0        0     1010 2023-06-14 09:29:36.678332 web3cli-1.1.9/src/web3cli/controllers/debug_controller.py
+-rw-r--r--   0        0        0     1479 2023-06-10 16:29:57.178158 web3cli-1.1.9/src/web3cli/controllers/keyfile_controller.py
+-rw-r--r--   0        0        0     4153 2023-06-10 18:07:14.344855 web3cli-1.1.9/src/web3cli/controllers/misc_controller.py
+-rw-r--r--   0        0        0     4471 2023-06-10 16:33:44.421618 web3cli-1.1.9/src/web3cli/controllers/replay_controller.py
+-rw-r--r--   0        0        0     2403 2023-06-10 16:33:58.579948 web3cli-1.1.9/src/web3cli/controllers/send_controller.py
+-rw-r--r--   0        0        0     7839 2023-06-15 15:32:43.279479 web3cli-1.1.9/src/web3cli/controllers/subscribe_controller.py
+-rw-r--r--   0        0        0     6878 2023-05-20 18:17:47.046015 web3cli-1.1.9/src/web3cli/controllers/swap_controller.py
+-rw-r--r--   0        0        0     8036 2023-06-15 15:48:09.549907 web3cli-1.1.9/src/web3cli/controllers/token_controller.py
+-rw-r--r--   0        0        0     2862 2023-05-20 18:17:47.047364 web3cli-1.1.9/src/web3cli/controllers/transact_controller.py
+-rw-r--r--   0        0        0     1239 2023-06-10 17:31:55.330976 web3cli-1.1.9/src/web3cli/controllers/tx_controller.py
+-rw-r--r--   0        0        0      341 2023-05-20 18:17:47.049010 web3cli-1.1.9/src/web3cli/exceptions.py
+-rw-r--r--   0        0        0     1329 2023-06-12 10:20:17.461216 web3cli-1.1.9/src/web3cli/framework/ext_print.py
+-rw-r--r--   0        0        0        0 2022-10-24 15:34:40.191413 web3cli-1.1.9/src/web3cli/helpers/__init__.py
+-rw-r--r--   0        0        0    18956 2023-06-15 14:56:32.866747 web3cli-1.1.9/src/web3cli/helpers/args.py
+-rw-r--r--   0        0        0     2198 2023-05-20 18:17:47.051274 web3cli-1.1.9/src/web3cli/helpers/client_factory.py
+-rw-r--r--   0        0        0     1252 2022-12-28 16:44:58.644508 web3cli-1.1.9/src/web3cli/helpers/config.py
+-rw-r--r--   0        0        0     2092 2023-05-18 11:14:15.678582 web3cli-1.1.9/src/web3cli/helpers/crypto.py
+-rw-r--r--   0        0        0     1228 2023-02-11 17:24:24.959766 web3cli-1.1.9/src/web3cli/helpers/database.py
+-rw-r--r--   0        0        0     1776 2023-06-10 18:08:11.403330 web3cli-1.1.9/src/web3cli/helpers/render.py
+-rw-r--r--   0        0        0     4548 2023-06-07 12:09:20.814550 web3cli-1.1.9/src/web3cli/helpers/send.py
+-rw-r--r--   0        0        0     2178 2023-05-20 18:17:47.053233 web3cli-1.1.9/src/web3cli/helpers/signer.py
+-rw-r--r--   0        0        0     1495 2023-06-15 15:32:59.212090 web3cli-1.1.9/src/web3cli/helpers/telegram.py
+-rw-r--r--   0        0        0     2132 2023-06-07 12:22:03.729729 web3cli-1.1.9/src/web3cli/helpers/tx.py
+-rw-r--r--   0        0        0      435 2023-06-15 13:26:41.473182 web3cli-1.1.9/src/web3cli/helpers/version.py
+-rw-r--r--   0        0        0     2595 2023-02-12 21:33:06.910919 web3cli-1.1.9/src/web3cli/hooks.py
+-rw-r--r--   0        0        0     7782 2023-06-15 14:45:13.341912 web3cli-1.1.9/src/web3cli/main.py
+-rw-r--r--   0        0        0        0 2023-01-29 11:30:42.897043 web3cli-1.1.9/src/web3cli/templates/__init__.py
+-rw-r--r--   0        0        0      243 2023-01-29 11:41:03.173746 web3cli-1.1.9/src/web3cli/templates/balance.jinja2
+-rw-r--r--   0        0        0      120 2022-11-03 17:39:28.958124 web3cli-1.1.9/src/web3core/__init__.py
+-rw-r--r--   0        0        0       72 2023-02-19 11:02:13.393953 web3cli-1.1.9/src/web3core/constants.py
+-rw-r--r--   0        0        0       90 2023-01-18 19:29:57.558367 web3cli-1.1.9/src/web3core/db.py
+-rw-r--r--   0        0        0     1762 2023-01-18 20:41:45.295870 web3cli-1.1.9/src/web3core/exceptions.py
+-rw-r--r--   0        0        0        0 2022-11-03 17:39:28.958845 web3cli-1.1.9/src/web3core/helpers/__init__.py
+-rw-r--r--   0        0        0     9448 2023-04-07 18:14:01.618698 web3cli-1.1.9/src/web3core/helpers/abi.py
+-rw-r--r--   0        0        0     1148 2023-05-17 09:47:21.910041 web3cli-1.1.9/src/web3core/helpers/blocks.py
+-rw-r--r--   0        0        0     3405 2023-05-20 18:17:47.055119 web3cli-1.1.9/src/web3core/helpers/client_factory.py
+-rw-r--r--   0        0        0     1060 2022-12-17 18:21:46.707584 web3cli-1.1.9/src/web3core/helpers/crypto.py
+-rw-r--r--   0        0        0      714 2023-02-11 17:32:11.986925 web3cli-1.1.9/src/web3core/helpers/database.py
+-rw-r--r--   0        0        0     1582 2023-04-07 18:14:01.619156 web3cli-1.1.9/src/web3core/helpers/dex.py
+-rw-r--r--   0        0        0      434 2022-12-19 20:01:36.985004 web3cli-1.1.9/src/web3core/helpers/format.py
+-rw-r--r--   0        0        0     3460 2023-06-14 08:43:47.711951 web3cli-1.1.9/src/web3core/helpers/misc.py
+-rw-r--r--   0        0        0      532 2022-12-16 06:48:29.391730 web3cli-1.1.9/src/web3core/helpers/os.py
+-rw-r--r--   0        0        0     1799 2023-06-10 15:39:08.908650 web3cli-1.1.9/src/web3core/helpers/resolve.py
+-rw-r--r--   0        0        0      827 2023-06-10 09:19:32.610030 web3cli-1.1.9/src/web3core/helpers/rpc.py
+-rw-r--r--   0        0        0     2158 2023-01-14 21:27:16.459461 web3cli-1.1.9/src/web3core/helpers/seed.py
+-rw-r--r--   0        0        0      786 2023-06-14 10:04:27.891523 web3cli-1.1.9/src/web3core/helpers/telegram.py
+-rw-r--r--   0        0        0     4697 2023-04-07 18:14:01.620145 web3cli-1.1.9/src/web3core/helpers/tx.py
+-rw-r--r--   0        0        0      553 2023-06-12 19:19:49.776790 web3cli-1.1.9/src/web3core/helpers/validation.py
+-rw-r--r--   0        0        0     1207 2022-12-28 16:44:58.644659 web3cli-1.1.9/src/web3core/helpers/yaml.py
+-rw-r--r--   0        0        0      424 2023-01-18 19:29:57.562778 web3cli-1.1.9/src/web3core/models/__init__.py
+-rw-r--r--   0        0        0     1790 2023-01-18 19:29:57.563744 web3cli-1.1.9/src/web3core/models/address.py
+-rw-r--r--   0        0        0     3433 2023-05-20 18:17:47.055757 web3cli-1.1.9/src/web3core/models/base_model.py
+-rw-r--r--   0        0        0     4923 2023-03-25 21:22:51.453293 web3cli-1.1.9/src/web3core/models/chain.py
+-rw-r--r--   0        0        0     4262 2023-05-31 08:53:51.850966 web3cli-1.1.9/src/web3core/models/contract.py
+-rw-r--r--   0        0        0     1405 2023-05-18 09:25:11.305140 web3cli-1.1.9/src/web3core/models/signer.py
+-rw-r--r--   0        0        0     1054 2022-12-28 16:44:59.161817 web3cli-1.1.9/src/web3core/models/timestamps_model.py
+-rw-r--r--   0        0        0     2550 2022-12-28 16:44:59.162568 web3cli-1.1.9/src/web3core/models/tx.py
+-rw-r--r--   0        0        0     1449 2023-01-18 19:29:57.566552 web3cli-1.1.9/src/web3core/models/types.py
+-rw-r--r--   0        0        0       48 2022-11-18 22:43:37.360850 web3cli-1.1.9/src/web3core/seeds/__init__.py
+-rw-r--r--   0        0        0     3164 2023-06-08 14:39:52.689918 web3cli-1.1.9/src/web3core/seeds/chain_seeds.py
+-rw-r--r--   0        0        0      521 2023-06-08 14:37:27.133219 web3cli-1.1.9/src/web3core/seeds/contract_seeds.py
+-rw-r--r--   0        0        0    49489 2023-02-19 09:09:21.024661 web3cli-1.1.9/src/web3core/seeds/contract_type_seeds.py
+-rw-r--r--   0        0        0     9720 2023-02-27 16:48:07.675984 web3cli-1.1.9/src/web3core/seeds/contracts/arb_contract_seeds.py
+-rw-r--r--   0        0        0     1881 2023-02-27 19:24:54.136969 web3cli-1.1.9/src/web3core/seeds/contracts/avax_contract_seeds.py
+-rw-r--r--   0        0        0      867 2023-06-10 15:43:36.615089 web3cli-1.1.9/src/web3core/seeds/contracts/bnb_contract_seeds.py
+-rw-r--r--   0        0        0      611 2023-05-25 15:43:35.647237 web3cli-1.1.9/src/web3core/seeds/contracts/era_contract_seeds.py
+-rw-r--r--   0        0        0      997 2023-06-08 14:37:20.947238 web3cli-1.1.9/src/web3core/seeds/contracts/erat_contract_seeds.py
+-rw-r--r--   0        0        0     1579 2023-02-27 16:48:24.467166 web3cli-1.1.9/src/web3core/seeds/contracts/eth_contract_seeds.py
+-rw-r--r--   0        0        0     1183 2023-05-26 15:20:05.535496 web3cli-1.1.9/src/web3core/seeds/contracts/gno_contract_seeds.py
+-rw-r--r--   0        0        0     1448 2023-02-19 10:37:03.165028 web3cli-1.1.9/src/web3core/types.py
+-rw-r--r--   0        0        0     6148 2023-06-14 09:22:36.471274 web3cli-1.1.9/tests/.DS_Store
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.296564 web3cli-1.1.9/tests/__init__.py
+-rw-r--r--   0        0        0    10244 2023-02-28 16:18:44.627516 web3cli-1.1.9/tests/ape/.DS_Store
+-rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.934034 web3cli-1.1.9/tests/ape/.build/Factory_IERC20.json
+-rw-r--r--   0        0        0      536 2023-04-06 17:43:03.934442 web3cli-1.1.9/tests/ape/.build/Factory_IUniswapV2Callee.json
+-rw-r--r--   0        0        0     3605 2023-04-06 17:43:03.935802 web3cli-1.1.9/tests/ape/.build/Factory_IUniswapV2ERC20.json
+-rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.936651 web3cli-1.1.9/tests/ape/.build/Factory_IUniswapV2Factory.json
+-rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.938968 web3cli-1.1.9/tests/ape/.build/Factory_IUniswapV2Pair.json
+-rw-r--r--   0        0        0      862 2023-04-06 17:43:03.939241 web3cli-1.1.9/tests/ape/.build/Factory_Math.json
+-rw-r--r--   0        0        0      866 2023-04-06 17:43:03.939527 web3cli-1.1.9/tests/ape/.build/Factory_SafeMath.json
+-rw-r--r--   0        0        0      867 2023-04-06 17:43:03.939780 web3cli-1.1.9/tests/ape/.build/Factory_UQ112x112.json
+-rw-r--r--   0        0        0     2609 2023-04-06 17:43:03.916870 web3cli-1.1.9/tests/ape/.build/Router_IERC20.json
+-rw-r--r--   0        0        0     2026 2023-04-06 17:43:03.917744 web3cli-1.1.9/tests/ape/.build/Router_IUniswapV2Factory.json
+-rw-r--r--   0        0        0     7527 2023-04-06 17:43:03.920204 web3cli-1.1.9/tests/ape/.build/Router_IUniswapV2Pair.json
+-rw-r--r--   0        0        0     9213 2023-04-06 17:43:03.922797 web3cli-1.1.9/tests/ape/.build/Router_IUniswapV2Router01.json
+-rw-r--r--   0        0        0    11845 2023-04-06 17:43:03.926066 web3cli-1.1.9/tests/ape/.build/Router_IUniswapV2Router02.json
+-rw-r--r--   0        0        0      683 2023-04-06 17:43:03.926558 web3cli-1.1.9/tests/ape/.build/Router_IWETH.json
+-rw-r--r--   0        0        0      872 2023-04-06 17:43:03.926867 web3cli-1.1.9/tests/ape/.build/Router_SafeMath.json
+-rw-r--r--   0        0        0      879 2023-04-06 17:43:03.927162 web3cli-1.1.9/tests/ape/.build/Router_TransferHelper.json
+-rw-r--r--   0        0        0      881 2023-04-06 17:43:03.927462 web3cli-1.1.9/tests/ape/.build/Router_UniswapV2Library.json
+-rw-r--r--   0        0        0    14895 2023-04-06 17:43:03.932635 web3cli-1.1.9/tests/ape/.build/Token.json
+-rw-r--r--   0        0        0      791 2023-04-06 17:43:03.932974 web3cli-1.1.9/tests/ape/.build/Token_SafeMath.json
+-rw-r--r--   0        0        0    14014 2023-04-06 17:43:03.941015 web3cli-1.1.9/tests/ape/.build/UniswapV2ERC20.json
+-rw-r--r--   0        0        0    46097 2023-04-06 17:43:03.942289 web3cli-1.1.9/tests/ape/.build/UniswapV2Factory.json
+-rw-r--r--   0        0        0    44784 2023-04-06 17:43:03.944616 web3cli-1.1.9/tests/ape/.build/UniswapV2Pair.json
+-rw-r--r--   0        0        0    85730 2023-04-06 17:43:03.931232 web3cli-1.1.9/tests/ape/.build/UniswapV2Router02.json
+-rw-r--r--   0        0        0   324962 2023-06-15 15:50:33.687168 web3cli-1.1.9/tests/ape/.build/__local__.json
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.620721 web3cli-1.1.9/tests/ape/__init__.py
+-rw-r--r--   0        0        0     6148 2023-02-28 16:18:44.554061 web3cli-1.1.9/tests/ape/contracts/.DS_Store
+-rw-r--r--   0        0        0     4101 2023-04-07 18:14:01.621230 web3cli-1.1.9/tests/ape/contracts/token/Token.sol
+-rw-r--r--   0        0        0      646 2023-04-07 18:14:01.621775 web3cli-1.1.9/tests/ape/contracts/token/Token_SafeMath.sol
+-rw-r--r--   0        0        0     6148 2023-02-28 15:31:57.501753 web3cli-1.1.9/tests/ape/contracts/uniswap/.DS_Store
+-rw-r--r--   0        0        0    21725 2023-04-07 18:14:01.622322 web3cli-1.1.9/tests/ape/contracts/uniswap/UniswapV2Factory.sol
+-rw-r--r--   0        0        0    34078 2023-04-07 18:14:01.622848 web3cli-1.1.9/tests/ape/contracts/uniswap/UniswapV2Router02.sol
+-rw-r--r--   0        0        0      236 2023-04-07 18:14:01.623357 web3cli-1.1.9/tests/ape/scripts/__init__.py
+-rw-r--r--   0        0        0      347 2023-04-07 18:14:01.623719 web3cli-1.1.9/tests/ape/scripts/db.py
+-rw-r--r--   0        0        0      200 2023-04-07 18:14:01.624050 web3cli-1.1.9/tests/ape/scripts/token.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624201 web3cli-1.1.9/tests/ape/tests/__init__.py
+-rw-r--r--   0        0        0    13902 2023-04-07 18:14:01.624793 web3cli-1.1.9/tests/ape/tests/fixtures.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.624997 web3cli-1.1.9/tests/ape/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      371 2023-04-07 18:14:01.625481 web3cli-1.1.9/tests/ape/tests/helpers/ape.py
+-rw-r--r--   0        0        0      881 2023-04-07 18:14:01.625860 web3cli-1.1.9/tests/ape/tests/helpers/token.py
+-rw-r--r--   0        0        0     3790 2023-04-07 18:14:01.626436 web3cli-1.1.9/tests/ape/tests/helpers/uniswap.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.626729 web3cli-1.1.9/tests/ape/tests/token/__init__.py
+-rw-r--r--   0        0        0     1983 2023-04-07 18:14:01.627373 web3cli-1.1.9/tests/ape/tests/token/test_ape_token_approve.py
+-rw-r--r--   0        0        0     2876 2023-04-07 18:14:01.627765 web3cli-1.1.9/tests/ape/tests/token/test_ape_token_transfer.py
+-rw-r--r--   0        0        0     6467 2023-04-07 18:14:01.628071 web3cli-1.1.9/tests/ape/tests/token/test_ape_token_transferFrom.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:14:01.628193 web3cli-1.1.9/tests/ape/tests/uniswap/__init__.py
+-rw-r--r--   0        0        0     4193 2023-04-07 18:14:01.628531 web3cli-1.1.9/tests/ape/tests/uniswap/test_ape_uniswap_v2_add_liquidity.py
+-rw-r--r--   0        0        0      794 2023-04-07 18:14:01.628890 web3cli-1.1.9/tests/ape/tests/uniswap/test_ape_uniswap_v2_create_pair.py
+-rw-r--r--   0        0        0      487 2023-04-07 18:14:01.629400 web3cli-1.1.9/tests/conftest.py
+-rw-r--r--   0        0        0     1130 2023-04-07 12:55:47.114434 web3cli-1.1.9/tests/helper.py
+-rw-r--r--   0        0        0     3240 2023-06-08 17:29:54.142209 web3cli-1.1.9/tests/seed.py
+-rw-r--r--   0        0        0        0 2022-12-28 17:01:25.438908 web3cli-1.1.9/tests/web3cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.297637 web3cli-1.1.9/tests/web3cli/controllers/__init__.py
+-rw-r--r--   0        0        0     3754 2023-05-20 18:17:47.056601 web3cli-1.1.9/tests/web3cli/controllers/crud/test_address_controller.py
+-rw-r--r--   0        0        0     3510 2023-06-10 17:49:12.472139 web3cli-1.1.9/tests/web3cli/controllers/crud/test_chain_controller.py
+-rw-r--r--   0        0        0     8222 2023-05-20 18:17:47.058165 web3cli-1.1.9/tests/web3cli/controllers/crud/test_contract_controller.py
+-rw-r--r--   0        0        0     2870 2023-05-20 18:17:47.058996 web3cli-1.1.9/tests/web3cli/controllers/crud/test_history_controller.py
+-rw-r--r--   0        0        0     3741 2023-06-10 17:49:22.329714 web3cli-1.1.9/tests/web3cli/controllers/crud/test_rpc_controller.py
+-rw-r--r--   0        0        0     4912 2023-06-10 17:49:27.241897 web3cli-1.1.9/tests/web3cli/controllers/crud/test_signer_controller.py
+-rw-r--r--   0        0        0     6497 2023-06-10 17:50:24.793662 web3cli-1.1.9/tests/web3cli/controllers/crud/test_token_controller.py
+-rw-r--r--   0        0        0     1848 2023-05-18 10:32:19.351291 web3cli-1.1.9/tests/web3cli/controllers/test_appkey_controller.py
+-rw-r--r--   0        0        0     6385 2023-06-10 17:54:02.470548 web3cli-1.1.9/tests/web3cli/controllers/test_call_controller.py
+-rw-r--r--   0        0        0     1027 2023-06-10 17:47:40.979271 web3cli-1.1.9/tests/web3cli/controllers/test_db_controller.py
+-rw-r--r--   0        0        0     1664 2023-06-10 18:03:21.873923 web3cli-1.1.9/tests/web3cli/controllers/test_keyfile_controller.py
+-rw-r--r--   0        0        0     5779 2023-06-14 08:57:38.527992 web3cli-1.1.9/tests/web3cli/controllers/test_misc_controller.py
+-rw-r--r--   0        0        0     1210 2023-06-07 17:12:04.381111 web3cli-1.1.9/tests/web3cli/controllers/test_replay_controller.py
+-rw-r--r--   0        0        0     3415 2023-05-20 18:17:47.063638 web3cli-1.1.9/tests/web3cli/controllers/test_send_controller.py
+-rw-r--r--   0        0        0     9593 2023-05-20 18:17:47.064509 web3cli-1.1.9/tests/web3cli/controllers/test_transact_controller.py
+-rw-r--r--   0        0        0     1265 2023-06-07 17:10:04.508480 web3cli-1.1.9/tests/web3cli/controllers/test_tx_controller.py
+-rw-r--r--   0        0        0     1293 2023-04-07 18:14:01.632176 web3cli-1.1.9/tests/web3cli/fixtures.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.303802 web3cli-1.1.9/tests/web3cli/helpers/__init__.py
+-rw-r--r--   0        0        0      684 2022-12-28 17:00:06.651527 web3cli-1.1.9/tests/web3cli/helpers/test_crypto_helper.py
+-rw-r--r--   0        0        0     1455 2023-02-12 12:11:39.416778 web3cli-1.1.9/tests/web3cli/main.py
+-rw-r--r--   0        0        0     1171 2023-02-11 18:15:39.713968 web3cli-1.1.9/tests/web3cli/test_db.py
+-rw-r--r--   0        0        0      393 2023-02-11 18:16:36.584225 web3cli-1.1.9/tests/web3cli/test_main.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301380 web3cli-1.1.9/tests/web3core/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-18 11:01:18.894137 web3cli-1.1.9/tests/web3core/fixtures.py
+-rw-r--r--   0        0        0        0 2022-11-10 21:50:51.301610 web3cli-1.1.9/tests/web3core/helpers/__init__.py
+-rw-r--r--   0        0        0     8923 2023-01-28 12:36:51.002666 web3cli-1.1.9/tests/web3core/helpers/test_abi_helper.py
+-rw-r--r--   0        0        0      528 2022-12-28 16:44:57.745951 web3cli-1.1.9/tests/web3core/helpers/test_crypto_helper.py
+-rw-r--r--   0        0        0     4807 2023-02-19 09:09:21.027684 web3cli-1.1.9/tests/web3core/helpers/test_resolve_address_helper.py
+-rw-r--r--   0        0        0     1022 2023-01-29 17:56:31.054122 web3cli-1.1.9/tests/web3core/helpers/test_validation_helper.py
+-rw-r--r--   0        0        0     1783 2023-01-14 21:27:16.475375 web3cli-1.1.9/tests/web3core/models/test_contract_model.py
+-rw-r--r--   0        0        0    12798 1970-01-01 00:00:00.000000 web3cli-1.1.9/PKG-INFO
```

### Comparing `web3cli-1.1.8/LICENSE` & `web3cli-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/README.md` & `web3cli-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/pyproject.toml` & `web3cli-1.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "web3cli"
-version = "1.1.8"
+version = "1.1.9"
 description = "Interact with blockchains and smart contracts using the command line"
 authors = [
     { name = "coccoinomane", email = "coccoinomane@gmail.com" },
 ]
 readme = "README.md"
 keywords = [
     "web3",
```

### Comparing `web3cli-1.1.8/src/web3cli/.DS_Store` & `web3cli-1.1.9/src/web3cli/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/controllers/abi_controller.py` & `web3cli-1.1.9/src/web3cli/controllers/abi_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/controllers/app_key_controller.py` & `web3cli-1.1.9/src/web3cli/controllers/app_key_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/controllers/base_controller.py` & `web3cli-1.1.9/src/web3cli/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/controllers/call_controller.py` & `web3cli-1.1.9/src/web3cli/controllers/call_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/controllers/config_controller.py` & `web3cli-1.1.9/src/web3cli/controllers/config_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/controllers/controller.py` & `web3cli-1.1.9/src/web3cli/controllers/controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/controllers/crud/address_controller.py` & `web3cli-1.1.9/src/web3cli/controllers/crud/address_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/controllers/crud/chain_controller.py` & `web3cli-1.1.9/src/web3cli/controllers/crud/chain_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/controllers/crud/contract_controller.py` & `web3cli-1.1.9/src/web3cli/controllers/crud/contract_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/controllers/crud/history_controller.py` & `web3cli-1.1.9/src/web3cli/controllers/crud/history_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/controllers/crud/rpc_controller.py` & `web3cli-1.1.9/src/web3cli/controllers/crud/rpc_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/controllers/crud/signer_controller.py` & `web3cli-1.1.9/src/web3cli/controllers/crud/signer_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/controllers/db_controller.py` & `web3cli-1.1.9/src/web3cli/controllers/db_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/controllers/debug_controller.py` & `web3cli-1.1.9/src/web3cli/controllers/debug_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/controllers/keyfile_controller.py` & `web3cli-1.1.9/src/web3cli/controllers/keyfile_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/controllers/misc_controller.py` & `web3cli-1.1.9/src/web3cli/controllers/misc_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/controllers/replay_controller.py` & `web3cli-1.1.9/src/web3cli/controllers/replay_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/controllers/send_controller.py` & `web3cli-1.1.9/src/web3cli/controllers/send_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/controllers/subscribe_controller.py` & `web3cli-1.1.9/src/web3cli/controllers/subscribe_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -178,15 +178,25 @@
                     silent=self.app.pargs.silent,
                 )
             # POST CALLBACK
             if self.app.pargs.post:
                 url = self.app.pargs.post[0]
                 if not is_valid_url(url):
                     raise Web3CliError(f"Invalid URL: {url}")
-                requests.post(
+                payload = {
+                    "notification_data": data,
+                    "notification_type": sub_type,
+                    "tx_data": tx,
+                }
+                response = requests.post(
                     url=url,
-                    data=json.dumps(data),
+                    data=json.dumps(payload),
                     headers={"Content-Type": "application/json"},
                     timeout=self.app.config.get("web3cli", "post_callback_timeout"),
                 )
+                self.app.log.debug(f"POST callback response: {response.text}")
+                if response.status_code != 200:
+                    self.app.log.error(
+                        f"POST callback failed with code {response.status_code} and response: {response.text}"
+                    )
 
         return callback
```

### Comparing `web3cli-1.1.8/src/web3cli/controllers/swap_controller.py` & `web3cli-1.1.9/src/web3cli/controllers/swap_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/controllers/token_controller.py` & `web3cli-1.1.9/src/web3cli/controllers/token_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 class TokenController(Controller):
     """Handler of the `w3 token` command"""
 
     class Meta:
         label = "token"
-        help = "transfer and approve tokens"
+        help = "interact with ERC20 tokens"
         stacked_type = "nested"
         stacked_on = "base"
 
     @ex(
         help="Approve the given spender to spend the given amount of tokens",
         arguments=[
             (["token"], {"help": "Token to approve"}),
@@ -130,14 +130,18 @@
         # Initialize client
         client = make_contract_client(self.app, self.app.pargs.token)
         decimals = client.functions["decimals"]().call()
         allowance_in_wei = client.functions["allowance"](owner, spender).call()
         allowance = allowance_in_wei / 10**decimals
         render(self.app, allowance)
 
+    @ex(help="Transfer tokens.  Not implemented yet.  Use `w3 send` instead.")
+    def transfer(self) -> None:
+        self.app.log.warning("Not implemented yet.  Use `w3 send` instead.")
+
     #    ____                      _
     #   / ___|  _ __   _   _    __| |
     #  | |     | '__| | | | |  / _` |
     #  | |___  | |    | |_| | | (_| |
     #   \____| |_|     \__,_|  \__,_|
 
     @ex(
```

### Comparing `web3cli-1.1.8/src/web3cli/controllers/transact_controller.py` & `web3cli-1.1.9/src/web3cli/controllers/transact_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/controllers/tx_controller.py` & `web3cli-1.1.9/src/web3cli/controllers/tx_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/framework/ext_print.py` & `web3cli-1.1.9/src/web3cli/framework/ext_print.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/helpers/args.py` & `web3cli-1.1.9/src/web3cli/helpers/args.py`

 * *Files 2% similar despite different names*

```diff
@@ -506,16 +506,20 @@
     )
 
 
 def subscribe_post(
     *name_or_flags: str, **kwargs: Any
 ) -> Tuple[List[str], dict[str, Any]]:
     return (
-        list(name_or_flags) or ["--post"],
-        {"help": "Send post notifications to this URL", "nargs": 1} | kwargs,
+        list(name_or_flags) or ["--post", "--webhook"],
+        {
+            "help": "Send a post notifications to this URL.  The body will be a JSON with fields: notification_data, notification_type and tx_data.  The latter field will be populated only when the --senders/--from argument is provided.",
+            "nargs": 1,
+        }
+        | kwargs,
     )
 
 
 def subscribe_print(
     *name_or_flags: str, **kwargs: Any
 ) -> Tuple[List[str], dict[str, Any]]:
     return (
```

### Comparing `web3cli-1.1.8/src/web3cli/helpers/client_factory.py` & `web3cli-1.1.9/src/web3cli/helpers/client_factory.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/helpers/config.py` & `web3cli-1.1.9/src/web3cli/helpers/config.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/helpers/crypto.py` & `web3cli-1.1.9/src/web3cli/helpers/crypto.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/helpers/database.py` & `web3cli-1.1.9/src/web3cli/helpers/database.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/helpers/render.py` & `web3cli-1.1.9/src/web3cli/helpers/render.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/helpers/send.py` & `web3cli-1.1.9/src/web3cli/helpers/send.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/helpers/signer.py` & `web3cli-1.1.9/src/web3cli/helpers/signer.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/helpers/telegram.py` & `web3cli-1.1.9/src/web3cli/helpers/telegram.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         The recipient chat or user.  If not provided, it will be read from the config.
     silent : bool
         Send a silent, so that it doesn't make the phone vibrate or make a sound.
     """
 
     api_key = app.config.get("web3cli", "telegram_api_key")
     chat_id = chat_id or app.config.get("web3cli", "telegram_chat_id")
-    timeout = app.config.get("web3cli", "telegram_send_timeout") or 5
+    timeout = int(app.config.get("web3cli", "telegram_send_timeout")) or 5
 
     if not api_key or not chat_id:
         raise Web3CliError(
             "Please set your Telegram API key and chat ID using `w3 config set telegram_api_key <api_key>` and `w3 config set telegram_chat_id <chat_id>``"
         )
 
     notification_result = False
```

### Comparing `web3cli-1.1.8/src/web3cli/helpers/tx.py` & `web3cli-1.1.9/src/web3cli/helpers/tx.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/hooks.py` & `web3cli-1.1.9/src/web3cli/hooks.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3cli/main.py` & `web3cli-1.1.9/src/web3cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,16 @@
         os.path.expanduser("~"), ".web3cli", "database", "web3cli.sqlite"
     ),
     "populate_db": True,
     "output_table_format": "fancy_grid",
     "output_table_wrap": 33,
     "telegram_api_key": "",
     "telegram_chat_id": "",
-    "telegram_send_timeout": 5,
-    "post_callback_timeout": 5,
+    "telegram_send_timeout": 15,
+    "post_callback_timeout": 15,
 }
 
 
 class Web3Cli(App):
     """Web3 Cli primary application."""
 
     class Meta:
```

### Comparing `web3cli-1.1.8/src/web3core/exceptions.py` & `web3cli-1.1.9/src/web3core/exceptions.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/helpers/abi.py` & `web3cli-1.1.9/src/web3core/helpers/abi.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/helpers/blocks.py` & `web3cli-1.1.9/src/web3core/helpers/blocks.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/helpers/client_factory.py` & `web3cli-1.1.9/src/web3core/helpers/client_factory.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/helpers/crypto.py` & `web3cli-1.1.9/src/web3core/helpers/crypto.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/helpers/database.py` & `web3cli-1.1.9/src/web3core/helpers/database.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/helpers/dex.py` & `web3cli-1.1.9/src/web3core/helpers/dex.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/helpers/misc.py` & `web3cli-1.1.9/src/web3core/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/helpers/os.py` & `web3cli-1.1.9/src/web3core/helpers/os.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/helpers/resolve.py` & `web3cli-1.1.9/src/web3core/helpers/resolve.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/helpers/rpc.py` & `web3cli-1.1.9/src/web3core/helpers/rpc.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/helpers/seed.py` & `web3cli-1.1.9/src/web3core/helpers/seed.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/helpers/telegram.py` & `web3cli-1.1.9/src/web3core/helpers/telegram.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/helpers/tx.py` & `web3cli-1.1.9/src/web3core/helpers/tx.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/helpers/validation.py` & `web3cli-1.1.9/src/web3core/helpers/validation.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/helpers/yaml.py` & `web3cli-1.1.9/src/web3core/helpers/yaml.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/models/address.py` & `web3cli-1.1.9/src/web3core/models/address.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/models/base_model.py` & `web3cli-1.1.9/src/web3core/models/base_model.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/models/chain.py` & `web3cli-1.1.9/src/web3core/models/chain.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/models/contract.py` & `web3cli-1.1.9/src/web3core/models/contract.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/models/signer.py` & `web3cli-1.1.9/src/web3core/models/signer.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/models/timestamps_model.py` & `web3cli-1.1.9/src/web3core/models/timestamps_model.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/models/tx.py` & `web3cli-1.1.9/src/web3core/models/tx.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/models/types.py` & `web3cli-1.1.9/src/web3core/models/types.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/seeds/chain_seeds.py` & `web3cli-1.1.9/src/web3core/seeds/chain_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/seeds/contract_seeds.py` & `web3cli-1.1.9/src/web3core/seeds/contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/seeds/contract_type_seeds.py` & `web3cli-1.1.9/src/web3core/seeds/contract_type_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/seeds/contracts/arb_contract_seeds.py` & `web3cli-1.1.9/src/web3core/seeds/contracts/arb_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/seeds/contracts/avax_contract_seeds.py` & `web3cli-1.1.9/src/web3core/seeds/contracts/avax_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/seeds/contracts/bnb_contract_seeds.py` & `web3cli-1.1.9/src/web3core/seeds/contracts/bnb_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/seeds/contracts/era_contract_seeds.py` & `web3cli-1.1.9/src/web3core/seeds/contracts/era_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/seeds/contracts/erat_contract_seeds.py` & `web3cli-1.1.9/src/web3core/seeds/contracts/erat_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/seeds/contracts/eth_contract_seeds.py` & `web3cli-1.1.9/src/web3core/seeds/contracts/eth_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/seeds/contracts/gno_contract_seeds.py` & `web3cli-1.1.9/src/web3core/seeds/contracts/gno_contract_seeds.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/src/web3core/types.py` & `web3cli-1.1.9/src/web3core/types.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/.DS_Store` & `web3cli-1.1.9/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/.DS_Store` & `web3cli-1.1.9/tests/ape/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/.build/Factory_IERC20.json` & `web3cli-1.1.9/tests/ape/.build/Factory_IERC20.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/.build/Factory_IUniswapV2Callee.json` & `web3cli-1.1.9/tests/ape/.build/Factory_IUniswapV2Callee.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/.build/Factory_IUniswapV2ERC20.json` & `web3cli-1.1.9/tests/ape/.build/Factory_IUniswapV2ERC20.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/.build/Factory_IUniswapV2Factory.json` & `web3cli-1.1.9/tests/ape/.build/Factory_IUniswapV2Factory.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/.build/Factory_IUniswapV2Pair.json` & `web3cli-1.1.9/tests/ape/.build/Factory_IUniswapV2Pair.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/.build/Factory_Math.json` & `web3cli-1.1.9/tests/ape/.build/Factory_Math.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/.build/Factory_SafeMath.json` & `web3cli-1.1.9/tests/ape/.build/Factory_SafeMath.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/.build/Factory_UQ112x112.json` & `web3cli-1.1.9/tests/ape/.build/Factory_UQ112x112.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/.build/Router_IERC20.json` & `web3cli-1.1.9/tests/ape/.build/Router_IERC20.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/.build/Router_IUniswapV2Factory.json` & `web3cli-1.1.9/tests/ape/.build/Router_IUniswapV2Factory.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/.build/Router_IUniswapV2Pair.json` & `web3cli-1.1.9/tests/ape/.build/Router_IUniswapV2Pair.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/.build/Router_IUniswapV2Router01.json` & `web3cli-1.1.9/tests/ape/.build/Router_IUniswapV2Router01.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/.build/Router_IUniswapV2Router02.json` & `web3cli-1.1.9/tests/ape/.build/Router_IUniswapV2Router02.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/.build/Router_IWETH.json` & `web3cli-1.1.9/tests/ape/.build/Router_IWETH.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/.build/Router_SafeMath.json` & `web3cli-1.1.9/tests/ape/.build/Router_SafeMath.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/.build/Router_TransferHelper.json` & `web3cli-1.1.9/tests/ape/.build/Router_TransferHelper.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/.build/Router_UniswapV2Library.json` & `web3cli-1.1.9/tests/ape/.build/Router_UniswapV2Library.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/.build/Token.json` & `web3cli-1.1.9/tests/ape/.build/Token.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/.build/Token_SafeMath.json` & `web3cli-1.1.9/tests/ape/.build/Token_SafeMath.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/.build/UniswapV2ERC20.json` & `web3cli-1.1.9/tests/ape/.build/UniswapV2ERC20.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/.build/UniswapV2Factory.json` & `web3cli-1.1.9/tests/ape/.build/UniswapV2Factory.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/.build/UniswapV2Pair.json` & `web3cli-1.1.9/tests/ape/.build/UniswapV2Pair.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/.build/UniswapV2Router02.json` & `web3cli-1.1.9/tests/ape/.build/UniswapV2Router02.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/.build/__local__.json` & `web3cli-1.1.9/tests/ape/.build/__local__.json`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/contracts/.DS_Store` & `web3cli-1.1.9/tests/ape/contracts/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/contracts/token/Token.sol` & `web3cli-1.1.9/tests/ape/contracts/token/Token.sol`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/contracts/token/Token_SafeMath.sol` & `web3cli-1.1.9/tests/ape/contracts/token/Token_SafeMath.sol`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/contracts/uniswap/.DS_Store` & `web3cli-1.1.9/tests/ape/contracts/uniswap/.DS_Store`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/contracts/uniswap/UniswapV2Factory.sol` & `web3cli-1.1.9/tests/ape/contracts/uniswap/UniswapV2Factory.sol`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/contracts/uniswap/UniswapV2Router02.sol` & `web3cli-1.1.9/tests/ape/contracts/uniswap/UniswapV2Router02.sol`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/tests/fixtures.py` & `web3cli-1.1.9/tests/ape/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/tests/helpers/token.py` & `web3cli-1.1.9/tests/ape/tests/helpers/token.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/tests/helpers/uniswap.py` & `web3cli-1.1.9/tests/ape/tests/helpers/uniswap.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/tests/token/test_ape_token_approve.py` & `web3cli-1.1.9/tests/ape/tests/token/test_ape_token_approve.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/tests/token/test_ape_token_transfer.py` & `web3cli-1.1.9/tests/ape/tests/token/test_ape_token_transfer.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/tests/token/test_ape_token_transferFrom.py` & `web3cli-1.1.9/tests/ape/tests/token/test_ape_token_transferFrom.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/tests/uniswap/test_ape_uniswap_v2_add_liquidity.py` & `web3cli-1.1.9/tests/ape/tests/uniswap/test_ape_uniswap_v2_add_liquidity.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/ape/tests/uniswap/test_ape_uniswap_v2_create_pair.py` & `web3cli-1.1.9/tests/ape/tests/uniswap/test_ape_uniswap_v2_create_pair.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/helper.py` & `web3cli-1.1.9/tests/helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/seed.py` & `web3cli-1.1.9/tests/seed.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3cli/controllers/crud/test_address_controller.py` & `web3cli-1.1.9/tests/web3cli/controllers/crud/test_address_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3cli/controllers/crud/test_chain_controller.py` & `web3cli-1.1.9/tests/web3cli/controllers/crud/test_chain_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3cli/controllers/crud/test_contract_controller.py` & `web3cli-1.1.9/tests/web3cli/controllers/crud/test_contract_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3cli/controllers/crud/test_history_controller.py` & `web3cli-1.1.9/tests/web3cli/controllers/crud/test_history_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3cli/controllers/crud/test_rpc_controller.py` & `web3cli-1.1.9/tests/web3cli/controllers/crud/test_rpc_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3cli/controllers/crud/test_signer_controller.py` & `web3cli-1.1.9/tests/web3cli/controllers/crud/test_signer_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3cli/controllers/crud/test_token_controller.py` & `web3cli-1.1.9/tests/web3cli/controllers/crud/test_token_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3cli/controllers/test_appkey_controller.py` & `web3cli-1.1.9/tests/web3cli/controllers/test_appkey_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3cli/controllers/test_call_controller.py` & `web3cli-1.1.9/tests/web3cli/controllers/test_call_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3cli/controllers/test_db_controller.py` & `web3cli-1.1.9/tests/web3cli/controllers/test_db_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3cli/controllers/test_keyfile_controller.py` & `web3cli-1.1.9/tests/web3cli/controllers/test_keyfile_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3cli/controllers/test_misc_controller.py` & `web3cli-1.1.9/tests/web3cli/controllers/test_misc_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3cli/controllers/test_replay_controller.py` & `web3cli-1.1.9/tests/web3cli/controllers/test_replay_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3cli/controllers/test_send_controller.py` & `web3cli-1.1.9/tests/web3cli/controllers/test_send_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3cli/controllers/test_transact_controller.py` & `web3cli-1.1.9/tests/web3cli/controllers/test_transact_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3cli/controllers/test_tx_controller.py` & `web3cli-1.1.9/tests/web3cli/controllers/test_tx_controller.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3cli/fixtures.py` & `web3cli-1.1.9/tests/web3cli/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3cli/helpers/test_crypto_helper.py` & `web3cli-1.1.9/tests/web3cli/helpers/test_crypto_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3cli/main.py` & `web3cli-1.1.9/tests/web3cli/main.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3cli/test_db.py` & `web3cli-1.1.9/tests/web3cli/test_db.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3core/fixtures.py` & `web3cli-1.1.9/tests/web3core/fixtures.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3core/helpers/test_abi_helper.py` & `web3cli-1.1.9/tests/web3core/helpers/test_abi_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3core/helpers/test_crypto_helper.py` & `web3cli-1.1.9/tests/web3core/helpers/test_crypto_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3core/helpers/test_resolve_address_helper.py` & `web3cli-1.1.9/tests/web3core/helpers/test_resolve_address_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3core/helpers/test_validation_helper.py` & `web3cli-1.1.9/tests/web3core/helpers/test_validation_helper.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/tests/web3core/models/test_contract_model.py` & `web3cli-1.1.9/tests/web3core/models/test_contract_model.py`

 * *Files identical despite different names*

### Comparing `web3cli-1.1.8/PKG-INFO` & `web3cli-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web3cli
-Version: 1.1.8
+Version: 1.1.9
 Summary: Interact with blockchains and smart contracts using the command line
 License: MIT
 Keywords: web3,w3,cli,evm,blockchain,ethereum,binance,avalanche
 Author-email: coccoinomane <coccoinomane@gmail.com>
 Requires-Python: >=3.9,<3.11
 Project-URL: homepage, https://github.com/coccoinomane/web3cli
 Project-URL: repository, https://github.com/coccoinomane/web3cli
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: web3cli Version: 1.1.8 Summary: Interact with
+Metadata-Version: 2.1 Name: web3cli Version: 1.1.9 Summary: Interact with
 blockchains and smart contracts using the command line License: MIT Keywords:
 web3,w3,cli,evm,blockchain,ethereum,binance,avalanche Author-email:
 coccoinomane
 gmail.com> Requires-Python: >=3.9,<3.11 Project-URL: homepage, https://
 github.com/coccoinomane/web3cli Project-URL: repository, https://github.com/
 coccoinomane/web3cli Description-Content-Type: text/markdown
 [https://img.shields.io/github/commit-activity/m/badges/shields?color=009051]
```

