# Comparing `tmp/techbureau-symbol-sdk-python-3.0.7.dev1.tar.gz` & `tmp/techbureau-symbol-sdk-python-3.0.7.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "techbureau-symbol-sdk-python-3.0.7.dev1.tar", last modified: Fri Apr 28 03:51:36 2023, max compression
+gzip compressed data, was "techbureau-symbol-sdk-python-3.0.7.dev2.tar", last modified: Fri Jun 16 02:05:14 2023, max compression
```

## Comparing `techbureau-symbol-sdk-python-3.0.7.dev1.tar` & `techbureau-symbol-sdk-python-3.0.7.dev2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:36.057877 techbureau-symbol-sdk-python-3.0.7.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-28 03:51:36.057877 techbureau-symbol-sdk-python-3.0.7.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 03:51:36.057877 techbureau-symbol-sdk-python-3.0.7.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:36.053877 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/AccountDescriptorRepository.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/ArrayHelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/BaseValue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/Bip32.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/BlockchainSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/BufferReader.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/BufferWriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/ByteArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/Cipher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/CodeWordsEncoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/CryptoTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/DiceMnemonicGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/Network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/NetworkTimestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/NodeDescriptorRepository.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/Ordered.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/PrivateKeyStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/QrSignatureStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/QrStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/RuleBasedTransactionFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/SharedKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/TransactionDescriptorProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/Transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:36.053877 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/external/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/external/ed25519.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:36.053877 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/facade/
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/facade/BatchOperations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/facade/NemFacade.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/facade/SymbolFacade.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/facade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:36.053877 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nc/
--rw-r--r--   0 runner    (1001) docker     (123)   178806 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:36.053877 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nem/
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nem/KeyPair.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nem/MessageEncoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nem/Network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nem/SharedKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nem/TransactionFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/ripemd160.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:36.053877 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/sc/
--rw-r--r--   0 runner    (1001) docker     (123)   477712 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/sc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:36.057877 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/IdGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/KeyPair.py
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/Merkle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/MessageEncoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/Metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/Network.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/SharedKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/TransactionFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/VotingKeysGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:36.057877 techbureau-symbol-sdk-python-3.0.7.dev1/techbureau_symbol_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-28 03:51:36.000000 techbureau-symbol-sdk-python-3.0.7.dev1/techbureau_symbol_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-28 03:51:36.000000 techbureau-symbol-sdk-python-3.0.7.dev1/techbureau_symbol_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 03:51:36.000000 techbureau-symbol-sdk-python-3.0.7.dev1/techbureau_symbol_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-28 03:51:36.000000 techbureau-symbol-sdk-python-3.0.7.dev1/techbureau_symbol_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 03:51:36.000000 techbureau-symbol-sdk-python-3.0.7.dev1/techbureau_symbol_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:05:14.964110 techbureau-symbol-sdk-python-3.0.7.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-16 02:05:14.964110 techbureau-symbol-sdk-python-3.0.7.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 02:05:14.964110 techbureau-symbol-sdk-python-3.0.7.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:05:14.960110 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/AccountDescriptorRepository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/ArrayHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/BaseValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/Bip32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/BlockchainSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/BufferReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/BufferWriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/ByteArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/Cipher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/CodeWordsEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/CryptoTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/DiceMnemonicGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/Network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/NetworkTimestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/NodeDescriptorRepository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/Ordered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/PrivateKeyStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/QrSignatureStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/QrStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/RuleBasedTransactionFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/SharedKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/TransactionDescriptorProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/Transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:05:14.960110 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/external/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/external/ed25519.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:05:14.960110 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/facade/
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/facade/BatchOperations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/facade/NemFacade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/facade/SymbolFacade.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/facade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:05:14.960110 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/nc/
+-rw-r--r--   0 runner    (1001) docker     (123)   178806 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/nc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:05:14.960110 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/nem/
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/nem/KeyPair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/nem/MessageEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/nem/Network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/nem/SharedKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/nem/TransactionFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/nem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/ripemd160.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:05:14.960110 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/sc/
+-rw-r--r--   0 runner    (1001) docker     (123)   477712 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/sc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:05:14.964110 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/symbol/
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/symbol/IdGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/symbol/KeyPair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/symbol/Merkle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/symbol/MessageEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/symbol/Metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/symbol/Network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/symbol/SharedKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/symbol/TransactionFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/symbol/VotingKeysGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:05:06.000000 techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/symbol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:05:14.964110 techbureau-symbol-sdk-python-3.0.7.dev2/techbureau_symbol_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-16 02:05:14.000000 techbureau-symbol-sdk-python-3.0.7.dev2/techbureau_symbol_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-16 02:05:14.000000 techbureau-symbol-sdk-python-3.0.7.dev2/techbureau_symbol_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 02:05:14.000000 techbureau-symbol-sdk-python-3.0.7.dev2/techbureau_symbol_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-16 02:05:14.000000 techbureau-symbol-sdk-python-3.0.7.dev2/techbureau_symbol_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 02:05:14.000000 techbureau-symbol-sdk-python-3.0.7.dev2/techbureau_symbol_sdk_python.egg-info/top_level.txt
```

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/README.md` & `techbureau-symbol-sdk-python-3.0.7.dev2/README.md`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/setup.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 {'': ['*']}
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup_kwargs = {
     'name': 'techbureau-symbol-sdk-python',
-    'version': '3.0.7.dev1',
+    'version': '3.0.7.dev2',
     'description': 'Symbol SDK',
     'long_description': 'This is symbol project core sdk python library.',
     'author': 'Techbureau Contributors',
     'author_email': 'development@techbureau.jp',
     'maintainer': 'Techbureau Contributors',
     'maintainer_email': 'development@techbureau.jp',
     'url': 'https://github.com/tech-bureau-jp/symbol/tree/dev/sdk/python',
```

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/AccountDescriptorRepository.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/AccountDescriptorRepository.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/ArrayHelpers.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/ArrayHelpers.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/BaseValue.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/BaseValue.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/Bip32.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/Bip32.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/BlockchainSettings.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/BlockchainSettings.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/BufferReader.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/BufferReader.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/BufferWriter.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/BufferWriter.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/ByteArray.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/ByteArray.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/Cipher.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/Cipher.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/CodeWordsEncoder.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/CodeWordsEncoder.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/CryptoTypes.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/CryptoTypes.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/DiceMnemonicGenerator.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/DiceMnemonicGenerator.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/Network.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/Network.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/NetworkTimestamp.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/NetworkTimestamp.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/NodeDescriptorRepository.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/NodeDescriptorRepository.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/PrivateKeyStorage.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/PrivateKeyStorage.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/QrSignatureStorage.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/QrSignatureStorage.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/QrStorage.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/QrStorage.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/RuleBasedTransactionFactory.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/RuleBasedTransactionFactory.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/SharedKey.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/SharedKey.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/TransactionDescriptorProcessor.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/TransactionDescriptorProcessor.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 			value = self.type_parsing_rules[type_hint](value)
 
 		return value
 
 	def lookup_value(self, key):
 		"""Looks up the value for key."""
 		value = self._lookup_value_and_apply_type_hints(key)
-		if not any(isinstance(value, type_class) for type_class in [str, bytes, tuple]) and hasattr(value, '__iter__'):
+		if not any(isinstance(value, type_class) for type_class in [str, bytes, tuple]) and isinstance(value, list):
 			return [self.type_converter(item) for item in value]
 
 		return self.type_converter(value)
 
 	def copy_to(self, transaction, ignore_keys=None):
 		"""Copies all descriptor information to a transaction."""
 		for key in self.transaction_descriptor.keys():
```

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/external/ed25519.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/external/ed25519.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/facade/BatchOperations.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/facade/BatchOperations.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/facade/NemFacade.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/facade/NemFacade.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/facade/SymbolFacade.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/facade/SymbolFacade.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nc/__init__.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/nc/__init__.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nem/KeyPair.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/nem/KeyPair.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nem/MessageEncoder.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/nem/MessageEncoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+import warnings
+
 import cryptography
 
 from symbolchain.CryptoTypes import PublicKey
 from symbolchain.impl.CipherHelpers import decode_aes_cbc, decode_aes_gcm, encode_aes_cbc, encode_aes_gcm
 from symbolchain.nc import Message, MessageType
 from symbolchain.nem.KeyPair import KeyPair
 from symbolchain.nem.SharedKey import SharedKey
 
 
 class MessageEncoder:
 	"""Encrypts and encodes messages between two parties."""
 
 	def __init__(self, key_pair: KeyPair):
 		"""Creates message encoder around key pair."""
+
 		self.key_pair = key_pair
 
 	def try_decode(self, recipient_public_key, encoded_message: Message):
 		"""Tries to decode encoded message, returns tuple:
 		* True, message - if message has been decoded and decrypted
 		* False, encoded_message - otherwise
 		"""
@@ -38,26 +41,32 @@
 				'Invalid IV size',
 				'The length of the provided data is not a multiple of the block length']
 			if not any(map(lambda message: message in str(exception), exceptions)):
 				raise
 
 		return False, encoded_message
 
-	def encode_deprecated(self, recipient_public_key: PublicKey, message: bytes):
-		"""Encodes message to recipient using deprecated encryption and key derivation."""
+	def encode(self, recipient_public_key: PublicKey, message: bytes):
+		"""Encodes message to recipient using recommended format."""
 
-		salt, initialization_vector, cipher_text = encode_aes_cbc(SharedKey, self.key_pair, recipient_public_key, message)
+		tag, initialization_vector, cipher_text = encode_aes_gcm(SharedKey, self.key_pair, recipient_public_key, message)
 
 		encoded_messsage = Message()
 		encoded_messsage.message_type = MessageType.ENCRYPTED
-		encoded_messsage.message = salt + initialization_vector + cipher_text
+		encoded_messsage.message = tag + initialization_vector + cipher_text
 		return encoded_messsage
 
-	def encode(self, recipient_public_key: PublicKey, message: bytes):
-		"""Encodes message to recipient using recommended format."""
+	def encode_deprecated(self, recipient_public_key: PublicKey, message: bytes):
+		"""Encodes message to recipient using deprecated encryption and key derivation."""
 
-		tag, initialization_vector, cipher_text = encode_aes_gcm(SharedKey, self.key_pair, recipient_public_key, message)
+		warnings.warn(
+			'This function is only provided for compatability with older NEM messages.\n'
+			'Please use `encode` in any new code.',
+			category=DeprecationWarning,
+			stacklevel=2)
+
+		salt, initialization_vector, cipher_text = encode_aes_cbc(SharedKey, self.key_pair, recipient_public_key, message)
 
 		encoded_messsage = Message()
 		encoded_messsage.message_type = MessageType.ENCRYPTED
-		encoded_messsage.message = tag + initialization_vector + cipher_text
+		encoded_messsage.message = salt + initialization_vector + cipher_text
 		return encoded_messsage
```

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nem/Network.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/nem/Network.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nem/SharedKey.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/nem/SharedKey.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nem/TransactionFactory.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/nem/TransactionFactory.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/sc/__init__.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/sc/__init__.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/IdGenerator.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/symbol/IdGenerator.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/KeyPair.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/symbol/KeyPair.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/Merkle.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/symbol/Merkle.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/Metadata.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/symbol/Metadata.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/Network.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/symbol/Network.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/TransactionFactory.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/symbol/TransactionFactory.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/VotingKeysGenerator.py` & `techbureau-symbol-sdk-python-3.0.7.dev2/symbolchain/symbol/VotingKeysGenerator.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.7.dev1/techbureau_symbol_sdk_python.egg-info/SOURCES.txt` & `techbureau-symbol-sdk-python-3.0.7.dev2/techbureau_symbol_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

