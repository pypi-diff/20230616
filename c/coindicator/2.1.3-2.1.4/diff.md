# Comparing `tmp/coindicator-2.1.3.tar.gz` & `tmp/coindicator-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coindicator-2.1.3.tar", last modified: Fri Jun 16 12:59:21 2023, max compression
+gzip compressed data, was "coindicator-2.1.4.tar", last modified: Fri Jun 16 13:05:14 2023, max compression
```

## Comparing `coindicator-2.1.3.tar` & `coindicator-2.1.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-16 12:59:21.973537 coindicator-2.1.3/
--rw-rw-r--   0 sander    (1000) sander    (1000)       83 2023-06-15 15:11:59.000000 coindicator-2.1.3/.gitignore
--rw-rw-r--   0 sander    (1000) sander    (1000)      899 2022-10-30 19:56:43.000000 coindicator-2.1.3/.pre-commit-config.yaml
--rw-r--r--   0 sander    (1000) sander    (1000)     1106 2020-04-16 00:57:46.000000 coindicator-2.1.3/LICENSE
--rw-rw-r--   0 sander    (1000) sander    (1000)       29 2023-06-16 11:46:09.000000 coindicator-2.1.3/MANIFEST.in
--rw-rw-r--   0 sander    (1000) sander    (1000)     4724 2023-06-16 12:59:21.973537 coindicator-2.1.3/PKG-INFO
--rw-rw-r--   0 sander    (1000) sander    (1000)     4213 2023-06-15 14:54:17.000000 coindicator-2.1.3/README.md
--rw-rw-r--   0 sander    (1000) sander    (1000)      369 2023-06-15 14:05:04.000000 coindicator-2.1.3/coindicator.desktop
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-16 12:59:21.953538 coindicator-2.1.3/img/
--rw-rw-r--   0 sander    (1000) sander    (1000)    27147 2022-10-30 19:56:43.000000 coindicator-2.1.3/img/gitcoin.png
--rw-rw-r--   0 sander    (1000) sander    (1000)   172307 2022-10-30 19:56:43.000000 coindicator-2.1.3/img/screenshot.png
--rwxrwxr-x   0 sander    (1000) sander    (1000)     1678 2023-06-16 12:21:52.000000 coindicator-2.1.3/install.sh
--rw-rw-r--   0 sander    (1000) sander    (1000)      293 2023-06-16 12:58:01.000000 coindicator-2.1.3/pyproject.toml
--rw-rw-r--   0 sander    (1000) sander    (1000)      794 2023-06-15 13:51:42.000000 coindicator-2.1.3/requirements.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)     1202 2023-06-16 12:59:21.973537 coindicator-2.1.3/setup.cfg
--rw-rw-r--   0 sander    (1000) sander    (1000)      521 2023-06-16 12:59:10.000000 coindicator-2.1.3/setup.py
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-16 12:59:21.949538 coindicator-2.1.3/src/
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-16 12:59:21.961537 coindicator-2.1.3/src/coin/
--rw-rw-r--   0 sander    (1000) sander    (1000)        0 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/__init__.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1537 2022-11-16 17:06:14.000000 coindicator-2.1.3/src/coin/about.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     6537 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/alarm.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     5794 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/asset_selection.py
--rwxrwxr-x   0 sander    (1000) sander    (1000)    12627 2023-06-16 12:18:23.000000 coindicator-2.1.3/src/coin/coin.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1751 2023-06-16 12:18:11.000000 coindicator-2.1.3/src/coin/coingecko_client.py
--rw-rw-r--   0 sander    (1000) sander    (1000)      609 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/config.py
--rw-rw-r--   0 sander    (1000) sander    (1000)      977 2022-11-16 17:07:14.000000 coindicator-2.1.3/src/coin/config.yaml
--rw-rw-r--   0 sander    (1000) sander    (1000)     1422 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/downloader.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1177 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/error.py
--rw-rw-r--   0 sander    (1000) sander    (1000)    10512 2023-06-16 12:11:35.000000 coindicator-2.1.3/src/coin/exchange.py
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-16 12:59:21.965537 coindicator-2.1.3/src/coin/exchanges/
--rw-rw-r--   0 sander    (1000) sander    (1000)     1771 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/exchanges/binance.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1579 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/exchanges/bitfinex.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1834 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/exchanges/bitkub.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1493 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/exchanges/bitstamp.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     2031 2022-11-16 17:02:06.000000 coindicator-2.1.3/src/coin/exchanges/bittrex.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1473 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/exchanges/cexio.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1499 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/exchanges/gemini.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1718 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/exchanges/hitbtc.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     2083 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/exchanges/kraken.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1273 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/exchanges/okcoin.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1547 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/exchanges/poloniex.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1281 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/exchanges/unocoin.py
--rw-rw-r--   0 sander    (1000) sander    (1000)    10370 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/indicator.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     2608 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/plugin_selection.py
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-16 12:59:21.969537 coindicator-2.1.3/src/coin/resources/
--rw-rw-r--   0 sander    (1000) sander    (1000)   294232 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/resources/ca-ching.wav
--rw-rw-r--   0 sander    (1000) sander    (1000)     5060 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/resources/icon.png
--rw-rw-r--   0 sander    (1000) sander    (1000)      983 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/resources/icon_32px.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     1440 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/resources/icon_48px.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     1673 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/resources/icon_64px.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     1889 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/resources/loading.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     4619 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/resources/logo_124px.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     7329 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/resources/logo_124pxs.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     6508 2022-10-30 19:56:43.000000 coindicator-2.1.3/src/coin/resources/logo_248px.png
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-16 12:59:21.973537 coindicator-2.1.3/src/coindicator.egg-info/
--rw-rw-r--   0 sander    (1000) sander    (1000)     4724 2023-06-16 12:59:21.000000 coindicator-2.1.3/src/coindicator.egg-info/PKG-INFO
--rw-rw-r--   0 sander    (1000) sander    (1000)     1388 2023-06-16 12:59:21.000000 coindicator-2.1.3/src/coindicator.egg-info/SOURCES.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-16 12:59:21.000000 coindicator-2.1.3/src/coindicator.egg-info/dependency_links.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)       47 2023-06-16 12:59:21.000000 coindicator-2.1.3/src/coindicator.egg-info/entry_points.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-16 11:50:35.000000 coindicator-2.1.3/src/coindicator.egg-info/not-zip-safe
--rw-rw-r--   0 sander    (1000) sander    (1000)      227 2023-06-16 12:59:21.000000 coindicator-2.1.3/src/coindicator.egg-info/requires.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)        5 2023-06-16 12:59:21.000000 coindicator-2.1.3/src/coindicator.egg-info/top_level.txt
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-16 13:05:14.569623 coindicator-2.1.4/
+-rw-rw-r--   0 sander    (1000) sander    (1000)       83 2023-06-16 13:04:41.000000 coindicator-2.1.4/.gitignore
+-rw-rw-r--   0 sander    (1000) sander    (1000)      899 2022-10-30 19:56:43.000000 coindicator-2.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 sander    (1000) sander    (1000)     1106 2020-04-16 00:57:46.000000 coindicator-2.1.4/LICENSE
+-rw-rw-r--   0 sander    (1000) sander    (1000)       29 2023-06-16 13:04:41.000000 coindicator-2.1.4/MANIFEST.in
+-rw-rw-r--   0 sander    (1000) sander    (1000)     4724 2023-06-16 13:05:14.569623 coindicator-2.1.4/PKG-INFO
+-rw-rw-r--   0 sander    (1000) sander    (1000)     4213 2023-06-16 13:04:41.000000 coindicator-2.1.4/README.md
+-rw-rw-r--   0 sander    (1000) sander    (1000)      369 2023-06-16 13:04:41.000000 coindicator-2.1.4/coindicator.desktop
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-16 13:05:14.553623 coindicator-2.1.4/img/
+-rw-rw-r--   0 sander    (1000) sander    (1000)    27147 2022-10-30 19:56:43.000000 coindicator-2.1.4/img/gitcoin.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)   172307 2022-10-30 19:56:43.000000 coindicator-2.1.4/img/screenshot.png
+-rwxrwxr-x   0 sander    (1000) sander    (1000)     1624 2023-06-16 13:04:41.000000 coindicator-2.1.4/install.sh
+-rw-rw-r--   0 sander    (1000) sander    (1000)      294 2023-06-16 13:04:41.000000 coindicator-2.1.4/pyproject.toml
+-rw-rw-r--   0 sander    (1000) sander    (1000)      794 2023-06-16 13:04:41.000000 coindicator-2.1.4/requirements.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1202 2023-06-16 13:05:14.569623 coindicator-2.1.4/setup.cfg
+-rw-rw-r--   0 sander    (1000) sander    (1000)      521 2023-06-16 13:04:41.000000 coindicator-2.1.4/setup.py
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-16 13:05:14.549622 coindicator-2.1.4/src/
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-16 13:05:14.557623 coindicator-2.1.4/src/coin/
+-rw-rw-r--   0 sander    (1000) sander    (1000)        0 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/__init__.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1537 2022-11-16 17:06:14.000000 coindicator-2.1.4/src/coin/about.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     6537 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/alarm.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     5794 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/asset_selection.py
+-rwxrwxr-x   0 sander    (1000) sander    (1000)    12627 2023-06-16 13:04:41.000000 coindicator-2.1.4/src/coin/coin.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1751 2023-06-16 13:04:41.000000 coindicator-2.1.4/src/coin/coingecko_client.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)      609 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/config.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)      977 2022-11-16 17:07:14.000000 coindicator-2.1.4/src/coin/config.yaml
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1422 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/downloader.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1177 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/error.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)    10512 2023-06-16 12:11:35.000000 coindicator-2.1.4/src/coin/exchange.py
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-16 13:05:14.561623 coindicator-2.1.4/src/coin/exchanges/
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1771 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/exchanges/binance.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1579 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/exchanges/bitfinex.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1834 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/exchanges/bitkub.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1493 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/exchanges/bitstamp.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2031 2022-11-16 17:02:06.000000 coindicator-2.1.4/src/coin/exchanges/bittrex.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1473 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/exchanges/cexio.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1499 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/exchanges/gemini.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1718 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/exchanges/hitbtc.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2083 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/exchanges/kraken.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1273 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/exchanges/okcoin.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1547 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/exchanges/poloniex.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1281 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/exchanges/unocoin.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)    10370 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/indicator.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2608 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/plugin_selection.py
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-16 13:05:14.565623 coindicator-2.1.4/src/coin/resources/
+-rw-rw-r--   0 sander    (1000) sander    (1000)   294232 2023-06-16 13:04:41.000000 coindicator-2.1.4/src/coin/resources/ca-ching.wav
+-rw-rw-r--   0 sander    (1000) sander    (1000)     5060 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/resources/icon.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)      983 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/resources/icon_32px.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1440 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/resources/icon_48px.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1673 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/resources/icon_64px.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1889 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/resources/loading.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     4619 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/resources/logo_124px.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     7329 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/resources/logo_124pxs.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     6508 2022-10-30 19:56:43.000000 coindicator-2.1.4/src/coin/resources/logo_248px.png
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-16 13:05:14.569623 coindicator-2.1.4/src/coindicator.egg-info/
+-rw-rw-r--   0 sander    (1000) sander    (1000)     4724 2023-06-16 13:05:14.000000 coindicator-2.1.4/src/coindicator.egg-info/PKG-INFO
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1388 2023-06-16 13:05:14.000000 coindicator-2.1.4/src/coindicator.egg-info/SOURCES.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-16 13:05:14.000000 coindicator-2.1.4/src/coindicator.egg-info/dependency_links.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)       47 2023-06-16 13:05:14.000000 coindicator-2.1.4/src/coindicator.egg-info/entry_points.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-16 11:50:35.000000 coindicator-2.1.4/src/coindicator.egg-info/not-zip-safe
+-rw-rw-r--   0 sander    (1000) sander    (1000)      227 2023-06-16 13:05:14.000000 coindicator-2.1.4/src/coindicator.egg-info/requires.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)        5 2023-06-16 13:05:14.000000 coindicator-2.1.4/src/coindicator.egg-info/top_level.txt
```

### Comparing `coindicator-2.1.3/.pre-commit-config.yaml` & `coindicator-2.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/LICENSE` & `coindicator-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/PKG-INFO` & `coindicator-2.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coindicator
-Version: 2.1.3
+Version: 2.1.4
 Summary: Coinprice Indicator
 Home-page: https://github.com/bluppfisk/coindicator/
 Author: Sander Van de Moortel
 Author-email: sander.vandemoortel@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/bluppfisk/coindicator/
 Platform: Linux
```

### Comparing `coindicator-2.1.3/README.md` & `coindicator-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/img/gitcoin.png` & `coindicator-2.1.4/img/gitcoin.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/img/screenshot.png` & `coindicator-2.1.4/img/screenshot.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/install.sh` & `coindicator-2.1.4/install.sh`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,15 @@
 # sudo apt update
 # sudo apt install cmake
 
 # Install python packages
 sudo mkdir ${args[0]} 2>/dev/null
 sudo python3 -m venv ${args[0]}/venv
 source ${args[0]}/venv/bin/activate
-sudo -E env PATH=$PATH pip3 install wheel setuptools_scm
-sudo -E env PATH=$PATH pip3 install --no-cache-dir --use-deprecated=legacy-resolver -U coindicator
+sudo -H -E env PATH=$PATH pip3 install --no-cache-dir --use-deprecated=legacy-resolver -U coindicator
 
 # Install shortcut
 cat > /tmp/coindicator.desktop << EOL
 
 [Desktop Entry]
 Name=Coindicator
 GenericName=Cryptocoin price ticker
```

### Comparing `coindicator-2.1.3/requirements.txt` & `coindicator-2.1.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/setup.cfg` & `coindicator-2.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/setup.py` & `coindicator-2.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/about.py` & `coindicator-2.1.4/src/coin/about.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/alarm.py` & `coindicator-2.1.4/src/coin/alarm.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/asset_selection.py` & `coindicator-2.1.4/src/coin/asset_selection.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/coin.py` & `coindicator-2.1.4/src/coin/coin.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/coingecko_client.py` & `coindicator-2.1.4/src/coin/coingecko_client.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/config.py` & `coindicator-2.1.4/src/coin/config.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/config.yaml` & `coindicator-2.1.4/src/coin/config.yaml`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/downloader.py` & `coindicator-2.1.4/src/coin/downloader.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/error.py` & `coindicator-2.1.4/src/coin/error.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/exchange.py` & `coindicator-2.1.4/src/coin/exchange.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/exchanges/binance.py` & `coindicator-2.1.4/src/coin/exchanges/binance.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/exchanges/bitfinex.py` & `coindicator-2.1.4/src/coin/exchanges/bitfinex.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/exchanges/bitkub.py` & `coindicator-2.1.4/src/coin/exchanges/bitkub.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/exchanges/bitstamp.py` & `coindicator-2.1.4/src/coin/exchanges/bitstamp.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/exchanges/bittrex.py` & `coindicator-2.1.4/src/coin/exchanges/bittrex.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/exchanges/cexio.py` & `coindicator-2.1.4/src/coin/exchanges/cexio.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/exchanges/gemini.py` & `coindicator-2.1.4/src/coin/exchanges/gemini.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/exchanges/hitbtc.py` & `coindicator-2.1.4/src/coin/exchanges/hitbtc.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/exchanges/kraken.py` & `coindicator-2.1.4/src/coin/exchanges/kraken.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/exchanges/okcoin.py` & `coindicator-2.1.4/src/coin/exchanges/okcoin.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/exchanges/poloniex.py` & `coindicator-2.1.4/src/coin/exchanges/poloniex.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/exchanges/unocoin.py` & `coindicator-2.1.4/src/coin/exchanges/unocoin.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/indicator.py` & `coindicator-2.1.4/src/coin/indicator.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/plugin_selection.py` & `coindicator-2.1.4/src/coin/plugin_selection.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/resources/ca-ching.wav` & `coindicator-2.1.4/src/coin/resources/ca-ching.wav`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/resources/icon.png` & `coindicator-2.1.4/src/coin/resources/icon.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/resources/icon_32px.png` & `coindicator-2.1.4/src/coin/resources/icon_32px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/resources/icon_48px.png` & `coindicator-2.1.4/src/coin/resources/icon_48px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/resources/icon_64px.png` & `coindicator-2.1.4/src/coin/resources/icon_64px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/resources/loading.png` & `coindicator-2.1.4/src/coin/resources/loading.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/resources/logo_124px.png` & `coindicator-2.1.4/src/coin/resources/logo_124px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/resources/logo_124pxs.png` & `coindicator-2.1.4/src/coin/resources/logo_124pxs.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coin/resources/logo_248px.png` & `coindicator-2.1.4/src/coin/resources/logo_248px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.3/src/coindicator.egg-info/PKG-INFO` & `coindicator-2.1.4/src/coindicator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coindicator
-Version: 2.1.3
+Version: 2.1.4
 Summary: Coinprice Indicator
 Home-page: https://github.com/bluppfisk/coindicator/
 Author: Sander Van de Moortel
 Author-email: sander.vandemoortel@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/bluppfisk/coindicator/
 Platform: Linux
```

### Comparing `coindicator-2.1.3/src/coindicator.egg-info/SOURCES.txt` & `coindicator-2.1.4/src/coindicator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

