# Comparing `tmp/bemserver-ui-0.5.2.tar.gz` & `tmp/bemserver-ui-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bemserver-ui-0.5.2.tar", last modified: Thu May 25 08:25:46 2023, max compression
+gzip compressed data, was "bemserver-ui-0.5.3.tar", last modified: Fri Jun 16 08:46:45 2023, max compression
```

## Comparing `bemserver-ui-0.5.2.tar` & `bemserver-ui-0.5.3.tar`

### file list

```diff
@@ -1,312 +1,317 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.745495 bemserver-ui-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-25 08:25:46.745495 bemserver-ui-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.709492 bemserver-ui-0.5.2/bemserver_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.713493 bemserver-ui-0.5.2/bemserver_ui/common/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/common/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/common/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/common/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/common/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.713493 bemserver-ui-0.5.2/bemserver_ui/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/campaign_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/flask_es6.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/jinja_custom_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/partners.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.713493 bemserver-ui-0.5.2/bemserver_ui/extensions/timezones/
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/timezones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66289 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/timezones/timezones-areas.json
--rw-r--r--   0 runner    (1001) docker     (123)   224723 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/timezones/timezones-full.json
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/timezones/timezones-regions.json
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/extensions/timezones/timezones.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.713493 bemserver-ui-0.5.2/bemserver_ui/internal_api/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.717493 bemserver-ui-0.5.2/bemserver_ui/internal_api/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/analysis/completeness.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/analysis/degree_days.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/analysis/energy_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/campaign_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.717493 bemserver-ui-0.5.2/bemserver_ui/internal_api/semantics/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/semantics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.717493 bemserver-ui-0.5.2/bemserver_ui/internal_api/semantics/energy/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/semantics/energy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/semantics/energy/consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/semantics/energy/production.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/semantics/weather.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.717493 bemserver-ui-0.5.2/bemserver_ui/internal_api/services/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/services/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/services/missing_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/services/outlier_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/services/weather_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/structural_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.717493 bemserver-ui-0.5.2/bemserver_ui/internal_api/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/timeseries/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/timeseries/datastates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/timeseries/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/user_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/internal_api/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.709492 bemserver-ui-0.5.2/bemserver_ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.717493 bemserver-ui-0.5.2/bemserver_ui/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/images/bemserver-ico.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/images/bemserver-min.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/images/bemserver.ico
--rw-r--r--   0 runner    (1001) docker     (123)    35322 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/images/bemserver.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.717493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/app.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.717493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.717493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/accordionList.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.717493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/charts/
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/charts/tsChartCompleteness.js
--rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/charts/tsChartDegreeDays.js
--rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/charts/tsChartEnergyConsumption.js
--rw-r--r--   0 runner    (1001) docker     (123)    14389 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/charts/tsChartExplore.js
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/dropZone.js
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/eventLevel.js
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/filterSelect.js
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/flash.js
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/itemsCount.js
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/modalConfirm.js
--rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/pagination.js
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/spinner.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.721493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/structuralElements/
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/structuralElements/selector.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.721493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/time/
--rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/time/datetimePicker.js
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/time/tzPicker.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.721493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/timeseries/bucketWidth.js
--rw-r--r--   0 runner    (1001) docker     (123)    32482 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/timeseries/selector.js
--rw-r--r--   0 runner    (1001) docker     (123)    14980 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/tree.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.721493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/userGroup/
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/userGroup/userGroupItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/flashTimer.js
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/formController.js
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/notifications.js
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/sidebar.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.721493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/array.js
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/dict.js
--rw-r--r--   0 runner    (1001) docker     (123)    12459 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/fetcher.js
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/flaskES6.js
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/parser.js
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/time.js
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/uuid.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.709492 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.721493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/analysis/degreeDays.js
--rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/analysis/energyConsumption.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.721493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/campaignScopes/
--rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/campaignScopes/manageGroups.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.721493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/campaigns/
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/campaigns/selector.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.721493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/events/
--rw-r--r--   0 runner    (1001) docker     (123)    39836 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/events/edit.js
--rw-r--r--   0 runner    (1001) docker     (123)    45177 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/events/list.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.721493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)    66390 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/notifications/explore.js
--rw-r--r--   0 runner    (1001) docker     (123)    15380 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/notifications/setup.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.721493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/cleanupManage.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.721493 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/missingData/
--rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/missingData/list.js
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/missingData/manage.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.725494 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/outlierData/
--rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/outlierData/list.js
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/outlierData/manage.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.725494 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/weatherData/
--rw-r--r--   0 runner    (1001) docker     (123)    28636 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/weatherData/manage.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.725494 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/structuralElements/
--rw-r--r--   0 runner    (1001) docker     (123)    27358 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/structuralElements/explore.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.725494 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.725494 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/data/
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/data/completeness.js
--rw-r--r--   0 runner    (1001) docker     (123)    12841 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/data/explore.js
--rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/delete.js
--rw-r--r--   0 runner    (1001) docker     (123)    25408 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/list.js
--rw-r--r--   0 runner    (1001) docker     (123)    18386 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/manageStructuralElements.js
--rw-r--r--   0 runner    (1001) docker     (123)    62819 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/semanticSetup.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.725494 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/users/list.js
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/users/manageGroups.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.725494 bemserver-ui-0.5.2/bemserver_ui/static/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/styles/app.css
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/styles/dragndrop.css
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/styles/main.css
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/styles/signin.css
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/static/styles/tree.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.709492 bemserver-ui-0.5.2/bemserver_ui/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.725494 bemserver-ui-0.5.2/bemserver_ui/templates/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.725494 bemserver-ui-0.5.2/bemserver_ui/templates/components/campaigns/
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/campaigns/selector.html
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/header.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.729494 bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_admin.html
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_analysis.html
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_campaign_context.html
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_campaign_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_dashboards.html
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_services.html
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_tsdata.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.729494 bemserver-ui-0.5.2/bemserver_ui/templates/components/user_groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/user_groups/group_for_campaign.html
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/user_groups/group_for_campaign_scope.html
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/user_groups/user_group_available.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.729494 bemserver-ui-0.5.2/bemserver_ui/templates/components/users/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/users/user_available.html
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/components/users/user_for_group.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.729494 bemserver-ui-0.5.2/bemserver_ui/templates/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.729494 bemserver-ui-0.5.2/bemserver_ui/templates/macros/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/macros/components/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/macros/components/structural_element_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/macros/components/ts_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/macros/flash.html
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/macros/partners.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.729494 bemserver-ui-0.5.2/bemserver_ui/templates/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/about.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.729494 bemserver-ui-0.5.2/bemserver_ui/templates/pages/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/analysis/degree_days.html
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/analysis/energy_consumption.html
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.729494 bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaign_scopes/
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaign_scopes/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaign_scopes/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaign_scopes/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaign_scopes/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.733494 bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaigns/
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaigns/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaigns/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaigns/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaigns/manage_groups.html
--rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaigns/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.733494 bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.733494 bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/categories/
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/categories/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/categories/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/categories/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/create.html
--rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/home.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.733494 bemserver-ui-0.5.2/bemserver_ui/templates/pages/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/notifications/explore.html
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/notifications/setup.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.709492 bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.733494 bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/cleanup/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/cleanup/manage.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.733494 bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/missing_data/
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/missing_data/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/missing_data/manage.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.733494 bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/outlier_data/
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/outlier_data/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/outlier_data/manage.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.733494 bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/weather_data/
--rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/weather_data/manage.html
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/signin.html
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/skeleton.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.737495 bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/create.html
--rw-r--r--   0 runner    (1001) docker     (123)    16005 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/explore.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.737495 bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/properties/
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/properties/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/properties/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/properties/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/upload.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.737495 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/create.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.737495 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/data/
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/data/completeness.html
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/data/delete.html
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/data/explore.html
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/data/upload.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.737495 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/datastates/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/datastates/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/datastates/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/datastates/list.html
--rw-r--r--   0 runner    (1001) docker     (123)    15056 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)    17296 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/manage_structural_elements.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.737495 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/properties/
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/properties/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/properties/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/properties/list.html
--rw-r--r--   0 runner    (1001) docker     (123)    15694 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/semantic_setup.html
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/upload.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.741495 bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/manage.html
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/manage_campaign_scopes.html
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/manage_campaigns.html
--rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.741495 bemserver-ui-0.5.2/bemserver_ui/templates/pages/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/users/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/users/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/users/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/templates/pages/users/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.741495 bemserver-ui-0.5.2/bemserver_ui/views/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.745495 bemserver-ui-0.5.2/bemserver_ui/views/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/analysis/degree_days.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/analysis/energy_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/campaign_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/campaigns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.745495 bemserver-ui-0.5.2/bemserver_ui/views/events/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/events/categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/events/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.745495 bemserver-ui-0.5.2/bemserver_ui/views/services/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/services/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/services/missing_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/services/outlier_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/services/weather_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.745495 bemserver-ui-0.5.2/bemserver_ui/views/structural_elements/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/structural_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/structural_elements/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/structural_elements/structural_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.745495 bemserver-ui-0.5.2/bemserver_ui/views/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/timeseries/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/timeseries/datastates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/timeseries/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/timeseries/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/user_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/bemserver_ui/views/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.709492 bemserver-ui-0.5.2/bemserver_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-25 08:25:46.000000 bemserver-ui-0.5.2/bemserver_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-05-25 08:25:46.000000 bemserver-ui-0.5.2/bemserver_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 08:25:46.000000 bemserver-ui-0.5.2/bemserver_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-25 08:25:46.000000 bemserver-ui-0.5.2/bemserver_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 08:25:46.000000 bemserver-ui-0.5.2/bemserver_ui.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:25:46.745495 bemserver-ui-0.5.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/requirements/install.txt
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-25 08:25:46.749496 bemserver-ui-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-25 08:25:38.000000 bemserver-ui-0.5.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.399373 bemserver-ui-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-16 08:46:45.399373 bemserver-ui-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.375373 bemserver-ui-0.5.3/bemserver_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.379373 bemserver-ui-0.5.3/bemserver_ui/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/common/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/common/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/common/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.379373 bemserver-ui-0.5.3/bemserver_ui/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/campaign_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/flask_es6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/jinja_custom_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/partners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.379373 bemserver-ui-0.5.3/bemserver_ui/extensions/timezones/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/timezones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66289 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/timezones/timezones-areas.json
+-rw-r--r--   0 runner    (1001) docker     (123)   224723 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/timezones/timezones-full.json
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/timezones/timezones-regions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/extensions/timezones/timezones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.379373 bemserver-ui-0.5.3/bemserver_ui/internal_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.379373 bemserver-ui-0.5.3/bemserver_ui/internal_api/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/analysis/completeness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/analysis/degree_days.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/analysis/energy_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/analysis/weather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/campaign_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.379373 bemserver-ui-0.5.3/bemserver_ui/internal_api/semantics/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/semantics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.379373 bemserver-ui-0.5.3/bemserver_ui/internal_api/semantics/energy/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/semantics/energy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/semantics/energy/consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/semantics/energy/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/semantics/weather.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.383373 bemserver-ui-0.5.3/bemserver_ui/internal_api/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/services/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/services/missing_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/services/outlier_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/services/weather_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/structural_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.383373 bemserver-ui-0.5.3/bemserver_ui/internal_api/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/timeseries/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/timeseries/datastates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/timeseries/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/internal_api/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.375373 bemserver-ui-0.5.3/bemserver_ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.383373 bemserver-ui-0.5.3/bemserver_ui/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/images/bemserver-ico.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/images/bemserver-min.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/images/bemserver.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    35322 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/images/bemserver.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.383373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/app.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.383373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.383373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/accordionList.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.383373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/charts/tsChartCompleteness.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/charts/tsChartDegreeDays.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/charts/tsChartEnergyConsumption.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16874 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/charts/tsChartExplore.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/charts/tsChartWeather.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/dropZone.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/eventLevel.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/filterSelect.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/flash.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/itemsCount.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/modalConfirm.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/pagination.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/spinner.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.383373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/structuralElements/
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/structuralElements/selector.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.383373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/time/
+-rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/time/datetimePicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/time/tzPicker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.383373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/timeseries/bucketWidth.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33290 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/timeseries/selector.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14980 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/tree.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.383373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/userGroup/
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/userGroup/userGroupItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/flashTimer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/formController.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/notifications.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/sidebar.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/array.js
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/dict.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12459 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/fetcher.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/flaskES6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/parser.js
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/time.js
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/uuid.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.375373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/analysis/degreeDays.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/analysis/energyConsumption.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16596 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/analysis/weather.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/campaignScopes/
+-rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/campaignScopes/manageGroups.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/campaigns/
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/campaigns/selector.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/events/
+-rw-r--r--   0 runner    (1001) docker     (123)    39836 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/events/edit.js
+-rw-r--r--   0 runner    (1001) docker     (123)    45177 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/events/list.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)    66390 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/notifications/explore.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15480 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/notifications/setup.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/cleanupManage.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/missingData/
+-rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/missingData/list.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/missingData/manage.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/outlierData/
+-rw-r--r--   0 runner    (1001) docker     (123)    11130 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/outlierData/list.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/outlierData/manage.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/weatherData/
+-rw-r--r--   0 runner    (1001) docker     (123)    28653 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/weatherData/manage.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/structuralElements/
+-rw-r--r--   0 runner    (1001) docker     (123)    27358 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/structuralElements/explore.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/data/completeness.js
+-rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/data/explore.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/delete.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25408 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/list.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18386 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/manageStructuralElements.js
+-rw-r--r--   0 runner    (1001) docker     (123)    62819 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/semanticSetup.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/users/list.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/users/manageGroups.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/static/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/styles/app.css
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/styles/dragndrop.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/styles/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/styles/signin.css
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/static/styles/tree.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.375373 bemserver-ui-0.5.3/bemserver_ui/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/templates/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/templates/components/campaigns/
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/campaigns/selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.387373 bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_admin.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_analysis.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_campaign_context.html
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_campaign_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_dashboards.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_services.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_tsdata.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/components/user_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/user_groups/group_for_campaign.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/user_groups/group_for_campaign_scope.html
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/user_groups/user_group_available.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/components/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/users/user_available.html
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/components/users/user_for_group.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/macros/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/macros/components/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/macros/components/structural_element_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/macros/components/ts_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/macros/flash.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/macros/partners.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/about.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/analysis/degree_days.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/analysis/energy_consumption.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/analysis/weather.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaign_scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaign_scopes/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaign_scopes/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaign_scopes/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaign_scopes/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaigns/
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaigns/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaigns/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaigns/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaigns/manage_groups.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaigns/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/categories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/categories/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/categories/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/categories/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/home.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)    10620 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/notifications/explore.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/notifications/setup.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.375373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/cleanup/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/cleanup/manage.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.391373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/missing_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/missing_data/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/missing_data/manage.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.395373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/outlier_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/outlier_data/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/outlier_data/manage.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.395373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/weather_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/weather_data/manage.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/signin.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/skeleton.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.395373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16005 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/explore.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.395373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/properties/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/properties/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/properties/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/upload.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.395373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/create.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.395373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/data/completeness.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/data/delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/data/explore.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/data/upload.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.395373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/datastates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/datastates/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/datastates/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/datastates/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15056 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17296 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/manage_structural_elements.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.395373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/properties/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/properties/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/properties/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15694 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/semantic_setup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/upload.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.395373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/manage.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/manage_campaign_scopes.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/manage_campaigns.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.395373 bemserver-ui-0.5.3/bemserver_ui/templates/pages/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/users/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/users/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/users/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/templates/pages/users/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.395373 bemserver-ui-0.5.3/bemserver_ui/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.399373 bemserver-ui-0.5.3/bemserver_ui/views/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/analysis/degree_days.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/analysis/energy_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/analysis/weather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/campaign_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/campaigns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.399373 bemserver-ui-0.5.3/bemserver_ui/views/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/events/categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.399373 bemserver-ui-0.5.3/bemserver_ui/views/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/services/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/services/missing_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/services/outlier_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/services/weather_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.399373 bemserver-ui-0.5.3/bemserver_ui/views/structural_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/structural_elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/structural_elements/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/structural_elements/structural_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.399373 bemserver-ui-0.5.3/bemserver_ui/views/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/timeseries/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/timeseries/datastates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/timeseries/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/timeseries/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/bemserver_ui/views/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.379373 bemserver-ui-0.5.3/bemserver_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-16 08:46:45.000000 bemserver-ui-0.5.3/bemserver_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-06-16 08:46:45.000000 bemserver-ui-0.5.3/bemserver_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 08:46:45.000000 bemserver-ui-0.5.3/bemserver_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-16 08:46:45.000000 bemserver-ui-0.5.3/bemserver_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 08:46:45.000000 bemserver-ui-0.5.3/bemserver_ui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 08:46:45.399373 bemserver-ui-0.5.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/requirements/install.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-16 08:46:45.399373 bemserver-ui-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-16 08:46:38.000000 bemserver-ui-0.5.3/tox.ini
```

### Comparing `bemserver-ui-0.5.2/LICENSE` & `bemserver-ui-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/PKG-INFO` & `bemserver-ui-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bemserver-ui
-Version: 0.5.2
+Version: 0.5.3
 Summary: BEMServer web interface
 Home-page: https://github.com/BEMServer/bemserver-ui
 Author: NOBATEK/INEF4
 Author-email: dfrederique@nobatek.inef4.com
 License: AGPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bemserver-ui-0.5.2/README.rst` & `bemserver-ui-0.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/__init__.py` & `bemserver-ui-0.5.3/bemserver_ui/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import flask
 
 from . import extensions
 from . import internal_api
 from . import views
 
 
-__version__ = "0.5.2"
+__version__ = "0.5.3"
 
 
 def create_app(config_override=None):
     """Create application"""
     app = flask.Flask(__name__)
     app.config.from_object("bemserver_ui.settings.Config")
     app.config.from_envvar("BEMSERVER_UI_SETTINGS_FILE", silent=True)
```

### Comparing `bemserver-ui-0.5.2/bemserver_ui/common/tree.py` & `bemserver-ui-0.5.3/bemserver_ui/common/tree.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/extensions/__init__.py` & `bemserver-ui-0.5.3/bemserver_ui/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/extensions/api_client.py` & `bemserver-ui-0.5.3/bemserver_ui/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/extensions/auth.py` & `bemserver-ui-0.5.3/bemserver_ui/extensions/auth.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/extensions/campaign_context.py` & `bemserver-ui-0.5.3/bemserver_ui/extensions/campaign_context.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/extensions/error_handlers.py` & `bemserver-ui-0.5.3/bemserver_ui/extensions/error_handlers.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/extensions/flask_es6.py` & `bemserver-ui-0.5.3/bemserver_ui/extensions/flask_es6.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/extensions/jinja_custom_filters.py` & `bemserver-ui-0.5.3/bemserver_ui/extensions/jinja_custom_filters.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/extensions/partners.py` & `bemserver-ui-0.5.3/bemserver_ui/extensions/partners.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/extensions/plugins.py` & `bemserver-ui-0.5.3/bemserver_ui/extensions/plugins.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/extensions/timezones/__init__.py` & `bemserver-ui-0.5.3/bemserver_ui/extensions/timezones/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/extensions/timezones/timezones-areas.json` & `bemserver-ui-0.5.3/bemserver_ui/extensions/timezones/timezones-areas.json`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/extensions/timezones/timezones-full.json` & `bemserver-ui-0.5.3/bemserver_ui/extensions/timezones/timezones-full.json`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/extensions/timezones/timezones.py` & `bemserver-ui-0.5.3/bemserver_ui/extensions/timezones/timezones.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/internal_api/__init__.py` & `bemserver-ui-0.5.3/bemserver_ui/internal_api/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/internal_api/analysis/completeness.py` & `bemserver-ui-0.5.3/bemserver_ui/internal_api/analysis/completeness.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/internal_api/analysis/degree_days.py` & `bemserver-ui-0.5.3/bemserver_ui/internal_api/analysis/degree_days.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/internal_api/analysis/energy_consumption.py` & `bemserver-ui-0.5.3/bemserver_ui/internal_api/analysis/energy_consumption.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/internal_api/campaign_scopes.py` & `bemserver-ui-0.5.3/bemserver_ui/internal_api/campaign_scopes.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/internal_api/campaigns.py` & `bemserver-ui-0.5.3/bemserver_ui/internal_api/campaigns.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/internal_api/events.py` & `bemserver-ui-0.5.3/bemserver_ui/internal_api/events.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/internal_api/notifications.py` & `bemserver-ui-0.5.3/bemserver_ui/internal_api/notifications.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/internal_api/semantics/energy/__init__.py` & `bemserver-ui-0.5.3/bemserver_ui/internal_api/semantics/energy/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/internal_api/semantics/energy/consumption.py` & `bemserver-ui-0.5.3/bemserver_ui/internal_api/semantics/energy/consumption.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/internal_api/semantics/energy/production.py` & `bemserver-ui-0.5.3/bemserver_ui/internal_api/semantics/energy/production.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/internal_api/semantics/weather.py` & `bemserver-ui-0.5.3/bemserver_ui/internal_api/semantics/weather.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/internal_api/services/cleanup.py` & `bemserver-ui-0.5.3/bemserver_ui/internal_api/services/cleanup.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/internal_api/services/missing_data.py` & `bemserver-ui-0.5.3/bemserver_ui/internal_api/services/missing_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/internal_api/services/outlier_data.py` & `bemserver-ui-0.5.3/bemserver_ui/internal_api/services/outlier_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/internal_api/services/weather_data.py` & `bemserver-ui-0.5.3/bemserver_ui/internal_api/services/weather_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/internal_api/structural_elements.py` & `bemserver-ui-0.5.3/bemserver_ui/internal_api/structural_elements.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/internal_api/timeseries/data.py` & `bemserver-ui-0.5.3/bemserver_ui/internal_api/timeseries/data.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from bemserver_api_client.enums import DataFormat, Aggregation, BucketWidthUnit
 from bemserver_ui.extensions import auth, ensure_campaign_context
 from bemserver_ui.common.time import (
     convert_html_form_datetime,
     convert_from_iso,
     strfdelta,
+    add_time,
 )
 from bemserver_ui.common.exceptions import BEMServerUICommonInvalidDatetimeError
 
 
 blp = flask.Blueprint("data", __name__, url_prefix="/data")
 
 
@@ -169,14 +170,80 @@
             "ts_datastate_name": ts_datastate_resp.data["name"],
             "ts_start_time": start_time,
             "ts_end_time": end_time,
         }
     )
 
 
+@blp.route("/retrieve_data_json")
+@auth.signin_required
+@ensure_campaign_context
+def retrieve_multiple_data_json():
+    ts_ids = [int(x) for x in flask.request.args["timeseries"].split(",")]
+    data_state_id = flask.request.args["data_state"]
+    tz_name = flask.request.args["timezone"]
+    period = flask.request.args["period"]
+    end_date = flask.request.args["end_date"]
+    end_time = flask.request.args.get("end_time", "00:00") or "00:00"
+    aggregation = flask.request.args.get("agg")
+    if aggregation == "none":
+        aggregation = None
+    bucket_width_value = flask.request.args.get("bucket_width_value")
+    bucket_width_unit = flask.request.args.get("bucket_width_unit")
+
+    tz = zoneinfo.ZoneInfo(tz_name)
+    try:
+        dt_end = convert_html_form_datetime(end_date, end_time, tz=tz)
+    except BEMServerUICommonInvalidDatetimeError:
+        flask.abort(422, description="Invalid end datetime!")
+
+    if period == "custom":
+        start_date = flask.request.args["start_date"]
+        start_time = flask.request.args.get("start_time", "00:00") or "00:00"
+        try:
+            dt_start = convert_html_form_datetime(start_date, start_time, tz=tz)
+        except BEMServerUICommonInvalidDatetimeError:
+            flask.abort(422, description="Invalid start datetime!")
+    else:
+        if period == "last-24-hours":
+            dt_start = dt_end - dt.timedelta(hours=24)
+        elif period == "last-7-days":
+            dt_start = dt_end - dt.timedelta(days=7)
+        elif period == "last-30-days":
+            dt_start = dt_end - dt.timedelta(days=30)
+        elif period == "last-12-months":
+            dt_start = add_time(dt_end, years=-1)
+
+    if (
+        aggregation is not None
+        and bucket_width_value is not None
+        and bucket_width_unit is not None
+    ):
+        ts_data_resp = flask.g.api_client.timeseries_data.download_aggregate(
+            dt_start.isoformat(),
+            dt_end.isoformat(),
+            data_state_id,
+            ts_ids,
+            timezone=tz_name,
+            aggregation=Aggregation(aggregation),
+            bucket_width_value=bucket_width_value,
+            bucket_width_unit=BucketWidthUnit(bucket_width_unit),
+        )
+    else:
+        ts_data_resp = flask.g.api_client.timeseries_data.download(
+            dt_start.isoformat(),
+            dt_end.isoformat(),
+            data_state_id,
+            ts_ids,
+            timezone=tz_name,
+        )
+
+    return flask.jsonify(ts_data_resp.data)
+
+
 @blp.route("/delete_data", methods=["POST"])
 @auth.signin_required
 @ensure_campaign_context
 def delete_data():
     tz_name = flask.request.json["timezone"]
     tz = zoneinfo.ZoneInfo(tz_name)
```

### Comparing `bemserver-ui-0.5.2/bemserver_ui/internal_api/timeseries/timeseries.py` & `bemserver-ui-0.5.3/bemserver_ui/internal_api/timeseries/timeseries.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/internal_api/user_groups.py` & `bemserver-ui-0.5.3/bemserver_ui/internal_api/user_groups.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/internal_api/users.py` & `bemserver-ui-0.5.3/bemserver_ui/internal_api/users.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/images/bemserver-ico.svg` & `bemserver-ui-0.5.3/bemserver_ui/static/images/bemserver-ico.svg`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/images/bemserver-min.svg` & `bemserver-ui-0.5.3/bemserver_ui/static/images/bemserver-min.svg`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/images/bemserver.ico` & `bemserver-ui-0.5.3/bemserver_ui/static/images/bemserver.ico`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/images/bemserver.svg` & `bemserver-ui-0.5.3/bemserver_ui/static/images/bemserver.svg`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/app.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/app.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/accordionList.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/accordionList.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/charts/tsChartCompleteness.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/charts/tsChartCompleteness.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/charts/tsChartDegreeDays.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/charts/tsChartDegreeDays.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/charts/tsChartEnergyConsumption.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/charts/tsChartEnergyConsumption.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/charts/tsChartExplore.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/charts/tsChartWeather.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,73 +1,58 @@
 import "https://cdn.jsdelivr.net/npm/echarts@5.4.1/dist/echarts.min.js";
 import {
     Parser
 } from "../../tools/parser.js";
-import {
-    TimeDisplay
-} from "../../tools/time.js";
 
 
-export class TimeseriesChartExplore extends HTMLDivElement {
+export class TimeseriesChartWeather extends HTMLDivElement {
 
     #chart = null;
 
     #initOptions = {
         height: 500,
+        width: "auto",
     };
     #theme = null;
 
-    #downloadCSVUrl = null;
-
-    #defaultTitle = "Timeseries data";
     #defaultOptions = {
         title: {
             left: "center",
-            text: this.#defaultTitle,
-            subtextStyle: {
-                fontSize: 14,
-            },
+            text: "",
         },
         grid: {
-            left: "5%",
+            left: "3%",
             right: "5%",
-            bottom: 100,
+            bottom: 90,
             containLabel: true,
         },
         toolbox: {
             feature: {
-                magicType: {
-                    type: ["line", "bar"],
-                    show: false,
+                myTSInfo: {
+                    show: true,
+                    title: "Weather parameters timeseries",
+                    icon: "path://M 12 2 C 6.4771525 2 2 6.4771525 2 12 C 2 17.522847 6.4771525 22 12 22 C 17.522847 22 22 17.522847 22 12 C 22 6.4771525 17.522847 2 12 2 z M 12 4 C 16.418278 4 20 7.581722 20 12 C 20 16.418278 16.418278 20 12 20 C 7.581722 20 4 16.418278 4 12 C 4 7.581722 7.581722 4 12 4 z M 11 6 L 11 8 L 13 8 L 13 6 L 11 6 z M 11 9 L 11 17 L 13 17 L 13 9 L 11 9 z",
+                    onclick: function() {
+                        this.#showTSInfo();
+                    },
                 },
                 dataZoom: {
                     yAxisIndex: "none",
                 },
                 dataView: {
                     readOnly: true,
                     buttonColor: "#95c11a",
                 },
                 saveAsImage: {},
-                myDownloadCSV: {
-                    show: false,
-                    title: "Download as CSV",
-                    icon: `image://data:image/svg+xml,
-<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-filetype-csv" viewBox="0 0 16 16">
-    <path fill-rule="evenodd" d="M14 4.5V14a2 2 0 0 1-2 2h-1v-1h1a1 1 0 0 0 1-1V4.5h-2A1.5 1.5 0 0 1 9.5 3V1H4a1 1 0 0 0-1 1v9H2V2a2 2 0 0 1 2-2h5.5L14 4.5ZM3.517 14.841a1.13 1.13 0 0 0 .401.823c.13.108.289.192.478.252.19.061.411.091.665.091.338 0 .624-.053.859-.158.236-.105.416-.252.539-.44.125-.189.187-.408.187-.656 0-.224-.045-.41-.134-.56a1.001 1.001 0 0 0-.375-.357 2.027 2.027 0 0 0-.566-.21l-.621-.144a.97.97 0 0 1-.404-.176.37.37 0 0 1-.144-.299c0-.156.062-.284.185-.384.125-.101.296-.152.512-.152.143 0 .266.023.37.068a.624.624 0 0 1 .246.181.56.56 0 0 1 .12.258h.75a1.092 1.092 0 0 0-.2-.566 1.21 1.21 0 0 0-.5-.41 1.813 1.813 0 0 0-.78-.152c-.293 0-.551.05-.776.15-.225.099-.4.24-.527.421-.127.182-.19.395-.19.639 0 .201.04.376.122.524.082.149.2.27.352.367.152.095.332.167.539.213l.618.144c.207.049.361.113.463.193a.387.387 0 0 1 .152.326.505.505 0 0 1-.085.29.559.559 0 0 1-.255.193c-.111.047-.249.07-.413.07-.117 0-.223-.013-.32-.04a.838.838 0 0 1-.248-.115.578.578 0 0 1-.255-.384h-.765ZM.806 13.693c0-.248.034-.46.102-.633a.868.868 0 0 1 .302-.399.814.814 0 0 1 .475-.137c.15 0 .283.032.398.097a.7.7 0 0 1 .272.26.85.85 0 0 1 .12.381h.765v-.072a1.33 1.33 0 0 0-.466-.964 1.441 1.441 0 0 0-.489-.272 1.838 1.838 0 0 0-.606-.097c-.356 0-.66.074-.911.223-.25.148-.44.359-.572.632-.13.274-.196.6-.196.979v.498c0 .379.064.704.193.976.131.271.322.48.572.626.25.145.554.217.914.217.293 0 .554-.055.785-.164.23-.11.414-.26.55-.454a1.27 1.27 0 0 0 .226-.674v-.076h-.764a.799.799 0 0 1-.118.363.7.7 0 0 1-.272.25.874.874 0 0 1-.401.087.845.845 0 0 1-.478-.132.833.833 0 0 1-.299-.392 1.699 1.699 0 0 1-.102-.627v-.495Zm8.239 2.238h-.953l-1.338-3.999h.917l.896 3.138h.038l.888-3.138h.879l-1.327 4Z"/>
-</svg>`,
-                    onclick: () => {
-                        this.#downloadCSV();
-                    },
-                },
             },
         },
         tooltip: {
             trigger: "axis",
             axisPointer: {
-                type: "cross",
+                type: "shadow",
             },
         },
         legend: [{
             data: [],
             width: "45%",
             bottom: 0,
             left: 0,
@@ -85,41 +70,37 @@
         }, ],
         xAxis: [{
             type: "time",
         }, ],
         yAxis: [{
             type: "value",
             nameLocation: "middle",
+            axisLabel: {},
             position: "left",
         }, {
             type: "value",
             nameLocation: "middle",
+            axisLabel: {},
             position: "right",
         }, ],
         series: [],
         useUTC: false,
     };
 
-    #colors = [
-        '#5470c6',
-        '#91cc75',
-        '#fac858',
-        '#ee6666',
-        '#73c0de',
-        '#3ba272',
-        '#fc8452',
-        '#9a60b4',
-        '#ea7ccc'
-    ];
-
-    get colors() {
-        return this.#colors;
-    }
+    #energyUseColors = {
+        "Air temperature": "#0880A4",
+        "Relative humidity": "#7C4F00",
+        "Direct normal solar radiation": "#EF1919",
+        "Surface solar radiation": "#E38028",
+        "Air temperature forecast": "#0880A4",
+        "Relative humidity forecast": "#7C4F00",
+        "Direct normal solar radiation forecast": "#EF1919",
+        "Surface solar radiation forecast": "#E38028",
+    };
 
-    // `theme` parameter can be "dark"
     constructor(options = null, theme = null) {
         super();
 
         this.#initOptions = options || this.#initOptions;
         this.#theme = theme;
     }
 
@@ -129,30 +110,21 @@
         });
 
         window.addEventListener("unload", (event) => {
             this.dispose();
         });
     }
 
-    connectedCallback() {
-        this.#chart = echarts.init(this, this.#theme, this.#initOptions);
-        this.#chart.setOption(this.#defaultOptions);
-
-        this.#initEventListeners();
+    #showTSInfo(tsInfoCallback = null) {
+        tsInfoCallback?.();
     }
 
-    #optionToContent(opt, units, timeFormat, tzName) {
+    #optionToContent(opt, dataset, timeFormat) {
         let timestamps = opt.series[0].data.map((serieData) => {
-            if (timeFormat != null) {
-                return echarts.time.format(serieData[0], timeFormat);
-            } else {
-                return TimeDisplay.toLocaleString(new Date(serieData[0]), {
-                    timezone: tzName
-                });
-            }
+            return echarts.time.format(serieData[0], timeFormat);
         });
 
         let mainContainerElmt = document.createElement("div");
         mainContainerElmt.classList.add("m-2", "me-3");
 
         let subtitleElmt = document.createElement("h5");
         subtitleElmt.innerText = opt.title[0].subtext;
@@ -170,61 +142,55 @@
         let tableHeadElmt = document.createElement("thead");
         let tableHeadTrElmt = document.createElement("tr");
         tableHeadTrElmt.classList.add("align-middle");
         let tableHeadTimestampElmt = document.createElement("th");
         tableHeadTimestampElmt.setAttribute("scope", "col");
         tableHeadTimestampElmt.innerText = "Timestamp";
         tableHeadTrElmt.appendChild(tableHeadTimestampElmt);
-        for (let [index, serie] of opt.series.entries()) {
+        for (let serie of opt.series) {
             let tableHeadThElmt = document.createElement("th");
             tableHeadThElmt.setAttribute("scope", "col");
-            if (units != null) {
-                tableHeadThElmt.innerText = `${serie.name}${units[index] ? ` (${units[index]})`: ""}`;
-            }
+            tableHeadThElmt.innerText = serie.name + (serie.unit ? ` (${serie.unit})` : "");
             tableHeadTrElmt.appendChild(tableHeadThElmt);
         }
         tableHeadElmt.appendChild(tableHeadTrElmt);
         tableElmt.appendChild(tableHeadElmt);
         let tableBodyElmt = document.createElement("tbody");
         tableBodyElmt.classList.add("table-group-divider");
         for (let [index, timestamp] of timestamps.entries()) {
             let tableTrElmt = document.createElement("tr");
             let tableCellTimestampElmt = document.createElement("td");
             tableCellTimestampElmt.innerText = timestamp;
             tableTrElmt.appendChild(tableCellTimestampElmt);
             for (let serie of opt.series) {
-                let tableCellElmt = document.createElement("td");
-                tableCellElmt.innerText = Parser.parseFloatOrDefault(serie.data[index][1], Number.NaN, 2);
-                tableTrElmt.appendChild(tableCellElmt);
+                if (serie.data && serie.data[index]) {
+                    let tableCellElmt = document.createElement("td");
+                    tableCellElmt.innerText = serie.data[index][1].toString();
+                    tableTrElmt.appendChild(tableCellElmt);
+                }
             }
             tableBodyElmt.appendChild(tableTrElmt);
         }
         tableElmt.appendChild(tableBodyElmt);
 
         tableContainerElmt.appendChild(tableElmt);
         mainContainerElmt.appendChild(tableContainerElmt);
         return mainContainerElmt;
     }
 
-    #tooltipFormatter(params, units, timeFormat, tzName) {
+    #tooltipFormatter(params, dataset, timeFormat) {
         let tooltipContainerElmt = document.createElement("div");
 
         let ulElmt = document.createElement("ul");
         ulElmt.classList.add("list-unstyled", "mx-2", "mt-2", "mb-0");
 
         for (let [index, serieParams] of params.entries()) {
             if (index == 0) {
                 let timeElmt = document.createElement("h6");
-                if (timeFormat != null) {
-                    timeElmt.innerText = echarts.time.format(serieParams.value[0], timeFormat);
-                } else {
-                    timeElmt.innerText = TimeDisplay.toLocaleString(new Date(serieParams.value[0]), {
-                        timezone: tzName
-                    });
-                }
+                timeElmt.innerText = echarts.time.format(serieParams.value[0], timeFormat);
                 tooltipContainerElmt.appendChild(timeElmt);
             }
 
             let liElmt = document.createElement("li");
             liElmt.classList.add("d-flex", "justify-content-between", "gap-4");
             ulElmt.appendChild(liElmt);
 
@@ -236,34 +202,37 @@
             serieValueContainerElmt.classList.add("d-flex", "gap-1");
 
             let serieValueElmt = document.createElement("span");
             serieValueElmt.classList.add("fw-bold");
             serieValueElmt.innerText = Parser.parseFloatOrDefault(serieParams.value[1], Number.NaN, 2).toString();
             serieValueContainerElmt.appendChild(serieValueElmt);
 
-            if (units != null) {
-                let serieValueUnitElmt = document.createElement("small");
-                serieValueUnitElmt.innerText = units[index];
-                serieValueContainerElmt.appendChild(serieValueUnitElmt);
+            let serieValueUnitElmt = document.createElement("small");
+            for (let [key, value] of Object.entries(dataset)) {
+                for (let [key2, value2] of Object.entries(value)) {
+                    if (value2.name == serieParams.seriesName) {
+                        serieValueUnitElmt.innerText = value2.timeseries.unit_symbol;
+                    }
+                }
             }
+            serieValueContainerElmt.appendChild(serieValueUnitElmt);
 
             liElmt.appendChild(serieNameElmt);
             liElmt.appendChild(serieValueContainerElmt);
         }
 
         tooltipContainerElmt.appendChild(ulElmt);
         return tooltipContainerElmt;
     }
 
-    #downloadCSV() {
-        if (this.#downloadCSVUrl != null) {
-            let link = document.createElement("a");
-            link.setAttribute("href", this.#downloadCSVUrl);
-            link.click();
-        }
+    connectedCallback() {
+        this.#chart = echarts.init(this, this.#theme, this.#initOptions);
+        this.#chart.setOption(this.#defaultOptions);
+
+        this.#initEventListeners();
     }
 
     resize() {
         this.#chart.resize();
     }
 
     dispose() {
@@ -274,103 +243,104 @@
         this.#chart.showLoading();
     }
 
     hideLoading() {
         this.#chart.hideLoading();
     }
 
-    load(data, parameters) {
+    load(name, dataset, timeFormat, tsInfoCallback = null) {
         this.hideLoading();
-        let listUnit = [];
-        let listDistinctUnitByAxis = {
+
+        let options = this.#chart.getOption();
+        let listUnit = {
             0: [],
-            1: [],
+            1: []
         };
-        let yAxisIndex = 0;
-        let options = this.#chart.getOption();
+
         options.legend[0].data = [];
         options.legend[1].data = [];
 
-        options.title[0].subtext = parameters.subtitle;
-        options.toolbox[0].feature.dataView.lang[0] = this.#defaultTitle;
+        options.title[0].text = `${name}`;
+
+        options.toolbox[0].feature.dataView.optionToContent = (opt) => {
+            return this.#optionToContent(opt, dataset, timeFormat);
+        };
+
+        options.toolbox[0].feature.myTSInfo.onclick = () => {
+            this.#showTSInfo(tsInfoCallback);
+        };
+
+        options.tooltip[0].formatter = (params) => {
+            return this.#tooltipFormatter(params, dataset, timeFormat);
+        };
 
         options.series.length = 0;
-        options.series = data.ts_headers.filter((header) => {
-            return header != "Datetime";
-        }).map((header) => {
-            parameters.series[header]?.position == "right" ? yAxisIndex = 1 : yAxisIndex = 0;
-            yAxisIndex == 0 ? options.legend[0].data.push(header) : options.legend[1].data.push(header);
-
-            let unitSymbol = parameters.series[header]?.symbol;
-            listUnit.push(unitSymbol);
-            if (unitSymbol != null && unitSymbol != "" && !listDistinctUnitByAxis[yAxisIndex].includes(unitSymbol)) {
-                listDistinctUnitByAxis[yAxisIndex].push(unitSymbol);
-            }
 
-            return {
-                id: header,
-                name: header,
-                type: parameters.series[header]?.type || "line",
-                color: parameters.series[header]?.color || "#000000",
-                lineStyle: {
-                    width: 2,
-                    type: parameters.series[header]?.style || "solid",
-                },
-                yAxisIndex: yAxisIndex,
-                smooth: true,
-                data: data.ts_data.map((row) => {
-                    return [row["Datetime"], Parser.parseFloatOrDefault(row[header], Number.NaN, 2)];
-                }),
-            };
-        });
+        let series = [];
+        for (let [_parameter, serieParams] of Object.entries(dataset)) {
+            for (let [_settings, value] of Object.entries(serieParams)) {
+                let chartData = Object.entries(value.data).map(([date, value]) => [date, Parser.parseFloatOrDefault(value, Number.NaN, 2)]);
+                if (chartData.length > 0) {
+                    let serie = {
+                        name: value.name,
+                        type: "line",
+                        data: Object.entries(value.data).map(([date, value]) => [date, Parser.parseFloatOrDefault(value, Number.NaN, 2)]),
+                        emphasis: {
+                            focus: "series"
+                        },
+                        itemStyle: {
+                            color: this.#energyUseColors[value.name]
+                        },
+                        lineStyle: {
+                            width: 2,
+                            type: value.name.includes("forecast") ? "dashed" : "solid",
+                        },
+                        yAxisIndex: value.yAxis,
+                        unit: value.timeseries.unit_symbol,
+                    };
+                    series.push(serie);
+                    if (!listUnit[value.yAxis].includes(serie.unit))
+                        listUnit[value.yAxis].push(serie.unit);
 
-        // Set distinct unit symbols as (left and right) Y-axis name.
-        options.yAxis[0].name = listDistinctUnitByAxis[0].join(", ");
-        options.yAxis[0].nameLocation = "middle";
-        options.yAxis[0].nameGap = 50;
-        options.yAxis[1].name = listDistinctUnitByAxis[1].join(", ");
-        options.yAxis[1].nameLocation = "middle";
-        options.yAxis[1].nameGap = 50;
+                    options.legend[value.yAxis].data.push(value.name);
+                }
+            }
+        }
+        options.series = series;
 
-        options.toolbox[0].feature.dataView.optionToContent = (opt) => {
-            return this.#optionToContent(opt, listUnit, null, parameters.timezone);
+        options.yAxis[0].data = options.series.map((serie) => serie.name);
+        options.yAxis[0].axisLabel.formatter = (value, index) => {
+            return `${value} (${listUnit[0]})`;
         };
-        options.tooltip[0].formatter = (params) => {
-            return this.#tooltipFormatter(params, listUnit, null, parameters.timezone);
+
+        options.yAxis[1].data = options.series.map((serie) => serie.name);
+        options.yAxis[1].axisLabel.formatter = (value, index) => {
+            return `${value} (${listUnit[1]})`;
+        };
+
+        if (options.legend[1].data.length == 0) {
+            options.legend[0].left = "center";
+            options.legend[0].width = "auto";
         };
 
         options.legend[0].formatter = (name) => {
-            return name + " [" + parameters.series[name]?.symbol + "] ";
+            let serie = options.series.find((serie) => serie.name == name);
+            return `${name} (${serie.unit})`;
         };
+
         options.legend[1].formatter = (name) => {
-            return name + " [" + parameters.series[name]?.symbol + "] ";
+            let serie = options.series.find((serie) => serie.name == name);
+            return `${name} (${serie.unit})`;
         };
 
         // Fix for bug, see: https://github.com/apache/incubator-echarts/issues/6202
         this.#chart.clear();
 
         this.#chart.setOption(options);
     }
-
-    setDownloadCSVLink(url) {
-        this.#downloadCSVUrl = url;
-
-        let options = this.#chart.getOption();
-        options.toolbox[0].feature.myDownloadCSV.show = true;
-        this.#chart.setOption(options);
-    }
-
-    removeDownloadCSVLink() {
-        this.#downloadCSVUrl = null;
-
-        let options = this.#chart.getOption();
-        options.toolbox[0].feature.myDownloadCSV.show = false;
-        this.#chart.setOption(options);
-    }
 }
 
-
-if (window.customElements.get("app-ts-chart-explore") == null) {
-    window.customElements.define("app-ts-chart-explore", TimeseriesChartExplore, {
+if (window.customElements.get("app-ts-chart-weather") == null) {
+    window.customElements.define("app-ts-chart-weather", TimeseriesChartWeather, {
         extends: "div"
     });
 }
```

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/dropZone.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/dropZone.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/eventLevel.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/eventLevel.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/filterSelect.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/filterSelect.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/flash.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/flash.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/itemsCount.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/itemsCount.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/modalConfirm.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/modalConfirm.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/pagination.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/pagination.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/structuralElements/selector.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/structuralElements/selector.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/time/datetimePicker.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/time/datetimePicker.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,18 @@
 import {
     Parser
-} from "../../tools/parser.js";
+} from "/static/scripts/modules/tools/parser.js";
 import {
     TimezoneTool
-} from "../../tools/timezones.js";
+} from "/static/scripts/modules/tools/timezones.js";
 
 
 export class DatetimePicker extends HTMLDivElement {
 
+    #initOptions = {};
     #tzTool = null;
 
     #titleSpanElmt = null;
     #dateInputElmt = null;
     #timeInputElmt = null;
     #tzInfoElmt = null;
     #dateInputFormBindElmt = null;
@@ -29,20 +30,25 @@
 
     #date = null;
     #time = null;
 
     constructor(options = {}) {
         super();
 
+        this.#initOptions = options;
         this.#tzTool = new TimezoneTool();
 
         this.#loadOptions(options);
         this.#cacheDOM();
     }
 
+    static get observedAttributes() {
+        return ["disabled", "required"];
+    }
+
     get date() {
         return this.#date;
     }
 
     get time() {
         return this.#time;
     }
@@ -199,55 +205,78 @@
         if (this.#timeInputFormBindElmt != null) {
             this.#timeInputFormBindElmt.value = this.#time;
         }
     }
 
     #updateTzInfo() {
         let tzInfo = this.#tzTool.getTzInfo(this.#tzName);
-        this.#tzInfoElmt.setAttribute("title", `<div class="d-grid"><span class="fw-bold">${tzInfo["area"]["label"]}</span><span class="fst-italic">${tzInfo["label"]}</span></div>`);
+
+        let tzInfoTitleContentElmt = document.createElement("div");
+        tzInfoTitleContentElmt.classList.add("d-grid");
+        let tzInfoAreaLabelElmt = document.createElement("span");
+        tzInfoAreaLabelElmt.classList.add("fw-bold");
+        tzInfoAreaLabelElmt.innerText = tzInfo["area"]["label"];
+        tzInfoTitleContentElmt.appendChild(tzInfoAreaLabelElmt);
+        let tzInfoLabelElmt = document.createElement("span");
+        tzInfoLabelElmt.classList.add("fst-italic");
+        tzInfoLabelElmt.innerText = tzInfo["label"];
+        tzInfoTitleContentElmt.appendChild(tzInfoLabelElmt);
+
+        this.#tzInfoElmt.setAttribute("title", tzInfoTitleContentElmt.outerHTML);
         this.#enableOrRefreshTooltips();
     }
 
     #enableOrRefreshTooltips() {
         // Enable (or refresh) Bootstrap tooltips.
         var tooltipTriggerList = [].slice.call(this.querySelectorAll(`[data-bs-toggle="tooltip"]`));
         tooltipTriggerList.map((tooltipTriggerEl) => {
             return new bootstrap.Tooltip(tooltipTriggerEl);
         });
     }
 
     connectedCallback() {
+        this.#loadOptions(this.#initOptions);
+
         this.innerHTML = "";
         this.classList.add("input-group", "input-group-sm");
+        this.style.minWidth = "230px";
 
         if (this.#title != null) {
             this.#titleSpanElmt = document.createElement("span");
             this.#titleSpanElmt.classList.add("input-group-text");
             this.#titleSpanElmt.innerText = this.#title;
             this.appendChild(this.#titleSpanElmt);
         }
 
         this.#dateInputElmt = document.createElement("input");
         this.#dateInputElmt.classList.add("form-control");
         this.#dateInputElmt.type = "date";
-        if (this.#isRequired) {
-            this.#dateInputElmt.setAttribute("required", true);
-        }
         if (this.#hasAutofocus) {
             this.#dateInputElmt.setAttribute("autofocus", true);
         }
+        if (this.#dateMin != null) {
+            this.#dateInputElmt.setAttribute("min", this.#dateMin);
+        }
+        if (this.#dateMax != null) {
+            this.#dateInputElmt.setAttribute("max", this.#dateMax);
+        }
+        this.#dateInputElmt.style.minWidth = "125px";
         this.appendChild(this.#dateInputElmt);
 
         this.#timeInputElmt = document.createElement("input");
         this.#timeInputElmt.classList.add("form-control");
         this.#timeInputElmt.type = "time";
+        this.#timeInputElmt.style.minWidth = "75px";
+        this.appendChild(this.#timeInputElmt);
+
         if (this.#isRequired) {
-            this.#timeInputElmt.setAttribute("required", true);
+            this.setRequired();
+        } else {
+            this.setOptional();
         }
-        this.appendChild(this.#timeInputElmt);
 
         this.#tzInfoElmt = document.createElement("i");
         this.#tzInfoElmt.classList.add("input-group-text", "bi", "bi-watch");
         this.#tzInfoElmt.setAttribute("data-bs-toggle", "tooltip");
         this.#tzInfoElmt.setAttribute("data-bs-html", true);
         this.appendChild(this.#tzInfoElmt);
 
@@ -255,14 +284,50 @@
         this.#updateDateAndTime();
         this.#updateTzInfo();
         this.#updateStyle();
 
         this.#initEventListeners();
     }
 
+    attributeChangedCallback(name, oldValue, newValue) {
+        if (oldValue != newValue) {
+            if (name == "disabled") {
+                if (newValue) {
+                    this.setDisabled();
+                } else {
+                    this.setEnabled();
+                }
+            } else if (name == "required") {
+                if (newValue) {
+                    this.setRequired();
+                } else {
+                    this.setOptional();
+                }
+            }
+        }
+    }
+
+    setEnabled() {
+        this.#dateInputElmt.removeAttribute("disabled");
+        this.#timeInputElmt.removeAttribute("disabled");
+    }
+    setDisabled() {
+        this.#dateInputElmt.setAttribute("disabled", true);
+        this.#timeInputElmt.setAttribute("disabled", true);
+    }
+
+    setRequired() {
+        this.#dateInputElmt.setAttribute("required", true);
+        this.#timeInputElmt.setAttribute("required", true);
+    }
+    setOptional() {
+        this.#dateInputElmt.removeAttribute("required");
+        this.#timeInputElmt.removeAttribute("required");
+    }
+
     focus(options = {
         focusOnTime: false
     }) {
         if (options.focusOnTime) {
             this.#timeInputElmt.focus();
         } else {
             this.#dateInputElmt.focus();
```

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/time/tzPicker.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/time/tzPicker.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/timeseries/bucketWidth.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/timeseries/bucketWidth.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,21 @@
 import {
     Parser
-} from "../../tools/parser.js";
+} from "/static/scripts/modules/tools/parser.js";
 
 
-const DURATIONS = {
+const DURATIONS = Object.freeze({
     "year": [1],
     "month": [1],
     "week": [1],
     "day": [1],
     "hour": [1, 2, 3, 4, 6, 8, 12],
     "minute": [1, 2, 3, 4, 5, 6, 10, 12, 15, 20, 30],
     "second": [1, 2, 3, 4, 5, 6, 10, 12, 15, 20, 30],
-};
+});
 
 
 export class TimeseriesBucketWidth extends HTMLDivElement {
 
     #title = null;
     #widthUnit = null;
     #widthValue = null;
@@ -25,17 +25,33 @@
 
     #selectElmt = null;
 
 
     get bucketWidthUnit() {
         return this.#widthUnit;
     }
+    set bucketWidthUnit(value) {
+        if (value != this.#widthUnit && Object.keys(DURATIONS).includes(value)) {
+            this.#widthUnit = value;
+            if (!DURATIONS[this.#widthUnit].includes(this.#widthValue)) {
+                this.#widthValue = DURATIONS[this.#widthUnit][0];
+            }
+            this.#selectElmt.value = `${this.#widthValue}_${this.#widthUnit}`;
+        }
+    }
+
     get bucketWidthValue() {
         return this.#widthValue;
     }
+    set bucketWidthValue(value) {
+        if (value != this.#widthValue && DURATIONS[this.#widthUnit].includes(value)) {
+            this.#widthValue = value;
+            this.#selectElmt.value = `${this.#widthValue}_${this.#widthUnit}`;
+        }
+    }
 
     static get observedAttributes() {
         return ["disabled"];
     }
 
 
     constructor(options = {}) {
@@ -120,12 +136,12 @@
             this.#widthValue = Parser.parseIntOrDefault(optParts[0], this.#defaultWidthValue);
             this.#widthUnit = optParts[1];
         });
     }
 }
 
 
-if (customElements.get("app-ts-bucket-width") == null) {
-    customElements.define("app-ts-bucket-width", TimeseriesBucketWidth, {
+if (window.customElements.get("app-ts-bucket-width") == null) {
+    window.customElements.define("app-ts-bucket-width", TimeseriesBucketWidth, {
         extends: "div"
     });
 }
```

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/timeseries/selector.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/timeseries/selector.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -241,14 +241,15 @@
     #selectReqID = null;
     #sitesTreeReqID = null;
     #zonesTreeReqID = null;
 
     #messagesElmt = null;
 
     #selectedItemsContainerElmt = null;
+    #clearSelectionBtnElmt = null;
     #selectedItems = [];
     #dropdownSearchPanelElmt = null;
     #bsDropdownSearchPanel = null;
 
     #searchInputElmt = null;
 
     #searchClearBtnElmt = null;
@@ -307,14 +308,15 @@
         }
     }
 
     #cacheDOM() {
         this.#messagesElmt = document.getElementById("messages");
 
         this.#selectedItemsContainerElmt = document.getElementById("selectedItemsContainer");
+        this.#clearSelectionBtnElmt = this.querySelector("#clearSelectionBtn");
         this.#dropdownSearchPanelElmt = document.getElementById("dropdownSearchPanel");
         this.#bsDropdownSearchPanel = bootstrap.Dropdown.getOrCreateInstance(this.#dropdownSearchPanelElmt);
 
         this.#searchInputElmt = document.getElementById("search");
 
         this.#searchClearBtnElmt = document.getElementById("clearSearchBtn");
         this.#filtersRemoveBtnElmt = document.getElementById("removeFiltersBtn");
@@ -334,14 +336,20 @@
         this.#countResultsSelectedElmt = document.getElementById("countResultsSelected");
         this.#selectAllResultsBtnElmt = document.getElementById("selectAllResultsBtn");
         this.#unselectAllResultsBtnElmt = document.getElementById("unselectAllResultsBtn");
         this.#clearAllSelectionBtnElmt = document.getElementById("clearAllSelectionBtn");
     }
 
     #initEventListeners() {
+        this.#clearSelectionBtnElmt.addEventListener("click", (event) => {
+            event.preventDefault();
+
+            this.clearAllSelection();
+        });
+
         this.#searchInputElmt.addEventListener("input", (event) => {
             event.preventDefault();
 
             this.#updateSearchInput();
             this.#searchResultsPaginationElmt.page = 1;
             this.refresh();
         });
@@ -463,14 +471,18 @@
 
         this.#siteSelectorRecursiveSwitchElmt.addEventListener("change", () => {
             if (this.#siteSelector.selectedData != null) {
                 this.#searchResultsPaginationElmt.page = 1;
                 this.refresh();
             }
         });
+
+        this.#dropdownSearchPanelElmt.addEventListener("shown.bs.dropdown", () => {
+            this.#fixDropdownSearchPanelPosition();
+        });
     }
 
     #updateSearchInput() {
         if (this.#searchInputElmt.value == "") {
             this.#searchInputElmt.classList.remove("border-info", "bg-info", "bg-opacity-10");
         } else if (!this.#searchInputElmt.classList.contains("border-info")) {
             this.#searchInputElmt.classList.add("border-info", "bg-info", "bg-opacity-10");
@@ -492,19 +504,23 @@
 
         this.#updateSelectedItemsContainer();
     }
 
     #updateSelectedItemsContainer() {
         if (this.#selectedItems.length <= 0) {
             this.#selectedItemsContainerElmt.innerHTML = "";
+
+            this.#clearSelectionBtnElmt.classList.add("d-none", "invisible");
         }
 
         this.#countResultsSelectedElmt.innerText = `No items selected`;
         if (this.#selectedItems.length > 0) {
             this.#countResultsSelectedElmt.innerText = `${this.#selectedItems.length.toString()}${this.#allowedSelectionLimit != -1 ? `/${this.#allowedSelectionLimit.toString()}`: ""} item${this.#selectedItems.length > 1 ? "s" : ""} selected out of ${this.#searchResultsPaginationElmt.totalItems.toString()}`;
+
+            this.#clearSelectionBtnElmt.classList.remove("d-none", "invisible");
         }
 
         if (this.#isSelectionLimitReached()) {
             this.#selectionLimitElmt.classList.replace("text-muted", "text-danger");
             this.#selectAllResultsBtnElmt.setAttribute("disabled", true);
 
             let notSelectedSearchResultElmts = [].slice.call(this.#searchResultsContainerElmt.querySelectorAll(`button:not(.active)`));
@@ -721,27 +737,31 @@
                 this.#updateSelectedItemsContainer();
             }
         });
 
         searchResultItem.addEventListener("toggle", (event) => {
             event.preventDefault();
 
-            // Update dropdown-menu position, taking in account selected items container height.
-            this.#dropdownSearchPanelElmt.style.transform = `translate(0px, ${this.#selectedItemsContainerElmt.offsetHeight + this.#bsDropdownSearchPanel._config.offset[1]}px)`;
+            this.#fixDropdownSearchPanelPosition();
 
             let toggleEvent = new CustomEvent("toggleItem", {
                 detail: event.detail,
                 bubbles: true
             });
             this.dispatchEvent(toggleEvent);
         });
 
         return searchResultItem;
     }
 
+    #fixDropdownSearchPanelPosition() {
+        // Update dropdown-menu position, taking in account selected items container height.
+        this.#dropdownSearchPanelElmt.style.transform = `translate(0px, ${this.#selectedItemsContainerElmt.offsetHeight + this.#bsDropdownSearchPanel._config.offset[1]}px)`;
+    }
+
     connectedCallback() {
         this.#initFilters();
         this.#initEventListeners();
         this.#update();
     }
 
     clearAllSelection() {
@@ -825,14 +845,22 @@
 
         if (needRefresh) {
             this.#searchResultsPaginationElmt.page = 1;
             this.refresh();
         }
     }
 
+    open() {
+        this.#bsDropdownSearchPanel.show();
+    }
+
+    close() {
+        this.#bsDropdownSearchPanel.hide();
+    }
+
     refresh() {
         if (this.#searchReqID != null) {
             this.#internalAPIRequester.abort(this.#searchReqID);
             this.#searchReqID = null;
         }
 
         this.#searchResultsCountElmt.setLoading();
```

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/tree.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/tree.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/components/userGroup/userGroupItem.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/components/userGroup/userGroupItem.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/flashTimer.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/flashTimer.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/formController.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/formController.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,26 +1,51 @@
 import {
     ModalConfirm
 } from "./components/modalConfirm.js";
 
 
+const requiredInputs = [
+    `form input:required`,
+    `form select:required`,
+    `form div[is^="app-"][required]`,
+    `input[form]:required`,
+    `select[form]:required`,
+    `div[is^="app-"][form][required]`,
+];
+
+const minMaxInputs = [
+    `form input[minlength]`,
+    `form input[maxlength]`,
+    `form textarea[minlength]`,
+    `form textarea[maxlength]`,
+    `form input[min]`,
+    `form input[max]`,
+    `input[form][minlength]`,
+    `input[form][maxlength]`,
+    `textarea[form][minlength]`,
+    `textarea[form][maxlength]`,
+    `input[form][min]`,
+    `input[form][max]`,
+];
+
+
 export class FormController {
 
     #confirmFormElmts = null;
     #requiredInputElmts = null;
     #minMaxInputElmts = null;
 
     constructor() {
         this.#cacheDOM();
     }
 
     #cacheDOM() {
         this.#confirmFormElmts = [].slice.call(document.querySelectorAll(`form[data-modal-confirm-message]`));
-        this.#requiredInputElmts = [].slice.call(document.querySelectorAll(`input:required, select:required, div[is^="app-"][required]`));
-        this.#minMaxInputElmts = [].slice.call(document.querySelectorAll(`input[minlength], input[maxlength], textarea[minlength], textarea[maxlength], input[min], input[max]`));
+        this.#requiredInputElmts = [].slice.call(document.querySelectorAll(requiredInputs.join(", ")));
+        this.#minMaxInputElmts = [].slice.call(document.querySelectorAll(minMaxInputs.join(", ")));
     }
 
     #getRequiredLabelElmt() {
         let requiredLabelElmt = document.createElement("small");
         requiredLabelElmt.classList.add("fst-italic", "text-danger", "ms-2", "fade-in");
         requiredLabelElmt.textContent = "* (required)";
         return requiredLabelElmt;
```

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/notifications.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/notifications.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/sidebar.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/sidebar.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/array.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/array.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/fetcher.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/fetcher.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/flaskES6.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/flaskES6.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/parser.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/parser.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/time.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/time.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/tools/uuid.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/tools/uuid.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/analysis/degreeDays.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/analysis/degreeDays.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/analysis/energyConsumption.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/analysis/energyConsumption.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/campaignScopes/manageGroups.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/campaignScopes/manageGroups.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/campaigns/selector.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/campaigns/selector.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/events/edit.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/events/edit.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/events/list.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/events/list.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/notifications/explore.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/notifications/explore.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/notifications/setup.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/notifications/setup.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -263,14 +263,15 @@
 
         let restoreEventCatMenuItemCallback = () => {
             rowElmt.remove();
             delete this.#config[eventCategoryConfigData.category_id];
             this.#availableEventCategoryIds.push(eventCategoryConfigData.category_id);
             this.#addEventCatMenuItemElmt(eventCategoryConfigData.category_id);
             this.#updateAddEventCategorySectionState();
+            this.#updateItemsCount();
         };
 
         // Add a modal confirm component for this item, defining an "ok" callback function to remove it.
         let modalConfirm = new ModalConfirm(eventCategoryConfigData.category_id, `Remove <mark>${eventCategoryConfigData.category_name}</mark> notification setup`, () => {
             if (this.#deleteReqID != null) {
                 this.#internalAPIRequester.abort(this.#deleteReqID);
                 this.#deleteReqID = null;
@@ -312,34 +313,29 @@
             } else {
                 restoreEventCatMenuItemCallback();
             }
         });
 
         this.#configTableBodyElmt.appendChild(rowElmt);
 
-        let totalCount = Object.keys(this.#config).length;
-        this.#itemsCountElmt.update({
-            firstItem: totalCount > 0 ? 1 : 0,
-            lastItem: totalCount,
-            totalCount: totalCount
-        });
+        this.#updateItemsCount();
     }
 
     #addEventCatMenuItemElmt(eventCategoryId) {
         let menuItemLinkElmt = document.createElement("a");
         menuItemLinkElmt.classList.add("dropdown-item");
         menuItemLinkElmt.setAttribute("role", "button");
         menuItemLinkElmt.innerText = this.#eventCategories[eventCategoryId];
 
         let menuItemElmt = document.createElement("li");
         menuItemElmt.appendChild(menuItemLinkElmt);
 
         this.#addEventCategoryMenuElmt.appendChild(menuItemElmt);
 
-        menuItemLinkElmt.addEventListener("click", (event) => {
+        menuItemLinkElmt.addEventListener("click", () => {
             menuItemElmt.remove();
             this.#availableEventCategoryIds = this.#availableEventCategoryIds.filter((availableEventCategoryId) => availableEventCategoryId != eventCategoryId);
 
             this.#config[eventCategoryId] = {
                 category_id: eventCategoryId,
                 category_name: this.#eventCategories[eventCategoryId],
                 notification_level: this.#editedNotificationLevelInputElmt.getAttribute("data-default"),
@@ -354,14 +350,23 @@
         if (this.#availableEventCategoryIds.length <= 0) {
             this.#addEventCategorySectionElmt.classList.add("d-none");
         } else {
             this.#addEventCategorySectionElmt.classList.remove("d-none");
         }
     }
 
+    #updateItemsCount() {
+        let totalCount = Object.keys(this.#config).length;
+        this.#itemsCountElmt.update({
+            firstItem: totalCount > 0 ? 1 : 0,
+            lastItem: totalCount,
+            totalCount: totalCount
+        });
+    }
+
     refresh() {
         this.#configTableBodyElmt.innerHTML = "";
 
         for (let eventCategoryConfigData of Object.values(this.#config)) {
             this.#addEventCategoryFromConfig(eventCategoryConfigData);
         }
```

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/cleanupManage.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/cleanupManage.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/missingData/list.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/missingData/list.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/missingData/manage.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/missingData/manage.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/outlierData/list.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/outlierData/list.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/outlierData/manage.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/outlierData/manage.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/services/weatherData/manage.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/services/weatherData/manage.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -487,15 +487,16 @@
                     if (this.#getSemanticsReqID != null) {
                         this.#internalAPIRequester.abort(this.#getSemanticsReqID);
                         this.#getSemanticsReqID = null;
                     }
 
                     this.#getSemanticsReqID = this.#internalAPIRequester.get(
                         flaskES6.urlFor(`api.semantics.weather.list`, {
-                            site: serviceStateData.site_id
+                            site: serviceStateData.site_id,
+                            forecast: false
                         }),
                         (data) => {
                             this.#fetchDataModalParamsContainerElmt.innerHTML = "";
 
                             if (data.data.length > 0) {
                                 let weatherParamsTitleElmt = document.createElement("h6");
                                 weatherParamsTitleElmt.innerText = `${data.data.length} weather parameter${data.data.length > 1 ? "s" : ""} will be fetched:`;
```

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/structuralElements/explore.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/structuralElements/explore.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/data/completeness.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/data/completeness.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/data/explore.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/users/manageGroups.js`

 * *Files 27% similar despite different names*

#### js-beautify {}

```diff
@@ -1,375 +1,293 @@
 import {
-    InternalAPIRequest
-} from "../../../tools/fetcher.js";
-import {
-    flaskES6
-} from "../../../../app.js";
+    DropZone
+} from "../../components/dropZone.js";
 import {
     FlashMessageTypes,
     FlashMessage
-} from "../../../components/flash.js";
-import {
-    TimeseriesChartExplore
-} from "../../../components/charts/tsChartExplore.js";
+} from "../../components/flash.js";
 import {
     Spinner
-} from "../../../components/spinner.js";
+} from "../../components/spinner.js";
+import {
+    UserGroupItem
+} from "../../components/userGroup/userGroupItem.js";
+import {
+    ModalConfirm
+} from "../../components/modalConfirm.js";
 import {
-    TimeseriesSelector
-} from "../../../components/timeseries/selector.js";
+    InternalAPIRequest
+} from "../../tools/fetcher.js";
+import {
+    flaskES6,
+    signedUser
+} from "../../../app.js";
 
 
-export class TimeseriesDataExploreView {
+export class UserManageGroupsView {
 
-    #internalAPIRequester = null;
-    #tsDataStatesReqID = null;
-    #tsDataCSVReqID = null;
+    #user = null;
 
+    #internalAPIRequester = null;
+    #getGroupListReqID = null;
     #messagesElmt = null;
-    #chartContainerElmt = null;
-    #loadBtnElmt = null;
-    #timezonePickerElmt = null;
-    #startDatetimePickerElmt = null;
-    #endDatetimePickerElmt = null;
-
-    #tsDataStatesSelectElmt = null;
 
-    #aggInputElmt = null;
-    #bucketElmt = null;
+    #userGroupTabElmt = null;
+    #userGroupAvailableBtnElmt = null;
+    #userGroupContainerElmt = null;
+    #userGroupCountElmt = null;
+
+    #userGroupAvailableColumnElmt = null;
+    #userGroupAvailableCollapsePanelElmt = null;
+    #userGroupAvailableContainerElmt = null;
+    #userGroupAvailableCountElmt = null;
 
-    #chartExplore = null;
-    #tsSelector = null;
+    #dropZoneElmt = null;
 
-    #tsParamsContainerElmt = null;
-
-    #tsChartParams = {};
-
-    constructor(options = {
-        height: 400
-    }) {
-        this.#tsSelector = TimeseriesSelector.getInstance("tsSelectorExplore");
+    constructor(user) {
+        this.#user = user;
 
         this.#cacheDOM();
-        this.#initElements();
-
-        this.#chartExplore = new TimeseriesChartExplore(options);
-        this.#chartContainerElmt.innerHTML = "";
-        this.#chartContainerElmt.appendChild(this.#chartExplore);
 
         this.#internalAPIRequester = new InternalAPIRequest();
 
+        this.#dropZoneElmt = new DropZone({
+            dropEffect: "move",
+            helpNoItemsText: `Not yet a member of any group.`,
+            helpBackgroundText: `Drag and drop groups here`
+        });
+        this.#dropZoneElmt.id = `dropZone-${this.#user.id}`;
+        this.#userGroupContainerElmt.appendChild(this.#dropZoneElmt);
+        this.#dropZoneElmt.hideHelp();
+
         this.#initEventListeners();
     }
 
     #cacheDOM() {
         this.#messagesElmt = document.getElementById("messages");
-        this.#chartContainerElmt = document.getElementById("chartContainer");
-        this.#loadBtnElmt = document.getElementById("loadBtn");
-
-        this.#tsDataStatesSelectElmt = document.getElementById("data_states");
-
-        this.#timezonePickerElmt = document.getElementById("timezonePicker");
-        this.#startDatetimePickerElmt = document.getElementById("start_datetime");
-        this.#endDatetimePickerElmt = document.getElementById("end_datetime");
-
-        this.#aggInputElmt = document.getElementById("agg");
-        this.#bucketElmt = document.getElementById("bucket");
-
-        this.#tsParamsContainerElmt = document.getElementById("tsParam");
-    }
-
-    #initElements() {
-        this.#updateLoadBtnState();
-        this.#updateAggregationBucketState();
-
-        this.#startDatetimePickerElmt.dateMax = this.#endDatetimePickerElmt.date;
-        this.#endDatetimePickerElmt.dateMin = this.#startDatetimePickerElmt.date;
-    }
-
-    #addTsParamInputs(tsData) {
-        this.#tsChartParams[tsData.name] = {
-            position: "left",
-            type: "line",
-            style: "solid",
-            color: this.#chartExplore.colors[(this.#tsSelector.selectedItems.length - 1) % this.#chartExplore.colors.length],
-            symbol: tsData.unit_symbol,
-        };
-
-        let tsParam = document.createElement("div");
-        tsParam.id = "tsParam-" + tsData.id;
-
-        let row = document.createElement("div");
-        row.className = "row d-xl-flex d-grid m-2 mb-3";
-
-        let h6 = document.createElement("h6");
-        h6.textContent = tsData.label;
-        row.appendChild(h6);
-
-        let col1 = document.createElement("div");
-        col1.className = "col pb-2 pb-xl-0";
-
-        let positionSelect = document.createElement("select");
-        positionSelect.className = "form-select form-select-sm";
-        positionSelect.name = "position";
-        positionSelect.setAttribute("aria-label", "Select a position");
-
-        for (let [optValue, optText] of Object.entries({
-                "left": "Left",
-                "right": "Right"
-            })) {
-            let optElmt = document.createElement("option");
-            optElmt.value = optValue;
-            optElmt.textContent = optText;
-            optElmt.selected = this.#tsChartParams[tsData.name].position == optValue;
-            positionSelect.appendChild(optElmt);
-        }
-
-        col1.appendChild(positionSelect);
-
-        let col2 = document.createElement("div");
-        col2.className = "col pb-2 pb-xl-0";
-
-        let typeSelect = document.createElement("select");
-        typeSelect.className = "form-select form-select-sm";
-        typeSelect.name = "type";
-        typeSelect.setAttribute("aria-label", "Select a type of graph");
-
-        for (let [optValue, optText] of Object.entries({
-                "line": "Line",
-                "bar": "Bar"
-            })) {
-            let optElmt = document.createElement("option");
-            optElmt.value = optValue;
-            optElmt.textContent = optText;
-            optElmt.selected = this.#tsChartParams[tsData.name].type == optValue;
-            typeSelect.appendChild(optElmt);
-        }
-
-        col2.appendChild(typeSelect);
-
-        let col3 = document.createElement("div");
-        col3.className = "col pb-2 pb-xl-0";
-
-        let styleSelect = document.createElement("select");
-        styleSelect.className = "form-select form-select-sm";
-        styleSelect.name = "style";
-        styleSelect.setAttribute("aria-label", "Select a style of line");
-
-        for (let [optValue, optText] of Object.entries({
-                "solid": "Solid",
-                "dashed": "Dashed",
-                "dotted": "Dotted"
-            })) {
-            let styleOptElmt = document.createElement("option");
-            styleOptElmt.value = optValue;
-            styleOptElmt.textContent = optText;
-            styleOptElmt.selected = this.#tsChartParams[tsData.name].style == optValue;
-            styleSelect.appendChild(styleOptElmt);
-        }
-
-        col3.appendChild(styleSelect);
-
-        let col4 = document.createElement("div");
-        col4.className = "col pb-2 pb-xl-0";
-
-        let colorInput = document.createElement("input");
-        colorInput.type = "color";
-        colorInput.className = "form-control form-control-sm";
-        colorInput.name = "color";
-        colorInput.value = this.#tsChartParams[tsData.name].color;
-        colorInput.setAttribute("aria-label", "Select a color");
-
-        col4.appendChild(colorInput);
-
-        row.appendChild(col1);
-        row.appendChild(col2);
-        row.appendChild(col3);
-        row.appendChild(col4);
-
-        tsParam.appendChild(row);
-        this.#tsParamsContainerElmt.appendChild(tsParam);
-
-        positionSelect.addEventListener("change", (event) => {
-            event.preventDefault();
-
-            this.#tsChartParams[tsData.name].position = positionSelect.value;
-        });
-
-        typeSelect.addEventListener("change", (event) => {
-            event.preventDefault();
-
-            this.#tsChartParams[tsData.name].type = typeSelect.value;
-        });
-
-        styleSelect.addEventListener("change", (event) => {
-            event.preventDefault();
-
-            this.#tsChartParams[tsData.name].style = styleSelect.value;
-        });
-
-        colorInput.addEventListener("change", (event) => {
-            event.preventDefault();
-
-            this.#tsChartParams[tsData.name].color = colorInput.value;
-        });
+        this.#userGroupTabElmt = document.getElementById("groups-tab");
+        this.#userGroupAvailableBtnElmt = document.getElementById("userGroupAvailableBtn");
+        this.#userGroupContainerElmt = document.getElementById("userGroupContainer");
+        this.#userGroupCountElmt = document.getElementById("userGroupCount");
+        this.#userGroupAvailableColumnElmt = document.getElementById("userGroupAvailableColumn");
+        this.#userGroupAvailableCollapsePanelElmt = document.getElementById("userGroupAvailableCollapsePanel");
+        this.#userGroupAvailableContainerElmt = document.getElementById("userGroupAvailableContainer");
+        this.#userGroupAvailableCountElmt = document.getElementById("userGroupAvailableCount");
     }
 
     #initEventListeners() {
-        this.#tsSelector.addEventListener("toggleItem", (event) => {
-            event.preventDefault();
-
-            this.#updateLoadBtnState();
+        this.#userGroupTabElmt.addEventListener("hide.bs.tab", () => {
+            let bsCollapse = bootstrap.Collapse.getOrCreateInstance(this.#userGroupAvailableCollapsePanelElmt, {
+                toggle: false
+            });
+            bsCollapse.hide();
+        });
 
-            if (event.detail.isActive) {
-                this.#addTsParamInputs(event.detail.timeseries);
-            } else {
-                delete this.#tsChartParams[event.detail.timeseries.name];
+        this.#userGroupAvailableCollapsePanelElmt.addEventListener("show.bs.collapse", (event) => {
+            // Only do this actions when main collapse element event is triggered.
+            if (event.target == this.#userGroupAvailableCollapsePanelElmt) {
+                this.#userGroupAvailableColumnElmt.classList.remove("d-none");
+
+                let iconElmt = document.createElement("i");
+                iconElmt.classList.add("bi", "bi-arrow-bar-right");
+                this.#userGroupAvailableBtnElmt.innerHTML = "";
+                this.#userGroupAvailableBtnElmt.appendChild(iconElmt);
 
-                document.getElementById(`tsParam-${event.detail.timeseries.id.toString()}`)?.remove();
+                this.#dropZoneElmt.showHelp();
             }
         });
 
-        this.#timezonePickerElmt.addEventListener("tzChange", (event) => {
-            event.preventDefault();
-
-            this.#startDatetimePickerElmt.tzName = this.#timezonePickerElmt.tzName;
-            this.#endDatetimePickerElmt.tzName = this.#timezonePickerElmt.tzName;
+        this.#userGroupAvailableCollapsePanelElmt.addEventListener("hide.bs.collapse", (event) => {
+            if (event.target == this.#userGroupAvailableCollapsePanelElmt) {
+                this.#dropZoneElmt.hideHelp();
+            }
         });
 
-        this.#startDatetimePickerElmt.addEventListener("dateChange", (event) => {
-            event.preventDefault();
-
-            this.#endDatetimePickerElmt.dateMin = this.#startDatetimePickerElmt.date;
-            this.#updateLoadBtnState();
+        this.#userGroupAvailableCollapsePanelElmt.addEventListener("hidden.bs.collapse", (event) => {
+            // Only do this actions when main collapse element event is triggered.
+            if (event.target == this.#userGroupAvailableCollapsePanelElmt) {
+                this.#userGroupAvailableColumnElmt.classList.add("d-none");
+
+                let textElmt = document.createElement("span");
+                textElmt.innerText = "Manage user's groups";
+                let iconElmt = document.createElement("i");
+                iconElmt.classList.add("bi", "bi-arrow-bar-left", "me-1");
+
+                this.#userGroupAvailableBtnElmt.innerHTML = "";
+                this.#userGroupAvailableBtnElmt.appendChild(iconElmt);
+                this.#userGroupAvailableBtnElmt.appendChild(textElmt);
+            }
         });
 
-        this.#endDatetimePickerElmt.addEventListener("dateChange", (event) => {
+        this.#dropZoneElmt.addEventListener("itemDrop", (event) => {
             event.preventDefault();
 
-            this.#startDatetimePickerElmt.dateMax = this.#endDatetimePickerElmt.date;
-            this.#updateLoadBtnState();
+            let jsonData = JSON.parse(event.detail.dataTransfer.getData("application/json"));
+            let groupId = jsonData.sourceNodeData.id;
+            let groupName = jsonData.sourceNodeData.name;
+
+            this.#internalAPIRequester.post(
+                flaskES6.urlFor(`api.user_groups.add_user`, {
+                    id: groupId
+                }), {
+                    user_id: this.#user.id
+                },
+                (data) => {
+                    let userGroupItemElmt = new UserGroupItem(groupId, groupName, false, signedUser.is_admin ? flaskES6.urlFor(`user_groups.view`, {
+                        id: groupId,
+                        tab: `users`
+                    }) : null, signedUser.is_admin ? this.#userGroupRemoveUserCallback.bind(this, groupId, groupName, data.data.id, this.#user.name) : null);
+                    this.#dropZoneElmt.addElement(userGroupItemElmt);
+
+                    let dropedItemElmt = document.getElementById(jsonData.sourceNodeId);
+                    dropedItemElmt.classList.add("d-none", "invisible");
+
+                    this.#refreshCounters();
+
+                    let flashMsgElmt = new FlashMessage({
+                        type: FlashMessageTypes.SUCCESS,
+                        text: `User added to ${groupName} group!`,
+                        isDismissible: true,
+                        delay: 4
+                    });
+                    this.#messagesElmt.appendChild(flashMsgElmt);
+                },
+                (error) => {
+                    let flashMsgElmt = new FlashMessage({
+                        type: FlashMessageTypes.ERROR,
+                        text: error.toString(),
+                        isDismissible: true
+                    });
+                    this.#messagesElmt.appendChild(flashMsgElmt);
+                },
+            );
         });
+    }
 
-        this.#loadBtnElmt.addEventListener("click", (event) => {
-            event.preventDefault();
+    #userGroupRemoveUserCallback(groupId, groupName, groupUserRelId, userName) {
+        let userGroupItemElmt = document.getElementById(`usergroup-${groupId}`);
 
-            this.#refreshChart();
+        // Add a modal confirm component for this item, defining an "ok" callback function to remove it.
+        let modalConfirm = new ModalConfirm(`usergroup-${groupId}`, `Remove <mark>${userName}</mark> user from <mark>${groupName}</mark> group`, () => {
+            // Inside the callback to remove user from group.
+            this.#internalAPIRequester.post(
+                flaskES6.urlFor("api.user_groups.remove_user", {
+                    id: groupId,
+                    rel_id: groupUserRelId
+                }),
+                null,
+                () => {
+                    let dropedItemElmt = document.getElementById(`drag-usergroup-${groupId}`);
+                    if (dropedItemElmt != null) {
+                        dropedItemElmt.classList.remove("d-none", "invisible");
+                    } else {
+                        dropedItemElmt = new UserGroupItem(groupId, groupName, true);
+                        this.#userGroupAvailableContainerElmt.appendChild(dropedItemElmt);
+                    }
+                    this.#dropZoneElmt.removeElement(userGroupItemElmt);
+
+                    this.#refreshCounters();
+
+                    let flashMsgElmt = new FlashMessage({
+                        type: FlashMessageTypes.SUCCESS,
+                        text: `User removed from ${groupName} group!`,
+                        isDismissible: true,
+                        delay: 4
+                    });
+                    this.#messagesElmt.appendChild(flashMsgElmt);
+                },
+                (error) => {
+                    let flashMsgElmt = new FlashMessage({
+                        type: FlashMessageTypes.ERROR,
+                        text: error.toString(),
+                        isDismissible: true
+                    });
+                    this.#messagesElmt.appendChild(flashMsgElmt);
+                },
+            );
         });
+        userGroupItemElmt.appendChild(modalConfirm);
 
-        this.#aggInputElmt.addEventListener("change", (event) => {
-            event.preventDefault();
-
-            this.#updateAggregationBucketState();
-        });
+        modalConfirm.show();
     }
 
-    #updateLoadBtnState() {
-        if (this.#tsSelector.selectedItems.length > 0 && this.#startDatetimePickerElmt.hasDatetime && this.#endDatetimePickerElmt.hasDatetime) {
-            this.#loadBtnElmt.removeAttribute("disabled");
-        } else {
-            this.#loadBtnElmt.setAttribute("disabled", true);
-        }
-    }
+    #refreshCounters() {
+        this.#userGroupCountElmt.innerText = this.#dropZoneElmt.count.toString();
+        let userGroupAvailableCount = this.#userGroupAvailableContainerElmt.querySelectorAll(":scope > div[draggable=true]:not(.d-none)").length;
+        this.#userGroupAvailableCountElmt.innerText = userGroupAvailableCount.toString();
 
-    #updateAggregationBucketState() {
-        if (this.#aggInputElmt.value == "none") {
-            this.#bucketElmt.setAttribute("disabled", true);
-            this.#bucketElmt.parentElement.classList.add("d-none", "invisible");
-        } else {
-            this.#bucketElmt.removeAttribute("disabled");
-            this.#bucketElmt.parentElement.classList.remove("d-none", "invisible");
+        if (this.#dropZoneElmt.count <= 0) {
+            this.#dropZoneElmt.showNoItems();
         }
-    }
-
-    #refreshChart() {
-        this.#chartExplore.showLoading();
-
-        let loadBtnInnerBackup = this.#loadBtnElmt.innerHTML;
-        this.#loadBtnElmt.innerHTML = "";
-        this.#loadBtnElmt.appendChild(new Spinner({
-            useSmallSize: true,
-            useSecondaryColor: true
-        }));
-        this.#loadBtnElmt.setAttribute("disabled", true);
-
-        let urlParams = {
-            timeseries: this.#tsSelector.selectedItems.map(ts => ts.name),
-            data_state: this.#tsDataStatesSelectElmt.value,
-            start_date: this.#startDatetimePickerElmt.date,
-            start_time: this.#startDatetimePickerElmt.time,
-            end_date: this.#endDatetimePickerElmt.date,
-            end_time: this.#endDatetimePickerElmt.time,
-            timezone: this.#timezonePickerElmt.tzName,
-        };
-        if (this.#aggInputElmt.value != "none") {
-            urlParams.agg = this.#aggInputElmt.value;
-            urlParams.bucket_width_value = this.#bucketElmt.bucketWidthValue;
-            urlParams.bucket_width_unit = this.#bucketElmt.bucketWidthUnit;
+        let noUserGroupAvailableInfoElmt = this.#userGroupAvailableContainerElmt.querySelector(":scope > span");
+        if (noUserGroupAvailableInfoElmt == null) {
+            noUserGroupAvailableInfoElmt = document.createElement("span");
+            noUserGroupAvailableInfoElmt.classList.add("fst-italic");
+            noUserGroupAvailableInfoElmt.innerText = "No groups available.";
+            this.#userGroupAvailableContainerElmt.appendChild(noUserGroupAvailableInfoElmt);
         }
-
-        if (this.#tsDataCSVReqID != null) {
-            this.#internalAPIRequester.abort(this.#tsDataCSVReqID);
-            this.#tsDataCSVReqID = null;
+        if (userGroupAvailableCount <= 0) {
+            noUserGroupAvailableInfoElmt.classList.remove("d-none");
+        } else {
+            noUserGroupAvailableInfoElmt.classList.add("d-none");
         }
-        this.#tsDataCSVReqID = this.#internalAPIRequester.get(
-            flaskES6.urlFor(`api.timeseries.data.retrieve_multiple_data`, urlParams),
-            (data) => {
-                this.#chartExplore.setDownloadCSVLink(flaskES6.urlFor(`timeseries.data.download_multiple`, urlParams));
-
-                let options = {
-                    subtitle: this.#tsDataStatesSelectElmt.options[this.#tsDataStatesSelectElmt.selectedIndex].text,
-                    timezone: this.#timezonePickerElmt.tzName,
-                    series: this.#tsChartParams,
-                };
-                this.#chartExplore.load(data, options);
-            },
-            (error) => {
-                let flashMsgElmt = new FlashMessage({
-                    type: FlashMessageTypes.ERROR,
-                    text: error.toString(),
-                    isDismissible: true
-                });
-                this.#messagesElmt.appendChild(flashMsgElmt);
-
-                this.#chartExplore.removeDownloadCSVLink();
-            },
-            () => {
-                this.#loadBtnElmt.innerHTML = loadBtnInnerBackup;
-                this.#loadBtnElmt.removeAttribute("disabled");
-            },
-        );
     }
 
     refresh() {
-        this.#tsDataStatesSelectElmt.innerHTML = "";
-        let loadingOptionElmt = document.createElement("option");
-        loadingOptionElmt.value = "None";
-        loadingOptionElmt.innerText = "loading...";
-        this.#tsDataStatesSelectElmt.appendChild(loadingOptionElmt);
-
-        if (this.#tsDataStatesReqID != null) {
-            this.#internalAPIRequester.abort(this.#tsDataStatesReqID);
-            this.#tsDataStatesReqID = null;
+        if (!this.#userGroupTabElmt.isLoaded) {
+            this.#userGroupCountElmt.innerHTML = "";
+            this.#userGroupCountElmt.appendChild(new Spinner({
+                useSmallSize: true,
+                useSecondaryColor: true
+            }));
+
+            this.#userGroupAvailableCountElmt.innerHTML = "";
+            this.#userGroupAvailableCountElmt.appendChild(new Spinner({
+                useSmallSize: true,
+                useSecondaryColor: true
+            }));
+
+            this.#userGroupAvailableContainerElmt.innnerHTML = "";
+            this.#userGroupAvailableContainerElmt.appendChild(new Spinner());
+
+            this.#dropZoneElmt.setLoading();
+
+            if (this.#getGroupListReqID != null) {
+                this.#internalAPIRequester.abort(this.#getGroupListReqID);
+                this.#getGroupListReqID = null;
+            }
+            this.#getGroupListReqID = this.#internalAPIRequester.get(
+                flaskES6.urlFor(`api.users.list_groups`, {
+                    id: this.#user.id
+                }),
+                (data) => {
+                    this.#dropZoneElmt.clear();
+                    for (let row of data.groups) {
+                        let userGroupItemElmt = new UserGroupItem(row.id, row.name, false, signedUser.is_admin ? flaskES6.urlFor(`user_groups.view`, {
+                            id: row.id,
+                            tab: `users`
+                        }) : null, signedUser.is_admin ? this.#userGroupRemoveUserCallback.bind(this, row.id, row.name, row.rel_id, this.#user.name) : null);
+                        this.#dropZoneElmt.addElement(userGroupItemElmt);
+                    }
+
+                    this.#userGroupAvailableContainerElmt.innerHTML = "";
+                    for (let row of data.available_groups) {
+                        let userGroupAvailableItemElmt = new UserGroupItem(row.id, row.name, true);
+                        this.#userGroupAvailableContainerElmt.appendChild(userGroupAvailableItemElmt);
+                    }
+
+                    this.#refreshCounters();
+
+                    this.#userGroupTabElmt.isLoaded = true;
+                },
+                (error) => {
+                    let flashMsgElmt = new FlashMessage({
+                        type: FlashMessageTypes.ERROR,
+                        text: error.toString(),
+                        isDismissible: true
+                    });
+                    this.#messagesElmt.appendChild(flashMsgElmt);
+                },
+            );
         }
-        this.#tsDataStatesReqID = this.#internalAPIRequester.get(
-            flaskES6.urlFor(`api.timeseries.datastates.retrieve_list`),
-            (data) => {
-                this.#tsDataStatesSelectElmt.innerHTML = "";
-                for (let option of data.data) {
-                    let optionElmt = document.createElement("option");
-                    optionElmt.value = option.id;
-                    optionElmt.innerText = option.name;
-                    this.#tsDataStatesSelectElmt.appendChild(optionElmt);
-                }
-            },
-            (error) => {
-                let flashMsgElmt = new FlashMessage({
-                    type: FlashMessageTypes.ERROR,
-                    text: error.toString(),
-                    isDismissible: true
-                });
-                this.#messagesElmt.appendChild(flashMsgElmt);
-            },
-        );
     }
 }
```

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/delete.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/delete.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/list.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/list.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/manageStructuralElements.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/manageStructuralElements.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/timeseries/semanticSetup.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/timeseries/semanticSetup.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/scripts/modules/views/users/list.js` & `bemserver-ui-0.5.3/bemserver_ui/static/scripts/modules/views/users/list.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/styles/app.css` & `bemserver-ui-0.5.3/bemserver_ui/static/styles/app.css`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 @import url("./tree.css");
 @import url("./dragndrop.css");
 
 
 :root {
     --app-sidebar-bg: #f3f8e9;
     --app-header-height: 60px;
+    --app-min-width: 420px;
 }
 
 body,
 .app-header {
-    min-width: 420px;
+    min-width: var(--app-min-width);
 }
 
 .app-messages {
     z-index: 1031;
 }
 .app-messages > .alert {
     min-width: 40vw !important;
@@ -219,7 +220,22 @@
 
 .app-notif-animate {
     position: absolute;
     top: 0;
     right: 0;
     animation: ring 8s 1s ease-in-out infinite;
 }
+
+.app-chart-settings-panel {
+    top: var(--app-header-height) !important;
+    width: 66% !important;
+}
+@media (max-width: 767.98px) {
+    .app-chart-settings-panel {
+        width: 100% !important;
+    }
+}
+@media (min-width: 768px) and (max-width: 991.98px) {
+    .app-chart-settings-panel {
+        width: 75% !important;
+    }
+}
```

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/styles/main.css` & `bemserver-ui-0.5.3/bemserver_ui/static/styles/main.css`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/styles/signin.css` & `bemserver-ui-0.5.3/bemserver_ui/static/styles/signin.css`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/static/styles/tree.css` & `bemserver-ui-0.5.3/bemserver_ui/static/styles/tree.css`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/components/campaigns/selector.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/components/campaigns/selector.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/components/header.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/components/header.html`

 * *Files 9% similar despite different names*

```diff
@@ -12,20 +12,26 @@
                 <img class="img-fluid app-logo-partner" src="{{ project_logo.src }}" alt="{{ project_logo.name }}">
             </a>
             {% endif %}
         </div>
         <div class="d-flex flex-nowrap justify-content-end gap-4 me-3">
             <a id="notifBell" href="{{ url_for('notifications.explore', state='unread') }}" class="link-secondary position-relative" title="You have no unread notifications" role="button"><i class="bi bi-bell"></i></a>
             <div class="dropdown">
-                <a role="button" title="{{ signed_user.name }}" class="link-secondary text-decoration-none dropdown-toggle d-flex align-items-center" id="userMenu" data-bs-toggle="dropdown" aria-expanded="false">
+                <a role="button" title="{{ signed_user.name }}" class="link-secondary text-decoration-none dropdown-toggle d-flex align-items-center" id="userMenu" data-bs-toggle="dropdown" data-bs-auto-close="outside" aria-expanded="false">
                     <i class="bi bi-person-circle me-1"></i>
                     <span class="fw-bold">{{ signed_user.name }}</span>
                 </a>
                 <ul class="dropdown-menu dropdown-menu-end shadow" aria-labelledby="userMenu">
                     <li><a class="dropdown-item" href="{{ url_for('users.view', id=signed_user.id) }}" title="My user profile">My profile</a></li>
+                    <li class="dropstart">
+                        <a class="dropdown-item dropdown-toggle" data-bs-toggle="dropdown" href="#" title="Settings">Settings...</a>
+                        <ul class="dropdown-menu">
+                            <li><a class="dropdown-item" href="{{ url_for('notifications.setup') }}" title="Notifications settings">Notifications</a></li>
+                        </ul>
+                    </li>
                     <li><hr class="dropdown-divider"></li>
                     <li><a class="dropdown-item" href="{{ url_for('main.about') }}" title="About BEMServer">About BEMServer...</a></li>
                     <li><a class="dropdown-item" href="{{ url_for('auth.signout', ignore_campaign_ctxt=True) }}" title="Sign out"><i class="bi bi-power"></i> Sign out</a></li>
                 </ul>
             </div>
         </div>
     </div>
```

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_admin.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_admin.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_analysis.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_analysis.html`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
         <div id="panelCollapseAnalysis" class="accordion-collapse collapse" aria-labelledby="panelHeadingAnalysis">
             <div class="accordion-body px-0 py-2">
                 <ul class="nav nav-pills flex-column gap-1">
                     {% filter indent(width=20, first=True) %}
                     {% if g.campaign_ctxt.has_campaign %}
                     {{- mac_sidebar.render_nav_item("Energy consumption", url_for("analysis.energy_consumption.explore"), "Energy consumption", ["bi", "bi-fire"]) -}}
                     {{- mac_sidebar.render_nav_item("Degree days", url_for("analysis.degree_days.explore"), "Degree days", ["bi", "bi-thermometer-half"]) -}}
+                    {{- mac_sidebar.render_nav_item("Weather data", url_for("analysis.weather.explore"), "Weather data", ["bi", "bi-cloud-sun"]) -}}
                     {% endif %}
                     {% for sidebar_section_plugin in sidebar_section_plugins %}
                     {{- mac_sidebar.render_nav_item_from_plugin(sidebar_section_plugin) -}}
                     {% endfor %}
                     {% endfilter %}
                 </ul>
             </div>
```

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_campaign_context.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_campaign_context.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_campaign_selector.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_campaign_selector.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_dashboards.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_dashboards.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_services.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_services.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/components/sidebar/sidebar_tsdata.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/components/sidebar/sidebar_tsdata.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/components/user_groups/group_for_campaign.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/components/user_groups/group_for_campaign.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/components/user_groups/group_for_campaign_scope.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/components/user_groups/group_for_campaign_scope.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/components/user_groups/user_group_available.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/components/user_groups/user_group_available.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/components/users/user_available.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/components/users/user_available.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/components/users/user_for_group.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/components/users/user_for_group.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/macros/components/sidebar.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/macros/components/sidebar.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/macros/components/structural_element_selector.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/macros/components/structural_element_selector.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/macros/components/ts_selector.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/macros/components/ts_selector.html`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 <app-ts-selector{% if element_id %} id="{{ element_id }}"{% endif %} selection-limit="{{ selection_limit }}"{% for filter_name, filter_value in filters.items() %} {{ filter_name }}={{ filter_value }}{% endfor %}>
     <div class="d-flex justify-content-between align-items-start gap-2">
         <h5>Timeseries selection</h5>
         <small id="countResultsSelected" class="text-muted"></small>
     </div>
     <div class="btn-group bg-white w-100">
         <div id="selectedItemsContainer" class="d-flex flex-wrap align-items-center border border-secondary bg-secondary bg-opacity-25 rounded-start w-100 gap-2 p-2 px-3"></div>
+        <button id="clearSelectionBtn" type="button" class="btn btn-outline-danger g-1 d-none invisible">
+            <i class="bi bi-x-lg"></i>
+            <span class="visually-hidden">Clear selection</span>
+        </button>
         <button id="dropdownSearchBtn" type="button" class="btn btn-outline-secondary dropdown-toggle dropdown-toggle-split g-1" data-bs-toggle="dropdown" data-bs-auto-close="outside" data-bs-reference="parent" aria-expanded="false">
             <i class="bi bi-search"></i>
             <span class="visually-hidden">Toggle search panel</span>
         </button>
         <div id="dropdownSearchPanel" class="dropdown-menu shadow w-100 p-4" aria-labelledby="dropdownSearchBtn">
             <div class="d-flex align-items-center gap-2 mb-2">
                 <input type="text" class="form-control form-control-sm" id="search" name="search" placeholder="Search..." aria-label="Search" aria-describedby="search" autofocus>
```

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/macros/flash.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/macros/flash.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/macros/partners.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/macros/partners.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/about.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/about.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/analysis/degree_days.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/analysis/degree_days.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/analysis/energy_consumption.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/analysis/energy_consumption.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/base.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/base.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaign_scopes/create.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaign_scopes/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaign_scopes/edit.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaign_scopes/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaign_scopes/list.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaign_scopes/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaign_scopes/view.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaign_scopes/view.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaigns/create.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaigns/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaigns/edit.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaigns/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaigns/list.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaigns/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaigns/manage_groups.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaigns/manage_groups.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/campaigns/view.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/campaigns/view.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/categories/create.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/categories/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/categories/edit.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/categories/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/categories/list.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/categories/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/create.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/edit.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/events/list.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/events/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/home.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/home.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/notifications/explore.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/notifications/explore.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,683 +1,664 @@
 00000000: 7b25 2065 7874 656e 6473 2022 7061 6765  {% extends "page
 00000010: 732f 6261 7365 2e68 746d 6c22 2025 7d0a  s/base.html" %}.
 00000020: 0a7b 2520 7365 7420 7469 746c 6520 3d20  .{% set title = 
 00000030: 224e 6f74 6966 6963 6174 696f 6e73 2220  "Notifications" 
 00000040: 257d 0a0a 7b25 2062 6c6f 636b 206d 6169  %}..{% block mai
-00000050: 6e5f 746f 6f6c 6261 7220 257d 0a7b 7b20  n_toolbar %}.{{ 
-00000060: 7375 7065 7228 2920 2d7d 7d0a 7b25 2066  super() -}}.{% f
-00000070: 696c 7465 7220 696e 6465 6e74 2877 6964  ilter indent(wid
-00000080: 7468 3d32 302c 2066 6972 7374 3d54 7275  th=20, first=Tru
-00000090: 6529 2025 7d0a 3c61 2068 7265 663d 227b  e) %}.<a href="{
-000000a0: 7b20 7572 6c5f 666f 7228 276e 6f74 6966  { url_for('notif
-000000b0: 6963 6174 696f 6e73 2e73 6574 7570 2729  ications.setup')
-000000c0: 207d 7d22 2063 6c61 7373 3d22 6274 6e20   }}" class="btn 
-000000d0: 6274 6e2d 736d 2062 746e 2d6f 7574 6c69  btn-sm btn-outli
-000000e0: 6e65 2d73 6563 6f6e 6461 7279 2074 6578  ne-secondary tex
-000000f0: 742d 6e6f 7772 6170 2220 7469 746c 653d  t-nowrap" title=
-00000100: 2253 6574 7570 206e 6f74 6966 6963 6174  "Setup notificat
-00000110: 696f 6e73 223e 3c69 2063 6c61 7373 3d22  ions"><i class="
-00000120: 6269 2062 692d 746f 6f6c 7322 3e3c 2f69  bi bi-tools"></i
-00000130: 3e20 5365 7475 703c 2f61 3e0a 7b25 2065  > Setup</a>.{% e
-00000140: 6e64 6669 6c74 6572 2025 7d0a 7b25 2065  ndfilter %}.{% e
-00000150: 6e64 626c 6f63 6b20 6d61 696e 5f74 6f6f  ndblock main_too
-00000160: 6c62 6172 2025 7d0a 0a7b 2520 626c 6f63  lbar %}..{% bloc
-00000170: 6b20 6d61 696e 5f63 6f6e 7465 6e74 2025  k main_content %
-00000180: 7d0a 7b7b 2073 7570 6572 2829 202d 7d7d  }.{{ super() -}}
-00000190: 0a3c 6469 7620 636c 6173 733d 2263 6f6e  .<div class="con
-000001a0: 7461 696e 6572 2d66 6c75 6964 223e 0a20  tainer-fluid">. 
-000001b0: 2020 203c 6469 7620 636c 6173 733d 2272     <div class="r
-000001c0: 6f77 206d 622d 3422 3e0a 2020 2020 2020  ow mb-4">.      
-000001d0: 2020 3c64 6976 2063 6c61 7373 3d22 636f    <div class="co
-000001e0: 6c22 3e0a 2020 2020 2020 2020 2020 2020  l">.            
-000001f0: 3c64 6976 2063 6c61 7373 3d22 6163 636f  <div class="acco
-00000200: 7264 696f 6e22 2069 643d 2261 6363 6f72  rdion" id="accor
-00000210: 6469 6f6e 4669 6c74 6572 7322 3e0a 2020  dionFilters">.  
-00000220: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00000230: 6976 2063 6c61 7373 3d22 6163 636f 7264  iv class="accord
-00000240: 696f 6e2d 6974 656d 223e 0a20 2020 2020  ion-item">.     
-00000250: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000260: 6832 2063 6c61 7373 3d22 6163 636f 7264  h2 class="accord
-00000270: 696f 6e2d 6865 6164 6572 2220 6964 3d22  ion-header" id="
-00000280: 6865 6164 696e 6746 696c 7465 7273 223e  headingFilters">
-00000290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000002a0: 2020 2020 2020 2020 203c 6275 7474 6f6e           <button
-000002b0: 2063 6c61 7373 3d22 6163 636f 7264 696f   class="accordio
-000002c0: 6e2d 6275 7474 6f6e 2063 6f6c 6c61 7073  n-button collaps
-000002d0: 6564 2220 7479 7065 3d22 6275 7474 6f6e  ed" type="button
-000002e0: 2220 6461 7461 2d62 732d 746f 6767 6c65  " data-bs-toggle
-000002f0: 3d22 636f 6c6c 6170 7365 2220 6461 7461  ="collapse" data
-00000300: 2d62 732d 7461 7267 6574 3d22 2363 6f6c  -bs-target="#col
-00000310: 6c61 7073 6546 696c 7465 7273 2220 6172  lapseFilters" ar
-00000320: 6961 2d63 6f6e 7472 6f6c 733d 2263 6f6c  ia-controls="col
-00000330: 6c61 7073 6546 696c 7465 7273 2220 6172  lapseFilters" ar
-00000340: 6961 2d65 7870 616e 6465 643d 2266 616c  ia-expanded="fal
-00000350: 7365 223e 0a20 2020 2020 2020 2020 2020  se">.           
-00000360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000370: 203c 7370 616e 2063 6c61 7373 3d22 6677   <span class="fw
-00000380: 2d62 6f6c 6420 7465 7874 2d73 6563 6f6e  -bold text-secon
-00000390: 6461 7279 223e 3c69 2063 6c61 7373 3d22  dary"><i class="
-000003a0: 6269 2062 692d 6675 6e6e 656c 223e 3c2f  bi bi-funnel"></
-000003b0: 693e 2046 696c 7465 7273 3c2f 7370 616e  i> Filters</span
-000003c0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000003d0: 2020 2020 2020 2020 2020 3c2f 6275 7474            </butt
-000003e0: 6f6e 3e0a 2020 2020 2020 2020 2020 2020  on>.            
-000003f0: 2020 2020 2020 2020 3c2f 6832 3e0a 2020          </h2>.  
-00000400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000410: 2020 3c64 6976 2069 643d 2263 6f6c 6c61    <div id="colla
-00000420: 7073 6546 696c 7465 7273 2220 636c 6173  pseFilters" clas
-00000430: 733d 2261 6363 6f72 6469 6f6e 2d63 6f6c  s="accordion-col
-00000440: 6c61 7073 6520 636f 6c6c 6170 7365 2220  lapse collapse" 
-00000450: 6172 6961 2d6c 6162 656c 6c65 6462 793d  aria-labelledby=
-00000460: 2268 6561 6469 6e67 4669 6c74 6572 7322  "headingFilters"
-00000470: 2064 6174 612d 6273 2d70 6172 656e 743d   data-bs-parent=
-00000480: 2223 6163 636f 7264 696f 6e46 696c 7465  "#accordionFilte
-00000490: 7273 223e 0a20 2020 2020 2020 2020 2020  rs">.           
-000004a0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-000004b0: 7620 636c 6173 733d 2261 6363 6f72 6469  v class="accordi
-000004c0: 6f6e 2d62 6f64 7922 3e0a 2020 2020 2020  on-body">.      
-000004d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000004e0: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-000004f0: 3d22 726f 7720 672d 3220 6d62 2d32 223e  ="row g-2 mb-2">
-00000500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000050: 6e5f 636f 6e74 656e 7420 257d 0a7b 7b20  n_content %}.{{ 
+00000060: 7375 7065 7228 2920 2d7d 7d0a 3c64 6976  super() -}}.<div
+00000070: 2063 6c61 7373 3d22 636f 6e74 6169 6e65   class="containe
+00000080: 722d 666c 7569 6422 3e0a 2020 2020 3c64  r-fluid">.    <d
+00000090: 6976 2063 6c61 7373 3d22 726f 7720 6d62  iv class="row mb
+000000a0: 2d34 223e 0a20 2020 2020 2020 203c 6469  -4">.        <di
+000000b0: 7620 636c 6173 733d 2263 6f6c 223e 0a20  v class="col">. 
+000000c0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+000000d0: 636c 6173 733d 2261 6363 6f72 6469 6f6e  class="accordion
+000000e0: 2220 6964 3d22 6163 636f 7264 696f 6e46  " id="accordionF
+000000f0: 696c 7465 7273 223e 0a20 2020 2020 2020  ilters">.       
+00000100: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00000110: 6173 733d 2261 6363 6f72 6469 6f6e 2d69  ass="accordion-i
+00000120: 7465 6d22 3e0a 2020 2020 2020 2020 2020  tem">.          
+00000130: 2020 2020 2020 2020 2020 3c68 3220 636c            <h2 cl
+00000140: 6173 733d 2261 6363 6f72 6469 6f6e 2d68  ass="accordion-h
+00000150: 6561 6465 7222 2069 643d 2268 6561 6469  eader" id="headi
+00000160: 6e67 4669 6c74 6572 7322 3e0a 2020 2020  ngFilters">.    
+00000170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000180: 2020 2020 3c62 7574 746f 6e20 636c 6173      <button clas
+00000190: 733d 2261 6363 6f72 6469 6f6e 2d62 7574  s="accordion-but
+000001a0: 746f 6e20 636f 6c6c 6170 7365 6422 2074  ton collapsed" t
+000001b0: 7970 653d 2262 7574 746f 6e22 2064 6174  ype="button" dat
+000001c0: 612d 6273 2d74 6f67 676c 653d 2263 6f6c  a-bs-toggle="col
+000001d0: 6c61 7073 6522 2064 6174 612d 6273 2d74  lapse" data-bs-t
+000001e0: 6172 6765 743d 2223 636f 6c6c 6170 7365  arget="#collapse
+000001f0: 4669 6c74 6572 7322 2061 7269 612d 636f  Filters" aria-co
+00000200: 6e74 726f 6c73 3d22 636f 6c6c 6170 7365  ntrols="collapse
+00000210: 4669 6c74 6572 7322 2061 7269 612d 6578  Filters" aria-ex
+00000220: 7061 6e64 6564 3d22 6661 6c73 6522 3e0a  panded="false">.
+00000230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000240: 2020 2020 2020 2020 2020 2020 3c73 7061              <spa
+00000250: 6e20 636c 6173 733d 2266 772d 626f 6c64  n class="fw-bold
+00000260: 2074 6578 742d 7365 636f 6e64 6172 7922   text-secondary"
+00000270: 3e3c 6920 636c 6173 733d 2262 6920 6269  ><i class="bi bi
+00000280: 2d66 756e 6e65 6c22 3e3c 2f69 3e20 4669  -funnel"></i> Fi
+00000290: 6c74 6572 733c 2f73 7061 6e3e 0a20 2020  lters</span>.   
+000002a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000002b0: 2020 2020 203c 2f62 7574 746f 6e3e 0a20       </button>. 
+000002c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000002d0: 2020 203c 2f68 323e 0a20 2020 2020 2020     </h2>.       
+000002e0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+000002f0: 7620 6964 3d22 636f 6c6c 6170 7365 4669  v id="collapseFi
+00000300: 6c74 6572 7322 2063 6c61 7373 3d22 6163  lters" class="ac
+00000310: 636f 7264 696f 6e2d 636f 6c6c 6170 7365  cordion-collapse
+00000320: 2063 6f6c 6c61 7073 6522 2061 7269 612d   collapse" aria-
+00000330: 6c61 6265 6c6c 6564 6279 3d22 6865 6164  labelledby="head
+00000340: 696e 6746 696c 7465 7273 2220 6461 7461  ingFilters" data
+00000350: 2d62 732d 7061 7265 6e74 3d22 2361 6363  -bs-parent="#acc
+00000360: 6f72 6469 6f6e 4669 6c74 6572 7322 3e0a  ordionFilters">.
+00000370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000380: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00000390: 7373 3d22 6163 636f 7264 696f 6e2d 626f  ss="accordion-bo
+000003a0: 6479 223e 0a20 2020 2020 2020 2020 2020  dy">.           
+000003b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000003c0: 203c 6469 7620 636c 6173 733d 2272 6f77   <div class="row
+000003d0: 2067 2d32 206d 622d 3222 3e0a 2020 2020   g-2 mb-2">.    
+000003e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000003f0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
+00000400: 2063 6c61 7373 3d22 636f 6c2d 3132 2063   class="col-12 c
+00000410: 6f6c 2d6c 672d 3620 642d 666c 6578 2061  ol-lg-6 d-flex a
+00000420: 6c69 676e 2d69 7465 6d73 2d63 656e 7465  lign-items-cente
+00000430: 7220 6761 702d 3222 3e0a 2020 2020 2020  r gap-2">.      
+00000440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000450: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
+00000460: 7061 6e3e 4265 7477 6565 6e3c 2f73 7061  pan>Between</spa
+00000470: 6e3e 0a20 2020 2020 2020 2020 2020 2020  n>.             
+00000480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000490: 2020 2020 2020 203c 6469 7620 6973 3d22         <div is="
+000004a0: 6170 702d 6461 7465 7469 6d65 2d70 6963  app-datetime-pic
+000004b0: 6b65 7222 2069 643d 2274 696d 6573 7461  ker" id="timesta
+000004c0: 6d70 5f6d 696e 2220 747a 6e61 6d65 3d22  mp_min" tzname="
+000004d0: 7b7b 2067 2e63 616d 7061 6967 6e5f 6374  {{ g.campaign_ct
+000004e0: 7874 2e74 7a5f 6e61 6d65 207d 7d22 2061  xt.tz_name }}" a
+000004f0: 732d 6669 6c74 6572 3d22 7472 7565 223e  s-filter="true">
+00000500: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
 00000510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000520: 203c 6469 7620 636c 6173 733d 2263 6f6c   <div class="col
-00000530: 2d31 3220 636f 6c2d 6c67 2d36 2064 2d66  -12 col-lg-6 d-f
-00000540: 6c65 7820 616c 6967 6e2d 6974 656d 732d  lex align-items-
-00000550: 6365 6e74 6572 2067 6170 2d32 223e 0a20  center gap-2">. 
-00000560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000580: 2020 203c 7370 616e 3e42 6574 7765 656e     <span>Between
-00000590: 3c2f 7370 616e 3e0a 2020 2020 2020 2020  </span>.        
+00000520: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
+00000530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000540: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
+00000550: 6976 2063 6c61 7373 3d22 636f 6c2d 3132  iv class="col-12
+00000560: 2063 6f6c 2d6c 672d 3620 642d 666c 6578   col-lg-6 d-flex
+00000570: 2061 6c69 676e 2d69 7465 6d73 2d63 656e   align-items-cen
+00000580: 7465 7220 6761 702d 3222 3e0a 2020 2020  ter gap-2">.    
+00000590: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000005a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005b0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-000005c0: 2069 733d 2261 7070 2d64 6174 6574 696d   is="app-datetim
-000005d0: 652d 7069 636b 6572 2220 6964 3d22 7469  e-picker" id="ti
-000005e0: 6d65 7374 616d 705f 6d69 6e22 2074 7a6e  mestamp_min" tzn
-000005f0: 616d 653d 227b 7b20 672e 6361 6d70 6169  ame="{{ g.campai
-00000600: 676e 5f63 7478 742e 747a 5f6e 616d 6520  gn_ctxt.tz_name 
-00000610: 7d7d 2220 6173 2d66 696c 7465 723d 2274  }}" as-filter="t
-00000620: 7275 6522 3e3c 2f64 6976 3e0a 2020 2020  rue"></div>.    
-00000630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000640: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-00000650: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
+000005b0: 3c73 7061 6e3e 616e 643c 2f73 7061 6e3e  <span>and</span>
+000005c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000005d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005e0: 2020 2020 203c 6469 7620 6973 3d22 6170       <div is="ap
+000005f0: 702d 6461 7465 7469 6d65 2d70 6963 6b65  p-datetime-picke
+00000600: 7222 2069 643d 2274 696d 6573 7461 6d70  r" id="timestamp
+00000610: 5f6d 6178 2220 747a 6e61 6d65 3d22 7b7b  _max" tzname="{{
+00000620: 2067 2e63 616d 7061 6967 6e5f 6374 7874   g.campaign_ctxt
+00000630: 2e74 7a5f 6e61 6d65 207d 7d22 2061 732d  .tz_name }}" as-
+00000640: 6669 6c74 6572 3d22 7472 7565 223e 3c2f  filter="true"></
+00000650: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
 00000660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000670: 2020 203c 6469 7620 636c 6173 733d 2263     <div class="c
-00000680: 6f6c 2d31 3220 636f 6c2d 6c67 2d36 2064  ol-12 col-lg-6 d
-00000690: 2d66 6c65 7820 616c 6967 6e2d 6974 656d  -flex align-item
-000006a0: 732d 6365 6e74 6572 2067 6170 2d32 223e  s-center gap-2">
-000006b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000006c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006d0: 2020 2020 203c 7370 616e 3e61 6e64 3c2f       <span>and</
-000006e0: 7370 616e 3e0a 2020 2020 2020 2020 2020  span>.          
-000006f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000700: 2020 2020 2020 2020 2020 3c64 6976 2069            <div i
-00000710: 733d 2261 7070 2d64 6174 6574 696d 652d  s="app-datetime-
-00000720: 7069 636b 6572 2220 6964 3d22 7469 6d65  picker" id="time
-00000730: 7374 616d 705f 6d61 7822 2074 7a6e 616d  stamp_max" tznam
-00000740: 653d 227b 7b20 672e 6361 6d70 6169 676e  e="{{ g.campaign
-00000750: 5f63 7478 742e 747a 5f6e 616d 6520 7d7d  _ctxt.tz_name }}
-00000760: 2220 6173 2d66 696c 7465 723d 2274 7275  " as-filter="tru
-00000770: 6522 3e3c 2f64 6976 3e0a 2020 2020 2020  e"></div>.      
+00000670: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00000680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000690: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+000006a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006b0: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
+000006c0: 636c 6173 733d 2272 6f77 2064 2d66 6c65  class="row d-fle
+000006d0: 7820 6a75 7374 6966 792d 636f 6e74 656e  x justify-conten
+000006e0: 742d 6265 7477 6565 6e20 616c 6967 6e2d  t-between align-
+000006f0: 6974 656d 732d 6365 6e74 6572 2067 2d32  items-center g-2
+00000700: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
+00000710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000720: 2020 203c 6469 7620 6964 3d22 6669 6c74     <div id="filt
+00000730: 6572 7343 6f6e 7461 696e 6572 2220 636c  ersContainer" cl
+00000740: 6173 733d 2263 6f6c 2d31 3220 636f 6c2d  ass="col-12 col-
+00000750: 6c67 2d61 7574 6f20 642d 666c 6578 2061  lg-auto d-flex a
+00000760: 6c69 676e 2d69 7465 6d73 2d63 656e 7465  lign-items-cente
+00000770: 7220 6761 702d 3222 3e3c 2f64 6976 3e0a  r gap-2"></div>.
 00000780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000790: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-000007a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000007b0: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-000007c0: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+00000790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007a0: 3c64 6976 2063 6c61 7373 3d22 636f 6c2d  <div class="col-
+000007b0: 3132 2063 6f6c 2d6c 672d 6175 746f 223e  12 col-lg-auto">
+000007c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000007d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007e0: 3c64 6976 2063 6c61 7373 3d22 726f 7720  <div class="row 
-000007f0: 642d 666c 6578 206a 7573 7469 6679 2d63  d-flex justify-c
-00000800: 6f6e 7465 6e74 2d62 6574 7765 656e 2061  ontent-between a
-00000810: 6c69 676e 2d69 7465 6d73 2d63 656e 7465  lign-items-cente
-00000820: 7220 672d 3222 3e0a 2020 2020 2020 2020  r g-2">.        
-00000830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000840: 2020 2020 2020 2020 3c64 6976 2069 643d          <div id=
-00000850: 2266 696c 7465 7273 436f 6e74 6169 6e65  "filtersContaine
-00000860: 7222 2063 6c61 7373 3d22 636f 6c2d 3132  r" class="col-12
-00000870: 2063 6f6c 2d6c 672d 6175 746f 2064 2d66   col-lg-auto d-f
-00000880: 6c65 7820 616c 6967 6e2d 6974 656d 732d  lex align-items-
-00000890: 6365 6e74 6572 2067 6170 2d32 223e 3c2f  center gap-2"></
-000008a0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-000008b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008c0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-000008d0: 2263 6f6c 2d31 3220 636f 6c2d 6c67 2d61  "col-12 col-lg-a
-000008e0: 7574 6f22 3e0a 2020 2020 2020 2020 2020  uto">.          
-000008f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000900: 2020 2020 2020 2020 2020 3c61 2069 643d            <a id=
-00000910: 2272 656d 6f76 6546 696c 7465 7273 4274  "removeFiltersBt
-00000920: 6e22 2063 6c61 7373 3d22 6274 6e20 6274  n" class="btn bt
-00000930: 6e2d 736d 2062 746e 2d6f 7574 6c69 6e65  n-sm btn-outline
-00000940: 2d73 6563 6f6e 6461 7279 2074 6578 742d  -secondary text-
-00000950: 6e6f 7772 6170 206d 792d 6175 746f 2077  nowrap my-auto w
-00000960: 2d31 3030 2220 726f 6c65 3d22 6275 7474  -100" role="butt
-00000970: 6f6e 2220 7469 746c 653d 2252 656d 6f76  on" title="Remov
-00000980: 6520 6669 6c74 6572 7322 3e3c 6920 636c  e filters"><i cl
-00000990: 6173 733d 2262 6920 6269 2d65 7261 7365  ass="bi bi-erase
-000009a0: 7222 3e3c 2f69 3e20 5265 6d6f 7665 3c2f  r"></i> Remove</
-000009b0: 613e 0a20 2020 2020 2020 2020 2020 2020  a>.             
-000009c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009d0: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
-000009e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009f0: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
-00000a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a10: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-00000a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a30: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
-00000a40: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-00000a50: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-00000a60: 0a20 2020 2020 2020 203c 2f64 6976 3e0a  .        </div>.
-00000a70: 2020 2020 3c2f 6469 763e 0a20 2020 203c      </div>.    <
-00000a80: 6469 7620 636c 6173 733d 2272 6f77 206d  div class="row m
-00000a90: 622d 3322 3e0a 2020 2020 2020 2020 3c64  b-3">.        <d
-00000aa0: 6976 2063 6c61 7373 3d22 636f 6c22 3e0a  iv class="col">.
-00000ab0: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00000ac0: 2063 6c61 7373 3d22 642d 666c 6578 206a   class="d-flex j
-00000ad0: 7573 7469 6679 2d63 6f6e 7465 6e74 2d73  ustify-content-s
-00000ae0: 7461 7274 2061 6c69 676e 2d69 7465 6d73  tart align-items
-00000af0: 2d63 656e 7465 7220 6761 702d 3322 3e0a  -center gap-3">.
-00000b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b10: 3c75 6c20 6964 3d22 6361 6d70 6169 676e  <ul id="campaign
-00000b20: 5461 6273 2220 636c 6173 733d 226e 6176  Tabs" class="nav
-00000b30: 206e 6176 2d74 6162 7320 6170 702d 7461   nav-tabs app-ta
-00000b40: 6273 2220 726f 6c65 3d22 7461 626c 6973  bs" role="tablis
-00000b50: 7422 3e3c 2f75 6c3e 0a20 2020 2020 2020  t"></ul>.       
-00000b60: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-00000b70: 6173 733d 2262 746e 2d67 726f 7570 223e  ass="btn-group">
-00000b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000b90: 2020 2020 203c 6275 7474 6f6e 2069 643d       <button id=
-00000ba0: 2261 6464 4361 6d70 6169 676e 4472 6f70  "addCampaignDrop
-00000bb0: 446f 776e 2220 7479 7065 3d22 6275 7474  Down" type="butt
-00000bc0: 6f6e 2220 636c 6173 733d 2262 746e 2062  on" class="btn b
-00000bd0: 746e 2d73 6d20 6274 6e2d 6f75 746c 696e  tn-sm btn-outlin
-00000be0: 652d 7072 696d 6172 7920 6472 6f70 646f  e-primary dropdo
-00000bf0: 776e 2d74 6f67 676c 6520 642d 6e6f 6e65  wn-toggle d-none
-00000c00: 2069 6e76 6973 6962 6c65 2220 6461 7461   invisible" data
-00000c10: 2d62 732d 746f 6767 6c65 3d22 6472 6f70  -bs-toggle="drop
-00000c20: 646f 776e 2220 6172 6961 2d65 7870 616e  down" aria-expan
-00000c30: 6465 643d 2266 616c 7365 2220 7469 746c  ded="false" titl
-00000c40: 653d 2249 6e63 6c75 6465 206f 7468 6572  e="Include other
-00000c50: 2063 616d 7061 6967 6e22 3e0a 2020 2020   campaign">.    
-00000c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c70: 2020 2020 3c69 2063 6c61 7373 3d22 6269      <i class="bi
-00000c80: 2062 692d 706c 7573 2d63 6972 636c 6522   bi-plus-circle"
-00000c90: 3e3c 2f69 3e0a 2020 2020 2020 2020 2020  ></i>.          
-00000ca0: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
-00000cb0: 7061 6e20 6964 3d22 6164 6443 616d 7061  pan id="addCampa
-00000cc0: 6967 6e44 726f 7044 6f77 6e4c 6162 656c  ignDropDownLabel
-00000cd0: 223e 496e 636c 7564 6520 6361 6d70 6169  ">Include campai
-00000ce0: 676e 3c2f 7370 616e 3e0a 2020 2020 2020  gn</span>.      
-00000cf0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00000d00: 6275 7474 6f6e 3e0a 2020 2020 2020 2020  button>.        
-00000d10: 2020 2020 2020 2020 2020 2020 3c75 6c20              <ul 
-00000d20: 636c 6173 733d 2264 726f 7064 6f77 6e2d  class="dropdown-
-00000d30: 6d65 6e75 2064 726f 7064 6f77 6e2d 6d65  menu dropdown-me
-00000d40: 6e75 2d65 6e64 2220 6964 3d22 6164 6443  nu-end" id="addC
-00000d50: 616d 7061 6967 6e44 726f 7044 6f77 6e4c  ampaignDropDownL
-00000d60: 6973 7422 2061 7269 612d 6c61 6265 6c6c  ist" aria-labell
-00000d70: 6564 6279 3d22 6164 6443 616d 7061 6967  edby="addCampaig
-00000d80: 6e44 726f 7044 6f77 6e22 3e3c 2f75 6c3e  nDropDown"></ul>
-00000d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000da0: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
-00000db0: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-00000dc0: 2020 2020 2020 203c 6469 7620 6964 3d22         <div id="
-00000dd0: 6361 6d70 6169 676e 5461 6243 6f6e 7465  campaignTabConte
-00000de0: 6e74 7322 2063 6c61 7373 3d22 7461 622d  nts" class="tab-
-00000df0: 636f 6e74 656e 7420 6f76 6572 666c 6f77  content overflow
-00000e00: 2d61 7574 6f20 626f 7264 6572 2062 6f72  -auto border bor
-00000e10: 6465 722d 746f 702d 3020 6267 2d77 6869  der-top-0 bg-whi
-00000e20: 7465 223e 3c2f 6469 763e 0a20 2020 2020  te"></div>.     
-00000e30: 2020 203c 2f64 6976 3e0a 2020 2020 3c2f     </div>.    </
-00000e40: 6469 763e 0a3c 2f64 6976 3e0a 3c64 6976  div>.</div>.<div
-00000e50: 2063 6c61 7373 3d22 6d6f 6461 6c22 2069   class="modal" i
-00000e60: 643d 226e 6f74 6966 496e 666f 4d6f 6461  d="notifInfoModa
-00000e70: 6c22 2064 6174 612d 6273 2d6b 6579 626f  l" data-bs-keybo
-00000e80: 6172 643d 2274 7275 6522 2074 6162 696e  ard="true" tabin
-00000e90: 6465 783d 222d 3122 2061 7269 612d 6c61  dex="-1" aria-la
-00000ea0: 6265 6c6c 6564 6279 3d22 6e6f 7469 6649  belledby="notifI
-00000eb0: 6e66 6f4d 6f64 616c 5469 746c 6522 2061  nfoModalTitle" a
-00000ec0: 7269 612d 6869 6464 656e 3d22 7472 7565  ria-hidden="true
-00000ed0: 223e 0a20 2020 203c 6469 7620 636c 6173  ">.    <div clas
-00000ee0: 733d 226d 6f64 616c 2d64 6961 6c6f 6720  s="modal-dialog 
-00000ef0: 6d6f 6461 6c2d 786c 206d 6f64 616c 2d64  modal-xl modal-d
-00000f00: 6961 6c6f 672d 6365 6e74 6572 6564 206d  ialog-centered m
-00000f10: 6f64 616c 2d64 6961 6c6f 672d 7363 726f  odal-dialog-scro
-00000f20: 6c6c 6162 6c65 2220 7374 796c 653d 2268  llable" style="h
-00000f30: 6569 6768 743a 2039 3025 3b22 3e0a 2020  eight: 90%;">.  
-00000f40: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
-00000f50: 3d22 6d6f 6461 6c2d 636f 6e74 656e 7422  ="modal-content"
-00000f60: 2073 7479 6c65 3d22 6865 6967 6874 3a20   style="height: 
-00000f70: 3930 253b 223e 0a20 2020 2020 2020 2020  90%;">.         
-00000f80: 2020 203c 6469 7620 636c 6173 733d 226d     <div class="m
-00000f90: 6f64 616c 2d68 6561 6465 7222 3e0a 2020  odal-header">.  
-00000fa0: 2020 2020 2020 2020 2020 2020 2020 3c68                <h
-00000fb0: 3520 636c 6173 733d 226d 6f64 616c 2d74  5 class="modal-t
-00000fc0: 6974 6c65 2066 6f6e 742d 6d6f 6e6f 7370  itle font-monosp
-00000fd0: 6163 6522 2069 643d 226e 6f74 6966 496e  ace" id="notifIn
-00000fe0: 666f 4d6f 6461 6c54 6974 6c65 223e 4e6f  foModalTitle">No
-00000ff0: 7469 6669 6361 7469 6f6e 2069 6e66 6f72  tification infor
-00001000: 6d61 7469 6f6e 3c2f 6835 3e0a 2020 2020  mation</h5>.    
-00001010: 2020 2020 2020 2020 2020 2020 3c62 7574              <but
-00001020: 746f 6e20 7479 7065 3d22 6275 7474 6f6e  ton type="button
-00001030: 2220 636c 6173 733d 2262 746e 2d63 6c6f  " class="btn-clo
-00001040: 7365 2220 6461 7461 2d62 732d 6469 736d  se" data-bs-dism
-00001050: 6973 733d 226d 6f64 616c 2220 6172 6961  iss="modal" aria
-00001060: 2d6c 6162 656c 3d22 436c 6f73 6522 3e3c  -label="Close"><
-00001070: 2f62 7574 746f 6e3e 0a20 2020 2020 2020  /button>.       
-00001080: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-00001090: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
-000010a0: 7373 3d22 6d6f 6461 6c2d 626f 6479 2220  ss="modal-body" 
-000010b0: 7374 796c 653d 2268 6569 6768 743a 2063  style="height: c
-000010c0: 616c 6328 3130 3025 202d 2031 3335 7078  alc(100% - 135px
-000010d0: 293b 223e 0a20 2020 2020 2020 2020 2020  );">.           
-000010e0: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-000010f0: 2272 6f77 206d 622d 3322 2069 643d 226e  "row mb-3" id="n
-00001100: 6f74 6966 496e 666f 436f 6e74 6169 6e65  otifInfoContaine
-00001110: 7222 3e3c 2f64 6976 3e0a 2020 2020 2020  r"></div>.      
-00001120: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
-00001130: 6c61 7373 3d22 726f 7720 6d62 2d33 223e  lass="row mb-3">
-00001140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001150: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00001160: 2263 6f6c 223e 0a20 2020 2020 2020 2020  "col">.         
-00001170: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001180: 6469 7620 636c 6173 733d 2274 6162 6c65  div class="table
-00001190: 2d72 6573 706f 6e73 6976 652d 786c 223e  -responsive-xl">
-000011a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000011b0: 2020 2020 2020 2020 2020 2020 203c 7461               <ta
-000011c0: 626c 6520 636c 6173 733d 2274 6162 6c65  ble class="table
-000011d0: 2074 6162 6c65 2d73 6d20 7461 626c 652d   table-sm table-
-000011e0: 686f 7665 7220 7461 626c 652d 626f 7264  hover table-bord
-000011f0: 6572 6564 2063 6170 7469 6f6e 2d74 6f70  ered caption-top
-00001200: 2220 6964 3d22 6576 656e 7473 5461 626c  " id="eventsTabl
-00001210: 6522 3e0a 2020 2020 2020 2020 2020 2020  e">.            
-00001220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001230: 2020 2020 3c63 6170 7469 6f6e 3e4e 6f74      <caption>Not
-00001240: 6966 6965 6420 6576 656e 7420 696e 666f  ified event info
-00001250: 726d 6174 696f 6e3c 2f63 6170 7469 6f6e  rmation</caption
-00001260: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000007e0: 2020 2020 203c 6120 6964 3d22 7265 6d6f       <a id="remo
+000007f0: 7665 4669 6c74 6572 7342 746e 2220 636c  veFiltersBtn" cl
+00000800: 6173 733d 2262 746e 2062 746e 2d73 6d20  ass="btn btn-sm 
+00000810: 6274 6e2d 6f75 746c 696e 652d 7365 636f  btn-outline-seco
+00000820: 6e64 6172 7920 7465 7874 2d6e 6f77 7261  ndary text-nowra
+00000830: 7020 6d79 2d61 7574 6f20 772d 3130 3022  p my-auto w-100"
+00000840: 2072 6f6c 653d 2262 7574 746f 6e22 2074   role="button" t
+00000850: 6974 6c65 3d22 5265 6d6f 7665 2066 696c  itle="Remove fil
+00000860: 7465 7273 223e 3c69 2063 6c61 7373 3d22  ters"><i class="
+00000870: 6269 2062 692d 6572 6173 6572 223e 3c2f  bi bi-eraser"></
+00000880: 693e 2052 656d 6f76 653c 2f61 3e0a 2020  i> Remove</a>.  
+00000890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008a0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+000008b0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+000008c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008d0: 203c 2f64 6976 3e0a 2020 2020 2020 2020   </div>.        
+000008e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008f0: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00000900: 2020 2020 2020 2020 2020 203c 2f64 6976             </div
+00000910: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00000920: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+00000930: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+00000940: 2020 2020 3c2f 6469 763e 0a20 2020 203c      </div>.    <
+00000950: 2f64 6976 3e0a 2020 2020 3c64 6976 2063  /div>.    <div c
+00000960: 6c61 7373 3d22 726f 7720 6d62 2d33 223e  lass="row mb-3">
+00000970: 0a20 2020 2020 2020 203c 6469 7620 636c  .        <div cl
+00000980: 6173 733d 2263 6f6c 223e 0a20 2020 2020  ass="col">.     
+00000990: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+000009a0: 733d 2264 2d66 6c65 7820 6a75 7374 6966  s="d-flex justif
+000009b0: 792d 636f 6e74 656e 742d 7374 6172 7420  y-content-start 
+000009c0: 616c 6967 6e2d 6974 656d 732d 6365 6e74  align-items-cent
+000009d0: 6572 2067 6170 2d33 223e 0a20 2020 2020  er gap-3">.     
+000009e0: 2020 2020 2020 2020 2020 203c 756c 2069             <ul i
+000009f0: 643d 2263 616d 7061 6967 6e54 6162 7322  d="campaignTabs"
+00000a00: 2063 6c61 7373 3d22 6e61 7620 6e61 762d   class="nav nav-
+00000a10: 7461 6273 2061 7070 2d74 6162 7322 2072  tabs app-tabs" r
+00000a20: 6f6c 653d 2274 6162 6c69 7374 223e 3c2f  ole="tablist"></
+00000a30: 756c 3e0a 2020 2020 2020 2020 2020 2020  ul>.            
+00000a40: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
+00000a50: 6274 6e2d 6772 6f75 7022 3e0a 2020 2020  btn-group">.    
+00000a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000a70: 3c62 7574 746f 6e20 6964 3d22 6164 6443  <button id="addC
+00000a80: 616d 7061 6967 6e44 726f 7044 6f77 6e22  ampaignDropDown"
+00000a90: 2074 7970 653d 2262 7574 746f 6e22 2063   type="button" c
+00000aa0: 6c61 7373 3d22 6274 6e20 6274 6e2d 736d  lass="btn btn-sm
+00000ab0: 2062 746e 2d6f 7574 6c69 6e65 2d70 7269   btn-outline-pri
+00000ac0: 6d61 7279 2064 726f 7064 6f77 6e2d 746f  mary dropdown-to
+00000ad0: 6767 6c65 2064 2d6e 6f6e 6520 696e 7669  ggle d-none invi
+00000ae0: 7369 626c 6522 2064 6174 612d 6273 2d74  sible" data-bs-t
+00000af0: 6f67 676c 653d 2264 726f 7064 6f77 6e22  oggle="dropdown"
+00000b00: 2061 7269 612d 6578 7061 6e64 6564 3d22   aria-expanded="
+00000b10: 6661 6c73 6522 2074 6974 6c65 3d22 496e  false" title="In
+00000b20: 636c 7564 6520 6f74 6865 7220 6361 6d70  clude other camp
+00000b30: 6169 676e 223e 0a20 2020 2020 2020 2020  aign">.         
+00000b40: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00000b50: 6920 636c 6173 733d 2262 6920 6269 2d70  i class="bi bi-p
+00000b60: 6c75 732d 6369 7263 6c65 223e 3c2f 693e  lus-circle"></i>
+00000b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000b80: 2020 2020 2020 2020 203c 7370 616e 2069           <span i
+00000b90: 643d 2261 6464 4361 6d70 6169 676e 4472  d="addCampaignDr
+00000ba0: 6f70 446f 776e 4c61 6265 6c22 3e49 6e63  opDownLabel">Inc
+00000bb0: 6c75 6465 2063 616d 7061 6967 6e3c 2f73  lude campaign</s
+00000bc0: 7061 6e3e 0a20 2020 2020 2020 2020 2020  pan>.           
+00000bd0: 2020 2020 2020 2020 203c 2f62 7574 746f           </butto
+00000be0: 6e3e 0a20 2020 2020 2020 2020 2020 2020  n>.             
+00000bf0: 2020 2020 2020 203c 756c 2063 6c61 7373         <ul class
+00000c00: 3d22 6472 6f70 646f 776e 2d6d 656e 7520  ="dropdown-menu 
+00000c10: 6472 6f70 646f 776e 2d6d 656e 752d 656e  dropdown-menu-en
+00000c20: 6422 2069 643d 2261 6464 4361 6d70 6169  d" id="addCampai
+00000c30: 676e 4472 6f70 446f 776e 4c69 7374 2220  gnDropDownList" 
+00000c40: 6172 6961 2d6c 6162 656c 6c65 6462 793d  aria-labelledby=
+00000c50: 2261 6464 4361 6d70 6169 676e 4472 6f70  "addCampaignDrop
+00000c60: 446f 776e 223e 3c2f 756c 3e0a 2020 2020  Down"></ul>.    
+00000c70: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
+00000c80: 763e 0a20 2020 2020 2020 2020 2020 203c  v>.            <
+00000c90: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00000ca0: 2020 3c64 6976 2069 643d 2263 616d 7061    <div id="campa
+00000cb0: 6967 6e54 6162 436f 6e74 656e 7473 2220  ignTabContents" 
+00000cc0: 636c 6173 733d 2274 6162 2d63 6f6e 7465  class="tab-conte
+00000cd0: 6e74 206f 7665 7266 6c6f 772d 6175 746f  nt overflow-auto
+00000ce0: 2062 6f72 6465 7220 626f 7264 6572 2d74   border border-t
+00000cf0: 6f70 2d30 2062 672d 7768 6974 6522 3e3c  op-0 bg-white"><
+00000d00: 2f64 6976 3e0a 2020 2020 2020 2020 3c2f  /div>.        </
+00000d10: 6469 763e 0a20 2020 203c 2f64 6976 3e0a  div>.    </div>.
+00000d20: 3c2f 6469 763e 0a3c 6469 7620 636c 6173  </div>.<div clas
+00000d30: 733d 226d 6f64 616c 2220 6964 3d22 6e6f  s="modal" id="no
+00000d40: 7469 6649 6e66 6f4d 6f64 616c 2220 6461  tifInfoModal" da
+00000d50: 7461 2d62 732d 6b65 7962 6f61 7264 3d22  ta-bs-keyboard="
+00000d60: 7472 7565 2220 7461 6269 6e64 6578 3d22  true" tabindex="
+00000d70: 2d31 2220 6172 6961 2d6c 6162 656c 6c65  -1" aria-labelle
+00000d80: 6462 793d 226e 6f74 6966 496e 666f 4d6f  dby="notifInfoMo
+00000d90: 6461 6c54 6974 6c65 2220 6172 6961 2d68  dalTitle" aria-h
+00000da0: 6964 6465 6e3d 2274 7275 6522 3e0a 2020  idden="true">.  
+00000db0: 2020 3c64 6976 2063 6c61 7373 3d22 6d6f    <div class="mo
+00000dc0: 6461 6c2d 6469 616c 6f67 206d 6f64 616c  dal-dialog modal
+00000dd0: 2d78 6c20 6d6f 6461 6c2d 6469 616c 6f67  -xl modal-dialog
+00000de0: 2d63 656e 7465 7265 6420 6d6f 6461 6c2d  -centered modal-
+00000df0: 6469 616c 6f67 2d73 6372 6f6c 6c61 626c  dialog-scrollabl
+00000e00: 6522 2073 7479 6c65 3d22 6865 6967 6874  e" style="height
+00000e10: 3a20 3930 253b 223e 0a20 2020 2020 2020  : 90%;">.       
+00000e20: 203c 6469 7620 636c 6173 733d 226d 6f64   <div class="mod
+00000e30: 616c 2d63 6f6e 7465 6e74 2220 7374 796c  al-content" styl
+00000e40: 653d 2268 6569 6768 743a 2039 3025 3b22  e="height: 90%;"
+00000e50: 3e0a 2020 2020 2020 2020 2020 2020 3c64  >.            <d
+00000e60: 6976 2063 6c61 7373 3d22 6d6f 6461 6c2d  iv class="modal-
+00000e70: 6865 6164 6572 223e 0a20 2020 2020 2020  header">.       
+00000e80: 2020 2020 2020 2020 203c 6835 2063 6c61           <h5 cla
+00000e90: 7373 3d22 6d6f 6461 6c2d 7469 746c 6520  ss="modal-title 
+00000ea0: 666f 6e74 2d6d 6f6e 6f73 7061 6365 2220  font-monospace" 
+00000eb0: 6964 3d22 6e6f 7469 6649 6e66 6f4d 6f64  id="notifInfoMod
+00000ec0: 616c 5469 746c 6522 3e4e 6f74 6966 6963  alTitle">Notific
+00000ed0: 6174 696f 6e20 696e 666f 726d 6174 696f  ation informatio
+00000ee0: 6e3c 2f68 353e 0a20 2020 2020 2020 2020  n</h5>.         
+00000ef0: 2020 2020 2020 203c 6275 7474 6f6e 2074         <button t
+00000f00: 7970 653d 2262 7574 746f 6e22 2063 6c61  ype="button" cla
+00000f10: 7373 3d22 6274 6e2d 636c 6f73 6522 2064  ss="btn-close" d
+00000f20: 6174 612d 6273 2d64 6973 6d69 7373 3d22  ata-bs-dismiss="
+00000f30: 6d6f 6461 6c22 2061 7269 612d 6c61 6265  modal" aria-labe
+00000f40: 6c3d 2243 6c6f 7365 223e 3c2f 6275 7474  l="Close"></butt
+00000f50: 6f6e 3e0a 2020 2020 2020 2020 2020 2020  on>.            
+00000f60: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00000f70: 2020 203c 6469 7620 636c 6173 733d 226d     <div class="m
+00000f80: 6f64 616c 2d62 6f64 7922 2073 7479 6c65  odal-body" style
+00000f90: 3d22 6865 6967 6874 3a20 6361 6c63 2831  ="height: calc(1
+00000fa0: 3030 2520 2d20 3133 3570 7829 3b22 3e0a  00% - 135px);">.
+00000fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fc0: 3c64 6976 2063 6c61 7373 3d22 726f 7720  <div class="row 
+00000fd0: 6d62 2d33 2220 6964 3d22 6e6f 7469 6649  mb-3" id="notifI
+00000fe0: 6e66 6f43 6f6e 7461 696e 6572 223e 3c2f  nfoContainer"></
+00000ff0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00001000: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00001010: 2272 6f77 206d 622d 3322 3e0a 2020 2020  "row mb-3">.    
+00001020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001030: 3c64 6976 2063 6c61 7373 3d22 636f 6c22  <div class="col"
+00001040: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00001050: 2020 2020 2020 2020 2020 3c64 6976 2063            <div c
+00001060: 6c61 7373 3d22 7461 626c 652d 7265 7370  lass="table-resp
+00001070: 6f6e 7369 7665 2d78 6c22 3e0a 2020 2020  onsive-xl">.    
+00001080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001090: 2020 2020 2020 2020 3c74 6162 6c65 2063          <table c
+000010a0: 6c61 7373 3d22 7461 626c 6520 7461 626c  lass="table tabl
+000010b0: 652d 736d 2074 6162 6c65 2d68 6f76 6572  e-sm table-hover
+000010c0: 2074 6162 6c65 2d62 6f72 6465 7265 6420   table-bordered 
+000010d0: 6361 7074 696f 6e2d 746f 7022 2069 643d  caption-top" id=
+000010e0: 2265 7665 6e74 7354 6162 6c65 223e 0a20  "eventsTable">. 
+000010f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001100: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001110: 6361 7074 696f 6e3e 4e6f 7469 6669 6564  caption>Notified
+00001120: 2065 7665 6e74 2069 6e66 6f72 6d61 7469   event informati
+00001130: 6f6e 3c2f 6361 7074 696f 6e3e 0a20 2020  on</caption>.   
+00001140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001150: 2020 2020 2020 2020 2020 2020 203c 7468               <th
+00001160: 6561 643e 0a20 2020 2020 2020 2020 2020  ead>.           
+00001170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001180: 2020 2020 2020 2020 203c 7472 2063 6c61           <tr cla
+00001190: 7373 3d22 616c 6967 6e2d 746f 7022 3e0a  ss="align-top">.
+000011a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011c0: 2020 2020 2020 2020 3c74 6820 7363 6f70          <th scop
+000011d0: 653d 2263 6f6c 223e 5469 6d65 7374 616d  e="col">Timestam
+000011e0: 703c 2f74 683e 0a20 2020 2020 2020 2020  p</th>.         
+000011f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001200: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001210: 7468 2073 636f 7065 3d22 636f 6c22 3e53  th scope="col">S
+00001220: 6f75 7263 653c 2f74 683e 0a20 2020 2020  ource</th>.     
+00001230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001250: 2020 203c 7468 2073 636f 7065 3d22 636f     <th scope="co
+00001260: 6c22 3e4c 6576 656c 3c2f 7468 3e0a 2020  l">Level</th>.  
 00001270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001280: 2020 3c74 6865 6164 3e0a 2020 2020 2020    <thead>.      
-00001290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012a0: 2020 2020 2020 2020 2020 2020 2020 3c74                <t
-000012b0: 7220 636c 6173 733d 2261 6c69 676e 2d74  r class="align-t
-000012c0: 6f70 223e 0a20 2020 2020 2020 2020 2020  op">.           
-000012d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012e0: 2020 2020 2020 2020 2020 2020 203c 7468               <th
-000012f0: 2073 636f 7065 3d22 636f 6c22 3e54 696d   scope="col">Tim
-00001300: 6573 7461 6d70 3c2f 7468 3e0a 2020 2020  estamp</th>.    
+00001280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001290: 2020 2020 2020 3c74 6820 7363 6f70 653d        <th scope=
+000012a0: 2263 6f6c 223e 4361 7465 676f 7279 3c2f  "col">Category</
+000012b0: 7468 3e0a 2020 2020 2020 2020 2020 2020  th>.            
+000012c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012d0: 2020 2020 2020 2020 2020 2020 3c74 6820              <th 
+000012e0: 7363 6f70 653d 2263 6f6c 223e 4361 6d70  scope="col">Camp
+000012f0: 6169 676e 2073 636f 7065 3c2f 7468 3e0a  aign scope</th>.
+00001300: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001330: 2020 2020 3c74 6820 7363 6f70 653d 2263      <th scope="c
-00001340: 6f6c 223e 536f 7572 6365 3c2f 7468 3e0a  ol">Source</th>.
-00001350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001320: 2020 2020 3c2f 7472 3e0a 2020 2020 2020      </tr>.      
+00001330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001340: 2020 2020 2020 2020 2020 3c2f 7468 6561            </thea
+00001350: 643e 0a20 2020 2020 2020 2020 2020 2020  d>.             
 00001360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001370: 2020 2020 2020 2020 3c74 6820 7363 6f70          <th scop
-00001380: 653d 2263 6f6c 223e 4c65 7665 6c3c 2f74  e="col">Level</t
-00001390: 683e 0a20 2020 2020 2020 2020 2020 2020  h>.             
-000013a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013b0: 2020 2020 2020 2020 2020 203c 7468 2073             <th s
-000013c0: 636f 7065 3d22 636f 6c22 3e43 6174 6567  cope="col">Categ
-000013d0: 6f72 793c 2f74 683e 0a20 2020 2020 2020  ory</th>.       
+00001370: 2020 203c 7462 6f64 7920 636c 6173 733d     <tbody class=
+00001380: 2274 6162 6c65 2d67 726f 7570 2d64 6976  "table-group-div
+00001390: 6964 6572 2220 6964 3d22 6576 656e 7449  ider" id="eventI
+000013a0: 6e66 6f43 6f6e 7461 696e 6572 223e 0a20  nfoContainer">. 
+000013b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013d0: 2020 203c 7472 3e0a 2020 2020 2020 2020     <tr>.        
 000013e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000013f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001400: 203c 7468 2073 636f 7065 3d22 636f 6c22   <th scope="col"
-00001410: 3e43 616d 7061 6967 6e20 7363 6f70 653c  >Campaign scope<
-00001420: 2f74 683e 0a20 2020 2020 2020 2020 2020  /th>.           
+00001400: 3c74 6420 636f 6c73 7061 6e3d 2235 2220  <td colspan="5" 
+00001410: 636c 6173 733d 2274 6578 742d 6365 6e74  class="text-cent
+00001420: 6572 2070 2d34 223e 0a20 2020 2020 2020  er p-4">.       
 00001430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001440: 2020 2020 2020 2020 203c 2f74 723e 0a20           </tr>. 
-00001450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001460: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001470: 2f74 6865 6164 3e0a 2020 2020 2020 2020  /thead>.        
+00001440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001450: 2020 2020 203c 6469 7620 6973 3d22 6170       <div is="ap
+00001460: 702d 7370 696e 6e65 7222 3e3c 2f64 6976  p-spinner"></div
+00001470: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
 00001480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001490: 2020 2020 2020 2020 3c74 626f 6479 2063          <tbody c
-000014a0: 6c61 7373 3d22 7461 626c 652d 6772 6f75  lass="table-grou
-000014b0: 702d 6469 7669 6465 7222 2069 643d 2265  p-divider" id="e
-000014c0: 7665 6e74 496e 666f 436f 6e74 6169 6e65  ventInfoContaine
-000014d0: 7222 3e0a 2020 2020 2020 2020 2020 2020  r">.            
-000014e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000014f0: 2020 2020 2020 2020 3c74 723e 0a20 2020          <tr>.   
+00001490: 2020 2020 2020 2020 2020 3c2f 7464 3e0a            </td>.
+000014a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014c0: 2020 2020 3c2f 7472 3e0a 2020 2020 2020      </tr>.      
+000014d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014e0: 2020 2020 2020 2020 2020 3c2f 7462 6f64            </tbod
+000014f0: 793e 0a20 2020 2020 2020 2020 2020 2020  y>.             
 00001500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001520: 2020 2020 203c 7464 2063 6f6c 7370 616e       <td colspan
-00001530: 3d22 3522 2063 6c61 7373 3d22 7465 7874  ="5" class="text
-00001540: 2d63 656e 7465 7220 702d 3422 3e0a 2020  -center p-4">.  
+00001510: 2020 203c 7466 6f6f 743e 0a20 2020 2020     <tfoot>.     
+00001520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001530: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001540: 7472 3e0a 2020 2020 2020 2020 2020 2020  tr>.            
 00001550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001570: 2020 2020 2020 2020 2020 3c64 6976 2069            <div i
-00001580: 733d 2261 7070 2d73 7069 6e6e 6572 223e  s="app-spinner">
-00001590: 3c2f 6469 763e 0a20 2020 2020 2020 2020  </div>.         
+00001560: 2020 2020 2020 2020 2020 2020 3c74 6420              <td 
+00001570: 636f 6c73 7061 6e3d 2235 2220 6964 3d22  colspan="5" id="
+00001580: 6576 656e 7449 6e66 6f44 6573 6372 6970  eventInfoDescrip
+00001590: 7469 6f6e 223e 2d3c 2f74 643e 0a20 2020  tion">-</td>.   
 000015a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015b0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-000015c0: 2f74 643e 0a20 2020 2020 2020 2020 2020  /td>.           
+000015b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015c0: 203c 2f74 723e 0a20 2020 2020 2020 2020   </tr>.         
 000015d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015e0: 2020 2020 2020 2020 203c 2f74 723e 0a20           </tr>. 
+000015e0: 2020 2020 2020 203c 2f74 666f 6f74 3e0a         </tfoot>.
 000015f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001600: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001610: 2f74 626f 6479 3e0a 2020 2020 2020 2020  /tbody>.        
-00001620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001630: 2020 2020 2020 2020 3c74 666f 6f74 3e0a          <tfoot>.
-00001640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001660: 2020 2020 3c74 723e 0a20 2020 2020 2020      <tr>.       
-00001670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001690: 203c 7464 2063 6f6c 7370 616e 3d22 3522   <td colspan="5"
-000016a0: 2069 643d 2265 7665 6e74 496e 666f 4465   id="eventInfoDe
-000016b0: 7363 7269 7074 696f 6e22 3e2d 3c2f 7464  scription">-</td
-000016c0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-000016d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016e0: 2020 2020 2020 3c2f 7472 3e0a 2020 2020        </tr>.    
-000016f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001700: 2020 2020 2020 2020 2020 2020 3c2f 7466              </tf
-00001710: 6f6f 743e 0a20 2020 2020 2020 2020 2020  oot>.           
-00001720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001730: 203c 2f74 6162 6c65 3e0a 2020 2020 2020   </table>.      
-00001740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001750: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
-00001760: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
-00001770: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
-00001780: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-00001790: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-000017a0: 6973 3d22 6170 702d 7370 696e 6e65 7222  is="app-spinner"
-000017b0: 2069 643d 2265 7665 6e74 496e 666f 5461   id="eventInfoTa
-000017c0: 6253 7069 6e6e 6572 2220 636c 6173 733d  bSpinner" class=
-000017d0: 2264 2d6e 6f6e 6522 3e3c 2f64 6976 3e0a  "d-none"></div>.
-000017e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017f0: 3c75 6c20 6964 3d22 6576 656e 7449 6e66  <ul id="eventInf
-00001800: 6f54 6162 7322 2063 6c61 7373 3d22 6e61  oTabs" class="na
-00001810: 7620 6e61 762d 7461 6273 2061 7070 2d74  v nav-tabs app-t
-00001820: 6162 7320 6a75 7374 6966 792d 636f 6e74  abs justify-cont
-00001830: 656e 742d 6365 6e74 6572 2064 2d6e 6f6e  ent-center d-non
-00001840: 6522 2072 6f6c 653d 2274 6162 6c69 7374  e" role="tablist
-00001850: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00001860: 2020 2020 2020 203c 6c69 2063 6c61 7373         <li class
-00001870: 3d22 6e61 762d 6974 656d 2220 726f 6c65  ="nav-item" role
-00001880: 3d22 7072 6573 656e 7461 7469 6f6e 223e  ="presentation">
-00001890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000018a0: 2020 2020 2020 2020 203c 6275 7474 6f6e           <button
-000018b0: 2063 6c61 7373 3d22 6e61 762d 6c69 6e6b   class="nav-link
-000018c0: 2061 6374 6976 6522 2069 643d 2274 732d   active" id="ts-
-000018d0: 7461 6222 2064 6174 612d 6273 2d74 6f67  tab" data-bs-tog
-000018e0: 676c 653d 2274 6162 2220 6461 7461 2d62  gle="tab" data-b
-000018f0: 732d 7461 7267 6574 3d22 2374 732d 7461  s-target="#ts-ta
-00001900: 6263 6f6e 7465 6e74 2220 7479 7065 3d22  bcontent" type="
-00001910: 6275 7474 6f6e 2220 726f 6c65 3d22 7461  button" role="ta
-00001920: 6222 2061 7269 612d 636f 6e74 726f 6c73  b" aria-controls
-00001930: 3d22 7473 2d74 6162 636f 6e74 656e 7422  ="ts-tabcontent"
-00001940: 2061 7269 612d 7365 6c65 6374 6564 3d22   aria-selected="
-00001950: 6661 6c73 6522 3e54 696d 6573 6572 6965  false">Timeserie
-00001960: 7320 3c73 7061 6e20 636c 6173 733d 2262  s <span class="b
-00001970: 6164 6765 2062 672d 7365 636f 6e64 6172  adge bg-secondar
-00001980: 7922 2069 643d 2274 7354 6f74 616c 436f  y" id="tsTotalCo
-00001990: 756e 7422 3e30 3c2f 7370 616e 3e3c 2f62  unt">0</span></b
-000019a0: 7574 746f 6e3e 0a20 2020 2020 2020 2020  utton>.         
-000019b0: 2020 2020 2020 2020 2020 203c 2f6c 693e             </li>
-000019c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000019d0: 2020 2020 207b 2520 666f 7220 7374 7275       {% for stru
-000019e0: 6374 5f65 6c6d 745f 7479 7065 2069 6e20  ct_elmt_type in 
-000019f0: 7374 7275 6374 7572 616c 5f65 6c65 6d65  structural_eleme
-00001a00: 6e74 5f74 7970 6573 2025 7d0a 2020 2020  nt_types %}.    
-00001a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a20: 3c6c 6920 636c 6173 733d 226e 6176 2d69  <li class="nav-i
-00001a30: 7465 6d22 2072 6f6c 653d 2270 7265 7365  tem" role="prese
-00001a40: 6e74 6174 696f 6e22 3e0a 2020 2020 2020  ntation">.      
-00001a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a60: 2020 3c62 7574 746f 6e20 636c 6173 733d    <button class=
-00001a70: 226e 6176 2d6c 696e 6b22 2069 643d 227b  "nav-link" id="{
-00001a80: 7b20 7374 7275 6374 5f65 6c6d 745f 7479  { struct_elmt_ty
-00001a90: 7065 207d 7d73 2d74 6162 2220 6461 7461  pe }}s-tab" data
-00001aa0: 2d62 732d 746f 6767 6c65 3d22 7461 6222  -bs-toggle="tab"
-00001ab0: 2064 6174 612d 6273 2d74 6172 6765 743d   data-bs-target=
-00001ac0: 2223 7b7b 2073 7472 7563 745f 656c 6d74  "#{{ struct_elmt
-00001ad0: 5f74 7970 6520 7d7d 732d 7461 6263 6f6e  _type }}s-tabcon
-00001ae0: 7465 6e74 2220 7479 7065 3d22 6275 7474  tent" type="butt
-00001af0: 6f6e 2220 726f 6c65 3d22 7461 6222 2061  on" role="tab" a
-00001b00: 7269 612d 636f 6e74 726f 6c73 3d22 7b7b  ria-controls="{{
-00001b10: 2073 7472 7563 745f 656c 6d74 5f74 7970   struct_elmt_typ
-00001b20: 6520 7d7d 732d 7461 6263 6f6e 7465 6e74  e }}s-tabcontent
-00001b30: 2220 6172 6961 2d73 656c 6563 7465 643d  " aria-selected=
-00001b40: 2266 616c 7365 223e 7b7b 2073 7472 7563  "false">{{ struc
-00001b50: 745f 656c 6d74 5f74 7970 6520 7c20 6361  t_elmt_type | ca
-00001b60: 7069 7461 6c69 7a65 207d 7d73 203c 7370  pitalize }}s <sp
-00001b70: 616e 2063 6c61 7373 3d22 6261 6467 6520  an class="badge 
-00001b80: 6267 2d73 6563 6f6e 6461 7279 2220 6964  bg-secondary" id
-00001b90: 3d22 7b7b 2073 7472 7563 745f 656c 6d74  ="{{ struct_elmt
-00001ba0: 5f74 7970 6520 7d7d 7354 6f74 616c 436f  _type }}sTotalCo
-00001bb0: 756e 7422 3e30 3c2f 7370 616e 3e3c 2f62  unt">0</span></b
-00001bc0: 7574 746f 6e3e 0a20 2020 2020 2020 2020  utton>.         
-00001bd0: 2020 2020 2020 2020 2020 203c 2f6c 693e             </li>
-00001be0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001bf0: 2020 2020 207b 2520 656e 6466 6f72 2025       {% endfor %
-00001c00: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00001c10: 2020 3c2f 756c 3e0a 2020 2020 2020 2020    </ul>.        
-00001c20: 2020 2020 2020 2020 3c64 6976 2069 643d          <div id=
-00001c30: 2265 7665 6e74 496e 666f 5461 6243 6f6e  "eventInfoTabCon
-00001c40: 7465 6e74 7322 2063 6c61 7373 3d22 7461  tents" class="ta
-00001c50: 622d 636f 6e74 656e 7420 6f76 6572 666c  b-content overfl
-00001c60: 6f77 2d61 7574 6f20 626f 7264 6572 2062  ow-auto border b
-00001c70: 6f72 6465 722d 746f 702d 3020 6267 2d77  order-top-0 bg-w
-00001c80: 6869 7465 2064 2d6e 6f6e 6522 3e0a 2020  hite d-none">.  
-00001c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ca0: 2020 3c64 6976 2063 6c61 7373 3d22 7461    <div class="ta
-00001cb0: 622d 7061 6e65 2073 686f 7720 6163 7469  b-pane show acti
-00001cc0: 7665 2070 2d33 2220 6964 3d22 7473 2d74  ve p-3" id="ts-t
-00001cd0: 6162 636f 6e74 656e 7422 2072 6f6c 653d  abcontent" role=
-00001ce0: 2274 6162 7061 6e65 6c22 2061 7269 612d  "tabpanel" aria-
-00001cf0: 6c61 6265 6c6c 6564 6279 3d22 7473 2d74  labelledby="ts-t
-00001d00: 6162 223e 0a20 2020 2020 2020 2020 2020  ab">.           
-00001d10: 2020 2020 2020 2020 2020 2020 203c 6469               <di
-00001d20: 7620 636c 6173 733d 2264 2d66 6c65 7820  v class="d-flex 
-00001d30: 6a75 7374 6966 792d 636f 6e74 656e 742d  justify-content-
-00001d40: 656e 6420 616c 6967 6e2d 6974 656d 732d  end align-items-
-00001d50: 6365 6e74 6572 2067 6170 2d32 206d 622d  center gap-2 mb-
-00001d60: 3222 3e0a 2020 2020 2020 2020 2020 2020  2">.            
-00001d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d80: 3c73 6d61 6c6c 2063 6c61 7373 3d22 7465  <small class="te
-00001d90: 7874 2d6e 6f77 7261 7020 7465 7874 2d6d  xt-nowrap text-m
-00001da0: 7574 6564 223e 3c61 7070 2d69 7465 6d73  uted"><app-items
-00001db0: 2d63 6f75 6e74 2069 643d 2274 7349 7465  -count id="tsIte
-00001dc0: 6d73 436f 756e 7422 3e3c 2f61 7070 2d69  msCount"></app-i
-00001dd0: 7465 6d73 2d63 6f75 6e74 3e3c 2f73 6d61  tems-count></sma
-00001de0: 6c6c 3e0a 2020 2020 2020 2020 2020 2020  ll>.            
-00001df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e00: 3c75 6c20 6973 3d22 6170 702d 7061 6769  <ul is="app-pagi
-00001e10: 6e61 7469 6f6e 2220 6964 3d22 7473 5061  nation" id="tsPa
-00001e20: 6769 6e61 7469 6f6e 223e 3c2f 756c 3e0a  gination"></ul>.
-00001e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e40: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-00001e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e60: 2020 2020 2020 203c 6469 7620 6964 3d22         <div id="
-00001e70: 7473 4c69 7374 436f 6e74 6169 6e65 7222  tsListContainer"
-00001e80: 2063 6c61 7373 3d22 6c69 7374 2d67 726f   class="list-gro
-00001e90: 7570 223e 3c2f 6469 763e 0a20 2020 2020  up"></div>.     
-00001ea0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00001eb0: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-00001ec0: 2020 2020 2020 2020 2020 7b25 2066 6f72            {% for
-00001ed0: 2073 7472 7563 745f 656c 6d74 5f74 7970   struct_elmt_typ
-00001ee0: 6520 696e 2073 7472 7563 7475 7261 6c5f  e in structural_
-00001ef0: 656c 656d 656e 745f 7479 7065 7320 257d  element_types %}
-00001f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001f10: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00001f20: 2274 6162 2d70 616e 6520 702d 3322 2069  "tab-pane p-3" i
-00001f30: 643d 227b 7b20 7374 7275 6374 5f65 6c6d  d="{{ struct_elm
-00001f40: 745f 7479 7065 207d 7d73 2d74 6162 636f  t_type }}s-tabco
-00001f50: 6e74 656e 7422 2072 6f6c 653d 2274 6162  ntent" role="tab
-00001f60: 7061 6e65 6c22 2061 7269 612d 6c61 6265  panel" aria-labe
-00001f70: 6c6c 6564 6279 3d22 7b7b 2073 7472 7563  lledby="{{ struc
-00001f80: 745f 656c 6d74 5f74 7970 6520 7d7d 732d  t_elmt_type }}s-
-00001f90: 7461 6222 3e0a 2020 2020 2020 2020 2020  tab">.          
-00001fa0: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00001fb0: 6976 2063 6c61 7373 3d22 642d 666c 6578  iv class="d-flex
-00001fc0: 206a 7573 7469 6679 2d63 6f6e 7465 6e74   justify-content
-00001fd0: 2d65 6e64 2061 6c69 676e 2d69 7465 6d73  -end align-items
-00001fe0: 2d63 656e 7465 7220 6761 702d 3220 6d62  -center gap-2 mb
-00001ff0: 2d32 223e 0a20 2020 2020 2020 2020 2020  -2">.           
-00002000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002010: 203c 736d 616c 6c20 636c 6173 733d 2274   <small class="t
-00002020: 6578 742d 6e6f 7772 6170 2074 6578 742d  ext-nowrap text-
-00002030: 6d75 7465 6422 3e3c 6170 702d 6974 656d  muted"><app-item
-00002040: 732d 636f 756e 7420 6964 3d22 7b7b 2073  s-count id="{{ s
-00002050: 7472 7563 745f 656c 6d74 5f74 7970 6520  truct_elmt_type 
-00002060: 7d7d 7349 7465 6d73 436f 756e 7422 3e3c  }}sItemsCount"><
-00002070: 2f61 7070 2d69 7465 6d73 2d63 6f75 6e74  /app-items-count
-00002080: 3e3c 2f73 6d61 6c6c 3e0a 2020 2020 2020  ></small>.      
-00002090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020a0: 2020 2020 2020 3c75 6c20 6973 3d22 6170        <ul is="ap
-000020b0: 702d 7061 6769 6e61 7469 6f6e 2220 6964  p-pagination" id
-000020c0: 3d22 7b7b 2073 7472 7563 745f 656c 6d74  ="{{ struct_elmt
-000020d0: 5f74 7970 6520 7d7d 7350 6167 696e 6174  _type }}sPaginat
-000020e0: 696f 6e22 3e3c 2f75 6c3e 0a20 2020 2020  ion"></ul>.     
-000020f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002100: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
-00002110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002120: 2020 3c64 6976 2069 643d 227b 7b20 7374    <div id="{{ st
-00002130: 7275 6374 5f65 6c6d 745f 7479 7065 207d  ruct_elmt_type }
-00002140: 7d73 4c69 7374 436f 6e74 6169 6e65 7222  }sListContainer"
-00002150: 2063 6c61 7373 3d22 6c69 7374 2d67 726f   class="list-gro
-00002160: 7570 223e 3c2f 6469 763e 0a20 2020 2020  up"></div>.     
-00002170: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002180: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
-00002190: 2020 2020 2020 2020 2020 7b25 2065 6e64            {% end
-000021a0: 666f 7220 257d 0a20 2020 2020 2020 2020  for %}.         
-000021b0: 2020 2020 2020 203c 2f64 6976 3e0a 2020         </div>.  
-000021c0: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
-000021d0: 0a20 2020 2020 2020 2020 2020 203c 6469  .            <di
-000021e0: 7620 636c 6173 733d 226d 6f64 616c 2d66  v class="modal-f
-000021f0: 6f6f 7465 7220 642d 666c 6578 206a 7573  ooter d-flex jus
-00002200: 7469 6679 2d63 6f6e 7465 6e74 2d62 6574  tify-content-bet
-00002210: 7765 656e 2067 6170 2d32 223e 0a20 2020  ween gap-2">.   
-00002220: 2020 2020 2020 2020 2020 2020 203c 6e61               <na
-00002230: 7620 636c 6173 733d 2268 7374 6163 6b20  v class="hstack 
-00002240: 6761 702d 3222 2061 7269 612d 6c61 6265  gap-2" aria-labe
-00002250: 6c3d 224e 6f74 6966 6963 6174 696f 6e73  l="Notifications
-00002260: 206e 6176 6967 6174 696f 6e22 3e0a 2020   navigation">.  
-00002270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002280: 2020 3c75 6c20 636c 6173 733d 2270 6167    <ul class="pag
-00002290: 696e 6174 696f 6e20 6a75 7374 6966 792d  ination justify-
-000022a0: 636f 6e74 656e 742d 656e 6420 6d62 2d30  content-end mb-0
-000022b0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-000022c0: 2020 2020 2020 2020 2020 203c 6c69 2063             <li c
-000022d0: 6c61 7373 3d22 7061 6765 2d69 7465 6d20  lass="page-item 
-000022e0: 6469 7361 626c 6564 223e 3c61 2069 643d  disabled"><a id=
-000022f0: 226e 6f74 6966 496e 666f 4e61 7646 6972  "notifInfoNavFir
-00002300: 7374 2220 636c 6173 733d 2270 6167 652d  st" class="page-
-00002310: 6c69 6e6b 2220 7469 746c 653d 2246 6972  link" title="Fir
-00002320: 7374 206e 6f74 6966 6963 6174 696f 6e22  st notification"
-00002330: 2072 6f6c 653d 2262 7574 746f 6e22 3e3c   role="button"><
-00002340: 6920 636c 6173 733d 2262 6920 6269 2d63  i class="bi bi-c
-00002350: 6865 7672 6f6e 2d64 6f75 626c 652d 6c65  hevron-double-le
-00002360: 6674 223e 3c2f 693e 3c2f 613e 3c2f 6c69  ft"></i></a></li
-00002370: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
-00002380: 2020 2020 2020 2020 2020 3c6c 6920 636c            <li cl
-00002390: 6173 733d 2270 6167 652d 6974 656d 2064  ass="page-item d
-000023a0: 6973 6162 6c65 6422 3e3c 6120 6964 3d22  isabled"><a id="
-000023b0: 6e6f 7469 6649 6e66 6f4e 6176 5072 6576  notifInfoNavPrev
-000023c0: 696f 7573 2220 636c 6173 733d 2270 6167  ious" class="pag
-000023d0: 652d 6c69 6e6b 2220 7469 746c 653d 2250  e-link" title="P
-000023e0: 7265 7669 6f75 7320 6e6f 7469 6669 6361  revious notifica
-000023f0: 7469 6f6e 2220 726f 6c65 3d22 6275 7474  tion" role="butt
-00002400: 6f6e 223e 3c69 2063 6c61 7373 3d22 6269  on"><i class="bi
-00002410: 2062 692d 6368 6576 726f 6e2d 6c65 6674   bi-chevron-left
-00002420: 223e 3c2f 693e 3c2f 613e 3c2f 6c69 3e0a  "></i></a></li>.
-00002430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002440: 2020 2020 2020 2020 3c6c 6920 636c 6173          <li clas
-00002450: 733d 2270 6167 652d 6974 656d 2064 6973  s="page-item dis
-00002460: 6162 6c65 6422 3e3c 6120 6964 3d22 6e6f  abled"><a id="no
-00002470: 7469 6649 6e66 6f4e 6176 4e65 7874 2220  tifInfoNavNext" 
-00002480: 636c 6173 733d 2270 6167 652d 6c69 6e6b  class="page-link
-00002490: 2220 7469 746c 653d 224e 6578 7420 6e6f  " title="Next no
-000024a0: 7469 6669 6361 7469 6f6e 2220 726f 6c65  tification" role
-000024b0: 3d22 6275 7474 6f6e 223e 3c69 2063 6c61  ="button"><i cla
-000024c0: 7373 3d22 6269 2062 692d 6368 6576 726f  ss="bi bi-chevro
-000024d0: 6e2d 7269 6768 7422 3e3c 2f69 3e3c 2f61  n-right"></i></a
-000024e0: 3e3c 2f6c 693e 0a20 2020 2020 2020 2020  ></li>.         
-000024f0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00002500: 6c69 2063 6c61 7373 3d22 7061 6765 2d69  li class="page-i
-00002510: 7465 6d20 6469 7361 626c 6564 223e 3c61  tem disabled"><a
-00002520: 2069 643d 226e 6f74 6966 496e 666f 4e61   id="notifInfoNa
-00002530: 764c 6173 7422 2063 6c61 7373 3d22 7061  vLast" class="pa
-00002540: 6765 2d6c 696e 6b22 2074 6974 6c65 3d22  ge-link" title="
-00002550: 4c61 7374 206e 6f74 6966 6963 6174 696f  Last notificatio
-00002560: 6e22 2072 6f6c 653d 2262 7574 746f 6e22  n" role="button"
-00002570: 3e3c 6920 636c 6173 733d 2262 6920 6269  ><i class="bi bi
-00002580: 2d63 6865 7672 6f6e 2d64 6f75 626c 652d  -chevron-double-
-00002590: 7269 6768 7422 3e3c 2f69 3e3c 2f61 3e3c  right"></i></a><
-000025a0: 2f6c 693e 0a20 2020 2020 2020 2020 2020  /li>.           
-000025b0: 2020 2020 2020 2020 203c 2f75 6c3e 0a20           </ul>. 
-000025c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025d0: 2020 203c 736d 616c 6c20 636c 6173 733d     <small class=
-000025e0: 2274 6578 742d 6d75 7465 6422 3e3c 7370  "text-muted"><sp
-000025f0: 616e 2069 643d 226e 6f74 6966 496e 666f  an id="notifInfo
-00002600: 526f 7749 6e64 6578 223e 3f3c 2f73 7061  RowIndex">?</spa
-00002610: 6e3e 202f 203c 7370 616e 2069 643d 226e  n> / <span id="n
-00002620: 6f74 6966 496e 666f 526f 7743 6f75 6e74  otifInfoRowCount
-00002630: 223e 3f3c 2f73 7061 6e3e 3c2f 736d 616c  ">?</span></smal
-00002640: 6c3e 0a20 2020 2020 2020 2020 2020 2020  l>.             
-00002650: 2020 2020 2020 203c 736d 616c 6c20 636c         <small cl
-00002660: 6173 733d 2274 6578 742d 6d75 7465 6422  ass="text-muted"
-00002670: 3e28 7061 6765 203c 7370 616e 2069 643d  >(page <span id=
-00002680: 226e 6f74 6966 496e 666f 5061 6765 496e  "notifInfoPageIn
-00002690: 6465 7822 3e3f 3c2f 7370 616e 3e20 2f20  dex">?</span> / 
-000026a0: 3c73 7061 6e20 6964 3d22 6e6f 7469 6649  <span id="notifI
-000026b0: 6e66 6f50 6167 6543 6f75 6e74 223e 3f3c  nfoPageCount">?<
-000026c0: 2f73 7061 6e3e 293c 2f73 6d61 6c6c 3e0a  /span>)</small>.
-000026d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026e0: 3c2f 6e61 763e 0a20 2020 2020 2020 2020  </nav>.         
-000026f0: 2020 2020 2020 203c 6275 7474 6f6e 2074         <button t
-00002700: 7970 653d 2262 7574 746f 6e22 2063 6c61  ype="button" cla
-00002710: 7373 3d22 6274 6e20 6274 6e2d 736d 2062  ss="btn btn-sm b
-00002720: 746e 2d6f 7574 6c69 6e65 2d73 6563 6f6e  tn-outline-secon
-00002730: 6461 7279 2220 6461 7461 2d62 732d 6469  dary" data-bs-di
-00002740: 736d 6973 733d 226d 6f64 616c 223e 436c  smiss="modal">Cl
-00002750: 6f73 653c 2f62 7574 746f 6e3e 0a20 2020  ose</button>.   
-00002760: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-00002770: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-00002780: 2020 203c 2f64 6976 3e0a 3c2f 6469 763e     </div>.</div>
-00002790: 0a7b 2520 656e 6462 6c6f 636b 206d 6169  .{% endblock mai
-000027a0: 6e5f 636f 6e74 656e 7420 257d 0a0a 7b25  n_content %}..{%
-000027b0: 2062 6c6f 636b 2062 6f64 795f 7363 7269   block body_scri
-000027c0: 7074 7320 257d 0a7b 7b20 7375 7065 7228  pts %}.{{ super(
-000027d0: 2920 2d7d 7d0a 7b25 2066 696c 7465 7220  ) -}}.{% filter 
-000027e0: 696e 6465 6e74 2877 6964 7468 3d38 2c20  indent(width=8, 
-000027f0: 6669 7273 743d 5472 7565 2920 257d 0a3c  first=True) %}.<
-00002800: 7363 7269 7074 2074 7970 653d 226d 6f64  script type="mod
-00002810: 756c 6522 3e0a 2020 2020 696d 706f 7274  ule">.    import
-00002820: 207b 204e 6f74 6966 6963 6174 696f 6e45   { NotificationE
-00002830: 7870 6c6f 7265 5669 6577 207d 2066 726f  xploreView } fro
-00002840: 6d20 227b 7b20 7572 6c5f 666f 7228 2773  m "{{ url_for('s
-00002850: 7461 7469 6327 2c20 6669 6c65 6e61 6d65  tatic', filename
-00002860: 3d27 7363 7269 7074 732f 6d6f 6475 6c65  ='scripts/module
-00002870: 732f 7669 6577 732f 6e6f 7469 6669 6361  s/views/notifica
-00002880: 7469 6f6e 732f 6578 706c 6f72 652e 6a73  tions/explore.js
-00002890: 2729 207d 7d22 3b0a 0a0a 2020 2020 646f  ') }}";...    do
-000028a0: 6375 6d65 6e74 2e61 6464 4576 656e 744c  cument.addEventL
-000028b0: 6973 7465 6e65 7228 2244 4f4d 436f 6e74  istener("DOMCont
-000028c0: 656e 744c 6f61 6465 6422 2c20 2829 203d  entLoaded", () =
-000028d0: 3e20 7b0a 0a20 2020 2020 2020 206c 6574  > {..        let
-000028e0: 206f 7074 696f 6e73 203d 207b 0a20 2020   options = {.   
-000028f0: 2020 2020 2020 2020 2073 7472 7563 7475           structu
-00002900: 7261 6c45 6c65 6d65 6e74 5479 7065 733a  ralElementTypes:
-00002910: 207b 7b20 7374 7275 6374 7572 616c 5f65   {{ structural_e
-00002920: 6c65 6d65 6e74 5f74 7970 6573 207c 2074  lement_types | t
-00002930: 6f6a 736f 6e20 7d7d 2c0a 2020 2020 2020  ojson }},.      
-00002940: 2020 2020 2020 6669 6c74 6572 733a 207b        filters: {
-00002950: 7b20 6669 6c74 6572 7320 7c20 746f 6a73  { filters | tojs
-00002960: 6f6e 207d 7d2c 0a20 2020 2020 2020 2020  on }},.         
-00002970: 2020 2063 616d 7061 6967 6e73 3a20 7b7b     campaigns: {{
-00002980: 2067 2e63 616d 7061 6967 6e5f 6374 7874   g.campaign_ctxt
-00002990: 2e63 616d 7061 6967 6e73 207c 2074 6f6a  .campaigns | toj
-000029a0: 736f 6e20 7d7d 2c0a 2020 2020 2020 2020  son }},.        
-000029b0: 2020 2020 6375 7272 656e 7443 616d 7061      currentCampa
-000029c0: 6967 6e3a 207b 7b20 672e 6361 6d70 6169  ign: {{ g.campai
-000029d0: 676e 5f63 7478 742e 6361 6d70 6169 676e  gn_ctxt.campaign
-000029e0: 207c 2074 6f6a 736f 6e20 7d7d 2c0a 2020   | tojson }},.  
-000029f0: 2020 2020 2020 7d3b 0a0a 2020 2020 2020        };..      
-00002a00: 2020 6c65 7420 6e6f 7469 6645 7870 6c6f    let notifExplo
-00002a10: 7265 5669 6577 203d 206e 6577 204e 6f74  reView = new Not
-00002a20: 6966 6963 6174 696f 6e45 7870 6c6f 7265  ificationExplore
-00002a30: 5669 6577 286f 7074 696f 6e73 293b 0a20  View(options);. 
-00002a40: 2020 2020 2020 206e 6f74 6966 4578 706c         notifExpl
-00002a50: 6f72 6556 6965 772e 7265 6672 6573 6828  oreView.refresh(
-00002a60: 293b 0a0a 2020 2020 7d29 3b0a 3c2f 7363  );..    });.</sc
-00002a70: 7269 7074 3e0a 7b25 2065 6e64 6669 6c74  ript>.{% endfilt
-00002a80: 6572 2025 7d0a 7b25 2065 6e64 626c 6f63  er %}.{% endbloc
-00002a90: 6b20 626f 6479 5f73 6372 6970 7473 2025  k body_scripts %
-00002aa0: 7d                                       }
+00001600: 2020 2020 2020 2020 2020 2020 3c2f 7461              </ta
+00001610: 626c 653e 0a20 2020 2020 2020 2020 2020  ble>.           
+00001620: 2020 2020 2020 2020 2020 2020 203c 2f64               </d
+00001630: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+00001640: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00001650: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+00001660: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00001670: 2020 2020 2020 3c64 6976 2069 733d 2261        <div is="a
+00001680: 7070 2d73 7069 6e6e 6572 2220 6964 3d22  pp-spinner" id="
+00001690: 6576 656e 7449 6e66 6f54 6162 5370 696e  eventInfoTabSpin
+000016a0: 6e65 7222 2063 6c61 7373 3d22 642d 6e6f  ner" class="d-no
+000016b0: 6e65 223e 3c2f 6469 763e 0a20 2020 2020  ne"></div>.     
+000016c0: 2020 2020 2020 2020 2020 203c 756c 2069             <ul i
+000016d0: 643d 2265 7665 6e74 496e 666f 5461 6273  d="eventInfoTabs
+000016e0: 2220 636c 6173 733d 226e 6176 206e 6176  " class="nav nav
+000016f0: 2d74 6162 7320 6170 702d 7461 6273 206a  -tabs app-tabs j
+00001700: 7573 7469 6679 2d63 6f6e 7465 6e74 2d63  ustify-content-c
+00001710: 656e 7465 7220 642d 6e6f 6e65 2220 726f  enter d-none" ro
+00001720: 6c65 3d22 7461 626c 6973 7422 3e0a 2020  le="tablist">.  
+00001730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001740: 2020 3c6c 6920 636c 6173 733d 226e 6176    <li class="nav
+00001750: 2d69 7465 6d22 2072 6f6c 653d 2270 7265  -item" role="pre
+00001760: 7365 6e74 6174 696f 6e22 3e0a 2020 2020  sentation">.    
+00001770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001780: 2020 2020 3c62 7574 746f 6e20 636c 6173      <button clas
+00001790: 733d 226e 6176 2d6c 696e 6b20 6163 7469  s="nav-link acti
+000017a0: 7665 2220 6964 3d22 7473 2d74 6162 2220  ve" id="ts-tab" 
+000017b0: 6461 7461 2d62 732d 746f 6767 6c65 3d22  data-bs-toggle="
+000017c0: 7461 6222 2064 6174 612d 6273 2d74 6172  tab" data-bs-tar
+000017d0: 6765 743d 2223 7473 2d74 6162 636f 6e74  get="#ts-tabcont
+000017e0: 656e 7422 2074 7970 653d 2262 7574 746f  ent" type="butto
+000017f0: 6e22 2072 6f6c 653d 2274 6162 2220 6172  n" role="tab" ar
+00001800: 6961 2d63 6f6e 7472 6f6c 733d 2274 732d  ia-controls="ts-
+00001810: 7461 6263 6f6e 7465 6e74 2220 6172 6961  tabcontent" aria
+00001820: 2d73 656c 6563 7465 643d 2266 616c 7365  -selected="false
+00001830: 223e 5469 6d65 7365 7269 6573 203c 7370  ">Timeseries <sp
+00001840: 616e 2063 6c61 7373 3d22 6261 6467 6520  an class="badge 
+00001850: 6267 2d73 6563 6f6e 6461 7279 2220 6964  bg-secondary" id
+00001860: 3d22 7473 546f 7461 6c43 6f75 6e74 223e  ="tsTotalCount">
+00001870: 303c 2f73 7061 6e3e 3c2f 6275 7474 6f6e  0</span></button
+00001880: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00001890: 2020 2020 2020 3c2f 6c69 3e0a 2020 2020        </li>.    
+000018a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018b0: 7b25 2066 6f72 2073 7472 7563 745f 656c  {% for struct_el
+000018c0: 6d74 5f74 7970 6520 696e 2073 7472 7563  mt_type in struc
+000018d0: 7475 7261 6c5f 656c 656d 656e 745f 7479  tural_element_ty
+000018e0: 7065 7320 257d 0a20 2020 2020 2020 2020  pes %}.         
+000018f0: 2020 2020 2020 2020 2020 203c 6c69 2063             <li c
+00001900: 6c61 7373 3d22 6e61 762d 6974 656d 2220  lass="nav-item" 
+00001910: 726f 6c65 3d22 7072 6573 656e 7461 7469  role="presentati
+00001920: 6f6e 223e 0a20 2020 2020 2020 2020 2020  on">.           
+00001930: 2020 2020 2020 2020 2020 2020 203c 6275               <bu
+00001940: 7474 6f6e 2063 6c61 7373 3d22 6e61 762d  tton class="nav-
+00001950: 6c69 6e6b 2220 6964 3d22 7b7b 2073 7472  link" id="{{ str
+00001960: 7563 745f 656c 6d74 5f74 7970 6520 7d7d  uct_elmt_type }}
+00001970: 732d 7461 6222 2064 6174 612d 6273 2d74  s-tab" data-bs-t
+00001980: 6f67 676c 653d 2274 6162 2220 6461 7461  oggle="tab" data
+00001990: 2d62 732d 7461 7267 6574 3d22 237b 7b20  -bs-target="#{{ 
+000019a0: 7374 7275 6374 5f65 6c6d 745f 7479 7065  struct_elmt_type
+000019b0: 207d 7d73 2d74 6162 636f 6e74 656e 7422   }}s-tabcontent"
+000019c0: 2074 7970 653d 2262 7574 746f 6e22 2072   type="button" r
+000019d0: 6f6c 653d 2274 6162 2220 6172 6961 2d63  ole="tab" aria-c
+000019e0: 6f6e 7472 6f6c 733d 227b 7b20 7374 7275  ontrols="{{ stru
+000019f0: 6374 5f65 6c6d 745f 7479 7065 207d 7d73  ct_elmt_type }}s
+00001a00: 2d74 6162 636f 6e74 656e 7422 2061 7269  -tabcontent" ari
+00001a10: 612d 7365 6c65 6374 6564 3d22 6661 6c73  a-selected="fals
+00001a20: 6522 3e7b 7b20 7374 7275 6374 5f65 6c6d  e">{{ struct_elm
+00001a30: 745f 7479 7065 207c 2063 6170 6974 616c  t_type | capital
+00001a40: 697a 6520 7d7d 7320 3c73 7061 6e20 636c  ize }}s <span cl
+00001a50: 6173 733d 2262 6164 6765 2062 672d 7365  ass="badge bg-se
+00001a60: 636f 6e64 6172 7922 2069 643d 227b 7b20  condary" id="{{ 
+00001a70: 7374 7275 6374 5f65 6c6d 745f 7479 7065  struct_elmt_type
+00001a80: 207d 7d73 546f 7461 6c43 6f75 6e74 223e   }}sTotalCount">
+00001a90: 303c 2f73 7061 6e3e 3c2f 6275 7474 6f6e  0</span></button
+00001aa0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+00001ab0: 2020 2020 2020 3c2f 6c69 3e0a 2020 2020        </li>.    
+00001ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ad0: 7b25 2065 6e64 666f 7220 257d 0a20 2020  {% endfor %}.   
+00001ae0: 2020 2020 2020 2020 2020 2020 203c 2f75               </u
+00001af0: 6c3e 0a20 2020 2020 2020 2020 2020 2020  l>.             
+00001b00: 2020 203c 6469 7620 6964 3d22 6576 656e     <div id="even
+00001b10: 7449 6e66 6f54 6162 436f 6e74 656e 7473  tInfoTabContents
+00001b20: 2220 636c 6173 733d 2274 6162 2d63 6f6e  " class="tab-con
+00001b30: 7465 6e74 206f 7665 7266 6c6f 772d 6175  tent overflow-au
+00001b40: 746f 2062 6f72 6465 7220 626f 7264 6572  to border border
+00001b50: 2d74 6f70 2d30 2062 672d 7768 6974 6520  -top-0 bg-white 
+00001b60: 642d 6e6f 6e65 223e 0a20 2020 2020 2020  d-none">.       
+00001b70: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00001b80: 7620 636c 6173 733d 2274 6162 2d70 616e  v class="tab-pan
+00001b90: 6520 7368 6f77 2061 6374 6976 6520 702d  e show active p-
+00001ba0: 3322 2069 643d 2274 732d 7461 6263 6f6e  3" id="ts-tabcon
+00001bb0: 7465 6e74 2220 726f 6c65 3d22 7461 6270  tent" role="tabp
+00001bc0: 616e 656c 2220 6172 6961 2d6c 6162 656c  anel" aria-label
+00001bd0: 6c65 6462 793d 2274 732d 7461 6222 3e0a  ledby="ts-tab">.
+00001be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001bf0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+00001c00: 7373 3d22 642d 666c 6578 206a 7573 7469  ss="d-flex justi
+00001c10: 6679 2d63 6f6e 7465 6e74 2d65 6e64 2061  fy-content-end a
+00001c20: 6c69 676e 2d69 7465 6d73 2d63 656e 7465  lign-items-cente
+00001c30: 7220 6761 702d 3220 6d62 2d32 223e 0a20  r gap-2 mb-2">. 
+00001c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c50: 2020 2020 2020 2020 2020 203c 736d 616c             <smal
+00001c60: 6c20 636c 6173 733d 2274 6578 742d 6e6f  l class="text-no
+00001c70: 7772 6170 2074 6578 742d 6d75 7465 6422  wrap text-muted"
+00001c80: 3e3c 6170 702d 6974 656d 732d 636f 756e  ><app-items-coun
+00001c90: 7420 6964 3d22 7473 4974 656d 7343 6f75  t id="tsItemsCou
+00001ca0: 6e74 223e 3c2f 6170 702d 6974 656d 732d  nt"></app-items-
+00001cb0: 636f 756e 743e 3c2f 736d 616c 6c3e 0a20  count></small>. 
+00001cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cd0: 2020 2020 2020 2020 2020 203c 756c 2069             <ul i
+00001ce0: 733d 2261 7070 2d70 6167 696e 6174 696f  s="app-paginatio
+00001cf0: 6e22 2069 643d 2274 7350 6167 696e 6174  n" id="tsPaginat
+00001d00: 696f 6e22 3e3c 2f75 6c3e 0a20 2020 2020  ion"></ul>.     
+00001d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d20: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00001d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d40: 2020 3c64 6976 2069 643d 2274 734c 6973    <div id="tsLis
+00001d50: 7443 6f6e 7461 696e 6572 2220 636c 6173  tContainer" clas
+00001d60: 733d 226c 6973 742d 6772 6f75 7022 3e3c  s="list-group"><
+00001d70: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00001d80: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00001d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001da0: 2020 2020 207b 2520 666f 7220 7374 7275       {% for stru
+00001db0: 6374 5f65 6c6d 745f 7479 7065 2069 6e20  ct_elmt_type in 
+00001dc0: 7374 7275 6374 7572 616c 5f65 6c65 6d65  structural_eleme
+00001dd0: 6e74 5f74 7970 6573 2025 7d0a 2020 2020  nt_types %}.    
+00001de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001df0: 3c64 6976 2063 6c61 7373 3d22 7461 622d  <div class="tab-
+00001e00: 7061 6e65 2070 2d33 2220 6964 3d22 7b7b  pane p-3" id="{{
+00001e10: 2073 7472 7563 745f 656c 6d74 5f74 7970   struct_elmt_typ
+00001e20: 6520 7d7d 732d 7461 6263 6f6e 7465 6e74  e }}s-tabcontent
+00001e30: 2220 726f 6c65 3d22 7461 6270 616e 656c  " role="tabpanel
+00001e40: 2220 6172 6961 2d6c 6162 656c 6c65 6462  " aria-labelledb
+00001e50: 793d 227b 7b20 7374 7275 6374 5f65 6c6d  y="{{ struct_elm
+00001e60: 745f 7479 7065 207d 7d73 2d74 6162 223e  t_type }}s-tab">
+00001e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001e80: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00001e90: 6173 733d 2264 2d66 6c65 7820 6a75 7374  ass="d-flex just
+00001ea0: 6966 792d 636f 6e74 656e 742d 656e 6420  ify-content-end 
+00001eb0: 616c 6967 6e2d 6974 656d 732d 6365 6e74  align-items-cent
+00001ec0: 6572 2067 6170 2d32 206d 622d 3222 3e0a  er gap-2 mb-2">.
+00001ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ee0: 2020 2020 2020 2020 2020 2020 3c73 6d61              <sma
+00001ef0: 6c6c 2063 6c61 7373 3d22 7465 7874 2d6e  ll class="text-n
+00001f00: 6f77 7261 7020 7465 7874 2d6d 7574 6564  owrap text-muted
+00001f10: 223e 3c61 7070 2d69 7465 6d73 2d63 6f75  "><app-items-cou
+00001f20: 6e74 2069 643d 227b 7b20 7374 7275 6374  nt id="{{ struct
+00001f30: 5f65 6c6d 745f 7479 7065 207d 7d73 4974  _elmt_type }}sIt
+00001f40: 656d 7343 6f75 6e74 223e 3c2f 6170 702d  emsCount"></app-
+00001f50: 6974 656d 732d 636f 756e 743e 3c2f 736d  items-count></sm
+00001f60: 616c 6c3e 0a20 2020 2020 2020 2020 2020  all>.           
+00001f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f80: 203c 756c 2069 733d 2261 7070 2d70 6167   <ul is="app-pag
+00001f90: 696e 6174 696f 6e22 2069 643d 227b 7b20  ination" id="{{ 
+00001fa0: 7374 7275 6374 5f65 6c6d 745f 7479 7065  struct_elmt_type
+00001fb0: 207d 7d73 5061 6769 6e61 7469 6f6e 223e   }}sPagination">
+00001fc0: 3c2f 756c 3e0a 2020 2020 2020 2020 2020  </ul>.          
+00001fd0: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
+00001fe0: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
+00001ff0: 2020 2020 2020 2020 2020 2020 203c 6469               <di
+00002000: 7620 6964 3d22 7b7b 2073 7472 7563 745f  v id="{{ struct_
+00002010: 656c 6d74 5f74 7970 6520 7d7d 734c 6973  elmt_type }}sLis
+00002020: 7443 6f6e 7461 696e 6572 2220 636c 6173  tContainer" clas
+00002030: 733d 226c 6973 742d 6772 6f75 7022 3e3c  s="list-group"><
+00002040: 2f64 6976 3e0a 2020 2020 2020 2020 2020  /div>.          
+00002050: 2020 2020 2020 2020 2020 3c2f 6469 763e            </div>
+00002060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002070: 2020 2020 207b 2520 656e 6466 6f72 2025       {% endfor %
+00002080: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00002090: 2020 3c2f 6469 763e 0a20 2020 2020 2020    </div>.       
+000020a0: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
+000020b0: 2020 2020 2020 2020 3c64 6976 2063 6c61          <div cla
+000020c0: 7373 3d22 6d6f 6461 6c2d 666f 6f74 6572  ss="modal-footer
+000020d0: 2064 2d66 6c65 7820 6a75 7374 6966 792d   d-flex justify-
+000020e0: 636f 6e74 656e 742d 6265 7477 6565 6e20  content-between 
+000020f0: 6761 702d 3222 3e0a 2020 2020 2020 2020  gap-2">.        
+00002100: 2020 2020 2020 2020 3c6e 6176 2063 6c61          <nav cla
+00002110: 7373 3d22 6873 7461 636b 2067 6170 2d32  ss="hstack gap-2
+00002120: 2220 6172 6961 2d6c 6162 656c 3d22 4e6f  " aria-label="No
+00002130: 7469 6669 6361 7469 6f6e 7320 6e61 7669  tifications navi
+00002140: 6761 7469 6f6e 223e 0a20 2020 2020 2020  gation">.       
+00002150: 2020 2020 2020 2020 2020 2020 203c 756c               <ul
+00002160: 2063 6c61 7373 3d22 7061 6769 6e61 7469   class="paginati
+00002170: 6f6e 206a 7573 7469 6679 2d63 6f6e 7465  on justify-conte
+00002180: 6e74 2d65 6e64 206d 622d 3022 3e0a 2020  nt-end mb-0">.  
+00002190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021a0: 2020 2020 2020 3c6c 6920 636c 6173 733d        <li class=
+000021b0: 2270 6167 652d 6974 656d 2064 6973 6162  "page-item disab
+000021c0: 6c65 6422 3e3c 6120 6964 3d22 6e6f 7469  led"><a id="noti
+000021d0: 6649 6e66 6f4e 6176 4669 7273 7422 2063  fInfoNavFirst" c
+000021e0: 6c61 7373 3d22 7061 6765 2d6c 696e 6b22  lass="page-link"
+000021f0: 2074 6974 6c65 3d22 4669 7273 7420 6e6f   title="First no
+00002200: 7469 6669 6361 7469 6f6e 2220 726f 6c65  tification" role
+00002210: 3d22 6275 7474 6f6e 223e 3c69 2063 6c61  ="button"><i cla
+00002220: 7373 3d22 6269 2062 692d 6368 6576 726f  ss="bi bi-chevro
+00002230: 6e2d 646f 7562 6c65 2d6c 6566 7422 3e3c  n-double-left"><
+00002240: 2f69 3e3c 2f61 3e3c 2f6c 693e 0a20 2020  /i></a></li>.   
+00002250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002260: 2020 2020 203c 6c69 2063 6c61 7373 3d22       <li class="
+00002270: 7061 6765 2d69 7465 6d20 6469 7361 626c  page-item disabl
+00002280: 6564 223e 3c61 2069 643d 226e 6f74 6966  ed"><a id="notif
+00002290: 496e 666f 4e61 7650 7265 7669 6f75 7322  InfoNavPrevious"
+000022a0: 2063 6c61 7373 3d22 7061 6765 2d6c 696e   class="page-lin
+000022b0: 6b22 2074 6974 6c65 3d22 5072 6576 696f  k" title="Previo
+000022c0: 7573 206e 6f74 6966 6963 6174 696f 6e22  us notification"
+000022d0: 2072 6f6c 653d 2262 7574 746f 6e22 3e3c   role="button"><
+000022e0: 6920 636c 6173 733d 2262 6920 6269 2d63  i class="bi bi-c
+000022f0: 6865 7672 6f6e 2d6c 6566 7422 3e3c 2f69  hevron-left"></i
+00002300: 3e3c 2f61 3e3c 2f6c 693e 0a20 2020 2020  ></a></li>.     
+00002310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002320: 2020 203c 6c69 2063 6c61 7373 3d22 7061     <li class="pa
+00002330: 6765 2d69 7465 6d20 6469 7361 626c 6564  ge-item disabled
+00002340: 223e 3c61 2069 643d 226e 6f74 6966 496e  "><a id="notifIn
+00002350: 666f 4e61 764e 6578 7422 2063 6c61 7373  foNavNext" class
+00002360: 3d22 7061 6765 2d6c 696e 6b22 2074 6974  ="page-link" tit
+00002370: 6c65 3d22 4e65 7874 206e 6f74 6966 6963  le="Next notific
+00002380: 6174 696f 6e22 2072 6f6c 653d 2262 7574  ation" role="but
+00002390: 746f 6e22 3e3c 6920 636c 6173 733d 2262  ton"><i class="b
+000023a0: 6920 6269 2d63 6865 7672 6f6e 2d72 6967  i bi-chevron-rig
+000023b0: 6874 223e 3c2f 693e 3c2f 613e 3c2f 6c69  ht"></i></a></li
+000023c0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000023d0: 2020 2020 2020 2020 2020 3c6c 6920 636c            <li cl
+000023e0: 6173 733d 2270 6167 652d 6974 656d 2064  ass="page-item d
+000023f0: 6973 6162 6c65 6422 3e3c 6120 6964 3d22  isabled"><a id="
+00002400: 6e6f 7469 6649 6e66 6f4e 6176 4c61 7374  notifInfoNavLast
+00002410: 2220 636c 6173 733d 2270 6167 652d 6c69  " class="page-li
+00002420: 6e6b 2220 7469 746c 653d 224c 6173 7420  nk" title="Last 
+00002430: 6e6f 7469 6669 6361 7469 6f6e 2220 726f  notification" ro
+00002440: 6c65 3d22 6275 7474 6f6e 223e 3c69 2063  le="button"><i c
+00002450: 6c61 7373 3d22 6269 2062 692d 6368 6576  lass="bi bi-chev
+00002460: 726f 6e2d 646f 7562 6c65 2d72 6967 6874  ron-double-right
+00002470: 223e 3c2f 693e 3c2f 613e 3c2f 6c69 3e0a  "></i></a></li>.
+00002480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002490: 2020 2020 3c2f 756c 3e0a 2020 2020 2020      </ul>.      
+000024a0: 2020 2020 2020 2020 2020 2020 2020 3c73                <s
+000024b0: 6d61 6c6c 2063 6c61 7373 3d22 7465 7874  mall class="text
+000024c0: 2d6d 7574 6564 223e 3c73 7061 6e20 6964  -muted"><span id
+000024d0: 3d22 6e6f 7469 6649 6e66 6f52 6f77 496e  ="notifInfoRowIn
+000024e0: 6465 7822 3e3f 3c2f 7370 616e 3e20 2f20  dex">?</span> / 
+000024f0: 3c73 7061 6e20 6964 3d22 6e6f 7469 6649  <span id="notifI
+00002500: 6e66 6f52 6f77 436f 756e 7422 3e3f 3c2f  nfoRowCount">?</
+00002510: 7370 616e 3e3c 2f73 6d61 6c6c 3e0a 2020  span></small>.  
+00002520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002530: 2020 3c73 6d61 6c6c 2063 6c61 7373 3d22    <small class="
+00002540: 7465 7874 2d6d 7574 6564 223e 2870 6167  text-muted">(pag
+00002550: 6520 3c73 7061 6e20 6964 3d22 6e6f 7469  e <span id="noti
+00002560: 6649 6e66 6f50 6167 6549 6e64 6578 223e  fInfoPageIndex">
+00002570: 3f3c 2f73 7061 6e3e 202f 203c 7370 616e  ?</span> / <span
+00002580: 2069 643d 226e 6f74 6966 496e 666f 5061   id="notifInfoPa
+00002590: 6765 436f 756e 7422 3e3f 3c2f 7370 616e  geCount">?</span
+000025a0: 3e29 3c2f 736d 616c 6c3e 0a20 2020 2020  >)</small>.     
+000025b0: 2020 2020 2020 2020 2020 203c 2f6e 6176             </nav
+000025c0: 3e0a 2020 2020 2020 2020 2020 2020 2020  >.              
+000025d0: 2020 3c62 7574 746f 6e20 7479 7065 3d22    <button type="
+000025e0: 6275 7474 6f6e 2220 636c 6173 733d 2262  button" class="b
+000025f0: 746e 2062 746e 2d73 6d20 6274 6e2d 6f75  tn btn-sm btn-ou
+00002600: 746c 696e 652d 7365 636f 6e64 6172 7922  tline-secondary"
+00002610: 2064 6174 612d 6273 2d64 6973 6d69 7373   data-bs-dismiss
+00002620: 3d22 6d6f 6461 6c22 3e43 6c6f 7365 3c2f  ="modal">Close</
+00002630: 6275 7474 6f6e 3e0a 2020 2020 2020 2020  button>.        
+00002640: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
+00002650: 2020 203c 2f64 6976 3e0a 2020 2020 3c2f     </div>.    </
+00002660: 6469 763e 0a3c 2f64 6976 3e0a 7b25 2065  div>.</div>.{% e
+00002670: 6e64 626c 6f63 6b20 6d61 696e 5f63 6f6e  ndblock main_con
+00002680: 7465 6e74 2025 7d0a 0a7b 2520 626c 6f63  tent %}..{% bloc
+00002690: 6b20 626f 6479 5f73 6372 6970 7473 2025  k body_scripts %
+000026a0: 7d0a 7b7b 2073 7570 6572 2829 202d 7d7d  }.{{ super() -}}
+000026b0: 0a7b 2520 6669 6c74 6572 2069 6e64 656e  .{% filter inden
+000026c0: 7428 7769 6474 683d 382c 2066 6972 7374  t(width=8, first
+000026d0: 3d54 7275 6529 2025 7d0a 3c73 6372 6970  =True) %}.<scrip
+000026e0: 7420 7479 7065 3d22 6d6f 6475 6c65 223e  t type="module">
+000026f0: 0a20 2020 2069 6d70 6f72 7420 7b20 4e6f  .    import { No
+00002700: 7469 6669 6361 7469 6f6e 4578 706c 6f72  tificationExplor
+00002710: 6556 6965 7720 7d20 6672 6f6d 2022 7b7b  eView } from "{{
+00002720: 2075 726c 5f66 6f72 2827 7374 6174 6963   url_for('static
+00002730: 272c 2066 696c 656e 616d 653d 2773 6372  ', filename='scr
+00002740: 6970 7473 2f6d 6f64 756c 6573 2f76 6965  ipts/modules/vie
+00002750: 7773 2f6e 6f74 6966 6963 6174 696f 6e73  ws/notifications
+00002760: 2f65 7870 6c6f 7265 2e6a 7327 2920 7d7d  /explore.js') }}
+00002770: 223b 0a0a 0a20 2020 2064 6f63 756d 656e  ";...    documen
+00002780: 742e 6164 6445 7665 6e74 4c69 7374 656e  t.addEventListen
+00002790: 6572 2822 444f 4d43 6f6e 7465 6e74 4c6f  er("DOMContentLo
+000027a0: 6164 6564 222c 2028 2920 3d3e 207b 0a0a  aded", () => {..
+000027b0: 2020 2020 2020 2020 6c65 7420 6f70 7469          let opti
+000027c0: 6f6e 7320 3d20 7b0a 2020 2020 2020 2020  ons = {.        
+000027d0: 2020 2020 7374 7275 6374 7572 616c 456c      structuralEl
+000027e0: 656d 656e 7454 7970 6573 3a20 7b7b 2073  ementTypes: {{ s
+000027f0: 7472 7563 7475 7261 6c5f 656c 656d 656e  tructural_elemen
+00002800: 745f 7479 7065 7320 7c20 746f 6a73 6f6e  t_types | tojson
+00002810: 207d 7d2c 0a20 2020 2020 2020 2020 2020   }},.           
+00002820: 2066 696c 7465 7273 3a20 7b7b 2066 696c   filters: {{ fil
+00002830: 7465 7273 207c 2074 6f6a 736f 6e20 7d7d  ters | tojson }}
+00002840: 2c0a 2020 2020 2020 2020 2020 2020 6361  ,.            ca
+00002850: 6d70 6169 676e 733a 207b 7b20 672e 6361  mpaigns: {{ g.ca
+00002860: 6d70 6169 676e 5f63 7478 742e 6361 6d70  mpaign_ctxt.camp
+00002870: 6169 676e 7320 7c20 746f 6a73 6f6e 207d  aigns | tojson }
+00002880: 7d2c 0a20 2020 2020 2020 2020 2020 2063  },.            c
+00002890: 7572 7265 6e74 4361 6d70 6169 676e 3a20  urrentCampaign: 
+000028a0: 7b7b 2067 2e63 616d 7061 6967 6e5f 6374  {{ g.campaign_ct
+000028b0: 7874 2e63 616d 7061 6967 6e20 7c20 746f  xt.campaign | to
+000028c0: 6a73 6f6e 207d 7d2c 0a20 2020 2020 2020  json }},.       
+000028d0: 207d 3b0a 0a20 2020 2020 2020 206c 6574   };..        let
+000028e0: 206e 6f74 6966 4578 706c 6f72 6556 6965   notifExploreVie
+000028f0: 7720 3d20 6e65 7720 4e6f 7469 6669 6361  w = new Notifica
+00002900: 7469 6f6e 4578 706c 6f72 6556 6965 7728  tionExploreView(
+00002910: 6f70 7469 6f6e 7329 3b0a 2020 2020 2020  options);.      
+00002920: 2020 6e6f 7469 6645 7870 6c6f 7265 5669    notifExploreVi
+00002930: 6577 2e72 6566 7265 7368 2829 3b0a 0a20  ew.refresh();.. 
+00002940: 2020 207d 293b 0a3c 2f73 6372 6970 743e     });.</script>
+00002950: 0a7b 2520 656e 6466 696c 7465 7220 257d  .{% endfilter %}
+00002960: 0a7b 2520 656e 6462 6c6f 636b 2062 6f64  .{% endblock bod
+00002970: 795f 7363 7269 7074 7320 257d            y_scripts %}
```

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/notifications/setup.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/notifications/setup.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,11 @@
 {% extends "pages/base.html" %}
 
 {% set title = "Notifications" %}
-{% set subtitle = "Setup" %}
-
-{% block main_toolbar %}
-{{ super() -}}
-{% filter indent(width=20, first=True) %}
-<a href="{{ url_for('notifications.explore') }}" class="btn btn-sm btn-outline-secondary text-nowrap" title="Back to notifications"><i class="bi bi-arrow-return-left"></i> Back to notifications</a>
-{% endfilter %}
-{% endblock main_toolbar %}
+{% set subtitle = "Settings" %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row mb-3">
         <div class="col">
             <div class="alert alert-info mb-0" role="alert">
```

#### html2text {}

```diff
@@ -1,13 +1,9 @@
 {% extends "pages/base.html" %} {% set title = "Notifications" %} {% set
-subtitle = "Setup" %} {% block main_toolbar %} {{ super() -}} {% filter indent
-(width=20, first=True) %}
- Back_to_notifications
- {% endfilter %} {% endblock main_toolbar %} {% block main_content %} {{ super
-() -}}
+subtitle = "Settings" %} {% block main_content %} {{ super() -}}
  Default notification level for not customized event categories is {
 { default_notification_level }}.
   Setup an event category
  Help
 You can add an event category to select the notification level wanted.
 Event category Notification level
 ** Notification setup **
```

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/cleanup/list.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/cleanup/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/cleanup/manage.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/cleanup/manage.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/missing_data/list.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/missing_data/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/missing_data/manage.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/missing_data/manage.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/outlier_data/list.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/outlier_data/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/outlier_data/manage.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/outlier_data/manage.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/services/weather_data/manage.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/services/weather_data/manage.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/signin.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/signin.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/skeleton.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/skeleton.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/create.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/edit.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/explore.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/explore.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/properties/create.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/properties/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/properties/edit.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/properties/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/properties/list.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/properties/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/structural_elements/upload.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/structural_elements/upload.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/create.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/data/completeness.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/data/completeness.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/data/delete.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/data/delete.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/data/upload.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/data/upload.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/datastates/create.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/datastates/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/datastates/edit.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/datastates/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/datastates/list.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/datastates/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/edit.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/list.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/manage_structural_elements.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/manage_structural_elements.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/properties/create.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/properties/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/properties/edit.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/properties/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/properties/list.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/properties/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/semantic_setup.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/semantic_setup.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/timeseries/upload.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/timeseries/upload.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/create.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/edit.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/list.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/manage.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/manage.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/manage_campaign_scopes.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/manage_campaign_scopes.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/manage_campaigns.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/manage_campaigns.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/user_groups/view.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/user_groups/view.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/users/create.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/users/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/users/edit.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/users/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/users/list.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/users/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/templates/pages/users/view.html` & `bemserver-ui-0.5.3/bemserver_ui/templates/pages/users/view.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/views/__init__.py` & `bemserver-ui-0.5.3/bemserver_ui/views/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/views/analysis/degree_days.py` & `bemserver-ui-0.5.3/bemserver_ui/views/analysis/degree_days.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/views/auth.py` & `bemserver-ui-0.5.3/bemserver_ui/views/auth.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/views/campaign_scopes.py` & `bemserver-ui-0.5.3/bemserver_ui/views/campaign_scopes.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/views/campaigns.py` & `bemserver-ui-0.5.3/bemserver_ui/views/campaigns.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/views/events/categories.py` & `bemserver-ui-0.5.3/bemserver_ui/views/events/categories.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/views/events/events.py` & `bemserver-ui-0.5.3/bemserver_ui/views/events/events.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/views/main.py` & `bemserver-ui-0.5.3/bemserver_ui/views/main.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/views/notifications.py` & `bemserver-ui-0.5.3/bemserver_ui/views/notifications.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/views/services/cleanup.py` & `bemserver-ui-0.5.3/bemserver_ui/views/services/cleanup.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/views/services/missing_data.py` & `bemserver-ui-0.5.3/bemserver_ui/views/services/missing_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/views/services/outlier_data.py` & `bemserver-ui-0.5.3/bemserver_ui/views/services/outlier_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/views/structural_elements/properties.py` & `bemserver-ui-0.5.3/bemserver_ui/views/structural_elements/properties.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/views/structural_elements/structural_elements.py` & `bemserver-ui-0.5.3/bemserver_ui/views/structural_elements/structural_elements.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/views/timeseries/data.py` & `bemserver-ui-0.5.3/bemserver_ui/views/timeseries/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,18 @@
     )
 
 
 @blp.route("/explore")
 @auth.signin_required
 @ensure_campaign_context
 def explore():
-    return flask.render_template("pages/timeseries/data/explore.html")
+    return flask.render_template(
+        "pages/timeseries/data/explore.html",
+        dt_end=dt.datetime.now(tz=zoneinfo.ZoneInfo(flask.g.campaign_ctxt.tz_name)),
+    )
 
 
 @blp.route("/completeness")
 @auth.signin_required
 @ensure_campaign_context
 def completeness():
     return flask.render_template(
```

### Comparing `bemserver-ui-0.5.2/bemserver_ui/views/timeseries/datastates.py` & `bemserver-ui-0.5.3/bemserver_ui/views/timeseries/datastates.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/views/timeseries/properties.py` & `bemserver-ui-0.5.3/bemserver_ui/views/timeseries/properties.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/views/timeseries/timeseries.py` & `bemserver-ui-0.5.3/bemserver_ui/views/timeseries/timeseries.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/views/user_groups.py` & `bemserver-ui-0.5.3/bemserver_ui/views/user_groups.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui/views/users.py` & `bemserver-ui-0.5.3/bemserver_ui/views/users.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.5.2/bemserver_ui.egg-info/PKG-INFO` & `bemserver-ui-0.5.3/bemserver_ui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bemserver-ui
-Version: 0.5.2
+Version: 0.5.3
 Summary: BEMServer web interface
 Home-page: https://github.com/BEMServer/bemserver-ui
 Author: NOBATEK/INEF4
 Author-email: dfrederique@nobatek.inef4.com
 License: AGPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bemserver-ui-0.5.2/bemserver_ui.egg-info/SOURCES.txt` & `bemserver-ui-0.5.3/bemserver_ui.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 bemserver_ui/internal_api/structural_elements.py
 bemserver_ui/internal_api/user_groups.py
 bemserver_ui/internal_api/users.py
 bemserver_ui/internal_api/analysis/__init__.py
 bemserver_ui/internal_api/analysis/completeness.py
 bemserver_ui/internal_api/analysis/degree_days.py
 bemserver_ui/internal_api/analysis/energy_consumption.py
+bemserver_ui/internal_api/analysis/weather.py
 bemserver_ui/internal_api/semantics/__init__.py
 bemserver_ui/internal_api/semantics/weather.py
 bemserver_ui/internal_api/semantics/energy/__init__.py
 bemserver_ui/internal_api/semantics/energy/consumption.py
 bemserver_ui/internal_api/semantics/energy/production.py
 bemserver_ui/internal_api/services/__init__.py
 bemserver_ui/internal_api/services/cleanup.py
@@ -76,14 +77,15 @@
 bemserver_ui/static/scripts/modules/components/pagination.js
 bemserver_ui/static/scripts/modules/components/spinner.js
 bemserver_ui/static/scripts/modules/components/tree.js
 bemserver_ui/static/scripts/modules/components/charts/tsChartCompleteness.js
 bemserver_ui/static/scripts/modules/components/charts/tsChartDegreeDays.js
 bemserver_ui/static/scripts/modules/components/charts/tsChartEnergyConsumption.js
 bemserver_ui/static/scripts/modules/components/charts/tsChartExplore.js
+bemserver_ui/static/scripts/modules/components/charts/tsChartWeather.js
 bemserver_ui/static/scripts/modules/components/structuralElements/selector.js
 bemserver_ui/static/scripts/modules/components/time/datetimePicker.js
 bemserver_ui/static/scripts/modules/components/time/tzPicker.js
 bemserver_ui/static/scripts/modules/components/timeseries/bucketWidth.js
 bemserver_ui/static/scripts/modules/components/timeseries/selector.js
 bemserver_ui/static/scripts/modules/components/userGroup/userGroupItem.js
 bemserver_ui/static/scripts/modules/tools/array.js
@@ -91,14 +93,15 @@
 bemserver_ui/static/scripts/modules/tools/fetcher.js
 bemserver_ui/static/scripts/modules/tools/flaskES6.js
 bemserver_ui/static/scripts/modules/tools/parser.js
 bemserver_ui/static/scripts/modules/tools/time.js
 bemserver_ui/static/scripts/modules/tools/uuid.js
 bemserver_ui/static/scripts/modules/views/analysis/degreeDays.js
 bemserver_ui/static/scripts/modules/views/analysis/energyConsumption.js
+bemserver_ui/static/scripts/modules/views/analysis/weather.js
 bemserver_ui/static/scripts/modules/views/campaignScopes/manageGroups.js
 bemserver_ui/static/scripts/modules/views/campaigns/selector.js
 bemserver_ui/static/scripts/modules/views/events/edit.js
 bemserver_ui/static/scripts/modules/views/events/list.js
 bemserver_ui/static/scripts/modules/views/notifications/explore.js
 bemserver_ui/static/scripts/modules/views/notifications/setup.js
 bemserver_ui/static/scripts/modules/views/services/cleanupManage.js
@@ -144,14 +147,15 @@
 bemserver_ui/templates/pages/about.html
 bemserver_ui/templates/pages/base.html
 bemserver_ui/templates/pages/home.html
 bemserver_ui/templates/pages/signin.html
 bemserver_ui/templates/pages/skeleton.html
 bemserver_ui/templates/pages/analysis/degree_days.html
 bemserver_ui/templates/pages/analysis/energy_consumption.html
+bemserver_ui/templates/pages/analysis/weather.html
 bemserver_ui/templates/pages/campaign_scopes/create.html
 bemserver_ui/templates/pages/campaign_scopes/edit.html
 bemserver_ui/templates/pages/campaign_scopes/list.html
 bemserver_ui/templates/pages/campaign_scopes/view.html
 bemserver_ui/templates/pages/campaigns/create.html
 bemserver_ui/templates/pages/campaigns/edit.html
 bemserver_ui/templates/pages/campaigns/list.html
@@ -213,14 +217,15 @@
 bemserver_ui/views/main.py
 bemserver_ui/views/notifications.py
 bemserver_ui/views/user_groups.py
 bemserver_ui/views/users.py
 bemserver_ui/views/analysis/__init__.py
 bemserver_ui/views/analysis/degree_days.py
 bemserver_ui/views/analysis/energy_consumption.py
+bemserver_ui/views/analysis/weather.py
 bemserver_ui/views/events/__init__.py
 bemserver_ui/views/events/categories.py
 bemserver_ui/views/events/events.py
 bemserver_ui/views/services/__init__.py
 bemserver_ui/views/services/cleanup.py
 bemserver_ui/views/services/missing_data.py
 bemserver_ui/views/services/outlier_data.py
```

### Comparing `bemserver-ui-0.5.2/requirements/dev.txt` & `bemserver-ui-0.5.3/requirements/dev.txt`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     # via virtualenv
 identify==2.5.0
     # via pre-commit
 nodeenv==1.6.0
     # via pre-commit
 platformdirs==2.5.2
     # via virtualenv
-pre-commit==3.3.2
+pre-commit==3.3.3
     # via -r requirements/dev.in
 pyyaml==6.0
     # via pre-commit
 six==1.16.0
     # via virtualenv
 virtualenv==20.14.1
     # via pre-commit
```

### Comparing `bemserver-ui-0.5.2/requirements/install.txt` & `bemserver-ui-0.5.3/requirements/install.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --output-file=requirements/install.txt --resolver=backtracking setup.py
 #
-bemserver-api-client==0.19.1
+bemserver-api-client==0.20.0
     # via bemserver-ui (setup.py)
 certifi==2021.10.8
     # via requests
 charset-normalizer==2.0.12
     # via requests
 click==8.1.3
     # via flask
```

### Comparing `bemserver-ui-0.5.2/setup.py` & `bemserver-ui-0.5.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # Get the long description from the README file
 with open("README.rst", encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="bemserver-ui",
-    version="0.5.2",
+    version="0.5.3",
     description="BEMServer web interface",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/BEMServer/bemserver-ui",
     author="NOBATEK/INEF4",
     author_email="dfrederique@nobatek.inef4.com",
     license="AGPLv3+",
@@ -44,13 +44,13 @@
             "GNU Affero General Public License v3 or later (AGPLv3+)"
         ),
     ],
     python_requires=">=3.9",
     install_requires=[
         "flask>=2.2.3,<3.0.0",
         "python-dotenv>=1.0.0,<2.0.0",
-        "bemserver-api-client>=0.19.1,<0.20.0",
+        "bemserver-api-client>=0.20.0,<0.21.0",
     ],
     extras_require=EXTRAS_REQUIRE,
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
 )
```

