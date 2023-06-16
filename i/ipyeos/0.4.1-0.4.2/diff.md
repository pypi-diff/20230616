# Comparing `tmp/ipyeos-0.4.1.tar.gz` & `tmp/ipyeos-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyeos-0.4.1.tar", last modified: Sun May 28 02:30:42 2023, max compression
+gzip compressed data, was "ipyeos-0.4.2.tar", last modified: Fri Jun 16 04:28:01 2023, max compression
```

## Comparing `ipyeos-0.4.1.tar` & `ipyeos-0.4.2.tar`

### file list

```diff
@@ -1,38 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-28 02:30:42.631235 ipyeos-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-05-28 02:30:35.000000 ipyeos-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-28 02:30:35.000000 ipyeos-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3485 2023-05-28 02:30:42.631235 ipyeos-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3272 2023-05-28 02:30:35.000000 ipyeos-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-28 02:30:42.627235 ipyeos-0.4.1/ipyeos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3485 2023-05-28 02:30:42.000000 ipyeos-0.4.1/ipyeos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      684 2023-05-28 02:30:42.000000 ipyeos-0.4.1/ipyeos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-28 02:30:42.000000 ipyeos-0.4.1/ipyeos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      115 2023-05-28 02:30:42.000000 ipyeos-0.4.1/ipyeos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-28 02:30:42.000000 ipyeos-0.4.1/ipyeos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-28 02:30:42.000000 ipyeos-0.4.1/ipyeos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-28 02:30:42.627235 ipyeos-0.4.1/pysrc/
--rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2140 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17367 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/chain.py
--rw-r--r--   0 runner    (1001) docker     (122)    16936 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/chainapi.py
--rw-r--r--   0 runner    (1001) docker     (122)    31105 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/chaintester.py
--rw-r--r--   0 runner    (1001) docker     (122)    10424 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3433 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/eos.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-28 02:30:42.631235 ipyeos-0.4.1/pysrc/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)   877453 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/interfaces/Apply.py
--rw-r--r--   0 runner    (1001) docker     (122)    15889 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/interfaces/ApplyRequest.py
--rw-r--r--   0 runner    (1001) docker     (122)   156885 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/interfaces/IPCChainTester.py
--rw-r--r--   0 runner    (1001) docker     (122)     8156 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/interfaces/PushActions.py
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      366 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/interfaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    31953 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/interfaces/ttypes.py
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/log.py
--rw-r--r--   0 runner    (1001) docker     (122)      238 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     5426 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/rpc_server.py
--rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/run.py
--rw-r--r--   0 runner    (1001) docker     (122)    52216 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/server.py
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-28 02:30:35.000000 ipyeos-0.4.1/pysrc/types.py
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-28 02:30:35.000000 ipyeos-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      272 2023-05-28 02:30:42.631235 ipyeos-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1270 2023-05-28 02:30:35.000000 ipyeos-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 04:28:01.773359 ipyeos-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-06-16 04:27:47.000000 ipyeos-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-16 04:27:47.000000 ipyeos-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4124 2023-06-16 04:28:01.773359 ipyeos-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3911 2023-06-16 04:27:47.000000 ipyeos-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 04:28:01.765359 ipyeos-0.4.2/ipyeos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4124 2023-06-16 04:28:01.000000 ipyeos-0.4.2/ipyeos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      764 2023-06-16 04:28:01.000000 ipyeos-0.4.2/ipyeos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 04:28:01.000000 ipyeos-0.4.2/ipyeos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      218 2023-06-16 04:28:01.000000 ipyeos-0.4.2/ipyeos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-06-16 04:28:01.000000 ipyeos-0.4.2/ipyeos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-16 04:28:01.000000 ipyeos-0.4.2/ipyeos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-16 04:27:47.000000 ipyeos-0.4.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 04:28:01.769359 ipyeos-0.4.2/pysrc/
+-rw-r--r--   0 runner    (1001) docker     (122)     2020 2023-06-16 04:27:47.000000 ipyeos-0.4.2/pysrc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-06-16 04:27:47.000000 ipyeos-0.4.2/pysrc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2082 2023-06-16 04:27:47.000000 ipyeos-0.4.2/pysrc/args.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17428 2023-06-16 04:27:47.000000 ipyeos-0.4.2/pysrc/chain.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16925 2023-06-16 04:27:47.000000 ipyeos-0.4.2/pysrc/chainapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31309 2023-06-16 04:27:47.000000 ipyeos-0.4.2/pysrc/chaintester.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10424 2023-06-16 04:27:47.000000 ipyeos-0.4.2/pysrc/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4231 2023-06-16 04:27:47.000000 ipyeos-0.4.2/pysrc/database.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4404 2023-06-16 04:27:47.000000 ipyeos-0.4.2/pysrc/eos.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 04:28:01.773359 ipyeos-0.4.2/pysrc/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)   877453 2023-06-16 04:27:47.000000 ipyeos-0.4.2/pysrc/interfaces/Apply.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15889 2023-06-16 04:27:47.000000 ipyeos-0.4.2/pysrc/interfaces/ApplyRequest.py
+-rw-r--r--   0 runner    (1001) docker     (122)   156885 2023-06-16 04:27:47.000000 ipyeos-0.4.2/pysrc/interfaces/IPCChainTester.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8156 2023-06-16 04:27:47.000000 ipyeos-0.4.2/pysrc/interfaces/PushActions.py
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-16 04:27:47.000000 ipyeos-0.4.2/pysrc/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2023-06-16 04:27:47.000000 ipyeos-0.4.2/pysrc/interfaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31953 2023-06-16 04:27:47.000000 ipyeos-0.4.2/pysrc/interfaces/ttypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2194 2023-06-16 04:27:47.000000 ipyeos-0.4.2/pysrc/ipykernel_embed.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15803 2023-06-16 04:27:47.000000 ipyeos-0.4.2/pysrc/ipython_embed.py
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-16 04:27:47.000000 ipyeos-0.4.2/pysrc/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4262 2023-06-16 04:27:47.000000 ipyeos-0.4.2/pysrc/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-06-16 04:27:47.000000 ipyeos-0.4.2/pysrc/rpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5198 2023-06-16 04:27:47.000000 ipyeos-0.4.2/pysrc/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)    52821 2023-06-16 04:27:47.000000 ipyeos-0.4.2/pysrc/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-16 04:27:47.000000 ipyeos-0.4.2/pysrc/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-16 04:27:47.000000 ipyeos-0.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-16 04:28:01.773359 ipyeos-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1285 2023-06-16 04:27:47.000000 ipyeos-0.4.2/setup.py
```

### Comparing `ipyeos-0.4.1/LICENSE` & `ipyeos-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.1/PKG-INFO` & `ipyeos-0.4.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: ipyeos
-Version: 0.4.1
-Summary: IPYEOS project
-Home-page: UNKNOWN
-Author: The IPYEOS Team
-License: MIT
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Interactive Python for Eos
 
 [![PyPi](https://img.shields.io/pypi/v/ipyeos.svg)](https://pypi.org/project/ipyeos)
 [![PyPi](https://img.shields.io/pypi/dm/ipyeos.svg)](https://pypi.org/project/ipyeos)
 
 
 ## What Is IPyEos
@@ -20,30 +9,61 @@
 - IPyEos is a Smart Contracts test framework for Eos
 - IPyEos is a Python binding for Eos
 
 ## Installation
 
 ```
 python3 -m pip install ipyeos
-cdt-init
 ```
 
 on the macOS platform, you may need to install `gmp` and `zstd` if you don't install them.
 
 ```bash
 brew reinstall gmp
 brew reinstall zstd
 ```
 
-Also, you can install the `ipyeos` docker image with the following command if your machine does not support install `ipyeos` directly.
+If your platform is Windows or MacOSX M1/M2, you also need to download an image that includes the ipyeos tool:
 
 ```bash
 docker pull ghcr.io/uuosio/ipyeos:latest
 ```
 
+If you have not installed the ipyeos image in Docker, then the ipyeos image will be automatically downloaded the first time you run `ipyeos` or `eosdebugger`.
+
+On macOS, the recommended software for installing and running Docker is [OrbStack](https://orbstack.dev/download). For other platforms, you can use [Docker Desktop](https://www.docker.com/products/docker-desktop).
+
+# Usage
+
+```python
+#test.py
+import os
+from ipyeos.chaintester import ChainTester
+
+chaintester.chain_config['contracts_console'] = True
+
+def test_example():
+    t = ChainTester(True)
+    with open('./hello/build/hello/hello.wasm', 'rb') as f:
+        code = f.read()
+    with open('./hello/build/hello/hello.abi', 'rb') as f:
+        abi = f.read()
+    t.deploy_contract('hello', code, abi)
+    t.produce_block()
+
+    t.push_action('hello', 'hi', {'nm': 'alice'}, {'hello': 'active'})
+    t.produce_block()
+```
+
+Test:
+
+```
+ipyeos -m pytest -x -s tests/test.py
+```
+
 ## Building
 
 To build this project, please follow the steps below:
 
 1. Clone the source code from the repository:
 
 ```bash
@@ -58,35 +78,29 @@
 cd ipyeos
 ./build.sh
 ```
 
 4. Install the Python package
 
 ```bash
-python3 -m pip install dist/pyeos-0.4.1**.whl
+python3 -m pip install dist/pyeos-0.4.2**.whl
 ```
 
 ## Run a Node
 
 ```bash
 eosnode
 ```
 
 ## Run a Debugging Server
 
 ```bash
 eosdebugger
 ```
 
-or use the following command if you have installed `ipyeos` docker image:
-
-```bash
-docker run -it --rm -p 9090:9090 -p 9092:9092 -t ghcr.io/uuosio/ipyeos
-```
-
 ## Testing
 
 test example code
 
 ```python
 #test.py
 import os
@@ -109,29 +123,27 @@
 
 ```
 ipyeos -m pytest -x -s tests/test.py
 ```
 
 ## Run a Testnet
 
-```
-ipyeos -m ipyeos eosnode --data-dir dd --config-dir cd -p eosio --plugin eosio::producer_plugin --plugin eosio::chain_api_plugin --plugin eosio::producer_api_plugin --plugin eosio::history_api_plugin -e --resource-monitor-space-threshold 99 --http-server-address 127.0.0.1:8889 --contracts-console --access-control-allow-origin="*" --backing-store rocksdb --wasm-runtime eos-vm-jit
+```bash
+ipyeos -m ipyeos eosnode --data-dir dd --config-dir cd -p eosio --plugin eosio::producer_plugin --plugin eosio::chain_api_plugin --plugin eosio::producer_api_plugin -e --resource-monitor-space-threshold 99 --http-server-address 127.0.0.1:8889 --contracts-console --access-control-allow-origin="*"  --wasm-runtime eos-vm-jit
 ```
 
 Also, you can run a test node with `eosnode` command directly.
 
-```
-eosnode --data-dir dd --config-dir cd -p eosio --plugin eosio::producer_plugin --plugin eosio::chain_api_plugin --plugin eosio::producer_api_plugin --plugin eosio::history_api_plugin -e --resource-monitor-space-threshold 99 --http-server-address 127.0.0.1:8889 --contracts-console --access-control-allow-origin="*" --backing-store rocksdb --wasm-runtime eos-vm-jit
+```bash
+eosnode --data-dir dd --config-dir cd -p eosio --plugin eosio::producer_plugin --plugin eosio::chain_api_plugin --plugin eosio::producer_api_plugin -e --resource-monitor-space-threshold 99 --http-server-address 127.0.0.1:8889 --contracts-console --access-control-allow-origin="*"  --wasm-runtime eos-vm-jit
 ```
 
 # Note
 
 If you encounter the error message during running the above commands like `Failed to load libpython3.7m.so!`, try running the following command in your terminal:
 
 ```bash
 export PYTHON_SHARED_LIB_PATH=path/to/libpython[.so|.dylib]
 ```
 
 # License
 [MIT](./LICENSE)
-
-
```

### Comparing `ipyeos-0.4.1/ipyeos.egg-info/PKG-INFO` & `ipyeos-0.4.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyeos
-Version: 0.4.1
+Version: 0.4.2
 Summary: IPYEOS project
 Home-page: UNKNOWN
 Author: The IPYEOS Team
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -20,30 +20,61 @@
 - IPyEos is a Smart Contracts test framework for Eos
 - IPyEos is a Python binding for Eos
 
 ## Installation
 
 ```
 python3 -m pip install ipyeos
-cdt-init
 ```
 
 on the macOS platform, you may need to install `gmp` and `zstd` if you don't install them.
 
 ```bash
 brew reinstall gmp
 brew reinstall zstd
 ```
 
-Also, you can install the `ipyeos` docker image with the following command if your machine does not support install `ipyeos` directly.
+If your platform is Windows or MacOSX M1/M2, you also need to download an image that includes the ipyeos tool:
 
 ```bash
 docker pull ghcr.io/uuosio/ipyeos:latest
 ```
 
+If you have not installed the ipyeos image in Docker, then the ipyeos image will be automatically downloaded the first time you run `ipyeos` or `eosdebugger`.
+
+On macOS, the recommended software for installing and running Docker is [OrbStack](https://orbstack.dev/download). For other platforms, you can use [Docker Desktop](https://www.docker.com/products/docker-desktop).
+
+# Usage
+
+```python
+#test.py
+import os
+from ipyeos.chaintester import ChainTester
+
+chaintester.chain_config['contracts_console'] = True
+
+def test_example():
+    t = ChainTester(True)
+    with open('./hello/build/hello/hello.wasm', 'rb') as f:
+        code = f.read()
+    with open('./hello/build/hello/hello.abi', 'rb') as f:
+        abi = f.read()
+    t.deploy_contract('hello', code, abi)
+    t.produce_block()
+
+    t.push_action('hello', 'hi', {'nm': 'alice'}, {'hello': 'active'})
+    t.produce_block()
+```
+
+Test:
+
+```
+ipyeos -m pytest -x -s tests/test.py
+```
+
 ## Building
 
 To build this project, please follow the steps below:
 
 1. Clone the source code from the repository:
 
 ```bash
@@ -58,35 +89,29 @@
 cd ipyeos
 ./build.sh
 ```
 
 4. Install the Python package
 
 ```bash
-python3 -m pip install dist/pyeos-0.4.1**.whl
+python3 -m pip install dist/pyeos-0.4.2**.whl
 ```
 
 ## Run a Node
 
 ```bash
 eosnode
 ```
 
 ## Run a Debugging Server
 
 ```bash
 eosdebugger
 ```
 
-or use the following command if you have installed `ipyeos` docker image:
-
-```bash
-docker run -it --rm -p 9090:9090 -p 9092:9092 -t ghcr.io/uuosio/ipyeos
-```
-
 ## Testing
 
 test example code
 
 ```python
 #test.py
 import os
@@ -109,22 +134,22 @@
 
 ```
 ipyeos -m pytest -x -s tests/test.py
 ```
 
 ## Run a Testnet
 
-```
-ipyeos -m ipyeos eosnode --data-dir dd --config-dir cd -p eosio --plugin eosio::producer_plugin --plugin eosio::chain_api_plugin --plugin eosio::producer_api_plugin --plugin eosio::history_api_plugin -e --resource-monitor-space-threshold 99 --http-server-address 127.0.0.1:8889 --contracts-console --access-control-allow-origin="*" --backing-store rocksdb --wasm-runtime eos-vm-jit
+```bash
+ipyeos -m ipyeos eosnode --data-dir dd --config-dir cd -p eosio --plugin eosio::producer_plugin --plugin eosio::chain_api_plugin --plugin eosio::producer_api_plugin -e --resource-monitor-space-threshold 99 --http-server-address 127.0.0.1:8889 --contracts-console --access-control-allow-origin="*"  --wasm-runtime eos-vm-jit
 ```
 
 Also, you can run a test node with `eosnode` command directly.
 
-```
-eosnode --data-dir dd --config-dir cd -p eosio --plugin eosio::producer_plugin --plugin eosio::chain_api_plugin --plugin eosio::producer_api_plugin --plugin eosio::history_api_plugin -e --resource-monitor-space-threshold 99 --http-server-address 127.0.0.1:8889 --contracts-console --access-control-allow-origin="*" --backing-store rocksdb --wasm-runtime eos-vm-jit
+```bash
+eosnode --data-dir dd --config-dir cd -p eosio --plugin eosio::producer_plugin --plugin eosio::chain_api_plugin --plugin eosio::producer_api_plugin -e --resource-monitor-space-threshold 99 --http-server-address 127.0.0.1:8889 --contracts-console --access-control-allow-origin="*"  --wasm-runtime eos-vm-jit
 ```
 
 # Note
 
 If you encounter the error message during running the above commands like `Failed to load libpython3.7m.so!`, try running the following command in your terminal:
 
 ```bash
```

### Comparing `ipyeos-0.4.1/ipyeos.egg-info/SOURCES.txt` & `ipyeos-0.4.2/ipyeos.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,19 +9,23 @@
 ipyeos.egg-info/SOURCES.txt
 ipyeos.egg-info/dependency_links.txt
 ipyeos.egg-info/entry_points.txt
 ipyeos.egg-info/requires.txt
 ipyeos.egg-info/top_level.txt
 pysrc/__init__.py
 pysrc/__main__.py
+pysrc/args.py
 pysrc/chain.py
 pysrc/chainapi.py
 pysrc/chaintester.py
 pysrc/config.py
+pysrc/database.py
 pysrc/eos.py
+pysrc/ipykernel_embed.py
+pysrc/ipython_embed.py
 pysrc/log.py
 pysrc/main.py
 pysrc/rpc_server.py
 pysrc/run.py
 pysrc/server.py
 pysrc/types.py
 pysrc/interfaces/Apply.py
```

### Comparing `ipyeos-0.4.1/pysrc/chain.py` & `ipyeos-0.4.2/pysrc/chain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 from datetime import datetime
-from typing import Dict, List, Union, Optional
+from typing import Dict, List, Optional, Union
 
-from . import _chain, _eos
-from . import log
+from . import _chain, _eos, log
 from .types import Name, PublicKey
 
 logger = log.get_logger(__name__)
 
 def isoformat(dt):
     return dt.isoformat(timespec='milliseconds')
 
@@ -75,14 +74,17 @@
     def id(self) -> str:
         """
         Get chain id
         :returns str: Return the chain id
         """
         return _chain.id(self.ptr)
 
+    def get_database(self):
+        return _chain.get_database(self.ptr)
+
     def start_block(self, _time: Union[datetime, str], confirm_block_count: int=0, features: Optional[list]=None) -> None:
         """
         Start a new block
         :param str _time
         :param int confirm_block_count
         :param list features
         """
```

### Comparing `ipyeos-0.4.1/pysrc/chainapi.py` & `ipyeos-0.4.2/pysrc/chainapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from typing import List, Dict, Union, Optional
 import json
-from . import _chainapi
-from . import _chain, _eos
+from typing import Dict, List, Optional, Union
+
+from . import _chain, _chainapi, _eos
+
 
 class ChainApi(object):
 
     def __init__(self, chain):
         self.ptr = chain.ptr
         self.chain = chain
```

### Comparing `ipyeos-0.4.1/pysrc/chaintester.py` & `ipyeos-0.4.2/pysrc/chaintester.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import os
-import json
-import pytest
 import atexit
+import json
 import logging
+import os
 import shutil
-import tempfile
 import subprocess
+import tempfile
+from datetime import datetime, timedelta, timezone
+from typing import Dict, List, Optional, Union
 
-from ipyeos import chain, chainapi, config
-from datetime import datetime, timedelta
-from datetime import timezone
+import pytest
 
-from . import log, eos
-from typing import List, Dict, Union, Optional
+from ipyeos import chain, chainapi, database, config
+
+from . import eos, log
 from .types import Name
 
 logger = log.get_logger(__name__)
 
 test_dir = os.path.dirname(__file__)
 
 # default_time = datetime.fromtimestamp(946684800000/1e3, tz=timezone.utc)
@@ -150,14 +150,16 @@
 
         self.chain_config = json.dumps(chain_config)
         self.genesis_test = json.dumps(genesis_test)
         self.chain = chain.Chain(self.chain_config, self.genesis_test, os.path.join(self.config_dir, "protocol_features"), "")
         self.chain.startup(True)
         self.api = chainapi.ChainApi(self.chain)
 
+        self.db = database.Database(self.chain.get_database())
+
         # logger.info(self.api.get_info())
         # logger.info(self.api.get_account('eosio'))
 
         self.feature_digests = []
 
         self.feature_digests = ['0ec7e080177b2c02b278d5088611686b49d739925a92d9bfcacd7fc6b74053bd']
         self.start_block()
@@ -733,27 +735,30 @@
             logger.exception(e)
             return 0.0
 
     def get_table_rows(self, _json, code, scope, table,
                                     lower_bound, upper_bound,
                                     limit,
                                     key_type='',
-                                    index_position='', 
+                                    index_position='',
+                                    encode_type='',
                                     reverse = False,
                                     show_payer = False):
         """ Fetch smart contract data from an account. 
-        key_type: "i64"|"i128"|"i256"|"float64"|"float128"|"sha256"|"ripemd160"
+        key_type: "name"|"i64"|"i128"|"i256"|"float64"|"float128"|"sha256"|"ripemd160"
         index_position: "2"|"3"|"4"|"5"|"6"|"7"|"8"|"9"|"10"
+        encode_type: "dec" or "hex", default to "dec"
         """
         return self.api.get_table_rows(
             _json, code, scope, table,
             lower_bound, upper_bound,
             limit,
             key_type=key_type,
             index_position=index_position, 
+            encode_type=encode_type,
             reverse=reverse,
             show_payer=show_payer
         )
 
     def s2n(self, s: str) -> int:
         return eos.s2n(s)
```

### Comparing `ipyeos-0.4.1/pysrc/config.py` & `ipyeos-0.4.2/pysrc/config.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+import argparse
 import os
 import sys
-import argparse
 
 default_abi_serializer_max_time_ms = 15*1000
 default_state_guard_size      =    128*1024*1024#
 default_reversible_cache_size = 340*1024*1024 # 1MB * 340 blocks based on 21 producer BFT delay
 default_reversible_guard_size = 2*1024*1024 # 1MB * 340 blocks based on 21 producer BFT delay
 
 block_interval_ms = 1000
```

### Comparing `ipyeos-0.4.1/pysrc/eos.py` & `ipyeos-0.4.2/pysrc/eos.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-import sys
 import json
+import sys
+from typing import Union
 
 from . import _eos
-from typing import Union
 from .types import Name
 
+
 class NativeType:
     handshake_message = 0
     chain_size_message = 1
     go_away_message = 2
     time_message = 3
     notice_message = 4
     request_message = 5
@@ -16,17 +17,42 @@
     signed_block_v0 = 7         # which = 7
     packed_transaction_v0 = 8   # which = 8
     signed_block = 9            # which = 9
     trx_message_v1 = 10         # which = 10
     genesis_state = 11
     abi_def = 12
 
+LOG_LEVEL_ALL = 0
+LOG_LEVEL_DEBUG = 1
+LOG_LEVEL_INFO = 2
+LOG_LEVEL_WARN = 3
+LOG_LEVEL_ERROR = 4
+LOG_LEVEL_OFF = 5
+
 def set_log_level(logger_name: str, level: int) -> None:
     _eos.set_log_level(logger_name, level)
 
+def set_all_level(logger_name: str) -> None:
+    _eos.set_log_level(logger_name, LOG_LEVEL_ALL)
+
+def set_debug_level(logger_name: str) -> None:
+    _eos.set_log_level(logger_name, LOG_LEVEL_DEBUG)
+
+def set_info_level(logger_name: str) -> None:
+    _eos.set_log_level(logger_name, LOG_LEVEL_INFO)
+
+def set_warn_level(logger_name: str) -> None:
+    _eos.set_log_level(logger_name, LOG_LEVEL_WARN)
+
+def set_error_level(logger_name: str) -> None:
+    _eos.set_log_level(logger_name, LOG_LEVEL_ERROR)
+
+def set_off_level(logger_name: str) -> None:
+    _eos.set_log_level(logger_name, LOG_LEVEL_OFF)
+
 def pack_native_object(_type: int, obj: Union[dict, str]) -> bytes:
     if isinstance(obj, dict):
         obj = json.dumps(obj)
     else:
         assert isinstance(obj, (str, bytes))
     return _eos.pack_native_object(_type, obj)
 
@@ -51,15 +77,22 @@
         return b''
     return pack_native_object(NativeType.abi_def, abi)
 
 def s2n(s: str) -> int:
     '''
     Convert a EOSIO name to uint64_t
     '''
-    return _eos.s2n(s)
+    ret = _eos.s2n(s)
+    if not ret == 0:
+        return ret
+    err = _eos.get_last_error()
+    if err:
+        _eos.set_last_error("")
+        raise Exception(err)
+    return ret
 
 def n2s(n: int) -> str:
     '''
     Convert int to a EOSIO name
     '''
     return _eos.n2s(n)
 
@@ -67,14 +100,33 @@
     n = s2n(s)
     return int.to_bytes(n, 8, 'little')
 
 def b2s(s: bytes) -> str:
     s = int.from_bytes(s, 'little')
     return n2s(s)
 
+def sym2n(s: str) -> int:
+    """convert symbol string to int
+
+    Args:
+        s (str): symbol name
+
+    Raises:
+        Exception: invalid symbol
+
+    Returns:
+        _type_: int
+    """
+    for c in s:
+        if not c.isupper():
+            raise Exception('invalid symbol')
+    ss = [c for c in s]
+    ss.reverse()
+    return int.from_bytes(''.join(ss).encode(), 'big')
+
 def get_native_contract(contract) -> str:
     contract = _eos.s2n(contract)
     return _eos.get_native_contract(contract)
 
 def enable_native_contracts(debug) -> None:
     _eos.enable_native_contracts(debug)
 
@@ -103,35 +155,23 @@
     ret = _eos.get_public_key(priv_key)
     return check_ret(ret)
 
 def sign_digest(digest: str, priv_key: str):
     ret = _eos.sign_digest(digest, priv_key)
     return check_ret(ret)
 
-def init(argv=None) -> bool:
+def init(argv=None) -> int:
     if argv:
         return _eos.init(argv)
     return _eos.init(sys.argv[1:])
 
-def start(argv) -> None:
-    if argv:
-        return _eos.start(argv)
-    _eos.start(sys.argv[1:])
-
-def sym2n(s: str) -> int:
-    """convert symbol string to int
+def run() -> int:
+    return _eos.run()
 
-    Args:
-        s (str): symbol name
+def run_once() -> int:
+    return _eos.run_once()
 
-    Raises:
-        Exception: invalid symbol
+def post(fn, *args, **kwargs):
+    return _eos.post(fn, *args, **kwargs)
 
-    Returns:
-        _type_: int
-    """
-    for c in s:
-        if not c.isupper():
-            raise Exception('invalid symbol')
-    ss = [c for c in s]
-    ss.reverse()
-    return int.from_bytes(''.join(ss).encode(), 'big')
+def quit() -> None:
+    _eos.quit()
```

### Comparing `ipyeos-0.4.1/pysrc/interfaces/Apply.py` & `ipyeos-0.4.2/pysrc/interfaces/Apply.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.1/pysrc/interfaces/ApplyRequest.py` & `ipyeos-0.4.2/pysrc/interfaces/ApplyRequest.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.1/pysrc/interfaces/IPCChainTester.py` & `ipyeos-0.4.2/pysrc/interfaces/IPCChainTester.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.1/pysrc/interfaces/PushActions.py` & `ipyeos-0.4.2/pysrc/interfaces/PushActions.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.1/pysrc/interfaces/ttypes.py` & `ipyeos-0.4.2/pysrc/interfaces/ttypes.py`

 * *Files identical despite different names*

### Comparing `ipyeos-0.4.1/pysrc/rpc_server.py` & `ipyeos-0.4.2/pysrc/rpc_server.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+from aiohttp import web
+import asyncio
 import json
-import asyncio as aio
 from concurrent.futures import ThreadPoolExecutor
-from flask import Flask, request, jsonify
-from waitress import serve
+from typing import Dict, List, NewType, Optional
+
+from flask import Flask, jsonify, request
 
-from .interfaces.ttypes import Action, ActionArguments
 from . import eos
+from .interfaces.ttypes import Action, ActionArguments
 
-from typing import NewType, List, Dict, Optional
 i32 = NewType('i32', int)
 i64 = NewType('i64', int)
 u64 = NewType('u64', int)
 
 class BaseChainTester:
     def produce_block(self, id):
         pass
@@ -36,15 +37,15 @@
 
     def pack_action_args(self, id, contract, action, action_args):
         pass
 
     def unpack_action_args(self, id, contract, action, raw_args):
         pass
 
-    def new_chain(self):
+    def new_chain(self, initialize: bool=True):
         pass
 
     def free_chain(self, id):
         pass
 
     def get_info(self, id: i32):
         pass
@@ -58,16 +59,16 @@
     def get_required_keys(self, id: i32, transaction: str, available_keys: List[str]):
         pass
 
 class ChainTesterProxy(object):
     def __init__(self, handler: BaseChainTester):
         self.handler = handler
 
-    def new_chain(self):
-        id = self.handler.new_chain()
+    def new_chain(self, initialize: bool=True):
+        id = self.handler.new_chain(initialize)
         return {"id": id}
 
     def free_chain(self, id):
         self.handler.free_chain(id)
         return {}
 
     def create_key(self, key_type):
@@ -138,24 +139,43 @@
         ret = self.handler.import_key(id, pub_key, priv_key)
         return {"data": "ok"}
 
     def get_required_keys(self, id: i32, transaction: str, available_keys: List[str]):
         ret = self.handler.get_required_keys(id, transaction, available_keys)
         return {"data": ret}
 
+    def quit(self):
+        ret = self.handler.quit()
+        return {"data": ret}
+
 proxy = None
-app = Flask(__name__)
 
-@app.route('/api/<method>', methods=['GET', 'POST'])
-def call_method(method):
-    global proxy
-    kwargs = request.json
-    # print(kwargs)
-    ret = getattr(proxy, method)(**kwargs)
-    if isinstance(ret, dict):
-        ret = json.dumps(ret)
-    return ret
+async def call_method(request: web.Request):
+    try:
+        kwargs = await request.json()
+        method = request.match_info.get('method', None)
+
+        ret = getattr(proxy, method)(**kwargs)
+        if isinstance(ret, dict):
+            ret = json.dumps(ret)
+        elif isinstance(ret, bytes):
+            ret = ret.decode()
+        return web.Response(text=ret)
+    except json.JSONDecodeError:
+        return web.HTTPBadRequest(text="Invalid JSON")
+    except Exception as e:
+        print(e)
+        return web.HTTPInternalServerError()
 
-def start(rpc_server_addr, rpc_server_port, handler: BaseChainTester):
+async def start(rpc_server_addr, rpc_server_port, handler: BaseChainTester):
     global proxy
     proxy = ChainTesterProxy(handler)
-    serve(app, listen=f'{rpc_server_addr}:{rpc_server_port}')
+    print('+++++++start rpc server', rpc_server_addr, rpc_server_port)
+    app = web.Application()
+    app.router.add_route('POST', '/api/{method}', call_method)
+    runner = web.AppRunner(app)
+    await runner.setup()
+    site = web.TCPSite(runner, rpc_server_addr, rpc_server_port)
+    await site.start()
+    print('rpc server started')
+    while True:
+        await asyncio.sleep(1000.0)
```

### Comparing `ipyeos-0.4.1/pysrc/server.py` & `ipyeos-0.4.2/pysrc/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,52 +1,51 @@
-import os
+import asyncio as aio
+from concurrent.futures import ThreadPoolExecutor
 import glob
-import sys
 import json
-import time
+import logging
+import os
+import queue
 import string
+import sys
 import threading
+import time
 import traceback
-import logging
 from datetime import datetime, timedelta
+from typing import Dict, List, NewType, Optional
 
-from typing import NewType, Dict, Optional, List
 i32 = NewType('i32', int)
 i64 = NewType('i64', int)
 u64 = NewType('u64', int)
 
 Iterator = NewType('Iterator', i32)
 
-from .interfaces import IPCChainTester, ApplyRequest, Apply
-
-from .interfaces.ttypes import Uint64, NextPreviousReturn,FindPrimaryReturn, FindSecondaryReturn, LowerBoundUpperBoundReturn
-from .interfaces.ttypes import GetResourceLimitsReturn
-from .interfaces.ttypes import Action, ActionArguments
-
-from thrift.transport import TSocket
-from thrift.transport import TTransport
 from thrift.protocol import TBinaryProtocol
-from thrift.server import TServer
 from thrift.protocol.THeaderProtocol import THeaderProtocolFactory
-from thrift.Thrift import TType, TMessageType, TApplicationException
+from thrift.server import TServer
+from thrift.Thrift import TApplicationException, TMessageType, TType
+from thrift.transport import TSocket, TTransport
 
-from . import chaintester 
-from . import eos, _vm_api, log
-from .chaintester import ChainTester
+from . import _chainapi, _eos, _vm_api, chaintester, eos, log, rpc_server
 from .chainapi import ChainApi
-from . import _chainapi
-from . import _eos
-
-from . import rpc_server
+from .chaintester import ChainTester
+from .interfaces import Apply, ApplyRequest, IPCChainTester
+from .interfaces.ttypes import (Action, ActionArguments, FindPrimaryReturn,
+                                FindSecondaryReturn, GetResourceLimitsReturn,
+                                LowerBoundUpperBoundReturn, NextPreviousReturn,
+                                Uint64)
 
 chaintester.chain_config['contracts_console'] = True
 
 logger = log.get_logger(__name__)
 logger.setLevel(logging.DEBUG)
 
+
+thread_queue = queue.Queue()
+
 def to_uint64(value):
     return Uint64(int.to_bytes(value, 8, 'little'))
 
 def from_uint64(value):
     assert len(value.rawValue) == 8, 'bad Uint64'
     return int.from_bytes(value.rawValue, 'little')
 
@@ -1076,14 +1075,18 @@
         )
         params = json.dumps(params)
         success, ret = _chainapi.get_required_keys(chain.ptr, params)
         if not success:
             return chain.get_last_error()
         return ret
 
+    def quit(self):
+        thread_queue.put('exit')
+        return True
+
 class VMAPIServer(TServer.TServer):
     """Simple single-threaded server that just pumps around one transport."""
 
     def __init__(self, *args):
         TServer.TServer.__init__(self, *args)
         self.serverTransport.listen()
 
@@ -1266,28 +1269,44 @@
 
 # result.addr, result.server_port, result.vm_api_port, result.apply_request_addr, result.apply_request_port
 def start_debug_server(addr='127.0.0.1', server_port=9090, vm_api_port=9092, apply_request_addr='127.0.0.1', apply_request_port=9091, rpc_server_addr='127.0.0.1', rpc_server_port=9093):
     eos.enable_debug(True)
     handler = ChainTesterHandler(addr, vm_api_port, apply_request_addr, apply_request_port)
     processor = IPCChainTesterProcessor(handler)
 
-    def run_server():
+    def start_server():
         print('Starting the EOS debugger server...')
         transport = TSocket.TServerSocket(host=addr, port=server_port)
         tfactory = TTransport.TBufferedTransportFactory()
         pfactory = TBinaryProtocol.TBinaryProtocolFactory()
 
         server = ChainTesterServer(processor, transport, tfactory, pfactory, handler=handler)
         server.serve()
         print('done.')
 
-    def run_rpc_server():
-        print('run rpc server')
-        rpc_server.start(rpc_server_addr, rpc_server_port, handler)
+    def start_rpc_server():
+        loop = aio.new_event_loop()
+        try:
+            loop.run_until_complete(rpc_server.start(rpc_server_addr, rpc_server_port, handler))
+        except KeyboardInterrupt:
+            loop.stop()
+            loop.close()
+
+    t = threading.Thread(target=start_rpc_server, daemon=True)
+    t.start()
 
-    t = threading.Thread(target=run_rpc_server)
+    t = threading.Thread(target=start_server, daemon=True)
     t.start()
-    run_server()
+
+    while True:
+        try:
+            command = thread_queue.get(block=True)
+            if command == 'exit':
+                time.sleep(1.0)
+                sys.exit(0)
+                break
+        except KeyboardInterrupt:
+            sys.exit(0)
 
 if __name__ == '__main__':
     start_debug_server()
```

### Comparing `ipyeos-0.4.1/setup.py` & `ipyeos-0.4.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     'tests/contracts/micropython/*',
     'tests/test_template.py',
     'tests/activate_kv.wasm',
 ])
 
 setup(
     name="ipyeos",
-    version="0.4.1",
+    version="0.4.2",
     description="IPYEOS project",
     author='The IPYEOS Team',
     license="MIT",
     packages=[
         'ipyeos',
         'ipyeos.interfaces'
     ],
@@ -41,13 +41,14 @@
         'ipyeos.interfaces': 'pysrc/interfaces'
     },
     package_data={'ipyeos': release_files},
 
     install_requires=[
         'thrift>=0.16.0',
         'pytest>=6.2.5',
-        'waitress>=2.1.2',
-        'flask>=2.2.2'
+        'aiohttp>=3.8.4',
+        'ipython',
+        'ipykernel'
     ],
     tests_require=[],
     include_package_data=True
 )
```

