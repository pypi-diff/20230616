# Comparing `tmp/nacos_sdk_rust_binding_py-0.1.2.tar.gz` & `tmp/nacos_sdk_rust_binding_py-0.3.0.tar.gz`

## Comparing `nacos_sdk_rust_binding_py-0.1.2.tar` & `nacos_sdk_rust_binding_py-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 nacos_sdk_rust_binding_py-0.1.2/Cargo.toml
--rw-r--r--   0     1001      123     2807 2023-06-11 11:10:43.000000 nacos_sdk_rust_binding_py-0.1.2/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      519 2023-06-11 11:10:43.000000 nacos_sdk_rust_binding_py-0.1.2/.gitignore
--rw-r--r--   0     1001      123    11357 2023-06-11 11:10:43.000000 nacos_sdk_rust_binding_py-0.1.2/LICENSE
--rw-r--r--   0     1001      123     6153 2023-06-11 11:10:43.000000 nacos_sdk_rust_binding_py-0.1.2/README.md
--rw-r--r--   0     1001      123       10 2023-06-11 11:12:34.000000 nacos_sdk_rust_binding_py-0.1.2/dist/nacos_sdk_rust_binding_py-0.1.2.tar.gz
--rw-r--r--   0     1001      123     1852 2023-06-11 11:10:43.000000 nacos_sdk_rust_binding_py-0.1.2/examples/config.py
--rw-r--r--   0     1001      123     1498 2023-06-11 11:10:43.000000 nacos_sdk_rust_binding_py-0.1.2/examples/naming.py
--rw-r--r--   0     1001      123      856 2023-06-11 11:10:43.000000 nacos_sdk_rust_binding_py-0.1.2/pyproject.toml
--rw-r--r--   0     1001      123     6025 2023-06-11 11:10:43.000000 nacos_sdk_rust_binding_py-0.1.2/src/config.rs
--rw-r--r--   0     1001      123     2647 2023-06-11 11:10:43.000000 nacos_sdk_rust_binding_py-0.1.2/src/lib.rs
--rw-r--r--   0     1001      123    11291 2023-06-11 11:10:43.000000 nacos_sdk_rust_binding_py-0.1.2/src/naming.rs
--rw-r--r--   0     1001      123      230 2023-06-11 11:10:43.000000 nacos_sdk_rust_binding_py-0.1.2/test.sh
--rw-r--r--   0     1001      123    38648 2023-06-11 11:12:33.000000 nacos_sdk_rust_binding_py-0.1.2/Cargo.lock
--rw-r--r--   0        0        0     7081 1970-01-01 00:00:00.000000 nacos_sdk_rust_binding_py-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 nacos_sdk_rust_binding_py-0.3.0/Cargo.toml
+-rw-r--r--   0     1001      123     2807 2023-06-16 15:27:19.000000 nacos_sdk_rust_binding_py-0.3.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      519 2023-06-16 15:27:19.000000 nacos_sdk_rust_binding_py-0.3.0/.gitignore
+-rw-r--r--   0     1001      123    11357 2023-06-16 15:27:19.000000 nacos_sdk_rust_binding_py-0.3.0/LICENSE
+-rw-r--r--   0     1001      123     6358 2023-06-16 15:27:19.000000 nacos_sdk_rust_binding_py-0.3.0/README.md
+-rw-r--r--   0     1001      123       10 2023-06-16 15:27:32.000000 nacos_sdk_rust_binding_py-0.3.0/dist/nacos_sdk_rust_binding_py-0.3.0.tar.gz
+-rw-r--r--   0     1001      123     1852 2023-06-16 15:27:19.000000 nacos_sdk_rust_binding_py-0.3.0/examples/config.py
+-rw-r--r--   0     1001      123     1498 2023-06-16 15:27:19.000000 nacos_sdk_rust_binding_py-0.3.0/examples/naming.py
+-rw-r--r--   0     1001      123      856 2023-06-16 15:27:19.000000 nacos_sdk_rust_binding_py-0.3.0/pyproject.toml
+-rw-r--r--   0     1001      123     6025 2023-06-16 15:27:19.000000 nacos_sdk_rust_binding_py-0.3.0/src/config.rs
+-rw-r--r--   0     1001      123     2647 2023-06-16 15:27:19.000000 nacos_sdk_rust_binding_py-0.3.0/src/lib.rs
+-rw-r--r--   0     1001      123    11291 2023-06-16 15:27:19.000000 nacos_sdk_rust_binding_py-0.3.0/src/naming.rs
+-rw-r--r--   0     1001      123      230 2023-06-16 15:27:19.000000 nacos_sdk_rust_binding_py-0.3.0/test.sh
+-rw-r--r--   0     1001      123    38636 2023-06-16 15:27:29.000000 nacos_sdk_rust_binding_py-0.3.0/Cargo.lock
+-rw-r--r--   0        0        0     7286 1970-01-01 00:00:00.000000 nacos_sdk_rust_binding_py-0.3.0/PKG-INFO
```

### Comparing `nacos_sdk_rust_binding_py-0.1.2/Cargo.toml` & `nacos_sdk_rust_binding_py-0.3.0/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "nacos-sdk-rust-binding-py"
-version = "0.1.2"
+version = "0.3.0"
 edition = "2021"
 license = "Apache-2.0"
 publish = false
 authors = ["CheirshCai <785427346@qq.com>"]
 readme = "README.md"
 repository = "https://github.com/opc-source/nacos-sdk-rust-binding-py.git"
 description = "nacos-sdk-rust binding for Python with PyO3."
@@ -16,14 +16,14 @@
 name = "nacos_sdk_rust_binding_py"
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 pyo3 = "0.18"
 
-nacos-sdk = { version = "0.3.0-pre", features = ["default"] }
+nacos-sdk = { version = "0.3.0", features = ["default"] }
 #nacos-sdk = { git = "https://github.com/nacos-group/nacos-sdk-rust.git", features = ["default"] }
 
 tracing-subscriber = { version = "0.3", features = ["default"] }
 #tracing-subscriber = { version = "0.3", features = ["env-filter", "local-time"] } # occur `<unknown time>`
 tracing-appender = "0.2"
 lazy_static = "1.4.0"
```

### Comparing `nacos_sdk_rust_binding_py-0.1.2/.github/workflows/CI.yml` & `nacos_sdk_rust_binding_py-0.3.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `nacos_sdk_rust_binding_py-0.1.2/.gitignore` & `nacos_sdk_rust_binding_py-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `nacos_sdk_rust_binding_py-0.1.2/LICENSE` & `nacos_sdk_rust_binding_py-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nacos_sdk_rust_binding_py-0.1.2/README.md` & `nacos_sdk_rust_binding_py-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,19 @@
 
 - project package see https://pypi.org/project/nacos-sdk-rust-binding-py
 
 ## Usage
 
 **使用样例请看仓库内的 examples 目录**
 
+环境变量 `NACOS_CLIENT_LOGGER_LEVEL=INFO` 可设置日志打印级别，默认 INFO
 - 客户端日志请在目录 `$HOME/logs/nacos/` 查看
 
+环境变量 `NACOS_CLIENT_COMMON_THREAD_CORES=4` 可设置客户端核心线程数，默认是 CPU 数目 num_cpus
+
 ### Definition of ClientOptions
 
 ```python
 class ClientOptions:
     # Server Addr, e.g. address:port[,address:port],...]
     #[pyo3(set, get)]
     server_addr: String,
```

### Comparing `nacos_sdk_rust_binding_py-0.1.2/examples/config.py` & `nacos_sdk_rust_binding_py-0.3.0/examples/config.py`

 * *Files identical despite different names*

### Comparing `nacos_sdk_rust_binding_py-0.1.2/examples/naming.py` & `nacos_sdk_rust_binding_py-0.3.0/examples/naming.py`

 * *Files identical despite different names*

### Comparing `nacos_sdk_rust_binding_py-0.1.2/pyproject.toml` & `nacos_sdk_rust_binding_py-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nacos_sdk_rust_binding_py-0.1.2/src/config.rs` & `nacos_sdk_rust_binding_py-0.3.0/src/config.rs`

 * *Files identical despite different names*

### Comparing `nacos_sdk_rust_binding_py-0.1.2/src/lib.rs` & `nacos_sdk_rust_binding_py-0.3.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nacos_sdk_rust_binding_py-0.1.2/src/naming.rs` & `nacos_sdk_rust_binding_py-0.3.0/src/naming.rs`

 * *Files identical despite different names*

### Comparing `nacos_sdk_rust_binding_py-0.1.2/Cargo.lock` & `nacos_sdk_rust_binding_py-0.3.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -130,17 +130,17 @@
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.15"
+version = "0.8.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
+checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "darling"
 version = "0.14.4"
@@ -483,17 +483,17 @@
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "js-sys"
-version = "0.3.63"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2f37a4a5928311ac501dee68b3c7613a1037d0edb30c8e5427bd832d55d1b790"
+checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
@@ -576,17 +576,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "nacos-sdk"
-version = "0.3.0-pre"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ac71132b385b73262c1a11f7b40c5c1aee6e4909438dd9eb64d92701b507b9"
+checksum = "c804bed6b1feec49f2113f8a273552ab37b0a13527ff9f155b56d889bfeacac0"
 dependencies = [
  "async-stream",
  "async-trait",
  "dashmap",
  "futures",
  "futures-util",
  "home",
@@ -605,15 +605,15 @@
  "tower",
  "tracing",
  "want",
 ]
 
 [[package]]
 name = "nacos-sdk-rust-binding-py"
-version = "0.1.2"
+version = "0.3.0"
 dependencies = [
  "lazy_static",
  "nacos-sdk",
  "pyo3",
  "tracing-appender",
  "tracing-subscriber",
 ]
@@ -936,17 +936,17 @@
  "proc-macro2",
  "quote",
  "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.96"
+version = "1.0.97"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
+checksum = "bdf3bf93142acad5821c99197022e170842cdbc1c30482b98750c688c640842a"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1359,99 +1359,98 @@
 name = "valuable"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830b7e5d4d90034032940e4ace0d9a9a057e7a45cd94e6c007832e39edb82f6d"
 
 [[package]]
 name = "want"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ce8a968cb1cd110d136ff8b819a556d6fb6d919363c61534f6860c7eb172ba0"
+checksum = "bfa7760aed19e106de2c7c0b581b509f2f25d3dacaf737cb82ac61bc6d760b0e"
 dependencies = [
- "log",
  "try-lock",
 ]
 
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5bba0e8cb82ba49ff4e229459ff22a191bbe9a1cb3a341610c9c33efc27ddf73"
+checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "19b04bc93f9d6bdee709f6bd2118f57dd6679cf1176a1af464fca3ab0d66d8fb"
+checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
  "syn 2.0.18",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.36"
+version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2d1985d03709c53167ce907ff394f5316aa22cb4e12761295c5dc57dacb6297e"
+checksum = "c02dbc21516f9f1f04f187958890d7e6026df8d16540b7ad9492bc34a67cea03"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14d6b024f1a526bb0234f52840389927257beb670610081360e5a03c5df9c258"
+checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e128beba882dd1eb6200e1dc92ae6c5dbaa4311aa7bb211ca035779e5efc39f8"
+checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.18",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed9d5b4305409d1fc9482fee2d7f9bcbf24b3972bf59817ef757e23982242a93"
+checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
 
 [[package]]
 name = "web-sys"
-version = "0.3.63"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3bdd9ef4e984da1187bf8110c5cf5b845fbc87a23602cdf912386a76fcd3a7c2"
+checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "winapi"
```

### Comparing `nacos_sdk_rust_binding_py-0.1.2/PKG-INFO` & `nacos_sdk_rust_binding_py-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nacos-sdk-rust-binding-py
-Version: 0.1.2
+Version: 0.3.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pdoc ; extra == 'docs'
 Requires-Dist: behave ; extra == 'test'
 Provides-Extra: docs
 Provides-Extra: test
@@ -33,16 +33,19 @@
 
 - project package see https://pypi.org/project/nacos-sdk-rust-binding-py
 
 ## Usage
 
 **使用样例请看仓库内的 examples 目录**
 
+环境变量 `NACOS_CLIENT_LOGGER_LEVEL=INFO` 可设置日志打印级别，默认 INFO
 - 客户端日志请在目录 `$HOME/logs/nacos/` 查看
 
+环境变量 `NACOS_CLIENT_COMMON_THREAD_CORES=4` 可设置客户端核心线程数，默认是 CPU 数目 num_cpus
+
 ### Definition of ClientOptions
 
 ```python
 class ClientOptions:
     # Server Addr, e.g. address:port[,address:port],...]
     #[pyo3(set, get)]
     server_addr: String,
```

