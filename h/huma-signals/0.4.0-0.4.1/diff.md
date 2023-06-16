# Comparing `tmp/huma_signals-0.4.0.tar.gz` & `tmp/huma_signals-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huma_signals-0.4.0.tar", max compression
+gzip compressed data, was "huma_signals-0.4.1.tar", max compression
```

## Comparing `huma_signals-0.4.0.tar` & `huma_signals-0.4.1.tar`

### file list

```diff
@@ -1,56 +1,51 @@
--rw-r--r--   0        0        0    34523 2023-06-13 21:53:22.735692 huma_signals-0.4.0/LICENSE
--rw-r--r--   0        0        0     2162 2023-06-13 21:53:22.735692 huma_signals-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/__init__.py
--rw-r--r--   0        0        0      586 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/ethereum_wallet/README.md
--rw-r--r--   0        0        0        0 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/ethereum_wallet/__init__.py
--rw-r--r--   0        0        0     3088 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/ethereum_wallet/adapter.py
--rw-r--r--   0        0        0      186 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/ethereum_wallet/settings.py
--rw-r--r--   0        0        0      586 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/lending_pools/README.md
--rw-r--r--   0        0        0        0 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/lending_pools/__init__.py
--rw-r--r--   0        0        0    23699 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/lending_pools/abi/BaseCreditPool.json
--rw-r--r--   0        0        0    30632 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/lending_pools/abi/BasePoolConfig.json
--rw-r--r--   0        0        0    32155 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/lending_pools/abi/ReceivableFactoringPool.json
--rw-r--r--   0        0        0    30290 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/lending_pools/abi/SuperfluidFactoringPool.json
--rw-r--r--   0        0        0     4533 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/lending_pools/adapter.py
--rw-r--r--   0        0        0     1938 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/lending_pools/registry.py
--rw-r--r--   0        0        0      158 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/lending_pools/settings.py
--rw-r--r--   0        0        0      145 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/models.py
--rw-r--r--   0        0        0      591 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/polygon_wallet/README.md
--rw-r--r--   0        0        0        0 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/polygon_wallet/__init__.py
--rw-r--r--   0        0        0     3201 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/polygon_wallet/adapter.py
--rw-r--r--   0        0        0      222 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/polygon_wallet/settings.py
--rw-r--r--   0        0        0      576 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/request_network/README.md
--rw-r--r--   0        0        0        0 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/request_network/__init__.py
--rw-r--r--   0        0        0     4156 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/request_network/models.py
--rw-r--r--   0        0        0     5466 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/request_network/request_invoice_adapter.py
--rw-r--r--   0        0        0     4930 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/request_network/request_transaction_adapter.py
--rw-r--r--   0        0        0      284 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/request_network/settings.py
--rw-r--r--   0        0        0        0 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/superfluid/__init__.py
--rw-r--r--   0        0        0      238 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/superfluid/settings.py
--rw-r--r--   0        0        0     4252 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/superfluid/superfluid_adapter.py
--rw-r--r--   0        0        0      501 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/adapters/superfluid/superfluid_models.py
--rw-r--r--   0        0        0        0 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/clients/eth_client/__init__.py
--rw-r--r--   0        0        0     1427 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/clients/eth_client/eth_client.py
--rw-r--r--   0        0        0      673 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/clients/eth_client/eth_types.py
--rw-r--r--   0        0        0        0 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/clients/polygon_client/__init__.py
--rw-r--r--   0        0        0     1503 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/clients/polygon_client/polygon_client.py
--rw-r--r--   0        0        0      685 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/clients/polygon_client/polygon_types.py
--rw-r--r--   0        0        0        0 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/clients/request_client/__init__.py
--rw-r--r--   0        0        0     8250 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/clients/request_client/request_client.py
--rw-r--r--   0        0        0      978 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/clients/request_client/request_types.py
--rw-r--r--   0        0        0        0 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/commons/__init__.py
--rw-r--r--   0        0        0      291 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/commons/chains.py
--rw-r--r--   0        0        0      330 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/commons/datetime_utils.py
--rw-r--r--   0        0        0      227 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/commons/pydantic_utils.py
--rw-r--r--   0        0        0      569 2023-06-13 21:53:22.735692 huma_signals-0.4.0/huma_signals/commons/string_utils.py
--rw-r--r--   0        0        0     1309 2023-06-13 21:53:22.739692 huma_signals-0.4.0/huma_signals/commons/tokens.py
--rw-r--r--   0        0        0     1078 2023-06-13 21:53:22.739692 huma_signals-0.4.0/huma_signals/commons/web3_utils.py
--rw-r--r--   0        0        0      499 2023-06-13 21:53:22.739692 huma_signals-0.4.0/huma_signals/dotenv/example.env
--rw-r--r--   0        0        0     1157 2023-06-13 21:53:22.739692 huma_signals-0.4.0/huma_signals/exceptions.py
--rw-r--r--   0        0        0      322 2023-06-13 21:53:22.739692 huma_signals-0.4.0/huma_signals/models.py
--rw-r--r--   0        0        0        0 2023-06-13 21:53:22.739692 huma_signals-0.4.0/huma_signals/py.typed
--rw-r--r--   0        0        0     1563 2023-06-13 21:53:22.739692 huma_signals-0.4.0/huma_signals/settings.py
--rw-r--r--   0        0        0     2792 2023-06-13 21:53:22.739692 huma_signals-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 huma_signals-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-16 00:13:36.301640 huma_signals-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2162 2023-06-16 00:13:36.301640 huma_signals-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-16 00:13:36.301640 huma_signals-0.4.1/huma_signals/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 00:13:36.301640 huma_signals-0.4.1/huma_signals/adapters/__init__.py
+-rw-r--r--   0        0        0      586 2023-06-16 00:13:36.301640 huma_signals-0.4.1/huma_signals/adapters/ethereum_wallet/README.md
+-rw-r--r--   0        0        0        0 2023-06-16 00:13:36.301640 huma_signals-0.4.1/huma_signals/adapters/ethereum_wallet/__init__.py
+-rw-r--r--   0        0        0     3079 2023-06-16 00:13:36.301640 huma_signals-0.4.1/huma_signals/adapters/ethereum_wallet/adapter.py
+-rw-r--r--   0        0        0      186 2023-06-16 00:13:36.301640 huma_signals-0.4.1/huma_signals/adapters/ethereum_wallet/settings.py
+-rw-r--r--   0        0        0      586 2023-06-16 00:13:36.301640 huma_signals-0.4.1/huma_signals/adapters/lending_pools/README.md
+-rw-r--r--   0        0        0        0 2023-06-16 00:13:36.301640 huma_signals-0.4.1/huma_signals/adapters/lending_pools/__init__.py
+-rw-r--r--   0        0        0    23699 2023-06-16 00:13:36.301640 huma_signals-0.4.1/huma_signals/adapters/lending_pools/abi/BaseCreditPool.json
+-rw-r--r--   0        0        0    30632 2023-06-16 00:13:36.301640 huma_signals-0.4.1/huma_signals/adapters/lending_pools/abi/BasePoolConfig.json
+-rw-r--r--   0        0        0    32155 2023-06-16 00:13:36.301640 huma_signals-0.4.1/huma_signals/adapters/lending_pools/abi/ReceivableFactoringPool.json
+-rw-r--r--   0        0        0    30290 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/lending_pools/abi/SuperfluidFactoringPool.json
+-rw-r--r--   0        0        0     4523 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/lending_pools/adapter.py
+-rw-r--r--   0        0        0     1963 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/lending_pools/registry.py
+-rw-r--r--   0        0        0      158 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/lending_pools/settings.py
+-rw-r--r--   0        0        0      145 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/models.py
+-rw-r--r--   0        0        0      591 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/polygon_wallet/README.md
+-rw-r--r--   0        0        0        0 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/polygon_wallet/__init__.py
+-rw-r--r--   0        0        0     3191 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/polygon_wallet/adapter.py
+-rw-r--r--   0        0        0      222 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/polygon_wallet/settings.py
+-rw-r--r--   0        0        0      576 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/request_network/README.md
+-rw-r--r--   0        0        0        0 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/request_network/__init__.py
+-rw-r--r--   0        0        0     4156 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/request_network/models.py
+-rw-r--r--   0        0        0     5481 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/request_network/request_invoice_adapter.py
+-rw-r--r--   0        0        0     4945 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/request_network/request_transaction_adapter.py
+-rw-r--r--   0        0        0      283 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/request_network/settings.py
+-rw-r--r--   0        0        0        0 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/superfluid/__init__.py
+-rw-r--r--   0        0        0      237 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/superfluid/settings.py
+-rw-r--r--   0        0        0     4252 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/superfluid/superfluid_adapter.py
+-rw-r--r--   0        0        0      491 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/superfluid/superfluid_models.py
+-rw-r--r--   0        0        0        0 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/clients/eth_client/__init__.py
+-rw-r--r--   0        0        0     1427 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/clients/eth_client/eth_client.py
+-rw-r--r--   0        0        0      662 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/clients/eth_client/eth_types.py
+-rw-r--r--   0        0        0        0 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/clients/polygon_client/__init__.py
+-rw-r--r--   0        0        0     1503 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/clients/polygon_client/polygon_client.py
+-rw-r--r--   0        0        0      674 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/clients/polygon_client/polygon_types.py
+-rw-r--r--   0        0        0        0 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/clients/request_client/__init__.py
+-rw-r--r--   0        0        0     8282 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/clients/request_client/request_client.py
+-rw-r--r--   0        0        0      978 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/clients/request_client/request_types.py
+-rw-r--r--   0        0        0        0 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/commons/__init__.py
+-rw-r--r--   0        0        0     1324 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/commons/tokens.py
+-rw-r--r--   0        0        0      499 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/dotenv/example.env
+-rw-r--r--   0        0        0     1157 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/exceptions.py
+-rw-r--r--   0        0        0      322 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/models.py
+-rw-r--r--   0        0        0        0 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/py.typed
+-rw-r--r--   0        0        0     1562 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/settings.py
+-rw-r--r--   0        0        0     2814 2023-06-16 00:13:36.305640 huma_signals-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3153 1970-01-01 00:00:00.000000 huma_signals-0.4.1/PKG-INFO
```

### Comparing `huma_signals-0.4.0/LICENSE` & `huma_signals-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.0/README.md` & `huma_signals-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.0/huma_signals/adapters/ethereum_wallet/README.md` & `huma_signals-0.4.1/huma_signals/adapters/ethereum_wallet/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.0/huma_signals/adapters/ethereum_wallet/adapter.py` & `huma_signals-0.4.1/huma_signals/adapters/ethereum_wallet/adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import datetime
 from typing import Any
 
+from huma_utils import datetime_utils
+
 from huma_signals import models
 from huma_signals.adapters import models as adapter_models
 from huma_signals.adapters.ethereum_wallet.settings import settings
 from huma_signals.clients.eth_client import eth_client, eth_types
-from huma_signals.commons import datetime_utils
 
 
 class EthereumWalletSignals(models.HumaBaseModel):
     total_transactions: int
     total_sent: int
     total_received: int
     wallet_tenure_in_days: int
```

### Comparing `huma_signals-0.4.0/huma_signals/adapters/lending_pools/README.md` & `huma_signals-0.4.1/huma_signals/adapters/lending_pools/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.0/huma_signals/adapters/lending_pools/abi/BaseCreditPool.json` & `huma_signals-0.4.1/huma_signals/adapters/lending_pools/abi/BaseCreditPool.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.0/huma_signals/adapters/lending_pools/abi/BasePoolConfig.json` & `huma_signals-0.4.1/huma_signals/adapters/lending_pools/abi/BasePoolConfig.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.0/huma_signals/adapters/lending_pools/abi/ReceivableFactoringPool.json` & `huma_signals-0.4.1/huma_signals/adapters/lending_pools/abi/ReceivableFactoringPool.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.0/huma_signals/adapters/lending_pools/abi/SuperfluidFactoringPool.json` & `huma_signals-0.4.1/huma_signals/adapters/lending_pools/abi/SuperfluidFactoringPool.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.0/huma_signals/adapters/lending_pools/adapter.py` & `huma_signals-0.4.1/huma_signals/adapters/lending_pools/adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from typing import Any, ClassVar
 
 import aiofiles
 import orjson
 import pydantic
 import structlog
 import web3
+from huma_utils import web3_utils
 from web3 import exceptions as web3_exceptions
 
 from huma_signals import exceptions, models
 from huma_signals.adapters import models as adapter_models
 from huma_signals.adapters.lending_pools import registry
 from huma_signals.adapters.lending_pools.settings import settings
-from huma_signals.commons import web3_utils
 
 logger = structlog.get_logger(__name__)
 
 
 class LendingPoolSignals(models.HumaBaseModel):
     # TODO: add other pool signals: utilization, liquidity, etc.
     # Pool policy signals
```

### Comparing `huma_signals-0.4.0/huma_signals/adapters/lending_pools/registry.py` & `huma_signals-0.4.1/huma_signals/adapters/lending_pools/registry.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,68 +1,68 @@
 import pathlib
 
 import eth_typing
 import web3
+from huma_utils import chain_utils
 
 from huma_signals import models
-from huma_signals.commons import chains
 
 
 class PoolSetting(models.HumaBaseModel):
     pool_address: eth_typing.ChecksumAddress
-    chain: chains.Chain
+    chain: chain_utils.Chain
     pool_abi_path: str
 
 
 _POOLS = [
     PoolSetting(
         pool_address=web3.Web3.to_checksum_address(
             "0xA22D20FB0c9980fb96A9B0B5679C061aeAf5dDE4"
         ),
-        chain=chains.Chain.GOERLI,
+        chain=chain_utils.Chain.GOERLI,
         pool_abi_path=str(
             pathlib.Path(__file__).parent.resolve() / "abi" / "BaseCreditPool.json"
         ),
     ),
     PoolSetting(
         pool_address=web3.Web3.to_checksum_address(
             "0x11672c0bBFF498c72BC2200f42461c0414855042"
         ),
-        chain=chains.Chain.GOERLI,
+        chain=chain_utils.Chain.GOERLI,
         pool_abi_path=str(
             pathlib.Path(__file__).parent.resolve()
             / "abi"
             / "ReceivableFactoringPool.json"
         ),
     ),
     PoolSetting(
         pool_address=web3.Web3.to_checksum_address(
             "0xC5BF9750A7BF93479990EF940d7e3984caa22558"
         ),
-        chain=chains.Chain.MUMBAI,
+        chain=chain_utils.Chain.MUMBAI,
         pool_abi_path=str(
             pathlib.Path(__file__).parent.resolve()
             / "abi"
             / "SuperfluidFactoringPool.json"
         ),
     ),
     PoolSetting(
         pool_address=web3.Web3.to_checksum_address(
             "0xAb3dc5221F373Dd879BEc070058c775A0f6Af759"
         ),
-        chain=chains.Chain.POLYGON,
+        chain=chain_utils.Chain.POLYGON,
         pool_abi_path=str(
             pathlib.Path(__file__).parent.resolve() / "abi" / "BaseCreditPool.json"
         ),
     ),
     PoolSetting(
         pool_address=web3.Web3.to_checksum_address(
             "0x58AAF1f9cB10F335111A2129273056bbED251B61"
         ),
-        chain=chains.Chain.POLYGON,
+        chain=chain_utils.Chain.POLYGON,
         pool_abi_path=str(
             pathlib.Path(__file__).parent.resolve()
             / "abi"
             / "ReceivableFactoringPool.json"
         ),
     ),
 ]
```

### Comparing `huma_signals-0.4.0/huma_signals/adapters/polygon_wallet/README.md` & `huma_signals-0.4.1/huma_signals/adapters/polygon_wallet/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.0/huma_signals/adapters/polygon_wallet/adapter.py` & `huma_signals-0.4.1/huma_signals/adapters/polygon_wallet/adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import datetime
 from typing import Any
 
 import structlog
+from huma_utils import datetime_utils
 
 from huma_signals import models
 from huma_signals.adapters import models as adapter_models
 from huma_signals.adapters.polygon_wallet.settings import settings
 from huma_signals.clients.polygon_client import polygon_client, polygon_types
-from huma_signals.commons import datetime_utils
 
 logger = structlog.get_logger()
 
 
 class PolygonWalletSignals(models.HumaBaseModel):
     total_transactions: int
     total_sent: int
```

### Comparing `huma_signals-0.4.0/huma_signals/adapters/request_network/README.md` & `huma_signals-0.4.1/huma_signals/adapters/request_network/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.0/huma_signals/adapters/request_network/models.py` & `huma_signals-0.4.1/huma_signals/adapters/request_network/models.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.0/huma_signals/adapters/request_network/request_invoice_adapter.py` & `huma_signals-0.4.1/huma_signals/adapters/request_network/request_invoice_adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import datetime
 from typing import Any
 
 import pandas as pd
 import structlog
 import web3
+from huma_utils import chain_utils
 
 from huma_signals import exceptions
 from huma_signals.adapters import models as adapter_models
 from huma_signals.adapters.ethereum_wallet import adapter as ethereum_wallet_adapter
 from huma_signals.adapters.polygon_wallet import adapter as polygon_wallet_adapter
 from huma_signals.adapters.request_network import models
 from huma_signals.adapters.request_network.settings import settings
 from huma_signals.clients.request_client import request_client
-from huma_signals.commons import chains
 
 logger = structlog.get_logger(__name__)
 
 _WALLET_ADAPTER_BY_CHAIN = {
-    chains.Chain.ETHEREUM: ethereum_wallet_adapter.EthereumWalletAdapter,
-    chains.Chain.GOERLI: ethereum_wallet_adapter.EthereumWalletAdapter,
-    chains.Chain.POLYGON: polygon_wallet_adapter.PolygonWalletAdapter,
+    chain_utils.Chain.ETHEREUM: ethereum_wallet_adapter.EthereumWalletAdapter,
+    chain_utils.Chain.GOERLI: ethereum_wallet_adapter.EthereumWalletAdapter,
+    chain_utils.Chain.POLYGON: polygon_wallet_adapter.PolygonWalletAdapter,
 }
 
 
 class RequestInvoiceAdapter(adapter_models.SignalAdapterBase):
     def __init__(  # pylint: disable=too-many-arguments
         self,
         request_client_: request_client.BaseRequestClient | None = None,
         wallet_adapter: ethereum_wallet_adapter.BaseEthereumWalletAdapter
         | polygon_wallet_adapter.BasePolygonWalletAdapter
         | None = None,
         request_network_subgraph_endpoint_url: str = settings.request_network_subgraph_endpoint_url,
         invoice_api_url: str = settings.request_network_invoice_api_url,
-        chain: chains.Chain = settings.chain,
+        chain: chain_utils.Chain = settings.chain,
     ) -> None:
         self.request_client = request_client_ or request_client.RequestClient(
             request_network_subgraph_endpoint_url=request_network_subgraph_endpoint_url,
             invoice_api_url=invoice_api_url,
         )
         self.chain = chain
         if wallet_adapter is not None:
```

### Comparing `huma_signals-0.4.0/huma_signals/adapters/request_network/request_transaction_adapter.py` & `huma_signals-0.4.1/huma_signals/adapters/request_network/request_transaction_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from typing import Any
 
 import pandas as pd
 import structlog
 import web3
+from huma_utils import chain_utils
 
 from huma_signals import exceptions
 from huma_signals.adapters import models as adapter_models
 from huma_signals.adapters.ethereum_wallet import adapter as ethereum_wallet_adapter
 from huma_signals.adapters.polygon_wallet import adapter as polygon_wallet_adapter
 from huma_signals.adapters.request_network import models
 from huma_signals.adapters.request_network.settings import settings
 from huma_signals.clients.request_client import request_client
-from huma_signals.commons import chains
 
 logger = structlog.get_logger(__name__)
 
 _WALLET_ADAPTER_BY_CHAIN = {
-    chains.Chain.ETHEREUM: ethereum_wallet_adapter.EthereumWalletAdapter,
-    chains.Chain.GOERLI: ethereum_wallet_adapter.EthereumWalletAdapter,
-    chains.Chain.POLYGON: polygon_wallet_adapter.PolygonWalletAdapter,
+    chain_utils.Chain.ETHEREUM: ethereum_wallet_adapter.EthereumWalletAdapter,
+    chain_utils.Chain.GOERLI: ethereum_wallet_adapter.EthereumWalletAdapter,
+    chain_utils.Chain.POLYGON: polygon_wallet_adapter.PolygonWalletAdapter,
 }
 
 
 class RequestTransactionAdapter(adapter_models.SignalAdapterBase):
     def __init__(  # pylint: disable=too-many-arguments
         self,
         request_client_: request_client.BaseRequestClient | None = None,
         wallet_adapter: ethereum_wallet_adapter.BaseEthereumWalletAdapter
         | polygon_wallet_adapter.BasePolygonWalletAdapter
         | None = None,
         request_network_subgraph_endpoint_url: str = settings.request_network_subgraph_endpoint_url,
         invoice_api_url: str = settings.request_network_invoice_api_url,
-        chain: chains.Chain = settings.chain,
+        chain: chain_utils.Chain = settings.chain,
     ) -> None:
         self.request_client = request_client_ or request_client.RequestClient(
             request_network_subgraph_endpoint_url=request_network_subgraph_endpoint_url,
             invoice_api_url=invoice_api_url,
         )
         self.chain = chain
         if wallet_adapter is not None:
```

### Comparing `huma_signals-0.4.0/huma_signals/adapters/superfluid/superfluid_adapter.py` & `huma_signals-0.4.1/huma_signals/adapters/superfluid/superfluid_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import httpx
 import structlog
 import web3
+from huma_utils import chain_utils
 
 from huma_signals import exceptions
 from huma_signals.adapters import models as adapter_models
 from huma_signals.adapters.superfluid import superfluid_models
 from huma_signals.adapters.superfluid.settings import settings
-from huma_signals.commons import chains
 
 logger = structlog.get_logger()
 
 
 _CURRENT_STREAM_QUERY = """
 query HumaCurrentStream($sender: String, $receiver: String, $token: String) {
     streams(
@@ -33,15 +33,15 @@
 """
 
 
 class SuperfluidAdapter(adapter_models.SignalAdapterBase):
     def __init__(
         self,
         superfluid_subgraph_endpoint_url: str = settings.superfluid_subgraph_endpoint_url,
-        chain: chains.Chain = settings.chain,
+        chain: chain_utils.Chain = settings.chain,
     ) -> None:
         self.superfluid_subgraph_endpoint_url = superfluid_subgraph_endpoint_url
         self.chain = chain
 
     async def fetch(  # pylint: disable=arguments-differ
         self,
         borrower_wallet_address: str,
```

### Comparing `huma_signals-0.4.0/huma_signals/clients/eth_client/eth_client.py` & `huma_signals-0.4.1/huma_signals/clients/eth_client/eth_client.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.0/huma_signals/clients/eth_client/eth_types.py` & `huma_signals-0.4.1/huma_signals/clients/eth_client/eth_types.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import pydantic
-
-from huma_signals.commons import pydantic_utils
+from huma_utils import pydantic_utils
 
 
 class EthTransaction(pydantic_utils.CamelCaseAliased):
     block_number: str
     time_stamp: str
     hash: str
     nonce: str
```

### Comparing `huma_signals-0.4.0/huma_signals/clients/polygon_client/polygon_client.py` & `huma_signals-0.4.1/huma_signals/clients/polygon_client/polygon_client.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.0/huma_signals/clients/request_client/request_client.py` & `huma_signals-0.4.1/huma_signals/clients/request_client/request_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 import decimal
 from typing import Any, Protocol
 
 import httpx
 import pandas as pd
 import structlog
 import web3
+from huma_utils import chain_utils
 
 from huma_signals import exceptions
 from huma_signals.clients.request_client import request_types
-from huma_signals.commons import chains, tokens
+from huma_signals.commons import tokens
 
 logger = structlog.get_logger(__name__)
 
 _DEFAULT_GRAPHQL_CHUNK_SIZE = 1000
 
 
 class BaseRequestClient(Protocol):
@@ -25,15 +26,15 @@
         pass
 
     async def get_invoice(self, request_id: str) -> request_types.Invoice:
         pass
 
     @classmethod
     def enrich_payments_data(
-        cls, payments_raw_df: pd.DataFrame, chain: chains.Chain
+        cls, payments_raw_df: pd.DataFrame, chain: chain_utils.Chain
     ) -> pd.DataFrame:
         """
         Enriches the raw payments data with additional information
         """
         if len(payments_raw_df) == 0:
             return pd.DataFrame(
                 columns=[
```

### Comparing `huma_signals-0.4.0/huma_signals/clients/request_client/request_types.py` & `huma_signals-0.4.1/huma_signals/clients/request_client/request_types.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.0/huma_signals/commons/tokens.py` & `huma_signals-0.4.1/huma_signals/commons/tokens.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from huma_signals.commons import chains
+from huma_utils import chain_utils
 
 TOKEN_ADDRESS_MAPPING = {
-    chains.Chain.ETHEREUM: {
+    chain_utils.Chain.ETHEREUM: {
         "0xa0b86991c6218b36c1d19d4a2e9eb0ce3606eb48": "USDC",
         "0x6b175474e89094c44da98b954eedeac495271d0f": "DAI",
         "0xdac17f958d2ee523a2206206994597c13d831ec7": "USDT",
         # "0x3845badade8e6dff049820680d1f14bd3903a5d0": "SAND",
         # "0xc944e90c64b2c07662a292be6244bdf05cda44a7": "GRT",
         # "0x967da4048cd07ab37855c090aaf366e4ce1b9f48": "OCEAN",
         # "0x8f8221afbb33998d8584a2b05749ba73c37a938a": "REQ",
     },
-    chains.Chain.POLYGON: {
+    chain_utils.Chain.POLYGON: {
         "0x2791bca1f2de4661ed88a30c99a7a9449aa84174": "USDC",
         "0x8f3cf7ad23cd3cadbd9735aff958023239c6a063": "DAI",
         "0xc2132d05d31c914a87c6611c10748aeb04b58e8f": "USDT",
     },
-    chains.Chain.GOERLI: {
+    chain_utils.Chain.GOERLI: {
         "0x07865c6e87b9f70255377e024ace6630c1eaa37f": "USDC",
         "0xdc31ee1784292379fbb2964b3b9c4124d8f89c60": "DAI",
         "0x56705db9f87c8a930ec87da0d458e00a657fccb0": "USDT",
     },
-    chains.Chain.MUMBAI: {
+    chain_utils.Chain.MUMBAI: {
         "0xe6b8a5cf854791412c1f6efc7caf629f5df1c747": "USDC",
         "0xa02f6adc7926efebbd59fd43a84f4e0c0c91e832": "USDT",
         "0xd393b1e02da9831ff419e22ea105aae4c47e1253": "DAI",
     },
 }
 
 TOKEN_USD_PRICE_MAPPING = {
```

### Comparing `huma_signals-0.4.0/huma_signals/exceptions.py` & `huma_signals-0.4.1/huma_signals/exceptions.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.0/huma_signals/settings.py` & `huma_signals-0.4.1/huma_signals/settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import enum
 import os
 import pathlib
 
 import dotenv
 import pydantic
-
-from huma_signals.commons import chains
+from huma_utils import chain_utils
 
 
 class Env(str, enum.Enum):
     DEVELOPMENT = "development"
     TEST = "test"
     STAGING = "staging"
     TESTNET = "testnet"
@@ -36,15 +35,15 @@
 
 
 class Settings(pydantic.BaseSettings):
     class Config:
         case_sensitive = False
 
     env: str
-    chain: chains.Chain
+    chain: chain_utils.Chain
     web3_provider_url: str
 
     instrumentation_enabled: bool
     datadog_api_key: str
 
     # adapter: allowlist
     allow_list_endpoint: str = "https://dev.allowlist.huma.finance/"
```

### Comparing `huma_signals-0.4.0/pyproject.toml` & `huma_signals-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "huma-signals"
-version = "0.4.0"
+version = "0.4.1"
 description = "Enables access to high-quality signals about a borrower's income, assets, and liabilities."
 authors = ["Jiatu Liu <jiatu@huma.finance>", "Ji Peng <ji@huma.finance>"]
 license = "AGPL v3"
 readme = "README.md"
 packages = [{include = "huma_signals"}]
 homepage = "https://github.com/00labs/huma-signals/"
 documentation = "https://docs.huma.finance/developer-guidelines/decentralized_signal_portfolio"
@@ -15,14 +15,15 @@
 structlog = "^22.3.0"
 pandas = "^1.5.2"
 web3 = "^6.1.0"
 httpx = "^0.24.0"
 aiofiles = "^22.1.0"
 orjson = "^3.8.5"
 urllib3 = "^1.26"
+huma-utils = "^0.2.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest-describe = "^2.0.1"
 pytest = "^7.2.0"
 isort = "^5.11.3"
 flake8 = "^6.0.0"
 black = "^22.12.0"
```

### Comparing `huma_signals-0.4.0/PKG-INFO` & `huma_signals-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: huma-signals
-Version: 0.4.0
+Version: 0.4.1
 Summary: Enables access to high-quality signals about a borrower's income, assets, and liabilities.
 Home-page: https://github.com/00labs/huma-signals/
 License: AGPL v3
 Author: Jiatu Liu
 Author-email: jiatu@huma.finance
 Requires-Python: >=3.10,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: aiofiles (>=22.1.0,<23.0.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: huma-utils (>=0.2.1,<0.3.0)
 Requires-Dist: orjson (>=3.8.5,<4.0.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
 Requires-Dist: structlog (>=22.3.0,<23.0.0)
 Requires-Dist: urllib3 (>=1.26,<2.0)
 Requires-Dist: web3 (>=6.1.0,<7.0.0)
 Project-URL: Documentation, https://docs.huma.finance/developer-guidelines/decentralized_signal_portfolio
 Project-URL: Repository, https://github.com/00labs/huma-signals.git
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: huma-signals Version: 0.4.0 Summary: Enables access
+Metadata-Version: 2.1 Name: huma-signals Version: 0.4.1 Summary: Enables access
 to high-quality signals about a borrower's income, assets, and liabilities.
 Home-page: https://github.com/00labs/huma-signals/ License: AGPL v3 Author:
 Jiatu Liu Author-email: jiatu@huma.finance Requires-Python: >=3.10,<3.11
 Classifier: License :: Other/Proprietary License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: aiofiles (>=22.1.0,<23.0.0) Requires-Dist: httpx
-(>=0.24.0,<0.25.0) Requires-Dist: orjson (>=3.8.5,<4.0.0) Requires-Dist: pandas
-(>=1.5.2,<2.0.0) Requires-Dist: structlog (>=22.3.0,<23.0.0) Requires-Dist:
-urllib3 (>=1.26,<2.0) Requires-Dist: web3 (>=6.1.0,<7.0.0) Project-URL:
-Documentation, https://docs.huma.finance/developer-guidelines/
-decentralized_signal_portfolio Project-URL: Repository, https://github.com/
-00labs/huma-signals.git Description-Content-Type: text/markdown
+(>=0.24.0,<0.25.0) Requires-Dist: huma-utils (>=0.2.1,<0.3.0) Requires-Dist:
+orjson (>=3.8.5,<4.0.0) Requires-Dist: pandas (>=1.5.2,<2.0.0) Requires-Dist:
+structlog (>=22.3.0,<23.0.0) Requires-Dist: urllib3 (>=1.26,<2.0) Requires-
+Dist: web3 (>=6.1.0,<7.0.0) Project-URL: Documentation, https://
+docs.huma.finance/developer-guidelines/decentralized_signal_portfolio Project-
+URL: Repository, https://github.com/00labs/huma-signals.git Description-
+Content-Type: text/markdown
                                 [Huma_Finance]
                  ****** Decentralized Signal Portfolio ******
     [Action_Status] [Version] [Documentation]  [License:_AGPLv3] [Twitter:
 humafinance] The Decentralized Signal Portfolio (DSP) is an open source package
 that enables access to high-quality signals about a borrower's income, assets,
   and liabilities. These signals are collected through Signal Adapters, which
 gather data from a variety of on-chain and off-chain sources. Any developer can
```

