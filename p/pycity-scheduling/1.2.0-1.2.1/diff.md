# Comparing `tmp/pycity_scheduling-1.2.0.tar.gz` & `tmp/pycity_scheduling-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycity_scheduling-1.2.0.tar", last modified: Sun May 28 13:22:11 2023, max compression
+gzip compressed data, was "pycity_scheduling-1.2.1.tar", last modified: Tue May 30 13:46:02 2023, max compression
```

## Comparing `pycity_scheduling-1.2.0.tar` & `pycity_scheduling-1.2.1.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 schwarz  (1000067) users    (1000001)        0 2023-05-28 13:22:11.267594 pycity_scheduling-1.2.0/
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     1181 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/LICENSE.txt
--rw-r--r--   0 schwarz  (1000067) users    (1000001)    14130 2023-05-28 13:22:11.267016 pycity_scheduling-1.2.0/PKG-INFO
--rw-r--r--   0 schwarz  (1000067) users    (1000001)    13079 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/README.md
--rw-r--r--   0 schwarz  (1000067) users    (1000001)       38 2023-05-28 13:22:11.267760 pycity_scheduling-1.2.0/setup.cfg
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     2997 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/setup.py
-drwxr-xr-x   0 schwarz  (1000067) users    (1000001)        0 2023-05-28 13:22:11.136260 pycity_scheduling-1.2.0/src/
-drwxr-xr-x   0 schwarz  (1000067) users    (1000001)        0 2023-05-28 13:22:11.145586 pycity_scheduling-1.2.0/src/pycity_scheduling/
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     1502 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/__init__.py
-drwxr-xr-x   0 schwarz  (1000067) users    (1000001)        0 2023-05-28 13:22:11.165029 pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     2407 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/__init__.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)    18247 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/algorithm.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     3790 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/central_optimization_algorithm.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     7560 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/dual_decomposition_algorithm.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)    13129 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/dual_decomposition_algorithm_mpi.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     9471 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/exchange_admm_algorithm.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)    15116 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/exchange_admm_algorithm_mpi.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)    38707 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/exchange_miqp_admm_algorithm.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)    46132 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/exchange_miqp_admm_algorithm_mpi.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     4292 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/local_optimization_algorithm.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     2048 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/stand_alone_optimization_algorithm.py
-drwxr-xr-x   0 schwarz  (1000067) users    (1000001)        0 2023-05-28 13:22:11.197266 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     6740 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/__init__.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     3290 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/apartment.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     8281 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/battery.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     4607 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/boiler.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)    11100 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/building.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     5741 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/building_energy_system.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     6643 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/chiller.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     5335 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/city_district.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     5130 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/combined_heat_power.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)    10897 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/curtailable_load.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)    10906 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/deferrable_load.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     4564 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/electric_heater.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)    11739 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/electric_vehicle.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     6922 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/electrical_entity.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     5658 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/entity_container.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     1406 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/environment.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     7916 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/fixed_load.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     6414 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/heat_pump.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)    13587 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/optimization_entity.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     6350 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/photovoltaic.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     9540 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/prices.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     4250 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/space_cooling.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     5768 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/space_heating.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     5680 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/thermal_cooling_storage.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     2598 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/thermal_entity_cooling.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     2598 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/thermal_entity_heating.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     5736 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/thermal_heating_storage.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)    11526 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/timer.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     1389 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/weather.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     4501 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/wind_energy_converter.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     1587 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/constants.py
-drwxr-xr-x   0 schwarz  (1000067) users    (1000001)        0 2023-05-28 13:22:11.219453 pycity_scheduling-1.2.0/src/pycity_scheduling/data/
--rw-r--r--   0 schwarz  (1000067) users    (1000001)   878254 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/data/TRY_2018.dat
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     1206 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/data/__init__.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)   245151 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/data/co2_emissions_quarter-hour_2015.txt
--rw-r--r--   0 schwarz  (1000067) users    (1000001)      157 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/data/consumer_prices_yearly.txt
--rw-r--r--   0 schwarz  (1000067) users    (1000001)   209814 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/data/da_prices_quarter-hour_2015.txt
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     3384 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/data/ev_data.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)    10134 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/data/tabula_data.py
-drwxr-xr-x   0 schwarz  (1000067) users    (1000001)        0 2023-05-28 13:22:11.246022 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     1206 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/__init__.py
-drwxr-xr-x   0 schwarz  (1000067) users    (1000001)        0 2023-05-28 13:22:11.247363 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/case_studies/
--rw-r--r--   0 schwarz  (1000067) users    (1000001)    14406 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/case_studies/illustrative_code_example_cost_minimization_use_case_interactive.ipynb
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     9230 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_00_fundamentals.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     4939 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_01_algorithm_central.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     4813 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_02_algorithm_local.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     4855 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_03_algorithm_stand-alone.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     5299 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_04_algorithm_dual-decomposition.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     5161 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_05_algorithm_exchange-admm.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     7873 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_06_algorithm_exchange-miqp-admm.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     7440 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_07_algorithm_warmstart.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     9238 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_08_algorithm_parallel_mpi.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     3982 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_09_objective_peak-shaving.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     3993 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_10_objective_self-consumption.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     4153 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_11_objective_max-consumption.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     4565 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_12_objective_price.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     4668 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_13_objective_co2.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     5161 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_14_objective_valley-filling.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     4942 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_15_district_generator.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     6531 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_16_scheduling_complex_city_district.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     6328 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_17_district_flexibility_quantification.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     4987 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_18_scheduling_pv+battery_system.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     6816 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_19_scheduling_heating_and_cooling_loads.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     7198 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_20_scheduling_convex_vs._integer_mode.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     4546 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_21_scheduling_robust_optimization.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     7526 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_22_post-processing_schedule_evaluation.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     4739 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_23_post-processing_metrics_evaluation.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     1605 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/exceptions.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     2448 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/solvers.py
-drwxr-xr-x   0 schwarz  (1000067) users    (1000001)        0 2023-05-28 13:22:11.248615 pycity_scheduling-1.2.0/src/pycity_scheduling/testing/
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     1206 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/testing/__init__.py
-drwxr-xr-x   0 schwarz  (1000067) users    (1000001)        0 2023-05-28 13:22:11.255606 pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     1206 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/__init__.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     9236 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/test_algorithms.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     2627 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/test_all_classes.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)    71186 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/test_classes.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     2064 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/test_examples.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)    19729 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/test_util.py
-drwxr-xr-x   0 schwarz  (1000067) users    (1000001)        0 2023-05-28 13:22:11.265858 pycity_scheduling-1.2.0/src/pycity_scheduling/util/
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     9168 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/util/__init__.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     4325 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/util/debug.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)    28659 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/util/district_analyzer.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)    19720 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/util/factory.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     5813 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/util/generic_constraints.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)    13889 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/util/metric.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     4488 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/util/mpi_interface.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)    10383 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/util/plot_schedules.py
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     5488 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/util/write_schedules.py
-drwxr-xr-x   0 schwarz  (1000067) users    (1000001)        0 2023-05-28 13:22:11.151627 pycity_scheduling-1.2.0/src/pycity_scheduling.egg-info/
--rw-r--r--   0 schwarz  (1000067) users    (1000001)    14130 2023-05-28 13:22:11.000000 pycity_scheduling-1.2.0/src/pycity_scheduling.egg-info/PKG-INFO
--rw-r--r--   0 schwarz  (1000067) users    (1000001)     5509 2023-05-28 13:22:11.000000 pycity_scheduling-1.2.0/src/pycity_scheduling.egg-info/SOURCES.txt
--rw-r--r--   0 schwarz  (1000067) users    (1000001)        1 2023-05-28 13:22:11.000000 pycity_scheduling-1.2.0/src/pycity_scheduling.egg-info/dependency_links.txt
--rw-r--r--   0 schwarz  (1000067) users    (1000001)        1 2023-05-28 13:22:11.000000 pycity_scheduling-1.2.0/src/pycity_scheduling.egg-info/not-zip-safe
--rw-r--r--   0 schwarz  (1000067) users    (1000001)      114 2023-05-28 13:22:11.000000 pycity_scheduling-1.2.0/src/pycity_scheduling.egg-info/requires.txt
--rw-r--r--   0 schwarz  (1000067) users    (1000001)       18 2023-05-28 13:22:11.000000 pycity_scheduling-1.2.0/src/pycity_scheduling.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:46:02.375507 pycity_scheduling-1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    16509 2023-05-30 13:46:02.375507 pycity_scheduling-1.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    13079 2023-05-30 10:02:23.000000 pycity_scheduling-1.2.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 13:46:02.376507 pycity_scheduling-1.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2997 2023-05-30 10:02:23.000000 pycity_scheduling-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:46:02.361507 pycity_scheduling-1.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:46:02.362506 pycity_scheduling-1.2.1/src/pycity_scheduling/
+-rw-rw-rw-   0 root         (0) root         (0)     1502 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:46:02.364507 pycity_scheduling-1.2.1/src/pycity_scheduling/algorithms/
+-rw-rw-rw-   0 root         (0) root         (0)     2407 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/algorithms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18247 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/algorithms/algorithm.py
+-rw-rw-rw-   0 root         (0) root         (0)     3790 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/algorithms/central_optimization_algorithm.py
+-rw-rw-rw-   0 root         (0) root         (0)     7560 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/algorithms/dual_decomposition_algorithm.py
+-rw-rw-rw-   0 root         (0) root         (0)    13129 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/algorithms/dual_decomposition_algorithm_mpi.py
+-rw-rw-rw-   0 root         (0) root         (0)     9471 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/algorithms/exchange_admm_algorithm.py
+-rw-rw-rw-   0 root         (0) root         (0)    15116 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/algorithms/exchange_admm_algorithm_mpi.py
+-rw-rw-rw-   0 root         (0) root         (0)    38707 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/algorithms/exchange_miqp_admm_algorithm.py
+-rw-rw-rw-   0 root         (0) root         (0)    46132 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/algorithms/exchange_miqp_admm_algorithm_mpi.py
+-rw-rw-rw-   0 root         (0) root         (0)     4292 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/algorithms/local_optimization_algorithm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2048 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/algorithms/stand_alone_optimization_algorithm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:46:02.368507 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/
+-rw-rw-rw-   0 root         (0) root         (0)     6740 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3290 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/apartment.py
+-rw-rw-rw-   0 root         (0) root         (0)     8281 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/battery.py
+-rw-rw-rw-   0 root         (0) root         (0)     4607 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/boiler.py
+-rw-rw-rw-   0 root         (0) root         (0)    11100 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/building.py
+-rw-rw-rw-   0 root         (0) root         (0)     5741 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/building_energy_system.py
+-rw-rw-rw-   0 root         (0) root         (0)     6643 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/chiller.py
+-rw-rw-rw-   0 root         (0) root         (0)     5335 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/city_district.py
+-rw-rw-rw-   0 root         (0) root         (0)     5130 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/combined_heat_power.py
+-rw-rw-rw-   0 root         (0) root         (0)    10897 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/curtailable_load.py
+-rw-rw-rw-   0 root         (0) root         (0)    10906 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/deferrable_load.py
+-rw-rw-rw-   0 root         (0) root         (0)     4564 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/electric_heater.py
+-rw-rw-rw-   0 root         (0) root         (0)    11739 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/electric_vehicle.py
+-rw-rw-rw-   0 root         (0) root         (0)     6922 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/electrical_entity.py
+-rw-rw-rw-   0 root         (0) root         (0)     5658 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/entity_container.py
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)     7916 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/fixed_load.py
+-rw-rw-rw-   0 root         (0) root         (0)     6414 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/heat_pump.py
+-rw-rw-rw-   0 root         (0) root         (0)    13587 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/optimization_entity.py
+-rw-rw-rw-   0 root         (0) root         (0)     6350 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/photovoltaic.py
+-rw-rw-rw-   0 root         (0) root         (0)     9540 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/prices.py
+-rw-rw-rw-   0 root         (0) root         (0)     4250 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/space_cooling.py
+-rw-rw-rw-   0 root         (0) root         (0)     5768 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/space_heating.py
+-rw-rw-rw-   0 root         (0) root         (0)     5680 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/thermal_cooling_storage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2598 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/thermal_entity_cooling.py
+-rw-rw-rw-   0 root         (0) root         (0)     2598 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/thermal_entity_heating.py
+-rw-rw-rw-   0 root         (0) root         (0)     5736 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/thermal_heating_storage.py
+-rw-rw-rw-   0 root         (0) root         (0)    11526 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/timer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1389 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/weather.py
+-rw-rw-rw-   0 root         (0) root         (0)     4501 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/classes/wind_energy_converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:46:02.370507 pycity_scheduling-1.2.1/src/pycity_scheduling/data/
+-rw-rw-rw-   0 root         (0) root         (0)   878254 2023-04-12 17:45:33.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/data/TRY_2018.dat
+-rw-rw-rw-   0 root         (0) root         (0)     1206 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   245151 2022-12-22 14:16:57.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/data/co2_emissions_quarter-hour_2015.txt
+-rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-22 14:16:57.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/data/consumer_prices_yearly.txt
+-rw-rw-rw-   0 root         (0) root         (0)   209814 2022-12-22 14:16:57.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/data/da_prices_quarter-hour_2015.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3384 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/data/ev_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    10134 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/data/tabula_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:46:02.373507 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     1206 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:46:02.373507 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/case_studies/
+-rw-rw-rw-   0 root         (0) root         (0)    14406 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/case_studies/illustrative_code_example_cost_minimization_use_case_interactive.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     9230 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_00_fundamentals.py
+-rw-rw-rw-   0 root         (0) root         (0)     4939 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_01_algorithm_central.py
+-rw-rw-rw-   0 root         (0) root         (0)     4813 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_02_algorithm_local.py
+-rw-rw-rw-   0 root         (0) root         (0)     4855 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_03_algorithm_stand-alone.py
+-rw-rw-rw-   0 root         (0) root         (0)     5299 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_04_algorithm_dual-decomposition.py
+-rw-rw-rw-   0 root         (0) root         (0)     5161 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_05_algorithm_exchange-admm.py
+-rw-rw-rw-   0 root         (0) root         (0)     7873 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_06_algorithm_exchange-miqp-admm.py
+-rw-rw-rw-   0 root         (0) root         (0)     7440 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_07_algorithm_warmstart.py
+-rw-rw-rw-   0 root         (0) root         (0)     9238 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_08_algorithm_parallel_mpi.py
+-rw-rw-rw-   0 root         (0) root         (0)     3982 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_09_objective_peak-shaving.py
+-rw-rw-rw-   0 root         (0) root         (0)     3993 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_10_objective_self-consumption.py
+-rw-rw-rw-   0 root         (0) root         (0)     4153 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_11_objective_max-consumption.py
+-rw-rw-rw-   0 root         (0) root         (0)     4565 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_12_objective_price.py
+-rw-rw-rw-   0 root         (0) root         (0)     4668 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_13_objective_co2.py
+-rw-rw-rw-   0 root         (0) root         (0)     5161 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_14_objective_valley-filling.py
+-rw-rw-rw-   0 root         (0) root         (0)     4942 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_15_district_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     6531 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_16_scheduling_complex_city_district.py
+-rw-rw-rw-   0 root         (0) root         (0)     6328 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_17_district_flexibility_quantification.py
+-rw-rw-rw-   0 root         (0) root         (0)     4987 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_18_scheduling_pv+battery_system.py
+-rw-rw-rw-   0 root         (0) root         (0)     6816 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_19_scheduling_heating_and_cooling_loads.py
+-rw-rw-rw-   0 root         (0) root         (0)     7198 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_20_scheduling_convex_vs._integer_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)     4546 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_21_scheduling_robust_optimization.py
+-rw-rw-rw-   0 root         (0) root         (0)     7526 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_22_post-processing_schedule_evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4739 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_23_post-processing_metrics_evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1605 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2448 2023-05-30 10:45:44.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/solvers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:46:02.373507 pycity_scheduling-1.2.1/src/pycity_scheduling/testing/
+-rw-rw-rw-   0 root         (0) root         (0)     1206 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/testing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:46:02.374507 pycity_scheduling-1.2.1/src/pycity_scheduling/testing/unit_tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1206 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/testing/unit_tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9236 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/testing/unit_tests/test_algorithms.py
+-rw-rw-rw-   0 root         (0) root         (0)     2627 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/testing/unit_tests/test_all_classes.py
+-rw-rw-rw-   0 root         (0) root         (0)    71186 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/testing/unit_tests/test_classes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/testing/unit_tests/test_examples.py
+-rw-rw-rw-   0 root         (0) root         (0)    19729 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/testing/unit_tests/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:46:02.375507 pycity_scheduling-1.2.1/src/pycity_scheduling/util/
+-rw-rw-rw-   0 root         (0) root         (0)     9168 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4325 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/util/debug.py
+-rw-rw-rw-   0 root         (0) root         (0)    28659 2023-04-12 18:51:40.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/util/district_analyzer.py
+-rw-rw-rw-   0 root         (0) root         (0)    19720 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/util/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5813 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/util/generic_constraints.py
+-rw-rw-rw-   0 root         (0) root         (0)    13889 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/util/metric.py
+-rw-rw-rw-   0 root         (0) root         (0)     4488 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/util/mpi_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)    10383 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/util/plot_schedules.py
+-rw-rw-rw-   0 root         (0) root         (0)     5488 2023-05-25 14:04:15.000000 pycity_scheduling-1.2.1/src/pycity_scheduling/util/write_schedules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:46:02.363507 pycity_scheduling-1.2.1/src/pycity_scheduling.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16509 2023-05-30 13:46:02.000000 pycity_scheduling-1.2.1/src/pycity_scheduling.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5509 2023-05-30 13:46:02.000000 pycity_scheduling-1.2.1/src/pycity_scheduling.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 13:46:02.000000 pycity_scheduling-1.2.1/src/pycity_scheduling.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 13:46:02.000000 pycity_scheduling-1.2.1/src/pycity_scheduling.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      114 2023-05-30 13:46:02.000000 pycity_scheduling-1.2.1/src/pycity_scheduling.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-30 13:46:02.000000 pycity_scheduling-1.2.1/src/pycity_scheduling.egg-info/top_level.txt
```

### Comparing `pycity_scheduling-1.2.0/LICENSE.txt` & `pycity_scheduling-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/PKG-INFO` & `pycity_scheduling-1.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: pycity_scheduling
-Version: 1.2.0
-Summary: A Python framework for the development, testing, and assessment of optimization-basedpower scheduling algorithms for multi-energy systems in city districts
-Home-page: https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling
-Author: Institute for Automation of Complex Power Systems (ACS),E.ON Energy Research Center (E.ON ERC),RWTH Aachen University
-Author-email: post_acs@eonerc.rwth-aachen.de
-License: MIT
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Scientific/Engineering
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE.txt
-
 <img src="https://fein-aachen.org/img/logos/pycity_scheduling.png" width="150"/>
 
 # pycity_scheduling
 
 Python package pycity_scheduling is a framework for the effective development, testing, and assessment of optimization-based power scheduling algorithms for local multi-energy systems in city districts.
 The framework primarily targets the elaboration of coordination concepts that can efficiently solve the power dispatch problem on the city district level.
 Its target users are researchers in the field of smart grid applications and the deployment of operational flexibility for local energy systems.
@@ -62,15 +39,15 @@
 - [bonmin](https://github.com/coin-or/Bonmin)
 - [Gurobi (gurobipy)](https://www.gurobi.com/products/gurobi-optimizer/) (default)
 - [IBM ILOG CPLEX](https://www.ibm.com/products/ilog-cplex-optimization-studio)
 
 
 ### Installation of pycity_scheduling
 
-The latest version of pycity_scheduling is v1.2.0.
+The latest version of pycity_scheduling is v1.2.1.
 
 If all the abovementioned dependencies are installed, you should be able to install package pycity_scheduling via [PyPI](https://pypi.org/) (using Python version >= 3.7) as follows:
 
 `pip install pycity_scheduling`
 
 or to install in editable mode:
```

### Comparing `pycity_scheduling-1.2.0/README.md` & `pycity_scheduling-1.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,299 +1,321 @@
-<img src="https://fein-aachen.org/img/logos/pycity_scheduling.png" width="150"/>
-
-# pycity_scheduling
-
-Python package pycity_scheduling is a framework for the effective development, testing, and assessment of optimization-based power scheduling algorithms for local multi-energy systems in city districts.
-The framework primarily targets the elaboration of coordination concepts that can efficiently solve the power dispatch problem on the city district level.
-Its target users are researchers in the field of smart grid applications and the deployment of operational flexibility for local energy systems.
-
-
-## Contribution
-
-1. Clone repository via SSH (`git clone git@git.rwth-aachen.de:acs/public/simulation/pycity_scheduling.git`) or clone repository via HTTPS (`git clone https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling.git`)
-2. Open an issue at [https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling/-/issues](https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling/-/issues)
-3. Checkout the development branch: `git checkout development` 
-4. Update your local development branch (if necessary): `git pull origin development`
-5. Create your feature/issue branch: `git checkout -b issueXY_explanation`
-6. Commit your changes: `git commit -m "Add feature #XY"`
-7. Push to the branch: `git push origin issueXY_explanation`
-8. Submit a merge request from issueXY_explanation to development branch via [https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling/-/merge_requests](https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling/-/merge_requests)
-9. Wait for approval or revision of the new implementations.
-
-## Installation
-
-pycity_scheduling requires at least the following Python packages:
-- numpy==1.19.5
-- pandas==1.1.5
-- matplotlib==3.3.4
-- pyomo==5.7.3
-- pycity_base==0.3.2
-- pylint (optional)
-- sphinx (optional)
-- numpydoc (optional)
-- pytest (optional)
-
-as well as the installation of at least one mathematical programming solver for convex and/or non-convex problems, which is supported by the [Pyomo](http://www.pyomo.org/) optimisation modelling library.
-We recommend one of the following solvers:
-
-- [SCIP](https://www.scipopt.org/)
-- [bonmin](https://github.com/coin-or/Bonmin)
-- [Gurobi (gurobipy)](https://www.gurobi.com/products/gurobi-optimizer/) (default)
-- [IBM ILOG CPLEX](https://www.ibm.com/products/ilog-cplex-optimization-studio)
-
-
-### Installation of pycity_scheduling
-
-The latest version of pycity_scheduling is v1.2.0.
-
-If all the abovementioned dependencies are installed, you should be able to install package pycity_scheduling via [PyPI](https://pypi.org/) (using Python version >= 3.7) as follows:
-
-`pip install pycity_scheduling`
-
-or to install in editable mode:
-
-`pip install -e '<your_path_to_pycity_scheduling_git_folder>'`
-
-or:
-
-`<path_to_your_python_binary> -m pip install -e '<your_path_to_pycity_scheduling_git_folder>/src'`
-
-The project can also be installed in editable mode directly from gitlab without the need for a previous download:
-
-`pip install -e "git+ssh://git.rwth-aachen.de:acs/public/simulation/pycity_scheduling.git"`
-
-or:
-
-`pip install --src <install_location> -e "git+ssh://git.rwth-aachen.de:acs/public/simulation/pycity_scheduling.git"`
-
-You can check if the installation has been successful by trying to import package pycity_scheduling into your Python environment.
-This import should be possible without any errors.
-
-`import pycity_scheduling`
-
-
-You may also try to run the pycity_scheduling's unit tests located in folder ./src/testing using Python module pytest.
-
-
-## Documentation
-
-The documentation for the latest pycity_scheduling release can be found in folder ./docs and on [this](https://acs.pages.rwth-aachen.de/public/simulation/pycity_scheduling/) GitLab page.
-
-For further information, please also visit the [FEIN Aachen association website](https://fein-aachen.org/en/projects/pycity_scheduling/).
-
-
-## Example usage
-
-```python
-import numpy as np
-import matplotlib.pyplot as plt
-
-from pycity_scheduling.classes import *
-from pycity_scheduling.algorithms import *
-import pycity_scheduling.util.debug as debug
-
-
-# This is a fundamental tutorial on how to use the pycity_scheduling package.
-
-
-def main(do_plot=False):
-    print("\n\n------ Example 00: Fundamentals ------\n\n")
-
-    # 1) Environment objects:
-
-    # (Almost) every object within pycity_scheduling requires an environment. The environment object holds general data,
-    # which is valid for all objects within pycity_scheduling, such as time data, weather data or energy market prices.
-    # Therefore, all objects point to an environment. The first step is usually to generate such an environment.
-
-    # Generate a timer object for the environment:
-    timer = Timer(step_size=3600, op_horizon=24, initial_date=(2015, 1, 1), initial_time=(0, 0, 0))
-
-    # Generate a weather object for the environment:
-    weather = Weather(timer=timer)
-
-    # Generate a price object for the environment:
-    price = Prices(timer=timer)
-
-    # Generate the environment object:
-    environment = Environment(timer=timer, weather=weather, prices=price)
-
-    # Now there is a distinct environment object with timer, weather and price data.
-    # We can use it to access different data of interest.
-
-    # For example, print the current weekday:
-    print('Weekday:')
-    print(environment.timer.weekday)
-
-    # For example, print the weather forecast for the outdoor temperature (only extract the first 10 timestep values):
-    print('\nOutdoor temperature forecast:')
-    print(environment.weather.getWeatherForecast(getTAmbient=True)[0][:10])
-
-    # For example, print the energy spot market day-ahead prices:
-    print('\nDay-ahead spot market prices on 2015/01/01:')
-    print(environment.prices.da_prices)
-
-    # 2) Buildings objects:
-
-    # After defining the environment, different building objects should be created. In pycity_scheduling, buildings
-    # represent the different customers of the local energy system / city district under investigation.
-    # In general, buildings should also be understood in a more abstract way. For instance, a building object must not
-    # necessarily represent a building structure, as it would be the case for a wind energy converter.
-
-    # Create a building object:
-    building = Building(environment=environment)
-
-    # This building is assumed to be equipped with a building energy system and one apartment (=single-family house).
-    # In general, every building object can, however, hold up to N different apartments (=multi-family house).
-    apartment = Apartment(environment=environment)
-    bes = BuildingEnergySystem(environment=environment)
-
-    building.addMultipleEntities([apartment, bes])
-
-    # Every apartment usually possesses both electrical and thermal loads:
-    # The electrical load is added to the apartment as follows:
-    load = FixedLoad(environment=environment, method=1, annual_demand=3000)
-
-    # Print and show the electrical power curve in Watt:
-    print('\nElectrical load in Watt:')
-    print(load.get_power(currentValues=False))
-    plt.plot(load.get_power(currentValues=False))
-    plt.xlabel('Time in hours')
-    plt.ylabel('Electrical power in Watt (fixed load)')
-    plt.title('Fixed load power curve')
-    if do_plot:
-        plt.show()
-
-    # The thermal load is added to the apartment as follows:
-    space_heating = SpaceHeating(environment=environment, method=1, living_area=150, specific_demand=100)
-
-    # Print and show space heating power curve in Watt:
-    print('\nSpace heating power curve in Watt:')
-    print(space_heating.get_power(currentValues=False))
-
-    plt.plot(space_heating.get_power(currentValues=False))
-    plt.xlabel('Time in hours')
-    plt.ylabel('Thermal power in Watt (space heating)')
-    plt.title('Space heating power curve')
-    if do_plot:
-        plt.show()
-
-    apartment.addMultipleEntities([load, space_heating])
-
-    # The BuildingEnergySystem (BES) class is a 'container' for all kind of building energy systems (i.e., electrical
-    # and/or thermal assets). For example, we can add an electro-thermal heating system (such as a heatpump plus thermal
-    # energy storage) and a photovoltaic unit to a building's BES as done below. In pycity_scheduling all BES devices
-    # automatically come with basic scheduling models, which include the required Pyomo optimization variables and
-    # several optimization constraints.
-    eh = HeatPump(environment=environment, p_th_nom=16.0)
-    ths = ThermalHeatingStorage(environment=environment, e_th_max=20.0, soc_init=0.5, loss_factor=0)
-    pv = Photovoltaic(environment=environment, method=0, peak_power=8.0)
-
-    bes.addMultipleDevices([eh, ths, pv])
-
-    # Verify if the assets were added successfully (method getHasDevice):
-    print('\nBES has heatpump? : ', bes.getHasDevices(all_devices=False, heatpump=True)[0])
-    print('BES has thermal heating storage? : ', bes.getHasDevices(all_devices=False, ths=True)[0])
-    print('BES has photovoltaic? : ', bes.getHasDevices(all_devices=False, pv=True)[0])
-
-    # 3) CityDistrict objects:
-
-    # In pycity_scheduling, a group of buildings form a CityDistrict object. The CityDistrict is the object to be
-    # "provided" to a power scheduling algorithm later on. In other word, it encapsulates all buildings together with
-    # their local assets and it hence includes all the optimization problem information and data.
-
-    # Create a city district object:
-    cd = CityDistrict(environment=environment)
-
-    # Add the building from above to the city district at a certain position/coordinate (x, y).
-    cd.addEntity(entity=building, position=[0, 0])
-
-    # Define and add three other buildings:
-    for i in range(3):
-        heat_demand = SpaceHeating(environment=environment, method=1, living_area=150, specific_demand=100)
-
-        el_load_demand = FixedLoad(environment=environment, method=1, annual_demand=3000)
-
-        pv = Photovoltaic(environment=environment, method=0, peak_power=5.0)
-        bl = Boiler(environment=environment, p_th_nom=24.0)
-
-        ap = Apartment(environment=environment)
-        ap.addEntity(heat_demand)
-        ap.addEntity(el_load_demand)
-
-        bes = BuildingEnergySystem(environment=environment)
-        bes.addDevice(pv)
-        bes.addDevice(bl)
-
-        bd = Building(environment=environment)
-        bd.addEntity(entity=ap)
-        bd.addEntity(entity=bes)
-
-        cd.addEntity(entity=bd, position=[0, i])
-
-    # Print the city district information:
-    print('\nTotal number of buildings in city district:')
-    print(cd.get_nb_of_building_entities())
-    print("\nDetailed city district information:")
-    debug.print_district(cd, 3)
-
-    # 4) Power scheduling:
-
-    # The final step is to schedule the buildings/assets inside the city district subject to a certain optimization
-    # objective, which can be, for example, peak-shaving. The scheduling is then performed by the user by "passing"
-    # the city district object to a certain power scheduling algorithm.
-    # Here, the central optimization algorithm is used.
-
-    # Set the city district / district operator objective and perform the power scheduling using the central
-    # optimization algorithm:
-    cd.set_objective("peak-shaving")
-    opt = CentralOptimization(cd)
-    opt.solve()
-
-    # The scheduling results obtained from the algorithm run can be (temporally) stored as follows:
-    cd.copy_schedule("my_central_scheduling")
-
-    # Print and show the scheduling result (city district power values for every time slot within the defined
-    # optimization horizon):
-    print("\nPower schedule of city district:")
-    print(list(cd.p_el_schedule))
-
-    plt.plot(cd.p_el_schedule, drawstyle='steps')
-    plt.xlabel('Time in hours')
-    plt.ylabel('Electrical power in Kilowatt')
-    plt.title('Electrical Power Schedule of CityDistrict')
-    if do_plot:
-        plt.show()
-    return
-
-
-if __name__ == '__main__':
-    # Run example:
-    main(do_plot=True)
-```
-
-## Tutorial
-
-The pycity_scheduling package comes with several example, tutorial, and simple case study scripts in folder ./src/examples.
-
-The unit tests can be found in folder ./src/testing.
-
-
-Moreover, also check the pycity_base package's tutorials for the basic usage of the framework's core functionalities. 
-
-
-## License
-
-The pycity_scheduling package is released by the Institute for Automation of Complex Power Systems (ACS), E.ON Energy Research Center (E.ON ERC), RWTH Aachen University under the [MIT License](https://opensource.org/licenses/MIT).
-
-
-## Contact
-
-- Sebastian Schwarz, M.Sc. <sebastian.schwarz@eonerc.rwth-aachen.de>
-- Sebastian Alexander Uerlich, B.Sc. <sebastian.uerlich@rwth-aachen.de>
-- Univ.-Prof. Antonello Monti, Ph.D. <post_acs@eonerc.rwth-aachen.de>
-
-[Institute for Automation of Complex Power Systems (ACS)](http://www.acs.eonerc.rwth-aachen.de) \
-[E.ON Energy Research Center (E.ON ERC)](http://www.eonerc.rwth-aachen.de) \
-[RWTH Aachen University, Germany](http://www.rwth-aachen.de)
-
-
-<img src="https://fein-aachen.org/img/logos/eonerc.png"/>
+Metadata-Version: 2.1
+Name: pycity_scheduling
+Version: 1.2.1
+Summary: A Python framework for the development, testing, and assessment of optimization-basedpower scheduling algorithms for multi-energy systems in city districts
+Home-page: https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling
+Author: Institute for Automation of Complex Power Systems (ACS),E.ON Energy Research Center (E.ON ERC),RWTH Aachen University
+Author-email: post_acs@eonerc.rwth-aachen.de
+License: MIT
+Description: <img src="https://fein-aachen.org/img/logos/pycity_scheduling.png" width="150"/>
+        
+        # pycity_scheduling
+        
+        Python package pycity_scheduling is a framework for the effective development, testing, and assessment of optimization-based power scheduling algorithms for local multi-energy systems in city districts.
+        The framework primarily targets the elaboration of coordination concepts that can efficiently solve the power dispatch problem on the city district level.
+        Its target users are researchers in the field of smart grid applications and the deployment of operational flexibility for local energy systems.
+        
+        
+        ## Contribution
+        
+        1. Clone repository via SSH (`git clone git@git.rwth-aachen.de:acs/public/simulation/pycity_scheduling.git`) or clone repository via HTTPS (`git clone https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling.git`)
+        2. Open an issue at [https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling/-/issues](https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling/-/issues)
+        3. Checkout the development branch: `git checkout development` 
+        4. Update your local development branch (if necessary): `git pull origin development`
+        5. Create your feature/issue branch: `git checkout -b issueXY_explanation`
+        6. Commit your changes: `git commit -m "Add feature #XY"`
+        7. Push to the branch: `git push origin issueXY_explanation`
+        8. Submit a merge request from issueXY_explanation to development branch via [https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling/-/merge_requests](https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling/-/merge_requests)
+        9. Wait for approval or revision of the new implementations.
+        
+        ## Installation
+        
+        pycity_scheduling requires at least the following Python packages:
+        - numpy==1.19.5
+        - pandas==1.1.5
+        - matplotlib==3.3.4
+        - pyomo==5.7.3
+        - pycity_base==0.3.2
+        - pylint (optional)
+        - sphinx (optional)
+        - numpydoc (optional)
+        - pytest (optional)
+        
+        as well as the installation of at least one mathematical programming solver for convex and/or non-convex problems, which is supported by the [Pyomo](http://www.pyomo.org/) optimisation modelling library.
+        We recommend one of the following solvers:
+        
+        - [SCIP](https://www.scipopt.org/)
+        - [bonmin](https://github.com/coin-or/Bonmin)
+        - [Gurobi (gurobipy)](https://www.gurobi.com/products/gurobi-optimizer/) (default)
+        - [IBM ILOG CPLEX](https://www.ibm.com/products/ilog-cplex-optimization-studio)
+        
+        
+        ### Installation of pycity_scheduling
+        
+        The latest version of pycity_scheduling is v1.2.1.
+        
+        If all the abovementioned dependencies are installed, you should be able to install package pycity_scheduling via [PyPI](https://pypi.org/) (using Python version >= 3.7) as follows:
+        
+        `pip install pycity_scheduling`
+        
+        or to install in editable mode:
+        
+        `pip install -e '<your_path_to_pycity_scheduling_git_folder>'`
+        
+        or:
+        
+        `<path_to_your_python_binary> -m pip install -e '<your_path_to_pycity_scheduling_git_folder>/src'`
+        
+        The project can also be installed in editable mode directly from gitlab without the need for a previous download:
+        
+        `pip install -e "git+ssh://git.rwth-aachen.de:acs/public/simulation/pycity_scheduling.git"`
+        
+        or:
+        
+        `pip install --src <install_location> -e "git+ssh://git.rwth-aachen.de:acs/public/simulation/pycity_scheduling.git"`
+        
+        You can check if the installation has been successful by trying to import package pycity_scheduling into your Python environment.
+        This import should be possible without any errors.
+        
+        `import pycity_scheduling`
+        
+        
+        You may also try to run the pycity_scheduling's unit tests located in folder ./src/testing using Python module pytest.
+        
+        
+        ## Documentation
+        
+        The documentation for the latest pycity_scheduling release can be found in folder ./docs and on [this](https://acs.pages.rwth-aachen.de/public/simulation/pycity_scheduling/) GitLab page.
+        
+        For further information, please also visit the [FEIN Aachen association website](https://fein-aachen.org/en/projects/pycity_scheduling/).
+        
+        
+        ## Example usage
+        
+        ```python
+        import numpy as np
+        import matplotlib.pyplot as plt
+        
+        from pycity_scheduling.classes import *
+        from pycity_scheduling.algorithms import *
+        import pycity_scheduling.util.debug as debug
+        
+        
+        # This is a fundamental tutorial on how to use the pycity_scheduling package.
+        
+        
+        def main(do_plot=False):
+            print("\n\n------ Example 00: Fundamentals ------\n\n")
+        
+            # 1) Environment objects:
+        
+            # (Almost) every object within pycity_scheduling requires an environment. The environment object holds general data,
+            # which is valid for all objects within pycity_scheduling, such as time data, weather data or energy market prices.
+            # Therefore, all objects point to an environment. The first step is usually to generate such an environment.
+        
+            # Generate a timer object for the environment:
+            timer = Timer(step_size=3600, op_horizon=24, initial_date=(2015, 1, 1), initial_time=(0, 0, 0))
+        
+            # Generate a weather object for the environment:
+            weather = Weather(timer=timer)
+        
+            # Generate a price object for the environment:
+            price = Prices(timer=timer)
+        
+            # Generate the environment object:
+            environment = Environment(timer=timer, weather=weather, prices=price)
+        
+            # Now there is a distinct environment object with timer, weather and price data.
+            # We can use it to access different data of interest.
+        
+            # For example, print the current weekday:
+            print('Weekday:')
+            print(environment.timer.weekday)
+        
+            # For example, print the weather forecast for the outdoor temperature (only extract the first 10 timestep values):
+            print('\nOutdoor temperature forecast:')
+            print(environment.weather.getWeatherForecast(getTAmbient=True)[0][:10])
+        
+            # For example, print the energy spot market day-ahead prices:
+            print('\nDay-ahead spot market prices on 2015/01/01:')
+            print(environment.prices.da_prices)
+        
+            # 2) Buildings objects:
+        
+            # After defining the environment, different building objects should be created. In pycity_scheduling, buildings
+            # represent the different customers of the local energy system / city district under investigation.
+            # In general, buildings should also be understood in a more abstract way. For instance, a building object must not
+            # necessarily represent a building structure, as it would be the case for a wind energy converter.
+        
+            # Create a building object:
+            building = Building(environment=environment)
+        
+            # This building is assumed to be equipped with a building energy system and one apartment (=single-family house).
+            # In general, every building object can, however, hold up to N different apartments (=multi-family house).
+            apartment = Apartment(environment=environment)
+            bes = BuildingEnergySystem(environment=environment)
+        
+            building.addMultipleEntities([apartment, bes])
+        
+            # Every apartment usually possesses both electrical and thermal loads:
+            # The electrical load is added to the apartment as follows:
+            load = FixedLoad(environment=environment, method=1, annual_demand=3000)
+        
+            # Print and show the electrical power curve in Watt:
+            print('\nElectrical load in Watt:')
+            print(load.get_power(currentValues=False))
+            plt.plot(load.get_power(currentValues=False))
+            plt.xlabel('Time in hours')
+            plt.ylabel('Electrical power in Watt (fixed load)')
+            plt.title('Fixed load power curve')
+            if do_plot:
+                plt.show()
+        
+            # The thermal load is added to the apartment as follows:
+            space_heating = SpaceHeating(environment=environment, method=1, living_area=150, specific_demand=100)
+        
+            # Print and show space heating power curve in Watt:
+            print('\nSpace heating power curve in Watt:')
+            print(space_heating.get_power(currentValues=False))
+        
+            plt.plot(space_heating.get_power(currentValues=False))
+            plt.xlabel('Time in hours')
+            plt.ylabel('Thermal power in Watt (space heating)')
+            plt.title('Space heating power curve')
+            if do_plot:
+                plt.show()
+        
+            apartment.addMultipleEntities([load, space_heating])
+        
+            # The BuildingEnergySystem (BES) class is a 'container' for all kind of building energy systems (i.e., electrical
+            # and/or thermal assets). For example, we can add an electro-thermal heating system (such as a heatpump plus thermal
+            # energy storage) and a photovoltaic unit to a building's BES as done below. In pycity_scheduling all BES devices
+            # automatically come with basic scheduling models, which include the required Pyomo optimization variables and
+            # several optimization constraints.
+            eh = HeatPump(environment=environment, p_th_nom=16.0)
+            ths = ThermalHeatingStorage(environment=environment, e_th_max=20.0, soc_init=0.5, loss_factor=0)
+            pv = Photovoltaic(environment=environment, method=0, peak_power=8.0)
+        
+            bes.addMultipleDevices([eh, ths, pv])
+        
+            # Verify if the assets were added successfully (method getHasDevice):
+            print('\nBES has heatpump? : ', bes.getHasDevices(all_devices=False, heatpump=True)[0])
+            print('BES has thermal heating storage? : ', bes.getHasDevices(all_devices=False, ths=True)[0])
+            print('BES has photovoltaic? : ', bes.getHasDevices(all_devices=False, pv=True)[0])
+        
+            # 3) CityDistrict objects:
+        
+            # In pycity_scheduling, a group of buildings form a CityDistrict object. The CityDistrict is the object to be
+            # "provided" to a power scheduling algorithm later on. In other word, it encapsulates all buildings together with
+            # their local assets and it hence includes all the optimization problem information and data.
+        
+            # Create a city district object:
+            cd = CityDistrict(environment=environment)
+        
+            # Add the building from above to the city district at a certain position/coordinate (x, y).
+            cd.addEntity(entity=building, position=[0, 0])
+        
+            # Define and add three other buildings:
+            for i in range(3):
+                heat_demand = SpaceHeating(environment=environment, method=1, living_area=150, specific_demand=100)
+        
+                el_load_demand = FixedLoad(environment=environment, method=1, annual_demand=3000)
+        
+                pv = Photovoltaic(environment=environment, method=0, peak_power=5.0)
+                bl = Boiler(environment=environment, p_th_nom=24.0)
+        
+                ap = Apartment(environment=environment)
+                ap.addEntity(heat_demand)
+                ap.addEntity(el_load_demand)
+        
+                bes = BuildingEnergySystem(environment=environment)
+                bes.addDevice(pv)
+                bes.addDevice(bl)
+        
+                bd = Building(environment=environment)
+                bd.addEntity(entity=ap)
+                bd.addEntity(entity=bes)
+        
+                cd.addEntity(entity=bd, position=[0, i])
+        
+            # Print the city district information:
+            print('\nTotal number of buildings in city district:')
+            print(cd.get_nb_of_building_entities())
+            print("\nDetailed city district information:")
+            debug.print_district(cd, 3)
+        
+            # 4) Power scheduling:
+        
+            # The final step is to schedule the buildings/assets inside the city district subject to a certain optimization
+            # objective, which can be, for example, peak-shaving. The scheduling is then performed by the user by "passing"
+            # the city district object to a certain power scheduling algorithm.
+            # Here, the central optimization algorithm is used.
+        
+            # Set the city district / district operator objective and perform the power scheduling using the central
+            # optimization algorithm:
+            cd.set_objective("peak-shaving")
+            opt = CentralOptimization(cd)
+            opt.solve()
+        
+            # The scheduling results obtained from the algorithm run can be (temporally) stored as follows:
+            cd.copy_schedule("my_central_scheduling")
+        
+            # Print and show the scheduling result (city district power values for every time slot within the defined
+            # optimization horizon):
+            print("\nPower schedule of city district:")
+            print(list(cd.p_el_schedule))
+        
+            plt.plot(cd.p_el_schedule, drawstyle='steps')
+            plt.xlabel('Time in hours')
+            plt.ylabel('Electrical power in Kilowatt')
+            plt.title('Electrical Power Schedule of CityDistrict')
+            if do_plot:
+                plt.show()
+            return
+        
+        
+        if __name__ == '__main__':
+            # Run example:
+            main(do_plot=True)
+        ```
+        
+        ## Tutorial
+        
+        The pycity_scheduling package comes with several example, tutorial, and simple case study scripts in folder ./src/examples.
+        
+        The unit tests can be found in folder ./src/testing.
+        
+        
+        Moreover, also check the pycity_base package's tutorials for the basic usage of the framework's core functionalities. 
+        
+        
+        ## License
+        
+        The pycity_scheduling package is released by the Institute for Automation of Complex Power Systems (ACS), E.ON Energy Research Center (E.ON ERC), RWTH Aachen University under the [MIT License](https://opensource.org/licenses/MIT).
+        
+        
+        ## Contact
+        
+        - Sebastian Schwarz, M.Sc. <sebastian.schwarz@eonerc.rwth-aachen.de>
+        - Sebastian Alexander Uerlich, B.Sc. <sebastian.uerlich@rwth-aachen.de>
+        - Univ.-Prof. Antonello Monti, Ph.D. <post_acs@eonerc.rwth-aachen.de>
+        
+        [Institute for Automation of Complex Power Systems (ACS)](http://www.acs.eonerc.rwth-aachen.de) \
+        [E.ON Energy Research Center (E.ON ERC)](http://www.eonerc.rwth-aachen.de) \
+        [RWTH Aachen University, Germany](http://www.rwth-aachen.de)
+        
+        
+        <img src="https://fein-aachen.org/img/logos/eonerc.png"/>
+        
+Platform: any
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Scientific/Engineering
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: test
```

### Comparing `pycity_scheduling-1.2.0/setup.py` & `pycity_scheduling-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setuptools.setup(
     name="pycity_scheduling",
     description="A Python framework for the development, testing, and assessment of optimization-based"
                 "power scheduling algorithms for multi-energy systems in city districts",
-    version="1.2.0",
+    version="1.2.1",
     author="Institute for Automation of Complex Power Systems (ACS),"
            "E.ON Energy Research Center (E.ON ERC),"
            "RWTH Aachen University",
     author_email="post_acs@eonerc.rwth-aachen.de",
     url="https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling",
     license="MIT",
     packages=setuptools.find_packages(where="src"),
```

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/__init__.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/__init__.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/__init__.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/algorithm.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/algorithms/algorithm.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/central_optimization_algorithm.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/algorithms/central_optimization_algorithm.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/dual_decomposition_algorithm.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/algorithms/dual_decomposition_algorithm.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/dual_decomposition_algorithm_mpi.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/algorithms/dual_decomposition_algorithm_mpi.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/exchange_admm_algorithm.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/algorithms/exchange_admm_algorithm.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/exchange_admm_algorithm_mpi.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/algorithms/exchange_admm_algorithm_mpi.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/exchange_miqp_admm_algorithm.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/algorithms/exchange_miqp_admm_algorithm.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/exchange_miqp_admm_algorithm_mpi.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/algorithms/exchange_miqp_admm_algorithm_mpi.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/local_optimization_algorithm.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/algorithms/local_optimization_algorithm.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/stand_alone_optimization_algorithm.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/algorithms/stand_alone_optimization_algorithm.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/__init__.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/apartment.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/apartment.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/battery.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/battery.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/boiler.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/boiler.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/building.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/building.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/building_energy_system.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/building_energy_system.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/chiller.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/chiller.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/city_district.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/city_district.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/combined_heat_power.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/combined_heat_power.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/curtailable_load.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/curtailable_load.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/deferrable_load.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/deferrable_load.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/electric_heater.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/electric_heater.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/electric_vehicle.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/electric_vehicle.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/electrical_entity.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/electrical_entity.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/entity_container.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/entity_container.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/environment.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/environment.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/fixed_load.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/fixed_load.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/heat_pump.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/heat_pump.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/optimization_entity.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/optimization_entity.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/photovoltaic.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/photovoltaic.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/prices.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/prices.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/space_cooling.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/space_cooling.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/space_heating.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/space_heating.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/thermal_cooling_storage.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/thermal_cooling_storage.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/thermal_entity_cooling.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/thermal_entity_cooling.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/thermal_entity_heating.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/thermal_entity_heating.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/thermal_heating_storage.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/thermal_heating_storage.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/timer.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/timer.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/weather.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/weather.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/wind_energy_converter.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/classes/wind_energy_converter.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/constants.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/constants.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/data/TRY_2018.dat` & `pycity_scheduling-1.2.1/src/pycity_scheduling/data/TRY_2018.dat`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/data/__init__.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/data/co2_emissions_quarter-hour_2015.txt` & `pycity_scheduling-1.2.1/src/pycity_scheduling/data/co2_emissions_quarter-hour_2015.txt`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/data/da_prices_quarter-hour_2015.txt` & `pycity_scheduling-1.2.1/src/pycity_scheduling/data/da_prices_quarter-hour_2015.txt`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/data/ev_data.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/data/ev_data.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/data/tabula_data.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/data/tabula_data.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/__init__.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/case_studies/illustrative_code_example_cost_minimization_use_case_interactive.ipynb` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/case_studies/illustrative_code_example_cost_minimization_use_case_interactive.ipynb`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_00_fundamentals.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_00_fundamentals.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_01_algorithm_central.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_01_algorithm_central.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_02_algorithm_local.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_02_algorithm_local.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_03_algorithm_stand-alone.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_03_algorithm_stand-alone.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_04_algorithm_dual-decomposition.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_04_algorithm_dual-decomposition.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_05_algorithm_exchange-admm.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_05_algorithm_exchange-admm.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_06_algorithm_exchange-miqp-admm.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_06_algorithm_exchange-miqp-admm.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_07_algorithm_warmstart.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_07_algorithm_warmstart.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_08_algorithm_parallel_mpi.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_08_algorithm_parallel_mpi.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_09_objective_peak-shaving.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_09_objective_peak-shaving.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_10_objective_self-consumption.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_10_objective_self-consumption.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_11_objective_max-consumption.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_11_objective_max-consumption.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_12_objective_price.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_12_objective_price.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_13_objective_co2.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_13_objective_co2.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_14_objective_valley-filling.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_14_objective_valley-filling.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_15_district_generator.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_15_district_generator.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_16_scheduling_complex_city_district.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_16_scheduling_complex_city_district.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_17_district_flexibility_quantification.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_17_district_flexibility_quantification.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_18_scheduling_pv+battery_system.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_18_scheduling_pv+battery_system.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_19_scheduling_heating_and_cooling_loads.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_19_scheduling_heating_and_cooling_loads.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_20_scheduling_convex_vs._integer_mode.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_20_scheduling_convex_vs._integer_mode.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_21_scheduling_robust_optimization.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_21_scheduling_robust_optimization.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_22_post-processing_schedule_evaluation.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_22_post-processing_schedule_evaluation.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_23_post-processing_metrics_evaluation.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/examples/example_23_post-processing_metrics_evaluation.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/exceptions.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/exceptions.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/solvers.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/solvers.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/testing/__init__.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/__init__.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/testing/unit_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/test_algorithms.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/testing/unit_tests/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/test_all_classes.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/testing/unit_tests/test_all_classes.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/test_classes.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/testing/unit_tests/test_classes.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/test_examples.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/testing/unit_tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/test_util.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/testing/unit_tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/util/__init__.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/util/debug.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/util/debug.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/util/district_analyzer.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/util/district_analyzer.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/util/factory.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/util/factory.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/util/generic_constraints.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/util/generic_constraints.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/util/metric.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/util/metric.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/util/mpi_interface.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/util/mpi_interface.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/util/plot_schedules.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/util/plot_schedules.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling/util/write_schedules.py` & `pycity_scheduling-1.2.1/src/pycity_scheduling/util/write_schedules.py`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling.egg-info/PKG-INFO` & `pycity_scheduling-1.2.1/src/pycity_scheduling.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,322 +1,321 @@
 Metadata-Version: 2.1
 Name: pycity-scheduling
-Version: 1.2.0
+Version: 1.2.1
 Summary: A Python framework for the development, testing, and assessment of optimization-basedpower scheduling algorithms for multi-energy systems in city districts
 Home-page: https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling
 Author: Institute for Automation of Complex Power Systems (ACS),E.ON Energy Research Center (E.ON ERC),RWTH Aachen University
 Author-email: post_acs@eonerc.rwth-aachen.de
 License: MIT
+Description: <img src="https://fein-aachen.org/img/logos/pycity_scheduling.png" width="150"/>
+        
+        # pycity_scheduling
+        
+        Python package pycity_scheduling is a framework for the effective development, testing, and assessment of optimization-based power scheduling algorithms for local multi-energy systems in city districts.
+        The framework primarily targets the elaboration of coordination concepts that can efficiently solve the power dispatch problem on the city district level.
+        Its target users are researchers in the field of smart grid applications and the deployment of operational flexibility for local energy systems.
+        
+        
+        ## Contribution
+        
+        1. Clone repository via SSH (`git clone git@git.rwth-aachen.de:acs/public/simulation/pycity_scheduling.git`) or clone repository via HTTPS (`git clone https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling.git`)
+        2. Open an issue at [https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling/-/issues](https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling/-/issues)
+        3. Checkout the development branch: `git checkout development` 
+        4. Update your local development branch (if necessary): `git pull origin development`
+        5. Create your feature/issue branch: `git checkout -b issueXY_explanation`
+        6. Commit your changes: `git commit -m "Add feature #XY"`
+        7. Push to the branch: `git push origin issueXY_explanation`
+        8. Submit a merge request from issueXY_explanation to development branch via [https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling/-/merge_requests](https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling/-/merge_requests)
+        9. Wait for approval or revision of the new implementations.
+        
+        ## Installation
+        
+        pycity_scheduling requires at least the following Python packages:
+        - numpy==1.19.5
+        - pandas==1.1.5
+        - matplotlib==3.3.4
+        - pyomo==5.7.3
+        - pycity_base==0.3.2
+        - pylint (optional)
+        - sphinx (optional)
+        - numpydoc (optional)
+        - pytest (optional)
+        
+        as well as the installation of at least one mathematical programming solver for convex and/or non-convex problems, which is supported by the [Pyomo](http://www.pyomo.org/) optimisation modelling library.
+        We recommend one of the following solvers:
+        
+        - [SCIP](https://www.scipopt.org/)
+        - [bonmin](https://github.com/coin-or/Bonmin)
+        - [Gurobi (gurobipy)](https://www.gurobi.com/products/gurobi-optimizer/) (default)
+        - [IBM ILOG CPLEX](https://www.ibm.com/products/ilog-cplex-optimization-studio)
+        
+        
+        ### Installation of pycity_scheduling
+        
+        The latest version of pycity_scheduling is v1.2.1.
+        
+        If all the abovementioned dependencies are installed, you should be able to install package pycity_scheduling via [PyPI](https://pypi.org/) (using Python version >= 3.7) as follows:
+        
+        `pip install pycity_scheduling`
+        
+        or to install in editable mode:
+        
+        `pip install -e '<your_path_to_pycity_scheduling_git_folder>'`
+        
+        or:
+        
+        `<path_to_your_python_binary> -m pip install -e '<your_path_to_pycity_scheduling_git_folder>/src'`
+        
+        The project can also be installed in editable mode directly from gitlab without the need for a previous download:
+        
+        `pip install -e "git+ssh://git.rwth-aachen.de:acs/public/simulation/pycity_scheduling.git"`
+        
+        or:
+        
+        `pip install --src <install_location> -e "git+ssh://git.rwth-aachen.de:acs/public/simulation/pycity_scheduling.git"`
+        
+        You can check if the installation has been successful by trying to import package pycity_scheduling into your Python environment.
+        This import should be possible without any errors.
+        
+        `import pycity_scheduling`
+        
+        
+        You may also try to run the pycity_scheduling's unit tests located in folder ./src/testing using Python module pytest.
+        
+        
+        ## Documentation
+        
+        The documentation for the latest pycity_scheduling release can be found in folder ./docs and on [this](https://acs.pages.rwth-aachen.de/public/simulation/pycity_scheduling/) GitLab page.
+        
+        For further information, please also visit the [FEIN Aachen association website](https://fein-aachen.org/en/projects/pycity_scheduling/).
+        
+        
+        ## Example usage
+        
+        ```python
+        import numpy as np
+        import matplotlib.pyplot as plt
+        
+        from pycity_scheduling.classes import *
+        from pycity_scheduling.algorithms import *
+        import pycity_scheduling.util.debug as debug
+        
+        
+        # This is a fundamental tutorial on how to use the pycity_scheduling package.
+        
+        
+        def main(do_plot=False):
+            print("\n\n------ Example 00: Fundamentals ------\n\n")
+        
+            # 1) Environment objects:
+        
+            # (Almost) every object within pycity_scheduling requires an environment. The environment object holds general data,
+            # which is valid for all objects within pycity_scheduling, such as time data, weather data or energy market prices.
+            # Therefore, all objects point to an environment. The first step is usually to generate such an environment.
+        
+            # Generate a timer object for the environment:
+            timer = Timer(step_size=3600, op_horizon=24, initial_date=(2015, 1, 1), initial_time=(0, 0, 0))
+        
+            # Generate a weather object for the environment:
+            weather = Weather(timer=timer)
+        
+            # Generate a price object for the environment:
+            price = Prices(timer=timer)
+        
+            # Generate the environment object:
+            environment = Environment(timer=timer, weather=weather, prices=price)
+        
+            # Now there is a distinct environment object with timer, weather and price data.
+            # We can use it to access different data of interest.
+        
+            # For example, print the current weekday:
+            print('Weekday:')
+            print(environment.timer.weekday)
+        
+            # For example, print the weather forecast for the outdoor temperature (only extract the first 10 timestep values):
+            print('\nOutdoor temperature forecast:')
+            print(environment.weather.getWeatherForecast(getTAmbient=True)[0][:10])
+        
+            # For example, print the energy spot market day-ahead prices:
+            print('\nDay-ahead spot market prices on 2015/01/01:')
+            print(environment.prices.da_prices)
+        
+            # 2) Buildings objects:
+        
+            # After defining the environment, different building objects should be created. In pycity_scheduling, buildings
+            # represent the different customers of the local energy system / city district under investigation.
+            # In general, buildings should also be understood in a more abstract way. For instance, a building object must not
+            # necessarily represent a building structure, as it would be the case for a wind energy converter.
+        
+            # Create a building object:
+            building = Building(environment=environment)
+        
+            # This building is assumed to be equipped with a building energy system and one apartment (=single-family house).
+            # In general, every building object can, however, hold up to N different apartments (=multi-family house).
+            apartment = Apartment(environment=environment)
+            bes = BuildingEnergySystem(environment=environment)
+        
+            building.addMultipleEntities([apartment, bes])
+        
+            # Every apartment usually possesses both electrical and thermal loads:
+            # The electrical load is added to the apartment as follows:
+            load = FixedLoad(environment=environment, method=1, annual_demand=3000)
+        
+            # Print and show the electrical power curve in Watt:
+            print('\nElectrical load in Watt:')
+            print(load.get_power(currentValues=False))
+            plt.plot(load.get_power(currentValues=False))
+            plt.xlabel('Time in hours')
+            plt.ylabel('Electrical power in Watt (fixed load)')
+            plt.title('Fixed load power curve')
+            if do_plot:
+                plt.show()
+        
+            # The thermal load is added to the apartment as follows:
+            space_heating = SpaceHeating(environment=environment, method=1, living_area=150, specific_demand=100)
+        
+            # Print and show space heating power curve in Watt:
+            print('\nSpace heating power curve in Watt:')
+            print(space_heating.get_power(currentValues=False))
+        
+            plt.plot(space_heating.get_power(currentValues=False))
+            plt.xlabel('Time in hours')
+            plt.ylabel('Thermal power in Watt (space heating)')
+            plt.title('Space heating power curve')
+            if do_plot:
+                plt.show()
+        
+            apartment.addMultipleEntities([load, space_heating])
+        
+            # The BuildingEnergySystem (BES) class is a 'container' for all kind of building energy systems (i.e., electrical
+            # and/or thermal assets). For example, we can add an electro-thermal heating system (such as a heatpump plus thermal
+            # energy storage) and a photovoltaic unit to a building's BES as done below. In pycity_scheduling all BES devices
+            # automatically come with basic scheduling models, which include the required Pyomo optimization variables and
+            # several optimization constraints.
+            eh = HeatPump(environment=environment, p_th_nom=16.0)
+            ths = ThermalHeatingStorage(environment=environment, e_th_max=20.0, soc_init=0.5, loss_factor=0)
+            pv = Photovoltaic(environment=environment, method=0, peak_power=8.0)
+        
+            bes.addMultipleDevices([eh, ths, pv])
+        
+            # Verify if the assets were added successfully (method getHasDevice):
+            print('\nBES has heatpump? : ', bes.getHasDevices(all_devices=False, heatpump=True)[0])
+            print('BES has thermal heating storage? : ', bes.getHasDevices(all_devices=False, ths=True)[0])
+            print('BES has photovoltaic? : ', bes.getHasDevices(all_devices=False, pv=True)[0])
+        
+            # 3) CityDistrict objects:
+        
+            # In pycity_scheduling, a group of buildings form a CityDistrict object. The CityDistrict is the object to be
+            # "provided" to a power scheduling algorithm later on. In other word, it encapsulates all buildings together with
+            # their local assets and it hence includes all the optimization problem information and data.
+        
+            # Create a city district object:
+            cd = CityDistrict(environment=environment)
+        
+            # Add the building from above to the city district at a certain position/coordinate (x, y).
+            cd.addEntity(entity=building, position=[0, 0])
+        
+            # Define and add three other buildings:
+            for i in range(3):
+                heat_demand = SpaceHeating(environment=environment, method=1, living_area=150, specific_demand=100)
+        
+                el_load_demand = FixedLoad(environment=environment, method=1, annual_demand=3000)
+        
+                pv = Photovoltaic(environment=environment, method=0, peak_power=5.0)
+                bl = Boiler(environment=environment, p_th_nom=24.0)
+        
+                ap = Apartment(environment=environment)
+                ap.addEntity(heat_demand)
+                ap.addEntity(el_load_demand)
+        
+                bes = BuildingEnergySystem(environment=environment)
+                bes.addDevice(pv)
+                bes.addDevice(bl)
+        
+                bd = Building(environment=environment)
+                bd.addEntity(entity=ap)
+                bd.addEntity(entity=bes)
+        
+                cd.addEntity(entity=bd, position=[0, i])
+        
+            # Print the city district information:
+            print('\nTotal number of buildings in city district:')
+            print(cd.get_nb_of_building_entities())
+            print("\nDetailed city district information:")
+            debug.print_district(cd, 3)
+        
+            # 4) Power scheduling:
+        
+            # The final step is to schedule the buildings/assets inside the city district subject to a certain optimization
+            # objective, which can be, for example, peak-shaving. The scheduling is then performed by the user by "passing"
+            # the city district object to a certain power scheduling algorithm.
+            # Here, the central optimization algorithm is used.
+        
+            # Set the city district / district operator objective and perform the power scheduling using the central
+            # optimization algorithm:
+            cd.set_objective("peak-shaving")
+            opt = CentralOptimization(cd)
+            opt.solve()
+        
+            # The scheduling results obtained from the algorithm run can be (temporally) stored as follows:
+            cd.copy_schedule("my_central_scheduling")
+        
+            # Print and show the scheduling result (city district power values for every time slot within the defined
+            # optimization horizon):
+            print("\nPower schedule of city district:")
+            print(list(cd.p_el_schedule))
+        
+            plt.plot(cd.p_el_schedule, drawstyle='steps')
+            plt.xlabel('Time in hours')
+            plt.ylabel('Electrical power in Kilowatt')
+            plt.title('Electrical Power Schedule of CityDistrict')
+            if do_plot:
+                plt.show()
+            return
+        
+        
+        if __name__ == '__main__':
+            # Run example:
+            main(do_plot=True)
+        ```
+        
+        ## Tutorial
+        
+        The pycity_scheduling package comes with several example, tutorial, and simple case study scripts in folder ./src/examples.
+        
+        The unit tests can be found in folder ./src/testing.
+        
+        
+        Moreover, also check the pycity_base package's tutorials for the basic usage of the framework's core functionalities. 
+        
+        
+        ## License
+        
+        The pycity_scheduling package is released by the Institute for Automation of Complex Power Systems (ACS), E.ON Energy Research Center (E.ON ERC), RWTH Aachen University under the [MIT License](https://opensource.org/licenses/MIT).
+        
+        
+        ## Contact
+        
+        - Sebastian Schwarz, M.Sc. <sebastian.schwarz@eonerc.rwth-aachen.de>
+        - Sebastian Alexander Uerlich, B.Sc. <sebastian.uerlich@rwth-aachen.de>
+        - Univ.-Prof. Antonello Monti, Ph.D. <post_acs@eonerc.rwth-aachen.de>
+        
+        [Institute for Automation of Complex Power Systems (ACS)](http://www.acs.eonerc.rwth-aachen.de) \
+        [E.ON Energy Research Center (E.ON ERC)](http://www.eonerc.rwth-aachen.de) \
+        [RWTH Aachen University, Germany](http://www.rwth-aachen.de)
+        
+        
+        <img src="https://fein-aachen.org/img/logos/eonerc.png"/>
+        
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
-License-File: LICENSE.txt
-
-<img src="https://fein-aachen.org/img/logos/pycity_scheduling.png" width="150"/>
-
-# pycity_scheduling
-
-Python package pycity_scheduling is a framework for the effective development, testing, and assessment of optimization-based power scheduling algorithms for local multi-energy systems in city districts.
-The framework primarily targets the elaboration of coordination concepts that can efficiently solve the power dispatch problem on the city district level.
-Its target users are researchers in the field of smart grid applications and the deployment of operational flexibility for local energy systems.
-
-
-## Contribution
-
-1. Clone repository via SSH (`git clone git@git.rwth-aachen.de:acs/public/simulation/pycity_scheduling.git`) or clone repository via HTTPS (`git clone https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling.git`)
-2. Open an issue at [https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling/-/issues](https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling/-/issues)
-3. Checkout the development branch: `git checkout development` 
-4. Update your local development branch (if necessary): `git pull origin development`
-5. Create your feature/issue branch: `git checkout -b issueXY_explanation`
-6. Commit your changes: `git commit -m "Add feature #XY"`
-7. Push to the branch: `git push origin issueXY_explanation`
-8. Submit a merge request from issueXY_explanation to development branch via [https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling/-/merge_requests](https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling/-/merge_requests)
-9. Wait for approval or revision of the new implementations.
-
-## Installation
-
-pycity_scheduling requires at least the following Python packages:
-- numpy==1.19.5
-- pandas==1.1.5
-- matplotlib==3.3.4
-- pyomo==5.7.3
-- pycity_base==0.3.2
-- pylint (optional)
-- sphinx (optional)
-- numpydoc (optional)
-- pytest (optional)
-
-as well as the installation of at least one mathematical programming solver for convex and/or non-convex problems, which is supported by the [Pyomo](http://www.pyomo.org/) optimisation modelling library.
-We recommend one of the following solvers:
-
-- [SCIP](https://www.scipopt.org/)
-- [bonmin](https://github.com/coin-or/Bonmin)
-- [Gurobi (gurobipy)](https://www.gurobi.com/products/gurobi-optimizer/) (default)
-- [IBM ILOG CPLEX](https://www.ibm.com/products/ilog-cplex-optimization-studio)
-
-
-### Installation of pycity_scheduling
-
-The latest version of pycity_scheduling is v1.2.0.
-
-If all the abovementioned dependencies are installed, you should be able to install package pycity_scheduling via [PyPI](https://pypi.org/) (using Python version >= 3.7) as follows:
-
-`pip install pycity_scheduling`
-
-or to install in editable mode:
-
-`pip install -e '<your_path_to_pycity_scheduling_git_folder>'`
-
-or:
-
-`<path_to_your_python_binary> -m pip install -e '<your_path_to_pycity_scheduling_git_folder>/src'`
-
-The project can also be installed in editable mode directly from gitlab without the need for a previous download:
-
-`pip install -e "git+ssh://git.rwth-aachen.de:acs/public/simulation/pycity_scheduling.git"`
-
-or:
-
-`pip install --src <install_location> -e "git+ssh://git.rwth-aachen.de:acs/public/simulation/pycity_scheduling.git"`
-
-You can check if the installation has been successful by trying to import package pycity_scheduling into your Python environment.
-This import should be possible without any errors.
-
-`import pycity_scheduling`
-
-
-You may also try to run the pycity_scheduling's unit tests located in folder ./src/testing using Python module pytest.
-
-
-## Documentation
-
-The documentation for the latest pycity_scheduling release can be found in folder ./docs and on [this](https://acs.pages.rwth-aachen.de/public/simulation/pycity_scheduling/) GitLab page.
-
-For further information, please also visit the [FEIN Aachen association website](https://fein-aachen.org/en/projects/pycity_scheduling/).
-
-
-## Example usage
-
-```python
-import numpy as np
-import matplotlib.pyplot as plt
-
-from pycity_scheduling.classes import *
-from pycity_scheduling.algorithms import *
-import pycity_scheduling.util.debug as debug
-
-
-# This is a fundamental tutorial on how to use the pycity_scheduling package.
-
-
-def main(do_plot=False):
-    print("\n\n------ Example 00: Fundamentals ------\n\n")
-
-    # 1) Environment objects:
-
-    # (Almost) every object within pycity_scheduling requires an environment. The environment object holds general data,
-    # which is valid for all objects within pycity_scheduling, such as time data, weather data or energy market prices.
-    # Therefore, all objects point to an environment. The first step is usually to generate such an environment.
-
-    # Generate a timer object for the environment:
-    timer = Timer(step_size=3600, op_horizon=24, initial_date=(2015, 1, 1), initial_time=(0, 0, 0))
-
-    # Generate a weather object for the environment:
-    weather = Weather(timer=timer)
-
-    # Generate a price object for the environment:
-    price = Prices(timer=timer)
-
-    # Generate the environment object:
-    environment = Environment(timer=timer, weather=weather, prices=price)
-
-    # Now there is a distinct environment object with timer, weather and price data.
-    # We can use it to access different data of interest.
-
-    # For example, print the current weekday:
-    print('Weekday:')
-    print(environment.timer.weekday)
-
-    # For example, print the weather forecast for the outdoor temperature (only extract the first 10 timestep values):
-    print('\nOutdoor temperature forecast:')
-    print(environment.weather.getWeatherForecast(getTAmbient=True)[0][:10])
-
-    # For example, print the energy spot market day-ahead prices:
-    print('\nDay-ahead spot market prices on 2015/01/01:')
-    print(environment.prices.da_prices)
-
-    # 2) Buildings objects:
-
-    # After defining the environment, different building objects should be created. In pycity_scheduling, buildings
-    # represent the different customers of the local energy system / city district under investigation.
-    # In general, buildings should also be understood in a more abstract way. For instance, a building object must not
-    # necessarily represent a building structure, as it would be the case for a wind energy converter.
-
-    # Create a building object:
-    building = Building(environment=environment)
-
-    # This building is assumed to be equipped with a building energy system and one apartment (=single-family house).
-    # In general, every building object can, however, hold up to N different apartments (=multi-family house).
-    apartment = Apartment(environment=environment)
-    bes = BuildingEnergySystem(environment=environment)
-
-    building.addMultipleEntities([apartment, bes])
-
-    # Every apartment usually possesses both electrical and thermal loads:
-    # The electrical load is added to the apartment as follows:
-    load = FixedLoad(environment=environment, method=1, annual_demand=3000)
-
-    # Print and show the electrical power curve in Watt:
-    print('\nElectrical load in Watt:')
-    print(load.get_power(currentValues=False))
-    plt.plot(load.get_power(currentValues=False))
-    plt.xlabel('Time in hours')
-    plt.ylabel('Electrical power in Watt (fixed load)')
-    plt.title('Fixed load power curve')
-    if do_plot:
-        plt.show()
-
-    # The thermal load is added to the apartment as follows:
-    space_heating = SpaceHeating(environment=environment, method=1, living_area=150, specific_demand=100)
-
-    # Print and show space heating power curve in Watt:
-    print('\nSpace heating power curve in Watt:')
-    print(space_heating.get_power(currentValues=False))
-
-    plt.plot(space_heating.get_power(currentValues=False))
-    plt.xlabel('Time in hours')
-    plt.ylabel('Thermal power in Watt (space heating)')
-    plt.title('Space heating power curve')
-    if do_plot:
-        plt.show()
-
-    apartment.addMultipleEntities([load, space_heating])
-
-    # The BuildingEnergySystem (BES) class is a 'container' for all kind of building energy systems (i.e., electrical
-    # and/or thermal assets). For example, we can add an electro-thermal heating system (such as a heatpump plus thermal
-    # energy storage) and a photovoltaic unit to a building's BES as done below. In pycity_scheduling all BES devices
-    # automatically come with basic scheduling models, which include the required Pyomo optimization variables and
-    # several optimization constraints.
-    eh = HeatPump(environment=environment, p_th_nom=16.0)
-    ths = ThermalHeatingStorage(environment=environment, e_th_max=20.0, soc_init=0.5, loss_factor=0)
-    pv = Photovoltaic(environment=environment, method=0, peak_power=8.0)
-
-    bes.addMultipleDevices([eh, ths, pv])
-
-    # Verify if the assets were added successfully (method getHasDevice):
-    print('\nBES has heatpump? : ', bes.getHasDevices(all_devices=False, heatpump=True)[0])
-    print('BES has thermal heating storage? : ', bes.getHasDevices(all_devices=False, ths=True)[0])
-    print('BES has photovoltaic? : ', bes.getHasDevices(all_devices=False, pv=True)[0])
-
-    # 3) CityDistrict objects:
-
-    # In pycity_scheduling, a group of buildings form a CityDistrict object. The CityDistrict is the object to be
-    # "provided" to a power scheduling algorithm later on. In other word, it encapsulates all buildings together with
-    # their local assets and it hence includes all the optimization problem information and data.
-
-    # Create a city district object:
-    cd = CityDistrict(environment=environment)
-
-    # Add the building from above to the city district at a certain position/coordinate (x, y).
-    cd.addEntity(entity=building, position=[0, 0])
-
-    # Define and add three other buildings:
-    for i in range(3):
-        heat_demand = SpaceHeating(environment=environment, method=1, living_area=150, specific_demand=100)
-
-        el_load_demand = FixedLoad(environment=environment, method=1, annual_demand=3000)
-
-        pv = Photovoltaic(environment=environment, method=0, peak_power=5.0)
-        bl = Boiler(environment=environment, p_th_nom=24.0)
-
-        ap = Apartment(environment=environment)
-        ap.addEntity(heat_demand)
-        ap.addEntity(el_load_demand)
-
-        bes = BuildingEnergySystem(environment=environment)
-        bes.addDevice(pv)
-        bes.addDevice(bl)
-
-        bd = Building(environment=environment)
-        bd.addEntity(entity=ap)
-        bd.addEntity(entity=bes)
-
-        cd.addEntity(entity=bd, position=[0, i])
-
-    # Print the city district information:
-    print('\nTotal number of buildings in city district:')
-    print(cd.get_nb_of_building_entities())
-    print("\nDetailed city district information:")
-    debug.print_district(cd, 3)
-
-    # 4) Power scheduling:
-
-    # The final step is to schedule the buildings/assets inside the city district subject to a certain optimization
-    # objective, which can be, for example, peak-shaving. The scheduling is then performed by the user by "passing"
-    # the city district object to a certain power scheduling algorithm.
-    # Here, the central optimization algorithm is used.
-
-    # Set the city district / district operator objective and perform the power scheduling using the central
-    # optimization algorithm:
-    cd.set_objective("peak-shaving")
-    opt = CentralOptimization(cd)
-    opt.solve()
-
-    # The scheduling results obtained from the algorithm run can be (temporally) stored as follows:
-    cd.copy_schedule("my_central_scheduling")
-
-    # Print and show the scheduling result (city district power values for every time slot within the defined
-    # optimization horizon):
-    print("\nPower schedule of city district:")
-    print(list(cd.p_el_schedule))
-
-    plt.plot(cd.p_el_schedule, drawstyle='steps')
-    plt.xlabel('Time in hours')
-    plt.ylabel('Electrical power in Kilowatt')
-    plt.title('Electrical Power Schedule of CityDistrict')
-    if do_plot:
-        plt.show()
-    return
-
-
-if __name__ == '__main__':
-    # Run example:
-    main(do_plot=True)
-```
-
-## Tutorial
-
-The pycity_scheduling package comes with several example, tutorial, and simple case study scripts in folder ./src/examples.
-
-The unit tests can be found in folder ./src/testing.
-
-
-Moreover, also check the pycity_base package's tutorials for the basic usage of the framework's core functionalities. 
-
-
-## License
-
-The pycity_scheduling package is released by the Institute for Automation of Complex Power Systems (ACS), E.ON Energy Research Center (E.ON ERC), RWTH Aachen University under the [MIT License](https://opensource.org/licenses/MIT).
-
-
-## Contact
-
-- Sebastian Schwarz, M.Sc. <sebastian.schwarz@eonerc.rwth-aachen.de>
-- Sebastian Alexander Uerlich, B.Sc. <sebastian.uerlich@rwth-aachen.de>
-- Univ.-Prof. Antonello Monti, Ph.D. <post_acs@eonerc.rwth-aachen.de>
-
-[Institute for Automation of Complex Power Systems (ACS)](http://www.acs.eonerc.rwth-aachen.de) \
-[E.ON Energy Research Center (E.ON ERC)](http://www.eonerc.rwth-aachen.de) \
-[RWTH Aachen University, Germany](http://www.rwth-aachen.de)
-
-
-<img src="https://fein-aachen.org/img/logos/eonerc.png"/>
```

### Comparing `pycity_scheduling-1.2.0/src/pycity_scheduling.egg-info/SOURCES.txt` & `pycity_scheduling-1.2.1/src/pycity_scheduling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

