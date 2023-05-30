# Comparing `tmp/gs_quant-1.0.1.tar.gz` & `tmp/gs_quant-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gs_quant-1.0.1.tar", last modified: Tue May 23 13:56:19 2023, max compression
+gzip compressed data, was "dist/gs_quant-1.0.2.tar", last modified: Tue May 30 16:26:35 2023, max compression
```

## Comparing `gs_quant-1.0.1.tar` & `gs_quant-1.0.2.tar`

### file list

```diff
@@ -1,421 +1,421 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-23 13:56:03.000000 gs_quant-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-23 13:56:19.000000 gs_quant-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-23 13:56:03.000000 gs_quant-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/analytics/common/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/common/enumerators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/common/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/analytics/core/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18717 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/core/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/core/processor_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/core/query_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/analytics/datagrid/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/datagrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/datagrid/data_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/datagrid/data_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/datagrid/data_row.py
--rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/datagrid/datagrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/datagrid/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/datagrid/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/analytics/processors/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/processors/analysis_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/processors/econometrics_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/processors/scale_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/processors/special_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21852 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/processors/statistics_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/processors/utility_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/analytics/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/workspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25146 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/workspaces/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    24692 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/analytics/workspaces/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/api/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/api/fred/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/fred/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/fred/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/fred/fred_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/api/gs/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/backtests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/base_screener.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/carbon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/countries.py
--rw-r--r--   0 runner    (1001) docker     (123)    38344 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/data_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/datagrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/esg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/hedges.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/monitors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    14356 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/price.py
--rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/risk.py
--rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/risk_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/screens.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/thematics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/gs/workspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    12505 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/risk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/backtests/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/backtests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/backtests/action_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9891 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/backtests/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/backtests/backtest_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    16834 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/backtests/backtest_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/backtests/backtest_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/backtests/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/backtests/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/backtests/data_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/backtests/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14179 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/backtests/equity_vol_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/backtests/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/backtests/execution_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    39790 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/backtests/generic_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/backtests/order.py
--rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/backtests/predefined_asset_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/backtests/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/backtests/strategy_systematic.py
--rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/backtests/triggers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/config/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/config/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/config.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/content/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/content/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/content/reports_and_screens/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/content/reports_and_screens/00_fx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/content/reports_and_screens/00_fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/content/reports_and_screens/00_fx/vol_screen_app.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/content/reports_and_screens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/context_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/data/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/data/coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/data/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/data/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/data/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/data/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/data/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/datetime/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/datetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/datetime/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/datetime/gscalendar.py
--rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/datetime/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/datetime/relative_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/datetime/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/datetime/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.datetime.date.business_day_count.html
--rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.datetime.date.business_day_offset.html
--rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.datetime.date.date_range.html
--rw-r--r--   0 runner    (1001) docker     (123)    10403 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.datetime.date.is_business_day.html
--rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.datetime.date.prev_business_date.html
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.datetime.point.point_sort_order.html
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.abs_.html
--rw-r--r--   0 runner    (1001) docker     (123)    14066 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.add.html
--rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.and_.html
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.ceil.html
--rw-r--r--   0 runner    (1001) docker     (123)    14106 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.divide.html
--rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.exp.html
--rw-r--r--   0 runner    (1001) docker     (123)    13221 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.filter_.html
--rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.floor.html
--rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.floordiv.html
--rw-r--r--   0 runner    (1001) docker     (123)    11096 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.if_.html
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.log.html
--rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.multiply.html
--rw-r--r--   0 runner    (1001) docker     (123)    10247 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.not_.html
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.or_.html
--rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.power.html
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.repeat.html
--rw-r--r--   0 runner    (1001) docker     (123)    11620 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.smooth_spikes.html
--rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.sqrt.html
--rw-r--r--   0 runner    (1001) docker     (123)    14183 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.subtract.html
--rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.weighted_sum.html
--rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.analysis.count.html
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.analysis.diff.html
--rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.analysis.first.html
--rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.analysis.lag.html
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.analysis.last.html
--rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.analysis.last_value.html
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.analysis.weighted_sum.html
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.backtesting.basket.html
--rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.datetime.align.html
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.datetime.date_range.html
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.datetime.day.html
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.datetime.interpolate.html
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.datetime.month.html
--rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.datetime.prepend.html
--rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.datetime.quarter.html
--rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.datetime.union.html
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.datetime.value.html
--rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.datetime.weekday.html
--rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.datetime.year.html
--rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.econometrics.annualize.html
--rw-r--r--   0 runner    (1001) docker     (123)    13874 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.econometrics.beta.html
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.econometrics.change.html
--rw-r--r--   0 runner    (1001) docker     (123)    13613 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.econometrics.correlation.html
--rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.econometrics.excess_returns_.html
--rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.econometrics.index.html
--rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.econometrics.max_drawdown.html
--rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.econometrics.prices.html
--rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.econometrics.returns.html
--rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.econometrics.sharpe_ratio.html
--rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.econometrics.volatility.html
--rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.cov.html
--rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.exponential_std.html
--rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.generate_series.html
--rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.max_.html
--rw-r--r--   0 runner    (1001) docker     (123)    14083 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.mean.html
--rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.median.html
--rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.min_.html
--rw-r--r--   0 runner    (1001) docker     (123)    13107 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.mode.html
--rw-r--r--   0 runner    (1001) docker     (123)    12906 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.percentile.html
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.percentiles.html
--rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.product.html
--rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.range_.html
--rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.std.html
--rw-r--r--   0 runner    (1001) docker     (123)    13622 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.sum_.html
--rw-r--r--   0 runner    (1001) docker     (123)    13834 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.var.html
--rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.winsorize.html
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.zscores.html
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.technicals.bollinger_bands.html
--rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.technicals.exponential_moving_average.html
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.technicals.exponential_spread_volatility.html
--rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.technicals.exponential_volatility.html
--rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.technicals.moving_average.html
--rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.technicals.relative_strength_index.html
--rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.technicals.smoothed_moving_average.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/entities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21932 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/entities/entitlements.py
--rw-r--r--   0 runner    (1001) docker     (123)    42358 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/entities/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/entities/tree_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/instrument/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/instrument/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13457 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/instrument/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/instrument/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/json_convertors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/json_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/markets/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/markets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39088 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/markets/baskets.py
--rw-r--r--   0 runner    (1001) docker     (123)    26457 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/markets/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/markets/factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    41479 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/markets/hedge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/markets/historical.py
--rw-r--r--   0 runner    (1001) docker     (123)    21287 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/markets/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    19950 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/markets/indices_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/markets/markets.py
--rw-r--r--   0 runner    (1001) docker     (123)    30382 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/markets/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    25417 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/markets/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)    24832 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/markets/portfolio_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/markets/portfolio_manager_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29040 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/markets/position_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    62817 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/markets/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/markets/report_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16415 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/markets/screens.py
--rw-r--r--   0 runner    (1001) docker     (123)    69212 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/markets/securities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/models/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29649 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/models/epidemiology.py
--rw-r--r--   0 runner    (1001) docker     (123)    96299 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/models/risk_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/models/risk_model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/priceable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/quote_reports/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/quote_reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/quote_reports/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/risk/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/risk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19410 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/risk/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/risk/measures.py
--rw-r--r--   0 runner    (1001) docker     (123)    14873 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/risk/result_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    39786 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/risk/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/risk/scenario_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/risk/scenarios.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/risk/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    28088 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/target/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30269 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/assets_screener.py
--rw-r--r--   0 runner    (1001) docker     (123)    30119 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/backtests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/base_screener.py
--rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/charts.py
--rw-r--r--   0 runner    (1001) docker     (123)   241626 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    15206 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/countries.py
--rw-r--r--   0 runner    (1001) docker     (123)    36383 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/data_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    23131 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/hedge.py
--rw-r--r--   0 runner    (1001) docker     (123)    28594 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/indices.py
--rw-r--r--   0 runner    (1001) docker     (123)   158854 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)    26039 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/measures.py
--rw-r--r--   0 runner    (1001) docker     (123)    15365 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10446 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/price.py
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    37770 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/risk.py
--rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/risk_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/screens.py
--rw-r--r--   0 runner    (1001) docker     (123)    17024 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/secmaster.py
--rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/trades.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/workflow_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)    19404 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/target/workspaces_markets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/test/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/analytics/test_datagrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/analytics/test_sorting_and_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/analytics/test_workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/test/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/api/test_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/api/test_backtests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/api/test_base_screener.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/api/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/api/test_carbon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/api/test_content.py
--rw-r--r--   0 runner    (1001) docker     (123)    19594 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/api/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/api/test_data_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/api/test_esg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/api/test_fred.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/api/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/api/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/api/test_instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/api/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/api/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/api/test_portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/api/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/api/test_risk.py
--rw-r--r--   0 runner    (1001) docker     (123)    30272 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/api/test_risk_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/api/test_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/api/test_thread_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/api/test_users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/test/backtest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/backtest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34874 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/backtest/test_backtest_eq_vol_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/backtest/test_backtest_flow_vol.py
--rw-r--r--   0 runner    (1001) docker     (123)     8314 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/backtest/test_backtest_predefined.py
--rw-r--r--   0 runner    (1001) docker     (123)    20499 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/backtest/test_generic_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/backtest/test_triggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/data/test_data_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/data/test_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/test/datetime_/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/datetime_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/datetime_/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/datetime_/test_gscalendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/datetime_/test_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/datetime_/test_relative_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/datetime_/test_time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/test/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/fixtures/content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/test/markets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/markets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12018 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/markets/test_baskets.py
--rw-r--r--   0 runner    (1001) docker     (123)   180924 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/markets/test_hedger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/markets/test_instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)    17017 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/markets/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)    59098 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/markets/test_portfolio_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/markets/test_pricing_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    20426 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/markets/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    62477 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/markets/test_securities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/test/models/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/models/test_epidemiology.py
--rw-r--r--   0 runner    (1001) docker     (123)    30540 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/models/test_risk_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/test/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/test/timeseries/multi_measure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/timeseries/multi_measure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/timeseries/multi_measure/test_commod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/timeseries/multi_measure/test_measure_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    19175 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/timeseries/test_algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/timeseries/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    19817 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/timeseries/test_backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/timeseries/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)    17631 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/timeseries/test_econometrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/timeseries/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)   238697 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/timeseries/test_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/timeseries/test_measures_countries.py
--rw-r--r--   0 runner    (1001) docker     (123)    22551 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/timeseries/test_measures_fx_vol.py
--rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/timeseries/test_measures_inflation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/timeseries/test_measures_portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)    58767 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/timeseries/test_measures_rates.py
--rw-r--r--   0 runner    (1001) docker     (123)    36565 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/timeseries/test_measures_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    10574 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/timeseries/test_measures_risk_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14552 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/timeseries/test_measures_xccy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/timeseries/test_rolling.py
--rw-r--r--   0 runner    (1001) docker     (123)    29280 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/timeseries/test_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/timeseries/test_tca.py
--rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/timeseries/test_technicals.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/timeseries/test_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/timeseries/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/utils/datagrid_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/utils/mock_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/utils/mock_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/utils/mock_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/test/utils/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23911 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/timeseries/algebra.py
--rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/timeseries/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/timeseries/backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)    21728 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/timeseries/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)    27160 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/timeseries/econometrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/timeseries/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/timeseries/measure_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)   227438 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/timeseries/measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/timeseries/measures_countries.py
--rw-r--r--   0 runner    (1001) docker     (123)    31461 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/timeseries/measures_fx_vol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/timeseries/measures_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    16985 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/timeseries/measures_inflation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/timeseries/measures_portfolios.py
--rw-r--r--   0 runner    (1001) docker     (123)   100015 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/timeseries/measures_rates.py
--rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/timeseries/measures_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/timeseries/measures_risk_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    20096 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/timeseries/measures_xccy.py
--rw-r--r--   0 runner    (1001) docker     (123)    54899 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/timeseries/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/timeseries/tca.py
--rw-r--r--   0 runner    (1001) docker     (123)    20055 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/timeseries/technicals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant/tracing/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/tracing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-23 13:56:03.000000 gs_quant-1.0.1/gs_quant/tracing/tracing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 13:56:19.000000 gs_quant-1.0.1/gs_quant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-23 13:56:19.000000 gs_quant-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-05-23 13:56:03.000000 gs_quant-1.0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83669 2023-05-23 13:56:03.000000 gs_quant-1.0.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-30 16:26:18.000000 gs_quant-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-30 16:26:35.000000 gs_quant-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-30 16:26:18.000000 gs_quant-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/analytics/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/common/enumerators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/common/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/analytics/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18717 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/core/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/core/processor_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/core/query_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/analytics/datagrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/datagrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/datagrid/data_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/datagrid/data_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/datagrid/data_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31289 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/datagrid/datagrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/datagrid/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/datagrid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/analytics/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/processors/analysis_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/processors/econometrics_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/processors/scale_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/processors/special_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21852 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/processors/statistics_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16176 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/processors/utility_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/analytics/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/workspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25146 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/workspaces/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24692 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/analytics/workspaces/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/api/fred/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/fred/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/fred/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/fred/fred_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/api/gs/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/backtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/base_screener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/carbon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38345 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/data_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/datagrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/esg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/hedges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/monitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14693 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/risk_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/screens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/thematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/gs/workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12505 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/backtests/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/backtests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/backtests/action_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9891 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/backtests/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/backtests/backtest_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16840 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/backtests/backtest_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/backtests/backtest_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/backtests/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/backtests/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/backtests/data_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/backtests/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14179 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/backtests/equity_vol_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/backtests/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/backtests/execution_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39790 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/backtests/generic_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/backtests/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/backtests/predefined_asset_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/backtests/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/backtests/strategy_systematic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/backtests/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/config/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/config.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/content/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/content/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/content/reports_and_screens/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/content/reports_and_screens/00_fx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/content/reports_and_screens/00_fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/content/reports_and_screens/00_fx/vol_screen_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/content/reports_and_screens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/context_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/data/coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/data/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/data/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/data/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/data/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/data/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/datetime/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/datetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/datetime/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/datetime/gscalendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/datetime/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/datetime/relative_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/datetime/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/datetime/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.datetime.date.business_day_count.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.datetime.date.business_day_offset.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.datetime.date.date_range.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10403 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.datetime.date.is_business_day.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.datetime.date.prev_business_date.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.datetime.point.point_sort_order.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.abs_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14066 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.add.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.and_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.ceil.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14106 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.divide.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.exp.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13221 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.filter_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.floor.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.floordiv.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11096 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.if_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.log.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.multiply.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10247 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.not_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.or_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.power.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.repeat.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11620 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.smooth_spikes.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.sqrt.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14183 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.subtract.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.weighted_sum.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9329 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.analysis.count.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.analysis.diff.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.analysis.first.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.analysis.lag.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.analysis.last.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9446 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.analysis.last_value.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.analysis.weighted_sum.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.backtesting.basket.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13116 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.datetime.align.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.datetime.date_range.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.datetime.day.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.datetime.interpolate.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.datetime.month.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.datetime.prepend.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.datetime.quarter.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.datetime.union.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.datetime.value.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.datetime.weekday.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.datetime.year.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.econometrics.annualize.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13874 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.econometrics.beta.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.econometrics.change.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13613 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.econometrics.correlation.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.econometrics.excess_returns_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.econometrics.index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.econometrics.max_drawdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.econometrics.prices.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.econometrics.returns.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.econometrics.sharpe_ratio.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.econometrics.volatility.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.cov.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.exponential_std.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.generate_series.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.max_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14083 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.mean.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.median.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.min_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13107 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.mode.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12906 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.percentile.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.percentiles.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.product.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.range_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13766 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.std.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13622 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.sum_.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13834 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.var.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.winsorize.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.zscores.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.technicals.bollinger_bands.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.technicals.exponential_moving_average.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.technicals.exponential_spread_volatility.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.technicals.exponential_volatility.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.technicals.moving_average.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.technicals.relative_strength_index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.technicals.smoothed_moving_average.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21932 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/entities/entitlements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42358 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/entities/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/entities/tree_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/instrument/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/instrument/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13457 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/instrument/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/instrument/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/json_convertors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/json_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/markets/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/markets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39088 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/markets/baskets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26457 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/markets/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/markets/factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41479 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/markets/hedge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/markets/historical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21287 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/markets/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/markets/indices_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/markets/markets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30382 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/markets/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25417 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/markets/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24832 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/markets/portfolio_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/markets/portfolio_manager_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29040 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/markets/position_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62817 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/markets/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/markets/report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16415 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/markets/screens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69212 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/markets/securities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29649 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/models/epidemiology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96299 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/models/risk_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/models/risk_model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/priceable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/quote_reports/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/quote_reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/quote_reports/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/risk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/risk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19996 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/risk/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/risk/measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16251 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/risk/result_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39862 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/risk/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/risk/scenario_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/risk/scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/risk/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28088 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/target/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30269 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/assets_screener.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30119 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/backtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/base_screener.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)   241626 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15206 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36383 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/data_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23131 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/hedge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28594 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)   158854 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26039 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15365 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10446 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37770 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/risk_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/screens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17024 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/secmaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/trades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/workflow_quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19404 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/target/workspaces_markets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/test/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/analytics/test_datagrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/analytics/test_sorting_and_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/analytics/test_workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/test/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/api/test_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/api/test_backtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/api/test_base_screener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/api/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/api/test_carbon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/api/test_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19594 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/api/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/api/test_data_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/api/test_esg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/api/test_fred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/api/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/api/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/api/test_instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/api/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/api/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/api/test_portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/api/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/api/test_risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30272 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/api/test_risk_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/api/test_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/api/test_thread_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/api/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/test/backtest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/backtest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34874 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/backtest/test_backtest_eq_vol_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/backtest/test_backtest_flow_vol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8314 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/backtest/test_backtest_predefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20499 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/backtest/test_generic_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/backtest/test_triggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/data/test_data_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/data/test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/test/datetime_/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/datetime_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/datetime_/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/datetime_/test_gscalendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/datetime_/test_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/datetime_/test_relative_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/datetime_/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/test/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/fixtures/content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/test/markets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/markets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12018 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/markets/test_baskets.py
+-rw-r--r--   0 runner    (1001) docker     (123)   180924 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/markets/test_hedger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/markets/test_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17017 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/markets/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59098 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/markets/test_portfolio_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/markets/test_pricing_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20426 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/markets/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62477 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/markets/test_securities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/test/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/models/test_epidemiology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30540 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/models/test_risk_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/test/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/test/timeseries/multi_measure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/timeseries/multi_measure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/timeseries/multi_measure/test_commod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/timeseries/multi_measure/test_measure_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19175 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/timeseries/test_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/timeseries/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19817 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/timeseries/test_backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/timeseries/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17631 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/timeseries/test_econometrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/timeseries/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238697 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/timeseries/test_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/timeseries/test_measures_countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22551 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/timeseries/test_measures_fx_vol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/timeseries/test_measures_inflation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/timeseries/test_measures_portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58767 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/timeseries/test_measures_rates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36565 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/timeseries/test_measures_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10574 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/timeseries/test_measures_risk_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14552 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/timeseries/test_measures_xccy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/timeseries/test_rolling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29280 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/timeseries/test_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/timeseries/test_tca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10202 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/timeseries/test_technicals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/timeseries/test_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/timeseries/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/utils/datagrid_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/utils/mock_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/utils/mock_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/utils/mock_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/test/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23911 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/timeseries/algebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/timeseries/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/timeseries/backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21728 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/timeseries/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27160 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/timeseries/econometrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/timeseries/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/timeseries/measure_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)   227438 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/timeseries/measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/timeseries/measures_countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31461 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/timeseries/measures_fx_vol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/timeseries/measures_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16985 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/timeseries/measures_inflation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/timeseries/measures_portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100015 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/timeseries/measures_rates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/timeseries/measures_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/timeseries/measures_risk_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20096 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/timeseries/measures_xccy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54899 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/timeseries/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/timeseries/tca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20055 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/timeseries/technicals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant/tracing/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/tracing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-05-30 16:26:18.000000 gs_quant-1.0.2/gs_quant/tracing/tracing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 16:26:35.000000 gs_quant-1.0.2/gs_quant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-30 16:26:35.000000 gs_quant-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-05-30 16:26:18.000000 gs_quant-1.0.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83669 2023-05-30 16:26:18.000000 gs_quant-1.0.2/versioneer.py
```

### Comparing `gs_quant-1.0.1/PKG-INFO` & `gs_quant-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs_quant
-Version: 1.0.1
+Version: 1.0.2
 Summary: Goldman Sachs Quant
 Home-page: https://marquee.gs.com
 Author: Goldman Sachs
 Author-email: developer@gs.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Description: # GS Quant
```

### Comparing `gs_quant-1.0.1/README.md` & `gs_quant-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/__init__.py` & `gs_quant-1.0.2/gs_quant/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/analytics/common/__init__.py` & `gs_quant-1.0.2/gs_quant/analytics/common/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/analytics/common/constants.py` & `gs_quant-1.0.2/gs_quant/analytics/common/constants.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/analytics/common/enumerators.py` & `gs_quant-1.0.2/gs_quant/analytics/common/enumerators.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/analytics/common/helpers.py` & `gs_quant-1.0.2/gs_quant/analytics/common/helpers.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/analytics/core/__init__.py` & `gs_quant-1.0.2/gs_quant/analytics/core/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/analytics/core/processor.py` & `gs_quant-1.0.2/gs_quant/analytics/core/processor.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/analytics/core/processor_result.py` & `gs_quant-1.0.2/gs_quant/analytics/core/processor_result.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/analytics/core/query_helpers.py` & `gs_quant-1.0.2/gs_quant/analytics/core/query_helpers.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/analytics/datagrid/__init__.py` & `gs_quant-1.0.2/gs_quant/analytics/datagrid/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/analytics/datagrid/data_cell.py` & `gs_quant-1.0.2/gs_quant/analytics/datagrid/data_cell.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/analytics/datagrid/data_column.py` & `gs_quant-1.0.2/gs_quant/analytics/datagrid/data_column.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/analytics/datagrid/data_row.py` & `gs_quant-1.0.2/gs_quant/analytics/datagrid/data_row.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/analytics/datagrid/datagrid.py` & `gs_quant-1.0.2/gs_quant/analytics/datagrid/datagrid.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/analytics/datagrid/serializers.py` & `gs_quant-1.0.2/gs_quant/analytics/datagrid/serializers.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/analytics/datagrid/utils.py` & `gs_quant-1.0.2/gs_quant/analytics/datagrid/utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/analytics/processors/__init__.py` & `gs_quant-1.0.2/gs_quant/analytics/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/analytics/processors/analysis_processors.py` & `gs_quant-1.0.2/gs_quant/analytics/processors/analysis_processors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/analytics/processors/econometrics_processors.py` & `gs_quant-1.0.2/gs_quant/analytics/processors/econometrics_processors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/analytics/processors/scale_processors.py` & `gs_quant-1.0.2/gs_quant/analytics/processors/scale_processors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/analytics/processors/special_processors.py` & `gs_quant-1.0.2/gs_quant/analytics/processors/special_processors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/analytics/processors/statistics_processors.py` & `gs_quant-1.0.2/gs_quant/analytics/processors/statistics_processors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/analytics/processors/utility_processors.py` & `gs_quant-1.0.2/gs_quant/analytics/processors/utility_processors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/analytics/workspaces/__init__.py` & `gs_quant-1.0.2/gs_quant/analytics/workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/analytics/workspaces/components.py` & `gs_quant-1.0.2/gs_quant/analytics/workspaces/components.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/analytics/workspaces/workspace.py` & `gs_quant-1.0.2/gs_quant/analytics/workspaces/workspace.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/__init__.py` & `gs_quant-1.0.2/gs_quant/api/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/data.py` & `gs_quant-1.0.2/gs_quant/api/data.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/fred/__init__.py` & `gs_quant-1.0.2/gs_quant/api/fred/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/fred/data.py` & `gs_quant-1.0.2/gs_quant/api/fred/data.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/fred/fred_query.py` & `gs_quant-1.0.2/gs_quant/api/fred/fred_query.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/__init__.py` & `gs_quant-1.0.2/gs_quant/api/gs/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/assets.py` & `gs_quant-1.0.2/gs_quant/api/gs/assets.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/backtests.py` & `gs_quant-1.0.2/gs_quant/api/gs/backtests.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/base_screener.py` & `gs_quant-1.0.2/gs_quant/api/gs/base_screener.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/carbon.py` & `gs_quant-1.0.2/gs_quant/api/gs/carbon.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/content.py` & `gs_quant-1.0.2/gs_quant/api/gs/content.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/countries.py` & `gs_quant-1.0.2/gs_quant/api/gs/countries.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/data.py` & `gs_quant-1.0.2/gs_quant/api/gs/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -812,15 +812,15 @@
             incoming_data_data_types = pd.DataFrame(sample).dtypes.to_dict()
 
             df = pd.DataFrame(data, columns={**dataset_types, **incoming_data_data_types})
 
             for field_name, type_name in dataset_types.items():
                 if df.get(field_name) is not None and type_name in ('date', 'date-time') and \
                         len(df.get(field_name).value_counts()) > 0:
-                    df = df.astype({field_name: 'datetime64[ns]'})
+                    df[field_name] = pd.to_datetime(df[field_name])
 
             field_names = dataset_types.keys()
 
             if 'date' in field_names:
                 df = df.set_index('date')
             elif 'time' in field_names:
                 df = df.set_index('time')
```

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/data_screen.py` & `gs_quant-1.0.2/gs_quant/api/gs/data_screen.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/datagrid.py` & `gs_quant-1.0.2/gs_quant/api/gs/datagrid.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/esg.py` & `gs_quant-1.0.2/gs_quant/api/gs/esg.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/groups.py` & `gs_quant-1.0.2/gs_quant/api/gs/groups.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/hedges.py` & `gs_quant-1.0.2/gs_quant/api/gs/hedges.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/indices.py` & `gs_quant-1.0.2/gs_quant/api/gs/indices.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/monitors.py` & `gs_quant-1.0.2/gs_quant/api/gs/monitors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/parser.py` & `gs_quant-1.0.2/gs_quant/api/gs/parser.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/plots.py` & `gs_quant-1.0.2/gs_quant/api/gs/plots.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/portfolios.py` & `gs_quant-1.0.2/gs_quant/api/gs/portfolios.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,26 +26,36 @@
 from gs_quant.target.risk_models import RiskModelTerm as Term
 from gs_quant.target.workflow_quote import WorkflowPosition, WorkflowPositionsResponse, SaveQuoteRequest
 
 _logger = logging.getLogger(__name__)
 
 
 class GsPortfolioApi:
-    """GS Asset API client implementation"""
+    """GS Asset API client implementation.
+
+    To pass additional query parameters, use kwargs."""
 
     @classmethod
     def get_portfolios(cls,
                        portfolio_ids: List[str] = None,
                        portfolio_names: List[str] = None,
-                       limit: int = 100) -> Tuple[Portfolio, ...]:
+                       limit: int = 100,
+                       **kwargs) -> Tuple[Portfolio, ...]:
         url = '/portfolios?'
         if portfolio_ids:
             url += f'&id={"&id=".join(portfolio_ids)}'
         if portfolio_names:
             url += f'&name={"&name=".join(portfolio_names)}'
+        for k, v in kwargs.items():
+            if isinstance(v, list):
+                for i in v:
+                    # in case v is not a list of strings
+                    url += f'&{k}={i}'
+            else:
+                url += f'&{k}={v}'
         return GsSession.current._get(f'{url}&limit={limit}', cls=Portfolio)['results']
 
     @classmethod
     def get_portfolio(cls, portfolio_id: str) -> Portfolio:
         return GsSession.current._get('/portfolios/{id}'.format(id=portfolio_id), cls=Portfolio)
 
     @classmethod
```

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/price.py` & `gs_quant-1.0.2/gs_quant/api/gs/price.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/reports.py` & `gs_quant-1.0.2/gs_quant/api/gs/reports.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/risk.py` & `gs_quant-1.0.2/gs_quant/api/gs/risk.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/risk_models.py` & `gs_quant-1.0.2/gs_quant/api/gs/risk_models.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/screens.py` & `gs_quant-1.0.2/gs_quant/api/gs/screens.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/thematics.py` & `gs_quant-1.0.2/gs_quant/api/gs/thematics.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/users.py` & `gs_quant-1.0.2/gs_quant/api/gs/users.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/gs/workspaces.py` & `gs_quant-1.0.2/gs_quant/api/gs/workspaces.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/risk.py` & `gs_quant-1.0.2/gs_quant/api/risk.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/api/utils.py` & `gs_quant-1.0.2/gs_quant/api/utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/backtests/__init__.py` & `gs_quant-1.0.2/gs_quant/backtests/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/backtests/action_handler.py` & `gs_quant-1.0.2/gs_quant/backtests/action_handler.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/backtests/actions.py` & `gs_quant-1.0.2/gs_quant/backtests/actions.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/backtests/backtest_engine.py` & `gs_quant-1.0.2/gs_quant/backtests/backtest_engine.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/backtests/backtest_objects.py` & `gs_quant-1.0.2/gs_quant/backtests/backtest_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         Get a dataframe showing the PV and other risks and cash on each day in the backtest
         :param show_units: choose to show the units in the column names
         :type show_units: bool default False
         :return: bool default False
         :rtype: pandas.dataframe
         """
         dates_with_results = list(filter(lambda x: len(x[1]), self._results.items()))
-        summary = pd.DataFrame({date: {risk: results[risk].aggregate(True)
+        summary = pd.DataFrame({date: {risk: results[risk].aggregate(True, True)
                                        for risk in results.risk_measures} for date, results in dates_with_results}).T
         cash_summary = defaultdict(dict)
         for date, results in self._cash_dict.items():
             for ccy, value in results.items():
                 cash_summary[f'Cumulative Cash {ccy}'][date] = value
         if len(cash_summary) > 1:
             raise RuntimeError('Cannot aggregate cash in multiple currencies')
```

### Comparing `gs_quant-1.0.1/gs_quant/backtests/backtest_utils.py` & `gs_quant-1.0.2/gs_quant/backtests/backtest_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/backtests/core.py` & `gs_quant-1.0.2/gs_quant/backtests/core.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/backtests/data_handler.py` & `gs_quant-1.0.2/gs_quant/backtests/data_handler.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/backtests/data_sources.py` & `gs_quant-1.0.2/gs_quant/backtests/data_sources.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/backtests/decorator.py` & `gs_quant-1.0.2/gs_quant/backtests/decorator.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/backtests/equity_vol_engine.py` & `gs_quant-1.0.2/gs_quant/backtests/equity_vol_engine.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/backtests/event.py` & `gs_quant-1.0.2/gs_quant/backtests/event.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/backtests/execution_engine.py` & `gs_quant-1.0.2/gs_quant/backtests/execution_engine.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/backtests/generic_engine.py` & `gs_quant-1.0.2/gs_quant/backtests/generic_engine.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/backtests/order.py` & `gs_quant-1.0.2/gs_quant/backtests/order.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/backtests/predefined_asset_engine.py` & `gs_quant-1.0.2/gs_quant/backtests/predefined_asset_engine.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/backtests/strategy.py` & `gs_quant-1.0.2/gs_quant/backtests/strategy.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/backtests/strategy_systematic.py` & `gs_quant-1.0.2/gs_quant/backtests/strategy_systematic.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/backtests/triggers.py` & `gs_quant-1.0.2/gs_quant/backtests/triggers.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/base.py` & `gs_quant-1.0.2/gs_quant/base.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/common.py` & `gs_quant-1.0.2/gs_quant/common.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/config/__init__.py` & `gs_quant-1.0.2/gs_quant/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/config/options.py` & `gs_quant-1.0.2/gs_quant/config/options.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/config.ini` & `gs_quant-1.0.2/gs_quant/config.ini`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/content/reports_and_screens/00_fx/vol_screen_app.py` & `gs_quant-1.0.2/gs_quant/content/reports_and_screens/00_fx/vol_screen_app.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/context_base.py` & `gs_quant-1.0.2/gs_quant/context_base.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/data/__init__.py` & `gs_quant-1.0.2/gs_quant/data/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/data/coordinate.py` & `gs_quant-1.0.2/gs_quant/data/coordinate.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/data/core.py` & `gs_quant-1.0.2/gs_quant/data/core.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/data/dataset.py` & `gs_quant-1.0.2/gs_quant/data/dataset.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/data/fields.py` & `gs_quant-1.0.2/gs_quant/data/fields.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/data/log.py` & `gs_quant-1.0.2/gs_quant/data/log.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/data/query.py` & `gs_quant-1.0.2/gs_quant/data/query.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/data/stream.py` & `gs_quant-1.0.2/gs_quant/data/stream.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/datetime/__init__.py` & `gs_quant-1.0.2/gs_quant/datetime/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/datetime/date.py` & `gs_quant-1.0.2/gs_quant/datetime/date.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/datetime/gscalendar.py` & `gs_quant-1.0.2/gs_quant/datetime/gscalendar.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/datetime/point.py` & `gs_quant-1.0.2/gs_quant/datetime/point.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/datetime/relative_date.py` & `gs_quant-1.0.2/gs_quant/datetime/relative_date.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/datetime/rules.py` & `gs_quant-1.0.2/gs_quant/datetime/rules.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/datetime/time.py` & `gs_quant-1.0.2/gs_quant/datetime/time.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.datetime.date.business_day_count.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.datetime.date.business_day_count.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.datetime.date.business_day_offset.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.datetime.date.business_day_offset.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.datetime.date.date_range.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.datetime.date.date_range.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.datetime.date.is_business_day.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.datetime.date.is_business_day.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.datetime.date.prev_business_date.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.datetime.date.prev_business_date.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.datetime.point.point_sort_order.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.datetime.point.point_sort_order.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.abs_.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.abs_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.add.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.add.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.and_.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.and_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.ceil.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.ceil.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.divide.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.divide.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.exp.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.exp.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.filter_.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.filter_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.floor.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.floor.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.floordiv.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.floordiv.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.if_.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.if_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.log.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.log.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.multiply.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.multiply.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.not_.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.not_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.or_.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.or_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.power.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.power.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.repeat.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.repeat.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.smooth_spikes.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.smooth_spikes.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.sqrt.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.sqrt.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.subtract.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.subtract.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.algebra.weighted_sum.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.algebra.weighted_sum.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.analysis.count.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.analysis.count.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.analysis.diff.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.analysis.diff.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.analysis.first.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.analysis.first.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.analysis.lag.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.analysis.lag.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.analysis.last.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.analysis.last.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.analysis.last_value.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.analysis.last_value.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.analysis.weighted_sum.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.analysis.weighted_sum.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.backtesting.basket.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.backtesting.basket.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.datetime.align.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.datetime.align.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.datetime.date_range.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.datetime.date_range.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.datetime.day.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.datetime.day.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.datetime.interpolate.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.datetime.interpolate.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.datetime.month.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.datetime.month.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.datetime.prepend.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.datetime.prepend.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.datetime.quarter.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.datetime.quarter.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.datetime.union.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.datetime.union.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.datetime.value.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.datetime.value.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.datetime.weekday.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.datetime.weekday.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.datetime.year.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.datetime.year.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.econometrics.annualize.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.econometrics.annualize.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.econometrics.beta.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.econometrics.beta.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.econometrics.change.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.econometrics.change.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.econometrics.correlation.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.econometrics.correlation.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.econometrics.excess_returns_.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.econometrics.excess_returns_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.econometrics.index.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.econometrics.index.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.econometrics.max_drawdown.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.econometrics.max_drawdown.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.econometrics.prices.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.econometrics.prices.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.econometrics.returns.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.econometrics.returns.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.econometrics.sharpe_ratio.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.econometrics.sharpe_ratio.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.econometrics.volatility.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.econometrics.volatility.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.cov.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.cov.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.exponential_std.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.exponential_std.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.generate_series.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.generate_series.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.max_.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.max_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.mean.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.mean.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.median.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.median.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.min_.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.min_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.mode.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.mode.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.percentile.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.percentile.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.percentiles.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.percentiles.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.product.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.product.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.range_.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.range_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.std.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.std.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.sum_.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.sum_.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.var.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.var.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.winsorize.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.winsorize.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.statistics.zscores.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.statistics.zscores.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.technicals.bollinger_bands.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.technicals.bollinger_bands.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.technicals.exponential_moving_average.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.technicals.exponential_moving_average.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.technicals.exponential_spread_volatility.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.technicals.exponential_spread_volatility.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.technicals.exponential_volatility.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.technicals.exponential_volatility.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.technicals.moving_average.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.technicals.moving_average.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.technicals.relative_strength_index.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.technicals.relative_strength_index.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/docs/gs_quant.timeseries.technicals.smoothed_moving_average.html` & `gs_quant-1.0.2/gs_quant/docs/gs_quant.timeseries.technicals.smoothed_moving_average.html`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/entities/entitlements.py` & `gs_quant-1.0.2/gs_quant/entities/entitlements.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/entities/entity.py` & `gs_quant-1.0.2/gs_quant/entities/entity.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/entities/tree_entity.py` & `gs_quant-1.0.2/gs_quant/entities/tree_entity.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/errors.py` & `gs_quant-1.0.2/gs_quant/errors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/instrument/__init__.py` & `gs_quant-1.0.2/gs_quant/instrument/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/instrument/core.py` & `gs_quant-1.0.2/gs_quant/instrument/core.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/instrument/overrides.py` & `gs_quant-1.0.2/gs_quant/instrument/overrides.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/json_convertors.py` & `gs_quant-1.0.2/gs_quant/json_convertors.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/json_encoder.py` & `gs_quant-1.0.2/gs_quant/json_encoder.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/markets/__init__.py` & `gs_quant-1.0.2/gs_quant/markets/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/markets/baskets.py` & `gs_quant-1.0.2/gs_quant/markets/baskets.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/markets/core.py` & `gs_quant-1.0.2/gs_quant/markets/core.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/markets/factor.py` & `gs_quant-1.0.2/gs_quant/markets/factor.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/markets/hedge.py` & `gs_quant-1.0.2/gs_quant/markets/hedge.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/markets/historical.py` & `gs_quant-1.0.2/gs_quant/markets/historical.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/markets/index.py` & `gs_quant-1.0.2/gs_quant/markets/index.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/markets/indices_utils.py` & `gs_quant-1.0.2/gs_quant/markets/indices_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 from gs_quant.api.utils import ThreadPoolManager
 from gs_quant.base import EnumBase
 from gs_quant.datetime.date import prev_business_date
 from gs_quant.session import GsSession
 from gs_quant.target.data import DataQuery
 
 
+QUERY_LIMIT = 1000
+
+
 class BasketType(EnumBase, Enum):
     """ Basket Types """
     CUSTOM_BASKET = 'Custom Basket'
     RESEARCH_BASKET = 'Research Basket'
 
     def __repr__(self):
         return self.value
@@ -98,22 +101,23 @@
         return self.value
 
 
 class IndicesDatasets(EnumBase, Enum):
     """ Indices Datasets """
     BASKET_FUNDAMENTALS = 'BASKET_FUNDAMENTALS'
     COMPOSITE_THEMATIC_BETAS = 'COMPOSITE_THEMATIC_BETAS'
-    THEMATIC_FACTOR_BETAS_V1_STANDARD = 'THEMATIC_FACTOR_BETAS_V1_STANDARD'
+    CREDIT_EOD_PRICING_V1_STANDARD = 'CREDIT_EOD_PRICING_V1_STANDARD'
     CORPORATE_ACTIONS = 'CA'
     GIRBASKETCONSTITUENTS = 'GIRBASKETCONSTITUENTS'
     GSBASKETCONSTITUENTS = 'GSBASKETCONSTITUENTS'
     GSCB_FLAGSHIP = 'GSCB_FLAGSHIP'
     GSCREDITBASKETCONSTITUENTS = 'GSCREDITBASKETCONSTITUENTS'
     STS_FUNDAMENTALS = 'STS_FUNDAMENTALS'
     STS_INDICATIVE_LEVELS = 'STS_INDICATIVE_LEVELS'
+    THEMATIC_FACTOR_BETAS_V1_STANDARD = 'THEMATIC_FACTOR_BETAS_V1_STANDARD'
 
     def __repr__(self):
         return self.value
 
 
 class PriceType(EnumBase, Enum):
     """ Index Price Types """
@@ -256,15 +260,26 @@
         query[k] = v
     if region:
         query['region'] = region
     if styles:
         query['styles'] = styles
     query = dict(fields=fields, type=basket_type, asset_class=asset_class, is_pair_basket=[False],
                  flagship=[True], **query)
-    return GsAssetApi.get_many_assets_data_scroll(**query, as_of=as_of, limit=2000, scroll='1m')
+    return GsAssetApi.get_many_assets_data_scroll(**query, as_of=as_of, limit=QUERY_LIMIT, scroll='1m')
+
+
+def __get_dataset_id(asset_class: AssetClass, basket_type: BasketType, data_type: str) -> str:
+    if asset_class == AssetClass.Equity or asset_class == AssetClass.Equity.value:
+        if data_type == 'price':
+            return IndicesDatasets.GSCB_FLAGSHIP.value
+        elif basket_type == BasketType.CUSTOM_BASKET or basket_type == BasketType.CUSTOM_BASKET.value:
+            return IndicesDatasets.GSBASKETCONSTITUENTS.value
+        else:
+            return IndicesDatasets.GIRBASKETCONSTITUENTS.value
+    raise NotImplementedError(f'{data_type} data for {asset_class} baskets is unsupported at this time')
 
 
 def get_flagship_baskets(fields: List[str] = [],
                          basket_type: List[BasketType] = BasketType.to_list(),
                          asset_class: List[AssetClass] = [AssetClass.Equity],
                          region: List[Region] = None,
                          styles: List[Union[CustomBasketStyles, ResearchBasketStyles]] = None,
@@ -384,24 +399,28 @@
 
     :func:`get_flagships_with_assets` :func:`get_flagship_baskets` :func:`get_flagships_constituents`
     """
     start, end = start or prev_business_date(), end or prev_business_date()
     assets = __get_baskets(fields=fields, basket_type=basket_type, asset_class=asset_class, region=region,
                            styles=styles, **kwargs)
     baskets = {b.get('id'): b for b in assets}
-    coverage = GsDataApi.get_coverage(dataset_id=IndicesDatasets.GSCB_FLAGSHIP.value, fields=['id'])
+    dataset_id = __get_dataset_id(asset_class=asset_class[0], basket_type=basket_type[0], data_type='price')
+    coverage = GsDataApi.get_coverage(dataset_id=dataset_id, fields=['id'])
     mqids = [b.get('assetId') for b in coverage if b.get('assetId') in baskets.keys()]
-    response = GsDataApi.query_data(query=DataQuery(where={'assetId': mqids}, startDate=start, endDate=end),
-                                    dataset_id=IndicesDatasets.GSCB_FLAGSHIP.value)
-    performance = []
+    batches = [mqids[i * 500:(i + 1) * 500] for i in range((len(mqids) + 500 - 1) // 500)]
+    response, performance = [], []
+    for b in batches:
+        response += GsDataApi.query_data(query=DataQuery(where={'assetId': b}, startDate=start, endDate=end),
+                                         dataset_id=dataset_id)
     for b in response:
         data = baskets.get(b.get('assetId'))
-        data['closePrice'] = b.get('closePrice')
-        data['date'] = b.get('date')
-        performance.append(data)
+        b.update(data)
+        b.pop('assetId')
+        b.pop('updateTime')
+        performance.append(b)
     return pd.DataFrame(performance)
 
 
 def get_flagships_constituents(fields: List[str] = [],
                                basket_type: List[BasketType] = BasketType.to_list(),
                                asset_class: List[AssetClass] = [AssetClass.Equity],
                                region: List[Region] = None,
@@ -437,46 +456,47 @@
     **See also**
 
     :func:`get_flagships_with_assets` :func:`get_flagships_performance` :func:`get_flagship_baskets`
     """
     start, end = start or prev_business_date(), end or prev_business_date()
     basket_fields = list(set(fields).union(set(['id', 'name', 'ticker', 'region', 'type', 'styles',
                                                'liveDate', 'assetClass'])))
+    fields = list(set(fields).union(set(['id'])))
     response = __get_baskets(fields=['id'], basket_type=basket_type, asset_class=asset_class,
                              region=region, styles=styles, **kwargs)
     basket_ids = [b.get('id') for b in response]
-    coverage = GsDataApi.get_coverage(dataset_id=IndicesDatasets.GSCB_FLAGSHIP.value, fields=basket_fields,
-                                      include_history=True)
+    cov_dataset_id = __get_dataset_id(asset_class=asset_class[0], basket_type=basket_type[0], data_type='price')
+    coverage = GsDataApi.get_coverage(dataset_id=cov_dataset_id, fields=basket_fields, include_history=True)
     basket_map = {b['assetId']: {**b, 'constituents': []} for b in coverage if b['assetId'] in basket_ids}
-    cbs = [b['assetId'] for b in basket_map.values() if b['type'] == BasketType.CUSTOM_BASKET.value]
-    rbs = [b['assetId'] for b in basket_map.values() if b['type'] == BasketType.RESEARCH_BASKET.value]
 
-    constituents_data, tasks = [], []
+    basket_dataset_query_map, constituents_data, tasks = {}, [], []
+    # get appropriate dataset for each basket
+    for b in basket_map.values():
+        dataset_id = __get_dataset_id(asset_class=b['assetClass'], basket_type=b['type'], data_type='constituents')
+        if dataset_id:
+            basket_dataset_query_map[dataset_id] = basket_dataset_query_map.get(dataset_id, []) + [b['assetId']]
+
     # query constituents in batches of 25
-    cb_batches = [cbs[i * 25:(i + 1) * 25] for i in range((len(cbs) + 25 - 1) // 25)]
-    rb_batches = [rbs[i * 25:(i + 1) * 25] for i in range((len(rbs) + 25 - 1) // 25)]
-    for batch in cb_batches:
-        tasks.append(partial(GsDataApi.query_data,
-                             query=DataQuery(where={'assetId': batch}, startDate=start, endDate=end),
-                             dataset_id=IndicesDatasets.GSBASKETCONSTITUENTS.value))
-    for batch in rb_batches:
-        tasks.append(partial(GsDataApi.query_data,
-                             query=DataQuery(where={'assetId': batch}, startDate=start, endDate=end),
-                             dataset_id=IndicesDatasets.GIRBASKETCONSTITUENTS.value))
+    for ds, ids in basket_dataset_query_map.items():
+        batches = [ids[i * 25:(i + 1) * 25] for i in range((len(ids) + 25 - 1) // 25)]
+        for batch in batches:
+            tasks.append(partial(GsDataApi.query_data,
+                                 query=DataQuery(where={'assetId': batch}, startDate=start, endDate=end),
+                                 dataset_id=ds))
 
     # run 5 parallel dataset queries at a time
     tasks = [tasks[i * 5:(i + 1) * 5] for i in range((len(tasks) + 5 - 1) // 5)]
     for task in tasks:
         constituents_data += ThreadPoolManager.run_async(task)
         sleep(1)
     constituents_data = reduce(lambda a, b: a + b, constituents_data)
 
     # fetch asset positions data
     asset_ids = set([row['underlyingAssetId'] for row in constituents_data])
-    asset_data = GsAssetApi.get_many_assets_data_scroll(id=asset_ids, fields=fields, limit=2000, scroll='1m')
+    asset_data = GsAssetApi.get_many_assets_data_scroll(id=asset_ids, fields=fields, limit=QUERY_LIMIT, scroll='1m')
     asset_data_map = {get(asset, 'id'): asset for asset in asset_data}
 
     for row in constituents_data:
         basket_id = get(row, 'assetId', '')
         asset_id = get(row, 'underlyingAssetId', '')
         asset_id_map = get(asset_data_map, asset_id, {})
         for f in fields:
@@ -515,9 +535,9 @@
 
     :func:`get_flagships_constituents`
     """
     query = dict(fields=['id', 'name', 'region', 'ticker', 'type', 'assetClass'], type=[basket_type],
                  asset_class=[asset_class], is_pair_basket=[False], listed=[True])
     if asset_class != AssetClass.Equity:
         query.pop('is_pair_basket')
-    response = GsAssetApi.get_many_assets_data_scroll(**query, as_of=as_of, limit=2000, scroll='1m')
+    response = GsAssetApi.get_many_assets_data_scroll(**query, as_of=as_of, limit=QUERY_LIMIT, scroll='1m')
     return pd.DataFrame(response)
```

### Comparing `gs_quant-1.0.1/gs_quant/markets/markets.py` & `gs_quant-1.0.2/gs_quant/markets/markets.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/markets/optimizer.py` & `gs_quant-1.0.2/gs_quant/markets/optimizer.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/markets/portfolio.py` & `gs_quant-1.0.2/gs_quant/markets/portfolio.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/markets/portfolio_manager.py` & `gs_quant-1.0.2/gs_quant/markets/portfolio_manager.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/markets/portfolio_manager_utils.py` & `gs_quant-1.0.2/gs_quant/markets/portfolio_manager_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/markets/position_set.py` & `gs_quant-1.0.2/gs_quant/markets/position_set.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/markets/report.py` & `gs_quant-1.0.2/gs_quant/markets/report.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/markets/report_utils.py` & `gs_quant-1.0.2/gs_quant/markets/report_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/markets/screens.py` & `gs_quant-1.0.2/gs_quant/markets/screens.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/markets/securities.py` & `gs_quant-1.0.2/gs_quant/markets/securities.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/models/__init__.py` & `gs_quant-1.0.2/gs_quant/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/models/epidemiology.py` & `gs_quant-1.0.2/gs_quant/models/epidemiology.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/models/risk_model.py` & `gs_quant-1.0.2/gs_quant/models/risk_model.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/models/risk_model_utils.py` & `gs_quant-1.0.2/gs_quant/models/risk_model_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/priceable.py` & `gs_quant-1.0.2/gs_quant/priceable.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/quote_reports/core.py` & `gs_quant-1.0.2/gs_quant/quote_reports/core.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/risk/__init__.py` & `gs_quant-1.0.2/gs_quant/risk/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/risk/core.py` & `gs_quant-1.0.2/gs_quant/risk/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -400,21 +400,24 @@
             self.validators = tuple([value])
 
     @property
     def raw_value(self):
         return self.validators
 
 
-def aggregate_risk(results: Iterable[Union[DataFrameWithInfo, Future]], threshold: Optional[float] = None) \
+def aggregate_risk(results: Iterable[Union[DataFrameWithInfo, Future]],
+                   threshold: Optional[float] = None,
+                   allow_heterogeneous_types: bool = False) \
         -> pd.DataFrame:
     """
     Combine the results of multiple InstrumentBase.calc() calls, into a single result
 
     :param results: An iterable of Dataframes and/or Futures (returned by InstrumentBase.calc())
     :param threshold: exclude values whose absolute value falls below this threshold
+    :param allow_heterogeneous_types: allow Series to be converted to DataFrames before aggregating
     :return: A Dataframe with the aggregated results
 
     **Examples**
 
     >>> from gs_quant.instrument import IRCap, IRFloor
     >>> from gs_quant.markets import PricingContext
     >>> from gs_quant.risk import IRDelta, IRVega
@@ -429,43 +432,51 @@
     >>>
     >>> delta = aggregate_risk(delta_f, threshold=0.1)
     >>> vega = aggregate_risk(vega_f)
 
     delta_f and vega_f are lists of futures, where the result will be a Dataframe
     delta and vega are Dataframes, representing the merged risk of the individual instruments
     """
-    dfs = [r.result().raw_value if isinstance(r, Future) else r.raw_value for r in results]
+    def get_df(result_obj):
+        if isinstance(result_obj, Future):
+            result_obj = result_obj.result()
+        if isinstance(result_obj, pd.Series) and allow_heterogeneous_types:
+            return pd.DataFrame(result_obj.raw_value).T
+        return result_obj.raw_value
+
+    dfs = [get_df(r) for r in results]
     result = pd.concat(dfs).fillna(0)
     result = result.groupby([c for c in result.columns if c != 'value'], as_index=False).sum()
 
     if threshold is not None:
         result = result[result.value.abs() > threshold]
 
     return sort_risk(result)
 
 
 ResultType = Union[None, dict, tuple, DataFrameWithInfo, FloatWithInfo, SeriesWithInfo]
 
 
-def aggregate_results(results: Iterable[ResultType], allow_mismatch_risk_keys=False) -> ResultType:
+def aggregate_results(results: Iterable[ResultType], allow_mismatch_risk_keys=False,
+                      allow_heterogeneous_types=False) -> ResultType:
     unit = None
     risk_key = None
     results = tuple(results)
 
     if not len(results):
         return None
 
     for result in results:
         if isinstance(result, Exception):
             raise Exception
 
         if result.error:
             raise ValueError('Cannot aggregate results in error')
 
-        if not isinstance(result, type(results[0])):
+        if not allow_heterogeneous_types and not isinstance(result, type(results[0])):
             raise ValueError(f'Cannot aggregate heterogeneous types: {type(result)} vs {type(results[0])}')
 
         if result.unit:
             if unit and unit != result.unit:
                 raise ValueError('Cannot aggregate results with different units')
 
             unit = unit or result.unit
@@ -481,15 +492,16 @@
     elif isinstance(inst, tuple):
         return tuple(set(itertools.chain.from_iterable(results)))
     elif isinstance(inst, FloatWithInfo):
         return FloatWithInfo(risk_key, sum(results), unit=unit)
     elif isinstance(inst, SeriesWithInfo):
         return SeriesWithInfo(sum(results), risk_key=risk_key, unit=unit)
     elif isinstance(inst, DataFrameWithInfo):
-        return DataFrameWithInfo(aggregate_risk(results), risk_key=risk_key, unit=unit)
+        return DataFrameWithInfo(aggregate_risk(results, allow_heterogeneous_types=allow_heterogeneous_types),
+                                 risk_key=risk_key, unit=unit)
 
 
 def subtract_risk(left: DataFrameWithInfo, right: DataFrameWithInfo) -> pd.DataFrame:
     """Subtract bucketed risk. Dimensions must be identical
 
     :param left: Results to substract from
     :param right: Results to substract
```

### Comparing `gs_quant-1.0.1/gs_quant/risk/measures.py` & `gs_quant-1.0.2/gs_quant/risk/measures.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/risk/result_handlers.py` & `gs_quant-1.0.2/gs_quant/risk/result_handlers.py`

 * *Files 9% similar despite different names*

```diff
@@ -308,14 +308,44 @@
                 ('mkt_tags', 'tags'),
                 ('mkt_quoting_style', 'quotingStyle'),
                 ('value', 'value'))
 
     return __dataframe_handler(coordinates, mappings, risk_key, request_id=request_id)
 
 
+def mmapi_pca_table_handler(result: dict, risk_key: RiskKey, _instrument: InstrumentBase,
+                            request_id: Optional[str] = None) -> DataFrameWithInfo:
+    coordinates = []
+    for r in result['rows']:
+        raw_point = r['coordinate'].get('point', '')
+        point = ';'.join(raw_point) if isinstance(raw_point, list) else raw_point
+        r['coordinate'].update({'point': point})
+        r['coordinate'].update({'value': r['value']})
+        r['coordinate'].update({'layer1': r['layer1']})
+        r['coordinate'].update({'layer2': r['layer2']})
+        r['coordinate'].update({'layer3': r['layer3']})
+        r['coordinate'].update({'level': r['level']})
+        r['coordinate'].update({'sensitivity': r['sensitivity']})
+        coordinates.append(r['coordinate'])
+
+    mappings = (('mkt_type', 'type'),
+                ('mkt_asset', 'asset'),
+                ('mkt_class', 'assetClass'),
+                ('mkt_point', 'point'),
+                ('mkt_quoting_style', 'quotingStyle'),
+                ('value', 'value'),
+                ('layer1', 'layer1'),
+                ('layer2', 'layer2'),
+                ('layer3', 'layer3'),
+                ('level', 'level'),
+                ('sensitivity', 'sensitivity'))
+
+    return __dataframe_handler(coordinates, mappings, risk_key, request_id=request_id)
+
+
 def mqvs_validators_handler(result: dict, risk_key: RiskKey, _instrument: InstrumentBase,
                             request_id: Optional[str] = None) -> MQVSValidatorDefnsWithInfo:
     validators = [MQVSValidatorDefn.from_dict(r) for r in result['validators']]
     return MQVSValidatorDefnsWithInfo(risk_key, tuple(validators), request_id=request_id)
 
 
 def market_handler(result: dict, risk_key: RiskKey, _instrument: InstrumentBase,
@@ -331,14 +361,15 @@
 result_handlers = {
     'Error': error_handler,
     'IRPCashflowTable': cashflows_handler,
     'LegDefinition': leg_definition_handler,
     'Message': message_handler,
     'MDAPITable': mdapi_table_handler,
     'MMAPITable': mmapi_table_handler,
+    'MMAPIPCA': mmapi_pca_table_handler,
     'MQVSValidators': mqvs_validators_handler,
     'NumberAndUnit': number_and_unit_handler,
     'RequireAssets': required_assets_handler,
     'Risk': risk_handler,
     'RiskByClass': risk_by_class_handler,
     'RiskVector': risk_vector_handler,
     'FixingTable': fixing_table_handler,
```

### Comparing `gs_quant-1.0.1/gs_quant/risk/results.py` & `gs_quant-1.0.2/gs_quant/risk/results.py`

 * *Files 0% similar despite different names*

```diff
@@ -771,20 +771,21 @@
                 transformed_future.set_result(result)
                 transformed_future.done()
                 futures.append(transformed_future)
             return PortfolioRiskResult(self.portfolio, self.risk_measures, futures)
         else:
             return self
 
-    def aggregate(self, allow_mismatch_risk_keys=False) -> Union[float, pd.DataFrame, pd.Series,
-                                                                 MultipleRiskMeasureResult]:
+    def aggregate(self, allow_mismatch_risk_keys=False,
+                  allow_heterogeneous_types=False) -> Union[float, pd.DataFrame, pd.Series, MultipleRiskMeasureResult]:
         if len(self.__risk_measures) > 1:
             return MultipleRiskMeasureResult(self.portfolio, ((r, self[r].aggregate()) for r in self.__risk_measures))
         else:
-            return aggregate_results(self.__results(), allow_mismatch_risk_keys=allow_mismatch_risk_keys)
+            return aggregate_results(self.__results(), allow_mismatch_risk_keys=allow_mismatch_risk_keys,
+                                     allow_heterogeneous_types=allow_heterogeneous_types)
 
     def _to_records(self, display_options: DisplayOptions = None):
         def get_records(rec):
             temp = []
             for f in rec.futures:
                 if isinstance(f.result(), ResultInfo) or isinstance(f.result(), MultipleRiskMeasureResult) \
                         or isinstance(f.result(), MultipleScenarioResult):
```

### Comparing `gs_quant-1.0.1/gs_quant/risk/scenario_utils.py` & `gs_quant-1.0.2/gs_quant/risk/scenario_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/risk/scenarios.py` & `gs_quant-1.0.2/gs_quant/risk/scenarios.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/risk/transform.py` & `gs_quant-1.0.2/gs_quant/risk/transform.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/session.py` & `gs_quant-1.0.2/gs_quant/session.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/__init__.py` & `gs_quant-1.0.2/gs_quant/target/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/assets.py` & `gs_quant-1.0.2/gs_quant/target/assets.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/assets_screener.py` & `gs_quant-1.0.2/gs_quant/target/assets_screener.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/backtests.py` & `gs_quant-1.0.2/gs_quant/target/backtests.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/base_screener.py` & `gs_quant-1.0.2/gs_quant/target/base_screener.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/charts.py` & `gs_quant-1.0.2/gs_quant/target/charts.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/common.py` & `gs_quant-1.0.2/gs_quant/target/common.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/content.py` & `gs_quant-1.0.2/gs_quant/target/content.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/coordinates.py` & `gs_quant-1.0.2/gs_quant/target/coordinates.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/countries.py` & `gs_quant-1.0.2/gs_quant/target/countries.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/data.py` & `gs_quant-1.0.2/gs_quant/target/data.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/data_screen.py` & `gs_quant-1.0.2/gs_quant/target/data_screen.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/groups.py` & `gs_quant-1.0.2/gs_quant/target/groups.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/hedge.py` & `gs_quant-1.0.2/gs_quant/target/hedge.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/indices.py` & `gs_quant-1.0.2/gs_quant/target/indices.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/instrument.py` & `gs_quant-1.0.2/gs_quant/target/instrument.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/measures.py` & `gs_quant-1.0.2/gs_quant/target/measures.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/monitor.py` & `gs_quant-1.0.2/gs_quant/target/monitor.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/portfolios.py` & `gs_quant-1.0.2/gs_quant/target/portfolios.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/price.py` & `gs_quant-1.0.2/gs_quant/target/price.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/reports.py` & `gs_quant-1.0.2/gs_quant/target/reports.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/risk.py` & `gs_quant-1.0.2/gs_quant/target/risk.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/risk_models.py` & `gs_quant-1.0.2/gs_quant/target/risk_models.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/screens.py` & `gs_quant-1.0.2/gs_quant/target/screens.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/secmaster.py` & `gs_quant-1.0.2/gs_quant/target/secmaster.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/trades.py` & `gs_quant-1.0.2/gs_quant/target/trades.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/workflow_quote.py` & `gs_quant-1.0.2/gs_quant/target/workflow_quote.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/target/workspaces_markets.py` & `gs_quant-1.0.2/gs_quant/target/workspaces_markets.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/analytics/test_datagrid.py` & `gs_quant-1.0.2/gs_quant/test/analytics/test_datagrid.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/analytics/test_sorting_and_filtering.py` & `gs_quant-1.0.2/gs_quant/test/analytics/test_sorting_and_filtering.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/analytics/test_workspace.py` & `gs_quant-1.0.2/gs_quant/test/analytics/test_workspace.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/api/test_assets.py` & `gs_quant-1.0.2/gs_quant/test/api/test_assets.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/api/test_backtests.py` & `gs_quant-1.0.2/gs_quant/test/api/test_backtests.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/api/test_base_screener.py` & `gs_quant-1.0.2/gs_quant/test/api/test_base_screener.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/api/test_cache.py` & `gs_quant-1.0.2/gs_quant/test/api/test_cache.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/api/test_carbon.py` & `gs_quant-1.0.2/gs_quant/test/api/test_carbon.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/api/test_content.py` & `gs_quant-1.0.2/gs_quant/test/api/test_content.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/api/test_data.py` & `gs_quant-1.0.2/gs_quant/test/api/test_data.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/api/test_data_screen.py` & `gs_quant-1.0.2/gs_quant/test/api/test_data_screen.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/api/test_esg.py` & `gs_quant-1.0.2/gs_quant/test/api/test_esg.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/api/test_fred.py` & `gs_quant-1.0.2/gs_quant/test/api/test_fred.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/api/test_groups.py` & `gs_quant-1.0.2/gs_quant/test/api/test_groups.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/api/test_index.py` & `gs_quant-1.0.2/gs_quant/test/api/test_index.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/api/test_instruments.py` & `gs_quant-1.0.2/gs_quant/test/api/test_instruments.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/api/test_json.py` & `gs_quant-1.0.2/gs_quant/test/api/test_json.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/api/test_monitor.py` & `gs_quant-1.0.2/gs_quant/test/api/test_monitor.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/api/test_portfolios.py` & `gs_quant-1.0.2/gs_quant/test/api/test_portfolios.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/api/test_reports.py` & `gs_quant-1.0.2/gs_quant/test/api/test_reports.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/api/test_risk.py` & `gs_quant-1.0.2/gs_quant/test/api/test_risk.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/api/test_risk_models.py` & `gs_quant-1.0.2/gs_quant/test/api/test_risk_models.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/api/test_target.py` & `gs_quant-1.0.2/gs_quant/test/api/test_target.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/api/test_thread_manager.py` & `gs_quant-1.0.2/gs_quant/test/api/test_thread_manager.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/api/test_users.py` & `gs_quant-1.0.2/gs_quant/test/api/test_users.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/backtest/test_backtest_eq_vol_engine.py` & `gs_quant-1.0.2/gs_quant/test/backtest/test_backtest_eq_vol_engine.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/backtest/test_backtest_flow_vol.py` & `gs_quant-1.0.2/gs_quant/test/backtest/test_backtest_flow_vol.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/backtest/test_backtest_predefined.py` & `gs_quant-1.0.2/gs_quant/test/backtest/test_backtest_predefined.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/backtest/test_generic_engine.py` & `gs_quant-1.0.2/gs_quant/test/backtest/test_generic_engine.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/backtest/test_triggers.py` & `gs_quant-1.0.2/gs_quant/test/backtest/test_triggers.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/data/test_data_coordinate.py` & `gs_quant-1.0.2/gs_quant/test/data/test_data_coordinate.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/data/test_dataset.py` & `gs_quant-1.0.2/gs_quant/test/data/test_dataset.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/datetime_/test_date.py` & `gs_quant-1.0.2/gs_quant/test/datetime_/test_date.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/datetime_/test_gscalendar.py` & `gs_quant-1.0.2/gs_quant/test/datetime_/test_gscalendar.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/datetime_/test_point.py` & `gs_quant-1.0.2/gs_quant/test/datetime_/test_point.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/datetime_/test_relative_date.py` & `gs_quant-1.0.2/gs_quant/test/datetime_/test_relative_date.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/datetime_/test_time.py` & `gs_quant-1.0.2/gs_quant/test/datetime_/test_time.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/fixtures/content.py` & `gs_quant-1.0.2/gs_quant/test/fixtures/content.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/markets/test_baskets.py` & `gs_quant-1.0.2/gs_quant/test/markets/test_baskets.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/markets/test_hedger.py` & `gs_quant-1.0.2/gs_quant/test/markets/test_hedger.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/markets/test_instrument.py` & `gs_quant-1.0.2/gs_quant/test/markets/test_instrument.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/markets/test_portfolio.py` & `gs_quant-1.0.2/gs_quant/test/markets/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/markets/test_portfolio_manager.py` & `gs_quant-1.0.2/gs_quant/test/markets/test_portfolio_manager.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/markets/test_pricing_context.py` & `gs_quant-1.0.2/gs_quant/test/markets/test_pricing_context.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/markets/test_report.py` & `gs_quant-1.0.2/gs_quant/test/markets/test_report.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/markets/test_securities.py` & `gs_quant-1.0.2/gs_quant/test/markets/test_securities.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/models/__init__.py` & `gs_quant-1.0.2/gs_quant/test/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/models/test_epidemiology.py` & `gs_quant-1.0.2/gs_quant/test/models/test_epidemiology.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/models/test_risk_model.py` & `gs_quant-1.0.2/gs_quant/test/models/test_risk_model.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/test_base.py` & `gs_quant-1.0.2/gs_quant/test/test_base.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/timeseries/multi_measure/test_commod.py` & `gs_quant-1.0.2/gs_quant/test/timeseries/multi_measure/test_commod.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/timeseries/multi_measure/test_measure_registry.py` & `gs_quant-1.0.2/gs_quant/test/timeseries/multi_measure/test_measure_registry.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/timeseries/test_algebra.py` & `gs_quant-1.0.2/gs_quant/test/timeseries/test_algebra.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/timeseries/test_analysis.py` & `gs_quant-1.0.2/gs_quant/test/timeseries/test_analysis.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/timeseries/test_backtesting.py` & `gs_quant-1.0.2/gs_quant/test/timeseries/test_backtesting.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/timeseries/test_datetime.py` & `gs_quant-1.0.2/gs_quant/test/timeseries/test_datetime.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/timeseries/test_econometrics.py` & `gs_quant-1.0.2/gs_quant/test/timeseries/test_econometrics.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/timeseries/test_helper.py` & `gs_quant-1.0.2/gs_quant/test/timeseries/test_helper.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/timeseries/test_measures.py` & `gs_quant-1.0.2/gs_quant/test/timeseries/test_measures.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/timeseries/test_measures_countries.py` & `gs_quant-1.0.2/gs_quant/test/timeseries/test_measures_countries.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/timeseries/test_measures_fx_vol.py` & `gs_quant-1.0.2/gs_quant/test/timeseries/test_measures_fx_vol.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/timeseries/test_measures_inflation.py` & `gs_quant-1.0.2/gs_quant/test/timeseries/test_measures_inflation.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/timeseries/test_measures_portfolios.py` & `gs_quant-1.0.2/gs_quant/test/timeseries/test_measures_portfolios.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/timeseries/test_measures_rates.py` & `gs_quant-1.0.2/gs_quant/test/timeseries/test_measures_rates.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/timeseries/test_measures_reports.py` & `gs_quant-1.0.2/gs_quant/test/timeseries/test_measures_reports.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/timeseries/test_measures_risk_models.py` & `gs_quant-1.0.2/gs_quant/test/timeseries/test_measures_risk_models.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/timeseries/test_measures_xccy.py` & `gs_quant-1.0.2/gs_quant/test/timeseries/test_measures_xccy.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/timeseries/test_rolling.py` & `gs_quant-1.0.2/gs_quant/test/timeseries/test_rolling.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/timeseries/test_statistics.py` & `gs_quant-1.0.2/gs_quant/test/timeseries/test_statistics.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/timeseries/test_tca.py` & `gs_quant-1.0.2/gs_quant/test/timeseries/test_tca.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/timeseries/test_technicals.py` & `gs_quant-1.0.2/gs_quant/test/timeseries/test_technicals.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/timeseries/test_timeseries.py` & `gs_quant-1.0.2/gs_quant/test/timeseries/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/timeseries/utils.py` & `gs_quant-1.0.2/gs_quant/test/timeseries/utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/utils/datagrid_test_utils.py` & `gs_quant-1.0.2/gs_quant/test/utils/datagrid_test_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/utils/mock_calc.py` & `gs_quant-1.0.2/gs_quant/test/utils/mock_calc.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/utils/mock_data.py` & `gs_quant-1.0.2/gs_quant/test/utils/mock_data.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/utils/mock_request.py` & `gs_quant-1.0.2/gs_quant/test/utils/mock_request.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/test/utils/test_utils.py` & `gs_quant-1.0.2/gs_quant/test/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/timeseries/__init__.py` & `gs_quant-1.0.2/gs_quant/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/timeseries/algebra.py` & `gs_quant-1.0.2/gs_quant/timeseries/algebra.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/timeseries/analysis.py` & `gs_quant-1.0.2/gs_quant/timeseries/analysis.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/timeseries/backtesting.py` & `gs_quant-1.0.2/gs_quant/timeseries/backtesting.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/timeseries/datetime.py` & `gs_quant-1.0.2/gs_quant/timeseries/datetime.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/timeseries/econometrics.py` & `gs_quant-1.0.2/gs_quant/timeseries/econometrics.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/timeseries/helper.py` & `gs_quant-1.0.2/gs_quant/timeseries/helper.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/timeseries/measure_registry.py` & `gs_quant-1.0.2/gs_quant/timeseries/measure_registry.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/timeseries/measures.py` & `gs_quant-1.0.2/gs_quant/timeseries/measures.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/timeseries/measures_countries.py` & `gs_quant-1.0.2/gs_quant/timeseries/measures_countries.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/timeseries/measures_fx_vol.py` & `gs_quant-1.0.2/gs_quant/timeseries/measures_fx_vol.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/timeseries/measures_helper.py` & `gs_quant-1.0.2/gs_quant/timeseries/measures_helper.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/timeseries/measures_inflation.py` & `gs_quant-1.0.2/gs_quant/timeseries/measures_inflation.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/timeseries/measures_portfolios.py` & `gs_quant-1.0.2/gs_quant/timeseries/measures_portfolios.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/timeseries/measures_rates.py` & `gs_quant-1.0.2/gs_quant/timeseries/measures_rates.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/timeseries/measures_reports.py` & `gs_quant-1.0.2/gs_quant/timeseries/measures_reports.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/timeseries/measures_risk_models.py` & `gs_quant-1.0.2/gs_quant/timeseries/measures_risk_models.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/timeseries/measures_xccy.py` & `gs_quant-1.0.2/gs_quant/timeseries/measures_xccy.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/timeseries/statistics.py` & `gs_quant-1.0.2/gs_quant/timeseries/statistics.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/timeseries/tca.py` & `gs_quant-1.0.2/gs_quant/timeseries/tca.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/timeseries/technicals.py` & `gs_quant-1.0.2/gs_quant/timeseries/technicals.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/tracing/__init__.py` & `gs_quant-1.0.2/gs_quant/tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant/tracing/tracing.py` & `gs_quant-1.0.2/gs_quant/tracing/tracing.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant.egg-info/PKG-INFO` & `gs_quant-1.0.2/gs_quant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-quant
-Version: 1.0.1
+Version: 1.0.2
 Summary: Goldman Sachs Quant
 Home-page: https://marquee.gs.com
 Author: Goldman Sachs
 Author-email: developer@gs.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Description: # GS Quant
```

### Comparing `gs_quant-1.0.1/gs_quant.egg-info/SOURCES.txt` & `gs_quant-1.0.2/gs_quant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/gs_quant.egg-info/requires.txt` & `gs_quant-1.0.2/gs_quant.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/setup.py` & `gs_quant-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `gs_quant-1.0.1/versioneer.py` & `gs_quant-1.0.2/versioneer.py`

 * *Files identical despite different names*

