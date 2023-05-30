# Comparing `tmp/opender-2.0.3.tar.gz` & `tmp/opender-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opender-2.0.3.tar", last modified: Fri Apr 14 18:15:31 2023, max compression
+gzip compressed data, was "opender-2.1.0.tar", last modified: Tue May 30 02:05:09 2023, max compression
```

## Comparing `opender-2.0.3.tar` & `opender-2.1.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.785634 opender-2.0.3/
--rw-rw-rw-   0        0        0     2383 2023-04-14 18:15:23.000000 opender-2.0.3/CHANGELOG.rst
--rw-rw-rw-   0        0        0     1707 2023-03-20 17:14:30.000000 opender-2.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0      288 2022-08-10 15:01:38.000000 opender-2.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6375 2023-04-14 18:15:31.785634 opender-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3063 2023-04-03 14:12:57.000000 opender-2.0.3/README.rst
--rw-rw-rw-   0        0        0       49 2022-08-10 15:01:38.000000 opender-2.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 18:15:31.786634 opender-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0     3432 2023-04-14 18:15:23.000000 opender-2.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.659614 opender-2.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.685610 opender-2.0.3/src/opender/
-drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.709614 opender-2.0.3/src/opender/Parameters/
--rw-rw-rw-   0        0        0     2183 2023-03-20 17:14:30.000000 opender-2.0.3/src/opender/Parameters/AS-with std-values.csv
--rw-rw-rw-   0        0        0      306 2022-08-10 15:01:38.000000 opender-2.0.3/src/opender/Parameters/Model-parameters.csv
--rw-rw-rw-   0        0        0      322 2023-04-14 18:15:23.000000 opender-2.0.3/src/opender/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.736621 opender-2.0.3/src/opender/active_power_support_funcs/
--rw-rw-rw-   0        0        0      780 2023-03-20 17:14:30.000000 opender-2.0.3/src/opender/active_power_support_funcs/__init__.py
--rw-rw-rw-   0        0        0     3415 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/active_power_support_funcs/active_power_limit.py
--rw-rw-rw-   0        0        0     2570 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/active_power_support_funcs/es_perf.py
--rw-rw-rw-   0        0        0     3516 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/active_power_support_funcs/es_perf_bess.py
--rw-rw-rw-   0        0        0     9671 2023-04-14 18:15:23.000000 opender-2.0.3/src/opender/active_power_support_funcs/frequency_droop.py
--rw-rw-rw-   0        0        0     1881 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/active_power_support_funcs/frequency_droop_bess.py
--rw-rw-rw-   0        0        0     7267 2023-04-14 18:15:23.000000 opender-2.0.3/src/opender/active_power_support_funcs/p_funcs.py
--rw-rw-rw-   0        0        0     6864 2023-04-14 18:15:23.000000 opender-2.0.3/src/opender/active_power_support_funcs/p_funcs_bess.py
--rw-rw-rw-   0        0        0     1257 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/active_power_support_funcs/p_funcs_pv.py
--rw-rw-rw-   0        0        0     5099 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/active_power_support_funcs/volt_watt.py
-drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.747624 opender-2.0.3/src/opender/auxiliary_funcs/
--rw-rw-rw-   0        0        0      780 2023-03-20 17:14:30.000000 opender-2.0.3/src/opender/auxiliary_funcs/__init__.py
--rw-rw-rw-   0        0        0     2543 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/auxiliary_funcs/cond_delay.py
--rw-rw-rw-   0        0        0     1851 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/auxiliary_funcs/flipflop.py
--rw-rw-rw-   0        0        0     2234 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/auxiliary_funcs/low_pass_filter.py
--rw-rw-rw-   0        0        0     2338 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/auxiliary_funcs/ramping.py
--rw-rw-rw-   0        0        0     1526 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/auxiliary_funcs/sym_component.py
--rw-rw-rw-   0        0        0     2996 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/auxiliary_funcs/time_delay.py
-drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.749624 opender-2.0.3/src/opender/bess_specifc/
--rw-rw-rw-   0        0        0      780 2023-03-20 17:14:30.000000 opender-2.0.3/src/opender/bess_specifc/__init__.py
--rw-rw-rw-   0        0        0     6806 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/bess_specifc/soc.py
--rw-rw-rw-   0        0        0    16960 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/capability_and_priority.py
-drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.760627 opender-2.0.3/src/opender/common_file_format/
--rw-rw-rw-   0        0        0      113 2022-08-26 15:18:01.000000 opender-2.0.3/src/opender/common_file_format/__init__.py
--rw-rw-rw-   0        0        0    92676 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/common_file_format/common_file_format.py
--rw-rw-rw-   0        0        0    10018 2023-04-14 18:15:23.000000 opender-2.0.3/src/opender/common_file_format/common_file_format_BESS.py
--rw-rw-rw-   0        0        0    11644 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/der.py
--rw-rw-rw-   0        0        0     2930 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/der_bess.py
--rw-rw-rw-   0        0        0     1302 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/der_pv.py
--rw-rw-rw-   0        0        0    11392 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/op_cond_proc.py
-drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.766627 opender-2.0.3/src/opender/operation_status/
--rw-rw-rw-   0        0        0      910 2023-03-20 17:14:30.000000 opender-2.0.3/src/opender/operation_status/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.770628 opender-2.0.3/src/opender/operation_status/enter_service_crit/
--rw-rw-rw-   0        0        0       85 2023-03-20 17:14:30.000000 opender-2.0.3/src/opender/operation_status/enter_service_crit/__init__.py
--rw-rw-rw-   0        0        0     6206 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/operation_status/enter_service_crit/es_crit.py
--rw-rw-rw-   0        0        0     1729 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/operation_status/enter_service_crit/es_crit_pv.py
--rw-rw-rw-   0        0        0     5618 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/operation_status/operating_status.py
--rw-rw-rw-   0        0        0     1519 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/operation_status/operating_status_pv.py
--rw-rw-rw-   0        0        0    11520 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/operation_status/rt_crit.py
-drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.775629 opender-2.0.3/src/opender/operation_status/trip_crit/
--rw-rw-rw-   0        0        0       73 2023-03-20 17:14:30.000000 opender-2.0.3/src/opender/operation_status/trip_crit/__init__.py
--rw-rw-rw-   0        0        0     7896 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/operation_status/trip_crit/trip_crit.py
--rw-rw-rw-   0        0        0     1613 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/operation_status/trip_crit/trip_crit_pv.py
--rw-rw-rw-   0        0        0     9166 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/output_options.py
-drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.783632 opender-2.0.3/src/opender/reactive_power_support_funcs/
--rw-rw-rw-   0        0        0        0 2022-08-10 15:01:38.000000 opender-2.0.3/src/opender/reactive_power_support_funcs/__init__.py
--rw-rw-rw-   0        0        0     3920 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/reactive_power_support_funcs/constant_pf.py
--rw-rw-rw-   0        0        0     2455 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/reactive_power_support_funcs/constant_vars.py
--rw-rw-rw-   0        0        0     9342 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/reactive_power_support_funcs/q_funcs.py
--rw-rw-rw-   0        0        0     6858 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/reactive_power_support_funcs/volt_var.py
--rw-rw-rw-   0        0        0     7676 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/reactive_power_support_funcs/watt_var.py
--rw-rw-rw-   0        0        0    15680 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/rt_perf.py
--rw-rw-rw-   0        0        0    10266 2023-04-03 14:12:57.000000 opender-2.0.3/src/opender/setting_execution_delay.py
-drwxrwxrwx   0        0        0        0 2023-04-14 18:15:31.706614 opender-2.0.3/src/opender.egg-info/
--rw-rw-rw-   0        0        0     6375 2023-04-14 18:15:31.000000 opender-2.0.3/src/opender.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2532 2023-04-14 18:15:31.000000 opender-2.0.3/src/opender.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 18:15:31.000000 opender-2.0.3/src/opender.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-14 18:15:31.000000 opender-2.0.3/src/opender.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       49 2023-04-14 18:15:31.000000 opender-2.0.3/src/opender.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-14 18:15:31.000000 opender-2.0.3/src/opender.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 02:05:09.257442 opender-2.1.0/
+-rw-rw-rw-   0        0        0     2687 2023-05-30 02:04:46.000000 opender-2.1.0/CHANGELOG.rst
+-rw-rw-rw-   0        0        0     1707 2023-03-20 17:14:30.000000 opender-2.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      288 2022-08-10 15:01:38.000000 opender-2.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6679 2023-05-30 02:05:09.256442 opender-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3063 2023-04-03 14:12:57.000000 opender-2.1.0/README.rst
+-rw-rw-rw-   0        0        0       49 2022-08-10 15:01:38.000000 opender-2.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 02:05:09.257442 opender-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     3432 2023-05-30 02:04:46.000000 opender-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 02:05:08.937963 opender-2.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-30 02:05:09.018066 opender-2.1.0/src/opender/
+drwxrwxrwx   0        0        0        0 2023-05-30 02:05:09.063950 opender-2.1.0/src/opender/Parameters/
+-rw-rw-rw-   0        0        0     2183 2023-03-20 17:14:30.000000 opender-2.1.0/src/opender/Parameters/AS-with std-values.csv
+-rw-rw-rw-   0        0        0      306 2022-08-10 15:01:38.000000 opender-2.1.0/src/opender/Parameters/Model-parameters.csv
+-rw-rw-rw-   0        0        0      322 2023-05-30 02:04:46.000000 opender-2.1.0/src/opender/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 02:05:09.097132 opender-2.1.0/src/opender/active_power_support_funcs/
+-rw-rw-rw-   0        0        0      780 2023-03-20 17:14:30.000000 opender-2.1.0/src/opender/active_power_support_funcs/__init__.py
+-rw-rw-rw-   0        0        0     3635 2023-05-30 02:04:46.000000 opender-2.1.0/src/opender/active_power_support_funcs/active_power_limit.py
+-rw-rw-rw-   0        0        0     2316 2023-05-30 02:04:46.000000 opender-2.1.0/src/opender/active_power_support_funcs/es_perf.py
+-rw-rw-rw-   0        0        0     9969 2023-05-30 02:04:46.000000 opender-2.1.0/src/opender/active_power_support_funcs/frequency_droop.py
+-rw-rw-rw-   0        0        0     1881 2023-04-03 14:12:57.000000 opender-2.1.0/src/opender/active_power_support_funcs/frequency_droop_bess.py
+-rw-rw-rw-   0        0        0     7473 2023-05-30 02:04:46.000000 opender-2.1.0/src/opender/active_power_support_funcs/p_funcs.py
+-rw-rw-rw-   0        0        0     5301 2023-05-30 02:04:46.000000 opender-2.1.0/src/opender/active_power_support_funcs/p_funcs_bess.py
+-rw-rw-rw-   0        0        0     1257 2023-04-03 14:12:57.000000 opender-2.1.0/src/opender/active_power_support_funcs/p_funcs_pv.py
+-rw-rw-rw-   0        0        0     5283 2023-05-30 02:04:46.000000 opender-2.1.0/src/opender/active_power_support_funcs/volt_watt.py
+drwxrwxrwx   0        0        0        0 2023-05-30 02:05:09.145965 opender-2.1.0/src/opender/auxiliary_funcs/
+-rw-rw-rw-   0        0        0      780 2023-03-20 17:14:30.000000 opender-2.1.0/src/opender/auxiliary_funcs/__init__.py
+-rw-rw-rw-   0        0        0     2543 2023-04-03 14:12:57.000000 opender-2.1.0/src/opender/auxiliary_funcs/cond_delay.py
+-rw-rw-rw-   0        0        0     1851 2023-04-03 14:12:57.000000 opender-2.1.0/src/opender/auxiliary_funcs/flipflop.py
+-rw-rw-rw-   0        0        0     2234 2023-04-03 14:12:57.000000 opender-2.1.0/src/opender/auxiliary_funcs/low_pass_filter.py
+-rw-rw-rw-   0        0        0     2338 2023-04-03 14:12:57.000000 opender-2.1.0/src/opender/auxiliary_funcs/ramping.py
+-rw-rw-rw-   0        0        0     1526 2023-04-03 14:12:57.000000 opender-2.1.0/src/opender/auxiliary_funcs/sym_component.py
+-rw-rw-rw-   0        0        0     2996 2023-04-03 14:12:57.000000 opender-2.1.0/src/opender/auxiliary_funcs/time_delay.py
+drwxrwxrwx   0        0        0        0 2023-05-30 02:05:09.151044 opender-2.1.0/src/opender/bess_specifc/
+-rw-rw-rw-   0        0        0      780 2023-03-20 17:14:30.000000 opender-2.1.0/src/opender/bess_specifc/__init__.py
+-rw-rw-rw-   0        0        0     2377 2023-05-30 02:04:46.000000 opender-2.1.0/src/opender/bess_specifc/bess_specific.py
+-rw-rw-rw-   0        0        0     6806 2023-05-30 02:04:46.000000 opender-2.1.0/src/opender/bess_specifc/soc.py
+-rw-rw-rw-   0        0        0    16960 2023-04-03 14:12:57.000000 opender-2.1.0/src/opender/capability_and_priority.py
+drwxrwxrwx   0        0        0        0 2023-05-30 02:05:09.173250 opender-2.1.0/src/opender/common_file_format/
+-rw-rw-rw-   0        0        0      113 2022-08-26 15:18:01.000000 opender-2.1.0/src/opender/common_file_format/__init__.py
+-rw-rw-rw-   0        0        0    92676 2023-04-03 14:12:57.000000 opender-2.1.0/src/opender/common_file_format/common_file_format.py
+-rw-rw-rw-   0        0        0    10653 2023-05-30 02:04:46.000000 opender-2.1.0/src/opender/common_file_format/common_file_format_BESS.py
+-rw-rw-rw-   0        0        0    11627 2023-05-30 02:04:46.000000 opender-2.1.0/src/opender/der.py
+-rw-rw-rw-   0        0        0     3033 2023-05-30 02:04:46.000000 opender-2.1.0/src/opender/der_bess.py
+-rw-rw-rw-   0        0        0     1302 2023-04-03 14:12:57.000000 opender-2.1.0/src/opender/der_pv.py
+-rw-rw-rw-   0        0        0    11392 2023-04-03 14:12:57.000000 opender-2.1.0/src/opender/op_cond_proc.py
+drwxrwxrwx   0        0        0        0 2023-05-30 02:05:09.198869 opender-2.1.0/src/opender/operation_status/
+-rw-rw-rw-   0        0        0      910 2023-03-20 17:14:30.000000 opender-2.1.0/src/opender/operation_status/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 02:05:09.223130 opender-2.1.0/src/opender/operation_status/enter_service_crit/
+-rw-rw-rw-   0        0        0       85 2023-03-20 17:14:30.000000 opender-2.1.0/src/opender/operation_status/enter_service_crit/__init__.py
+-rw-rw-rw-   0        0        0     6206 2023-04-03 14:12:57.000000 opender-2.1.0/src/opender/operation_status/enter_service_crit/es_crit.py
+-rw-rw-rw-   0        0        0     1729 2023-04-03 14:12:57.000000 opender-2.1.0/src/opender/operation_status/enter_service_crit/es_crit_pv.py
+-rw-rw-rw-   0        0        0     5389 2023-05-30 02:04:46.000000 opender-2.1.0/src/opender/operation_status/operating_status.py
+-rw-rw-rw-   0        0        0     1519 2023-04-03 14:12:57.000000 opender-2.1.0/src/opender/operation_status/operating_status_pv.py
+-rw-rw-rw-   0        0        0    11520 2023-04-03 14:12:57.000000 opender-2.1.0/src/opender/operation_status/rt_crit.py
+drwxrwxrwx   0        0        0        0 2023-05-30 02:05:09.246088 opender-2.1.0/src/opender/operation_status/trip_crit/
+-rw-rw-rw-   0        0        0       73 2023-03-20 17:14:30.000000 opender-2.1.0/src/opender/operation_status/trip_crit/__init__.py
+-rw-rw-rw-   0        0        0     7896 2023-04-03 14:12:57.000000 opender-2.1.0/src/opender/operation_status/trip_crit/trip_crit.py
+-rw-rw-rw-   0        0        0     1613 2023-04-03 14:12:57.000000 opender-2.1.0/src/opender/operation_status/trip_crit/trip_crit_pv.py
+-rw-rw-rw-   0        0        0     9166 2023-04-03 14:12:57.000000 opender-2.1.0/src/opender/output_options.py
+drwxrwxrwx   0        0        0        0 2023-05-30 02:05:09.254442 opender-2.1.0/src/opender/reactive_power_support_funcs/
+-rw-rw-rw-   0        0        0        0 2022-08-10 15:01:38.000000 opender-2.1.0/src/opender/reactive_power_support_funcs/__init__.py
+-rw-rw-rw-   0        0        0     4153 2023-05-30 02:04:46.000000 opender-2.1.0/src/opender/reactive_power_support_funcs/constant_pf.py
+-rw-rw-rw-   0        0        0     2925 2023-05-30 02:04:46.000000 opender-2.1.0/src/opender/reactive_power_support_funcs/constant_vars.py
+-rw-rw-rw-   0        0        0     9601 2023-05-30 02:04:46.000000 opender-2.1.0/src/opender/reactive_power_support_funcs/q_funcs.py
+-rw-rw-rw-   0        0        0     7165 2023-05-30 02:04:46.000000 opender-2.1.0/src/opender/reactive_power_support_funcs/volt_var.py
+-rw-rw-rw-   0        0        0     7900 2023-05-30 02:04:46.000000 opender-2.1.0/src/opender/reactive_power_support_funcs/watt_var.py
+-rw-rw-rw-   0        0        0    15680 2023-04-03 14:12:57.000000 opender-2.1.0/src/opender/rt_perf.py
+-rw-rw-rw-   0        0        0    10266 2023-04-03 14:12:57.000000 opender-2.1.0/src/opender/setting_execution_delay.py
+drwxrwxrwx   0        0        0        0 2023-05-30 02:05:09.048859 opender-2.1.0/src/opender.egg-info/
+-rw-rw-rw-   0        0        0     6679 2023-05-30 02:05:08.000000 opender-2.1.0/src/opender.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2519 2023-05-30 02:05:08.000000 opender-2.1.0/src/opender.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 02:05:08.000000 opender-2.1.0/src/opender.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-30 02:05:08.000000 opender-2.1.0/src/opender.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       49 2023-05-30 02:05:08.000000 opender-2.1.0/src/opender.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-30 02:05:08.000000 opender-2.1.0/src/opender.egg-info/top_level.txt
```

### Comparing `opender-2.0.3/CHANGELOG.rst` & `opender-2.1.0/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 
 Changelog
 =========
+2.1.0 (2023-05-29)
+------------------
+* Updated interaction between enter service ramp and ride-through. Now DER returns to enter service ramp
+  after ride-through
+* Added an optional charge/discharge ramp rate limit for BESS DER
+* Added resets for all grid-support functions when DER is tripped
+
 2.0.3 (2023-04-14)
 ------------------
 * Fixed the option to update BESS DER parameter when creating the object.
 * Fixed a bug when initializing a BESS DER during abnormal frequency condition.
 
 2.0.2 (2023-04-03)
 ------------------
```

### Comparing `opender-2.0.3/LICENSE.txt` & `opender-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/PKG-INFO` & `opender-2.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opender
-Version: 2.0.3
+Version: 2.1.0
 Summary: Open-source Distributed Energy Resources (DER) Model that represents IEEE Standard 1547-2018 requirements for steady-state and dynamic analyses
 Home-page: https://github.com/epri-dev/opender
 Author: Yiwei Ma, Wei Ren, Paulo Radatz, Jithendar Anandan
 Author-email: yma@epri.com, wren@epri.com, pradatz@epri.com
 License: BSD
 Project-URL: Homepage, https://www.epri.com/OpenDER
 Project-URL: Model Specification, https://www.epri.com/research/products/000000003002021694
@@ -95,14 +95,21 @@
 Execution command: pytest path-to-package\\tests
 
 
 
 
 Changelog
 =========
+2.1.0 (2023-05-29)
+------------------
+* Updated interaction between enter service ramp and ride-through. Now DER returns to enter service ramp
+  after ride-through
+* Added an optional charge/discharge ramp rate limit for BESS DER
+* Added resets for all grid-support functions when DER is tripped
+
 2.0.3 (2023-04-14)
 ------------------
 * Fixed the option to update BESS DER parameter when creating the object.
 * Fixed a bug when initializing a BESS DER during abnormal frequency condition.
 
 2.0.2 (2023-04-03)
 ------------------
```

### Comparing `opender-2.0.3/README.rst` & `opender-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/setup.py` & `opender-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         encoding=kwargs.get('encoding', 'utf8')
     ) as fh:
         return fh.read()
 
 
 setup(
     name='opender',
-    version='2.0.3',
+    version='2.1.0',
     license='BSD',
     description='Open-source Distributed Energy Resources (DER) Model that represents IEEE Standard 1547-2018 '
                 'requirements for steady-state and dynamic analyses',
     long_description='%s\n%s' % (
         re.compile('^.. start-badges.*^.. end-badges', re.M | re.S).sub('', read('README.rst')),
         re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst'))
     ),
```

### Comparing `opender-2.0.3/src/opender/Parameters/AS-with std-values.csv` & `opender-2.1.0/src/opender/Parameters/AS-with std-values.csv`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender/active_power_support_funcs/__init__.py` & `opender-2.1.0/src/opender/active_power_support_funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender/active_power_support_funcs/active_power_limit.py` & `opender-2.1.0/src/opender/active_power_support_funcs/active_power_limit.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,24 +43,29 @@
         :param AP_RT:	Active power limit response time
         :param NP_REACT_TIME:   DER grid support function reaction time
 
         Output:
         :param ap_limit_rt:	Active power limit
         """
 
-        # Eq. 3.7.1-5, AP_LIMIT is based on NP_P_MAX if positive, and NP_P_MAX_CHARGE if negative. This is to
+        # Eq. 3.7.1-6, AP_LIMIT is based on NP_P_MAX if positive, and NP_P_MAX_CHARGE if negative. This is to
         # convert to a per-unit value based on NP_P_MAX.
         self.ap_limit_pu = self.exec_delay.ap_limit_exec if self.exec_delay.ap_limit_exec > 0 else \
                            self.exec_delay.ap_limit_exec * self.der_file.NP_P_MAX_CHARGE / self.der_file.NP_P_MAX
 
-        # Eq. 3.7.1-6, The final power limitation is subjected to the response time. In this model a ramp rate limit
+        # Eq. 3.7.1-7, The final power limitation is subjected to the response time. In this model a ramp rate limit
         # followed by a time delay (to model reaction time) is applied. Note that there can be multiple different ways
         # to implement this behavior in an actual DER.
         if self.exec_delay.ap_limit_enable_exec:
             self.ap_limit_ramp = self.ap_limit_ramping.ramp(self.ap_limit_pu, self.der_file.AP_RT - self.der_file.NP_REACT_TIME, self.der_file.AP_RT - self.der_file.NP_REACT_TIME)
+            self.ap_limit_rt = self.ap_limit_delay.tdelay(self.ap_limit_ramp, self.der_file.NP_REACT_TIME)
         else:
             # If active power limit function is not enabled, the "limited active power" value is set to 1
-            self.ap_limit_ramp = self.ap_limit_ramping.ramp(1, 0, 0)
-        # Apply reaction time
-        self.ap_limit_rt = self.ap_limit_delay.tdelay(self.ap_limit_ramp, self.der_file.NP_REACT_TIME)
+            self.reset()
 
         return self.ap_limit_rt
+
+    def reset(self):
+        # Eq. 3.7.1-8, resetting active power limit output and state variables to 1pu when DER is tripped or function
+        # is disabled
+        self.ap_limit_ramp = self.ap_limit_ramping.ramp(1, 0, 0)
+        self.ap_limit_rt = self.ap_limit_delay.tdelay(1, 0)
```

### Comparing `opender-2.0.3/src/opender/active_power_support_funcs/es_perf.py` & `opender-2.1.0/src/opender/active_power_support_funcs/es_perf.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,20 +37,19 @@
         :param der_status:	Status of DER (Trip, Entering Service, etc)
         :param es_ramp_rate_exec:	Enter service soft-start duration (ES_RAMP_RATE) signal after execution delay
 
         Output:
         :param p_es_pu:	DER enter service ramp reference
         """
 
-        if self.der_obj.der_status == "Entering Service":
-            # Eq 3.7.1-7, if DER is entering service, enter service ramp reference linearly ramp to a value slightly
+        if self.der_obj.der_status == "Trip":
+            self.reset()
+        else:
+            # Eq 3.7.1-10, if DER is entering service, enter service ramp reference linearly ramp to a value slightly
             # greater than 1. The purpose is to identify if enter service process is completed
             self.p_es_pu = self.rrl.ramp(1.1, self.exec_delay.es_ramp_rate_exec, 0)
-        elif self.der_obj.der_status == "Trip":
-            # Eq 3.7.1-8, if DER is tripped, the reference should be reset to 0
-            self.p_es_pu = self.rrl.ramp(0, 0, 0)
-        else:
-            # Eq 3.7.1-9, if DER is not tripped and enter service process is completed, the reference is set to high,
-            # so that it will not impact output active power
-            self.p_es_pu = self.rrl.ramp(1.1, 0, 0)
 
         return self.p_es_pu
+
+    def reset(self):
+        # Eq 3.7.1-9, if DER is tripped, the reference should be reset to 0
+        self.p_es_pu = self.rrl.ramp(0, 0, 0)
```

### Comparing `opender-2.0.3/src/opender/active_power_support_funcs/frequency_droop.py` & `opender-2.1.0/src/opender/active_power_support_funcs/frequency_droop.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
         Output:
         :param p_pf_pu:     Output active power from frequency-droop function
         :param pf_uf_active:    Frequency-droop under-frequency active
         :param pf_of_active:    Frequency-droop over-frequency active
         """
 
-        # Eq. 3.7.1-10, detect if in under-frequency or over-frequency condition
+        # Eq. 3.7.1-11, detect if in under-frequency or over-frequency condition
         if(self.der_input.freq_hz < (60 - self.exec_delay.pf_dbuf_exec)) and self.der_file.PF_MODE_ENABLE:
             self.pf_uf = 1
         else:
             self.pf_uf = 0
             
         if(self.der_input.freq_hz > (60 + self.exec_delay.pf_dbof_exec)) and self.der_file.PF_MODE_ENABLE:
             self.pf_of = 1
@@ -109,67 +109,75 @@
         else:
             self.p_out_w_prev = p_out_w
 
         # Initialize internal state variables of pre-disturbance active power output
         if self.p_pf_pre_pu_prev is None:
             self.p_pf_pre_pu_prev = min(self.get_p_pu(), ap_limit_rt, p_pv_limit_pu)
 
-        # Eq. 3.7.1-11, calculate pre-disturbance active power output
+        # Eq. 3.7.1-12, calculate pre-disturbance active power output
         if self.pf_uf == 1 and self.pf_uf_prev == 1:
             self.p_pf_pre_pu = self.p_pf_pre_pu_prev
         elif self.pf_of == 1 and self.pf_of_prev == 1:
             self.p_pf_pre_pu = self.p_pf_pre_pu_prev
         else:
             self.p_pf_pre_pu = self.p_out_w_prev / self.der_file.NP_P_MAX
 
-        # Eq. 3.7.1-12, calculate active power reference according to frequency-droop - overfrequency
+        # Eq. 3.7.1-13, calculate active power reference according to frequency-droop - overfrequency
         self.p_pf_of_pu = max(self.p_pf_pre_pu - 
                               ((self.der_input.freq_hz - (60 + self.exec_delay.pf_dbof_exec)) 
                                / (60 * self.exec_delay.pf_kof_exec)),
                               self.der_file.NP_P_MIN_PU)
 
-        # Eq. 3.7.1-13, calculate active power reference according to frequency-droop - underfrequency
+        # Eq. 3.7.1-14, calculate active power reference according to frequency-droop - underfrequency
         self.p_pf_uf_pu = min(self.p_pf_pre_pu + 
                               (((60 - self.exec_delay.pf_dbof_exec) - self.der_input.freq_hz) 
                                / ((60 * self.exec_delay.pf_kuf_exec)))
                               , self.der_input.p_avl_pu)
 
-        # Eq. 3.7.1-15, calculate active power reference according to frequency-droop
+        # Eq. 3.7.1-15,16, calculate active power reference according to frequency-droop
         if self.pf_of == 1:
             self.p_pf_ref_pu = self.p_pf_of_pu
         elif self.pf_uf == 1:
             self.p_pf_ref_pu = self.p_pf_uf_pu
         else:
             self.p_pf_ref_pu = min(self.p_pf_normal_pu(), ap_limit_rt, p_pv_limit_pu)
 
-        # Eq. 3.7.1-16, apply the low pass filter
+        # Eq. 3.7.1-17, apply the low pass filter
         self.pf_olrt_appl = self.exec_delay.pf_olrt_exec if self.pf_uf or self.pf_of or self.pf_uf_active or self.pf_of_active else 0
         self.p_pf_lpf_pu = self.pf_lpf.low_pass_filter(self.p_pf_ref_pu, self.pf_olrt_appl - self.der_file.NP_REACT_TIME)
         self.p_pf_pu = self.pf_delay.tdelay(self.p_pf_lpf_pu, self.der_file.NP_REACT_TIME)
 
-        # Eq. 3.7.1-17, decide if frequency droop function is active
+        # Eq. 3.7.1-18, decide if frequency droop function is active
         self.pf_uf_active = self.pf_uf_active_ff.flipflop(self.pf_uf and self.der_file.PF_MODE_ENABLE,
                                                           (not (self.pf_uf and self.der_file.PF_MODE_ENABLE))
                                                           and abs(self.p_pf_pu-self.p_pf_ref_pu)<1.e-3)
 
         self.pf_of_active = self.pf_of_active_ff.flipflop(self.pf_of and self.der_file.PF_MODE_ENABLE,
                                                           (not (self.pf_of and self.der_file.PF_MODE_ENABLE))
                                                           and abs(self.p_pf_pu-self.p_pf_ref_pu)<1.e-3)
 
         # Save the values for calculations in next time step
         self.pf_uf_prev = self.pf_uf
         self.pf_of_prev = self.pf_of
         self.p_pf_pre_pu_prev = self.p_pf_pre_pu
 
+        if self.der_file.PF_MODE_ENABLE == False:
+            self.reset()
+
         return self.p_pf_pu, self.pf_uf_active, self.pf_of_active
 
     def p_pf_normal_pu(self):
         # Eq. 3.7.1-14, if DER is entering service, the pre-disturbance power is obtained from the DER output power
         # in the previous simulation time step.
         if self.der_obj.der_status == 'Entering Service':
             return self.der_obj.p_out_w/self.der_file.NP_P_MAX
         else:
             return self.der_input.p_avl_pu
 
     def get_p_pu(self):
         # For initialization of p_pf_pre_pu_prev and p_out_w_prev
-        return self.der_input.p_avl_pu
+        return self.der_input.p_avl_pu
+
+    def reset(self):
+        # Eq. 3.7.1-19, if DER is tripped, the reference should be reset to 0
+        self.p_pf_pu = self.pf_delay.tdelay(0, 0)
+        self.p_pf_lpf_pu = self.pf_lpf.low_pass_filter(0, 0)
```

### Comparing `opender-2.0.3/src/opender/active_power_support_funcs/frequency_droop_bess.py` & `opender-2.1.0/src/opender/active_power_support_funcs/frequency_droop_bess.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender/active_power_support_funcs/p_funcs.py` & `opender-2.1.0/src/opender/active_power_support_funcs/p_funcs.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,18 @@
         # Intermediate variables
         self.pf_uf_active = None        # Frequency-droop under-frequency condition active
         self.pf_of_active = None        # Frequency-droop over-frequency condition active
         self.p_pf_pu = None             # Active power from frequency droop function
         self.ap_limit_rt = None         # Active power limit from active power limit function
         self.p_pv_limit_pu = None       # Active power limit from volt-watt function
         self.p_es_pu = None             # Active power reference from enter service ramp requirements
-        self.es_completed = False       # Flag to indicate enter service has completed
+        if self.der_file.STATUS_INIT:
+            self.es_completed = True    # Flag to indicate enter service has completed
+        else:
+            self.es_completed = False
         self.p_desired_pu = None        # Desired active power from all active power support functions
 
         self.aplimit = active_power_limit.ActivePowerLimit(self.der_file, self.exec_delay)
         self.voltwatt = volt_watt.VoltWatt(self.der_file, self.exec_delay, self.der_input)
         self.freqdroop = frequency_droop.FreqDroop(self.der_obj)
         self.enterserviceperf = es_perf.EnterServicePerformance(der_obj)
 
@@ -47,29 +50,46 @@
         """
         Call active power support functions and based on the results, generate desired active power output
 
         Output:
         :param p_desired_pu:	Desired output active power from active power support functions in per unit
         """
 
-        # Active power limit function
-        self.ap_limit_rt = self.aplimit.calculate_ap_limit_rt()
+        if self.der_obj.der_status != 'Trip':
+
+            # Active power limit function
+            self.ap_limit_rt = self.aplimit.calculate_ap_limit_rt()
 
-        # Volt-watt function
-        self.p_pv_limit_pu = self.voltwatt.calculate_p_pv_limit_pu()
+            # Volt-watt function
+            self.p_pv_limit_pu = self.voltwatt.calculate_p_pv_limit_pu()
 
-        # Frequency-droop function
-        self.p_pf_pu, self.pf_uf_active, self.pf_of_active = self.freqdroop.calculate_p_pf_pu(p_out_w,
-                                                                                              self.ap_limit_rt,
-                                                                                              self.p_pv_limit_pu)
-        # Enter service ramp performance
-        self.p_es_pu = self.enterserviceperf.es_performance()
+            # Frequency-droop function
+            self.p_pf_pu, self.pf_uf_active, self.pf_of_active = self.freqdroop.calculate_p_pf_pu(p_out_w,
+                                                                                                  self.ap_limit_rt,
+                                                                                                  self.p_pv_limit_pu)
+            # Enter service ramp performance
+            self.p_es_pu = self.enterserviceperf.es_performance()
 
-        # Calculate final desired active power based on other functions
-        self.p_desired_pu = self.calculate_p_desired_pu(p_out_w)
+            # Calculate final desired active power based on other functions
+            self.p_desired_pu = self.calculate_p_desired_pu(p_out_w)
+
+            # Eq 3.7.1-19, if the enter service ramp reference is greater than 1,
+            # it is considered that the DER enter service is completed.
+            if self.p_es_pu > 1:
+                self.es_completed = True
+
+        else:
+            # Eq 3.7.1-20, if DER is not in service, the desired active power should be 0, and it is not considered
+            # that enter service is completed
+            self.p_desired_pu = 0
+            self.es_completed = False
+            self.freqdroop.reset()
+            self.voltwatt.reset()
+            self.enterserviceperf.reset()
+            self.aplimit.reset()
 
         return self.p_desired_pu
 
     def calculate_p_desired_pu(self, p_out_w):
         """
         Based on the calculated values from volt-watt, frequency-droop, active power limit, and enter service ramp,
         their enabling signal, and DER operating status, generate the DER desired active power output
@@ -78,54 +98,44 @@
         Variable used in this function:
         :param ap_limit_enable_exec:	Active power limit enable (AP_LIMIT_ENABLE) signal after execution delay
         :param pv_mode_enable_exec:	    Volt-watt enable (PV_MODE_ENABLE) signal after execution delay
         :param der_status:	Status of DER (Trip, Entering Service, etc)
         :param p_avl_pu:    DER available active power in per unit considering efficiency
         """
 
-        if self.der_obj.der_status != 'Trip':
-
-            # Eq 3.7.1-18, calculate desired active power in per unit based on the enabling signals from the
-            # grid-support functions
-            if self.exec_delay.ap_limit_enable_exec == False and self.exec_delay.pv_mode_enable_exec == False \
-                    and self.pf_uf_active == False and self.pf_of_active == False:
-                self.p_desired_pu = min(self.der_input.p_avl_pu, self.p_es_pu, 1)
+        # Eq 3.7.1-18, calculate desired active power in per unit based on the enabling signals from the
+        # grid-support functions
+        if self.exec_delay.ap_limit_enable_exec == False and self.exec_delay.pv_mode_enable_exec == False \
+                and self.pf_uf_active == False and self.pf_of_active == False:
+            self.p_desired_pu = min(self.der_input.p_avl_pu, self.p_es_pu, 1)
+
+        if self.exec_delay.ap_limit_enable_exec == True and self.exec_delay.pv_mode_enable_exec == False \
+                and self.pf_uf_active == False and self.pf_of_active == False:
+            self.p_desired_pu = min(self.der_input.p_avl_pu, self.p_es_pu, self.ap_limit_rt, 1)
+
+        if self.exec_delay.ap_limit_enable_exec == False and self.exec_delay.pv_mode_enable_exec == True \
+                and self.pf_uf_active == False and self.pf_of_active == False:
+            self.p_desired_pu = min(self.der_input.p_avl_pu, self.p_es_pu, self.p_pv_limit_pu, 1)
+
+        if (self.exec_delay.ap_limit_enable_exec == True and self.exec_delay.pv_mode_enable_exec == True
+                and self.pf_uf_active == False and self.pf_of_active == False):
+            self.p_desired_pu = min(self.der_input.p_avl_pu, self.ap_limit_rt, self.p_pv_limit_pu, 1)
+
+        if self.exec_delay.pv_mode_enable_exec == False and self.pf_of_active == True:
+            self.p_desired_pu = min(self.der_input.p_avl_pu, self.p_pf_pu, 1)
 
-            if self.exec_delay.ap_limit_enable_exec == True and self.exec_delay.pv_mode_enable_exec == False \
-                    and self.pf_uf_active == False and self.pf_of_active == False:
-                self.p_desired_pu = min(self.der_input.p_avl_pu, self.p_es_pu, self.ap_limit_rt, 1)
+        if self.exec_delay.pv_mode_enable_exec == True and self.pf_of_active == True:
+            self.p_desired_pu = min(self.der_input.p_avl_pu, self.p_pv_limit_pu, self.p_pf_pu, 1)
 
-            if self.exec_delay.ap_limit_enable_exec == False and self.exec_delay.pv_mode_enable_exec == True \
-                    and self.pf_uf_active == False and self.pf_of_active == False:
-                self.p_desired_pu = min(self.der_input.p_avl_pu, self.p_es_pu, self.p_pv_limit_pu, 1)
-
-            if (self.exec_delay.ap_limit_enable_exec == True and self.exec_delay.pv_mode_enable_exec == True
-                    and self.pf_uf_active == False and self.pf_of_active == False):
-                self.p_desired_pu = min(self.der_input.p_avl_pu, self.ap_limit_rt, self.p_pv_limit_pu, 1)
-
-            if self.exec_delay.pv_mode_enable_exec == False and self.pf_of_active == True:
-                self.p_desired_pu = min(self.der_input.p_avl_pu, self.p_pf_pu, 1)
-
-            if self.exec_delay.pv_mode_enable_exec == True and self.pf_of_active == True:
-                self.p_desired_pu = min(self.der_input.p_avl_pu, self.p_pv_limit_pu, self.p_pf_pu, 1)
-
-            if self.exec_delay.pv_mode_enable_exec == False and self.pf_uf_active == True:
-                self.p_desired_pu = min(self.der_input.p_avl_pu, self.p_pf_pu, 1)
-
-            if self.exec_delay.pv_mode_enable_exec == True and self.pf_uf_active == True:
-                self.p_desired_pu = min(self.der_input.p_avl_pu, self.p_pv_limit_pu, self.p_pf_pu, 1)
-
-            # Eq 3.7.1-19, if the enter service ramp reference is greater than the desired active power,
-            # it is considered that the DER enter service is completed.
-            if self.p_es_pu > self.p_desired_pu:
-                self.es_completed = True
-        else:
-            # Eq 3.7.1-20, if DER is not in service, the desired active power should be 0, and it is not considered
-            # that enter service is completed
-            self.p_desired_pu = 0
-            self.es_completed = False
+        if self.exec_delay.pv_mode_enable_exec == False and self.pf_uf_active == True:
+            self.p_desired_pu = min(self.der_input.p_avl_pu, self.p_pf_pu, 1)
 
+        if self.exec_delay.pv_mode_enable_exec == True and self.pf_uf_active == True:
+            self.p_desired_pu = min(self.der_input.p_avl_pu, self.p_pv_limit_pu, self.p_pf_pu, 1)
 
         return self.p_desired_pu
 
     def __str__(self):
         return f"ap_limit_rt = {self.ap_limit_rt}, p_pv_limit_pu = {self.p_pv_limit_pu}, p_pf_pu = {self.p_pf_pu}, p_desired_pu = {self.p_desired_pu}"
+
+    def bess_specific(self):
+        pass
```

### Comparing `opender-2.0.3/src/opender/active_power_support_funcs/p_funcs_bess.py` & `opender-2.1.0/src/opender/active_power_support_funcs/p_funcs_bess.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,31 +9,28 @@
 #   and/or other materials provided with the distribution.
 # · Neither the name of the EPRI nor the names of its contributors may be used
 #   to endorse or promote products derived from this software without specific
 #   prior written permission.
 
 
 from opender.active_power_support_funcs.p_funcs import DesiredActivePower
-from opender.bess_specifc.soc import StateOfCharge
+
 from .frequency_droop_bess import FreqDroopBESS
-from .es_perf_bess import EnterServicePerformanceBESS
 from opender import DER
 
 
 class DesiredActivePowerBESS(DesiredActivePower):
     """
     Desired active power calculation from active power support functions for BESS DER
     EPRI Report Reference: Section 3.7.3 in Report #3002026631: IEEE 1547-2018 OpenDER Model
     """
     def __init__(self, der_obj):
         super(DesiredActivePowerBESS, self).__init__(der_obj)
 
         self.freqdroop = FreqDroopBESS(self.der_obj)
-        self.soc_calc = StateOfCharge(self.der_file)
-        self.enterserviceperf = EnterServicePerformanceBESS(der_obj)
 
         self.p_act_supp_bess_pu = None      # Desired output active power from active power support functions in per
                                             # unit without considering the BESS related constraints
         self.p_es_dem_pu = None             # Active power demand considering enter service ramp
 
     def calculate_p_desired_pu(self, p_out_w):
         """
@@ -47,69 +44,41 @@
         :param pv_mode_enable_exec:	    Volt-watt enable (PV_MODE_ENABLE) signal after execution delay
         :param der_status:	Status of DER (Trip, Entering Service, etc)
         :param NP_P_MAX_CHARGE:	DER active power charge rating
         :param NP_P_MAX:	    Active power rating at unity power factor
         :param p_dem_pu:        BESS DER active power demand in pu
         """
 
-        if DER.t_s <= 7200 and self.der_file.NP_BESS_CAPACITY is not None:
-            # For time series simulation
-            # Calculate SoC
-            self.soc_calc.calculate_soc(p_out_w)
-
-            # Calculate P limits
-            self.soc_calc.calculate_p_max_by_soc()
-        else:
-            # For snapshot analysis
-            self.soc_calc.snapshot_limits()
-
-        if self.der_obj.der_status != 'Trip':
-
-            # Eq 3.7.3-6, calculate active power demand considering enter service ramp
-            if self.der_input.p_dem_pu > 0:
-                self.p_es_dem_pu = min(self.der_input.p_dem_pu, self.p_es_pu)
-            else:
-                self.p_es_dem_pu = max(self.der_input.p_dem_pu, self.p_es_pu)
-
-            # Eq 3.7.3-7, calculate desired active power without considering BESS SoC related constraints
-            if self.exec_delay.ap_limit_enable_exec == False and self.exec_delay.pv_mode_enable_exec == False \
-                    and self.pf_uf_active == False and self.pf_of_active == False:
-                self.p_act_supp_bess_pu = min(self.p_es_dem_pu, 1)
-            if self.exec_delay.ap_limit_enable_exec == True and self.exec_delay.pv_mode_enable_exec == False \
-                    and self.pf_uf_active == False and self.pf_of_active == False:
-                self.p_act_supp_bess_pu = min(self.p_es_dem_pu, self.ap_limit_rt, 1)
-            if self.exec_delay.ap_limit_enable_exec == False and self.exec_delay.pv_mode_enable_exec == True \
-                    and self.pf_uf_active == False and self.pf_of_active == False:
-                self.p_act_supp_bess_pu = min(self.p_es_dem_pu, self.p_pv_limit_pu, 1)
-            if self.exec_delay.ap_limit_enable_exec == True and self.exec_delay.pv_mode_enable_exec == True \
-                    and self.pf_uf_active == False and self.pf_of_active == False:
-                self.p_act_supp_bess_pu = min(self.ap_limit_rt, self.p_pv_limit_pu, 1)
-            if self.exec_delay.pv_mode_enable_exec == False and self.pf_of_active == True:
-                self.p_act_supp_bess_pu = min(self.p_pf_pu, 1)
-            if self.exec_delay.pv_mode_enable_exec == True and self.pf_of_active == True:
-                self.p_act_supp_bess_pu = min(self.der_input.p_dem_pu, self.p_pv_limit_pu, self.p_pf_pu, 1)
-            if self.exec_delay.pv_mode_enable_exec == False and self.pf_uf_active == True:
-                self.p_act_supp_bess_pu = min(self.p_pf_pu, 1)
-            if self.exec_delay.pv_mode_enable_exec == True and self.pf_uf_active == True:
-                self.p_act_supp_bess_pu = min(self.p_pv_limit_pu, self.p_pf_pu, 1)
-
-            # Eq. 3.7.3-8, calculate desired active power, considering maximum limits by SOC, DER nameplate active
-            # power charge rating, and active power demand from system operator or higher level grid support functions
-            self.p_desired_pu = max(-self.soc_calc.p_max_charge_pu,
-                                    -self.der_file.NP_P_MAX_CHARGE / self.der_file.NP_P_MAX,
-                                    min(self.p_act_supp_bess_pu, self.soc_calc.p_max_discharge_pu))
-
-            # Eq. 3.7.3-9, the completion of enter service ramp is identified if the magnitude of enter service ramp
-            # reference is greater than the magnitude of actual DER output.
-            if self.der_input.p_dem_pu > 0:
-                if self.p_es_pu > self.p_desired_pu:
-                    self.es_completed = True
-            else:
-                if self.p_es_pu < self.p_desired_pu:
-                    self.es_completed = True
-        else:
-            # Eq. 3.7.1-20, if DER is not in service, the desired active power should be 0, and it is not considered
-            # that enter service process is completed.
-            self.p_desired_pu = 0
-            self.es_completed = False
+        # Eq 3.7.3-6, calculate active power demand considering enter service ramp
+        self.p_es_dem_pu = max(min(self.der_obj.bessspecific.p_dem_ramp_pu, self.p_es_pu), -self.p_es_pu)
+
+        # Eq 3.7.3-7, calculate desired active power without considering BESS SoC related constraints
+        if self.exec_delay.ap_limit_enable_exec == False and self.exec_delay.pv_mode_enable_exec == False \
+                and self.pf_uf_active == False and self.pf_of_active == False:
+            self.p_act_supp_bess_pu = min(self.p_es_dem_pu, 1)
+        if self.exec_delay.ap_limit_enable_exec == True and self.exec_delay.pv_mode_enable_exec == False \
+                and self.pf_uf_active == False and self.pf_of_active == False:
+            self.p_act_supp_bess_pu = min(self.p_es_dem_pu, self.ap_limit_rt, 1)
+        if self.exec_delay.ap_limit_enable_exec == False and self.exec_delay.pv_mode_enable_exec == True \
+                and self.pf_uf_active == False and self.pf_of_active == False:
+            self.p_act_supp_bess_pu = min(self.p_es_dem_pu, self.p_pv_limit_pu, 1)
+        if self.exec_delay.ap_limit_enable_exec == True and self.exec_delay.pv_mode_enable_exec == True \
+                and self.pf_uf_active == False and self.pf_of_active == False:
+            self.p_act_supp_bess_pu = min(self.ap_limit_rt, self.p_pv_limit_pu, 1)
+        if self.exec_delay.pv_mode_enable_exec == False and self.pf_of_active == True:
+            self.p_act_supp_bess_pu = min(self.p_pf_pu, 1)
+        if self.exec_delay.pv_mode_enable_exec == True and self.pf_of_active == True:
+            self.p_act_supp_bess_pu = min(self.der_input.p_dem_pu, self.p_pv_limit_pu, self.p_pf_pu, 1)
+        if self.exec_delay.pv_mode_enable_exec == False and self.pf_uf_active == True:
+            self.p_act_supp_bess_pu = min(self.p_pf_pu, 1)
+        if self.exec_delay.pv_mode_enable_exec == True and self.pf_uf_active == True:
+            self.p_act_supp_bess_pu = min(self.p_pv_limit_pu, self.p_pf_pu, 1)
+
+        # Eq. 3.7.3-8, calculate desired active power, considering maximum limits by SOC, DER nameplate active
+        # power charge rating, and active power demand from system operator or higher level grid support functions
+        self.p_desired_pu = max(-self.der_obj.bessspecific.soc_calc.p_max_charge_pu,
+                                -self.der_file.NP_P_MAX_CHARGE / self.der_file.NP_P_MAX,
+                                min(self.p_act_supp_bess_pu, self.der_obj.bessspecific.soc_calc.p_max_discharge_pu))
+
 
         return self.p_desired_pu
+
```

### Comparing `opender-2.0.3/src/opender/active_power_support_funcs/p_funcs_pv.py` & `opender-2.1.0/src/opender/active_power_support_funcs/p_funcs_pv.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender/active_power_support_funcs/volt_watt.py` & `opender-2.1.0/src/opender/active_power_support_funcs/volt_watt.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,15 +76,20 @@
                                 / (self.exec_delay.pv_curve_v2_exec-self.exec_delay.pv_curve_v1_exec) \
                                 * (self.pv_curve_p1_w - self.pv_curve_p2_w)
 
         # Eq. 3.7.1-3, convert volt-watt limit to per-unit using NP_P_MAX as base
         self.p_pv_limit_ref_pu = self.p_pv_limit_ref_w / self.der_file.NP_P_MAX
 
         # Eq. 3.7.1-4, apply the low pass filter and reaction time delay,
-        # if function disabled, reset limit to 1 immediately
         if self.exec_delay.pv_mode_enable_exec:
             self.p_pv_limit_lpf_pu = self.pv_lpf.low_pass_filter(self.p_pv_limit_ref_pu, self.exec_delay.pv_olrt_exec - self.der_file.NP_REACT_TIME)
+            self.p_pv_limit_pu = self.pv_delay.tdelay(self.p_pv_limit_lpf_pu, self.der_file.NP_REACT_TIME)
         else:
-            self.p_pv_limit_lpf_pu = self.pv_lpf.low_pass_filter(1, 0)
-        self.p_pv_limit_pu = self.pv_delay.tdelay(self.p_pv_limit_lpf_pu, self.der_file.NP_REACT_TIME)
+            self.reset()
 
         return self.p_pv_limit_pu
+
+    def reset(self):
+        # Eq. 3.7.1-5, resetting volt-watt function output and state variables to 1pu when DER is tripped or function
+        # is disabled
+        self.p_pv_limit_pu = self.pv_delay.tdelay(1,0)
+        self.p_pv_limit_lpf_pu = self.pv_lpf.low_pass_filter(1, 0)
```

### Comparing `opender-2.0.3/src/opender/auxiliary_funcs/__init__.py` & `opender-2.1.0/src/opender/auxiliary_funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender/auxiliary_funcs/cond_delay.py` & `opender-2.1.0/src/opender/auxiliary_funcs/cond_delay.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender/auxiliary_funcs/flipflop.py` & `opender-2.1.0/src/opender/auxiliary_funcs/flipflop.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender/auxiliary_funcs/low_pass_filter.py` & `opender-2.1.0/src/opender/auxiliary_funcs/low_pass_filter.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender/auxiliary_funcs/ramping.py` & `opender-2.1.0/src/opender/auxiliary_funcs/ramping.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender/auxiliary_funcs/sym_component.py` & `opender-2.1.0/src/opender/auxiliary_funcs/sym_component.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender/auxiliary_funcs/time_delay.py` & `opender-2.1.0/src/opender/auxiliary_funcs/time_delay.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender/bess_specifc/__init__.py` & `opender-2.1.0/src/opender/bess_specifc/__init__.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender/bess_specifc/soc.py` & `opender-2.1.0/src/opender/bess_specifc/soc.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,18 +76,18 @@
         if self.bess_soc <= 0:
             self.bess_soc = 0
 
     def calculate_p_max_by_soc(self):
 
         # Eq. 3.6.2-1 Calculate maximum discharge and charge active power at current SOC, defined by the capability
         # curve NP_BESS_P_MAX_BU_SOC
-        self.p_max_discharge_pu_soc = np.interp(self.bess_soc, self.der_file.NP_BESS_P_MAX_BY_SOC['SOC_P_CHARGE_MAX'],
+        self.p_max_charge_pu_soc = np.interp(self.bess_soc, self.der_file.NP_BESS_P_MAX_BY_SOC['SOC_P_CHARGE_MAX'],
                                                 self.der_file.NP_BESS_P_MAX_BY_SOC['P_CHARGE_MAX_PU'])
 
-        self.p_max_charge_pu_soc = np.interp(self.bess_soc, self.der_file.NP_BESS_P_MAX_BY_SOC['SOC_P_DISCHARGE_MAX'],
+        self.p_max_discharge_pu_soc = np.interp(self.bess_soc, self.der_file.NP_BESS_P_MAX_BY_SOC['SOC_P_DISCHARGE_MAX'],
                                              self.der_file.NP_BESS_P_MAX_BY_SOC['P_DISCHARGE_MAX_PU'])
 
         # Eq. 3.6.2-2 Calculate P charge limit to avoid over-charging in the next time step
         self.p_max_charge_pu_ts = min(((self.der_file.NP_BESS_SOC_MAX - self.bess_soc) / DER.t_s * 3600 +
                                        self.der_file.NP_BESS_SELF_DISCHARGE_SOC * self.bess_soc +
                                        self.der_file.NP_BESS_SELF_DISCHARGE) * self.der_file.NP_BESS_CAPACITY /
                                       self.der_file.NP_EFFICIENCY / self.der_file.NP_P_MAX_CHARGE, 1)
@@ -95,16 +95,16 @@
         # Eq. 3.6.2-3 Calculate P discharge limit to avoid over-discharging in the next time step
         self.p_max_discharge_pu_ts = max(0, min(((self.bess_soc - self.der_file.NP_BESS_SOC_MIN) / DER.t_s * 3600 -
                                                  self.der_file.NP_BESS_SELF_DISCHARGE_SOC * self.bess_soc -
                                                  self.der_file.NP_BESS_SELF_DISCHARGE) * self.der_file.NP_BESS_CAPACITY
                                                 / self.der_file.NP_P_MAX, 1))
 
         # Eq. 3.6.2-4 Calculate final maximum discharge/charge power using the two previously calculated limits
-        self.p_max_discharge_pu = min(self.p_max_charge_pu_soc, self.p_max_discharge_pu_ts)
-        self.p_max_charge_pu = min(self.p_max_discharge_pu_soc, self.p_max_charge_pu_ts)
+        self.p_max_discharge_pu = min(self.p_max_discharge_pu_soc, self.p_max_discharge_pu_ts)
+        self.p_max_charge_pu = min(self.p_max_charge_pu_soc, self.p_max_charge_pu_ts)
 
     def snapshot_limits(self):
         # Eq. 3.6.2-5, For snapshot analysis, the operational active power limits are set to 1, so they do not
         # impact other module calculations
         self.p_max_discharge_pu = 1
         self.p_max_charge_pu = 1
```

### Comparing `opender-2.0.3/src/opender/capability_and_priority.py` & `opender-2.1.0/src/opender/capability_and_priority.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender/common_file_format/common_file_format.py` & `opender-2.1.0/src/opender/common_file_format/common_file_format.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender/common_file_format/common_file_format_BESS.py` & `opender-2.1.0/src/opender/common_file_format/common_file_format_BESS.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 import logging
 from opender.common_file_format.common_file_format import DERCommonFileFormat
 
 
 class DERCommonFileFormatBESS(DERCommonFileFormat):
     parameters_list = DERCommonFileFormat.parameters_list + \
                       ['NP_BESS_SOC_MAX', 'NP_BESS_SOC_MIN', 'NP_BESS_CAPACITY', 'NP_BESS_SELF_DISCHARGE',
-                       'NP_BESS_SELF_DISCHARGE_SOC', 'NP_BESS_P_MAX_BY_SOC', 'P_DISCHARGE_MAX_PU',
-                       'SOC_P_DISCHARGE_MAX', 'P_CHARGE_MAX_PU', 'SOC_P_CHARGE_MAX', 'SOC_INIT'
+                       'NP_BESS_SELF_DISCHARGE_SOC', 'NP_BESS_P_MAX_BY_SOC', 'NP_BESS_P_RAMP_TIME',
+                       'P_DISCHARGE_MAX_PU', 'SOC_P_DISCHARGE_MAX', 'P_CHARGE_MAX_PU', 'SOC_P_CHARGE_MAX', 'SOC_INIT'
                        ]
 
     __slots__ = tuple(['_' + param for param in parameters_list]) + tuple(['param_inputs'])
 
     def __init__(self,
                  as_file_path=pathlib.Path(os.path.dirname(__file__)).joinpath("../Parameters", "AS-with std-values.csv"),
                  model_file_path=pathlib.Path(os.path.dirname(__file__)).joinpath("../Parameters","Model-parameters.csv"),
@@ -54,27 +54,30 @@
         self._NP_BESS_SELF_DISCHARGE_SOC = 0
         self._NP_BESS_P_MAX_BY_SOC = dict()
         self._P_DISCHARGE_MAX_PU = None
         self._SOC_P_DISCHARGE_MAX = None
         self._P_CHARGE_MAX_PU = None
         self._SOC_P_CHARGE_MAX = None
         self._SOC_INIT = 0.5
+        self._NP_BESS_P_RAMP_TIME = 0
 
         if self.isNotNaN(self.param_inputs.NP_BESS_SOC_MAX):
             self.NP_BESS_SOC_MAX = self.param_inputs.NP_BESS_SOC_MAX
         if self.isNotNaN(self.param_inputs.NP_BESS_SOC_MIN):
             self.NP_BESS_SOC_MIN = self.param_inputs.NP_BESS_SOC_MIN
         if self.isNotNaN(self.param_inputs.NP_BESS_CAPACITY):
             self.NP_BESS_CAPACITY = self.param_inputs.NP_BESS_CAPACITY
         if self.isNotNaN(self.param_inputs.NP_BESS_SELF_DISCHARGE):
             self.NP_BESS_SELF_DISCHARGE = self.param_inputs.NP_BESS_SELF_DISCHARGE
         if self.isNotNaN(self.param_inputs.NP_BESS_SELF_DISCHARGE_SOC):
             self.NP_BESS_SELF_DISCHARGE_SOC = self.param_inputs.NP_BESS_SELF_DISCHARGE_SOC
         if self.isNotNaN(self.param_inputs.NP_BESS_P_MAX_BY_SOC):
             self.NP_BESS_P_MAX_BY_SOC = self.param_inputs.NP_BESS_P_MAX_BY_SOC
+        if self.isNotNaN(self.param_inputs.NP_BESS_P_RAMP_TIME):
+            self.NP_BESS_P_RAMP_TIME = self.param_inputs.NP_BESS_P_RAMP_TIME
         if self.isNotNaN(self.param_inputs.P_DISCHARGE_MAX_PU):
             self.P_DISCHARGE_MAX_PU = self.param_inputs.P_DISCHARGE_MAX_PU
         if self.isNotNaN(self.param_inputs.SOC_P_DISCHARGE_MAX):
             self.SOC_P_DISCHARGE_MAX = self.param_inputs.SOC_P_DISCHARGE_MAX
         if self.isNotNaN(self.param_inputs.P_CHARGE_MAX_PU):
             self.P_CHARGE_MAX_PU = self.param_inputs.P_CHARGE_MAX_PU
         if self.isNotNaN(self.param_inputs.SOC_P_CHARGE_MAX):
@@ -181,14 +184,26 @@
         return self._NP_BESS_P_MAX_BY_SOC
 
     @NP_BESS_P_MAX_BY_SOC.setter
     def NP_BESS_P_MAX_BY_SOC(self, NP_BESS_P_MAX_BY_SOC):
         self._NP_BESS_P_MAX_BY_SOC = NP_BESS_P_MAX_BY_SOC
 
     @property
+    def NP_BESS_P_RAMP_TIME(self):
+        return self._NP_BESS_P_RAMP_TIME
+
+    @NP_BESS_P_RAMP_TIME.setter
+    def NP_BESS_P_RAMP_TIME(self, NP_BESS_P_RAMP_TIME):
+        if NP_BESS_P_RAMP_TIME<0:
+            logging.warning('Warning: BESS normal ramp time should be greater than 0')
+            self._NP_BESS_P_RAMP_TIME = 0
+        else:
+            self._NP_BESS_P_RAMP_TIME = NP_BESS_P_RAMP_TIME
+
+    @property
     def P_DISCHARGE_MAX_PU(self):
         return self._P_DISCHARGE_MAX_PU
 
     @P_DISCHARGE_MAX_PU.setter
     def P_DISCHARGE_MAX_PU(self, P_DISCHARGE_MAX_PU):
         self._P_DISCHARGE_MAX_PU = P_DISCHARGE_MAX_PU
```

### Comparing `opender-2.0.3/src/opender/der.py` & `opender-2.1.0/src/opender/der.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,19 +62,14 @@
         self.q_out_kvar = None
 
         if self.der_file.STATUS_INIT:
             self.der_status = 'Continuous Operation'
         else:
             self.der_status = 'Trip'
 
-        self.es_crit = None
-
-        self.p_out_w = None
-        self.q_out_var = None
-
         # DER model modules
         self.der_input = DERInputs(self.der_file)
         self.exec_delay = setting_execution_delay.SettingExecutionDelay(self.der_file)
         self.opstatus = OperatingStatus(self)
         self.activepowerfunc = DesiredActivePower(self)
         self.reactivepowerfunc = DesiredReactivePower(self)
         self.limited_p_q = CapabilityPriority(self)
@@ -183,14 +178,16 @@
 
         # Execution delay
         self.exec_delay.mode_and_execution_delay()
 
         # Determine DER operating status
         self.der_status = self.opstatus.determine_der_status()
 
+        self.bess_specific()
+
         # Calculate desired active power
         self.p_desired_pu = self.activepowerfunc.calculate_p_funcs(self.p_out_w)
 
         # Calculate desired reactive power
         self.q_desired_pu = self.reactivepowerfunc.calculate_reactive_funcs(self.p_desired_pu, self.der_status)
 
         # Limit DER output based on kVA rating and DER capability curve
@@ -257,7 +254,10 @@
         return f"{self.time:.1f}: {self.name} ({self.der_status})- " \
                f"v_meas_pu={self.der_input.v_meas_pu:.5f}, " \
                f"p_desired_pu={self.p_desired_pu:.2f}, q_desired_pu={self.q_desired_pu:.2f}, " \
                f"p_out_kw={self.p_out_kw:.3f}, q_out_kvar={self.q_out_kvar:.3f}"
 
     def get_DERCommonFileFormat(self, **kwargs):
         return DERCommonFileFormat(**kwargs)
+
+    def bess_specific(self):
+        pass
```

### Comparing `opender-2.0.3/src/opender/der_bess.py` & `opender-2.1.0/src/opender/der_bess.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,26 +10,27 @@
 # · Neither the name of the EPRI nor the names of its contributors may be used
 #   to endorse or promote products derived from this software without specific
 #   prior written permission.
 
 
 from . import DERCommonFileFormatBESS
 from .der import DER
+from .bess_specifc import bess_specific
 from .active_power_support_funcs.p_funcs_bess import DesiredActivePowerBESS
 from typing import Union, List
 
 class DER_BESS(DER):
     def __init__(self, der_file_obj=None, **kwargs):
         super(DER_BESS, self).__init__(der_file_obj, **kwargs)
         self.der_file.NP_Q_CAPABILITY_LOW_P = 'SAME'
         self.der_file.initialize_NP_Q_CAPABILTY_BY_P_CURVE()
 
         # replace active power support functions and enter service
         self.activepowerfunc = DesiredActivePowerBESS(self)
-        # self.enterservicetrip = EnterServiceCritBESS(self)
+        self.bessspecific = bess_specific.BESSspecific(self)
 
     def update_der_input(self, p_dem_w: float = None, v: Union[List[float], float] = None,
                          theta: Union[List[float], float] = None, v_symm_pu: List[complex] = None,
                          f: float = None, v_pu: Union[List[float], float] = None,
                          p_dem_pu: float = None, p_dem_kw: float = None) -> None:
         """
         Update DER inputs
@@ -54,8 +55,11 @@
 
         self._update_der_input_v_f(v, theta, v_symm_pu, f, v_pu)
 
     def get_DERCommonFileFormat(self):
         return DERCommonFileFormatBESS()
 
     def get_bess_soc(self) -> float:
-        return self.activepowerfunc.soc_calc.bess_soc
+        return self.bessspecific.soc_calc.bess_soc
+
+    def bess_specific(self):
+        self.bessspecific.run()
```

### Comparing `opender-2.0.3/src/opender/der_pv.py` & `opender-2.1.0/src/opender/der_pv.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender/op_cond_proc.py` & `opender-2.1.0/src/opender/op_cond_proc.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender/operation_status/__init__.py` & `opender-2.1.0/src/opender/operation_status/__init__.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender/operation_status/enter_service_crit/es_crit.py` & `opender-2.1.0/src/opender/operation_status/enter_service_crit/es_crit.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender/operation_status/enter_service_crit/es_crit_pv.py` & `opender-2.1.0/src/opender/operation_status/enter_service_crit/es_crit_pv.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender/operation_status/operating_status.py` & `opender-2.1.0/src/opender/operation_status/operating_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,33 +72,29 @@
         if self.der_status == 'Trip':
             if es_crit:
                 if opender.der.DER.t_s <= self.exec_delay.es_ramp_rate_exec:
                     self.der_status = 'Entering Service'
                 else:
                     self.der_status = 'Continuous Operation'
 
-        # Eq 3.5.1-53, If DER was Entering Service, and the enter service process has completed, DER goes to
-        # "Continuous Operation"
-        if self.der_status == 'Entering Service':
-            if self.der_obj.activepowerfunc.es_completed:
-                self.der_status = 'Continuous Operation'
-
-        # Eq 3.5.1-54~58, If DER is not Tripped (Entering Service, Continuous Operation, or all other Ride-through
+        # Eq 3.5.1-53~58, If DER is not Tripped (Entering Service, Continuous Operation, or all other Ride-through
         # modes), DER status depends on ride-through modes, in the priority of: Not Defined (frequency ride-through),
         # Other ride-through modes, and Continuous Operation.
         if self.der_status != 'Trip':
             if self.ridethroughcrit.rt_mode_f == 'Not Defined':
                 self.der_status = 'Not Defined'
             elif self.ridethroughcrit.rt_mode_v in ['Cease to Energize', 'Permissive Operation', 'Momentary Cessation']:
                 self.der_status = self.ridethroughcrit.rt_mode_v
             elif self.ridethroughcrit.rt_mode_v == 'Mandatory Operation' or self.ridethroughcrit.rt_mode_f == 'Mandatory Operation':
                 self.der_status = 'Mandatory Operation'
             else:
-                if self.der_status != 'Entering Service':
+                if self.der_obj.activepowerfunc.es_completed:
                     self.der_status = 'Continuous Operation'
+                else:
+                    self.der_status = 'Entering Service'
                 # Eq 3.5.1-57, If DER is in continuous operation, reset the flag that indicates required
                 # ride-through time has passed
                 self.ridethroughcrit.reset_rt_pass_time_req()
 
         # Eq. 3.5.1-59, if trip criteria is met, DER goes to Trip mode
         if trip_crit:
             self.der_status = 'Trip'
```

### Comparing `opender-2.0.3/src/opender/operation_status/operating_status_pv.py` & `opender-2.1.0/src/opender/operation_status/operating_status_pv.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender/operation_status/rt_crit.py` & `opender-2.1.0/src/opender/operation_status/rt_crit.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender/operation_status/trip_crit/trip_crit.py` & `opender-2.1.0/src/opender/operation_status/trip_crit/trip_crit.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender/operation_status/trip_crit/trip_crit_pv.py` & `opender-2.1.0/src/opender/operation_status/trip_crit/trip_crit_pv.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender/output_options.py` & `opender-2.1.0/src/opender/output_options.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender/reactive_power_support_funcs/constant_pf.py` & `opender-2.1.0/src/opender/reactive_power_support_funcs/constant_pf.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,7 +66,12 @@
         # Eq 3.8.1-2, apply the low pass filter and time delay (to model reaction time) to the reference reactive
         # power. Note that there can be multiple  different ways to implement this behavior in an actual DER.
         # The model may be updated in a future version, according to the lab test results.
         self.q_const_pf_lpf_pu = self.pf_lpf.low_pass_filter(self.q_const_pf_desired_ref_pu, self.der_file.CONST_PF_RT - self.der_file.NP_REACT_TIME)
         self.q_const_pf_desired_pu = self.pf_delay.tdelay(self.q_const_pf_lpf_pu, self.der_file.NP_REACT_TIME)
 
         return self.q_const_pf_desired_pu
+
+    def reset(self):
+        # Eq. 3.8.1-3, if DER is tripped, the reference should be reset to 0
+        self.q_const_pf_lpf_pu = self.pf_lpf.low_pass_filter(0, 0)
+        self.q_const_pf_desired_pu = self.pf_delay.tdelay(0, 0)
```

### Comparing `opender-2.0.3/src/opender/reactive_power_support_funcs/constant_vars.py` & `opender-2.1.0/src/opender/reactive_power_support_funcs/constant_vars.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     def __init__(self, der_obj):
 
         self.der_file = der_obj.der_file
         self.exec_delay = der_obj.exec_delay
 
         self.const_q_lpf = LowPassFilter()
         self.const_q_delay = TimeDelay()
+        self.q_const_q_lpf_pu = None
+        self.q_const_q_desired_pu = None
 
     def calculate_const_q_desired_var(self):
         """
         Calculates and returns output reactive power from Constant Power Factor function
 
         Variable used in this function:
         
@@ -40,14 +42,19 @@
         :param NP_REACT_TIME:	DER grid support function reaction time
 
         Output:
         
         :param const_q_desired_pu:	Output reactive power from constant reactive power function
         """
 
-        # Eq. 3.9.1-17, apply the low pass filter to the reference reactive power. Note that there can be multiple
+        # Eq. 3.8.1-13, apply the low pass filter to the reference reactive power. Note that there can be multiple
         # different ways to implement this behavior in an actual DER. The model may be updated in a future version,
         # according to the lab test results.
-        q_const_q_lpf_pu = self.const_q_lpf.low_pass_filter(self.exec_delay.const_q_exec, self.der_file.CONST_Q_RT - self.der_file.NP_REACT_TIME)
-        q_const_q_desired_pu = self.const_q_delay.tdelay(q_const_q_lpf_pu, self.der_file.NP_REACT_TIME)
+        self.q_const_q_lpf_pu = self.const_q_lpf.low_pass_filter(self.exec_delay.const_q_exec, self.der_file.CONST_Q_RT - self.der_file.NP_REACT_TIME)
+        self.q_const_q_desired_pu = self.const_q_delay.tdelay(self.q_const_q_lpf_pu, self.der_file.NP_REACT_TIME)
 
-        return q_const_q_desired_pu
+        return self.q_const_q_desired_pu
+
+    def reset(self):
+        # Eq. 3.8.1-14, if DER is tripped, the reference should be reset to 0
+        self.q_const_q_lpf_pu = self.const_q_lpf.low_pass_filter(self.exec_delay.const_q_exec, self.der_file.CONST_Q_RT - self.der_file.NP_REACT_TIME)
+        self.q_const_q_desired_pu = self.const_q_delay.tdelay(self.q_const_q_lpf_pu, self.der_file.NP_REACT_TIME)
```

### Comparing `opender-2.0.3/src/opender/reactive_power_support_funcs/q_funcs.py` & `opender-2.1.0/src/opender/reactive_power_support_funcs/q_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,29 +59,38 @@
         self.desired_var_ramp = Ramping()
         self.desired_var_ff = FlipFlop(0)
 
     def calculate_reactive_funcs(self, p_desired_pu, der_status):
         """
         Calculate desired reactive power for all 4 reactive power control modes defined in IEEE 1547-2018
         """
+        if der_status != 'Trip':
+            # Constant power factor function
+            self.q_const_pf_desired_pu = self.constpf.calculate_q_const_pf_desired_var(p_desired_pu)
 
-        # Constant power factor function
-        self.q_const_pf_desired_pu = self.constpf.calculate_q_const_pf_desired_var(p_desired_pu)
+            # Constant reactive power function
+            self.q_const_q_desired_pu = self.constq.calculate_const_q_desired_var()
 
-        # Constant reactive power function
-        self.q_const_q_desired_pu = self.constq.calculate_const_q_desired_var()
+            # Volt-var function
+            self.q_qv_desired_pu = self.voltvar.calculate_q_qv_desired_var()
 
-        # Volt-var function
-        self.q_qv_desired_pu = self.voltvar.calculate_q_qv_desired_var()
+            # Watt-var function
+            self.q_qp_desired_pu = self.wattvar.calculate_q_qp_desired_var(p_desired_pu)
 
-        # Watt-var function
-        self.q_qp_desired_pu = self.wattvar.calculate_q_qp_desired_var(p_desired_pu)
+            # Calculate reactive power based on grid-support functions
+            self.calculate_q_desired_pu(der_status)
+        else:
+            self.q_desired_pu = 0
+            self.q_mode_ramp_flag = self.desired_var_ff.flipflop(0,1)
+            self.q_desired_ramp_pu = self.desired_var_ramp.ramp(0,0,0)
+            self.constpf.reset()
+            self.constq.reset()
+            self.voltvar.reset()
+            self.wattvar.reset()
 
-        # Calculate reactive power based on grid-support functions
-        self.calculate_q_desired_pu(der_status)
 
         return self.q_desired_pu
 
 
     def calculate_q_desired_pu(self, der_status):
         """
         Calculate Desired reactive power considering the transition requirements defined by IEEE 1547-2018
@@ -98,59 +107,58 @@
 
 
         Output:
         
         :param q_desired_pu:	Desired output reactive power from reactive power support functions
         """
 
-        # Eq. 3.8.1-11, calculate desired reactive power reference, without smooth mode transition
-        if der_status != 'Trip':
-            if self.exec_delay.const_pf_mode_enable_exec == 1:
-                self.q_desired_ref_pu = self.q_const_pf_desired_pu
-            elif self.exec_delay.qv_mode_enable_exec == 1:
-                self.q_desired_ref_pu = self.q_qv_desired_pu
-            elif self.exec_delay.qp_mode_enable_exec == 1:
-                self.q_desired_ref_pu = self.q_qp_desired_pu
-            elif self.exec_delay.const_q_mode_enable_exec == 1:
-                self.q_desired_ref_pu = self.q_const_q_desired_pu
-            else:
-                self.q_desired_ref_pu = 0
+        # Eq. 3.8.1-15, calculate desired reactive power reference, without smooth mode transition
+
+        if self.exec_delay.const_pf_mode_enable_exec == 1:
+            self.q_desired_ref_pu = self.q_const_pf_desired_pu
+        elif self.exec_delay.qv_mode_enable_exec == 1:
+            self.q_desired_ref_pu = self.q_qv_desired_pu
+        elif self.exec_delay.qp_mode_enable_exec == 1:
+            self.q_desired_ref_pu = self.q_qp_desired_pu
+        elif self.exec_delay.const_q_mode_enable_exec == 1:
+            self.q_desired_ref_pu = self.q_const_q_desired_pu
         else:
             self.q_desired_ref_pu = 0
 
-        # Eq. 3.8.1-12, the ramp rate limit only applies when there is a mode change.
+
+        # Eq. 3.8.1-16, the ramp rate limit only applies when there is a mode change.
         if self.exec_delay.const_pf_mode_enable_exec != self.const_pf_mode_enable_exec_prev or \
                 self.exec_delay.qv_mode_enable_exec != self.qv_mode_enable_exec_prev or \
                 self.exec_delay.qp_mode_enable_exec != self.qp_mode_enable_exec_prev or \
                 self.exec_delay.const_q_mode_enable_exec != self.const_q_mode_enable_exec_prev:
             self.q_mode_ramp_flag_set = 1
         else:
             self.q_mode_ramp_flag_set = 0
 
         if self.q_mode_ramp_flag_set or self.q_mode_ramp_flag == 1:
-            # Eq. 3.8.1-13, apply the ramp rate limit
+            # Eq. 3.8.1-17, apply the ramp rate limit
             self.q_desired_ramp_pu = self.desired_var_ramp.ramp(self.q_desired_ref_pu,
                                                                 self.der_file.NP_MODE_TRANSITION_TIME,
                                                                 self.der_file.NP_MODE_TRANSITION_TIME)
         else:
-            # Eq. 3.8.1-14, if not in mode transition, ramp time of 0 is used to allow q_desired_ramp_var follow the
+            # Eq. 3.8.1-18, if not in mode transition, ramp time of 0 is used to allow q_desired_ramp_var follow the
             # desired reactive power
             self.q_desired_ramp_pu = self.desired_var_ramp.ramp(self.q_desired_ref_pu/self.der_file.NP_VA_MAX, 0, 0)
 
-        # Eq. 3.8.1-15, the ramp rate limit stops to apply when the mode transition is completed (value before and
+        # Eq. 3.8.1-19, the ramp rate limit stops to apply when the mode transition is completed (value before and
         # after ramp rate limit is the same
-        if self.q_desired_ref_pu == self.q_desired_ramp_pu or der_status == 0:
+        if self.q_desired_ref_pu == self.q_desired_ramp_pu:
             self.q_mode_ramp_flag_reset = 1
         else:
             self.q_mode_ramp_flag_reset = 0
 
-        # Eq. 3.8.1-16, apply the flipflop logic to decide if in mode transition
+        # Eq. 3.8.1-20, apply the flipflop logic to decide if in mode transition
         self.q_mode_ramp_flag = self.desired_var_ff.flipflop(self.q_mode_ramp_flag_set, self.q_mode_ramp_flag_reset)
 
-        # Eq. 3.8.1-17, if in mode transition, pass ramp rate limited value as output. If not, pass original value.
+        # Eq. 3.8.1-21, if in mode transition, pass ramp rate limited value as output. If not, pass original value.
         if self.q_mode_ramp_flag == 1:
             self.q_desired_pu = self.q_desired_ramp_pu
         else:
             self.q_desired_pu = self.q_desired_ref_pu
 
         # Save the values in for calculation in next time step
         self.const_pf_mode_enable_exec_prev = self.exec_delay.const_pf_mode_enable_exec
```

### Comparing `opender-2.0.3/src/opender/reactive_power_support_funcs/volt_var.py` & `opender-2.1.0/src/opender/reactive_power_support_funcs/volt_var.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,30 +65,30 @@
         :param qv_olrt_exec: Volt-var open loop response time after execution delay
 
 
         Output variables:
         :param q_qv_desired_pu: Output reactive power from volt-var function
         """
 
-        # Eq 3.8.1-3, The applied VRef is determined by either the VRef control setpoint or low pass filtered
+        # Eq 3.8.1-4, The applied VRef is determined by either the VRef control setpoint or low pass filtered
         # applicable voltage, depending on the enable signal
         self.qv_vref_lpf = max(0.95, min(self.v_meas_qv_vref_lpf_pu.low_pass_filter(self.der_input.v_meas_pu, self.exec_delay.qv_vref_time_exec),1.05))
         if self.exec_delay.qv_vref_auto_mode_exec == 0:
             self.qv_vref_appl = self.exec_delay.qv_vref_exec
         else:
             self.qv_vref_appl = self.qv_vref_lpf
 
-        # Eq 3.8.1-4, The applied volt-var curve voltage settings should shift according to the changes of the applied
+        # Eq 3.8.1-5, The applied volt-var curve voltage settings should shift according to the changes of the applied
         # VRef.
         self.qv_curve_v1_appl = self.exec_delay.qv_curve_v1_exec + self.qv_vref_appl - 1
         self.qv_curve_v2_appl = self.exec_delay.qv_curve_v2_exec + self.qv_vref_appl - 1
         self.qv_curve_v3_appl = self.exec_delay.qv_curve_v3_exec + self.qv_vref_appl - 1
         self.qv_curve_v4_appl = self.exec_delay.qv_curve_v4_exec + self.qv_vref_appl - 1
 
-        # Eq. 3.8.1-5, Volt-VAR Reactive power reference calculation in p.u
+        # Eq. 3.8.1-6, Volt-VAR Reactive power reference calculation in p.u
         if self.der_input.v_meas_pu < self.qv_curve_v1_appl:
             self.q_qv_desired_ref_pu = self.exec_delay.qv_curve_q1_exec
             
         if self.qv_curve_v2_appl >= self.der_input.v_meas_pu >= self.qv_curve_v1_appl:
             self.q_qv_desired_ref_pu = self.exec_delay.qv_curve_q1_exec - ((self.der_input.v_meas_pu - self.qv_curve_v1_appl)/(self.qv_curve_v2_appl - self.qv_curve_v1_appl)) * (self.exec_delay.qv_curve_q1_exec - self.exec_delay.qv_curve_q2_exec)
             
         if self.qv_curve_v3_appl > self.der_input.v_meas_pu > self.qv_curve_v2_appl:
@@ -96,14 +96,19 @@
             
         if self.qv_curve_v4_appl >= self.der_input.v_meas_pu >= self.qv_curve_v3_appl:
             self.q_qv_desired_ref_pu = self.exec_delay.qv_curve_q3_exec - ((self.der_input.v_meas_pu - self.qv_curve_v3_appl)/(self.qv_curve_v4_appl - self.qv_curve_v3_appl)) * (self.exec_delay.qv_curve_q3_exec - self.exec_delay.qv_curve_q4_exec)
         
         if self.der_input.v_meas_pu > self.qv_curve_v4_appl:
             self.q_qv_desired_ref_pu = self.exec_delay.qv_curve_q4_exec
 
-        # Eq. 3.9.1-6, OLRT using LPF followed by a time delay to represent a reaction delay
+        # Eq. 3.8.1-7, OLRT using LPF followed by a time delay to represent a reaction delay
         self.q_qv_lpf_pu = self.qv_lpf.low_pass_filter(self.q_qv_desired_ref_pu, self.exec_delay.qv_olrt_exec - self.der_file.NP_REACT_TIME)
         self.q_qv_desired_pu = self.qv_delay.tdelay(self.q_qv_lpf_pu, self.der_file.NP_REACT_TIME)
 
             
         return self.q_qv_desired_pu
-            
+
+    def reset(self):
+        # Eq. 3.8.1-8, if DER is tripped, the reference should be reset to 0
+        self.q_qv_lpf_pu = self.qv_lpf.low_pass_filter(0,0)
+        self.q_qv_desired_pu = self.qv_delay.tdelay(0,0)
+        self.qv_vref_lpf = self.v_meas_qv_vref_lpf_pu.low_pass_filter(self.der_input.v_meas_pu, 0)
```

### Comparing `opender-2.0.3/src/opender/reactive_power_support_funcs/watt_var.py` & `opender-2.1.0/src/opender/reactive_power_support_funcs/watt_var.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,18 +58,18 @@
         :param NP_VA_MAX:	Apparent power maximum rating
 
         Output:
         :param q_qp_desired_pu:	Output reactive power from watt-var function
 
         """
 
-        # Eq. 3.8.1-7, Calculate desired active power in per unit
+        # Eq. 3.8.1-9, Calculate desired active power in per unit
         self.p_desired_qp_pu = p_desired_pu * (1 if p_desired_pu > 0 else self.der_file.NP_P_MAX/self.der_file.NP_P_MAX_CHARGE)
 
-        # Eq. 3.8.1-8, calculate reactive power reference in per unit according to watt-var curve
+        # Eq. 3.8.1-10, calculate reactive power reference in per unit according to watt-var curve
         if self.p_desired_qp_pu <= self.exec_delay.qp_curve_p3_load_exec:
             self.q_qp_desired_ref_pu = self.exec_delay.qp_curve_q3_load_exec
 
         if (self.p_desired_qp_pu <= self.exec_delay.qp_curve_p2_load_exec) and (self.p_desired_qp_pu > self.exec_delay.qp_curve_p3_load_exec):
             self.q_qp_desired_ref_pu = self.exec_delay.qp_curve_q3_load_exec - ((self.p_desired_qp_pu - self.exec_delay.qp_curve_p3_load_exec)
                                   / (self.exec_delay.qp_curve_p2_load_exec - self.exec_delay.qp_curve_p3_load_exec)) \
                                   * (self.exec_delay.qp_curve_q3_load_exec - self.exec_delay.qp_curve_q2_load_exec)
@@ -93,14 +93,19 @@
             self.q_qp_desired_ref_pu = self.exec_delay.qp_curve_q2_gen_exec - ((self.p_desired_qp_pu - self.exec_delay.qp_curve_p2_gen_exec)
                                   / (self.exec_delay.qp_curve_p3_gen_exec - self.exec_delay.qp_curve_p2_gen_exec)) \
                                   * (self.exec_delay.qp_curve_q2_gen_exec - self.exec_delay.qp_curve_q3_gen_exec)
             
         if self.p_desired_qp_pu > self.exec_delay.qp_curve_p3_gen_exec:
             self.q_qp_desired_ref_pu = self.exec_delay.qp_curve_q3_gen_exec
 
-        # Eq. 3.8.1-9, apply a low pass filter and time delay to represent a possible time response of watt-var
+        # Eq. 3.8.1-11, apply a low pass filter and time delay to represent a possible time response of watt-var
         # function. Note that there can be multiple different ways to implement this behavior in actual DER.
         # The model may be updated in a future version, according to the lab test results.
         self.q_qp_lpf_pu = self.qp_lpf.low_pass_filter(self.q_qp_desired_ref_pu, self.der_file.QP_RT - self.der_file.NP_REACT_TIME)
         self.q_qp_desired_pu = self.qp_delay.tdelay(self.q_qp_lpf_pu, self.der_file.NP_REACT_TIME)
 
         return self.q_qp_desired_pu
+
+    def reset(self):
+        # Eq. 3.8.1-12, if DER is tripped, the reference should be reset to 0
+        self.q_qp_lpf_pu = self.qp_lpf.low_pass_filter(0,0)
+        self.q_qp_desired_pu = self.qp_delay.tdelay(0,0)
```

### Comparing `opender-2.0.3/src/opender/rt_perf.py` & `opender-2.1.0/src/opender/rt_perf.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender/setting_execution_delay.py` & `opender-2.1.0/src/opender/setting_execution_delay.py`

 * *Files identical despite different names*

### Comparing `opender-2.0.3/src/opender.egg-info/PKG-INFO` & `opender-2.1.0/src/opender.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opender
-Version: 2.0.3
+Version: 2.1.0
 Summary: Open-source Distributed Energy Resources (DER) Model that represents IEEE Standard 1547-2018 requirements for steady-state and dynamic analyses
 Home-page: https://github.com/epri-dev/opender
 Author: Yiwei Ma, Wei Ren, Paulo Radatz, Jithendar Anandan
 Author-email: yma@epri.com, wren@epri.com, pradatz@epri.com
 License: BSD
 Project-URL: Homepage, https://www.epri.com/OpenDER
 Project-URL: Model Specification, https://www.epri.com/research/products/000000003002021694
@@ -95,14 +95,21 @@
 Execution command: pytest path-to-package\\tests
 
 
 
 
 Changelog
 =========
+2.1.0 (2023-05-29)
+------------------
+* Updated interaction between enter service ramp and ride-through. Now DER returns to enter service ramp
+  after ride-through
+* Added an optional charge/discharge ramp rate limit for BESS DER
+* Added resets for all grid-support functions when DER is tripped
+
 2.0.3 (2023-04-14)
 ------------------
 * Fixed the option to update BESS DER parameter when creating the object.
 * Fixed a bug when initializing a BESS DER during abnormal frequency condition.
 
 2.0.2 (2023-04-03)
 ------------------
```

### Comparing `opender-2.0.3/src/opender.egg-info/SOURCES.txt` & `opender-2.1.0/src/opender.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 src/opender.egg-info/requires.txt
 src/opender.egg-info/top_level.txt
 src/opender/Parameters/AS-with std-values.csv
 src/opender/Parameters/Model-parameters.csv
 src/opender/active_power_support_funcs/__init__.py
 src/opender/active_power_support_funcs/active_power_limit.py
 src/opender/active_power_support_funcs/es_perf.py
-src/opender/active_power_support_funcs/es_perf_bess.py
 src/opender/active_power_support_funcs/frequency_droop.py
 src/opender/active_power_support_funcs/frequency_droop_bess.py
 src/opender/active_power_support_funcs/p_funcs.py
 src/opender/active_power_support_funcs/p_funcs_bess.py
 src/opender/active_power_support_funcs/p_funcs_pv.py
 src/opender/active_power_support_funcs/volt_watt.py
 src/opender/auxiliary_funcs/__init__.py
 src/opender/auxiliary_funcs/cond_delay.py
 src/opender/auxiliary_funcs/flipflop.py
 src/opender/auxiliary_funcs/low_pass_filter.py
 src/opender/auxiliary_funcs/ramping.py
 src/opender/auxiliary_funcs/sym_component.py
 src/opender/auxiliary_funcs/time_delay.py
 src/opender/bess_specifc/__init__.py
+src/opender/bess_specifc/bess_specific.py
 src/opender/bess_specifc/soc.py
 src/opender/common_file_format/__init__.py
 src/opender/common_file_format/common_file_format.py
 src/opender/common_file_format/common_file_format_BESS.py
 src/opender/operation_status/__init__.py
 src/opender/operation_status/operating_status.py
 src/opender/operation_status/operating_status_pv.py
```

