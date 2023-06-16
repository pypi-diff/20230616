# Comparing `tmp/blockchain-apis-0.1.4.tar.gz` & `tmp/blockchain-apis-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockchain-apis-0.1.4.tar", last modified: Mon Jun 12 14:54:01 2023, max compression
+gzip compressed data, was "blockchain-apis-0.2.0.tar", last modified: Fri Jun 16 11:35:00 2023, max compression
```

## Comparing `blockchain-apis-0.1.4.tar` & `blockchain-apis-0.2.0.tar`

### file list

```diff
@@ -1,58 +1,65 @@
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-12 14:54:01.143603 blockchain-apis-0.1.4/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1095 2023-05-30 13:02:28.000000 blockchain-apis-0.1.4/LICENSE
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4722 2023-06-12 14:54:01.143603 blockchain-apis-0.1.4/PKG-INFO
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3170 2023-06-02 15:30:18.000000 blockchain-apis-0.1.4/README.md
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       38 2023-06-12 14:54:01.143603 blockchain-apis-0.1.4/setup.cfg
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1970 2023-06-12 14:53:32.000000 blockchain-apis-0.1.4/setup.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-12 14:54:01.135603 blockchain-apis-0.1.4/src/
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-12 14:54:01.135603 blockchain-apis-0.1.4/src/blockchain_apis.egg-info/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4722 2023-06-12 14:54:01.000000 blockchain-apis-0.1.4/src/blockchain_apis.egg-info/PKG-INFO
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1718 2023-06-12 14:54:01.000000 blockchain-apis-0.1.4/src/blockchain_apis.egg-info/SOURCES.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)        1 2023-06-12 14:54:01.000000 blockchain-apis-0.1.4/src/blockchain_apis.egg-info/dependency_links.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       17 2023-06-12 14:54:01.000000 blockchain-apis-0.1.4/src/blockchain_apis.egg-info/requires.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       15 2023-06-12 14:54:01.000000 blockchain-apis-0.1.4/src/blockchain_apis.egg-info/top_level.txt
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-12 14:54:01.135603 blockchain-apis-0.1.4/src/blockchainapis/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    26306 2023-06-12 14:52:41.000000 blockchain-apis-0.1.4/src/blockchainapis/BlockchainAPIs.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    25252 2023-06-12 14:53:10.000000 blockchain-apis-0.1.4/src/blockchainapis/BlockchainAPIsSync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      622 2023-06-12 14:52:13.000000 blockchain-apis-0.1.4/src/blockchainapis/__init__.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-12 14:54:01.135603 blockchain-apis-0.1.4/src/blockchainapis/exceptions/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      454 2023-06-12 14:51:30.000000 blockchain-apis-0.1.4/src/blockchainapis/exceptions/BlockchainAPIsException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      681 2023-06-12 14:51:30.000000 blockchain-apis-0.1.4/src/blockchainapis/exceptions/BlockchainNotSupportedException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      674 2023-06-12 14:51:30.000000 blockchain-apis-0.1.4/src/blockchainapis/exceptions/ExchangeNotSupportedException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      771 2023-06-12 14:51:30.000000 blockchain-apis-0.1.4/src/blockchainapis/exceptions/InvalidPageException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      794 2023-06-12 14:51:30.000000 blockchain-apis-0.1.4/src/blockchainapis/exceptions/PairNotFoundException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      773 2023-06-12 14:51:30.000000 blockchain-apis-0.1.4/src/blockchainapis/exceptions/TokenNotFoundException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      708 2023-06-12 14:51:30.000000 blockchain-apis-0.1.4/src/blockchainapis/exceptions/TooManyRequestsException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      691 2023-06-12 14:51:30.000000 blockchain-apis-0.1.4/src/blockchainapis/exceptions/UnauthorizedException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      922 2023-06-12 14:51:30.000000 blockchain-apis-0.1.4/src/blockchainapis/exceptions/__init__.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-12 14:54:01.139603 blockchain-apis-0.1.4/src/blockchainapis/models/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      859 2023-06-12 14:51:30.000000 blockchain-apis-0.1.4/src/blockchainapis/models/AmountIn.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      870 2023-06-12 14:51:30.000000 blockchain-apis-0.1.4/src/blockchainapis/models/AmountOut.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      579 2023-06-12 14:51:30.000000 blockchain-apis-0.1.4/src/blockchainapis/models/Blockchain.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      547 2023-06-12 14:51:30.000000 blockchain-apis-0.1.4/src/blockchainapis/models/Exchange.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      863 2023-06-12 14:51:30.000000 blockchain-apis-0.1.4/src/blockchainapis/models/Exchanges.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      677 2023-06-12 14:51:30.000000 blockchain-apis-0.1.4/src/blockchainapis/models/Pair.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      933 2023-06-12 14:51:30.000000 blockchain-apis-0.1.4/src/blockchainapis/models/Pairs.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      794 2023-06-12 14:51:30.000000 blockchain-apis-0.1.4/src/blockchainapis/models/Reserve.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      760 2023-06-12 14:51:30.000000 blockchain-apis-0.1.4/src/blockchainapis/models/Token.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1826 2023-06-12 14:51:30.000000 blockchain-apis-0.1.4/src/blockchainapis/models/Tokens.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1475 2023-06-12 14:51:30.000000 blockchain-apis-0.1.4/src/blockchainapis/models/__init__.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-12 14:54:01.143603 blockchain-apis-0.1.4/tests/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1564 2023-06-10 14:12:58.000000 blockchain-apis-0.1.4/tests/test_amount_in.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1540 2023-06-10 14:12:58.000000 blockchain-apis-0.1.4/tests/test_amount_in_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1568 2023-06-10 14:12:58.000000 blockchain-apis-0.1.4/tests/test_amount_out.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1544 2023-06-10 14:12:58.000000 blockchain-apis-0.1.4/tests/test_amount_out_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      425 2023-06-10 14:12:58.000000 blockchain-apis-0.1.4/tests/test_blockchains.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      419 2023-06-10 14:12:58.000000 blockchain-apis-0.1.4/tests/test_blockchains_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      569 2023-06-10 14:12:58.000000 blockchain-apis-0.1.4/tests/test_decimals.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      563 2023-06-10 14:12:58.000000 blockchain-apis-0.1.4/tests/test_decimals_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1291 2023-06-10 14:12:58.000000 blockchain-apis-0.1.4/tests/test_exchanges.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1231 2023-06-10 14:12:58.000000 blockchain-apis-0.1.4/tests/test_exchanges_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      593 2023-06-10 14:12:58.000000 blockchain-apis-0.1.4/tests/test_info.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      587 2023-06-10 14:12:58.000000 blockchain-apis-0.1.4/tests/test_info_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2699 2023-06-10 14:12:58.000000 blockchain-apis-0.1.4/tests/test_pairs.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2567 2023-06-10 14:12:58.000000 blockchain-apis-0.1.4/tests/test_pairs_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1392 2023-06-10 14:12:58.000000 blockchain-apis-0.1.4/tests/test_reserves.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1368 2023-06-10 14:12:58.000000 blockchain-apis-0.1.4/tests/test_reserves_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1249 2023-06-10 14:12:58.000000 blockchain-apis-0.1.4/tests/test_tokens.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1189 2023-06-10 14:12:58.000000 blockchain-apis-0.1.4/tests/test_tokens_sync.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-16 11:35:00.608572 blockchain-apis-0.2.0/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1095 2023-05-30 13:02:28.000000 blockchain-apis-0.2.0/LICENSE
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4722 2023-06-16 11:35:00.608572 blockchain-apis-0.2.0/PKG-INFO
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3170 2023-06-02 15:30:18.000000 blockchain-apis-0.2.0/README.md
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       38 2023-06-16 11:35:00.608572 blockchain-apis-0.2.0/setup.cfg
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1970 2023-06-16 11:33:21.000000 blockchain-apis-0.2.0/setup.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-16 11:35:00.592571 blockchain-apis-0.2.0/src/
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-16 11:35:00.596572 blockchain-apis-0.2.0/src/blockchain_apis.egg-info/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4722 2023-06-16 11:35:00.000000 blockchain-apis-0.2.0/src/blockchain_apis.egg-info/PKG-INFO
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2009 2023-06-16 11:35:00.000000 blockchain-apis-0.2.0/src/blockchain_apis.egg-info/SOURCES.txt
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)        1 2023-06-16 11:35:00.000000 blockchain-apis-0.2.0/src/blockchain_apis.egg-info/dependency_links.txt
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       17 2023-06-16 11:35:00.000000 blockchain-apis-0.2.0/src/blockchain_apis.egg-info/requires.txt
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       15 2023-06-16 11:35:00.000000 blockchain-apis-0.2.0/src/blockchain_apis.egg-info/top_level.txt
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-16 11:35:00.596572 blockchain-apis-0.2.0/src/blockchainapis/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    30775 2023-06-16 11:29:53.000000 blockchain-apis-0.2.0/src/blockchainapis/BlockchainAPIs.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    29587 2023-06-16 11:32:43.000000 blockchain-apis-0.2.0/src/blockchainapis/BlockchainAPIsSync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      622 2023-06-16 11:33:29.000000 blockchain-apis-0.2.0/src/blockchainapis/__init__.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-16 11:35:00.600572 blockchain-apis-0.2.0/src/blockchainapis/exceptions/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      460 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/exceptions/BlockchainAPIsException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      683 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/exceptions/BlockchainNotSupportedException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      676 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/exceptions/ExchangeNotSupportedException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      773 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/exceptions/InvalidPageException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      796 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/exceptions/PairNotFoundException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      775 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/exceptions/TokenNotFoundException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      710 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/exceptions/TooManyRequestsException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      693 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/exceptions/UnauthorizedException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      418 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/exceptions/UnknownBlockchainAPIsException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      922 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/exceptions/__init__.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-16 11:35:00.600572 blockchain-apis-0.2.0/src/blockchainapis/models/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      859 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/models/AmountIn.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      870 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/models/AmountOut.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      579 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/models/Blockchain.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      547 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/models/Exchange.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      863 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/models/Exchanges.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      677 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/models/Pair.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      933 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/models/Pairs.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      794 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/models/Reserve.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      760 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/models/Token.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1826 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/models/Tokens.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1475 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/src/blockchainapis/models/__init__.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-16 11:35:00.608572 blockchain-apis-0.2.0/tests/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1564 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_amount_in.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1540 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_amount_in_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1568 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_amount_out.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1544 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_amount_out_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      425 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_blockchains.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      419 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_blockchains_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3237 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_decimal_unsigned.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3169 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_decimal_unsigned_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      569 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_decimals.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      563 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_decimals_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1291 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_exchanges.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1231 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_exchanges_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1322 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_get_token_decimal_form.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1296 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_get_token_decimal_form_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1561 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_get_token_unsigned_form.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1529 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_get_token_unsigned_form_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      593 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_info.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      587 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_info_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2699 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_pairs.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2567 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_pairs_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1392 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_reserves.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1368 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_reserves_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1249 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_tokens.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1189 2023-06-16 11:29:16.000000 blockchain-apis-0.2.0/tests/test_tokens_sync.py
```

### Comparing `blockchain-apis-0.1.4/LICENSE` & `blockchain-apis-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/PKG-INFO` & `blockchain-apis-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockchain-apis
-Version: 0.1.4
+Version: 0.2.0
 Summary: Fastest and easiest way to access decentralized finance data
 Home-page: https://www.blockchainapis.io
 Author: Clarensia
 Author-email: contact@blockchainapis.io
 License: MIT
 Project-URL: Documentation, https://api.blockchainapis.io/docs
 Project-URL: Source, https://github.com/blockchainapis/blockchain-apis-python-client
```

### Comparing `blockchain-apis-0.1.4/README.md` & `blockchain-apis-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/setup.py` & `blockchain-apis-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
     
 setup(
     name = "blockchain-apis",
-    version = "0.1.4",
+    version = "0.2.0",
     author = "Clarensia",
     author_email = "contact@blockchainapis.io",
     description = "Fastest and easiest way to access decentralized finance data",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://www.blockchainapis.io",
     license="MIT",
```

### Comparing `blockchain-apis-0.1.4/src/blockchain_apis.egg-info/PKG-INFO` & `blockchain-apis-0.2.0/src/blockchain_apis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockchain-apis
-Version: 0.1.4
+Version: 0.2.0
 Summary: Fastest and easiest way to access decentralized finance data
 Home-page: https://www.blockchainapis.io
 Author: Clarensia
 Author-email: contact@blockchainapis.io
 License: MIT
 Project-URL: Documentation, https://api.blockchainapis.io/docs
 Project-URL: Source, https://github.com/blockchainapis/blockchain-apis-python-client
```

### Comparing `blockchain-apis-0.1.4/src/blockchain_apis.egg-info/SOURCES.txt` & `blockchain-apis-0.2.0/src/blockchain_apis.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 src/blockchainapis/exceptions/BlockchainNotSupportedException.py
 src/blockchainapis/exceptions/ExchangeNotSupportedException.py
 src/blockchainapis/exceptions/InvalidPageException.py
 src/blockchainapis/exceptions/PairNotFoundException.py
 src/blockchainapis/exceptions/TokenNotFoundException.py
 src/blockchainapis/exceptions/TooManyRequestsException.py
 src/blockchainapis/exceptions/UnauthorizedException.py
+src/blockchainapis/exceptions/UnknownBlockchainAPIsException.py
 src/blockchainapis/exceptions/__init__.py
 src/blockchainapis/models/AmountIn.py
 src/blockchainapis/models/AmountOut.py
 src/blockchainapis/models/Blockchain.py
 src/blockchainapis/models/Exchange.py
 src/blockchainapis/models/Exchanges.py
 src/blockchainapis/models/Pair.py
@@ -31,18 +32,24 @@
 src/blockchainapis/models/__init__.py
 tests/test_amount_in.py
 tests/test_amount_in_sync.py
 tests/test_amount_out.py
 tests/test_amount_out_sync.py
 tests/test_blockchains.py
 tests/test_blockchains_sync.py
+tests/test_decimal_unsigned.py
+tests/test_decimal_unsigned_sync.py
 tests/test_decimals.py
 tests/test_decimals_sync.py
 tests/test_exchanges.py
 tests/test_exchanges_sync.py
+tests/test_get_token_decimal_form.py
+tests/test_get_token_decimal_form_sync.py
+tests/test_get_token_unsigned_form.py
+tests/test_get_token_unsigned_form_sync.py
 tests/test_info.py
 tests/test_info_sync.py
 tests/test_pairs.py
 tests/test_pairs_sync.py
 tests/test_reserves.py
 tests/test_reserves_sync.py
 tests/test_tokens.py
```

### Comparing `blockchain-apis-0.1.4/src/blockchainapis/BlockchainAPIs.py` & `blockchain-apis-0.2.0/src/blockchainapis/BlockchainAPIs.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from .exceptions import BlockchainNotSupportedException
 from .exceptions import ExchangeNotSupportedException
 from .exceptions import InvalidPageException
 from .exceptions import TokenNotFoundException
 from .exceptions import PairNotFoundException
 from .exceptions import TooManyRequestsException
 from .exceptions import UnauthorizedException
+from .exceptions import UnknownBlockchainAPIsException
 
 
 class BlockchainAPIs:
     """High-frequency DEX API
 
     Our API empowers you to access live financial data across multiple blockchains
     (currently supporting 6, with more on the way) with unparalleled speed and efficiency.
@@ -99,14 +100,23 @@
         await self.close()
 
     async def _do_request(self, path: str, params: Dict[str, Any] | None = None) -> Dict[str, Any]:
         """Make raw API request (that return the json result).
         
         This method additionaly adds the user API key to the request if it is present.
 
+        :raises BlockchainNotSupportedException: Thrown when an Invalid blockchain id is put during a call to the API.
+        :raises ExchangeNotSupportedException: Thrown when an Invalid exchange id is given during a call to the API.
+        :raises InvalidPageException: Thrown when you given an invalid page index during calls to responses thatgives paginated results.
+        :raises TokenNotFoundException: Thrown when you try to get informations on a token that does not exist inside of our database.
+        :raises PairNotFoundException: Thrown when you try to get some data about a pair that does not exist.
+        :raises TooManyRequestsException: Thrown when you are doing more request than you are allowed to the API.
+        :raises UnauthorizedException: Thrown when you are trying to make an API request with an invalid or expiredAPI key.
+        :raises UnknownBlockchainAPIsException: When an unknown exception happens
+
         :param path: The path to the request
         :type path: str
         :param params: The optional query parameters of the request, defaults to None
         :type params: Dict[str, Any] | None, optional
         :return: The json-formated result
         :rtype: Dict[str, None]
         """
@@ -125,16 +135,16 @@
                         raise TokenNotFoundException(response.status, error_data["detail"]["detail"])
                     case "PairNotFoundException":
                         raise PairNotFoundException(response.status, error_data["detail"]["detail"])
                     case "TooManyRequestsException":
                         raise TooManyRequestsException(response.status, error_data["detail"]["detail"])
                     case "UnauthorizedException":
                         raise UnauthorizedException(response.status, error_data["detail"]["detail"])
-                    case unknown:
-                        raise Exception(f"Unkwnown Exception type: {unknown}.\nGot this exception while handling:\n{error_data} with status code: {response.status}")
+                    case _:
+                        raise UnknownBlockchainAPIsException(response.status, f"Unkwnown Exception type: {error_type}.\nGot this exception while handling:\n{error_data} with status code: {response.status}")
 
             return await response.json()
 
     async def blockchains(self) -> List[Blockchain]:
         """Get the list of blockchains supported by the API
 
 
@@ -658,15 +668,16 @@
             decimals=ret["decimals"],
             market_cap=ret["market_cap"]
         )
 
     async def decimals(self, blockchain: str, token: str) -> int:
         """Get the decimals of the given token
 
-        :raises HTTPValidationError: Validation Error
+        :raises BlockchainNotSupportedException: When an invalid blockchain id is given
+        :raises TokenNotFoundException: WHen the given token is not found
 
         :param blockchain: The id of the blockchain of the token
         :type blockchain: str
         :example blockchain: ethereum
         :param token: The address of the token that you want to get the decimals from
         :type token: str
         :example token: 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2
@@ -680,7 +691,90 @@
         :rtype: int
         """
         params = {}
         params["blockchain"] = blockchain
         params["token"] = token
         ret = await self._do_request("/v0/tokens/decimals", params)
         return int(ret)
+
+    def get_token_decimal_form(self, amount: int, decimals: int) -> str:
+        """Convert a token from his unsigned integer form to his decimal form.
+        
+        This method should be used when you want to display a token to a user.
+        
+        For highest precision, the implementation is made using only str.
+
+        :param amount: The integer amount that you want to convert
+        :type amount: int
+        :example amount: 2500000000000000000
+        :param decimals: The amount of decimals that the token you are trying to convert
+                         has. You can use the [decimals](/docs/python-sdk/blockchain-apis/decimals)
+                         method in order to get the amount of decimals.
+        :type decimals: int
+        :example decimals: 18
+        :return: The given amount in a decimal form.
+        
+        Example response:
+        ```json
+        2.5
+        ```
+        :rtype: str
+        """
+        str_amount = str(amount)
+
+        # special case when decimals is 0
+        if decimals == 0:
+            return str_amount
+
+        # Check if the string length is less than the decimals
+        if len(str_amount) <= decimals:
+            # Add leading zeros to the string
+            str_amount = '0' * (decimals - len(str_amount) + 1) + str_amount
+            
+        # Insert the decimal point at the correct position
+        str_amount = str_amount[:-decimals] + "." + str_amount[-decimals:]
+        
+        str_amount = str_amount.rstrip('0').rstrip('.') if '.' in str_amount else str_amount
+        return str_amount
+
+    def get_token_unsigned_form(self, amount: str, decimals: int) -> int:
+        """Convert a token from his decimal form back to his unsigned integer form (this
+        method does the reverse of get_token_decimal_form)
+        
+        This method should be used when you receive an amount from a user, in order to convert his
+        input.
+
+        For the highest precision, the implementation only uses str
+
+        :param amount: The amount in str format that you want to convert
+        :type amount: str
+        :example amount: 2.5
+        :param decimals: The amount of decimals that the token has. You can use the [decimals](/docs/python-sdk/blockchain-apis/decimals)
+                         method in order to get the amount of decimals.
+        :type decimals: int
+        :example decimals: 18
+        :return: The amount converted to unsigned integer
+        
+        Example response:
+        ```json
+        2500000000000000000
+        ```
+        :rtype: int
+        """
+        split = amount.split('.')
+        if len(split) >= 2:
+            integer_part, fractional_part = split
+        else:
+            integer_part, fractional_part = split[0], ""
+
+        # Check if the fractional part has less digits than the decimal places
+        if len(fractional_part) < decimals:
+            # Append zeros to the end of the fractional part
+            fractional_part += '0' * (decimals - len(fractional_part))
+        else:
+            # Trim the fractional part to the number of decimal places
+            fractional_part = fractional_part[:decimals]
+
+        # Combine the integer and fractional parts and convert to an integer
+        integer_token_amount = int(integer_part + fractional_part)
+
+        return integer_token_amount
```

### Comparing `blockchain-apis-0.1.4/src/blockchainapis/BlockchainAPIsSync.py` & `blockchain-apis-0.2.0/src/blockchainapis/BlockchainAPIsSync.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from .exceptions import BlockchainNotSupportedException
 from .exceptions import ExchangeNotSupportedException
 from .exceptions import InvalidPageException
 from .exceptions import TokenNotFoundException
 from .exceptions import PairNotFoundException
 from .exceptions import TooManyRequestsException
 from .exceptions import UnauthorizedException
+from .exceptions import UnknownBlockchainAPIsException
 
 
 class BlockchainAPIsSync:
     """High-frequency DEX API
 
     Our API empowers you to access live financial data across multiple blockchains
     (currently supporting 6, with more on the way) with unparalleled speed and efficiency.
@@ -38,17 +39,14 @@
     protocols. With our API, you can reuse the same code without changing a single line, simplifying
     the development process and saving you valuable time.
     
     Ready to try it out? [Sign up for a free API key here](https://dashboard.blockchainapis.io)
     or start exploring the possibilities on this page. Need support or have questions? Join our
     [Discord community](https://discord.gg/GphRMJXmS5) where our team and fellow developers are
     eager to help you make the most of our powerful API.
-
-    Please note that this class is not async which is less optimized. To run more otpimized
-    requests, please use: BlockchainAPIs
     """
     
     def __init__(self, api_key: str | None = None):
         """Creates a BlockchainAPIsSync sync instance that allow you to make API calls
         in a synchronous way.
 
         The client works without an API key, but for better performance, we advise you
@@ -67,14 +65,23 @@
 
     def _do_request(self, path: str, params: Dict[str, Any] | None = None) -> Dict[str, Any]:
         """Make a raw API request (that return the json result).
         
         It makes the request in a synchronous way and you don't need to close the
         BlockchainAPIs instance.
 
+        :raises BlockchainNotSupportedException: Thrown when an Invalid blockchain id is put during a call to the API.
+        :raises ExchangeNotSupportedException: Thrown when an Invalid exchange id is given during a call to the API.
+        :raises InvalidPageException: Thrown when you given an invalid page index during calls to responses thatgives paginated results.
+        :raises TokenNotFoundException: Thrown when you try to get informations on a token that does not exist inside of our database.
+        :raises PairNotFoundException: Thrown when you try to get some data about a pair that does not exist.
+        :raises TooManyRequestsException: Thrown when you are doing more request than you are allowed to the API.
+        :raises UnauthorizedException: Thrown when you are trying to make an API request with an invalid or expiredAPI key.
+        :raises UnknownBlockchainAPIsException: When an unknown exception happens
+
         :param path: The path of the request
         :type path: str
         :param params: The optional query parameters of the request, defaults to None
         :type params: Dict[str, Any] | None, optional
         :return: The json-formated result
         :rtype: Dict[str, Any]
         """
@@ -94,16 +101,16 @@
                     raise TokenNotFoundException(response.status_code, error_data["detail"]["detail"])
                 case "PairNotFoundException":
                     raise PairNotFoundException(response.status_code, error_data["detail"]["detail"])
                 case "TooManyRequestsException":
                     raise TooManyRequestsException(response.status_code, error_data["detail"]["detail"])
                 case "UnauthorizedException":
                     raise UnauthorizedException(response.status_code, error_data["detail"]["detail"])
-                case unknown:
-                    raise Exception(f"Unkwnown Exception type: {unknown}.\nGot this exception while handling:\n{error_data} with status code: {response.status}")
+                case _:
+                    raise UnknownBlockchainAPIsException(response.status, f"Unkwnown Exception type: {error_type}.\nGot this exception while handling:\n{error_data} with status code: {response.status}")
 
         return response.json()
 
     def blockchains(self) -> List[Blockchain]:
         """Get the list of blockchains supported by the API
 
 
@@ -627,15 +634,16 @@
             decimals=ret["decimals"],
             market_cap=ret["market_cap"]
         )
 
     def decimals(self, blockchain: str, token: str) -> int:
         """Get the decimals of the given token
 
-        :raises HTTPValidationError: Validation Error
+        :raises BlockchainNotSupportedException: When an invalid blockchain id is given
+        :raises TokenNotFoundException: WHen the given token is not found
 
         :param blockchain: The id of the blockchain of the token
         :type blockchain: str
         :example blockchain: ethereum
         :param token: The address of the token that you want to get the decimals from
         :type token: str
         :example token: 0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2
@@ -649,7 +657,90 @@
         :rtype: int
         """
         params = {}
         params["blockchain"] = blockchain
         params["token"] = token
         ret = self._do_request("/v0/tokens/decimals", params)
         return int(ret)
+
+    def get_token_decimal_form(self, amount: int, decimals: int) -> str:
+        """Convert a token from his unsigned integer form to his decimal form.
+        
+        This method should be used when you want to display a token to a user.
+        
+        For highest precision, the implementation is made using only str.
+
+        :param amount: The integer amount that you want to convert
+        :type amount: int
+        :example amount: 2500000000000000000
+        :param decimals: The amount of decimals that the token you are trying to convert
+                         has. You can use the [decimals](/docs/python-sdk/blockchain-apis/decimals)
+                         method in order to get the amount of decimals.
+        :type decimals: int
+        :example decimals: 18
+        :return: The given amount in a decimal form.
+        
+        Example response:
+        ```json
+        2.5
+        ```
+        :rtype: str
+        """
+        str_amount = str(amount)
+
+        # special case when decimals is 0
+        if decimals == 0:
+            return str_amount
+
+        # Check if the string length is less than the decimals
+        if len(str_amount) <= decimals:
+            # Add leading zeros to the string
+            str_amount = '0' * (decimals - len(str_amount) + 1) + str_amount
+            
+        # Insert the decimal point at the correct position
+        str_amount = str_amount[:-decimals] + "." + str_amount[-decimals:]
+        
+        str_amount = str_amount.rstrip('0').rstrip('.') if '.' in str_amount else str_amount
+        return str_amount
+
+    def get_token_unsigned_form(self, amount: str, decimals: int) -> int:
+        """Convert a token from his decimal form back to his unsigned integer form (this
+        method does the reverse of get_token_decimal_form)
+        
+        This method should be used when you receive an amount from a user, in order to convert his
+        input.
+
+        For the highest precision, the implementation only uses str
+
+        :param amount: The amount in str format that you want to convert
+        :type amount: str
+        :example amount: 2.5
+        :param decimals: The amount of decimals that the token has. You can use the [decimals](/docs/python-sdk/blockchain-apis/decimals)
+                         method in order to get the amount of decimals.
+        :type decimals: int
+        :example decimals: 18
+        :return: The amount converted to unsigned integer
+        
+        Example response:
+        ```json
+        2500000000000000000
+        ```
+        :rtype: int
+        """
+        split = amount.split('.')
+        if len(split) >= 2:
+            integer_part, fractional_part = split
+        else:
+            integer_part, fractional_part = split[0], ""
+
+        # Check if the fractional part has less digits than the decimal places
+        if len(fractional_part) < decimals:
+            # Append zeros to the end of the fractional part
+            fractional_part += '0' * (decimals - len(fractional_part))
+        else:
+            # Trim the fractional part to the number of decimal places
+            fractional_part = fractional_part[:decimals]
+
+        # Combine the integer and fractional parts and convert to an integer
+        integer_token_amount = int(integer_part + fractional_part)
+
+        return integer_token_amount
```

### Comparing `blockchain-apis-0.1.4/src/blockchainapis/__init__.py` & `blockchain-apis-0.2.0/src/blockchainapis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,13 +9,13 @@
 you can use the BlockchainAPIsSync class.
 
 """
 
 # Clarensia: https://www.clarensia.com is the company behind
 # the development of https://www.blockchainapis.io
 __author__ = "Clarensia"
-__version__ = "0.1.4"
+__version__ = "0.2.0"
 
 from .BlockchainAPIs import BlockchainAPIs
 from .BlockchainAPIsSync import BlockchainAPIsSync
 
 __all__ = ['BlockchainAPIs']
```

### Comparing `blockchain-apis-0.1.4/src/blockchainapis/exceptions/BlockchainNotSupportedException.py` & `blockchain-apis-0.2.0/src/blockchainapis/exceptions/BlockchainNotSupportedException.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 class BlockchainNotSupportedException(BlockchainAPIsException):
     """
     Thrown when an Invalid blockchain id is put during a call to the API.
     
     To get the list of valid blockchain ids, call `/blockchains`
     """
 
-    status_code: str
+    status_code: int
     """The error code returned by the call to the API
     
     For example: 422
     """
 
     detail: str
     """Some details about the error that occured
     
     For example:
     Blockchain with id "test" is not supported. You can find a list of valid blockchain ids in /blockchains
     """
 
-    def __init__(self, error_code: int, detail: str):
-        super().__init__(error_code, detail)    
+    def __init__(self, status_code: int, detail: str):
+        super().__init__(status_code, detail)
```

### Comparing `blockchain-apis-0.1.4/src/blockchainapis/exceptions/ExchangeNotSupportedException.py` & `blockchain-apis-0.2.0/src/blockchainapis/exceptions/ExchangeNotSupportedException.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 class ExchangeNotSupportedException(BlockchainAPIsException):
     """
     Thrown when an Invalid exchange id is given during a call to the API.
     
     To get the list of supported exchange ids, call `/exchanges`
     """
 
-    status_code: str
+    status_code: int
     """The error code returned by the call to the API
     
     For example: 422
     """
 
     detail: str
     """Some details about the error that occured
     
     For example:
     Exchange with id "test" is not supported. You can get the list of valid exchange ids in /exchanges
     """
 
-    def __init__(self, error_code: int, detail: str):
-        super().__init__(error_code, detail)    
+    def __init__(self, status_code: int, detail: str):
+        super().__init__(status_code, detail)
```

### Comparing `blockchain-apis-0.1.4/src/blockchainapis/exceptions/InvalidPageException.py` & `blockchain-apis-0.2.0/src/blockchainapis/exceptions/InvalidPageException.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,22 +9,22 @@
     * A number lower or equal to 0
     * A page way too high
     
     You should start with 1 as page, and then the response object will give you
     the amount of pages available.
     """
 
-    status_code: str
+    status_code: int
     """The error code returned by the call to the API
     
     For example: 400
     """
 
     detail: str
     """Some details about the error that occured
     
     For example:
     -2 is not a valid page number.
     """
 
-    def __init__(self, error_code: int, detail: str):
-        super().__init__(error_code, detail)    
+    def __init__(self, status_code: int, detail: str):
+        super().__init__(status_code, detail)
```

### Comparing `blockchain-apis-0.1.4/src/blockchainapis/exceptions/PairNotFoundException.py` & `blockchain-apis-0.2.0/src/blockchainapis/exceptions/UnauthorizedException.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from . import BlockchainAPIsException
 
-class PairNotFoundException(BlockchainAPIsException):
+class UnauthorizedException(BlockchainAPIsException):
     """
-    Thrown when you try to get some data about a pair that does not exist.
+    Thrown when you are trying to make an API request with an invalid or expired
+    API key.
     
-    To avoid getting this error, you can get the list of available pairs for
-    the blockchain and exchange that you are interested in by calling `/exchanges/pairs`
+    To prevent this exception, you can:
+    - Make the request without an API key
+    - Update/get a valid API key at: https://dashboard.blockchainapis.io/
     """
 
-    status_code: str
+    status_code: int
     """The error code returned by the call to the API
     
-    For example: 422
+    For example: 401
     """
 
     detail: str
     """Some details about the error that occured
     
     For example:
-    Pair 0x8E870D67F660D95d5be530380D0eC0bd388289E1->0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2 not found in blockchain Arbitrum
+    Unauthorized
     """
 
-    def __init__(self, error_code: int, detail: str):
-        super().__init__(error_code, detail)    
+    def __init__(self, status_code: int, detail: str):
+        super().__init__(status_code, detail)
```

### Comparing `blockchain-apis-0.1.4/src/blockchainapis/exceptions/TokenNotFoundException.py` & `blockchain-apis-0.2.0/src/blockchainapis/exceptions/TokenNotFoundException.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,22 @@
     Thrown when you try to get informations on a token that does not exist inside of our database.
     
     At BlockchainAPIs, we only handle tokens that are inside of a liquidity pool.
     
     You can get a list of all of the available tokens by calling `/tokens`
     """
 
-    status_code: str
+    status_code: int
     """The error code returned by the call to the API
     
     For example: 404
     """
 
     detail: str
     """Some details about the error that occured
     
     For example:
     Token 0x8E870D67F660D95d5be530380D0eC0bd388289E1 not found for blockchain ethereum
     """
 
-    def __init__(self, error_code: int, detail: str):
-        super().__init__(error_code, detail)    
+    def __init__(self, status_code: int, detail: str):
+        super().__init__(status_code, detail)
```

### Comparing `blockchain-apis-0.1.4/src/blockchainapis/exceptions/UnauthorizedException.py` & `blockchain-apis-0.2.0/src/blockchainapis/exceptions/TooManyRequestsException.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from . import BlockchainAPIsException
 
-class UnauthorizedException(BlockchainAPIsException):
+class TooManyRequestsException(BlockchainAPIsException):
     """
-    Thrown when you are trying to make an API request with an invalid or expired
-    API key.
+    Thrown when you are doing more request than you are allowed to the API.
     
-    To prevent this exception, you can:
-    - Make the request without an API key
-    - Update/get a valid API key at: https://dashboard.blockchainapis.io/
+    To prevent this exception you can:
+    - Lower the amount of requests that you make to the API per second
+    - Upgrade your subscription at: https://dashboard.blockchainapis.io/
     """
 
-    status_code: str
+    status_code: int
     """The error code returned by the call to the API
     
-    For example: 401
+    For example: 429
     """
 
     detail: str
     """Some details about the error that occured
     
     For example:
-    Unauthorized
+    Too many requests
     """
 
-    def __init__(self, error_code: int, detail: str):
-        super().__init__(error_code, detail)    
+    def __init__(self, status_code: int, detail: str):
+        super().__init__(status_code, detail)
```

### Comparing `blockchain-apis-0.1.4/src/blockchainapis/exceptions/__init__.py` & `blockchain-apis-0.2.0/src/blockchainapis/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/src/blockchainapis/models/AmountIn.py` & `blockchain-apis-0.2.0/src/blockchainapis/models/AmountIn.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/src/blockchainapis/models/AmountOut.py` & `blockchain-apis-0.2.0/src/blockchainapis/models/AmountOut.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/src/blockchainapis/models/Blockchain.py` & `blockchain-apis-0.2.0/src/blockchainapis/models/Blockchain.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/src/blockchainapis/models/Exchange.py` & `blockchain-apis-0.2.0/src/blockchainapis/models/Exchange.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/src/blockchainapis/models/Exchanges.py` & `blockchain-apis-0.2.0/src/blockchainapis/models/Exchanges.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/src/blockchainapis/models/Pair.py` & `blockchain-apis-0.2.0/src/blockchainapis/models/Pair.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/src/blockchainapis/models/Pairs.py` & `blockchain-apis-0.2.0/src/blockchainapis/models/Pairs.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/src/blockchainapis/models/Reserve.py` & `blockchain-apis-0.2.0/src/blockchainapis/models/Reserve.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/src/blockchainapis/models/Token.py` & `blockchain-apis-0.2.0/src/blockchainapis/models/Token.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/src/blockchainapis/models/Tokens.py` & `blockchain-apis-0.2.0/src/blockchainapis/models/Tokens.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/src/blockchainapis/models/__init__.py` & `blockchain-apis-0.2.0/src/blockchainapis/models/__init__.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/tests/test_amount_in.py` & `blockchain-apis-0.2.0/tests/test_amount_in.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/tests/test_amount_in_sync.py` & `blockchain-apis-0.2.0/tests/test_amount_in_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/tests/test_amount_out.py` & `blockchain-apis-0.2.0/tests/test_amount_out.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/tests/test_amount_out_sync.py` & `blockchain-apis-0.2.0/tests/test_amount_out_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/tests/test_decimals.py` & `blockchain-apis-0.2.0/tests/test_decimals.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/tests/test_decimals_sync.py` & `blockchain-apis-0.2.0/tests/test_decimals_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/tests/test_exchanges.py` & `blockchain-apis-0.2.0/tests/test_exchanges.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/tests/test_exchanges_sync.py` & `blockchain-apis-0.2.0/tests/test_exchanges_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/tests/test_info.py` & `blockchain-apis-0.2.0/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/tests/test_info_sync.py` & `blockchain-apis-0.2.0/tests/test_info_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/tests/test_pairs.py` & `blockchain-apis-0.2.0/tests/test_pairs.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/tests/test_pairs_sync.py` & `blockchain-apis-0.2.0/tests/test_pairs_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/tests/test_reserves.py` & `blockchain-apis-0.2.0/tests/test_reserves.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/tests/test_reserves_sync.py` & `blockchain-apis-0.2.0/tests/test_reserves_sync.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/tests/test_tokens.py` & `blockchain-apis-0.2.0/tests/test_tokens.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.1.4/tests/test_tokens_sync.py` & `blockchain-apis-0.2.0/tests/test_tokens_sync.py`

 * *Files identical despite different names*

