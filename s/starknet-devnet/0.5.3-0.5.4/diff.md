# Comparing `tmp/starknet_devnet-0.5.3.tar.gz` & `tmp/starknet_devnet-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starknet_devnet-0.5.3.tar", max compression
+gzip compressed data, was "starknet_devnet-0.5.4.tar", max compression
```

## Comparing `starknet_devnet-0.5.3.tar` & `starknet_devnet-0.5.4.tar`

### file list

```diff
@@ -1,59 +1,60 @@
--rw-r--r--   0        0        0     1067 2023-06-01 14:55:07.944823 starknet_devnet-0.5.3/LICENSE
--rw-r--r--   0        0        0     1054 2023-06-01 14:55:07.944823 starknet_devnet-0.5.3/README.md
--rw-r--r--   0        0        0     1818 2023-06-01 14:55:07.956824 starknet_devnet-0.5.3/pyproject.toml
--rw-r--r--   0        0        0   208485 2023-06-01 14:55:07.960824 starknet_devnet-0.5.3/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json
--rw-r--r--   0        0        0    32739 2023-06-01 14:55:07.960824 starknet_devnet-0.5.3/starknet_devnet/MockStarknetMessaging.json
--rw-r--r--   0        0        0    35645 2023-06-01 14:55:07.960824 starknet_devnet-0.5.3/starknet_devnet/UDC_OZ_0.5.0.json
--rw-r--r--   0        0        0     2958 2023-06-01 14:55:07.960824 starknet_devnet-0.5.3/starknet_devnet/__init__.py
--rw-r--r--   0        0        0     2130 2023-06-01 14:55:07.960824 starknet_devnet-0.5.3/starknet_devnet/account.py
--rw-r--r--   0        0        0     3784 2023-06-01 14:55:07.960824 starknet_devnet-0.5.3/starknet_devnet/account_util.py
--rw-r--r--   0        0        0     2692 2023-06-01 14:55:07.960824 starknet_devnet-0.5.3/starknet_devnet/accounts.py
--rw-r--r--   0        0        0   118818 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json
--rw-r--r--   0        0        0     1784 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json
--rw-r--r--   0        0        0     1866 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/block_info_generator.py
--rw-r--r--   0        0        0    12337 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blocks.py
--rw-r--r--   0        0        0        0 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/__init__.py
--rw-r--r--   0        0        0     7523 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/base.py
--rw-r--r--   0        0        0    14072 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/feeder_gateway.py
--rw-r--r--   0        0        0     2228 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/gateway.py
--rw-r--r--   0        0        0     3959 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/postman.py
--rw-r--r--   0        0        0        0 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/__init__.py
--rw-r--r--   0        0        0     2138 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/blocks.py
--rw-r--r--   0        0        0     2120 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/call.py
--rw-r--r--   0        0        0     2195 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/classes.py
--rw-r--r--   0        0        0     6257 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/misc.py
--rw-r--r--   0        0        0     4878 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/routes.py
--rw-r--r--   0        0        0   116673 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/rpc_spec.py
--rw-r--r--   0        0        0     6049 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/rpc_spec_write.py
--rw-r--r--   0        0        0     6925 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/schema.py
--rw-r--r--   0        0        0     1144 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/state.py
--rw-r--r--   0        0        0      929 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/storage.py
--rw-r--r--   0        0        0        0 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/structures/__init__.py
--rw-r--r--   0        0        0    28429 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/structures/payloads.py
--rw-r--r--   0        0        0     6544 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/structures/responses.py
--rw-r--r--   0        0        0     3457 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/structures/types.py
--rw-r--r--   0        0        0     7212 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/transactions.py
--rw-r--r--   0        0        0     3542 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/utils.py
--rw-r--r--   0        0        0      899 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/shared.py
--rw-r--r--   0        0        0    24763 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/cairo_rs_py_patch.py
--rw-r--r--   0        0        0      877 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/chargeable_account.py
--rw-r--r--   0        0        0     5133 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/compiler.py
--rw-r--r--   0        0        0     1239 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/constants.py
--rw-r--r--   0        0        0      646 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/contract_class_wrapper.py
--rw-r--r--   0        0        0    14596 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/devnet_config.py
--rw-r--r--   0        0        0      784 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/dump.py
--rw-r--r--   0        0        0     5592 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/fee_token.py
--rw-r--r--   0        0        0     8161 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/forked_state.py
--rw-r--r--   0        0        0     1640 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/general_config.py
--rw-r--r--   0        0        0     9005 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/origin.py
--rw-r--r--   0        0        0    10015 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/postman_wrapper.py
--rw-r--r--   0        0        0     1970 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/predeployed_contract_wrapper.py
--rw-r--r--   0        0        0     4275 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/server.py
--rw-r--r--   0        0        0    39769 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/starknet_wrapper.py
--rw-r--r--   0        0        0     1988 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/state.py
--rw-r--r--   0        0        0     2573 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/state_archive.py
--rw-r--r--   0        0        0    11617 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/transactions.py
--rw-r--r--   0        0        0     1626 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/udc.py
--rw-r--r--   0        0        0     8580 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/util.py
--rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 starknet_devnet-0.5.3/setup.py
--rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 starknet_devnet-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-16 12:50:09.375941 starknet_devnet-0.5.4/LICENSE
+-rw-r--r--   0        0        0     1054 2023-06-16 12:50:09.375941 starknet_devnet-0.5.4/README.md
+-rw-r--r--   0        0        0     1818 2023-06-16 12:50:09.387941 starknet_devnet-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0   208485 2023-06-16 12:50:09.387941 starknet_devnet-0.5.4/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json
+-rw-r--r--   0        0        0    32739 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/MockStarknetMessaging.json
+-rw-r--r--   0        0        0    35645 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/UDC_OZ_0.5.0.json
+-rw-r--r--   0        0        0     2958 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/__init__.py
+-rw-r--r--   0        0        0     2595 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/account.py
+-rw-r--r--   0        0        0     3784 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/account_util.py
+-rw-r--r--   0        0        0     2511 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/accounts.py
+-rw-r--r--   0        0        0   118818 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json
+-rw-r--r--   0        0        0     1784 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json
+-rw-r--r--   0        0        0     1866 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/block_info_generator.py
+-rw-r--r--   0        0        0    12337 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blocks.py
+-rw-r--r--   0        0        0        0 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/__init__.py
+-rw-r--r--   0        0        0     7585 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/base.py
+-rw-r--r--   0        0        0    14072 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/feeder_gateway.py
+-rw-r--r--   0        0        0     2256 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/gateway.py
+-rw-r--r--   0        0        0     3959 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/postman.py
+-rw-r--r--   0        0        0        0 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/__init__.py
+-rw-r--r--   0        0        0     2138 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/blocks.py
+-rw-r--r--   0        0        0     2120 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/call.py
+-rw-r--r--   0        0        0     2195 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/classes.py
+-rw-r--r--   0        0        0     6257 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/misc.py
+-rw-r--r--   0        0        0     4953 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/routes.py
+-rw-r--r--   0        0        0   116673 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/rpc_spec.py
+-rw-r--r--   0        0        0     6049 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/rpc_spec_write.py
+-rw-r--r--   0        0        0    16310 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/rpc_trace_spec.py
+-rw-r--r--   0        0        0     7135 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/schema.py
+-rw-r--r--   0        0        0     1144 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/state.py
+-rw-r--r--   0        0        0      929 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/storage.py
+-rw-r--r--   0        0        0        0 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/structures/__init__.py
+-rw-r--r--   0        0        0    31253 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/structures/payloads.py
+-rw-r--r--   0        0        0     6544 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/structures/responses.py
+-rw-r--r--   0        0        0     3457 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/structures/types.py
+-rw-r--r--   0        0        0     8789 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/transactions.py
+-rw-r--r--   0        0        0     3542 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/utils.py
+-rw-r--r--   0        0        0      899 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/blueprints/shared.py
+-rw-r--r--   0        0        0    24763 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/cairo_rs_py_patch.py
+-rw-r--r--   0        0        0     1038 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/chargeable_account.py
+-rw-r--r--   0        0        0     5310 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/compiler.py
+-rw-r--r--   0        0        0     1239 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/constants.py
+-rw-r--r--   0        0        0      646 2023-06-16 12:50:09.391941 starknet_devnet-0.5.4/starknet_devnet/contract_class_wrapper.py
+-rw-r--r--   0        0        0    16387 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/devnet_config.py
+-rw-r--r--   0        0        0      784 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/dump.py
+-rw-r--r--   0        0        0     6119 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/fee_token.py
+-rw-r--r--   0        0        0     8161 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/forked_state.py
+-rw-r--r--   0        0        0     1640 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/general_config.py
+-rw-r--r--   0        0        0     9005 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/origin.py
+-rw-r--r--   0        0        0    10015 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/postman_wrapper.py
+-rw-r--r--   0        0        0     2237 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/predeployed_contract_wrapper.py
+-rw-r--r--   0        0        0     4353 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/server.py
+-rw-r--r--   0        0        0    40357 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/starknet_wrapper.py
+-rw-r--r--   0        0        0     1988 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/state.py
+-rw-r--r--   0        0        0     2573 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/state_archive.py
+-rw-r--r--   0        0        0    11617 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/transactions.py
+-rw-r--r--   0        0        0     1822 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/udc.py
+-rw-r--r--   0        0        0    10902 2023-06-16 12:50:09.395941 starknet_devnet-0.5.4/starknet_devnet/util.py
+-rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 starknet_devnet-0.5.4/setup.py
+-rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 starknet_devnet-0.5.4/PKG-INFO
```

### Comparing `starknet_devnet-0.5.3/LICENSE` & `starknet_devnet-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/README.md` & `starknet_devnet-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/pyproject.toml` & `starknet_devnet-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "starknet_devnet"
-version = "0.5.3"
+version = "0.5.4"
 description = "A local testnet for Starknet"
 authors = ["FabijanC <fabijan.corak@gmail.com>"]
 license = "MIT"
 
 readme = "README.md"
 repository = "https://github.com/0xSpaceShard/starknet-devnet"
 homepage = "https://github.com/0xSpaceShard/starknet-devnet"
```

### Comparing `starknet_devnet-0.5.3/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json` & `starknet_devnet-0.5.4/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/MockStarknetMessaging.json` & `starknet_devnet-0.5.4/starknet_devnet/MockStarknetMessaging.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/UDC_OZ_0.5.0.json` & `starknet_devnet-0.5.4/starknet_devnet/UDC_OZ_0.5.0.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/__init__.py` & `starknet_devnet-0.5.4/starknet_devnet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # pylint: disable=unused-import
 # pylint: disable=import-outside-toplevel
 
 import os
 import sys
 
-__version__ = "0.5.3"
+__version__ = "0.5.4"
 
 
 def _patch_pedersen_hash():
     """
     Improves performance by substituting the default Python implementation of Pedersen hash
     with Software Mansion's Python wrapper of C++ implementation.
     """
```

### Comparing `starknet_devnet-0.5.3/starknet_devnet/account.py` & `starknet_devnet-0.5.4/starknet_devnet/account.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 """
 Account class and its predefined constants.
 """
 
+from typing import Optional
+
 from starkware.starknet.core.os.contract_address.contract_address import (
     calculate_contract_address_from_hash,
 )
 from starkware.starknet.public.abi import get_selector_from_name
 from starkware.starknet.testing.starknet import Starknet
 
 from starknet_devnet.account_util import set_balance
 from starknet_devnet.contract_class_wrapper import CompiledClassWrapper
 from starknet_devnet.predeployed_contract_wrapper import PredeployedContractWrapper
 
 
+# pylint: disable=too-many-instance-attributes
 class Account(PredeployedContractWrapper):
     """Account contract wrapper."""
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         starknet_wrapper,
         private_key: int,
         public_key: int,
         initial_balance: int,
         account_class_wrapper: CompiledClassWrapper,
+        index: Optional[int] = None,
     ):
         self.starknet_wrapper = starknet_wrapper
         self.private_key = private_key
         self.public_key = public_key
         self.contract_class = account_class_wrapper.contract_class
         self.class_hash = account_class_wrapper.hash
 
@@ -37,14 +41,17 @@
             salt=20,
             class_hash=0x3FCBF77B28C96F4F2FB5BD2D176AB083A12A5E123ADEB0DE955D7EE228C9854,
             constructor_calldata=[public_key],
             deployer_address=0,
         )
         self.initial_balance = initial_balance
 
+        self.__index = index
+        """Index used when logging/displaying account to user on startup"""
+
     def to_json(self):
         """Return json account"""
         return {
             "initial_balance": self.initial_balance,
             "private_key": hex(self.private_key),
             "public_key": hex(self.public_key),
             "address": hex(self.address),
@@ -54,7 +61,14 @@
         starknet: Starknet = self.starknet_wrapper.starknet
 
         await starknet.state.state.set_storage_at(
             self.address, get_selector_from_name("Account_public_key"), self.public_key
         )
 
         await set_balance(starknet.state, self.address, self.initial_balance)
+
+    def print(self):
+        print(f"Account #{self.__index}:")
+        print(f"Address: {hex(self.address)}")
+        print(f"Public key: {hex(self.public_key)}")
+        print(f"Private key: {hex(self.private_key)}")
+        print(flush=True)
```

### Comparing `starknet_devnet-0.5.3/starknet_devnet/account_util.py` & `starknet_devnet-0.5.4/starknet_devnet/account_util.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/accounts.py` & `starknet_devnet-0.5.4/starknet_devnet/accounts.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,60 +26,55 @@
         self.__seed = starknet_wrapper.config.seed
         if self.__seed is None:
             self.__seed = random.getrandbits(32)
 
         self.list = []
 
         self.__generate()
-        if (
-            starknet_wrapper.config.accounts
-            and not starknet_wrapper.config.hide_predeployed_accounts
-        ):
-            self.__print()
 
     def __getitem__(self, index) -> Account:
         return self.list[index]
 
     async def deploy(self):
         """deploy listed accounts"""
         for account in self.list:
             await account.deploy()
+        if self.starknet_wrapper.config.accounts and (
+            self.starknet_wrapper.config.verbose
+            or not self.starknet_wrapper.config.hide_predeployed_contracts
+        ):
+            self.__print()
 
     def add(self, account):
         """append account to list"""
         self.list.append(account)
         return account
 
     def __generate(self):
         """Generates accounts without deploying them"""
         random_generator = random.Random()
         random_generator.seed(self.__seed)
 
-        for _ in range(self.__n_accounts):
+        for i in range(self.__n_accounts):
             private_key = random_generator.getrandbits(128)
             public_key = private_to_stark_key(private_key)
 
             self.add(
                 Account(
                     self.starknet_wrapper,
                     private_key=private_key,
                     public_key=public_key,
                     initial_balance=self.__initial_balance,
                     account_class_wrapper=self.__account_class_wrapper,
+                    index=i,
                 )
             )
 
     def __print(self):
         """stdout accounts list"""
-        for idx, account in enumerate(self):
-            print(f"Account #{idx}")
-            print(f"Address: {hex(account.address)}")
-            print(f"Public key: {hex(account.public_key)}")
-            print(f"Private key: {hex(account.private_key)}\n")
-
         print(f"Initial balance of each account: {self.__initial_balance} WEI")
         print("Seed to replicate this account sequence:", self.__seed)
         warn(
             "WARNING: Use these accounts and their keys ONLY for local testing. "
             "DO NOT use them on mainnet or other live networks because you will LOSE FUNDS.\n",
             file=sys.stderr,
         )
```

### Comparing `starknet_devnet-0.5.3/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json` & `starknet_devnet-0.5.4/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json` & `starknet_devnet-0.5.4/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/block_info_generator.py` & `starknet_devnet-0.5.4/starknet_devnet/block_info_generator.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/blocks.py` & `starknet_devnet-0.5.4/starknet_devnet/blocks.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/blueprints/base.py` & `starknet_devnet-0.5.4/starknet_devnet/blueprints/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from starkware.starkware_utils.error_handling import StarkErrorCode
 
 from starknet_devnet.fee_token import FeeToken
 from starknet_devnet.state import state
 from starknet_devnet.util import (
     StarknetDevnetException,
     check_valid_dump_path,
+    log_request,
     parse_hex_string,
 )
 
 base = Blueprint("base", __name__)
 
 
 def extract_int(value):
@@ -122,14 +123,15 @@
         )
 
     state.load(load_path)
     return Response(status=200)
 
 
 @base.route("/increase_time", methods=["POST"])
+@log_request()
 async def increase_time():
     """Increases the block timestamp offset and generates a new block"""
     request_dict = request.json or {}
     time_s = extract_positive(request_dict, "time")
 
     # Increase block time only when there are no pending transactions
     if not state.starknet_wrapper.pending_txs:
@@ -143,14 +145,15 @@
         code=StarkErrorCode.INVALID_REQUEST,
         status_code=400,
         message="Block time can be increased only if there are no pending transactions.",
     )
 
 
 @base.route("/set_time", methods=["POST"])
+@log_request()
 async def set_time():
     """Sets the block timestamp offset and generates a new block"""
     request_dict = request.json or {}
     time_s = extract_positive(request_dict, "time")
 
     # Set block time only when there are no pending transactions
     if not state.starknet_wrapper.pending_txs:
@@ -186,14 +189,15 @@
     """Get the address of the fee token"""
     fee_token_address = FeeToken.ADDRESS
     symbol = FeeToken.SYMBOL
     return jsonify({"symbol": symbol, "address": hex(fee_token_address)})
 
 
 @base.route("/mint", methods=["POST"])
+@log_request()
 async def mint():
     """Mint token and transfer to the provided address"""
     request_json = request.json or {}
 
     address = hex_converter(request_json, "address")
     amount = extract_positive(request_json, "amount")
     is_lite = request_json.get("lite", False)
```

### Comparing `starknet_devnet-0.5.3/starknet_devnet/blueprints/feeder_gateway.py` & `starknet_devnet-0.5.4/starknet_devnet/blueprints/feeder_gateway.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/blueprints/gateway.py` & `starknet_devnet-0.5.4/starknet_devnet/blueprints/gateway.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 from flask import Blueprint, jsonify, request
 from starkware.starknet.definitions.error_codes import StarknetErrorCode
 from starkware.starknet.definitions.transaction_type import TransactionType
 from starkware.starkware_utils.error_handling import StarkErrorCode
 
 from starknet_devnet.devnet_config import DumpOn
 from starknet_devnet.state import state
-from starknet_devnet.util import StarknetDevnetException, fixed_length_hex
+from starknet_devnet.util import StarknetDevnetException, fixed_length_hex, log_request
 
 from .shared import validate_transaction
 
 gateway = Blueprint("gateway", __name__, url_prefix="/gateway")
 
 
 @gateway.route("/add_transaction", methods=["POST"])
+@log_request()
 async def add_transaction():
     """Endpoint for accepting (state-changing) transactions."""
 
     transaction = validate_transaction(request.get_data())
     tx_type = transaction.tx_type
 
     response_dict = {
```

### Comparing `starknet_devnet-0.5.3/starknet_devnet/blueprints/postman.py` & `starknet_devnet-0.5.4/starknet_devnet/blueprints/postman.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/blocks.py` & `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/blocks.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/call.py` & `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/call.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/classes.py` & `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/classes.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/misc.py` & `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/misc.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/routes.py` & `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     add_deploy_account_transaction,
     add_invoke_transaction,
     estimate_fee,
     get_transaction_by_block_id_and_index,
     get_transaction_by_hash,
     get_transaction_receipt,
     pending_transactions,
+    simulate_transaction,
 )
 from starknet_devnet.blueprints.rpc.utils import rpc_error, rpc_response
 from starknet_devnet.util import StarknetDevnetException
 
 methods = {
     "getBlockWithTxHashes": get_block_with_tx_hashes,
     "getBlockWithTxs": get_block_with_txs,
@@ -69,14 +70,15 @@
     "pendingTransactions": pending_transactions,
     "syncing": syncing,
     "getEvents": get_events,
     "getNonce": get_nonce,
     "addInvokeTransaction": add_invoke_transaction,
     "addDeclareTransaction": add_declare_transaction,
     "addDeployAccountTransaction": add_deploy_account_transaction,
+    "simulateTransaction": simulate_transaction,
 }
 
 rpc = Blueprint("rpc", __name__, url_prefix="/rpc")
 
 
 @rpc.route("", methods=["POST"])
 async def base_route():
```

### Comparing `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/rpc_spec.py` & `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/rpc_spec.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/rpc_spec_write.py` & `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/rpc_spec_write.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/schema.py` & `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,25 +10,31 @@
 from typing import Tuple
 
 from jsonschema import validate
 from jsonschema.exceptions import ValidationError
 
 from starknet_devnet.blueprints.rpc.rpc_spec import RPC_SPECIFICATION
 from starknet_devnet.blueprints.rpc.rpc_spec_write import RPC_SPECIFICATION_WRITE
+from starknet_devnet.blueprints.rpc.rpc_trace_spec import RPC_SPECIFICATION_TRACE
 from starknet_devnet.state import state
 
 
 # Cache the function result so schemas are not reloaded from disk on every call
 @lru_cache
 def _load_schemas() -> Tuple[Dict[str, Any], Dict[str, Any]]:
     specs_json = json.loads(RPC_SPECIFICATION)
     write_specs_json = json.loads(RPC_SPECIFICATION_WRITE)
+    trace_specs_json = json.loads(RPC_SPECIFICATION_TRACE)
     schemas = specs_json["components"]["schemas"]
 
-    methods = {**_extract_methods(specs_json), **_extract_methods(write_specs_json)}
+    methods = {
+        **_extract_methods(specs_json),
+        **_extract_methods(write_specs_json),
+        **_extract_methods(trace_specs_json),
+    }
 
     return methods, schemas
 
 
 def _extract_methods(specs_json: Dict[str, Any]) -> Dict[str, Any]:
     return {method["name"]: method for method in specs_json["methods"]}
```

### Comparing `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/state.py` & `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/state.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/storage.py` & `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/storage.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/structures/payloads.py` & `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/structures/payloads.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+# pylint: disable=too-many-lines
+
 """
 RPC payload structures
 """
 
 from __future__ import annotations
 
+from enum import Enum, auto
 from typing import Callable, Dict, List, Optional, Union
 
 from marshmallow.exceptions import MarshmallowError
 from starkware.starknet.definitions.constants import QUERY_VERSION_BASE
 from starkware.starknet.definitions.general_config import StarknetGeneralConfig
 from starkware.starknet.public.abi import AbiEntryType
 from starkware.starknet.services.api.contract_class.contract_class import (
@@ -23,14 +26,15 @@
     DeployAccountSpecificInfo,
     DeploySpecificInfo,
     FeeEstimationInfo,
     InvokeSpecificInfo,
     L1HandlerSpecificInfo,
     StarknetBlock,
     TransactionSpecificInfo,
+    TransactionTrace,
     TransactionType,
 )
 from starkware.starknet.services.api.gateway.transaction import (
     Declare,
     DeployAccount,
     DeprecatedDeclare,
     InvokeFunction,
@@ -199,31 +203,45 @@
 class RpcInvokeTransactionV1(RpcTransactionCommon):
     """TypedDict for rpc invoke transaction version 1"""
 
     sender_address: Address
     calldata: List[Felt]
 
 
+RpcInvokeTransaction = Union[RpcInvokeTransactionV0, RpcInvokeTransactionV1]
+
+
 class RpcL1HandlerTransaction(TypedDict):
     """TypedDict for rpc L1 -> L2 message transaction"""
 
     contract_address: Address
     entry_point_selector: Felt
     calldata: List[Felt]
     transaction_hash: TxnHash
     version: NumAsHex
     type: RpcTxnType
     nonce: Felt
 
 
-class RpcDeclareTransaction(RpcTransactionCommon):
-    """TypedDict for rpc declare transaction"""
+class RpcDeclareV1Transaction(RpcTransactionCommon):
+    """TypedDict for rpc declare transaction version 1"""
+
+    class_hash: Felt
+    sender_address: Address
+
+
+class RpcDeclareV2Transaction(RpcTransactionCommon):
+    """TypedDict for rpc declare transaction version 2"""
 
     class_hash: Felt
     sender_address: Address
+    compiled_class_hash: Felt
+
+
+RpcDeclareTransaction = Union[RpcDeclareV1Transaction, RpcDeclareV2Transaction]
 
 
 class RpcDeployTransaction(TypedDict):
     """TypedDict for rpc deploy transaction"""
 
     transaction_hash: TxnHash
     class_hash: Felt
@@ -238,16 +256,15 @@
 
     contract_address_salt: Felt
     constructor_calldata: List[Felt]
     class_hash: Felt
 
 
 RpcTransaction = Union[
-    RpcInvokeTransactionV0,
-    RpcInvokeTransactionV1,
+    RpcInvokeTransaction,
     RpcL1HandlerTransaction,
     RpcDeclareTransaction,
     RpcDeployTransaction,
     RpcDeployAccountTransaction,
 ]
 
 
@@ -280,15 +297,15 @@
         entry_point_selector=int(function_call["entry_point_selector"], 16),
         calldata=[int(data, 16) for data in function_call["calldata"]],
     )
 
 
 def rpc_invoke_transaction(
     transaction: InvokeSpecificInfo,
-) -> Union[RpcInvokeTransactionV0, RpcInvokeTransactionV1]:
+) -> RpcInvokeTransaction:
     """
     Convert gateway invoke transaction to rpc format
     """
     common_data = {
         "transaction_hash": rpc_felt(transaction.transaction_hash),
         "calldata": [rpc_felt(data) for data in transaction.calldata],
         "max_fee": rpc_felt(transaction.max_fee),
@@ -312,24 +329,31 @@
     return txn
 
 
 def rpc_declare_transaction(transaction: DeclareSpecificInfo) -> RpcDeclareTransaction:
     """
     Convert gateway declare transaction to rpc format
     """
-    txn: RpcDeclareTransaction = {
+    common_data = {
         "class_hash": rpc_felt(transaction.class_hash),
         "sender_address": rpc_felt(transaction.sender_address),
         "transaction_hash": rpc_felt(transaction.transaction_hash),
         "max_fee": rpc_felt(transaction.max_fee),
         "version": hex(transaction.version),
         "signature": [rpc_felt(value) for value in transaction.signature],
         "nonce": rpc_felt(transaction.nonce),
         "type": rpc_txn_type(transaction.tx_type.name),
     }
+    if transaction.version == SUPPORTED_RPC_DECLARE_TX_VERSION:
+        txn: RpcDeclareV2Transaction = {
+            "compiled_class_hash": rpc_felt(transaction.compiled_class_hash),
+            **common_data,
+        }
+    else:
+        txn: RpcDeclareV1Transaction = {**common_data}
     return txn
 
 
 def rpc_deploy_transaction(transaction: DeploySpecificInfo) -> RpcDeployTransaction:
     """
     Convert gateway deploy transaction to rpc format
     """
@@ -615,14 +639,21 @@
     size: int  # minimum 1
     members: List[StructMember]
 
 
 AbiEntry = Union[FunctionAbiEntry, EventAbiEntry, StructAbiEntry]
 
 
+class SimulationFlag(Enum):
+    """Enum with flags for simulate transaction"""
+
+    SKIP_VALIDATE = auto()
+    SKIP_EXECUTE = auto()
+
+
 def function_abi_entry(abi_entry: AbiEntryType) -> FunctionAbiEntry:
     """
     Convert function gateway abi entry to rpc FunctionAbiEntry
     """
     rpc_function_abi_entry = FunctionAbiEntry(
         type=abi_entry["type"],
         name=abi_entry["name"],
@@ -940,7 +971,68 @@
     rpc_state: RpcStateUpdate = {
         "block_hash": rpc_felt(state_update.block_hash),
         "new_root": rpc_root(state_update.new_root.hex()),
         "old_root": rpc_root(state_update.old_root.hex()),
         "state_diff": state_diff,
     }
     return rpc_state
+
+
+def rpc_map_traces(
+    traces: List[TransactionTrace], types: List[TransactionType]
+) -> List[Dict[str, Dict]]:
+    """
+    The purpose of this method is to map RPC trace responses based on different transaction types.
+    """
+    # traces number must be equal to types to properly map objects
+    assert len(traces) == len(types)
+
+    result = []
+    for i, trace in enumerate(traces):
+        trace_dict = trace.dump()
+
+        if types[i] == TransactionType.INVOKE_FUNCTION:
+            trace = rpc_invoke_txn_trace(trace_dict)
+        elif types[i] == TransactionType.DECLARE:
+            trace = rpc_declare_txn_trace(trace_dict)
+        elif types[i] == TransactionType.DEPLOY_ACCOUNT:
+            trace = rpc_deploy_account_txn_trace(trace_dict)
+        else:
+            raise RpcError(
+                code=-1, message=f"Transaction type '{types[i]}' is not supported."
+            )
+
+        result.append(trace)
+
+    return result
+
+
+def rpc_invoke_txn_trace(trace_dict: dict) -> Dict[str, Dict]:
+    """
+    Mapping for the execution trace of a invoke transaction.
+    """
+    return {
+        "validate_invocation": trace_dict.get("validate_invocation"),
+        "execute_invocation": trace_dict.get("function_invocation"),
+        "fee_transfer_invocation": trace_dict.get("fee_transfer_invocation"),
+    }
+
+
+def rpc_declare_txn_trace(trace_dict: dict) -> Dict[str, Dict]:
+    """
+    Mapping for the execution trace of a declare transaction.
+    """
+    return {
+        "validate_invocation": trace_dict.get("validate_invocation"),
+        "fee_transfer_invocation": trace_dict.get("fee_transfer_invocation"),
+    }
+
+
+def rpc_deploy_account_txn_trace(trace_dict: dict) -> Dict[str, Dict]:
+    """
+    Mapping for the execution trace of a deploy account transaction.
+    """
+    return {
+        "validate_invocation": trace_dict.get("validate_invocation"),
+        "constructor_invocation": trace_dict.get("function_invocation"),
+        "fee_transfer_invocation": trace_dict.get("fee_transfer_invocation"),
+    }
```

### Comparing `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/structures/responses.py` & `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/structures/responses.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/structures/types.py` & `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/structures/types.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/transactions.py` & `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/transactions.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 from starknet_devnet.blueprints.rpc.schema import validate_schema
 from starknet_devnet.blueprints.rpc.structures.payloads import (
     RpcBroadcastedDeclareTxn,
     RpcBroadcastedDeployAccountTxn,
     RpcBroadcastedInvokeTxn,
     RpcBroadcastedTxn,
     RpcTransaction,
+    SimulationFlag,
     make_declare,
     make_deploy_account,
     make_invoke_function,
     rpc_fee_estimate,
+    rpc_map_traces,
     rpc_transaction,
 )
 from starknet_devnet.blueprints.rpc.structures.responses import (
     RpcDeclareTransactionResult,
     RpcDeployAccountTransactionResult,
     RpcInvokeTransactionResult,
     rpc_transaction_receipt,
@@ -33,15 +35,15 @@
 from starknet_devnet.blueprints.rpc.utils import (
     assert_block_id_is_valid,
     get_block_by_block_id,
     rpc_felt,
 )
 from starknet_devnet.constants import LEGACY_TX_VERSION
 from starknet_devnet.state import state
-from starknet_devnet.util import StarknetDevnetException
+from starknet_devnet.util import StarknetDevnetException, log_request
 
 
 @validate_schema("getTransactionByHash")
 async def get_transaction_by_hash(transaction_hash: TxnHash) -> dict:
     """
     Get the details and status of a submitted transaction
     """
@@ -96,29 +98,29 @@
     """
     Returns the transactions in the transaction pool, recognized by this sequencer
     """
     raise NotImplementedError()
 
 
 @validate_schema("addInvokeTransaction")
+@log_request(rpc=True)
 async def add_invoke_transaction(invoke_transaction: RpcBroadcastedInvokeTxn) -> dict:
     """
     Submit a new transaction to be added to the chain
     """
-    invoke_function = make_invoke_function(invoke_transaction)
-
     _, transaction_hash = await state.starknet_wrapper.invoke(
-        external_tx=invoke_function
+        external_tx=make_invoke_function(invoke_transaction)
     )
     return RpcInvokeTransactionResult(
         transaction_hash=rpc_felt(transaction_hash),
     )
 
 
 @validate_schema("addDeclareTransaction")
+@log_request(rpc=True)
 async def add_declare_transaction(
     declare_transaction: RpcBroadcastedDeclareTxn,
 ) -> dict:
     """
     Submit a new class declaration transaction
     """
     if int(declare_transaction["version"], 0) == LEGACY_TX_VERSION:
@@ -142,24 +144,23 @@
     return RpcDeclareTransactionResult(
         transaction_hash=rpc_felt(transaction_hash),
         class_hash=rpc_felt(class_hash),
     )
 
 
 @validate_schema("addDeployAccountTransaction")
+@log_request(rpc=True)
 async def add_deploy_account_transaction(
     deploy_account_transaction: RpcBroadcastedDeployAccountTxn,
 ) -> dict:
     """
     Submit a new deploy account transaction
     """
-    deploy_account_tx = make_deploy_account(deploy_account_transaction)
-
     contract_address, transaction_hash = await state.starknet_wrapper.deploy_account(
-        external_tx=deploy_account_tx
+        external_tx=make_deploy_account(deploy_account_transaction)
     )
 
     status_response = await state.starknet_wrapper.transactions.get_transaction_status(
         hex(transaction_hash)
     )
     if (
         status_response["tx_status"] == "REJECTED"
@@ -185,31 +186,77 @@
     if txn_type == "DEPLOY":
         raise RpcError(code=-1, message="DEPLOY transactions are deprecated")
     if txn_type == "DEPLOY_ACCOUNT":
         return make_deploy_account(txn)
     raise NotImplementedError(f"Unexpected type {txn_type}.")
 
 
-@validate_schema("estimateFee")
-async def estimate_fee(request: List[RpcBroadcastedTxn], block_id: BlockId) -> list:
-    """
-    Estimate the fee for a given Starknet transaction
-    """
+async def _calculate_traces_and_fees(
+    transactions: List[AccountTransaction], block_id: BlockId, skip_validate: bool
+):
+    """Common for estimate_fee and simulate_transaction. Handles errors."""
+
     await assert_block_id_is_valid(block_id)
-    transactions = list(map(make_transaction, request))
 
     try:
-        _, fee_response = await state.starknet_wrapper.calculate_traces_and_fees(
+        return await state.starknet_wrapper.calculate_traces_and_fees(
             transactions,
-            skip_validate=False,
+            skip_validate=skip_validate,
             block_id=block_id,
         )
     except StarkException as ex:
         if "Entry point" in ex.message and "not found" in ex.message:
             raise RpcError.from_spec_name("CONTRACT_ERROR") from ex
         if "While handling calldata" in ex.message:
             raise RpcError.from_spec_name("CONTRACT_ERROR") from ex
         if "is not deployed" in ex.message:
             raise RpcError.from_spec_name("CONTRACT_NOT_FOUND") from ex
         raise RpcError(code=-1, message=ex.message) from ex
 
-    return rpc_fee_estimate(fee_response)
+
+@validate_schema("estimateFee")
+async def estimate_fee(request: List[RpcBroadcastedTxn], block_id: BlockId) -> list:
+    """Estimate the fee for the given Starknet transaction"""
+
+    gateway_transactions = list(map(make_transaction, request))
+    _, fee_responses = await _calculate_traces_and_fees(
+        gateway_transactions, block_id, skip_validate=False
+    )
+    return rpc_fee_estimate(fee_responses)
+
+
+@validate_schema("simulateTransaction")
+async def simulate_transaction(
+    block_id: BlockId,
+    transactions: List[RpcBroadcastedTxn],
+    simulation_flags: List[SimulationFlag],
+) -> list:
+    """
+    Simulate transactions.
+    SKIP_EXECUTE SimulationFlag is not supported.
+    """
+    skip_validate = SimulationFlag.SKIP_VALIDATE.name in simulation_flags
+    skip_execute = SimulationFlag.SKIP_EXECUTE.name in simulation_flags
+
+    if skip_execute:
+        raise RpcError(code=-1, message="SKIP_EXECUTE flag is not supported")
+
+    gateway_transactions = list(map(make_transaction, transactions))
+    traces, fees = await _calculate_traces_and_fees(
+        gateway_transactions, block_id, skip_validate
+    )
+
+    tx_types = [tx.tx_type for tx in gateway_transactions]
+    rpc_traces = rpc_map_traces(traces, tx_types)
+    rpc_estimations = rpc_fee_estimate(fees)
+
+    # traces number must be equal to estimations
+    assert len(rpc_traces) == len(rpc_estimations)
+    simulated_transactions = [
+        {
+            "transaction_trace": trace,
+            "fee_estimation": estimation,
+        }
+        for trace, estimation in zip(rpc_traces, rpc_estimations)
+    ]
+
+    return simulated_transactions
```

### Comparing `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/utils.py` & `starknet_devnet-0.5.4/starknet_devnet/blueprints/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/blueprints/shared.py` & `starknet_devnet-0.5.4/starknet_devnet/blueprints/shared.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/cairo_rs_py_patch.py` & `starknet_devnet-0.5.4/starknet_devnet/cairo_rs_py_patch.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/chargeable_account.py` & `starknet_devnet-0.5.4/starknet_devnet/chargeable_account.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
-Account that is charged with a fee when nobody else can be charged.
+Account that can be charged with a fee when nothing else can be charged.
+Intended for development and internal testing purposes.
 """
 
 from starknet_devnet.account import Account
 
 
 class ChargeableAccount(Account):
     """
@@ -19,7 +20,10 @@
         super().__init__(
             starknet_wrapper,
             private_key=ChargeableAccount.PRIVATE_KEY,
             public_key=ChargeableAccount.PUBLIC_KEY,
             initial_balance=2**251,  # loads of cash
             account_class_wrapper=starknet_wrapper.config.account_class,
         )
+
+    def print(self):
+        """Since this is a development/testing class, it needn't be logged"""
```

### Comparing `starknet_devnet-0.5.3/starknet_devnet/compiler.py` & `starknet_devnet-0.5.4/starknet_devnet/compiler.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 from starknet_devnet.devnet_config import DevnetConfig
 from starknet_devnet.util import StarknetDevnetException
 
 
 class ContractClassCompiler(ABC):
     """Base class of contract class compilers"""
 
+    def __init__(self, compiler_args: List[str]):
+        self._compiler_args = compiler_args
+
     def compile_contract_class(self, contract_class: ContractClass) -> CompiledClass:
         """Take the sierra and return the compiled instance"""
         raise NotImplementedError
 
 
 COMPILATION_ERROR_MSG = """
 Failed compilation from Sierra to Casm! Make sure you compiled the contract with the same compiler version Devnet is using for recompilation.
@@ -37,15 +40,15 @@
 class DefaultContractClassCompiler(ContractClassCompiler):
     """Uses the default internal cairo-lang compiler"""
 
     def compile_contract_class(self, contract_class: ContractClass) -> CompiledClass:
         try:
             return compile_contract_class(
                 contract_class,
-                compiler_args="--add-pythonic-hints --allowed-libfuncs-list-name experimental_v0.1.0",
+                compiler_args=" ".join(self._compiler_args),
             )
         except PermissionError as permission_error:
             raise StarknetDevnetException(
                 code=StarknetErrorCode.COMPILATION_FAILED,
                 message=str(permission_error) + COMPILATION_ERROR_MSG,
             ) from permission_error
         except StarkException as stark_exception:
@@ -70,17 +73,15 @@
             with open(contract_json, mode="w", encoding="utf-8") as tmp_file:
                 contract_class_dumped = contract_class.dump()
                 contract_class_dumped["abi"] = json.loads(contract_class_dumped["abi"])
                 json.dump(contract_class_dumped, tmp_file)
 
             compilation_args = [
                 *self.get_sierra_compiler_command(),
-                "--allowed-libfuncs-list-name",
-                "experimental_v0.1.0",
-                "--add-pythonic-hints",
+                *self._compiler_args,
                 contract_json,
                 contract_casm,
             ]
             compilation = subprocess.run(
                 compilation_args, capture_output=True, check=False
             )
             if compilation.returncode:
@@ -94,16 +95,16 @@
                 compiled_class = CompiledClass.loads(casm_file.read())
             return compiled_class
 
 
 class ManifestContractClassCompiler(CustomContractClassCompiler):
     """Sierra compiler relying on the compiler repo manifest"""
 
-    def __init__(self, compiler_manifest: str):
-        super().__init__()
+    def __init__(self, compiler_manifest: str, compiler_args: List[str]):
+        super().__init__(compiler_args)
         self._compiler_command = [
             "cargo",
             "run",
             "--bin",
             "starknet-sierra-compile",
             "--manifest-path",
             compiler_manifest,
@@ -113,23 +114,28 @@
     def get_sierra_compiler_command(self) -> List[str]:
         return self._compiler_command
 
 
 class BinaryContractClassCompiler(CustomContractClassCompiler):
     """Sierra compiler relying on the starknet-sierra-compile binary executable"""
 
-    def __init__(self, executable_path: str):
+    def __init__(self, executable_path: str, compiler_args: List[str]):
+        super().__init__(compiler_args)
         self._compiler_command = [executable_path]
 
     def get_sierra_compiler_command(self) -> List[str]:
         return self._compiler_command
 
 
 def select_compiler(config: DevnetConfig) -> ContractClassCompiler:
     """Selects the compiler class according to the specification in the config object"""
     if config.cairo_compiler_manifest:
-        return ManifestContractClassCompiler(config.cairo_compiler_manifest)
+        return ManifestContractClassCompiler(
+            config.cairo_compiler_manifest, config.compiler_args
+        )
 
     if config.sierra_compiler_path:
-        return BinaryContractClassCompiler(config.sierra_compiler_path)
+        return BinaryContractClassCompiler(
+            config.sierra_compiler_path, config.compiler_args
+        )
 
-    return DefaultContractClassCompiler()
+    return DefaultContractClassCompiler(config.compiler_args)
```

### Comparing `starknet_devnet-0.5.3/starknet_devnet/constants.py` & `starknet_devnet-0.5.4/starknet_devnet/constants.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/contract_class_wrapper.py` & `starknet_devnet-0.5.4/starknet_devnet/contract_class_wrapper.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/devnet_config.py` & `starknet_devnet-0.5.4/starknet_devnet/devnet_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from starkware.starknet.services.api.contract_class.contract_class import (
     DeprecatedCompiledClass,
 )
 from starkware.starknet.services.api.feeder_gateway.feeder_gateway_client import (
     FeederGatewayClient,
 )
 
-from starknet_devnet.util import suppress_feeder_gateway_client_logger
+from starknet_devnet.util import suppress_feeder_gateway_client_logger, warn
 
 from . import __version__
 from .constants import (
     DEFAULT_ACCOUNTS,
     DEFAULT_GAS_PRICE,
     DEFAULT_HOST,
     DEFAULT_INITIAL_BALANCE,
@@ -45,14 +45,20 @@
     "alpha-goerli2": "https://alpha4-2.starknet.io",
     "alpha-mainnet": "https://alpha-mainnet.starknet.io",
 }
 NETWORK_NAMES = ", ".join(NETWORK_TO_URL.keys())
 CHAIN_IDS = ", ".join([member.name for member in StarknetChainId])
 DEFAULT_CHAIN_ID = StarknetChainId.TESTNET
 
+DEFAULT_COMPILER_ARGS = [
+    "--add-pythonic-hints",
+    "--allowed-libfuncs-list-name",
+    "experimental_v0.1.0",
+]
+
 
 def _fork_network(network_id: str):
     """
     Return the URL corresponding to the provided name.
     If it's not one of predefined names, assumes it is already a URL.
     """
     return NETWORK_TO_URL.get(network_id, network_id)
@@ -206,14 +212,31 @@
 
         if value <= 0:
             parser.error(error_msg)
 
         setattr(namespace, self.dest, value)
 
 
+class WarnIfDeprecatedArgumentAction(argparse.Action):
+    """
+    Action to warn if user uses old flag;
+    """
+
+    def __init__(self, nargs=0, **kw):
+        super().__init__(nargs=nargs, **kw)
+
+    def __call__(self, parser, namespace, values, option_string=None):
+        if option_string == "--hide-predeployed-accounts":
+            warn(
+                "WARNING: Argument --hide-predeployed-accounts is deprecated; applying --hide-predeployed-contracts instead",
+                file=sys.stderr,
+            )
+        setattr(namespace, self.dest, True)
+
+
 def _assert_valid_compiler(command: List[str]):
     """Assert user machine can compile with cairo 1"""
     check = subprocess.run(
         command,
         check=False,
         capture_output=True,
     )
@@ -246,14 +269,18 @@
     if not (os.path.isfile(compiler_path) and os.access(compiler_path, os.X_OK)):
         sys.exit("Error: The argument of --sierra-compiler-path must be an executable")
 
     _assert_valid_compiler([compiler_path, "--version"])
     return compiler_path
 
 
+def _parse_compiler_args(compiler_args: str):
+    return compiler_args.split()
+
+
 def parse_args(raw_args: List[str]):
     """
     Parses CLI arguments.
     """
     parser = argparse.ArgumentParser(
         description="Run a local instance of Starknet Devnet"
     )
@@ -261,14 +288,24 @@
         "-v",
         "--version",
         help="Print the version",
         action="version",
         version=__version__,
     )
     parser.add_argument(
+        "--verbose",
+        action="store_true",
+        help="Show more verbose output. Has higher priority than --hide-server-logs and --hide-predeployed-contracts",
+    )
+    parser.add_argument(
+        "--hide-server-logs",
+        action="store_true",
+        help="Hide server access logging",
+    )
+    parser.add_argument(
         "--host",
         help=f"Specify the address to listen at; defaults to {DEFAULT_HOST} "
         "(use the address the program outputs on start)",
         default=DEFAULT_HOST,
     )
     parser.add_argument(
         "--port",
@@ -313,17 +350,18 @@
     )
     parser.add_argument(
         "--seed",
         type=int,
         help="Specify the seed for randomness of accounts to be predeployed",
     )
     parser.add_argument(
-        "--hide-predeployed-accounts",
-        action="store_true",
-        help="Prevents from printing the predeployed accounts details",
+        "--hide-predeployed-contracts",
+        "--hide-predeployed-accounts",  # for backwards compatibility
+        action=WarnIfDeprecatedArgumentAction,
+        help="Prevents from printing the predeployed contracts details. Argument --hide-predeployed-accounts is deprecated",
     )
     parser.add_argument(
         "--start-time",
         action=NonNegativeAction,
         help="Specify the start time of the genesis block in Unix time seconds",
     )
     parser.add_argument(
@@ -394,14 +432,23 @@
         "if omitted, the default x86-compatible compiler (from cairo-lang package) is used",
     )
     parser.add_argument(
         "--sierra-compiler-path",
         type=_parse_sierra_compiler_path,
         help="Specify the path to the binary executable of starknet-sierra-compile",
     )
+    parser.add_argument(
+        "--compiler-args",
+        type=_parse_compiler_args,
+        default=DEFAULT_COMPILER_ARGS,
+        help="Specify the CLI args used internally by the Cairo 1.0 compiler for recompiling. "
+        "Provide them as a single space-separated string. "
+        "No validation is done on the arguments on Devnet startup, only when they are put to use. "
+        f"Defaults to '{' '.join(DEFAULT_COMPILER_ARGS)}'",
+    )
 
     parsed_args = parser.parse_args(raw_args)
     if parsed_args.dump_on and not parsed_args.dump_path:
         sys.exit("Error: --dump-path required if --dump-on present")
 
     if parsed_args.fork_block and not parsed_args.fork_network:
         sys.exit("Error: --fork-network required if --fork-block present")
@@ -433,15 +480,17 @@
         self.seed = self.args.seed
         self.start_time = self.args.start_time
         self.gas_price = self.args.gas_price
         self.allow_max_fee_zero = self.args.allow_max_fee_zero
         self.lite_mode = self.args.lite_mode
         self.blocks_on_demand = self.args.blocks_on_demand
         self.account_class = self.args.account_class
-        self.hide_predeployed_accounts = self.args.hide_predeployed_accounts
+        self.hide_predeployed_contracts = self.args.hide_predeployed_contracts
         self.fork_network = self.args.fork_network
         self.fork_block = self.args.fork_block
         self.chain_id = self.args.chain_id
         self.validate_rpc_requests = not self.args.disable_rpc_request_validation
         self.validate_rpc_responses = not self.args.disable_rpc_response_validation
         self.cairo_compiler_manifest = self.args.cairo_compiler_manifest
         self.sierra_compiler_path = self.args.sierra_compiler_path
+        self.compiler_args = self.args.compiler_args
+        self.verbose = self.args.verbose
```

### Comparing `starknet_devnet-0.5.3/starknet_devnet/dump.py` & `starknet_devnet-0.5.4/starknet_devnet/dump.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/fee_token.py` & `starknet_devnet-0.5.4/starknet_devnet/fee_token.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 Fee token and its predefined constants.
 """
+import pprint
+import sys
 
 from starkware.solidity.utils import load_nearby_contract
 from starkware.starknet.business_logic.transaction.objects import InternalInvokeFunction
 from starkware.starknet.compiler.compile import get_selector_from_name
 from starkware.starknet.services.api.contract_class.contract_class import (
     CompiledClassBase,
     DeprecatedCompiledClass,
@@ -12,15 +14,15 @@
 from starkware.starknet.services.api.gateway.transaction import InvokeFunction
 from starkware.starknet.testing.starknet import Starknet
 
 from starknet_devnet.account_util import get_execute_args
 from starknet_devnet.chargeable_account import ChargeableAccount
 from starknet_devnet.constants import SUPPORTED_TX_VERSION
 from starknet_devnet.predeployed_contract_wrapper import PredeployedContractWrapper
-from starknet_devnet.util import Uint256, str_to_felt
+from starknet_devnet.util import Uint256, logger, str_to_felt
 
 
 class FeeToken(PredeployedContractWrapper):
     """Wrapper of token for charging fees."""
 
     CONTRACT_CLASS: CompiledClassBase = None  # loaded lazily
 
@@ -127,18 +129,31 @@
         Mint `amount` tokens at address `to_address`.
         Returns the `tx_hash` (as hex str) if not `lite`; else returns `None`
         """
         amount_uint256 = Uint256.from_felt(amount)
 
         tx_hash = None
         transaction = await self.get_mint_transaction(to_address, amount_uint256)
+        logger.info(transaction)
         starknet: Starknet = self.starknet_wrapper.starknet
         if lite:
             internal_tx = InternalInvokeFunction.from_external(
                 transaction, starknet.state.general_config
             )
-            await starknet.state.execute_tx(internal_tx)
+            execution_info = await starknet.state.execute_tx(internal_tx)
+            logger.info(
+                "transaction execution info: %s", pprint.pformat(execution_info.dump())
+            )
         else:
+            # execution info logs inside starknet_wrapper.invoke call
             _, tx_hash_int = await self.starknet_wrapper.invoke(transaction)
             tx_hash = hex(tx_hash_int)
 
         return tx_hash
+
+    def print(self):
+        print("")
+        print("Predeployed FeeToken")
+        print(f"Address: {hex(self.address)}")
+        print(f"Class Hash: {hex(self.class_hash)}")
+        print(f"Symbol: {self.SYMBOL}\n")
+        sys.stdout.flush()
```

### Comparing `starknet_devnet-0.5.3/starknet_devnet/forked_state.py` & `starknet_devnet-0.5.4/starknet_devnet/forked_state.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/general_config.py` & `starknet_devnet-0.5.4/starknet_devnet/general_config.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/origin.py` & `starknet_devnet-0.5.4/starknet_devnet/origin.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/postman_wrapper.py` & `starknet_devnet-0.5.4/starknet_devnet/postman_wrapper.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/predeployed_contract_wrapper.py` & `starknet_devnet-0.5.4/starknet_devnet/predeployed_contract_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,7 +48,17 @@
         await self._mimic_constructor()
 
         self.contract = StarknetContract(
             state=starknet.state,
             abi=self.contract_class.abi,
             contract_address=self.address,
         )
+
+        if (
+            self.starknet_wrapper.config.verbose
+            or not self.starknet_wrapper.config.hide_predeployed_contracts
+        ):
+            self.print()
+
+    def print(self):
+        """Prints contract info"""
+        raise NotImplementedError()
```

### Comparing `starknet_devnet-0.5.3/starknet_devnet/server.py` & `starknet_devnet-0.5.4/starknet_devnet/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,22 +53,23 @@
         self.cfg.set("workers", 1)
         self.cfg.set("timeout", self.args.timeout)
         self.cfg.set(
             "logconfig_dict",
             {
                 "loggers": {
                     "gunicorn.error": {
-                        # Disable info messages like "Starting gunicorn"
-                        "level": "WARNING",
+                        "level": "INFO" if self.args.verbose else "WARNING",
                         "handlers": ["error_console"],
                         "propagate": False,
                         "qualname": "gunicorn.error",
                     },
                     "gunicorn.access": {
-                        "level": "INFO",
+                        "level": "INFO"
+                        if self.args.verbose or not self.args.hide_server_logs
+                        else "WARNING",
                         # Log access to stderr to maintain backward compatibility
                         "handlers": ["error_console"],
                         "propagate": False,
                         "qualname": "gunicorn.access",
                     },
                 },
             },
```

### Comparing `starknet_devnet-0.5.3/starknet_devnet/starknet_wrapper.py` & `starknet_devnet-0.5.4/starknet_devnet/starknet_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # pylint: disable=too-many-lines
 """
 This module introduces `StarknetWrapper`, a wrapper class of
 starkware.starknet.testing.starknet.Starknet.
 """
+import pprint
 from copy import deepcopy
 from types import TracebackType
 from typing import Dict, List, Optional, Set, Tuple, Type, Union
 
 import cloudpickle as pickle
 from starkware.starknet.business_logic.state.state import BlockInfo, CachedState
 from starkware.starknet.business_logic.transaction.fee import calculate_tx_fee
@@ -101,14 +102,15 @@
     enable_pickling,
     get_all_declared_cairo0_classes,
     get_all_declared_cairo1_classes,
     get_fee_estimation_info,
     get_replaced_classes,
     get_storage_diffs,
     group_classes_by_version,
+    logger,
     warn,
 )
 
 enable_pickling()
 
 DEFAULT_BLOCK_ID = LATEST_BLOCK_ID
 
@@ -507,14 +509,22 @@
                     self.starknet_wrapper._store_transaction(transaction)
 
                     await self.starknet_wrapper.update_pending_block(state_update)
 
                     if not self.starknet_wrapper.config.blocks_on_demand:
                         await self.starknet_wrapper.generate_latest_block()
 
+                logger.info(
+                    "transaction execution info: %s",
+                    pprint.pformat(self.execution_info.dump()),
+                )
+                logger.info(
+                    "transaction receipt: %s",
+                    pprint.pformat(transaction.get_receipt().dump()),
+                )
                 return True  # indicates the caught exception was handled successfully
 
         return TransactionHandler(self)
 
     async def deploy_account(self, external_tx: DeployAccount):
         """Deploys account and returns (address, tx_hash)"""
 
@@ -936,14 +946,17 @@
         state = await self.__get_query_state(block_id)
         return await state.state.get_nonce_at(contract_address)
 
     async def __predeclare_starknet_cli_account(self):
         """Predeclares the account class used by Starknet CLI"""
         state = self.get_state().state
         state.compiled_classes[STARKNET_CLI_ACCOUNT_CLASS_HASH] = oz_account_class
+        if self.config.verbose or not self.config.hide_predeployed_contracts:
+            print("Predeclared Starknet CLI account: ", flush=True)
+            print(f"Class hash: {hex(STARKNET_CLI_ACCOUNT_CLASS_HASH)}\n", flush=True)
 
     async def __deploy_chargeable_account(self):
         if await self.is_deployed(ChargeableAccount.ADDRESS):
             warn("Chargeable account already deployed")
         else:
             await ChargeableAccount(self).deploy()
```

### Comparing `starknet_devnet-0.5.3/starknet_devnet/state.py` & `starknet_devnet-0.5.4/starknet_devnet/state.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/state_archive.py` & `starknet_devnet-0.5.4/starknet_devnet/state_archive.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/transactions.py` & `starknet_devnet-0.5.4/starknet_devnet/transactions.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.3/starknet_devnet/udc.py` & `starknet_devnet-0.5.4/starknet_devnet/udc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """UDC and its constants"""
 
+import sys
+
 from starkware.solidity.utils import load_nearby_contract
 from starkware.starknet.services.api.contract_class.contract_class import (
     CompiledClassBase,
     DeprecatedCompiledClass,
 )
 
 from starknet_devnet.predeployed_contract_wrapper import PredeployedContractWrapper
@@ -40,7 +42,13 @@
     @property
     def contract_class(self) -> CompiledClassBase:
         """Same as `get_contract_class`, used by `PredeployedContractWrapper` parent"""
         return self.get_contract_class()
 
     async def _mimic_constructor(self):
         pass
+
+    def print(self):
+        print("Predeployed UDC")
+        print(f"Address: {hex(self.address)}")
+        print(f"Class Hash: {hex(self.class_hash)}\n")
+        sys.stdout.flush()
```

### Comparing `starknet_devnet-0.5.3/starknet_devnet/util.py` & `starknet_devnet-0.5.4/starknet_devnet/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 """
 Utility functions used across the project.
 """
+import functools
+import json
 import logging
 import os
+import pprint
 import sys
 from dataclasses import dataclass
 from typing import Dict, List, Set, Tuple
 
+from flask import request
 from starkware.starknet.business_logic.state.state import CachedState
 from starkware.starknet.definitions.error_codes import StarknetErrorCode
 from starkware.starknet.services.api.feeder_gateway.response_objects import (
     ClassHashPair,
     ContractAddressHashPair,
     FeeEstimationInfo,
     StorageEntry,
@@ -259,7 +263,75 @@
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.logger.disabled = False
 
 
 # FeederGatewayClient is implemented in such a way that it logs and raises;
 # this suppresses the logging
 suppress_feeder_gateway_client_logger = LogSuppressor("services.external_api.client")
+
+logger = logging.getLogger("gunicorn.error")
+
+
+def extract_transaction_info_to_log(transaction: dict) -> dict:
+    """Getting info about transaction for logging"""
+    keys_to_exclude = [
+        "contract_class",  # mainly unreadable data
+    ]
+    to_log = {}
+    for key, val in transaction.items():
+        if key not in keys_to_exclude:
+            if isinstance(val, dict):
+                val = extract_transaction_info_to_log(val)
+            to_log[key] = val
+
+    return to_log
+
+
+def log_request(rpc=False):
+    "decorator to log endpoint request, response"
+
+    def decorator(func):
+        @functools.wraps(func)
+        async def wrapper(*args, **kwargs):
+            if rpc:
+                logger.info(
+                    "%s RPC request: %s",
+                    func.__name__,
+                    pprint.pformat(extract_transaction_info_to_log(kwargs)),
+                )
+            else:
+                logger.info(
+                    "%s request: %s",
+                    func.__name__,
+                    pprint.pformat(
+                        extract_transaction_info_to_log(json.loads(request.get_data()))
+                    ),
+                )
+            try:
+                resp = await func(*args, **kwargs)
+                if rpc:
+                    logger.info(
+                        "%s RPC response: %s", func.__name__, pprint.pformat(resp)
+                    )
+                else:
+                    logger.info(
+                        "%s response: %s",
+                        func.__name__,
+                        pprint.pformat(resp.get_json()),
+                    )
+                return resp
+            except Exception:
+                exc_type, exc_val, exc_tb = sys.exc_info()
+                if isinstance(exc_type, StarkException):
+                    error_message = {
+                        "message": exc_val.message,
+                        "code": str(exc_val.code),
+                        "trace": exc_tb,
+                    }
+                else:
+                    error_message = {"message": str(exc_val), "trace": exc_tb}
+                logger.error("%s request failed: %s", func.__name__, error_message)
+                raise
+
+        return wrapper
+
+    return decorator
```

### Comparing `starknet_devnet-0.5.3/setup.py` & `starknet_devnet-0.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
  'web3>=6.0.0,<6.1.0']
 
 entry_points = \
 {'console_scripts': ['starknet-devnet = starknet_devnet.server:main']}
 
 setup_kwargs = {
     'name': 'starknet-devnet',
-    'version': '0.5.3',
+    'version': '0.5.4',
     'description': 'A local testnet for Starknet',
     'long_description': '<!-- logo / title -->\n<p align="center" style="margin-bottom: 0px !important">\n  <img width="200" src="https://user-images.githubusercontent.com/2848732/193076972-da6fa36e-11f7-4cb3-aa29-673224f8576d.png" alt="Devnet" align="center">\n</p>\n<h1 align="center" style="margin-top: 0px !important">Starknet Devnet</h1>\n\nA Flask wrapper of Starknet state. Similar in purpose to Ganache.\n\nAims to mimic Starknet\'s Alpha testnet, but with simplified functionality.\n\n## 🌐 Docs\n\nOn the following links you can find the documentation of:\n\n- [the latest official release](https://0xspaceshard.github.io/starknet-devnet/)\n- [the latest master commit (not officially released)](https://github.com/0xSpaceShard/starknet-devnet/tree/master/page/docs)\n\n## ✏️ Contributing\n\nWe ❤️ and encourage all contributions!\n\n[Click here](https://0xspaceshard.github.io/starknet-devnet/docs/guide/development) for the development guide.\n\n## 🙌 Special Thanks\n\nSpecial thanks to all the [contributors](https://github.com/0xSpaceShard/starknet-devnet/graphs/contributors)!\n',
     'author': 'FabijanC',
     'author_email': 'fabijan.corak@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/0xSpaceShard/starknet-devnet',
```

### Comparing `starknet_devnet-0.5.3/PKG-INFO` & `starknet_devnet-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starknet-devnet
-Version: 0.5.3
+Version: 0.5.4
 Summary: A local testnet for Starknet
 Home-page: https://github.com/0xSpaceShard/starknet-devnet
 License: MIT
 Keywords: starknet,cairo,testnet,local,server
 Author: FabijanC
 Author-email: fabijan.corak@gmail.com
 Requires-Python: >=3.9,<3.10
```

