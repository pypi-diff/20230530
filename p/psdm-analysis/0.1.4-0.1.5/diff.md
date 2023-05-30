# Comparing `tmp/psdm-analysis-0.1.4.tar.gz` & `tmp/psdm-analysis-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psdm-analysis-0.1.4.tar", max compression
+gzip compressed data, was "psdm-analysis-0.1.5.tar", max compression
```

## Comparing `psdm-analysis-0.1.4.tar` & `psdm-analysis-0.1.5.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0     1581 2023-01-31 09:55:39.404671 psdm-analysis-0.1.4/LICENSE
--rw-r--r--   0        0        0      373 2023-04-19 12:49:15.037328 psdm-analysis-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038177 psdm-analysis-0.1.4/psdm_analysis/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038287 psdm-analysis-0.1.4/psdm_analysis/analysis/__init__.py
--rw-r--r--   0        0        0      601 2023-04-19 12:49:15.038571 psdm-analysis-0.1.4/psdm_analysis/analysis/calc.py
--rw-r--r--   0        0        0     1200 2023-04-19 12:49:15.038918 psdm-analysis-0.1.4/psdm_analysis/analysis/grid.py
--rw-r--r--   0        0        0        0 2023-05-02 07:38:45.729757 psdm-analysis-0.1.4/psdm_analysis/conversion/__init__.py
--rw-r--r--   0        0        0     3960 2023-05-02 07:38:45.730387 psdm-analysis-0.1.4/psdm_analysis/conversion/pandapower.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038964 psdm-analysis-0.1.4/psdm_analysis/io/__init__.py
--rw-r--r--   0        0        0     2842 2023-04-19 12:49:15.039092 psdm-analysis-0.1.4/psdm_analysis/io/utils.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039122 psdm-analysis-0.1.4/psdm_analysis/models/__init__.py
--rw-r--r--   0        0        0     9503 2023-05-23 11:13:37.867698 psdm-analysis-0.1.4/psdm_analysis/models/entity.py
--rw-r--r--   0        0        0     6788 2023-05-26 10:45:12.995987 psdm-analysis-0.1.4/psdm_analysis/models/grid_with_results.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039422 psdm-analysis-0.1.4/psdm_analysis/models/input/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039466 psdm-analysis-0.1.4/psdm_analysis/models/input/connector/__init__.py
--rw-r--r--   0        0        0     1195 2023-05-23 11:13:37.868712 psdm-analysis-0.1.4/psdm_analysis/models/input/connector/connector.py
--rw-r--r--   0        0        0     1888 2023-05-23 11:13:37.869005 psdm-analysis-0.1.4/psdm_analysis/models/input/connector/lines.py
--rw-r--r--   0        0        0      674 2023-05-23 11:13:37.869378 psdm-analysis-0.1.4/psdm_analysis/models/input/connector/switches.py
--rw-r--r--   0        0        0     2240 2023-05-29 07:50:38.432624 psdm-analysis-0.1.4/psdm_analysis/models/input/connector/transformer.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.040065 psdm-analysis-0.1.4/psdm_analysis/models/input/container/__init__.py
--rw-r--r--   0        0        0     6724 2023-05-29 07:47:15.753072 psdm-analysis-0.1.4/psdm_analysis/models/input/container/grid_container.py
--rw-r--r--   0        0        0     3456 2023-05-04 10:09:12.848994 psdm-analysis-0.1.4/psdm_analysis/models/input/container/mixins.py
--rw-r--r--   0        0        0     6312 2023-05-23 11:13:37.870997 psdm-analysis-0.1.4/psdm_analysis/models/input/container/participants_container.py
--rw-r--r--   0        0        0     3134 2023-05-23 11:13:37.871280 psdm-analysis-0.1.4/psdm_analysis/models/input/enums.py
--rw-r--r--   0        0        0     1365 2023-05-23 11:13:37.871527 psdm-analysis-0.1.4/psdm_analysis/models/input/node.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.041104 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/__init__.py
--rw-r--r--   0        0        0     1368 2023-04-19 12:49:15.041213 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/bm.py
--rw-r--r--   0        0        0     3138 2023-04-19 12:49:15.041309 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/charging.py
--rw-r--r--   0        0        0      654 2023-04-19 12:49:15.041628 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/em.py
--rw-r--r--   0        0        0      936 2023-04-19 12:49:15.041802 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/evcs.py
--rw-r--r--   0        0        0      965 2023-04-19 12:49:15.041899 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/evs.py
--rw-r--r--   0        0        0      527 2023-04-19 12:49:15.042031 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/fixed_feed_in.py
--rw-r--r--   0        0        0      813 2023-05-23 11:13:37.872710 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/hp.py
--rw-r--r--   0        0        0      953 2023-04-19 12:49:15.042385 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/load.py
--rw-r--r--   0        0        0     1266 2023-05-23 11:13:37.873708 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/participant.py
--rw-r--r--   0        0        0     1320 2023-04-19 12:49:15.042694 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/pv.py
--rw-r--r--   0        0        0     1527 2023-04-19 12:49:15.042799 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/storage.py
--rw-r--r--   0        0        0     1113 2023-04-19 12:49:15.042895 psdm-analysis-0.1.4/psdm_analysis/models/input/participant/wec.py
--rw-r--r--   0        0        0     4354 2023-05-23 11:13:37.874172 psdm-analysis-0.1.4/psdm_analysis/models/primary_data.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043156 psdm-analysis-0.1.4/psdm_analysis/models/result/__init__.py
--rw-r--r--   0        0        0     2243 2023-04-19 12:49:15.043509 psdm-analysis-0.1.4/psdm_analysis/models/result/flex_option.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043543 psdm-analysis-0.1.4/psdm_analysis/models/result/grid/__init__.py
--rw-r--r--   0        0        0     2842 2023-05-23 11:13:37.874372 psdm-analysis-0.1.4/psdm_analysis/models/result/grid/connector.py
--rw-r--r--   0        0        0     2284 2023-05-26 10:46:52.073721 psdm-analysis-0.1.4/psdm_analysis/models/result/grid/enhanced_node.py
--rw-r--r--   0        0        0     2626 2023-05-26 10:48:25.443146 psdm-analysis-0.1.4/psdm_analysis/models/result/grid/node.py
--rw-r--r--   0        0        0     1701 2023-05-23 11:13:37.875468 psdm-analysis-0.1.4/psdm_analysis/models/result/grid/transformer.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043823 psdm-analysis-0.1.4/psdm_analysis/models/result/participant/__init__.py
--rw-r--r--   0        0        0     6696 2023-05-29 07:46:12.859811 psdm-analysis-0.1.4/psdm_analysis/models/result/participant/dict.py
--rw-r--r--   0        0        0     3170 2023-04-19 12:49:15.044163 psdm-analysis-0.1.4/psdm_analysis/models/result/participant/flex_options.py
--rw-r--r--   0        0        0     3619 2023-05-26 10:49:03.203272 psdm-analysis-0.1.4/psdm_analysis/models/result/participant/participant.py
--rw-r--r--   0        0        0    10556 2023-05-26 09:57:21.675417 psdm-analysis-0.1.4/psdm_analysis/models/result/participant/participants_res_container.py
--rw-r--r--   0        0        0     5842 2023-05-23 11:13:37.877331 psdm-analysis-0.1.4/psdm_analysis/models/result/power.py
--rw-r--r--   0        0        0     4499 2023-05-23 11:13:37.878078 psdm-analysis-0.1.4/psdm_analysis/models/result/res_container.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.044717 psdm-analysis-0.1.4/psdm_analysis/plots/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 11:13:37.878152 psdm-analysis-0.1.4/psdm_analysis/plots/common/__init__.py
--rw-r--r--   0        0        0     2431 2023-05-23 11:13:37.878287 psdm-analysis-0.1.4/psdm_analysis/plots/common/bar_plot.py
--rw-r--r--   0        0        0     1103 2023-05-23 11:13:37.878583 psdm-analysis-0.1.4/psdm_analysis/plots/common/line_plot.py
--rw-r--r--   0        0        0     5500 2023-05-25 08:03:08.060857 psdm-analysis-0.1.4/psdm_analysis/plots/common/utils.py
--rw-r--r--   0        0        0     4128 2023-05-23 11:13:37.879462 psdm-analysis-0.1.4/psdm_analysis/plots/grid.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.044851 psdm-analysis-0.1.4/psdm_analysis/plots/results/__init__.py
--rw-r--r--   0        0        0     6143 2023-05-23 11:13:37.879649 psdm-analysis-0.1.4/psdm_analysis/plots/results/connector_plot.py
--rw-r--r--   0        0        0     3467 2023-05-23 11:13:37.880115 psdm-analysis-0.1.4/psdm_analysis/plots/results/flex_plot.py
--rw-r--r--   0        0        0     1083 2023-04-19 12:49:15.045811 psdm-analysis-0.1.4/psdm_analysis/plots/results/nodes.py
--rw-r--r--   0        0        0    11960 2023-05-23 11:13:37.880667 psdm-analysis-0.1.4/psdm_analysis/plots/results/power_plot.py
--rw-r--r--   0        0        0     7726 2023-05-29 07:50:11.470993 psdm-analysis-0.1.4/psdm_analysis/plots/results/voltage_plot.py
--rw-r--r--   0        0        0        0 2023-04-19 12:49:15.046127 psdm-analysis-0.1.4/psdm_analysis/processing/__init__.py
--rw-r--r--   0        0        0     1217 2023-05-04 10:44:30.440027 psdm-analysis-0.1.4/psdm_analysis/processing/dataframe.py
--rw-r--r--   0        0        0     2174 2023-04-19 12:49:15.046324 psdm-analysis-0.1.4/psdm_analysis/processing/series.py
--rw-r--r--   0        0        0      789 2023-05-29 07:51:17.774103 psdm-analysis-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1799 1970-01-01 00:00:00.000000 psdm-analysis-0.1.4/setup.py
--rw-r--r--   0        0        0     1156 1970-01-01 00:00:00.000000 psdm-analysis-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1581 2023-01-31 09:55:39.404671 psdm-analysis-0.1.5/LICENSE
+-rw-r--r--   0        0        0      373 2023-04-19 12:49:15.037328 psdm-analysis-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038177 psdm-analysis-0.1.5/psdm_analysis/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038287 psdm-analysis-0.1.5/psdm_analysis/analysis/__init__.py
+-rw-r--r--   0        0        0      601 2023-04-19 12:49:15.038571 psdm-analysis-0.1.5/psdm_analysis/analysis/calc.py
+-rw-r--r--   0        0        0     1200 2023-04-19 12:49:15.038918 psdm-analysis-0.1.5/psdm_analysis/analysis/grid.py
+-rw-r--r--   0        0        0        0 2023-05-02 07:38:45.729757 psdm-analysis-0.1.5/psdm_analysis/conversion/__init__.py
+-rw-r--r--   0        0        0     3960 2023-05-02 07:38:45.730387 psdm-analysis-0.1.5/psdm_analysis/conversion/pandapower.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.038964 psdm-analysis-0.1.5/psdm_analysis/io/__init__.py
+-rw-r--r--   0        0        0     2842 2023-04-19 12:49:15.039092 psdm-analysis-0.1.5/psdm_analysis/io/utils.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039122 psdm-analysis-0.1.5/psdm_analysis/models/__init__.py
+-rw-r--r--   0        0        0     9503 2023-05-23 11:13:37.867698 psdm-analysis-0.1.5/psdm_analysis/models/entity.py
+-rw-r--r--   0        0        0     6788 2023-05-30 12:42:51.429533 psdm-analysis-0.1.5/psdm_analysis/models/grid_with_results.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039422 psdm-analysis-0.1.5/psdm_analysis/models/input/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.039466 psdm-analysis-0.1.5/psdm_analysis/models/input/connector/__init__.py
+-rw-r--r--   0        0        0     1329 2023-05-30 12:42:56.398213 psdm-analysis-0.1.5/psdm_analysis/models/input/connector/connector.py
+-rw-r--r--   0        0        0     1888 2023-05-23 11:13:37.869005 psdm-analysis-0.1.5/psdm_analysis/models/input/connector/lines.py
+-rw-r--r--   0        0        0      779 2023-05-30 12:42:56.398558 psdm-analysis-0.1.5/psdm_analysis/models/input/connector/switches.py
+-rw-r--r--   0        0        0     2240 2023-05-29 07:50:38.432624 psdm-analysis-0.1.5/psdm_analysis/models/input/connector/transformer.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.040065 psdm-analysis-0.1.5/psdm_analysis/models/input/container/__init__.py
+-rw-r--r--   0        0        0     6786 2023-05-30 12:42:51.429869 psdm-analysis-0.1.5/psdm_analysis/models/input/container/grid_container.py
+-rw-r--r--   0        0        0     3456 2023-05-04 10:09:12.848994 psdm-analysis-0.1.5/psdm_analysis/models/input/container/mixins.py
+-rw-r--r--   0        0        0     6312 2023-05-23 11:13:37.870997 psdm-analysis-0.1.5/psdm_analysis/models/input/container/participants_container.py
+-rw-r--r--   0        0        0     3134 2023-05-23 11:13:37.871280 psdm-analysis-0.1.5/psdm_analysis/models/input/enums.py
+-rw-r--r--   0        0        0     1365 2023-05-23 11:13:37.871527 psdm-analysis-0.1.5/psdm_analysis/models/input/node.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.041104 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/__init__.py
+-rw-r--r--   0        0        0     1368 2023-04-19 12:49:15.041213 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/bm.py
+-rw-r--r--   0        0        0     3138 2023-04-19 12:49:15.041309 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/charging.py
+-rw-r--r--   0        0        0      654 2023-04-19 12:49:15.041628 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/em.py
+-rw-r--r--   0        0        0      936 2023-04-19 12:49:15.041802 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/evcs.py
+-rw-r--r--   0        0        0      965 2023-04-19 12:49:15.041899 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/evs.py
+-rw-r--r--   0        0        0      527 2023-04-19 12:49:15.042031 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/fixed_feed_in.py
+-rw-r--r--   0        0        0      813 2023-05-23 11:13:37.872710 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/hp.py
+-rw-r--r--   0        0        0      953 2023-04-19 12:49:15.042385 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/load.py
+-rw-r--r--   0        0        0     1266 2023-05-23 11:13:37.873708 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/participant.py
+-rw-r--r--   0        0        0     1320 2023-04-19 12:49:15.042694 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/pv.py
+-rw-r--r--   0        0        0     1527 2023-04-19 12:49:15.042799 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/storage.py
+-rw-r--r--   0        0        0     1113 2023-04-19 12:49:15.042895 psdm-analysis-0.1.5/psdm_analysis/models/input/participant/wec.py
+-rw-r--r--   0        0        0     4354 2023-05-23 11:13:37.874172 psdm-analysis-0.1.5/psdm_analysis/models/primary_data.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043156 psdm-analysis-0.1.5/psdm_analysis/models/result/__init__.py
+-rw-r--r--   0        0        0     2243 2023-04-19 12:49:15.043509 psdm-analysis-0.1.5/psdm_analysis/models/result/flex_option.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043543 psdm-analysis-0.1.5/psdm_analysis/models/result/grid/__init__.py
+-rw-r--r--   0        0        0     2842 2023-05-23 11:13:37.874372 psdm-analysis-0.1.5/psdm_analysis/models/result/grid/connector.py
+-rw-r--r--   0        0        0     2284 2023-05-30 12:42:51.430207 psdm-analysis-0.1.5/psdm_analysis/models/result/grid/enhanced_node.py
+-rw-r--r--   0        0        0     2626 2023-05-30 12:42:51.430763 psdm-analysis-0.1.5/psdm_analysis/models/result/grid/node.py
+-rw-r--r--   0        0        0     1701 2023-05-23 11:13:37.875468 psdm-analysis-0.1.5/psdm_analysis/models/result/grid/transformer.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.043823 psdm-analysis-0.1.5/psdm_analysis/models/result/participant/__init__.py
+-rw-r--r--   0        0        0     6696 2023-05-30 12:42:51.431347 psdm-analysis-0.1.5/psdm_analysis/models/result/participant/dict.py
+-rw-r--r--   0        0        0     3170 2023-04-19 12:49:15.044163 psdm-analysis-0.1.5/psdm_analysis/models/result/participant/flex_options.py
+-rw-r--r--   0        0        0     3619 2023-05-30 12:42:51.431649 psdm-analysis-0.1.5/psdm_analysis/models/result/participant/participant.py
+-rw-r--r--   0        0        0    10556 2023-05-26 09:57:21.675417 psdm-analysis-0.1.5/psdm_analysis/models/result/participant/participants_res_container.py
+-rw-r--r--   0        0        0     5842 2023-05-23 11:13:37.877331 psdm-analysis-0.1.5/psdm_analysis/models/result/power.py
+-rw-r--r--   0        0        0     4499 2023-05-23 11:13:37.878078 psdm-analysis-0.1.5/psdm_analysis/models/result/res_container.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.044717 psdm-analysis-0.1.5/psdm_analysis/plots/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:13:37.878152 psdm-analysis-0.1.5/psdm_analysis/plots/common/__init__.py
+-rw-r--r--   0        0        0     2431 2023-05-23 11:13:37.878287 psdm-analysis-0.1.5/psdm_analysis/plots/common/bar_plot.py
+-rw-r--r--   0        0        0     1103 2023-05-23 11:13:37.878583 psdm-analysis-0.1.5/psdm_analysis/plots/common/line_plot.py
+-rw-r--r--   0        0        0     5500 2023-05-30 12:42:51.432073 psdm-analysis-0.1.5/psdm_analysis/plots/common/utils.py
+-rw-r--r--   0        0        0     4128 2023-05-23 11:13:37.879462 psdm-analysis-0.1.5/psdm_analysis/plots/grid.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.044851 psdm-analysis-0.1.5/psdm_analysis/plots/results/__init__.py
+-rw-r--r--   0        0        0     6143 2023-05-23 11:13:37.879649 psdm-analysis-0.1.5/psdm_analysis/plots/results/connector_plot.py
+-rw-r--r--   0        0        0     3467 2023-05-23 11:13:37.880115 psdm-analysis-0.1.5/psdm_analysis/plots/results/flex_plot.py
+-rw-r--r--   0        0        0     1083 2023-04-19 12:49:15.045811 psdm-analysis-0.1.5/psdm_analysis/plots/results/nodes.py
+-rw-r--r--   0        0        0    11960 2023-05-23 11:13:37.880667 psdm-analysis-0.1.5/psdm_analysis/plots/results/power_plot.py
+-rw-r--r--   0        0        0     7726 2023-05-30 12:42:51.432565 psdm-analysis-0.1.5/psdm_analysis/plots/results/voltage_plot.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:49:15.046127 psdm-analysis-0.1.5/psdm_analysis/processing/__init__.py
+-rw-r--r--   0        0        0     1217 2023-05-04 10:44:30.440027 psdm-analysis-0.1.5/psdm_analysis/processing/dataframe.py
+-rw-r--r--   0        0        0     2174 2023-04-19 12:49:15.046324 psdm-analysis-0.1.5/psdm_analysis/processing/series.py
+-rw-r--r--   0        0        0      789 2023-05-30 13:16:04.964764 psdm-analysis-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1799 1970-01-01 00:00:00.000000 psdm-analysis-0.1.5/setup.py
+-rw-r--r--   0        0        0     1156 1970-01-01 00:00:00.000000 psdm-analysis-0.1.5/PKG-INFO
```

### Comparing `psdm-analysis-0.1.4/LICENSE` & `psdm-analysis-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/analysis/calc.py` & `psdm-analysis-0.1.5/psdm_analysis/analysis/calc.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/analysis/grid.py` & `psdm-analysis-0.1.5/psdm_analysis/analysis/grid.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/conversion/pandapower.py` & `psdm-analysis-0.1.5/psdm_analysis/conversion/pandapower.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/io/utils.py` & `psdm-analysis-0.1.5/psdm_analysis/io/utils.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/entity.py` & `psdm-analysis-0.1.5/psdm_analysis/models/entity.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/grid_with_results.py` & `psdm-analysis-0.1.5/psdm_analysis/models/grid_with_results.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/input/connector/connector.py` & `psdm-analysis-0.1.5/psdm_analysis/models/input/connector/connector.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 from psdm_analysis.models.entity import Entities
 from psdm_analysis.models.input.node import Nodes
 
 
 @dataclass(frozen=True)
 class Connector(Entities, ABC):
+    @staticmethod
+    def attributes() -> list[str]:
+        return Entities.attributes() + ["node_a", "node_b", "parallel_devices"]
+
     @property
     def node_a(self):
         return self.data["node_a"]
 
     @property
     def node_b(self):
         return self.data["node_b"]
```

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/input/connector/lines.py` & `psdm-analysis-0.1.5/psdm_analysis/models/input/connector/lines.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/input/connector/transformer.py` & `psdm-analysis-0.1.5/psdm_analysis/models/input/connector/transformer.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/input/container/grid_container.py` & `psdm-analysis-0.1.5/psdm_analysis/models/input/container/grid_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,16 @@
         )
 
     def get_branches(self) -> list[list[str]]:
         """
         Returns all branches, branching off from the slack node of the grid.
         The branches are returned as a list of lists, where each list contains the node uuids of the branch,
         starting at the slack node.
+
+        Currently only works for single slack node and single voltage level grids.
         """
 
         slack_node = self.nodes.get_slack_nodes()
         if len(slack_node.data) != 1:
             raise ValueError("Currently only implemented for singular slack nodes.")
         transformers = self.transformers_2_w
         slack_transformers = Transformers2W(
@@ -99,18 +101,16 @@
         graph = Graph()
         closed_switches = self.switches.get_closed()
         line_data_dicts = self.lines.data.apply(
             lambda row: {"length": row["length"]}, axis=1
         )
 
         graph.add_nodes_from(self.nodes.uuids)
-        graph.add_edges_from(zip(self.lines.node_a, self.lines.node_b))
-        graph.add_edges_from(
-            zip(closed_switches.node_a, closed_switches.node_b, line_data_dicts)
-        )
+        graph.add_edges_from(zip(self.lines.node_a, self.lines.node_b, line_data_dicts))
+        graph.add_edges_from(zip(closed_switches.node_a, closed_switches.node_b))
         return graph
 
 
 @dataclass(frozen=True)
 class GridContainer(ContainerMixin):
     raw_grid: RawGridContainer
     # todo: we keep the participant containers effectively twice with the mapping
```

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/input/container/mixins.py` & `psdm-analysis-0.1.5/psdm_analysis/models/input/container/mixins.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/input/container/participants_container.py` & `psdm-analysis-0.1.5/psdm_analysis/models/input/container/participants_container.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/input/enums.py` & `psdm-analysis-0.1.5/psdm_analysis/models/input/enums.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/input/node.py` & `psdm-analysis-0.1.5/psdm_analysis/models/input/node.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/input/participant/bm.py` & `psdm-analysis-0.1.5/psdm_analysis/models/input/participant/bm.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/input/participant/charging.py` & `psdm-analysis-0.1.5/psdm_analysis/models/input/participant/charging.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/input/participant/em.py` & `psdm-analysis-0.1.5/psdm_analysis/models/input/participant/em.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/input/participant/evcs.py` & `psdm-analysis-0.1.5/psdm_analysis/models/input/participant/evcs.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/input/participant/evs.py` & `psdm-analysis-0.1.5/psdm_analysis/models/input/participant/evs.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/input/participant/fixed_feed_in.py` & `psdm-analysis-0.1.5/psdm_analysis/models/input/participant/fixed_feed_in.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/input/participant/hp.py` & `psdm-analysis-0.1.5/psdm_analysis/models/input/participant/hp.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/input/participant/load.py` & `psdm-analysis-0.1.5/psdm_analysis/models/input/participant/load.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/input/participant/participant.py` & `psdm-analysis-0.1.5/psdm_analysis/models/input/participant/participant.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/input/participant/pv.py` & `psdm-analysis-0.1.5/psdm_analysis/models/input/participant/pv.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/input/participant/storage.py` & `psdm-analysis-0.1.5/psdm_analysis/models/input/participant/storage.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/input/participant/wec.py` & `psdm-analysis-0.1.5/psdm_analysis/models/input/participant/wec.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/primary_data.py` & `psdm-analysis-0.1.5/psdm_analysis/models/primary_data.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/result/flex_option.py` & `psdm-analysis-0.1.5/psdm_analysis/models/result/flex_option.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/result/grid/connector.py` & `psdm-analysis-0.1.5/psdm_analysis/models/result/grid/connector.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/result/grid/enhanced_node.py` & `psdm-analysis-0.1.5/psdm_analysis/models/result/grid/enhanced_node.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/result/grid/node.py` & `psdm-analysis-0.1.5/psdm_analysis/models/result/grid/node.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/result/grid/transformer.py` & `psdm-analysis-0.1.5/psdm_analysis/models/result/grid/transformer.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/result/participant/dict.py` & `psdm-analysis-0.1.5/psdm_analysis/models/result/participant/dict.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/result/participant/flex_options.py` & `psdm-analysis-0.1.5/psdm_analysis/models/result/participant/flex_options.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/result/participant/participant.py` & `psdm-analysis-0.1.5/psdm_analysis/models/result/participant/participant.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/result/participant/participants_res_container.py` & `psdm-analysis-0.1.5/psdm_analysis/models/result/participant/participants_res_container.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/result/power.py` & `psdm-analysis-0.1.5/psdm_analysis/models/result/power.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/models/result/res_container.py` & `psdm-analysis-0.1.5/psdm_analysis/models/result/res_container.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/plots/common/bar_plot.py` & `psdm-analysis-0.1.5/psdm_analysis/plots/common/bar_plot.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/plots/common/line_plot.py` & `psdm-analysis-0.1.5/psdm_analysis/plots/common/line_plot.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/plots/common/utils.py` & `psdm-analysis-0.1.5/psdm_analysis/plots/common/utils.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/plots/grid.py` & `psdm-analysis-0.1.5/psdm_analysis/plots/grid.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/plots/results/connector_plot.py` & `psdm-analysis-0.1.5/psdm_analysis/plots/results/connector_plot.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/plots/results/flex_plot.py` & `psdm-analysis-0.1.5/psdm_analysis/plots/results/flex_plot.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/plots/results/nodes.py` & `psdm-analysis-0.1.5/psdm_analysis/plots/results/nodes.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/plots/results/power_plot.py` & `psdm-analysis-0.1.5/psdm_analysis/plots/results/power_plot.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/plots/results/voltage_plot.py` & `psdm-analysis-0.1.5/psdm_analysis/plots/results/voltage_plot.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/processing/dataframe.py` & `psdm-analysis-0.1.5/psdm_analysis/processing/dataframe.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/psdm_analysis/processing/series.py` & `psdm-analysis-0.1.5/psdm_analysis/processing/series.py`

 * *Files identical despite different names*

### Comparing `psdm-analysis-0.1.4/pyproject.toml` & `psdm-analysis-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psdm-analysis"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["Thomas Oberliessen <thomas.oberliessen@googlemail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">3.10, <3.12"
 pandas = "2.0.1"
```

### Comparing `psdm-analysis-0.1.4/setup.py` & `psdm-analysis-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
  'requests>=2.27.1,<3.0.0',
  'scipy>=1.10.0,<2.0.0',
  'seaborn>=0.12.1,<0.13.0',
  'shapely>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'psdm-analysis',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': '',
     'long_description': '# psdm-analysis\n\nThe psdm-analysis tool is meant to parse the [Power System Data Model (PSDM)](https://github.com/ie3-institute/PowerSystemDataModel) as well as provide calculation and plotting utilities to analyze the respective data.\n\nIt is currently under development and therefore highly unstable. So if you want to use it, expect it to change quite frequently for now.',
     'author': 'Thomas Oberliessen',
     'author_email': 'thomas.oberliessen@googlemail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `psdm-analysis-0.1.4/PKG-INFO` & `psdm-analysis-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psdm-analysis
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Thomas Oberliessen
 Author-email: thomas.oberliessen@googlemail.com
 Requires-Python: >3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.6.0,<4.0.0)
```

