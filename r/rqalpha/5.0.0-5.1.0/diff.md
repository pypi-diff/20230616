# Comparing `tmp/rqalpha-5.0.0.tar.gz` & `tmp/rqalpha-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/rqalpha/rqalpha/dist/.tmp-74wqqrpp/rqalpha-5.0.0.tar", last modified: Fri Jun  2 01:50:19 2023, max compression
+gzip compressed data, was "/home/runner/work/rqalpha/rqalpha/dist/.tmp-vb2rqxte/rqalpha-5.1.0.tar", last modified: Fri Jun 16 08:08:38 2023, max compression
```

## Comparing `rqalpha-5.0.0.tar` & `rqalpha-5.1.0.tar`

### file list

```diff
@@ -1,243 +1,243 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    61035 2023-06-02 01:50:10.000000 rqalpha-5.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-02 01:50:10.000000 rqalpha-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-02 01:50:10.000000 rqalpha-5.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-02 01:50:19.000000 rqalpha-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-06-02 01:50:10.000000 rqalpha-5.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/apis/
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24556 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/apis/api_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    35283 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/apis/api_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    52911 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/apis/api_rqdatac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/apis/names.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/cmds/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/cmds/bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/cmds/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/cmds/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/cmds/mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/cmds/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/core/execution_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/core/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/core/global_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/core/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/core/strategy_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/core/strategy_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/core/strategy_universe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/data/bar_dict_price_board.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/data/base_data_source/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/data/base_data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/data/base_data_source/adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/data/base_data_source/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/data/base_data_source/storage_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/data/base_data_source/storages.py
--rw-r--r--   0 runner    (1001) docker     (123)    17445 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/data/bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/data/data_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/data/trading_dates_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    22343 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/IF1706_20161108.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/IF_macd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/buy_and_hold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/examples/data_source/
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/data_source/get_csv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/data_source/import_get_csv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/data_source/read_csv_as_df.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/examples/extend_api/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/extend_api/test_extend_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/golden_cross.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/macd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/pair_trading.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/rsi.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/run_code_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/run_file_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/run_func_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/subscribe_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/test_pt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/examples/turtle.py
--rw-r--r--   0 runner    (1001) docker     (123)    21124 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    12580 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py
--rw-r--r--   0 runner    (1001) docker     (123)    34524 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/component_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py
--rw-r--r--   0 runner    (1001) docker     (123)    20020 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24306 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    15036 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/summary.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_progress/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_progress/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/mod.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py
--rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29229 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/mod_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/model/bar.py
--rw-r--r--   0 runner    (1001) docker     (123)    24670 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/model/instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)    13053 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/model/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/model/tick.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/model/trade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/portfolio/
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/portfolio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20437 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/portfolio/account.py
--rw-r--r--   0 runner    (1001) docker     (123)    14772 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/portfolio/position.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/resource/
--rw-r--r--   0 runner    (1001) docker     (123)    32799 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/resource/ricequant-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/user_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18080 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/arg_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/class_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/click_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/datetime_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/dict_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/log_capture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/package_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/persisit_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/repr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/risk_free_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/rq_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/strategy_loader_help.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/testing/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/testing/mocking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/utils/translations/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/translations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/utils/translations/zh_Hans_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    51160 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/translations/zh_Hans_CN/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-02 01:50:10.000000 rqalpha-5.0.0/rqalpha/utils/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 01:50:19.000000 rqalpha-5.0.0/rqalpha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-02 01:50:19.000000 rqalpha-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-02 01:50:10.000000 rqalpha-5.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/tests/api_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/tests/api_tests/mod/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_accounts/test_account_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_accounts/test_futures_settlement_price_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_accounts/test_margin_stocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_accounts/test_position_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_scheduler/test_physical_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_scheduler/test_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_simulation/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_simulation/test_management_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_simulation/test_signal_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_simulation/test_simulation_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_transaction_cost/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_transaction_cost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/mod/sys_transaction_cost/test_commission_multiplier.py
--rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/test_api_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/test_api_future.py
--rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/test_api_stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/api_tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/test_f_buy_and_hold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/test_f_macd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/test_f_macd_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/test_f_mean_reverting.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/test_s_buy_and_hold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/test_s_dual_thrust.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/test_s_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/test_s_tick_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/test_s_turtle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/test_s_turtle_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/test_sf_buy_and_hold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/tests/unittest/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/unittest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/tests/unittest/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/unittest/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/unittest/test_data/test_instrument_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/unittest/test_data/test_trading_dates_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/tests/unittest/test_mod/
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/unittest/test_mod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:50:19.000000 rqalpha-5.0.0/tests/unittest/test_mod/test_sys_simulation/
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/unittest/test_mod/test_sys_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-02 01:50:10.000000 rqalpha-5.0.0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    79879 2023-06-02 01:50:10.000000 rqalpha-5.0.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    61279 2023-06-16 08:08:28.000000 rqalpha-5.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-16 08:08:28.000000 rqalpha-5.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-16 08:08:28.000000 rqalpha-5.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-16 08:08:38.000000 rqalpha-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-06-16 08:08:28.000000 rqalpha-5.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24556 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/apis/api_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35283 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/apis/api_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59090 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/apis/api_rqdatac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/apis/names.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/cmds/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/cmds/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/cmds/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/cmds/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/cmds/mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/cmds/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/core/execution_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/core/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/core/global_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/core/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/core/strategy_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/core/strategy_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/core/strategy_universe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/data/bar_dict_price_board.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/data/base_data_source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/data/base_data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/data/base_data_source/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/data/base_data_source/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/data/base_data_source/storage_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/data/base_data_source/storages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17445 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/data/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/data/data_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/data/trading_dates_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    22343 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/IF1706_20161108.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/IF_macd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/buy_and_hold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/examples/data_source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/data_source/get_csv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/data_source/import_get_csv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/data_source/read_csv_as_df.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/examples/extend_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/extend_api/test_extend_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/golden_cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/macd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/pair_trading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/rsi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/run_code_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/run_file_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/run_func_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/subscribe_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/test_pt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/examples/turtle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21124 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12580 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34687 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/component_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20020 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25635 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    22158 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/templates/summary.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_progress/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_progress/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/mod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29229 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/mod_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/model/bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24670 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/model/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13053 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/model/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/model/tick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/model/trade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/portfolio/
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/portfolio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20437 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/portfolio/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/portfolio/position.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)    32799 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/resource/ricequant-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/user_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18080 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/arg_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/class_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/click_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10415 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/datetime_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/dict_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/log_capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/package_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/persisit_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/risk_free_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/rq_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/strategy_loader_help.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/testing/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/testing/mocking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/utils/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/translations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/utils/translations/zh_Hans_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    51160 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/translations/zh_Hans_CN/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-16 08:08:28.000000 rqalpha-5.1.0/rqalpha/utils/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 08:08:38.000000 rqalpha-5.1.0/rqalpha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-16 08:08:38.000000 rqalpha-5.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-16 08:08:28.000000 rqalpha-5.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/tests/api_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/tests/api_tests/mod/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_accounts/test_account_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_accounts/test_futures_settlement_price_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_accounts/test_margin_stocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_accounts/test_position_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_scheduler/test_physical_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_scheduler/test_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_simulation/test_management_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_simulation/test_signal_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_simulation/test_simulation_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_transaction_cost/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_transaction_cost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/mod/sys_transaction_cost/test_commission_multiplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/test_api_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/test_api_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/test_api_stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/api_tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/test_f_buy_and_hold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/test_f_macd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/test_f_macd_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/test_f_mean_reverting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/test_s_buy_and_hold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/test_s_dual_thrust.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/test_s_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/test_s_tick_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/test_s_turtle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/test_s_turtle_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/test_sf_buy_and_hold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/tests/unittest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/unittest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/tests/unittest/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/unittest/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/unittest/test_data/test_instrument_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/unittest/test_data/test_trading_dates_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/tests/unittest/test_mod/
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/unittest/test_mod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:08:38.000000 rqalpha-5.1.0/tests/unittest/test_mod/test_sys_simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/unittest/test_mod/test_sys_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-16 08:08:28.000000 rqalpha-5.1.0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79879 2023-06-16 08:08:28.000000 rqalpha-5.1.0/versioneer.py
```

### Comparing `rqalpha-5.0.0/CHANGELOG.rst` & `rqalpha-5.1.0/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 ==================
 CHANGELOG
 ==================
 
+5.1.0
+==================
+- 新增个股权重检测, summary报告中新增了表格
+- 新增api futures.get_dominant_price,支持动态复权
+- 修复pandas1.5.0以下无法产生report
+- 修复在日内回转交易时trading_pnl计算错误
+
 5.0.0
 ==================
 - 适配pandas2.0
 - 交易指数标的时，不检查上市日期，根据行情数据有无决定
 - 撮合时屏蔽已完成的订单
 - 修复get_prev_settlement取不到第一天的，采用prev_settlement字段
 - 新增算法单：VWAPOrder 和 TWAPOrder
```

### Comparing `rqalpha-5.0.0/LICENSE` & `rqalpha-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/PKG-INFO` & `rqalpha-5.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rqalpha
-Version: 5.0.0
+Version: 5.1.0
 Summary: Ricequant Algorithm Trading System
 Home-page: https://github.com/ricequant/rqalpha
 Author: ricequant
 Author-email: public@ricequant.com
 License: Apache License v2
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
```

### Comparing `rqalpha-5.0.0/README.rst` & `rqalpha-5.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/__init__.py` & `rqalpha-5.1.0/rqalpha/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/__main__.py` & `rqalpha-5.1.0/rqalpha/__main__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/api.py` & `rqalpha-5.1.0/rqalpha/api.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/apis/__init__.py` & `rqalpha-5.1.0/rqalpha/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/apis/api_abstract.py` & `rqalpha-5.1.0/rqalpha/apis/api_abstract.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/apis/api_base.py` & `rqalpha-5.1.0/rqalpha/apis/api_base.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/apis/api_rqdatac.py` & `rqalpha-5.1.0/rqalpha/apis/api_rqdatac.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #         除非法律有要求或以书面形式达成协议，否则本软件分发时需保持当前许可“原样”不变，且不得附加任何条件。
 #
 #     * 商业用途（商业用途指个人出于任何商业目的使用本软件，或者法人或其他组织出于任何目的使用本软件）：
 #         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 import datetime
+from functools import lru_cache
 from typing import Union, Optional, Iterable, List
 
 import six
 from dateutil.parser import parse
 import pandas as pd
 
 from rqalpha.const import EXECUTION_PHASE
@@ -28,17 +29,20 @@
 from rqalpha.core.execution_context import ExecutionContext
 from rqalpha.environment import Environment
 from rqalpha.utils.arg_checker import apply_rules, verify_that
 from rqalpha.utils.exception import RQInvalidArgument
 from rqalpha.apis.api_base import assure_order_book_id
 from rqalpha.utils.i18n import gettext as _
 from rqalpha.utils.logger import user_log
+from rqalpha.utils import check_items_in_container
 
 try:
     import rqdatac
+    from rqdatac.services.future import _get_future_factors_df
+    _get_all_future_factors_df = lru_cache(1)(_get_future_factors_df)
 except ImportError:
     class DummyRQDatac:
         __name__ = "rqdatac"
 
         def __getattr__(self, item):
             return self
 
@@ -992,14 +996,143 @@
         start_date = end_date
     else:
         start_date = env.data_proxy.get_previous_trading_date(end_date, count - 1)
 
     return rqdatac.futures.get_warehouse_stocks(underlying_symbols, start_date=start_date, end_date=end_date)
 
 
+VALID_ADJUST_TYPES = ['none', 'pre', 'post']
+VALID_ADJUST_METHODS = ['prev_close_spread', 'open_spread', 'prev_close_ratio', 'open_ratio']
+
+
+def _get_ex_factor(underlying_symbols, adjust_type, adjust_method, adjust_date):
+    df = _get_all_future_factors_df().loc[underlying_symbols].reset_index()
+    need_cols = ["underlying_symbol", "ex_date", "ex_factor"]
+    factor = df[df["ex_date"] <= adjust_date].rename(columns={adjust_method: "ex_factor"})[need_cols]
+
+    pre, ratio = adjust_type == 'pre', adjust_method.endswith('ratio')
+
+    def _process(x):
+        if ratio:
+            x['ex_cum_factor'] = x['ex_factor'].cumprod()
+            if pre:
+                x['ex_cum_factor'] = x['ex_cum_factor'] / x['ex_cum_factor'].iloc[-1]
+        else:
+            x['ex_cum_factor'] = x['ex_factor'].cumsum()
+            if pre:
+                x['ex_cum_factor'] = x['ex_cum_factor'] - x['ex_cum_factor'].iloc[-1]
+        return x.set_index('ex_date')
+
+    factor = factor.groupby('underlying_symbol', as_index=True).apply(_process)
+    return factor['ex_cum_factor']
+
+
+DOMINANT_PRICE_ADJUST_FIELDS = [
+    'open', 'high', 'low', 'close', 'last', 'limit_up', 'limit_down', 'settlement', 'prev_settlement', 'prev_close',
+    'a1', 'a2', 'a3', 'a4', 'a5', 'b1', 'b2', 'b3', 'b4', 'b5'
+]
+
+
+def _futures_get_dominant_price(
+        underlying_symbols, start_date=None, end_date=None, frequency="1d", fields=None, adjust_type="pre",
+        adjust_method="prev_close_spread"
+):
+    """ 获取主力合约行情数据
+
+    :param underlying_symbols: 期货合约品种，可传入 underlying_symbol, underlying_symbol list
+    :param start_date: 开始日期, 最小日期为 20100104
+    :param end_date: 结束日期
+    :param frequency: 历史数据的频率。 支持/日/分钟/tick 级别的历史数据，默认为'1d'。
+        1m- 分钟线，1d-日线，分钟可选取不同频率，例如'5m'代表 5 分钟线
+    :param fields: 字段名称列表
+    :param adjust_type: 复权方式，不复权 - none，前复权 - pre，后复权 - post
+    :param adjust_method: 复权方法 ，prev_close_spread/open_spread:基于价差复权因子进行复权，
+        prev_close_ratio/open_ratio:基于比例复权因子进行复权，
+        默认为‘prev_close_spread',adjust_type为None 时，adjust_method 复权方法设置无效
+    :return: MultiIndex DataFrame
+
+    :example:
+
+    获取基于价差前复权计算的主力合约数据（策略当前日期是2015-01-27，则以策略当天为准，而不是已现实最新日期为准来计算复权因子）:
+
+    ..  code-block:: python3
+        :linenos:
+
+        get_dominant_price(underlying_symbols='CU', start_date='2015-01-20', end_date='2015-01-23', adjust_type="pre",
+                           adjust_method="prev_close_spread", fields=["close", "settlement"],)
+        #[Out]
+        #                               close     settlement
+        # underlying_symbol date
+        # CU                2015-01-20  40990.0     41080.0
+        #                   2015-01-21  41000.0     41060.0
+        #                   2015-01-22  41300.0     41340.0
+        #                   2015-01-23  40750.0     40950.0
+        #                   2015-01-26  39250.0     39660.0
+        #                   2015-01-27  40260.0     40210.0
+
+    """
+    env = Environment.get_instance()
+    if not isinstance(underlying_symbols, list):
+        underlying_symbols = [underlying_symbols]
+    if fields and not isinstance(fields, list):
+        fields = [fields]
+    end_date = env.trading_dt if end_date is None else pd.to_datetime(end_date)
+    start_date = end_date - datetime.timedelta(days=3) if start_date is None else pd.to_datetime(start_date)
+    if start_date > end_date:
+        raise RQInvalidArgument('in futures.get_dominant_price, start_date {} > end_date {}'.format(
+            start_date.date(), end_date.date()
+        ))
+    if end_date > pd.to_datetime(env.trading_dt):
+        raise RQInvalidArgument('in futures.get_dominant_price, end_date {} > trading day {}'.format(
+            end_date.date(), env.trading_dt.date()
+        ))
+
+    check_items_in_container([adjust_type], VALID_ADJUST_TYPES, 'adjust_type')
+    check_items_in_container([adjust_method], VALID_ADJUST_METHODS, 'adjust_method')
+
+    _date_key = 'date' if frequency == '1d' else 'trading_date'
+    _fields = fields
+    if fields and frequency != '1d' and 'trading_date' not in fields:
+        _fields = ['trading_date'] + fields
+
+    obs = [u + '88' for u in underlying_symbols]
+    df = rqdatac.get_price(
+        order_book_ids=obs, start_date=start_date, end_date=end_date, frequency=frequency, adjust_type='none',
+        fields=_fields, expect_df=True
+    )
+    if df is None:
+        return
+
+    df.reset_index(inplace=True)
+    df['underlying_symbol'] = df['order_book_id'].str[:-2]
+    df.set_index(['underlying_symbol', _date_key], inplace=True)
+    if adjust_type != 'none':
+        # 复权调整
+        factor = _get_ex_factor(underlying_symbols, adjust_type, adjust_method, pd.to_datetime(env.trading_dt.date()))
+        factor = factor.reindex(factor.index.union(df.index.unique())).groupby(level=0).ffill()
+        values = factor.loc[df.index].values
+        _fields = fields if fields else df.columns.tolist()
+        adjust_fields = [f for f in DOMINANT_PRICE_ADJUST_FIELDS if f in _fields]
+        if adjust_method.endswith('spread'):
+            for field in adjust_fields:
+                df[field] += values
+        elif adjust_method.endswith('ratio'):
+            for field in adjust_fields:
+                df[field] *= values
+        if 'total_turnover' in df.columns:
+            df['total_turnover'] = 0
+
+    if frequency != '1d':
+        df = df.reset_index().set_index(['underlying_symbol', 'datetime'])
+    df.sort_index(inplace=True)
+    del df['order_book_id']
+    return df[fields] if fields else df
+
+
+futures.get_dominant_price = staticmethod(_futures_get_dominant_price)
 futures.get_dominant = staticmethod(_futures_get_dominant)
 futures.get_member_rank = staticmethod(_futures_get_member_rank)
 futures.get_warehouse_stocks = staticmethod(_futures_get_warehouse_stocks)
 
 
 @export_as_api
 @apply_rules(verify_that('entry_date').is_valid_date(ignore_none=True),
```

### Comparing `rqalpha-5.0.0/rqalpha/apis/names.py` & `rqalpha-5.1.0/rqalpha/apis/names.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/cmds/__init__.py` & `rqalpha-5.1.0/rqalpha/cmds/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/cmds/bundle.py` & `rqalpha-5.1.0/rqalpha/cmds/bundle.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/cmds/entry.py` & `rqalpha-5.1.0/rqalpha/cmds/entry.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/cmds/misc.py` & `rqalpha-5.1.0/rqalpha/cmds/misc.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/cmds/mod.py` & `rqalpha-5.1.0/rqalpha/cmds/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/cmds/run.py` & `rqalpha-5.1.0/rqalpha/cmds/run.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/config.yml` & `rqalpha-5.1.0/rqalpha/config.yml`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/const.py` & `rqalpha-5.1.0/rqalpha/const.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/core/__init__.py` & `rqalpha-5.1.0/rqalpha/core/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/core/events.py` & `rqalpha-5.1.0/rqalpha/core/events.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/core/execution_context.py` & `rqalpha-5.1.0/rqalpha/core/execution_context.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/core/executor.py` & `rqalpha-5.1.0/rqalpha/core/executor.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/core/global_var.py` & `rqalpha-5.1.0/rqalpha/core/global_var.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/core/strategy.py` & `rqalpha-5.1.0/rqalpha/core/strategy.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/core/strategy_context.py` & `rqalpha-5.1.0/rqalpha/core/strategy_context.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/core/strategy_loader.py` & `rqalpha-5.1.0/rqalpha/core/strategy_loader.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/core/strategy_universe.py` & `rqalpha-5.1.0/rqalpha/core/strategy_universe.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/data/__init__.py` & `rqalpha-5.1.0/rqalpha/data/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/data/bar_dict_price_board.py` & `rqalpha-5.1.0/rqalpha/data/bar_dict_price_board.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/data/base_data_source/__init__.py` & `rqalpha-5.1.0/rqalpha/data/base_data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/data/base_data_source/adjust.py` & `rqalpha-5.1.0/rqalpha/data/base_data_source/adjust.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/data/base_data_source/data_source.py` & `rqalpha-5.1.0/rqalpha/data/base_data_source/data_source.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/data/base_data_source/storage_interface.py` & `rqalpha-5.1.0/rqalpha/data/base_data_source/storage_interface.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/data/base_data_source/storages.py` & `rqalpha-5.1.0/rqalpha/data/base_data_source/storages.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/data/bundle.py` & `rqalpha-5.1.0/rqalpha/data/bundle.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/data/data_proxy.py` & `rqalpha-5.1.0/rqalpha/data/data_proxy.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/data/trading_dates_mixin.py` & `rqalpha-5.1.0/rqalpha/data/trading_dates_mixin.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/environment.py` & `rqalpha-5.1.0/rqalpha/environment.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/examples/IF1706_20161108.csv` & `rqalpha-5.1.0/rqalpha/examples/IF1706_20161108.csv`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/examples/IF_macd.py` & `rqalpha-5.1.0/rqalpha/examples/IF_macd.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/examples/buy_and_hold.py` & `rqalpha-5.1.0/rqalpha/examples/buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/examples/data_source/get_csv_module.py` & `rqalpha-5.1.0/rqalpha/examples/data_source/get_csv_module.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/examples/data_source/import_get_csv_module.py` & `rqalpha-5.1.0/rqalpha/examples/data_source/import_get_csv_module.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/examples/data_source/read_csv_as_df.py` & `rqalpha-5.1.0/rqalpha/examples/data_source/read_csv_as_df.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py` & `rqalpha-5.1.0/rqalpha/examples/extend_api/rqalpha_mod_extend_api_demo.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/examples/extend_api/test_extend_api.py` & `rqalpha-5.1.0/rqalpha/examples/extend_api/test_extend_api.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/examples/golden_cross.py` & `rqalpha-5.1.0/rqalpha/examples/golden_cross.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/examples/macd.py` & `rqalpha-5.1.0/rqalpha/examples/macd.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/examples/pair_trading.py` & `rqalpha-5.1.0/rqalpha/examples/pair_trading.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/examples/rsi.py` & `rqalpha-5.1.0/rqalpha/examples/rsi.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/examples/run_code_demo.py` & `rqalpha-5.1.0/rqalpha/examples/run_code_demo.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/examples/run_func_demo.py` & `rqalpha-5.1.0/rqalpha/examples/run_func_demo.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/examples/subscribe_event.py` & `rqalpha-5.1.0/rqalpha/examples/subscribe_event.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/examples/test_pt.py` & `rqalpha-5.1.0/rqalpha/examples/test_pt.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/examples/turtle.py` & `rqalpha-5.1.0/rqalpha/examples/turtle.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/interface.py` & `rqalpha-5.1.0/rqalpha/interface.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/main.py` & `rqalpha-5.1.0/rqalpha/main.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/__init__.py` & `rqalpha-5.1.0/rqalpha/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_future.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/api/api_stock.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,16 @@
         raise RQInvalidArgument(_(u"Limit order price should not be nan."))
     price = env.data_proxy.get_last_price(ins.order_book_id)
     if not is_valid_price(price):
         user_system_log.warn(
             _(u"Order Creation Failed: [{order_book_id}] No market data").format(order_book_id=ins.order_book_id))
         return
 
-    if (side == SIDE.BUY) or (side == SIDE.SELL and current_quantity != abs(amount)):
+    if (side == SIDE.BUY and current_quantity != -amount) or (side == SIDE.SELL and current_quantity != abs(amount)):
+        # 在融券回测中，需要用买单作为平空，对于此种情况下出现的碎股，亦允许一次性申报卖出
         amount = _round_order_quantity(ins, amount)
 
     if amount == 0:
         user_system_log.warn(_(
             u"Order Creation Failed: 0 order quantity, order_book_id={order_book_id}"
         ).format(order_book_id=ins.order_book_id))
         return
```

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/component_validator.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/component_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/position_model.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/position_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_accounts/validator.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_accounts/validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/mod.py`

 * *Files 3% similar despite different names*

```diff
@@ -264,14 +264,15 @@
             if position:
                 for field in ['margin', 'contract_multiplier', 'last_price']:
                     data[field] = self._safe_convert(getattr(position, field))
             direction_pos_iter = ((pos.direction, pos) for pos in (long, short) if pos)
             for direction_prefix, pos in direction_pos_iter:
                 data[direction_prefix + "_pnl"] = self._safe_convert(getattr(pos, "pnl", None))
                 data[direction_prefix + "_margin"] = self._safe_convert(pos.margin)
+                data[direction_prefix + "_market_value"] = self._safe_convert(pos.market_value)
                 data[direction_prefix + "_quantity"] = self._safe_convert(pos.quantity)
                 data[direction_prefix + "_avg_open_price"] = self._safe_convert(getattr(pos, "avg_price", None))
         return data
 
     def _to_trade_record(self, trade):
         return {
             'datetime': trade.datetime.strftime("%Y-%m-%d %H:%M:%S"),
@@ -485,14 +486,34 @@
             positions_list = self._positions[account_type]
             df = pd.DataFrame(positions_list)
             if "date" in df.columns:
                 df["date"] = pd.to_datetime(df["date"])
                 df = df.set_index("date").sort_index()
             result_dict["{}_positions".format(account_name)] = df
 
+        # 个股权重
+        df_list = []
+        need_cols = ["order_book_id", "market_value"]
+        for table_name in ["stock_positions", "future_positions"]:
+            if table_name not in result_dict:
+                continue
+            table = result_dict[table_name]
+            for field in ["market_value", "LONG_market_value", "SHORT_market_value"]:
+                if field not in table.columns:
+                    continue
+                df_list.append(table.rename(columns={field: "market_value"})[need_cols])
+        if len(df_list) > 0:
+            positions_weight_df = pd.concat(df_list).dropna()
+            positions_weight_df["total_value"] = positions_weight_df.groupby(by="date")["market_value"].sum()
+            positions_weight_df["weight"] = positions_weight_df["market_value"] / positions_weight_df["total_value"]
+            positions_weight_df = positions_weight_df.groupby(by="date")["weight"].describe()
+        else:
+            positions_weight_df = pd.DataFrame(columns=["count", "mean", "std", "min", "25%", "50%", "75%", "max"])
+        positions_weight_df = positions_weight_df.reindex(total_portfolios.index).fillna(value=0)
+        result_dict["positions_weight"] = positions_weight_df
         result_dict["yearly_risk_free_rates"] = dict(_get_yearly_risk_free_rates(data_proxy, start_date, end_date))
 
         if self._mod_config.output_file:
             with open(self._mod_config.output_file, 'wb') as f:
                 pickle.dump(result_dict, f)
 
         if self._mod_config.report_save_path:
```

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/consts.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/plot.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot/utils.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/plot_store.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/excel_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,15 +77,16 @@
 
 class SummaryTemplate(ExcelTemplate):
     TEMPLATE_NAME = "summary"
     SCHEMA_CLASSES = {
         "概览": SingleCellSchema,
         "年度指标": VerticalSeriesSchema,
         "月度收益": VerticalSeriesSchema,
-        "月度超额收益（几何）": VerticalSeriesSchema
+        "月度超额收益（几何）": VerticalSeriesSchema,
+        "个股权重": VerticalSeriesSchema,
     }
 
 
 SUMMARY_TEMPLATE = SummaryTemplate()
 
 
 def generate_xlsx_reports(data, output_path):
```

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_analyser/report/report.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,14 +102,19 @@
             b_month_returns = b_returns.loc[p_month_returns.index]
             data.loc[year, month] = (p_month_returns + 1).prod() / (b_month_returns + 1).prod() - 1
         b_year_returns = b_returns.loc[p_year_returns.index]
         data.loc[year, "cum"] = (p_year_returns + 1).prod() / (b_year_returns + 1).prod() - 1
     return ChainMap({str(c): data[c] for c in data.columns}, {"year": data.index})
 
 
+def _gen_positions_weight(df):
+    rename = {"{}%".format(i): "percent_{}".format(i) for i in [25, 50, 75]}
+    return df.reset_index().rename(columns=rename).to_dict(orient="list")
+
+
 def generate_report(result_dict, output_path):
     from six import StringIO
 
     try:
         os.mkdir(output_path)
     except:
         pass
@@ -124,32 +129,37 @@
         b_returns = _returns(b_nav)
     else:
         b_nav = b_returns = None
     generate_xlsx_reports({
         "概览": summary,
         "年度指标": _yearly_indicators(p_nav, p_returns, b_nav, b_returns, result_dict["yearly_risk_free_rates"]),
         "月度收益": _monthly_returns(p_returns),
-        "月度超额收益（几何）": _monthly_geometric_excess_returns(p_returns, b_returns)
+        "月度超额收益（几何）": _monthly_geometric_excess_returns(p_returns, b_returns),
+        "个股权重": _gen_positions_weight(result_dict["positions_weight"]),
     }, output_path)
 
     for name in ["portfolio", "stock_account", "future_account",
-                 "stock_positions", "future_positions", "trades"]:
+                 "stock_positions", "future_positions", "trades", "positions_weight"]:
         try:
             df = result_dict[name]
         except KeyError:
             continue
 
         # replace all date in dataframe as string
         if df.index.name == "date":
             df = df.reset_index()
             df["date"] = df["date"].apply(lambda x: x.strftime("%Y-%m-%d"))
             df = df.set_index("date")
 
         csv_txt = StringIO()
-        csv_txt.write(df.to_csv(encoding='utf-8', lineterminator='\n'))
+        try:
+            csv_txt.write(df.to_csv(encoding='utf-8', lineterminator='\n'))
+        except TypeError as e:
+            # pandas 1.5.0 以下是 line_terminator
+            csv_txt.write(df.to_csv(encoding='utf-8', line_terminator='\n'))
 
         with open(os.path.join(output_path, "{}.csv".format(name)), 'w') as csvfile:
             csvfile.write(csv_txt.getvalue())
 
 
 if __name__ == "__main__":
     import pickle
```

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_progress/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_progress/mod.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_progress/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/mod.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/cash_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/is_trading_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/price_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_risk/validators/self_trade_validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_scheduler/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/matcher.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/signal_broker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_broker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/simulation_event_source.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/slippage.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/testing.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_simulation/validator.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_simulation/validator.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/deciders.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py` & `rqalpha-5.1.0/rqalpha/mod/rqalpha_mod_sys_transaction_cost/mod.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/mod/utils.py` & `rqalpha-5.1.0/rqalpha/mod/utils.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/model/__init__.py` & `rqalpha-5.1.0/rqalpha/model/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/model/bar.py` & `rqalpha-5.1.0/rqalpha/model/bar.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/model/instrument.py` & `rqalpha-5.1.0/rqalpha/model/instrument.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/model/order.py` & `rqalpha-5.1.0/rqalpha/model/order.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/model/tick.py` & `rqalpha-5.1.0/rqalpha/model/tick.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/model/trade.py` & `rqalpha-5.1.0/rqalpha/model/trade.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/portfolio/__init__.py` & `rqalpha-5.1.0/rqalpha/portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/portfolio/account.py` & `rqalpha-5.1.0/rqalpha/portfolio/account.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/portfolio/position.py` & `rqalpha-5.1.0/rqalpha/portfolio/position.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from rqalpha.interface import AbstractPosition
 from rqalpha.model.instrument import Instrument
 from rqalpha.model.order import Order
 from rqalpha.model.trade import Trade
 from rqalpha.utils import is_valid_price
 from rqalpha.utils.i18n import gettext as _
 from rqalpha.utils.repr import PropertyReprMeta, property_repr
+from rqalpha.utils.logger import user_system_log
 
 
 def new_position_meta():
     type_map = {}
 
     class Meta(PropertyReprMeta):
         def __new__(mcs, *args, **kwargs):
@@ -115,15 +116,15 @@
         # type: () -> float
         return self._avg_price
 
     @property
     def trading_pnl(self):
         # type: () -> float
         trade_quantity = self._quantity - self._logical_old_quantity
-        return (trade_quantity * self.last_price - self._trade_cost) * self._direction_factor if trade_quantity else 0
+        return (trade_quantity * self.last_price - self._trade_cost) * self._direction_factor
 
     @property
     def position_pnl(self):
         # type: () -> float
         if self._logical_old_quantity:
             return self._logical_old_quantity * (self.last_price - self.prev_close) * self._direction_factor
         else:
@@ -145,22 +146,28 @@
     @property
     def equity(self):
         # type: () -> float
         return self.last_price * self._quantity if self._quantity else 0
 
     @property
     def prev_close(self):
+        # type: () -> float
         if not is_valid_price(self._prev_close):
             self._prev_close = self._env.data_proxy.get_prev_close(self._order_book_id, self._env.trading_dt)
+            if not is_valid_price(self._prev_close):
+                user_system_log.warn("invalid prev close of {}: {}".format(self._order_book_id, self._prev_close))
         return self._prev_close
 
     @property
     def last_price(self):
+        # type: () -> float
         if not is_valid_price(self._last_price):
             self._last_price = self._env.data_proxy.get_last_price(self._order_book_id)
+            if not is_valid_price(self._last_price):
+                user_system_log.warn("invalid last price of {}: {}".format(self._order_book_id, self._last_price))
         return self._last_price
 
     @property
     def closable(self):
         # type: () -> int
         """
         可平仓位
```

### Comparing `rqalpha-5.0.0/rqalpha/resource/ricequant-logo.png` & `rqalpha-5.1.0/rqalpha/resource/ricequant-logo.png`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/user_module.py` & `rqalpha-5.1.0/rqalpha/user_module.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/__init__.py` & `rqalpha-5.1.0/rqalpha/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,7 +237,14 @@
     trading_period = STOCK_TRADING_PERIOD if DEFAULT_ACCOUNT_TYPE.STOCK in accounts else []
     return Environment.get_instance().data_proxy.get_trading_period(universe, trading_period)
 
 
 def safe_div(dividend, divisor):
     return dividend / divisor if divisor else np.nan
 
+
+def check_items_in_container(items, should_in, name):
+    for item in items:
+        if item not in should_in:
+            raise ValueError(
+                "{}: got invalided value {}, choose any in {}".format(name, item, should_in)
+            )
```

### Comparing `rqalpha-5.0.0/rqalpha/utils/arg_checker.py` & `rqalpha-5.1.0/rqalpha/utils/arg_checker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/class_helper.py` & `rqalpha-5.1.0/rqalpha/utils/class_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/click_helper.py` & `rqalpha-5.1.0/rqalpha/utils/click_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/concurrent.py` & `rqalpha-5.1.0/rqalpha/utils/concurrent.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/config.py` & `rqalpha-5.1.0/rqalpha/utils/config.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/datetime_func.py` & `rqalpha-5.1.0/rqalpha/utils/datetime_func.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/dict_func.py` & `rqalpha-5.1.0/rqalpha/utils/dict_func.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/exception.py` & `rqalpha-5.1.0/rqalpha/utils/exception.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/functools.py` & `rqalpha-5.1.0/rqalpha/utils/functools.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/i18n.py` & `rqalpha-5.1.0/rqalpha/utils/i18n.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/log_capture.py` & `rqalpha-5.1.0/rqalpha/utils/log_capture.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/logger.py` & `rqalpha-5.1.0/rqalpha/utils/logger.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/package_helper.py` & `rqalpha-5.1.0/rqalpha/utils/package_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/persisit_helper.py` & `rqalpha-5.1.0/rqalpha/utils/persisit_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/repr.py` & `rqalpha-5.1.0/rqalpha/utils/repr.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/risk_free_helper.py` & `rqalpha-5.1.0/rqalpha/utils/risk_free_helper.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/rq_json.py` & `rqalpha-5.1.0/rqalpha/utils/rq_json.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/strategy_loader_help.py` & `rqalpha-5.1.0/rqalpha/utils/strategy_loader_help.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/testing/__init__.py` & `rqalpha-5.1.0/rqalpha/utils/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/testing/fixtures.py` & `rqalpha-5.1.0/rqalpha/utils/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/testing/mocking.py` & `rqalpha-5.1.0/rqalpha/utils/testing/mocking.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/translations/__init__.py` & `rqalpha-5.1.0/rqalpha/utils/translations/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py` & `rqalpha-5.1.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo` & `rqalpha-5.1.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po` & `rqalpha-5.1.0/rqalpha/utils/translations/zh_Hans_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/translations/zh_Hans_CN/__init__.py` & `rqalpha-5.1.0/rqalpha/utils/translations/zh_Hans_CN/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha/utils/typing.py` & `rqalpha-5.1.0/rqalpha/utils/typing.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/rqalpha.egg-info/PKG-INFO` & `rqalpha-5.1.0/rqalpha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rqalpha
-Version: 5.0.0
+Version: 5.1.0
 Summary: Ricequant Algorithm Trading System
 Home-page: https://github.com/ricequant/rqalpha
 Author: ricequant
 Author-email: public@ricequant.com
 License: Apache License v2
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
```

### Comparing `rqalpha-5.0.0/rqalpha.egg-info/SOURCES.txt` & `rqalpha-5.1.0/rqalpha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/setup.py` & `rqalpha-5.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/__init__.py` & `rqalpha-5.1.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/api_tests/__init__.py` & `rqalpha-5.1.0/tests/api_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/api_tests/mod/__init__.py` & `rqalpha-5.1.0/tests/api_tests/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/api_tests/mod/sys_accounts/__init__.py` & `rqalpha-5.1.0/tests/api_tests/mod/sys_accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/api_tests/mod/sys_accounts/test_account_model.py` & `rqalpha-5.1.0/tests/api_tests/mod/sys_accounts/test_account_model.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/api_tests/mod/sys_accounts/test_futures_settlement_price_type.py` & `rqalpha-5.1.0/tests/api_tests/mod/sys_accounts/test_futures_settlement_price_type.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/api_tests/mod/sys_accounts/test_margin_stocks.py` & `rqalpha-5.1.0/tests/api_tests/mod/sys_accounts/test_margin_stocks.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/api_tests/mod/sys_accounts/test_position_models.py` & `rqalpha-5.1.0/tests/api_tests/mod/sys_transaction_cost/test_commission_multiplier.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,43 +9,47 @@
 #
 #     * 商业用途（商业用途指个人出于任何商业目的使用本软件，或者法人或其他组织出于任何目的使用本软件）：
 #         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 
 from rqalpha.apis import *
+from rqalpha.environment import Environment
 
 __config__ = {
     "base": {
-        "start_date": "2016-03-07",
-        "end_date": "2016-03-08",
+        "start_date": "2022-01-01",
+        "end_date": "2022-01-30",
         "frequency": "1d",
         "accounts": {
             "stock": 1000000,
+            "future": 1000000,
         }
     },
-    "extra": {
-        "log_level": "error",
-    },
     "mod": {
-        "sys_progress": {
-            "enabled": True,
-            "show": True,
+        "sys_transaction_cost": {
+            "stock_commission_multiplier": 2,
+            "futures_commission_multiplier": 3,
         }
-    },
+    }
 }
 
 
-def test_stock_sellable():
-    def init(context):
-        context.fired = False
-        context.s = "000001.XSHE"
+def test_commission_multiplier():
 
-    def handle_bar(context, _):
-        if not context.fired:
-            order_shares(context.s, 1000)
-            sellable = context.portfolio.positions[context.s].sellable
-            assert sellable == 0, "wrong sellable {}, supposed to be {}".format(sellable, 0)
-            context.fired = True
+    def init(context):
+        context.s1 = "000001.XSHE"
+        context.s2 = "IC2203"
+        context.fixed = True
+
+    def handle_bar(context, bar_dict):
+        if context.fixed:
+            stock_order = order_percent(context.s1, 1)
+            future_order = buy_open(context.s2, 1)
+            env = Environment.get_instance()
+            future_commission_info = env.data_proxy.get_commission_info(context.s2)
+            context.fixed = False
+            assert stock_order.transaction_cost == 16.66 * 59900 * 8 / 10000 * 2
+            assert future_order.transaction_cost == 7308 * 200 * future_commission_info["open_commission_ratio"] * 3
 
     return locals()
```

### Comparing `rqalpha-5.0.0/tests/api_tests/mod/sys_scheduler/test_physical_time.py` & `rqalpha-5.1.0/tests/api_tests/mod/sys_scheduler/test_physical_time.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/api_tests/mod/sys_scheduler/test_scheduler.py` & `rqalpha-5.1.0/tests/api_tests/mod/sys_scheduler/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/api_tests/mod/sys_simulation/__init__.py` & `rqalpha-5.1.0/tests/api_tests/mod/sys_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/api_tests/mod/sys_simulation/test_management_fee.py` & `rqalpha-5.1.0/tests/api_tests/mod/sys_simulation/test_management_fee.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/api_tests/mod/sys_simulation/test_signal_broker.py` & `rqalpha-5.1.0/tests/api_tests/mod/sys_simulation/test_signal_broker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/api_tests/mod/sys_simulation/test_simulation_broker.py` & `rqalpha-5.1.0/tests/api_tests/mod/sys_simulation/test_simulation_broker.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py` & `rqalpha-5.1.0/tests/api_tests/mod/sys_simulation/test_simulation_event_source.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/api_tests/mod/sys_transaction_cost/test_commission_multiplier.py` & `rqalpha-5.1.0/tests/unittest/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,48 +8,24 @@
 #         除非法律有要求或以书面形式达成协议，否则本软件分发时需保持当前许可“原样”不变，且不得附加任何条件。
 #
 #     * 商业用途（商业用途指个人出于任何商业目的使用本软件，或者法人或其他组织出于任何目的使用本软件）：
 #         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 
-from rqalpha.apis import *
-from rqalpha.environment import Environment
+import os
 
-__config__ = {
-    "base": {
-        "start_date": "2022-01-01",
-        "end_date": "2022-01-30",
-        "frequency": "1d",
-        "accounts": {
-            "stock": 1000000,
-            "future": 1000000,
-        }
-    },
-    "mod": {
-        "sys_transaction_cost": {
-            "stock_commission_multiplier": 2,
-            "futures_commission_multiplier": 3,
-        }
-    }
-}
-
-
-def test_commission_multiplier():
-
-    def init(context):
-        context.s1 = "000001.XSHE"
-        context.s2 = "IC2203"
-        context.fixed = True
-
-    def handle_bar(context, bar_dict):
-        if context.fixed:
-            stock_order = order_percent(context.s1, 1)
-            future_order = buy_open(context.s2, 1)
-            env = Environment.get_instance()
-            future_commission_info = env.data_proxy.get_commission_info(context.s2)
-            context.fixed = False
-            assert stock_order.transaction_cost == 16.66 * 59900 * 8 / 10000 * 2
-            assert future_order.transaction_cost == 7308 * 200 * future_commission_info["open_commission_ratio"] * 3
+from unittest import TestLoader, TestSuite, TextTestRunner
 
-    return locals()
 
+def load_tests():
+    test_suite = TestSuite()
+    this_dir = os.path.dirname(__file__)
+    loader = TestLoader()
+    package_tests = loader.discover(start_dir=this_dir)
+    test_suite.addTests(package_tests)
+    return test_suite
+
+
+if __name__ == "__main__":
+    runner = TextTestRunner(verbosity=2)
+    runner.run(load_tests())
```

### Comparing `rqalpha-5.0.0/tests/api_tests/test_api_base.py` & `rqalpha-5.1.0/tests/api_tests/test_api_base.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/api_tests/test_api_future.py` & `rqalpha-5.1.0/tests/api_tests/test_api_future.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/api_tests/test_api_stock.py` & `rqalpha-5.1.0/tests/api_tests/test_api_stock.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/api_tests/test_config.py` & `rqalpha-5.1.0/tests/api_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/test_f_buy_and_hold.py` & `rqalpha-5.1.0/tests/test_f_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/test_f_macd.py` & `rqalpha-5.1.0/tests/test_f_macd.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/test_f_macd_signal.py` & `rqalpha-5.1.0/tests/test_f_macd_signal.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/test_f_mean_reverting.py` & `rqalpha-5.1.0/tests/test_f_mean_reverting.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/test_s_buy_and_hold.py` & `rqalpha-5.1.0/tests/test_s_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/test_s_dual_thrust.py` & `rqalpha-5.1.0/tests/test_s_dual_thrust.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/test_s_scheduler.py` & `rqalpha-5.1.0/tests/test_s_scheduler.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/test_s_tick_size.py` & `rqalpha-5.1.0/tests/test_s_tick_size.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/test_s_turtle.py` & `rqalpha-5.1.0/tests/test_s_turtle.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/test_s_turtle_signal.py` & `rqalpha-5.1.0/tests/test_s_turtle_signal.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/test_sf_buy_and_hold.py` & `rqalpha-5.1.0/tests/test_sf_buy_and_hold.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/unittest/__init__.py` & `rqalpha-5.1.0/tests/unittest/test_mod/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,22 +10,12 @@
 #     * 商业用途（商业用途指个人出于任何商业目的使用本软件，或者法人或其他组织出于任何目的使用本软件）：
 #         未经米筐科技授权，任何个人不得出于任何商业目的使用本软件（包括但不限于向第三方提供、销售、出租、出借、转让本软件、本软件的衍生产品、引用或借鉴了本软件功能或源代码的产品或服务），任何法人或其他组织不得出于任何目的使用本软件，否则米筐科技有权追究相应的知识产权侵权责任。
 #         在此前提下，对本软件的使用同样需要遵守 Apache 2.0 许可，Apache 2.0 许可与本许可冲突之处，以本许可为准。
 #         详细的授权流程，请联系 public@ricequant.com 获取。
 
 import os
 
-from unittest import TestLoader, TestSuite, TextTestRunner
 
-
-def load_tests():
-    test_suite = TestSuite()
+def load_tests(loader, standard_tests, pattern):
     this_dir = os.path.dirname(__file__)
-    loader = TestLoader()
-    package_tests = loader.discover(start_dir=this_dir)
-    test_suite.addTests(package_tests)
-    return test_suite
-
-
-if __name__ == "__main__":
-    runner = TextTestRunner(verbosity=2)
-    runner.run(load_tests())
+    standard_tests.addTests(loader.discover(start_dir=this_dir, pattern=pattern))
+    return standard_tests
```

### Comparing `rqalpha-5.0.0/tests/unittest/test_data/test_instrument_mixin.py` & `rqalpha-5.1.0/tests/unittest/test_data/test_instrument_mixin.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/unittest/test_data/test_trading_dates_mixin.py` & `rqalpha-5.1.0/tests/unittest/test_data/test_trading_dates_mixin.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/unittest/test_mod/__init__.py` & `rqalpha-5.1.0/tests/unittest/test_mod/test_sys_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py` & `rqalpha-5.1.0/tests/unittest/test_mod/test_sys_simulation/test_simulation_event_source.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/tests/utils.py` & `rqalpha-5.1.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `rqalpha-5.0.0/versioneer.py` & `rqalpha-5.1.0/versioneer.py`

 * *Files identical despite different names*

