# Comparing `tmp/python-microgrid-1.3.0.tar.gz` & `tmp/python-microgrid-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-microgrid-1.3.0.tar", last modified: Thu Apr  6 17:27:14 2023, max compression
+gzip compressed data, was "python-microgrid-1.4.0.tar", last modified: Tue May 30 20:36:29 2023, max compression
```

## Comparing `python-microgrid-1.3.0.tar` & `python-microgrid-1.4.0.tar`

### file list

```diff
@@ -1,363 +1,373 @@
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.799322 python-microgrid-1.3.0/
--rw-r--r--   0 ahalev     (502) staff       (20)     7652 2020-08-13 19:47:38.000000 python-microgrid-1.3.0/LICENSE
--rw-r--r--   0 ahalev     (502) staff       (20)       31 2023-04-05 06:27:25.000000 python-microgrid-1.3.0/MANIFEST.in
--rw-r--r--   0 ahalev     (502) staff       (20)     7369 2023-04-06 17:27:14.799445 python-microgrid-1.3.0/PKG-INFO
--rw-r--r--   0 ahalev     (502) staff       (20)     6760 2023-04-06 17:21:27.000000 python-microgrid-1.3.0/README.md
--rw-r--r--   0 ahalev     (502) staff       (20)      191 2023-03-29 00:42:14.000000 python-microgrid-1.3.0/pyproject.toml
--rw-r--r--   0 ahalev     (502) staff       (20)      124 2023-04-06 17:27:14.799832 python-microgrid-1.3.0/setup.cfg
--rw-r--r--   0 ahalev     (502) staff       (20)     1645 2023-04-06 17:22:47.000000 python-microgrid-1.3.0/setup.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.546870 python-microgrid-1.3.0/src/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.549733 python-microgrid-1.3.0/src/pymgrid/
--rw-r--r--   0 ahalev     (502) staff       (20)    26580 2023-02-11 01:32:23.000000 python-microgrid-1.3.0/src/pymgrid/MicrogridGenerator.py
--rw-r--r--   0 ahalev     (502) staff       (20)      513 2023-04-01 21:07:37.000000 python-microgrid-1.3.0/src/pymgrid/__init__.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.549981 python-microgrid-1.3.0/src/pymgrid/_deprecated/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.571117 python-microgrid-1.3.0/src/pymgrid/_deprecated/Environments/
--rw-r--r--   0 ahalev     (502) staff       (20)    21520 2022-12-02 00:01:20.000000 python-microgrid-1.3.0/src/pymgrid/_deprecated/Environments/Environment.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1991 2022-12-02 00:01:20.000000 python-microgrid-1.3.0/src/pymgrid/_deprecated/Environments/Preprocessing.py
--rw-r--r--   0 ahalev     (502) staff       (20)        1 2022-12-02 00:01:20.000000 python-microgrid-1.3.0/src/pymgrid/_deprecated/Environments/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)    27816 2022-12-17 17:21:34.000000 python-microgrid-1.3.0/src/pymgrid/_deprecated/Environments/pymgrid_csca.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1616 2022-12-02 00:01:20.000000 python-microgrid-1.3.0/src/pymgrid/_deprecated/Environments/pymgrid_csca_old.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1614 2022-12-02 00:01:20.000000 python-microgrid-1.3.0/src/pymgrid/_deprecated/Environments/pymgrid_csda.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1979 2022-12-02 00:01:20.000000 python-microgrid-1.3.0/src/pymgrid/_deprecated/Environments/pymgrid_cspla.py
--rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-12-02 00:01:20.000000 python-microgrid-1.3.0/src/pymgrid/_deprecated/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)    55258 2022-12-02 00:01:20.000000 python-microgrid-1.3.0/src/pymgrid/_deprecated/non_modular_microgrid.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.571725 python-microgrid-1.3.0/src/pymgrid/algos/
--rw-r--r--   0 ahalev     (502) staff       (20)    17127 2022-12-17 17:21:34.000000 python-microgrid-1.3.0/src/pymgrid/algos/Control.py
--rw-r--r--   0 ahalev     (502) staff       (20)       82 2022-12-10 02:06:45.000000 python-microgrid-1.3.0/src/pymgrid/algos/__init__.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.572083 python-microgrid-1.3.0/src/pymgrid/algos/mpc/
--rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-10-25 19:17:19.000000 python-microgrid-1.3.0/src/pymgrid/algos/mpc/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)    43966 2023-03-30 03:14:25.000000 python-microgrid-1.3.0/src/pymgrid/algos/mpc/mpc.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.573469 python-microgrid-1.3.0/src/pymgrid/algos/priority_list/
--rw-r--r--   0 ahalev     (502) staff       (20)       99 2022-12-17 03:06:50.000000 python-microgrid-1.3.0/src/pymgrid/algos/priority_list/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)     7099 2023-03-29 21:20:42.000000 python-microgrid-1.3.0/src/pymgrid/algos/priority_list/priority_list.py
--rw-r--r--   0 ahalev     (502) staff       (20)     2783 2023-02-04 17:02:47.000000 python-microgrid-1.3.0/src/pymgrid/algos/priority_list/priority_list_element.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.574259 python-microgrid-1.3.0/src/pymgrid/algos/rbc/
--rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-12-02 00:00:07.000000 python-microgrid-1.3.0/src/pymgrid/algos/rbc/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)    13272 2022-12-17 03:06:50.000000 python-microgrid-1.3.0/src/pymgrid/algos/rbc/_nonmodular_rbc.py
--rw-r--r--   0 ahalev     (502) staff       (20)     4155 2023-04-05 05:54:52.000000 python-microgrid-1.3.0/src/pymgrid/algos/rbc/rbc.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.574820 python-microgrid-1.3.0/src/pymgrid/algos/saa/
--rw-r--r--   0 ahalev     (502) staff       (20)       43 2022-10-25 19:17:19.000000 python-microgrid-1.3.0/src/pymgrid/algos/saa/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)     7336 2022-12-17 06:16:17.000000 python-microgrid-1.3.0/src/pymgrid/algos/saa/saa.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.575915 python-microgrid-1.3.0/src/pymgrid/convert/
--rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-12-02 00:01:20.000000 python-microgrid-1.3.0/src/pymgrid/convert/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)      367 2022-11-30 07:09:17.000000 python-microgrid-1.3.0/src/pymgrid/convert/conversion_test_sandbox.py
--rw-r--r--   0 ahalev     (502) staff       (20)     2635 2022-12-02 00:01:20.000000 python-microgrid-1.3.0/src/pymgrid/convert/convert.py
--rw-r--r--   0 ahalev     (502) staff       (20)     4368 2022-12-10 02:06:16.000000 python-microgrid-1.3.0/src/pymgrid/convert/get_module.py
--rw-r--r--   0 ahalev     (502) staff       (20)    10537 2022-12-10 02:06:16.000000 python-microgrid-1.3.0/src/pymgrid/convert/to_nonmodular_ops.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.576229 python-microgrid-1.3.0/src/pymgrid/data/
--rw-r--r--   0 ahalev     (502) staff       (20)        0 2020-10-27 20:16:24.000000 python-microgrid-1.3.0/src/pymgrid/data/__init__.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.576387 python-microgrid-1.3.0/src/pymgrid/data/co2/
--rw-r--r--   0 ahalev     (502) staff       (20)        1 2020-10-27 20:16:24.000000 python-microgrid-1.3.0/src/pymgrid/data/co2/__init__.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.577879 python-microgrid-1.3.0/src/pymgrid/data/load/
--rw-r--r--   0 ahalev     (502) staff       (20)        0 2020-10-27 20:16:24.000000 python-microgrid-1.3.0/src/pymgrid/data/load/__init__.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.577997 python-microgrid-1.3.0/src/pymgrid/data/pv/
--rw-r--r--   0 ahalev     (502) staff       (20)        0 2020-10-27 20:16:24.000000 python-microgrid-1.3.0/src/pymgrid/data/pv/__init__.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.578829 python-microgrid-1.3.0/src/pymgrid/data/scenario/
--rw-r--r--   0 ahalev     (502) staff       (20)     6148 2022-11-09 16:21:41.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/.DS_Store
--rw-r--r--   0 ahalev     (502) staff       (20)        1 2020-10-27 20:16:24.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/__init__.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.545585 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.592910 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/
--rw-r--r--   0 ahalev     (502) staff       (20)     6148 2022-12-17 18:41:28.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/.DS_Store
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.612254 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/
--rw-r--r--   0 ahalev     (502) staff       (20)     6148 2022-12-17 18:42:51.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/.DS_Store
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.612661 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/
--rw-r--r--   0 ahalev     (502) staff       (20)     6148 2022-12-17 18:42:57.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/.DS_Store
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.612880 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    71000 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.613517 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    95750 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.614114 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    41119 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2066 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/microgrid_0.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.614401 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.538019 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.538179 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.614718 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    70450 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.615293 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    98740 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.615873 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    43703 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2621 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/microgrid_1.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.616328 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.538372 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.538540 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.616776 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    71849 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.617158 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    99947 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.618289 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    40530 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2640 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/microgrid_10.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.619192 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.538703 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.538863 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.622574 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    70730 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.623282 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    98933 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.623824 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    44288 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2058 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/microgrid_11.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.624165 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.539022 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.539176 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.624615 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    71849 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.625119 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)   101899 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.625599 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    40454 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2052 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/microgrid_12.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.626129 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.539349 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.539529 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.626574 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    69997 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.627055 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)   101801 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.627792 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    41997 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2613 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/microgrid_13.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.628274 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.539718 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.539881 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.628674 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    70730 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.629367 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    92053 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.630029 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    43518 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2054 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/microgrid_14.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.630322 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.540040 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.540139 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.688694 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    98126 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.691578 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    43802 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2143 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/microgrid_15.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.692014 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.540324 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.540514 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.692649 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    71849 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.693725 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    92018 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.694431 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    43220 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2100 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/microgrid_16.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.694751 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.540686 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.540785 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.695176 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    91889 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.695624 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    41880 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2157 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/microgrid_17.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.695972 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.541040 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.541260 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.697933 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    69997 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.698587 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)   101812 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.699011 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    42455 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2611 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/microgrid_18.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.699425 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.541462 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.541573 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.699760 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    98334 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.700280 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    41498 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2166 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/microgrid_19.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.700558 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.541771 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.541872 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.701001 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    98535 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.701582 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    42761 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2151 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/microgrid_2.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.701877 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.542039 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.542138 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.702319 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)   100312 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.702895 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    43495 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2141 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/microgrid_20.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.703263 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.542300 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.542396 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.703853 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)   100892 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.704613 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    43999 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2151 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/microgrid_21.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.705046 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.542553 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.542809 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.706159 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    69997 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.708186 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    99857 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.710966 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    42241 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2617 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/microgrid_22.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.711275 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.543005 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.543131 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.711710 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    97388 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.712267 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    42142 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2133 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/microgrid_23.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.712679 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.543332 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.543521 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.713147 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    70790 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.714467 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    91809 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.716053 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    42978 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2628 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/microgrid_24.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.716977 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.543725 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.543828 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.718601 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)   100230 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.720486 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    42513 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2140 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/microgrid_3.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.722084 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.544011 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.544202 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.722595 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    69997 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.724968 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    99793 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.726951 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    42889 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2051 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/microgrid_4.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.729677 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.544375 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.544482 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.731556 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    98745 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.736442 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    38378 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2146 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/microgrid_5.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.737024 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.544684 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.544869 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.737377 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    69997 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.737998 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)   100276 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.743811 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    43091 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2090 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/microgrid_6.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.745282 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.545055 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.545171 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.745725 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    99461 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.746101 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    42132 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2132 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/microgrid_7.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.747634 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.545328 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.545520 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.748073 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    72045 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.748666 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    92074 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.749284 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    41768 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2640 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/microgrid_8.yaml
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.749627 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.545692 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.545875 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.749928 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/GridModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    71462 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/GridModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.750470 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/LoadModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    98674 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/LoadModule/time_series.csv.gz
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.751012 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/RenewableModule/
--rw-r--r--   0 ahalev     (502) staff       (20)    44237 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/RenewableModule/time_series.csv.gz
--rw-r--r--   0 ahalev     (502) staff       (20)     2657 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/microgrid_9.yaml
--rw-r--r--   0 ahalev     (502) staff       (20)  7790780 2022-11-09 16:19:50.000000 python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25.pkl
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.751310 python-microgrid-1.3.0/src/pymgrid/envs/
--rw-r--r--   0 ahalev     (502) staff       (20)      110 2022-12-02 00:01:20.000000 python-microgrid-1.3.0/src/pymgrid/envs/__init__.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.752506 python-microgrid-1.3.0/src/pymgrid/envs/base/
--rw-r--r--   0 ahalev     (502) staff       (20)       35 2022-12-02 00:01:20.000000 python-microgrid-1.3.0/src/pymgrid/envs/base/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)    10729 2023-04-01 21:07:37.000000 python-microgrid-1.3.0/src/pymgrid/envs/base/base.py
--rw-r--r--   0 ahalev     (502) staff       (20)      400 2022-12-02 00:01:20.000000 python-microgrid-1.3.0/src/pymgrid/envs/base/skip_init.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.753197 python-microgrid-1.3.0/src/pymgrid/envs/continuous/
--rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-12-02 00:01:20.000000 python-microgrid-1.3.0/src/pymgrid/envs/continuous/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)     3565 2023-03-03 20:03:15.000000 python-microgrid-1.3.0/src/pymgrid/envs/continuous/continuous.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.774155 python-microgrid-1.3.0/src/pymgrid/envs/discrete/
--rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-12-02 00:01:20.000000 python-microgrid-1.3.0/src/pymgrid/envs/discrete/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)     5297 2023-03-22 08:15:22.000000 python-microgrid-1.3.0/src/pymgrid/envs/discrete/discrete.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.775499 python-microgrid-1.3.0/src/pymgrid/forecast/
--rw-r--r--   0 ahalev     (502) staff       (20)      119 2022-12-10 02:06:16.000000 python-microgrid-1.3.0/src/pymgrid/forecast/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)    14669 2023-02-22 02:13:22.000000 python-microgrid-1.3.0/src/pymgrid/forecast/forecaster.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.780183 python-microgrid-1.3.0/src/pymgrid/microgrid/
--rw-r--r--   0 ahalev     (502) staff       (20)       55 2022-12-02 00:01:20.000000 python-microgrid-1.3.0/src/pymgrid/microgrid/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)      784 2022-11-23 02:52:46.000000 python-microgrid-1.3.0/src/pymgrid/microgrid/convert_scenario_sandbox.py
--rw-r--r--   0 ahalev     (502) staff       (20)    38967 2023-04-05 05:54:52.000000 python-microgrid-1.3.0/src/pymgrid/microgrid/microgrid.py
--rw-r--r--   0 ahalev     (502) staff       (20)     4283 2022-11-23 02:52:46.000000 python-microgrid-1.3.0/src/pymgrid/microgrid/modular_microgrid_sandbox.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.781732 python-microgrid-1.3.0/src/pymgrid/microgrid/reward_shaping/
--rw-r--r--   0 ahalev     (502) staff       (20)      116 2023-03-18 01:38:19.000000 python-microgrid-1.3.0/src/pymgrid/microgrid/reward_shaping/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)      548 2023-03-18 01:38:19.000000 python-microgrid-1.3.0/src/pymgrid/microgrid/reward_shaping/base.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1190 2023-03-21 00:34:25.000000 python-microgrid-1.3.0/src/pymgrid/microgrid/reward_shaping/battery_discharge_shaper.py
--rw-r--r--   0 ahalev     (502) staff       (20)      454 2023-03-18 01:38:19.000000 python-microgrid-1.3.0/src/pymgrid/microgrid/reward_shaping/pv_curtailment_shaper.py
--rw-r--r--   0 ahalev     (502) staff       (20)      211 2023-03-17 04:48:01.000000 python-microgrid-1.3.0/src/pymgrid/microgrid/serialization_sandbox.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.788972 python-microgrid-1.3.0/src/pymgrid/microgrid/trajectory/
--rw-r--r--   0 ahalev     (502) staff       (20)      129 2023-03-04 01:40:10.000000 python-microgrid-1.3.0/src/pymgrid/microgrid/trajectory/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)      627 2023-03-04 01:40:10.000000 python-microgrid-1.3.0/src/pymgrid/microgrid/trajectory/base.py
--rw-r--r--   0 ahalev     (502) staff       (20)      383 2023-03-18 01:38:19.000000 python-microgrid-1.3.0/src/pymgrid/microgrid/trajectory/deterministic.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1025 2023-03-09 22:23:21.000000 python-microgrid-1.3.0/src/pymgrid/microgrid/trajectory/stochastic.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.789463 python-microgrid-1.3.0/src/pymgrid/microgrid/utils/
--rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-11-23 03:05:26.000000 python-microgrid-1.3.0/src/pymgrid/microgrid/utils/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1860 2023-02-08 21:37:02.000000 python-microgrid-1.3.0/src/pymgrid/microgrid/utils/step.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.791871 python-microgrid-1.3.0/src/pymgrid/modules/
--rw-r--r--   0 ahalev     (502) staff       (20)      316 2023-04-01 21:07:37.000000 python-microgrid-1.3.0/src/pymgrid/modules/__init__.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.792508 python-microgrid-1.3.0/src/pymgrid/modules/base/
--rw-r--r--   0 ahalev     (502) staff       (20)      122 2022-12-02 00:01:20.000000 python-microgrid-1.3.0/src/pymgrid/modules/base/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)    29836 2023-03-29 02:19:50.000000 python-microgrid-1.3.0/src/pymgrid/modules/base/base_module.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.793448 python-microgrid-1.3.0/src/pymgrid/modules/base/timeseries/
--rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-12-02 00:01:20.000000 python-microgrid-1.3.0/src/pymgrid/modules/base/timeseries/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)    12245 2023-03-22 08:15:22.000000 python-microgrid-1.3.0/src/pymgrid/modules/base/timeseries/base_timeseries_module.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.793855 python-microgrid-1.3.0/src/pymgrid/modules/battery/
--rw-r--r--   0 ahalev     (502) staff       (20)        0 2023-04-01 21:07:37.000000 python-microgrid-1.3.0/src/pymgrid/modules/battery/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)    13007 2023-04-01 21:07:37.000000 python-microgrid-1.3.0/src/pymgrid/modules/battery/battery_module.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.794953 python-microgrid-1.3.0/src/pymgrid/modules/battery/transition_models/
--rw-r--r--   0 ahalev     (502) staff       (20)      169 2023-04-01 21:07:37.000000 python-microgrid-1.3.0/src/pymgrid/modules/battery/transition_models/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1157 2023-04-06 17:21:30.000000 python-microgrid-1.3.0/src/pymgrid/modules/battery/transition_models/biased_transition_model.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1196 2023-04-05 06:27:25.000000 python-microgrid-1.3.0/src/pymgrid/modules/battery/transition_models/decay_transition_model.py
--rw-r--r--   0 ahalev     (502) staff       (20)     3566 2023-04-05 06:27:25.000000 python-microgrid-1.3.0/src/pymgrid/modules/battery/transition_models/transition_model.py
--rw-r--r--   0 ahalev     (502) staff       (20)    18133 2023-03-22 08:15:22.000000 python-microgrid-1.3.0/src/pymgrid/modules/genset_module.py
--rw-r--r--   0 ahalev     (502) staff       (20)    11607 2023-02-22 02:13:22.000000 python-microgrid-1.3.0/src/pymgrid/modules/grid_module.py
--rw-r--r--   0 ahalev     (502) staff       (20)     3685 2023-02-22 02:13:22.000000 python-microgrid-1.3.0/src/pymgrid/modules/load_module.py
--rw-r--r--   0 ahalev     (502) staff       (20)    14320 2023-04-05 05:54:52.000000 python-microgrid-1.3.0/src/pymgrid/modules/module_container.py
--rw-r--r--   0 ahalev     (502) staff       (20)     3927 2023-02-22 02:13:22.000000 python-microgrid-1.3.0/src/pymgrid/modules/renewable_module.py
--rw-r--r--   0 ahalev     (502) staff       (20)     3035 2023-03-22 08:15:22.000000 python-microgrid-1.3.0/src/pymgrid/modules/unbalanced_energy_module.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.798392 python-microgrid-1.3.0/src/pymgrid/utils/
--rw-r--r--   0 ahalev     (502) staff       (20)    46856 2022-02-25 19:51:24.000000 python-microgrid-1.3.0/src/pymgrid/utils/DataGenerator.py
--rw-r--r--   0 ahalev     (502) staff       (20)       82 2023-04-01 21:07:37.000000 python-microgrid-1.3.0/src/pymgrid/utils/__init__.py
--rw-r--r--   0 ahalev     (502) staff       (20)      666 2023-04-01 21:07:37.000000 python-microgrid-1.3.0/src/pymgrid/utils/dry_run.py
--rw-r--r--   0 ahalev     (502) staff       (20)     1324 2023-01-25 21:07:28.000000 python-microgrid-1.3.0/src/pymgrid/utils/logger.py
--rw-r--r--   0 ahalev     (502) staff       (20)      632 2023-02-01 02:22:51.000000 python-microgrid-1.3.0/src/pymgrid/utils/ray.py
--rw-r--r--   0 ahalev     (502) staff       (20)     4033 2023-04-05 06:27:25.000000 python-microgrid-1.3.0/src/pymgrid/utils/serialize.py
--rw-r--r--   0 ahalev     (502) staff       (20)     9938 2023-03-22 08:15:22.000000 python-microgrid-1.3.0/src/pymgrid/utils/space.py
--rw-r--r--   0 ahalev     (502) staff       (20)       22 2023-04-06 17:26:35.000000 python-microgrid-1.3.0/src/pymgrid/version.py
-drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-04-06 17:27:14.799181 python-microgrid-1.3.0/src/python_microgrid.egg-info/
--rw-r--r--   0 ahalev     (502) staff       (20)     7369 2023-04-06 17:27:14.000000 python-microgrid-1.3.0/src/python_microgrid.egg-info/PKG-INFO
--rw-r--r--   0 ahalev     (502) staff       (20)    11875 2023-04-06 17:27:14.000000 python-microgrid-1.3.0/src/python_microgrid.egg-info/SOURCES.txt
--rw-r--r--   0 ahalev     (502) staff       (20)        1 2023-04-06 17:27:14.000000 python-microgrid-1.3.0/src/python_microgrid.egg-info/dependency_links.txt
--rw-r--r--   0 ahalev     (502) staff       (20)      343 2023-04-06 17:27:14.000000 python-microgrid-1.3.0/src/python_microgrid.egg-info/requires.txt
--rw-r--r--   0 ahalev     (502) staff       (20)        8 2023-04-06 17:27:14.000000 python-microgrid-1.3.0/src/python_microgrid.egg-info/top_level.txt
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.972581 python-microgrid-1.4.0/
+-rw-r--r--   0 ahalev     (502) staff       (20)     7652 2020-08-13 19:47:38.000000 python-microgrid-1.4.0/LICENSE
+-rw-r--r--   0 ahalev     (502) staff       (20)       31 2023-04-05 06:27:25.000000 python-microgrid-1.4.0/MANIFEST.in
+-rw-r--r--   0 ahalev     (502) staff       (20)     7383 2023-05-30 20:36:29.972766 python-microgrid-1.4.0/PKG-INFO
+-rw-r--r--   0 ahalev     (502) staff       (20)     6767 2023-04-19 19:28:19.000000 python-microgrid-1.4.0/README.md
+-rw-r--r--   0 ahalev     (502) staff       (20)      191 2023-03-29 00:42:14.000000 python-microgrid-1.4.0/pyproject.toml
+-rw-r--r--   0 ahalev     (502) staff       (20)      124 2023-05-30 20:36:29.973139 python-microgrid-1.4.0/setup.cfg
+-rw-r--r--   0 ahalev     (502) staff       (20)     1652 2023-04-08 01:25:01.000000 python-microgrid-1.4.0/setup.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.745041 python-microgrid-1.4.0/src/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.748528 python-microgrid-1.4.0/src/pymgrid/
+-rw-r--r--   0 ahalev     (502) staff       (20)    26580 2023-02-11 01:32:23.000000 python-microgrid-1.4.0/src/pymgrid/MicrogridGenerator.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      513 2023-04-01 21:07:37.000000 python-microgrid-1.4.0/src/pymgrid/__init__.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.748794 python-microgrid-1.4.0/src/pymgrid/_deprecated/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.753828 python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/
+-rw-r--r--   0 ahalev     (502) staff       (20)    21520 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/Environment.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1991 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/Preprocessing.py
+-rw-r--r--   0 ahalev     (502) staff       (20)        1 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    27816 2022-12-17 17:21:34.000000 python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/pymgrid_csca.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1616 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/pymgrid_csca_old.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1614 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/pymgrid_csda.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1979 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/pymgrid_cspla.py
+-rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/_deprecated/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    55258 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/_deprecated/non_modular_microgrid.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.755318 python-microgrid-1.4.0/src/pymgrid/algos/
+-rw-r--r--   0 ahalev     (502) staff       (20)    17127 2022-12-17 17:21:34.000000 python-microgrid-1.4.0/src/pymgrid/algos/Control.py
+-rw-r--r--   0 ahalev     (502) staff       (20)       82 2022-12-10 02:06:45.000000 python-microgrid-1.4.0/src/pymgrid/algos/__init__.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.755831 python-microgrid-1.4.0/src/pymgrid/algos/mpc/
+-rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-10-25 19:17:19.000000 python-microgrid-1.4.0/src/pymgrid/algos/mpc/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    44174 2023-04-27 05:44:00.000000 python-microgrid-1.4.0/src/pymgrid/algos/mpc/mpc.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.757722 python-microgrid-1.4.0/src/pymgrid/algos/priority_list/
+-rw-r--r--   0 ahalev     (502) staff       (20)       99 2022-12-17 03:06:50.000000 python-microgrid-1.4.0/src/pymgrid/algos/priority_list/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     7099 2023-04-25 23:15:20.000000 python-microgrid-1.4.0/src/pymgrid/algos/priority_list/priority_list.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     2783 2023-02-04 17:02:47.000000 python-microgrid-1.4.0/src/pymgrid/algos/priority_list/priority_list_element.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.759141 python-microgrid-1.4.0/src/pymgrid/algos/rbc/
+-rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-12-02 00:00:07.000000 python-microgrid-1.4.0/src/pymgrid/algos/rbc/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    13272 2022-12-17 03:06:50.000000 python-microgrid-1.4.0/src/pymgrid/algos/rbc/_nonmodular_rbc.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     4139 2023-04-27 05:44:00.000000 python-microgrid-1.4.0/src/pymgrid/algos/rbc/rbc.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.759965 python-microgrid-1.4.0/src/pymgrid/algos/saa/
+-rw-r--r--   0 ahalev     (502) staff       (20)       43 2022-10-25 19:17:19.000000 python-microgrid-1.4.0/src/pymgrid/algos/saa/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     7336 2022-12-17 06:16:17.000000 python-microgrid-1.4.0/src/pymgrid/algos/saa/saa.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.780995 python-microgrid-1.4.0/src/pymgrid/convert/
+-rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/convert/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      367 2022-11-30 07:09:17.000000 python-microgrid-1.4.0/src/pymgrid/convert/conversion_test_sandbox.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     2635 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/convert/convert.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     4368 2022-12-10 02:06:16.000000 python-microgrid-1.4.0/src/pymgrid/convert/get_module.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    10537 2023-05-19 17:52:32.000000 python-microgrid-1.4.0/src/pymgrid/convert/to_nonmodular_ops.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.781754 python-microgrid-1.4.0/src/pymgrid/data/
+-rw-r--r--   0 ahalev     (502) staff       (20)        0 2020-10-27 20:16:24.000000 python-microgrid-1.4.0/src/pymgrid/data/__init__.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.781890 python-microgrid-1.4.0/src/pymgrid/data/co2/
+-rw-r--r--   0 ahalev     (502) staff       (20)        1 2020-10-27 20:16:24.000000 python-microgrid-1.4.0/src/pymgrid/data/co2/__init__.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.782391 python-microgrid-1.4.0/src/pymgrid/data/load/
+-rw-r--r--   0 ahalev     (502) staff       (20)        0 2020-10-27 20:16:24.000000 python-microgrid-1.4.0/src/pymgrid/data/load/__init__.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.782582 python-microgrid-1.4.0/src/pymgrid/data/pv/
+-rw-r--r--   0 ahalev     (502) staff       (20)        0 2020-10-27 20:16:24.000000 python-microgrid-1.4.0/src/pymgrid/data/pv/__init__.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.783545 python-microgrid-1.4.0/src/pymgrid/data/scenario/
+-rw-r--r--   0 ahalev     (502) staff       (20)     6148 2022-11-09 16:21:41.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/.DS_Store
+-rw-r--r--   0 ahalev     (502) staff       (20)        1 2020-10-27 20:16:24.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/__init__.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.743411 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.802322 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/
+-rw-r--r--   0 ahalev     (502) staff       (20)     6148 2022-12-17 18:41:28.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/.DS_Store
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.804022 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/
+-rw-r--r--   0 ahalev     (502) staff       (20)     6148 2022-12-17 18:42:51.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/.DS_Store
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.804454 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/
+-rw-r--r--   0 ahalev     (502) staff       (20)     6148 2022-12-17 18:42:57.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/.DS_Store
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.804751 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    71000 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.805408 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    95750 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.806001 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    41119 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2348 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/microgrid_0.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.806324 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.729928 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.730138 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.806698 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    70450 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.807195 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    98740 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.807838 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    43703 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2955 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/microgrid_1.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.808253 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.730346 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.730572 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.808588 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    71849 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.809061 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    99947 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.809631 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    40530 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2974 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/microgrid_10.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.810178 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.730815 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.731031 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.810597 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    70730 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.811040 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    98933 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.811572 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    44288 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2340 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/microgrid_11.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.811908 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.731268 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.731493 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.812275 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    71849 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.812931 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)   101899 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.813497 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    40454 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2334 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/microgrid_12.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.813764 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.731728 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.731941 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.814063 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    69997 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.814569 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)   101801 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.814985 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    41997 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2947 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/microgrid_13.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.815366 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.732157 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.732379 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.815685 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    70730 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.816031 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    92053 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.817898 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    43518 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2336 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/microgrid_14.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.818215 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.735725 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.735987 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.818506 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    98126 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.819141 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    43802 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2425 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/microgrid_15.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.819589 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.736240 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.736474 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.819848 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    71849 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.820154 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    92018 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.820572 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    43220 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2382 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/microgrid_16.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.820826 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.736711 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.736858 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.821487 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    91889 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.843741 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    41880 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2439 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/microgrid_17.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.844390 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.737077 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.737305 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.844914 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    69997 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.845615 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)   101812 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.846351 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    42455 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2945 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/microgrid_18.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.846840 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.737535 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.737670 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.847238 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    98334 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.847950 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    41498 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2448 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/microgrid_19.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.849729 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.737889 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.738021 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.850292 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    98535 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.864132 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    42761 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2433 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/microgrid_2.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.865233 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.738251 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.738392 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.866229 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)   100312 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.868494 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    43495 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2423 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/microgrid_20.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.868859 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.738643 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.738795 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.869179 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)   100892 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.871209 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    43999 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2433 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/microgrid_21.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.872151 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.739044 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.739282 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.872619 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    69997 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.873871 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    99857 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.878056 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    42241 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2951 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/microgrid_22.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.878454 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.739510 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.739661 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.878763 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    97388 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.879368 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    42142 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2415 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/microgrid_23.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.879740 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.739982 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.740260 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.880157 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    70790 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.880888 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    91809 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.881443 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    42978 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2962 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/microgrid_24.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.904170 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.740522 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.740673 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.905032 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)   100230 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.905686 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    42513 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2422 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/microgrid_3.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.906065 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.740922 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.741276 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.906379 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    69997 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.907322 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    99793 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.942276 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    42889 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2333 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/microgrid_4.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.943284 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.741503 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.741641 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.943802 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    98745 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.944345 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    38378 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2428 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/microgrid_5.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.944616 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.741861 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.742076 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.944923 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    69997 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.947170 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)   100276 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.947630 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    43091 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2372 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/microgrid_6.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.948041 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.742404 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.742596 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.948333 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    99461 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.948793 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    42132 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2414 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/microgrid_7.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.949048 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.743022 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.743322 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.949364 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    72045 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.949828 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    92074 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.950236 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    41768 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2974 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/microgrid_8.yaml
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.950731 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.743554 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.743770 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.951036 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/GridModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    71462 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/GridModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.951443 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/LoadModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    98674 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/LoadModule/time_series.csv.gz
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.951973 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/RenewableModule/
+-rw-r--r--   0 ahalev     (502) staff       (20)    44237 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/RenewableModule/time_series.csv.gz
+-rw-r--r--   0 ahalev     (502) staff       (20)     2991 2023-05-19 17:41:02.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/microgrid_9.yaml
+-rw-r--r--   0 ahalev     (502) staff       (20)  7790780 2022-11-09 16:19:50.000000 python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25.pkl
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.952256 python-microgrid-1.4.0/src/pymgrid/envs/
+-rw-r--r--   0 ahalev     (502) staff       (20)      141 2023-05-21 00:24:12.000000 python-microgrid-1.4.0/src/pymgrid/envs/__init__.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.952989 python-microgrid-1.4.0/src/pymgrid/envs/base/
+-rw-r--r--   0 ahalev     (502) staff       (20)       35 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/envs/base/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    14870 2023-05-30 20:36:18.000000 python-microgrid-1.4.0/src/pymgrid/envs/base/base.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      400 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/envs/base/skip_init.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.953374 python-microgrid-1.4.0/src/pymgrid/envs/continuous/
+-rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/envs/continuous/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     8940 2023-05-30 20:36:25.000000 python-microgrid-1.4.0/src/pymgrid/envs/continuous/continuous.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.953689 python-microgrid-1.4.0/src/pymgrid/envs/discrete/
+-rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/envs/discrete/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     5524 2023-05-21 00:24:12.000000 python-microgrid-1.4.0/src/pymgrid/envs/discrete/discrete.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.954324 python-microgrid-1.4.0/src/pymgrid/forecast/
+-rw-r--r--   0 ahalev     (502) staff       (20)      119 2022-12-10 02:06:16.000000 python-microgrid-1.4.0/src/pymgrid/forecast/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    14675 2023-05-12 00:09:47.000000 python-microgrid-1.4.0/src/pymgrid/forecast/forecaster.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.955863 python-microgrid-1.4.0/src/pymgrid/microgrid/
+-rw-r--r--   0 ahalev     (502) staff       (20)       55 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      784 2022-11-23 02:52:46.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/convert_scenario_sandbox.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    40304 2023-05-30 20:36:18.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/microgrid.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     4283 2022-11-23 02:52:46.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/modular_microgrid_sandbox.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.957862 python-microgrid-1.4.0/src/pymgrid/microgrid/reward_shaping/
+-rw-r--r--   0 ahalev     (502) staff       (20)      158 2023-05-30 20:36:25.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/reward_shaping/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     2484 2023-05-30 20:35:30.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/reward_shaping/analyze_shaper.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      565 2023-05-30 20:36:25.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/reward_shaping/base.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1595 2023-05-30 20:35:30.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/reward_shaping/baseline_shaper.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1207 2023-05-30 20:36:25.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/reward_shaping/battery_discharge_shaper.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      471 2023-05-30 20:36:25.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/reward_shaping/pv_curtailment_shaper.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      504 2023-05-30 20:36:25.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/reward_shaping/rescale_shaper.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      211 2023-03-17 04:48:01.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/serialization_sandbox.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.958936 python-microgrid-1.4.0/src/pymgrid/microgrid/trajectory/
+-rw-r--r--   0 ahalev     (502) staff       (20)      129 2023-03-04 01:40:10.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/trajectory/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      627 2023-03-04 01:40:10.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/trajectory/base.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      383 2023-03-18 01:38:19.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/trajectory/deterministic.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1025 2023-03-09 22:23:21.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/trajectory/stochastic.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.959455 python-microgrid-1.4.0/src/pymgrid/microgrid/utils/
+-rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-11-23 03:05:26.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/utils/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     2018 2023-05-30 20:36:25.000000 python-microgrid-1.4.0/src/pymgrid/microgrid/utils/step.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.961657 python-microgrid-1.4.0/src/pymgrid/modules/
+-rw-r--r--   0 ahalev     (502) staff       (20)      316 2023-05-19 17:52:32.000000 python-microgrid-1.4.0/src/pymgrid/modules/__init__.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.964310 python-microgrid-1.4.0/src/pymgrid/modules/base/
+-rw-r--r--   0 ahalev     (502) staff       (20)      122 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/modules/base/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    32031 2023-05-23 21:18:26.000000 python-microgrid-1.4.0/src/pymgrid/modules/base/base_module.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.965106 python-microgrid-1.4.0/src/pymgrid/modules/base/timeseries/
+-rw-r--r--   0 ahalev     (502) staff       (20)        0 2022-12-02 00:01:20.000000 python-microgrid-1.4.0/src/pymgrid/modules/base/timeseries/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    12400 2023-04-28 04:26:05.000000 python-microgrid-1.4.0/src/pymgrid/modules/base/timeseries/base_timeseries_module.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.965696 python-microgrid-1.4.0/src/pymgrid/modules/battery/
+-rw-r--r--   0 ahalev     (502) staff       (20)        0 2023-04-01 21:07:37.000000 python-microgrid-1.4.0/src/pymgrid/modules/battery/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    13095 2023-05-19 18:57:42.000000 python-microgrid-1.4.0/src/pymgrid/modules/battery/battery_module.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.967354 python-microgrid-1.4.0/src/pymgrid/modules/battery/transition_models/
+-rw-r--r--   0 ahalev     (502) staff       (20)      169 2023-04-01 21:07:37.000000 python-microgrid-1.4.0/src/pymgrid/modules/battery/transition_models/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1077 2023-04-06 17:45:24.000000 python-microgrid-1.4.0/src/pymgrid/modules/battery/transition_models/biased_transition_model.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1196 2023-04-05 06:27:25.000000 python-microgrid-1.4.0/src/pymgrid/modules/battery/transition_models/decay_transition_model.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     3566 2023-04-05 06:27:25.000000 python-microgrid-1.4.0/src/pymgrid/modules/battery/transition_models/transition_model.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    18628 2023-05-21 00:24:12.000000 python-microgrid-1.4.0/src/pymgrid/modules/genset_module.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    11686 2023-05-30 20:36:18.000000 python-microgrid-1.4.0/src/pymgrid/modules/grid_module.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     4020 2023-05-21 00:24:12.000000 python-microgrid-1.4.0/src/pymgrid/modules/load_module.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    16512 2023-05-25 23:30:21.000000 python-microgrid-1.4.0/src/pymgrid/modules/module_container.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     3999 2023-05-19 18:57:42.000000 python-microgrid-1.4.0/src/pymgrid/modules/renewable_module.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     3102 2023-05-19 18:57:42.000000 python-microgrid-1.4.0/src/pymgrid/modules/unbalanced_energy_module.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.969764 python-microgrid-1.4.0/src/pymgrid/utils/
+-rw-r--r--   0 ahalev     (502) staff       (20)    46856 2022-02-25 19:51:24.000000 python-microgrid-1.4.0/src/pymgrid/utils/DataGenerator.py
+-rw-r--r--   0 ahalev     (502) staff       (20)       82 2023-04-01 21:07:37.000000 python-microgrid-1.4.0/src/pymgrid/utils/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      259 2023-04-28 04:22:30.000000 python-microgrid-1.4.0/src/pymgrid/utils/dry_run.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1781 2023-05-12 23:54:14.000000 python-microgrid-1.4.0/src/pymgrid/utils/eq.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     1550 2023-05-12 00:09:47.000000 python-microgrid-1.4.0/src/pymgrid/utils/logger.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      632 2023-02-01 02:22:51.000000 python-microgrid-1.4.0/src/pymgrid/utils/ray.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     4056 2023-05-30 20:36:25.000000 python-microgrid-1.4.0/src/pymgrid/utils/serialize.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.970833 python-microgrid-1.4.0/src/pymgrid/utils/space/
+-rw-r--r--   0 ahalev     (502) staff       (20)      103 2023-05-21 00:24:12.000000 python-microgrid-1.4.0/src/pymgrid/utils/space/__init__.py
+-rw-r--r--   0 ahalev     (502) staff       (20)    15426 2023-05-25 23:30:21.000000 python-microgrid-1.4.0/src/pymgrid/utils/space/space.py
+-rw-r--r--   0 ahalev     (502) staff       (20)      484 2023-05-21 00:24:12.000000 python-microgrid-1.4.0/src/pymgrid/utils/space/utils.py
+-rw-r--r--   0 ahalev     (502) staff       (20)       22 2023-05-30 20:36:25.000000 python-microgrid-1.4.0/src/pymgrid/version.py
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.971866 python-microgrid-1.4.0/src/python_microgrid.egg-info/
+-rw-r--r--   0 ahalev     (502) staff       (20)     7383 2023-05-30 20:36:29.000000 python-microgrid-1.4.0/src/python_microgrid.egg-info/PKG-INFO
+-rw-r--r--   0 ahalev     (502) staff       (20)    12208 2023-05-30 20:36:29.000000 python-microgrid-1.4.0/src/python_microgrid.egg-info/SOURCES.txt
+-rw-r--r--   0 ahalev     (502) staff       (20)        1 2023-05-30 20:36:29.000000 python-microgrid-1.4.0/src/python_microgrid.egg-info/dependency_links.txt
+-rw-r--r--   0 ahalev     (502) staff       (20)      343 2023-05-30 20:36:29.000000 python-microgrid-1.4.0/src/python_microgrid.egg-info/requires.txt
+-rw-r--r--   0 ahalev     (502) staff       (20)        8 2023-05-30 20:36:29.000000 python-microgrid-1.4.0/src/python_microgrid.egg-info/top_level.txt
+drwxr-xr-x   0 ahalev     (502) staff       (20)        0 2023-05-30 20:36:29.972287 python-microgrid-1.4.0/tests/
+-rw-r--r--   0 ahalev     (502) staff       (20)     2474 2022-12-10 02:06:16.000000 python-microgrid-1.4.0/tests/test_microgridgenerator.py
+-rw-r--r--   0 ahalev     (502) staff       (20)     2071 2022-12-02 00:00:07.000000 python-microgrid-1.4.0/tests/test_nonmodular_microgrid.py
```

### Comparing `python-microgrid-1.3.0/LICENSE` & `python-microgrid-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/PKG-INFO` & `python-microgrid-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: python-microgrid
-Version: 1.3.0
+Version: 1.4.0
 Summary: A simulator for tertiary control of electrical microgrids
-Download-URL: https://github.com/Total-RD/pymgrid/archive/refs/tags/v1.3.0.tar.gz
+Download-URL: https://github.com/ahalev/python-microgrid/archive/refs/tags/v1.4.0.tar.gz
 Maintainer: Avishai Halev
 Maintainer-email: avishaihalev@gmail.com
 License: GNU LGPL 3.0
 Project-URL: Source Code, https://github.com/ahalev/python-microgrid
 Project-URL: Documentation, https://python-microgrid.readthedocs.io/
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -14,15 +14,15 @@
 Provides-Extra: dev
 Provides-Extra: rtd
 Provides-Extra: all
 License-File: LICENSE
 
 # python-microgrid
 
-![Build](https://github.com/Total-RD/pymgrid/workflows/build/badge.svg?dummy=unused)
+![Build](https://github.com/ahalev/python-microgrid/workflows/build/badge.svg?dummy=unused)
 
 *python-microgrid* is a python library to generate and simulate a large number of microgrids. It is an extension of TotalEnergies' [*pymgrid*](https://github.com/Total-RD/pymgrid).
 
 For more context, please see the [presentation](https://www.climatechange.ai/papers/neurips2020/3) done at Climate Change AI
 and the [documentation](https://python-microgrid.readthedocs.io/).
 
 ## Installation
```

### Comparing `python-microgrid-1.3.0/README.md` & `python-microgrid-1.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # python-microgrid
 
-![Build](https://github.com/Total-RD/pymgrid/workflows/build/badge.svg?dummy=unused)
+![Build](https://github.com/ahalev/python-microgrid/workflows/build/badge.svg?dummy=unused)
 
 *python-microgrid* is a python library to generate and simulate a large number of microgrids. It is an extension of TotalEnergies' [*pymgrid*](https://github.com/Total-RD/pymgrid).
 
 For more context, please see the [presentation](https://www.climatechange.ai/papers/neurips2020/3) done at Climate Change AI
 and the [documentation](https://python-microgrid.readthedocs.io/).
 
 ## Installation
```

### Comparing `python-microgrid-1.3.0/setup.py` & `python-microgrid-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from setuptools import setup, find_packages
 
 v = {}
 exec(open('src/pymgrid/version.py').read(), v)  # read __version__
 VERSION = v['__version__']
 DESCRIPTION = "A simulator for tertiary control of electrical microgrids"
-DOWNLOAD_URL = f"https://github.com/Total-RD/pymgrid/archive/refs/tags/v{VERSION}.tar.gz"
+DOWNLOAD_URL = f"https://github.com/ahalev/python-microgrid/archive/refs/tags/v{VERSION}.tar.gz"
 MAINTAINER = "Avishai Halev"
 MAINTAINER_EMAIL = "avishaihalev@gmail.com"
 LICENSE = "GNU LGPL 3.0"
 PROJECT_URLS = {"Source Code": "https://github.com/ahalev/python-microgrid",
                 "Documentation": "https://python-microgrid.readthedocs.io/"}
 
 EXTRAS = dict()
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/MicrogridGenerator.py` & `python-microgrid-1.4.0/src/pymgrid/MicrogridGenerator.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/__init__.py` & `python-microgrid-1.4.0/src/pymgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/_deprecated/Environments/Environment.py` & `python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/Environment.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/_deprecated/Environments/Preprocessing.py` & `python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/Preprocessing.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/_deprecated/Environments/pymgrid_csca.py` & `python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/pymgrid_csca.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/_deprecated/Environments/pymgrid_csca_old.py` & `python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/pymgrid_csca_old.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/_deprecated/Environments/pymgrid_csda.py` & `python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/pymgrid_csda.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/_deprecated/Environments/pymgrid_cspla.py` & `python-microgrid-1.4.0/src/pymgrid/_deprecated/Environments/pymgrid_cspla.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/_deprecated/non_modular_microgrid.py` & `python-microgrid-1.4.0/src/pymgrid/_deprecated/non_modular_microgrid.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/algos/Control.py` & `python-microgrid-1.4.0/src/pymgrid/algos/Control.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/algos/mpc/mpc.py` & `python-microgrid-1.4.0/src/pymgrid/algos/mpc/mpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -491,14 +491,29 @@
         else:
             self.costs.value[0::7] = import_price.reshape(-1) + grid_co2.reshape(-1) * cost_co2
             self.costs.value[1::7] = export_price.reshape(-1)
 
         if np.isnan(self.costs.value).any():
             raise RuntimeError('There are still nan values in self.costs.value, something is wrong')
 
+    def reset(self):
+        """
+        Reset the underlying microgrid.
+
+        If already reset (e.g. current step is initial step), do nothing.
+
+        Returns
+        -------
+        obs : dict[str, list[float]]
+            Observations from resetting the modules as well as the flushed balance log.
+
+        """
+        if self.microgrid.current_step != self.microgrid.initial_step:
+            self.microgrid.reset()
+
     def run(self, max_steps=None, verbose=False):
         """
         Run the model prediction control algorithm.
 
         Parameters
         ---------
         max_steps : int or None, default None
@@ -534,29 +549,27 @@
         sample = return_underlying_data(self.microgrid)
         sample = sample.reset_index(drop=True)
         return self._run_mpc_on_sample(sample, forecast_steps=forecast_steps, verbose=verbose)
 
     def _run_mpc_on_modular(self, forecast_steps=None, verbose=False):
 
         num_iter = self._get_num_iter(forecast_steps)
-        self.microgrid.reset()
 
-        for i in tqdm(range(num_iter), desc="MPC Progress", disable=(not verbose)):
-            control = self._set_and_solve(*self._get_modular_state_values(),
-                                         iteration=i,
-                                         total_iterations=num_iter,
-                                          verbose=verbose>1)
+        for _ in tqdm(range(num_iter), desc="MPC Progress", disable=(not verbose)):
+            control = self.get_action()
 
             _, _, done, _ = self.microgrid.run(control, normalized=False)
 
             if done:
                 break
 
         return self.microgrid.get_log()
 
+    def get_action(self, verbose=0):
+        return self._set_and_solve(*self._get_modular_state_values(), verbose=verbose > 1)
 
     def _get_num_iter(self, forecast_steps=None):
         if forecast_steps is not None:
             assert forecast_steps <= len(self.microgrid), 'forecast steps cannot be longer than data length.'
             return forecast_steps
 
         elif not self.is_modular:
@@ -729,16 +742,14 @@
                       p_max_import,
                       p_max_export,
                       soc_0,
                       p_genset_max,
                       cost_co2,
                       grid_co2,
                       genset_co2,
-                      iteration=None,
-                      total_iterations=None,
                       return_steps=0,
                        verbose=False):
         """
         Sets the parameters in the problem and then solves the problem.
             Specifically, sets the right-hand sides b and d from the paper of the
             equality and inequality equations, respectively, and the costs vector by calling _set_parameters, then
             solves the problem and returns a control dictionary
@@ -891,17 +902,17 @@
 
         if grid_import > 0 and grid_export > 0:
             if verbose and not np.isclose([grid_import, grid_export], 0, atol=1e-4).any():
                 warn(f"grid_import={grid_import} and grid_export={grid_export} are both nonzero. "
                     f"Flattening to the difference, leading to a {'import' if grid_diff > 0 else 'export'} of {grid_diff}.")
 
         if "grid" in self.microgrid_module_names.keys():
-            control.update({self.microgrid_module_names["grid"]: grid_diff})
+            control[self.microgrid_module_names["grid"]] = [grid_diff]
 
-        control.update({self.microgrid_module_names["battery"]: battery_diff})
+        control[self.microgrid_module_names["battery"]] = [battery_diff]
 
         return control
 
     def _get_modular_state_values(self):
 
         load_state = -1.0 * self.microgrid.modules[self.microgrid_module_names["load"]].item().state # state is negative, want positive values.
         pv_state = self.microgrid.modules[self.microgrid_module_names["renewable"]].item().state
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/algos/priority_list/priority_list.py` & `python-microgrid-1.4.0/src/pymgrid/algos/priority_list/priority_list.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/algos/priority_list/priority_list_element.py` & `python-microgrid-1.4.0/src/pymgrid/algos/priority_list/priority_list_element.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/algos/rbc/_nonmodular_rbc.py` & `python-microgrid-1.4.0/src/pymgrid/algos/rbc/_nonmodular_rbc.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/algos/rbc/rbc.py` & `python-microgrid-1.4.0/src/pymgrid/algos/rbc/rbc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from copy import deepcopy
 from tqdm import tqdm
 
+from pymgrid import Microgrid
 from pymgrid.algos.priority_list import PriorityListAlgo
 
 
 class RuleBasedControl(PriorityListAlgo):
     """
 
     Run a rule-based (heuristic) control algorithm on a microgrid.
@@ -19,17 +20,21 @@
         Microgrid on which to run rule-based control.
 
     priority_list : list of :class:`.PriorityListElement` or None, default None.
         Priority list to use. If None, the order will be defined automatically from the module with the lowest marginal
         cost to the highest.
 
     """
+
+    microgrid : Microgrid
+    'Microgrid on which to run rule-based control.'
+
     def __init__(self, microgrid, priority_list=None, remove_redundant_gensets=True):
         super().__init__()
-        self._microgrid = microgrid
+        self.microgrid = microgrid
         self._priority_list = self._get_priority_list(priority_list, remove_redundant_gensets)
 
     def _get_priority_list(self, priority_list, remove_redundant_gensets):
         """
         Given a microgrid, return the optimal order of module deployment.
         """
         priority_lists = self.get_priority_lists(remove_redundant_gensets=remove_redundant_gensets)
@@ -39,31 +44,28 @@
 
         if priority_list not in priority_lists:
             raise ValueError('Invalid priority list. Use RuleBasedControl.get_priority_lists to view all '
                              'valid priority lists.')
 
         return priority_list
 
-    def _get_action(self):
-        """
-        Given the priority list, define an action.
-        """
-        return self._populate_action(self._priority_list)
-
     def reset(self):
         """
         Reset the underlying microgrid.
 
+        If already reset (e.g. current step is initial step), do nothing.
+
         Returns
         -------
         obs : dict[str, list[float]]
             Observations from resetting the modules as well as the flushed balance log.
 
         """
-        return self._microgrid.reset()
+        if self.microgrid.current_step != self.microgrid.initial_step:
+            self.microgrid.reset()
 
     def run(self, max_steps=None, verbose=False):
         """
         Get the priority list and then deploy on the microgrid for some number of steps.
 
         Parameters
         ---------
@@ -78,59 +80,52 @@
         log : pd.DataFrame
             Results of running the rule-based control algorithm.
 
         """
         self.reset()
 
         for _ in tqdm(range(self._get_num_iter(max_steps)), desc="RBC Progress", disable=(not verbose)):
-            action = self._get_action()
-            _, _, done, _ = self._microgrid.run(action, normalized=False)
+            action = self.get_action()
+            _, _, done, _ = self.microgrid.run(action, normalized=False)
             if done:
                 break
 
-        return self._microgrid.get_log(as_frame=True)
+        return self.microgrid.get_log(as_frame=True)
 
     def _get_num_iter(self, max_steps):
         if max_steps is not None:
             return max_steps
         return self.microgrid.final_step - self.microgrid.initial_step
 
-    def get_empty_action(self):
+    def get_action(self):
         """
-        :meta private:
+        Given the priority list, define an action.
         """
-        return self._microgrid.get_empty_action()
+        return self._populate_action(self._priority_list)
 
-    @property
-    def microgrid(self):
+    def get_empty_action(self):
         """
-        View of the microgrid.
-
-        Returns
-        -------
-        microgrid : :class:`pymgrid.Microgrid`
-            The microgrid that RBC is being run on.
-
+        :meta private:
         """
-        return self._microgrid
+        return self.microgrid.get_empty_action()
 
     @property
     def fixed(self):
         """:meta private:"""
-        return self._microgrid.fixed
+        return self.microgrid.fixed
 
     @property
     def flex(self):
         """:meta private:"""
-        return self._microgrid.flex
+        return self.microgrid.flex
 
     @property
     def modules(self):
         """:meta private:"""
-        return self._microgrid.modules
+        return self.microgrid.modules
 
     @property
     def priority_list(self):
         """
         Order in which to deploy controllable modules.
 
         Returns
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/algos/saa/saa.py` & `python-microgrid-1.4.0/src/pymgrid/algos/saa/saa.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/convert/convert.py` & `python-microgrid-1.4.0/src/pymgrid/convert/convert.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/convert/get_module.py` & `python-microgrid-1.4.0/src/pymgrid/convert/get_module.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/convert/to_nonmodular_ops.py` & `python-microgrid-1.4.0/src/pymgrid/convert/to_nonmodular_ops.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/.DS_Store` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/.DS_Store`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/.DS_Store` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/.DS_Store`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/.DS_Store` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/.DS_Store` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/.DS_Store`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:42 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:45 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:42 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:43 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:42 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:43 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/microgrid_0.yaml` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/microgrid_6.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/LoadModule/time_series.csv.gz'
     name:
     - load
     - 0
     state:
       _current_step: 0
@@ -23,67 +26,79 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: renewable_used
       raise_errors: false
       time_series: !NDArray 'data/cls_params/RenewableModule/time_series.csv.gz'
     name:
     - pv
     - 0
     state:
       _current_step: 0
 - - unbalanced_energy
   - !UnbalancedEnergyModule
     cls_params:
       initial_step: 0
       loss_load_cost: 10
+      normalized_action_bounds:
+      - 0
+      - 1
       overgeneration_cost: 1
       raise_errors: false
     name:
     - unbalanced_energy
     - 0
     state:
       _current_step: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
-      battery_transition_model: null
+      battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
-      init_soc: 0.2
+      init_soc: 0.960305168086668
       initial_step: 0
-      max_capacity: 1452
-      max_charge: 363
-      max_discharge: 363
-      min_capacity: 290.40000000000003
+      max_capacity: 179373
+      max_charge: 44844
+      max_discharge: 44844
+      min_capacity: 35874.6
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
-      current_charge: 290.40000000000003
-      soc: 0.2
+      current_charge: 172252.8189152099
+      soc: 0.960305168086668
 - - grid
   - !GridModule
     cls_params:
       cost_per_unit_co2: 0.1
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
-      max_export: 1920
-      max_import: 1920
+      max_export: 98432
+      max_import: 98432
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/GridModule/time_series.csv.gz'
     name:
     - grid
     - 0
     state:
       _current_step: 0
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:42 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:46 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:42 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:46 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:42 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:46 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/microgrid_1.yaml` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_1/microgrid_1.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/LoadModule/time_series.csv.gz'
     name:
     - load
     - 0
     state:
       _current_step: 0
@@ -23,27 +26,33 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: renewable_used
       raise_errors: false
       time_series: !NDArray 'data/cls_params/RenewableModule/time_series.csv.gz'
     name:
     - pv
     - 0
     state:
       _current_step: 0
 - - unbalanced_energy
   - !UnbalancedEnergyModule
     cls_params:
       initial_step: 0
       loss_load_cost: 10
+      normalized_action_bounds:
+      - 0
+      - 1
       overgeneration_cost: 1
       raise_errors: false
     name:
     - unbalanced_energy
     - 0
     state:
       _current_step: 0
@@ -52,14 +61,17 @@
     cls_params:
       allow_abortion: true
       co2_per_unit: 2
       cost_per_unit_co2: 0.1
       genset_cost: 0.4
       init_start_up: true
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: genset_production
       raise_errors: false
       running_max_production: 60363.0
       running_min_production: 3353.5
       start_up_time: 0
       wind_down_time: 0
     name:
@@ -71,23 +83,26 @@
       _goal_status: true
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
-      battery_transition_model: null
+      battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
       init_soc: 0.2
       initial_step: 0
       max_capacity: 91274
       max_charge: 22819
       max_discharge: 22819
       min_capacity: 18254.8
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
       current_charge: 18254.8
@@ -100,14 +115,17 @@
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
       max_export: 120726
       max_import: 120726
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/GridModule/time_series.csv.gz'
     name:
     - grid
     - 0
     state:
       _current_step: 0
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:44 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:48 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:44 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:48 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:44 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:48 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/microgrid_10.yaml` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/microgrid_8.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/LoadModule/time_series.csv.gz'
     name:
     - load
     - 0
     state:
       _current_step: 0
@@ -23,27 +26,33 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: renewable_used
       raise_errors: false
       time_series: !NDArray 'data/cls_params/RenewableModule/time_series.csv.gz'
     name:
     - pv
     - 0
     state:
       _current_step: 0
 - - unbalanced_energy
   - !UnbalancedEnergyModule
     cls_params:
       initial_step: 0
       loss_load_cost: 10
+      normalized_action_bounds:
+      - 0
+      - 1
       overgeneration_cost: 1
       raise_errors: false
     name:
     - unbalanced_energy
     - 0
     state:
       _current_step: 0
@@ -52,18 +61,21 @@
     cls_params:
       allow_abortion: true
       co2_per_unit: 2
       cost_per_unit_co2: 0.1
       genset_cost: 0.4
       init_start_up: true
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: genset_production
       raise_errors: false
-      running_max_production: 60144.3
-      running_min_production: 3341.3500000000004
+      running_max_production: 64065.6
+      running_min_production: 3559.2000000000003
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
       _current_status: true
@@ -71,43 +83,49 @@
       _goal_status: true
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
-      battery_transition_model: null
+      battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
       init_soc: 0.2
       initial_step: 0
-      max_capacity: 219201
-      max_charge: 54801
-      max_discharge: 54801
-      min_capacity: 43840.200000000004
+      max_capacity: 105583
+      max_charge: 26396
+      max_discharge: 26396
+      min_capacity: 21116.600000000002
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
-      current_charge: 43840.200000000004
+      current_charge: 21116.600000000002
       soc: 0.2
 - - grid
   - !GridModule
     cls_params:
       cost_per_unit_co2: 0.1
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
-      max_export: 120288
-      max_import: 120288
+      max_export: 128130
+      max_import: 128130
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/GridModule/time_series.csv.gz'
     name:
     - grid
     - 0
     state:
       _current_step: 0
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:44 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:48 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:44 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:48 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:44 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:48 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/microgrid_11.yaml` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_11/microgrid_11.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/LoadModule/time_series.csv.gz'
     name:
     - load
     - 0
     state:
       _current_step: 0
@@ -23,47 +26,56 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: renewable_used
       raise_errors: false
       time_series: !NDArray 'data/cls_params/RenewableModule/time_series.csv.gz'
     name:
     - pv
     - 0
     state:
       _current_step: 0
 - - unbalanced_energy
   - !UnbalancedEnergyModule
     cls_params:
       initial_step: 0
       loss_load_cost: 10
+      normalized_action_bounds:
+      - 0
+      - 1
       overgeneration_cost: 1
       raise_errors: false
     name:
     - unbalanced_energy
     - 0
     state:
       _current_step: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
-      battery_transition_model: null
+      battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
       init_soc: 1
       initial_step: 0
       max_capacity: 69594
       max_charge: 17399
       max_discharge: 17399
       min_capacity: 13918.800000000001
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
       current_charge: 69594
@@ -76,14 +88,17 @@
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
       max_export: 55230
       max_import: 55230
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/GridModule/time_series.csv.gz'
     name:
     - grid
     - 0
     state:
       _current_step: 0
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:45 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:48 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:45 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:48 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:45 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:48 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/microgrid_12.yaml` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/microgrid_9.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/LoadModule/time_series.csv.gz'
     name:
     - load
     - 0
     state:
       _current_step: 0
@@ -23,67 +26,106 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: renewable_used
       raise_errors: false
       time_series: !NDArray 'data/cls_params/RenewableModule/time_series.csv.gz'
     name:
     - pv
     - 0
     state:
       _current_step: 0
 - - unbalanced_energy
   - !UnbalancedEnergyModule
     cls_params:
       initial_step: 0
       loss_load_cost: 10
+      normalized_action_bounds:
+      - 0
+      - 1
       overgeneration_cost: 1
       raise_errors: false
     name:
     - unbalanced_energy
     - 0
     state:
       _current_step: 0
+- - genset
+  - !Genset
+    cls_params:
+      allow_abortion: true
+      co2_per_unit: 2
+      cost_per_unit_co2: 0.1
+      genset_cost: 0.4
+      init_start_up: true
+      initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
+      provided_energy_name: genset_production
+      raise_errors: false
+      running_max_production: 98996.40000000001
+      running_min_production: 5499.8
+      start_up_time: 0
+      wind_down_time: 0
+    name:
+    - genset
+    - 0
+    state:
+      _current_status: true
+      _current_step: 0
+      _goal_status: true
+      _steps_until_down: 0
+      _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
-      battery_transition_model: null
+      battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
-      init_soc: 0.2
+      init_soc: 0.5374787046064285
       initial_step: 0
-      max_capacity: 143726
-      max_charge: 35932
-      max_discharge: 35932
-      min_capacity: 28745.2
+      max_capacity: 199587
+      max_charge: 49897
+      max_discharge: 49897
+      min_capacity: 39917.4
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
-      current_charge: 28745.2
-      soc: 0.2
+      current_charge: 107273.76221628326
+      soc: 0.5374787046064285
 - - grid
   - !GridModule
     cls_params:
       cost_per_unit_co2: 0.1
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
-      max_export: 96428
-      max_import: 96428
+      max_export: 197992
+      max_import: 197992
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/GridModule/time_series.csv.gz'
     name:
     - grid
     - 0
     state:
       _current_step: 0
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:45 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:49 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:45 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:48 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:45 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:49 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/microgrid_13.yaml` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/microgrid_3.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/LoadModule/time_series.csv.gz'
     name:
     - load
     - 0
     state:
       _current_step: 0
@@ -23,27 +26,33 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: renewable_used
       raise_errors: false
       time_series: !NDArray 'data/cls_params/RenewableModule/time_series.csv.gz'
     name:
     - pv
     - 0
     state:
       _current_step: 0
 - - unbalanced_energy
   - !UnbalancedEnergyModule
     cls_params:
       initial_step: 0
       loss_load_cost: 10
+      normalized_action_bounds:
+      - 0
+      - 1
       overgeneration_cost: 1
       raise_errors: false
     name:
     - unbalanced_energy
     - 0
     state:
       _current_step: 0
@@ -52,18 +61,21 @@
     cls_params:
       allow_abortion: true
       co2_per_unit: 2
       cost_per_unit_co2: 0.1
       genset_cost: 0.4
       init_start_up: true
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: genset_production
       raise_errors: false
-      running_max_production: 19941.3
-      running_min_production: 1107.8500000000001
+      running_max_production: 78147.0
+      running_min_production: 4341.5
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
       _current_status: true
@@ -71,44 +83,28 @@
       _goal_status: true
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
-      battery_transition_model: null
+      battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
       init_soc: 0.2
       initial_step: 0
-      max_capacity: 47556
-      max_charge: 11889
-      max_discharge: 11889
-      min_capacity: 9511.2
+      max_capacity: 102450
+      max_charge: 25613
+      max_discharge: 25613
+      min_capacity: 20490.0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
-      current_charge: 9511.2
+      current_charge: 20490.0
       soc: 0.2
-- - grid
-  - !GridModule
-    cls_params:
-      cost_per_unit_co2: 0.1
-      final_step: 8759
-      forecast_horizon: 23
-      forecaster: oracle
-      forecaster_increase_uncertainty: false
-      forecaster_relative_noise: false
-      initial_step: 0
-      max_export: 39882
-      max_import: 39882
-      raise_errors: false
-      time_series: !NDArray 'data/cls_params/GridModule/time_series.csv.gz'
-    name:
-    - grid
-    - 0
-    state:
-      _current_step: 0
 trajectory_func: null
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:45 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:49 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:45 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:49 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:45 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:49 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/microgrid_14.yaml` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_14/microgrid_14.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/LoadModule/time_series.csv.gz'
     name:
     - load
     - 0
     state:
       _current_step: 0
@@ -23,47 +26,56 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: renewable_used
       raise_errors: false
       time_series: !NDArray 'data/cls_params/RenewableModule/time_series.csv.gz'
     name:
     - pv
     - 0
     state:
       _current_step: 0
 - - unbalanced_energy
   - !UnbalancedEnergyModule
     cls_params:
       initial_step: 0
       loss_load_cost: 10
+      normalized_action_bounds:
+      - 0
+      - 1
       overgeneration_cost: 1
       raise_errors: false
     name:
     - unbalanced_energy
     - 0
     state:
       _current_step: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
-      battery_transition_model: null
+      battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
       init_soc: 0.2
       initial_step: 0
       max_capacity: 162570
       max_charge: 40643
       max_discharge: 40643
       min_capacity: 32514.0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
       current_charge: 32514.0
@@ -76,14 +88,17 @@
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
       max_export: 197286
       max_import: 197286
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/GridModule/time_series.csv.gz'
     name:
     - grid
     - 0
     state:
       _current_step: 0
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:46 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:49 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:46 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:49 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/microgrid_15.yaml` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/microgrid_2.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/LoadModule/time_series.csv.gz'
     name:
     - load
     - 0
     state:
       _current_step: 0
@@ -23,27 +26,33 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: renewable_used
       raise_errors: false
       time_series: !NDArray 'data/cls_params/RenewableModule/time_series.csv.gz'
     name:
     - pv
     - 0
     state:
       _current_step: 0
 - - unbalanced_energy
   - !UnbalancedEnergyModule
     cls_params:
       initial_step: 0
       loss_load_cost: 10
+      normalized_action_bounds:
+      - 0
+      - 1
       overgeneration_cost: 1
       raise_errors: false
     name:
     - unbalanced_energy
     - 0
     state:
       _current_step: 0
@@ -52,18 +61,21 @@
     cls_params:
       allow_abortion: true
       co2_per_unit: 2
       cost_per_unit_co2: 0.1
       genset_cost: 0.4
       init_start_up: true
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: genset_production
       raise_errors: false
-      running_max_production: 17296.2
-      running_min_production: 960.9000000000001
+      running_max_production: 43725.6
+      running_min_production: 2429.2000000000003
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
       _current_status: true
@@ -71,25 +83,28 @@
       _goal_status: true
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
-      battery_transition_model: null
+      battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
-      init_soc: 1
+      init_soc: 0.2
       initial_step: 0
-      max_capacity: 26153
-      max_charge: 6539
-      max_discharge: 6539
-      min_capacity: 5230.6
+      max_capacity: 66116
+      max_charge: 16529
+      max_discharge: 16529
+      min_capacity: 13223.2
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
-      current_charge: 26153
-      soc: 1.0
+      current_charge: 13223.2
+      soc: 0.2
 trajectory_func: null
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:46 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:49 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:46 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:49 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:46 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:49 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/microgrid_16.yaml` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_12/microgrid_12.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/LoadModule/time_series.csv.gz'
     name:
     - load
     - 0
     state:
       _current_step: 0
@@ -23,67 +26,79 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: renewable_used
       raise_errors: false
       time_series: !NDArray 'data/cls_params/RenewableModule/time_series.csv.gz'
     name:
     - pv
     - 0
     state:
       _current_step: 0
 - - unbalanced_energy
   - !UnbalancedEnergyModule
     cls_params:
       initial_step: 0
       loss_load_cost: 10
+      normalized_action_bounds:
+      - 0
+      - 1
       overgeneration_cost: 1
       raise_errors: false
     name:
     - unbalanced_energy
     - 0
     state:
       _current_step: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
-      battery_transition_model: null
+      battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
-      init_soc: 0.534118811938557
+      init_soc: 0.2
       initial_step: 0
-      max_capacity: 60099
-      max_charge: 15025
-      max_discharge: 15025
-      min_capacity: 12019.800000000001
+      max_capacity: 143726
+      max_charge: 35932
+      max_discharge: 35932
+      min_capacity: 28745.2
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
-      current_charge: 32100.00647869534
-      soc: 0.534118811938557
+      current_charge: 28745.2
+      soc: 0.2
 - - grid
   - !GridModule
     cls_params:
       cost_per_unit_co2: 0.1
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
-      max_export: 97244
-      max_import: 97244
+      max_export: 96428
+      max_import: 96428
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/GridModule/time_series.csv.gz'
     name:
     - grid
     - 0
     state:
       _current_step: 0
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:46 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:49 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:46 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:49 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_17/microgrid_17.yaml` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/microgrid_7.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/LoadModule/time_series.csv.gz'
     name:
     - load
     - 0
     state:
       _current_step: 0
@@ -23,27 +26,33 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: renewable_used
       raise_errors: false
       time_series: !NDArray 'data/cls_params/RenewableModule/time_series.csv.gz'
     name:
     - pv
     - 0
     state:
       _current_step: 0
 - - unbalanced_energy
   - !UnbalancedEnergyModule
     cls_params:
       initial_step: 0
       loss_load_cost: 10
+      normalized_action_bounds:
+      - 0
+      - 1
       overgeneration_cost: 1
       raise_errors: false
     name:
     - unbalanced_energy
     - 0
     state:
       _current_step: 0
@@ -52,18 +61,21 @@
     cls_params:
       allow_abortion: true
       co2_per_unit: 2
       cost_per_unit_co2: 0.1
       genset_cost: 0.4
       init_start_up: true
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: genset_production
       raise_errors: false
-      running_max_production: 31257.0
-      running_min_production: 1736.5
+      running_max_production: 11798.1
+      running_min_production: 655.45
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
       _current_status: true
@@ -71,25 +83,28 @@
       _goal_status: true
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
-      battery_transition_model: null
+      battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
-      init_soc: 0.2
+      init_soc: 1
       initial_step: 0
-      max_capacity: 38636
-      max_charge: 9659
-      max_discharge: 9659
-      min_capacity: 7727.200000000001
+      max_capacity: 19334
+      max_charge: 4834
+      max_discharge: 4834
+      min_capacity: 3866.8
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
-      current_charge: 7727.200000000001
-      soc: 0.2
+      current_charge: 19334
+      soc: 1.0
 trajectory_func: null
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:46 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:46 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:46 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:50 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:46 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:50 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/microgrid_18.yaml` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/microgrid_18.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/LoadModule/time_series.csv.gz'
     name:
     - load
     - 0
     state:
       _current_step: 0
@@ -23,27 +26,33 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: renewable_used
       raise_errors: false
       time_series: !NDArray 'data/cls_params/RenewableModule/time_series.csv.gz'
     name:
     - pv
     - 0
     state:
       _current_step: 0
 - - unbalanced_energy
   - !UnbalancedEnergyModule
     cls_params:
       initial_step: 0
       loss_load_cost: 10
+      normalized_action_bounds:
+      - 0
+      - 1
       overgeneration_cost: 1
       raise_errors: false
     name:
     - unbalanced_energy
     - 0
     state:
       _current_step: 0
@@ -52,14 +61,17 @@
     cls_params:
       allow_abortion: true
       co2_per_unit: 2
       cost_per_unit_co2: 0.1
       genset_cost: 0.4
       init_start_up: true
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: genset_production
       raise_errors: false
       running_max_production: 34418.700000000004
       running_min_production: 1912.15
       start_up_time: 0
       wind_down_time: 0
     name:
@@ -71,23 +83,26 @@
       _goal_status: true
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
-      battery_transition_model: null
+      battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
       init_soc: 1
       initial_step: 0
       max_capacity: 82080
       max_charge: 20520
       max_discharge: 20520
       min_capacity: 16416.0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
       current_charge: 82080
@@ -100,14 +115,17 @@
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
       max_export: 68836
       max_import: 68836
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/GridModule/time_series.csv.gz'
     name:
     - grid
     - 0
     state:
       _current_step: 0
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:47 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:50 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:47 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:50 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/microgrid_19.yaml` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/microgrid_24.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/LoadModule/time_series.csv.gz'
     name:
     - load
     - 0
     state:
       _current_step: 0
@@ -23,27 +26,33 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: renewable_used
       raise_errors: false
       time_series: !NDArray 'data/cls_params/RenewableModule/time_series.csv.gz'
     name:
     - pv
     - 0
     state:
       _current_step: 0
 - - unbalanced_energy
   - !UnbalancedEnergyModule
     cls_params:
       initial_step: 0
       loss_load_cost: 10
+      normalized_action_bounds:
+      - 0
+      - 1
       overgeneration_cost: 1
       raise_errors: false
     name:
     - unbalanced_energy
     - 0
     state:
       _current_step: 0
@@ -52,18 +61,21 @@
     cls_params:
       allow_abortion: true
       co2_per_unit: 2
       cost_per_unit_co2: 0.1
       genset_cost: 0.4
       init_start_up: true
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: genset_production
       raise_errors: false
-      running_max_production: 1529.1000000000001
-      running_min_production: 84.95
+      running_max_production: 50157.0
+      running_min_production: 2786.5
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
       _current_status: true
@@ -71,25 +83,50 @@
       _goal_status: true
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
-      battery_transition_model: null
+      battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
       init_soc: 0.2
       initial_step: 0
-      max_capacity: 2506
-      max_charge: 627
-      max_discharge: 627
-      min_capacity: 501.20000000000005
+      max_capacity: 103328
+      max_charge: 25832
+      max_discharge: 25832
+      min_capacity: 20665.600000000002
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
-      current_charge: 501.20000000000005
+      current_charge: 20665.600000000002
       soc: 0.2
+- - grid
+  - !GridModule
+    cls_params:
+      cost_per_unit_co2: 0.1
+      final_step: 8759
+      forecast_horizon: 23
+      forecaster: oracle
+      forecaster_increase_uncertainty: false
+      forecaster_relative_noise: false
+      initial_step: 0
+      max_export: 100314
+      max_import: 100314
+      normalized_action_bounds:
+      - 0
+      - 1
+      raise_errors: false
+      time_series: !NDArray 'data/cls_params/GridModule/time_series.csv.gz'
+    name:
+    - grid
+    - 0
+    state:
+      _current_step: 0
 trajectory_func: null
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:42 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:46 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:42 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:46 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_2/microgrid_2.yaml` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/microgrid_21.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/LoadModule/time_series.csv.gz'
     name:
     - load
     - 0
     state:
       _current_step: 0
@@ -23,27 +26,33 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: renewable_used
       raise_errors: false
       time_series: !NDArray 'data/cls_params/RenewableModule/time_series.csv.gz'
     name:
     - pv
     - 0
     state:
       _current_step: 0
 - - unbalanced_energy
   - !UnbalancedEnergyModule
     cls_params:
       initial_step: 0
       loss_load_cost: 10
+      normalized_action_bounds:
+      - 0
+      - 1
       overgeneration_cost: 1
       raise_errors: false
     name:
     - unbalanced_energy
     - 0
     state:
       _current_step: 0
@@ -52,18 +61,21 @@
     cls_params:
       allow_abortion: true
       co2_per_unit: 2
       cost_per_unit_co2: 0.1
       genset_cost: 0.4
       init_start_up: true
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: genset_production
       raise_errors: false
-      running_max_production: 43725.6
-      running_min_production: 2429.2000000000003
+      running_max_production: 95435.1
+      running_min_production: 5301.950000000001
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
       _current_status: true
@@ -71,25 +83,28 @@
       _goal_status: true
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
-      battery_transition_model: null
+      battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
       init_soc: 0.2
       initial_step: 0
-      max_capacity: 66116
-      max_charge: 16529
-      max_discharge: 16529
-      min_capacity: 13223.2
+      max_capacity: 170694
+      max_charge: 42674
+      max_discharge: 42674
+      min_capacity: 34138.8
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
-      current_charge: 13223.2
+      current_charge: 34138.8
       soc: 0.2
 trajectory_func: null
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:47 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:50 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:47 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:50 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/microgrid_20.yaml` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/microgrid_22.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/LoadModule/time_series.csv.gz'
     name:
     - load
     - 0
     state:
       _current_step: 0
@@ -23,27 +26,33 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: renewable_used
       raise_errors: false
       time_series: !NDArray 'data/cls_params/RenewableModule/time_series.csv.gz'
     name:
     - pv
     - 0
     state:
       _current_step: 0
 - - unbalanced_energy
   - !UnbalancedEnergyModule
     cls_params:
       initial_step: 0
       loss_load_cost: 10
+      normalized_action_bounds:
+      - 0
+      - 1
       overgeneration_cost: 1
       raise_errors: false
     name:
     - unbalanced_energy
     - 0
     state:
       _current_step: 0
@@ -52,18 +61,21 @@
     cls_params:
       allow_abortion: true
       co2_per_unit: 2
       cost_per_unit_co2: 0.1
       genset_cost: 0.4
       init_start_up: true
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: genset_production
       raise_errors: false
-      running_max_production: 79186.5
-      running_min_production: 4399.25
+      running_max_production: 80372.7
+      running_min_production: 4465.150000000001
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
       _current_status: true
@@ -71,25 +83,50 @@
       _goal_status: true
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
-      battery_transition_model: null
+      battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
       init_soc: 0.2
       initial_step: 0
-      max_capacity: 129765
-      max_charge: 32442
-      max_discharge: 32442
-      min_capacity: 25953.0
+      max_capacity: 292924
+      max_charge: 73231
+      max_discharge: 73231
+      min_capacity: 58584.8
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
-      current_charge: 25953.0
+      current_charge: 58584.8
       soc: 0.2
+- - grid
+  - !GridModule
+    cls_params:
+      cost_per_unit_co2: 0.1
+      final_step: 8759
+      forecast_horizon: 23
+      forecaster: oracle
+      forecaster_increase_uncertainty: false
+      forecaster_relative_noise: false
+      initial_step: 0
+      max_export: 160744
+      max_import: 160744
+      normalized_action_bounds:
+      - 0
+      - 1
+      raise_errors: false
+      time_series: !NDArray 'data/cls_params/GridModule/time_series.csv.gz'
+    name:
+    - grid
+    - 0
+    state:
+      _current_step: 0
 trajectory_func: null
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:47 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:50 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:47 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:50 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_21/microgrid_21.yaml` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_20/microgrid_20.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/LoadModule/time_series.csv.gz'
     name:
     - load
     - 0
     state:
       _current_step: 0
@@ -23,27 +26,33 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: renewable_used
       raise_errors: false
       time_series: !NDArray 'data/cls_params/RenewableModule/time_series.csv.gz'
     name:
     - pv
     - 0
     state:
       _current_step: 0
 - - unbalanced_energy
   - !UnbalancedEnergyModule
     cls_params:
       initial_step: 0
       loss_load_cost: 10
+      normalized_action_bounds:
+      - 0
+      - 1
       overgeneration_cost: 1
       raise_errors: false
     name:
     - unbalanced_energy
     - 0
     state:
       _current_step: 0
@@ -52,18 +61,21 @@
     cls_params:
       allow_abortion: true
       co2_per_unit: 2
       cost_per_unit_co2: 0.1
       genset_cost: 0.4
       init_start_up: true
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: genset_production
       raise_errors: false
-      running_max_production: 95435.1
-      running_min_production: 5301.950000000001
+      running_max_production: 79186.5
+      running_min_production: 4399.25
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
       _current_status: true
@@ -71,25 +83,28 @@
       _goal_status: true
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
-      battery_transition_model: null
+      battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
       init_soc: 0.2
       initial_step: 0
-      max_capacity: 170694
-      max_charge: 42674
-      max_discharge: 42674
-      min_capacity: 34138.8
+      max_capacity: 129765
+      max_charge: 32442
+      max_discharge: 32442
+      min_capacity: 25953.0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
-      current_charge: 34138.8
+      current_charge: 25953.0
       soc: 0.2
 trajectory_func: null
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:47 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:47 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:47 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:50 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:47 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:50 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/microgrid_22.yaml` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/microgrid_23.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/LoadModule/time_series.csv.gz'
     name:
     - load
     - 0
     state:
       _current_step: 0
@@ -23,27 +26,33 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: renewable_used
       raise_errors: false
       time_series: !NDArray 'data/cls_params/RenewableModule/time_series.csv.gz'
     name:
     - pv
     - 0
     state:
       _current_step: 0
 - - unbalanced_energy
   - !UnbalancedEnergyModule
     cls_params:
       initial_step: 0
       loss_load_cost: 10
+      normalized_action_bounds:
+      - 0
+      - 1
       overgeneration_cost: 1
       raise_errors: false
     name:
     - unbalanced_energy
     - 0
     state:
       _current_step: 0
@@ -52,18 +61,21 @@
     cls_params:
       allow_abortion: true
       co2_per_unit: 2
       cost_per_unit_co2: 0.1
       genset_cost: 0.4
       init_start_up: true
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: genset_production
       raise_errors: false
-      running_max_production: 80372.7
-      running_min_production: 4465.150000000001
+      running_max_production: 9453.6
+      running_min_production: 525.2
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
       _current_status: true
@@ -71,44 +83,28 @@
       _goal_status: true
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
-      battery_transition_model: null
+      battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
       init_soc: 0.2
       initial_step: 0
-      max_capacity: 292924
-      max_charge: 73231
-      max_discharge: 73231
-      min_capacity: 58584.8
+      max_capacity: 14294
+      max_charge: 3574
+      max_discharge: 3574
+      min_capacity: 2858.8
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
-      current_charge: 58584.8
+      current_charge: 2858.8
       soc: 0.2
-- - grid
-  - !GridModule
-    cls_params:
-      cost_per_unit_co2: 0.1
-      final_step: 8759
-      forecast_horizon: 23
-      forecaster: oracle
-      forecaster_increase_uncertainty: false
-      forecaster_relative_noise: false
-      initial_step: 0
-      max_export: 160744
-      max_import: 160744
-      raise_errors: false
-      time_series: !NDArray 'data/cls_params/GridModule/time_series.csv.gz'
-    name:
-    - grid
-    - 0
-    state:
-      _current_step: 0
 trajectory_func: null
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:47 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:51 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:47 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:51 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_23/microgrid_23.yaml` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/microgrid_5.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/LoadModule/time_series.csv.gz'
     name:
     - load
     - 0
     state:
       _current_step: 0
@@ -23,27 +26,33 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: renewable_used
       raise_errors: false
       time_series: !NDArray 'data/cls_params/RenewableModule/time_series.csv.gz'
     name:
     - pv
     - 0
     state:
       _current_step: 0
 - - unbalanced_energy
   - !UnbalancedEnergyModule
     cls_params:
       initial_step: 0
       loss_load_cost: 10
+      normalized_action_bounds:
+      - 0
+      - 1
       overgeneration_cost: 1
       raise_errors: false
     name:
     - unbalanced_energy
     - 0
     state:
       _current_step: 0
@@ -52,18 +61,21 @@
     cls_params:
       allow_abortion: true
       co2_per_unit: 2
       cost_per_unit_co2: 0.1
       genset_cost: 0.4
       init_start_up: true
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: genset_production
       raise_errors: false
-      running_max_production: 9453.6
-      running_min_production: 525.2
+      running_max_production: 28560.600000000002
+      running_min_production: 1586.7
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
       _current_status: true
@@ -71,25 +83,28 @@
       _goal_status: true
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
-      battery_transition_model: null
+      battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
-      init_soc: 0.2
+      init_soc: 1
       initial_step: 0
-      max_capacity: 14294
-      max_charge: 3574
-      max_discharge: 3574
-      min_capacity: 2858.8
+      max_capacity: 57581
+      max_charge: 14396
+      max_discharge: 14396
+      min_capacity: 11516.2
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
-      current_charge: 2858.8
-      soc: 0.2
+      current_charge: 57581
+      soc: 1.0
 trajectory_func: null
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:48 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:51 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:48 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:51 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:48 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:51 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_24/microgrid_24.yaml` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_0/microgrid_0.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/LoadModule/time_series.csv.gz'
     name:
     - load
     - 0
     state:
       _current_step: 0
@@ -23,91 +26,79 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: renewable_used
       raise_errors: false
       time_series: !NDArray 'data/cls_params/RenewableModule/time_series.csv.gz'
     name:
     - pv
     - 0
     state:
       _current_step: 0
 - - unbalanced_energy
   - !UnbalancedEnergyModule
     cls_params:
       initial_step: 0
       loss_load_cost: 10
+      normalized_action_bounds:
+      - 0
+      - 1
       overgeneration_cost: 1
       raise_errors: false
     name:
     - unbalanced_energy
     - 0
     state:
       _current_step: 0
-- - genset
-  - !Genset
-    cls_params:
-      allow_abortion: true
-      co2_per_unit: 2
-      cost_per_unit_co2: 0.1
-      genset_cost: 0.4
-      init_start_up: true
-      initial_step: 0
-      provided_energy_name: genset_production
-      raise_errors: false
-      running_max_production: 50157.0
-      running_min_production: 2786.5
-      start_up_time: 0
-      wind_down_time: 0
-    name:
-    - genset
-    - 0
-    state:
-      _current_status: true
-      _current_step: 0
-      _goal_status: true
-      _steps_until_down: 0
-      _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
-      battery_transition_model: null
+      battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
       init_soc: 0.2
       initial_step: 0
-      max_capacity: 103328
-      max_charge: 25832
-      max_discharge: 25832
-      min_capacity: 20665.600000000002
+      max_capacity: 1452
+      max_charge: 363
+      max_discharge: 363
+      min_capacity: 290.40000000000003
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
-      current_charge: 20665.600000000002
+      current_charge: 290.40000000000003
       soc: 0.2
 - - grid
   - !GridModule
     cls_params:
       cost_per_unit_co2: 0.1
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
-      max_export: 100314
-      max_import: 100314
+      max_export: 1920
+      max_import: 1920
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/GridModule/time_series.csv.gz'
     name:
     - grid
     - 0
     state:
       _current_step: 0
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:42 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:46 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:42 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:46 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_3/microgrid_3.yaml` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_13/microgrid_13.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/LoadModule/time_series.csv.gz'
     name:
     - load
     - 0
     state:
       _current_step: 0
@@ -23,27 +26,33 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: renewable_used
       raise_errors: false
       time_series: !NDArray 'data/cls_params/RenewableModule/time_series.csv.gz'
     name:
     - pv
     - 0
     state:
       _current_step: 0
 - - unbalanced_energy
   - !UnbalancedEnergyModule
     cls_params:
       initial_step: 0
       loss_load_cost: 10
+      normalized_action_bounds:
+      - 0
+      - 1
       overgeneration_cost: 1
       raise_errors: false
     name:
     - unbalanced_energy
     - 0
     state:
       _current_step: 0
@@ -52,18 +61,21 @@
     cls_params:
       allow_abortion: true
       co2_per_unit: 2
       cost_per_unit_co2: 0.1
       genset_cost: 0.4
       init_start_up: true
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: genset_production
       raise_errors: false
-      running_max_production: 78147.0
-      running_min_production: 4341.5
+      running_max_production: 19941.3
+      running_min_production: 1107.8500000000001
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
       _current_status: true
@@ -71,25 +83,50 @@
       _goal_status: true
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
-      battery_transition_model: null
+      battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
       init_soc: 0.2
       initial_step: 0
-      max_capacity: 102450
-      max_charge: 25613
-      max_discharge: 25613
-      min_capacity: 20490.0
+      max_capacity: 47556
+      max_charge: 11889
+      max_discharge: 11889
+      min_capacity: 9511.2
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
-      current_charge: 20490.0
+      current_charge: 9511.2
       soc: 0.2
+- - grid
+  - !GridModule
+    cls_params:
+      cost_per_unit_co2: 0.1
+      final_step: 8759
+      forecast_horizon: 23
+      forecaster: oracle
+      forecaster_increase_uncertainty: false
+      forecaster_relative_noise: false
+      initial_step: 0
+      max_export: 39882
+      max_import: 39882
+      normalized_action_bounds:
+      - 0
+      - 1
+      raise_errors: false
+      time_series: !NDArray 'data/cls_params/GridModule/time_series.csv.gz'
+    name:
+    - grid
+    - 0
+    state:
+      _current_step: 0
 trajectory_func: null
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_18/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:43 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:50 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:43 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:46 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:43 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:46 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/microgrid_4.yaml` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_4/microgrid_4.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/LoadModule/time_series.csv.gz'
     name:
     - load
     - 0
     state:
       _current_step: 0
@@ -23,47 +26,56 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: renewable_used
       raise_errors: false
       time_series: !NDArray 'data/cls_params/RenewableModule/time_series.csv.gz'
     name:
     - pv
     - 0
     state:
       _current_step: 0
 - - unbalanced_energy
   - !UnbalancedEnergyModule
     cls_params:
       initial_step: 0
       loss_load_cost: 10
+      normalized_action_bounds:
+      - 0
+      - 1
       overgeneration_cost: 1
       raise_errors: false
     name:
     - unbalanced_energy
     - 0
     state:
       _current_step: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
-      battery_transition_model: null
+      battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
       init_soc: 0.2
       initial_step: 0
       max_capacity: 65305
       max_charge: 16327
       max_discharge: 16327
       min_capacity: 13061.0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
       current_charge: 13061.0
@@ -76,14 +88,17 @@
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
       max_export: 99625
       max_import: 99625
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/GridModule/time_series.csv.gz'
     name:
     - grid
     - 0
     state:
       _current_step: 0
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:43 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:46 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:43 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:47 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_5/microgrid_5.yaml` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_19/microgrid_19.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/LoadModule/time_series.csv.gz'
     name:
     - load
     - 0
     state:
       _current_step: 0
@@ -23,27 +26,33 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: renewable_used
       raise_errors: false
       time_series: !NDArray 'data/cls_params/RenewableModule/time_series.csv.gz'
     name:
     - pv
     - 0
     state:
       _current_step: 0
 - - unbalanced_energy
   - !UnbalancedEnergyModule
     cls_params:
       initial_step: 0
       loss_load_cost: 10
+      normalized_action_bounds:
+      - 0
+      - 1
       overgeneration_cost: 1
       raise_errors: false
     name:
     - unbalanced_energy
     - 0
     state:
       _current_step: 0
@@ -52,18 +61,21 @@
     cls_params:
       allow_abortion: true
       co2_per_unit: 2
       cost_per_unit_co2: 0.1
       genset_cost: 0.4
       init_start_up: true
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: genset_production
       raise_errors: false
-      running_max_production: 28560.600000000002
-      running_min_production: 1586.7
+      running_max_production: 1529.1000000000001
+      running_min_production: 84.95
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
       _current_status: true
@@ -71,25 +83,28 @@
       _goal_status: true
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
-      battery_transition_model: null
+      battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
-      init_soc: 1
+      init_soc: 0.2
       initial_step: 0
-      max_capacity: 57581
-      max_charge: 14396
-      max_discharge: 14396
-      min_capacity: 11516.2
+      max_capacity: 2506
+      max_charge: 627
+      max_discharge: 627
+      min_capacity: 501.20000000000005
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
-      current_charge: 57581
-      soc: 1.0
+      current_charge: 501.20000000000005
+      soc: 0.2
 trajectory_func: null
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_22/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:43 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:50 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:43 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:47 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:43 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:47 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_6/microgrid_6.yaml` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_10/microgrid_10.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/LoadModule/time_series.csv.gz'
     name:
     - load
     - 0
     state:
       _current_step: 0
@@ -23,67 +26,106 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: renewable_used
       raise_errors: false
       time_series: !NDArray 'data/cls_params/RenewableModule/time_series.csv.gz'
     name:
     - pv
     - 0
     state:
       _current_step: 0
 - - unbalanced_energy
   - !UnbalancedEnergyModule
     cls_params:
       initial_step: 0
       loss_load_cost: 10
+      normalized_action_bounds:
+      - 0
+      - 1
       overgeneration_cost: 1
       raise_errors: false
     name:
     - unbalanced_energy
     - 0
     state:
       _current_step: 0
+- - genset
+  - !Genset
+    cls_params:
+      allow_abortion: true
+      co2_per_unit: 2
+      cost_per_unit_co2: 0.1
+      genset_cost: 0.4
+      init_start_up: true
+      initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
+      provided_energy_name: genset_production
+      raise_errors: false
+      running_max_production: 60144.3
+      running_min_production: 3341.3500000000004
+      start_up_time: 0
+      wind_down_time: 0
+    name:
+    - genset
+    - 0
+    state:
+      _current_status: true
+      _current_step: 0
+      _goal_status: true
+      _steps_until_down: 0
+      _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
-      battery_transition_model: null
+      battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
-      init_soc: 0.960305168086668
+      init_soc: 0.2
       initial_step: 0
-      max_capacity: 179373
-      max_charge: 44844
-      max_discharge: 44844
-      min_capacity: 35874.6
+      max_capacity: 219201
+      max_charge: 54801
+      max_discharge: 54801
+      min_capacity: 43840.200000000004
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
-      current_charge: 172252.8189152099
-      soc: 0.960305168086668
+      current_charge: 43840.200000000004
+      soc: 0.2
 - - grid
   - !GridModule
     cls_params:
       cost_per_unit_co2: 0.1
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
-      max_export: 98432
-      max_import: 98432
+      max_export: 120288
+      max_import: 120288
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/GridModule/time_series.csv.gz'
     name:
     - grid
     - 0
     state:
       _current_step: 0
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:43 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:47 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:43 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:47 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_7/microgrid_7.yaml` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_15/microgrid_15.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/LoadModule/time_series.csv.gz'
     name:
     - load
     - 0
     state:
       _current_step: 0
@@ -23,27 +26,33 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: renewable_used
       raise_errors: false
       time_series: !NDArray 'data/cls_params/RenewableModule/time_series.csv.gz'
     name:
     - pv
     - 0
     state:
       _current_step: 0
 - - unbalanced_energy
   - !UnbalancedEnergyModule
     cls_params:
       initial_step: 0
       loss_load_cost: 10
+      normalized_action_bounds:
+      - 0
+      - 1
       overgeneration_cost: 1
       raise_errors: false
     name:
     - unbalanced_energy
     - 0
     state:
       _current_step: 0
@@ -52,18 +61,21 @@
     cls_params:
       allow_abortion: true
       co2_per_unit: 2
       cost_per_unit_co2: 0.1
       genset_cost: 0.4
       init_start_up: true
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: genset_production
       raise_errors: false
-      running_max_production: 11798.1
-      running_min_production: 655.45
+      running_max_production: 17296.2
+      running_min_production: 960.9000000000001
       start_up_time: 0
       wind_down_time: 0
     name:
     - genset
     - 0
     state:
       _current_status: true
@@ -71,25 +83,28 @@
       _goal_status: true
       _steps_until_down: 0
       _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
-      battery_transition_model: null
+      battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
       init_soc: 1
       initial_step: 0
-      max_capacity: 19334
-      max_charge: 4834
-      max_discharge: 4834
-      min_capacity: 3866.8
+      max_capacity: 26153
+      max_charge: 6539
+      max_discharge: 6539
+      min_capacity: 5230.6
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
-      current_charge: 19334
+      current_charge: 26153
       soc: 1.0
 trajectory_func: null
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:43 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:47 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:43 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:47 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:43 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:47 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_8/microgrid_8.yaml` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_16/microgrid_16.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/LoadModule/time_series.csv.gz'
     name:
     - load
     - 0
     state:
       _current_step: 0
@@ -23,91 +26,79 @@
     cls_params:
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
+      normalized_action_bounds:
+      - 0
+      - 1
       provided_energy_name: renewable_used
       raise_errors: false
       time_series: !NDArray 'data/cls_params/RenewableModule/time_series.csv.gz'
     name:
     - pv
     - 0
     state:
       _current_step: 0
 - - unbalanced_energy
   - !UnbalancedEnergyModule
     cls_params:
       initial_step: 0
       loss_load_cost: 10
+      normalized_action_bounds:
+      - 0
+      - 1
       overgeneration_cost: 1
       raise_errors: false
     name:
     - unbalanced_energy
     - 0
     state:
       _current_step: 0
-- - genset
-  - !Genset
-    cls_params:
-      allow_abortion: true
-      co2_per_unit: 2
-      cost_per_unit_co2: 0.1
-      genset_cost: 0.4
-      init_start_up: true
-      initial_step: 0
-      provided_energy_name: genset_production
-      raise_errors: false
-      running_max_production: 64065.6
-      running_min_production: 3559.2000000000003
-      start_up_time: 0
-      wind_down_time: 0
-    name:
-    - genset
-    - 0
-    state:
-      _current_status: true
-      _current_step: 0
-      _goal_status: true
-      _steps_until_down: 0
-      _steps_until_up: 0
 - - battery
   - !BatteryModule
     cls_params:
       battery_cost_cycle: 0.02
-      battery_transition_model: null
+      battery_transition_model: !BatteryTransitionModel {}
       efficiency: 0.9
       init_charge: null
-      init_soc: 0.2
+      init_soc: 0.534118811938557
       initial_step: 0
-      max_capacity: 105583
-      max_charge: 26396
-      max_discharge: 26396
-      min_capacity: 21116.600000000002
+      max_capacity: 60099
+      max_charge: 15025
+      max_discharge: 15025
+      min_capacity: 12019.800000000001
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
     name:
     - battery
     - 0
     state:
       _current_step: 0
-      current_charge: 21116.600000000002
-      soc: 0.2
+      current_charge: 32100.00647869534
+      soc: 0.534118811938557
 - - grid
   - !GridModule
     cls_params:
       cost_per_unit_co2: 0.1
       final_step: 8759
       forecast_horizon: 23
       forecaster: oracle
       forecaster_increase_uncertainty: false
       forecaster_relative_noise: false
       initial_step: 0
-      max_export: 128130
-      max_import: 128130
+      max_export: 97244
+      max_import: 97244
+      normalized_action_bounds:
+      - 0
+      - 1
       raise_errors: false
       time_series: !NDArray 'data/cls_params/GridModule/time_series.csv.gz'
     name:
     - grid
     - 0
     state:
       _current_step: 0
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/GridModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/GridModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:44 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:47 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/LoadModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/LoadModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:44 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:47 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/RenewableModule/time_series.csv.gz` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25/microgrid_9/data/cls_params/RenewableModule/time_series.csv.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_series.csv", last modified: Fri Mar  3 19:54:44 2023, max compression
+gzip compressed data, was "time_series.csv", last modified: Wed Apr 19 21:34:47 2023, max compression
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/data/scenario/pymgrid25.pkl` & `python-microgrid-1.4.0/src/pymgrid/data/scenario/pymgrid25.pkl`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/envs/base/base.py` & `python-microgrid-1.4.0/src/pymgrid/envs/base/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import numpy as np
 import pandas as pd
 
 from gym import Env
 from gym.spaces import Box, Dict, Tuple, flatten_space, flatten
 from abc import abstractmethod
 
 from pymgrid import NonModularMicrogrid, Microgrid
@@ -50,14 +51,20 @@
     trajectory_func : callable or None, default None
         Callable that sets an initial and final step for an episode. ``trajectory_func`` must take two inputs:
         :attr:`.initial_step` and :attr:`.final_step`, and return two integers: the initial and final step for
         that particular episode, respectively. This function will be called every time :meth:`.reset` is called.
 
         If None, :attr:`.initial_step` and :attr:`.final_step` are used to define every episode.
 
+    step_callback: callable or None, default None
+        Function to call on every ``step``.
+
+    reset_callback: callable or None, default None
+        Function to call on every ``reset``.
+
     """
 
     action_space = None
     'Space object corresponding to valid actions.'
 
     observation_space = None
     'Space object corresponding to valid observations.'
@@ -86,26 +93,30 @@
                  modules,
                  add_unbalanced_module=True,
                  loss_load_cost=10,
                  overgeneration_cost=2,
                  reward_shaping_func=None,
                  trajectory_func=None,
                  flat_spaces=True,
-                 observation_keys=()
+                 observation_keys=(),
+                 step_callback=None,
+                 reset_callback=None
                  ):
 
         super().__init__(modules,
                          add_unbalanced_module=add_unbalanced_module,
                          loss_load_cost=loss_load_cost,
                          overgeneration_cost=overgeneration_cost,
                          reward_shaping_func=reward_shaping_func,
                          trajectory_func=trajectory_func)
 
         self._flat_spaces = flat_spaces
         self.observation_keys = self._validate_observation_keys(observation_keys)
+        self.step_callback = step_callback if step_callback is not None else lambda *a, **k: None
+        self.reset_callback = reset_callback if reset_callback is not None else lambda *a, **k: None
 
         self.action_space = self._get_action_space()
         self.observation_space, self._nested_observation_space = self._get_observation_space()
 
     def _validate_observation_keys(self, keys):
         if not keys:
             return keys
@@ -154,37 +165,43 @@
                             dtype=normalized_space.dtype
                         )
 
                         tup.append(box_slice)
             if tup:
                 obs_space[name] = Tuple(tup)
 
+        if self.observation_keys and 'net_load' in self.observation_keys:
+            obs_space['net_load'] = Tuple([Box(low=-np.inf, high=1, shape=(1, ), dtype=np.float64)])
+
         obs_space = Dict(obs_space)
 
         return (flatten_space(obs_space) if self._flat_spaces else obs_space), obs_space
 
     def potential_observation_keys(self):
         return self.state_series().index.get_level_values(-1).unique()
 
     def reset(self):
         obs = super().reset()
+        obs.pop('balance')
+        obs.pop('other')
+        self.reset_callback()
         return self._get_obs(obs)
 
     def step(self, action, normalized=True):
         """
         Run one timestep of the environment's dynamics.
 
         When the end of the episode is reached, you are responsible for calling `reset()`
         to reset the environment's state.
 
         Accepts an action and returns a tuple (observation, reward, done, info).
 
         Parameters
         ----------
-        action : dict[str, list[float]]
+        action : int or np.ndarray
             An action provided by the agent.
 
         normalized : bool, default True
             Whether the passed action is normalized or not.
 
         Returns
         -------
@@ -200,38 +217,142 @@
         done : bool
             Whether the microgrid terminates.
 
         info : dict
             Additional information from this step.
 
         """
+        action = self.convert_action(action)
+        self._log_action(action, normalized)
 
         obs, reward, done, info = self.run(action, normalized=normalized)
-
         obs = self._get_obs(obs)
+        self.step_callback(**self._get_step_callback_info(action, obs, reward, done, info))
 
         return obs, reward, done, info
 
+    @abstractmethod
+    def convert_action(self, action):
+        """
+        Convert a reinforcement learning action to a microgrid control.
+
+        In a discrete environment, for example, converts an integer to a microgrid control.
+
+        Parameters
+        ----------
+        action : int, np.ndarray or dict
+            Action to convert. Integer if discrete, np.ndarray if continuous,
+            dict if converting from a microgrid action.
+
+        Returns
+        -------
+        converted_action : dict[str, list[float]]
+            Resultant microgrid control.
+        """
+        pass
+
+    def _log_action(self, action, normalized, log_column='converted_action'):
+        d = {}
+
+        log_items = [(log_column, action)]
+
+        if normalized:
+            log_items.append((f'denormalized_{log_column}', self.microgrid_action_space.denormalize(action)))
+
+        for key, action in log_items:
+            for module, action_list in action.items():
+                for j, act in enumerate(action_list):
+                    if not pd.api.types.is_list_like(act):
+                        act = [act]
+                    d.update({(key, j, f'{module}_{el_num}'): act_n for el_num, act_n in enumerate(act)})
+
+        self._microgrid_logger.log(d)
+
     def _get_obs(self, obs):
         if self.observation_keys:
             obs = self.state_series(normalized=True).loc[pd.IndexSlice[:, :, self.observation_keys]]
 
             if self._flat_spaces:
                 obs = obs.values
             else:
                 obs = obs.to_frame().unstack(level=1).T.droplevel(level=1, axis=1).to_dict(orient='list')
 
         elif self._flat_spaces:
-            obs = flatten(self._nested_observation_space, obs)
+            obs = self.flatten_obs(self._nested_observation_space, obs)
 
         return obs
 
+    def _get_step_callback_info(self, action, obs, reward, done, info):
+        return {
+            'action': action,
+            'obs': obs,
+            'reward': reward,
+            'done': done,
+            'info': info
+        }
+
     def render(self, mode="human"):
         """:meta private:"""
-        raise NotImplementedError
+        raise RuntimeError('rendering is not possible in Microgrid environments.')
+
+    def sample_action(self, strict_bound=False, sample_flex_modules=False):
+        return self.action_space.sample()
+
+    def compute_net_load(self, normalized=False):
+        """
+        Compute the net load at the current step.
+
+        Net load is load minus renewables.
+        -------
+
+        Returns
+        -------
+        net_load : float
+            Net load.
+
+        """
+
+        if self.current_step == self.final_step:
+            return 0.0
+
+        try:
+            fixed_consumption = self.modules.fixed.get_attrs('max_consumption', as_pandas=False, drop_attr_names=True)
+            fixed_consumption = np.sum(list(fixed_consumption.values()))
+        except AttributeError:
+            fixed_consumption = 0.0
+
+        flex_max_prod = [m.max_production for m in self.modules.flex.iterlist() if m.marginal_cost == 0]
+        flex_production = sum(flex_max_prod)
+
+        net_load = fixed_consumption - flex_production
+
+        if normalized:
+            if fixed_consumption:
+                return net_load / fixed_consumption
+            return -1.0
+
+        return net_load
+
+    def state_dict(self, normalized=False, as_run_output=False):
+        sd = super().state_dict(normalized=normalized, as_run_output=as_run_output)
+
+        net_load = self.compute_net_load(normalized=normalized)
+
+        if as_run_output:
+            net_load_entry = np.array([net_load])
+        else:
+            net_load_entry = {'net_load': net_load}
+
+        sd['general'] = [net_load_entry]
+
+        return sd
+
+    @staticmethod
+    def flatten_obs(observation_space, obs):
+        return np.concatenate([flatten(observation_space[k], v) for k, v in obs.items()])
 
     @property
     def unwrapped(self):
         """:meta private:"""
         return super().unwrapped
 
     @property
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/envs/discrete/discrete.py` & `python-microgrid-1.4.0/src/pymgrid/envs/discrete/discrete.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,24 +40,28 @@
                  add_unbalanced_module=True,
                  loss_load_cost=10,
                  overgeneration_cost=2,
                  reward_shaping_func=None,
                  trajectory_func=None,
                  flat_spaces=True,
                  observation_keys=None,
-                 remove_redundant_gensets=True
+                 remove_redundant_gensets=True,
+                 step_callback=None,
+                 reset_callback=None
                  ):
         super().__init__(modules,
                          add_unbalanced_module=add_unbalanced_module,
                          loss_load_cost=loss_load_cost,
                          overgeneration_cost=overgeneration_cost,
                          reward_shaping_func=reward_shaping_func,
                          trajectory_func=trajectory_func,
                          flat_spaces=flat_spaces,
-                         observation_keys=observation_keys)
+                         observation_keys=observation_keys,
+                         step_callback=step_callback,
+                         reset_callback=reset_callback)
 
         self.action_space, self.actions_list = self._get_action_space(remove_redundant_gensets)
 
     def _get_action_space(self, remove_redundant_gensets=False):
         """
         An action here is a priority list - in what order to deploy controllable source modules.
         Compute the total expected load
@@ -75,19 +79,21 @@
             warn(f'Microgrid with {len(priority_lists[0])} fixed source modules defines large action space with '
                  f'{n_actions} elements.')
 
         space = Discrete(n_actions)
 
         return space, priority_lists
 
-    def _get_action(self, action_num):
-        if action_num not in self.action_space:
-            raise ValueError(f" Action {action_num} not in action space {self.action_space}")
+    def convert_action(self, action):
+        if action not in self.action_space:
+            raise ValueError(f" Action {action} not in action space {self.action_space}")
 
-        priority_list = list(self.actions_list[action_num])
+        self._microgrid_logger.log(action=action)
+
+        priority_list = list(self.actions_list[action])
 
         return self._populate_action(priority_list)
 
     def remove_action(self, action_number):
         """
         Remove an action from the action space.
 
@@ -134,19 +140,19 @@
         done : bool
             Whether the microgrid terminates.
 
         info : dict
             Additional information from this step.
 
         """
-        self._microgrid_logger.log(action=action)
-        microgrid_action = self._get_action(action)
-        return super().step(microgrid_action, normalized=False)
+        return super().step(action, normalized=False)
 
-    def sample_action(self, strict_bound=False, sample_flex_modules=False):
-        return self.action_space.sample()
+    def _get_step_callback_info(self, action, obs, reward, done, info):
+        info = super()._get_step_callback_info(action, obs, reward, done, info)
+        info['action'] = self._microgrid_logger['action'][-1]
+        return info
 
     def __repr__(self):
         return f"DiscreteMicrogridEnv({super().__repr__()}"
 
     def __str__(self):
         return self.__repr__()
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/forecast/forecaster.py` & `python-microgrid-1.4.0/src/pymgrid/forecast/forecaster.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         )
         self._forecast_shaped_space = self._get_forecast_shaped_space(new_shape)
 
     def __eq__(self, other):
         if type(self) != type(other):
             return NotImplemented
 
-        return (self._fill_arr == other._fill_arr).all() and \
+        return np.array_equal(self._fill_arr, other._fill_arr) and \
                all(v == other.__dict__[k] for k, v in self.__dict__.items() if k != '_fill_arr')
 
     def __call__(self, val_c, val_c_n, n):
         if len(val_c_n.shape) == 1:
             val_c_n = val_c_n.reshape((-1, 1))
 
         if val_c_n.shape[0] > self._forecast_shaped_space.shape[0]:
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/microgrid/convert_scenario_sandbox.py` & `python-microgrid-1.4.0/src/pymgrid/microgrid/convert_scenario_sandbox.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/microgrid/microgrid.py` & `python-microgrid-1.4.0/src/pymgrid/microgrid/microgrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 import yaml
 
 from copy import deepcopy
 from warnings import warn
 
 from pymgrid.microgrid import DEFAULT_HORIZON
 from pymgrid.modules import ModuleContainer, UnbalancedEnergyModule
-from pymgrid.utils.logger import ModularLogger
 from pymgrid.microgrid.utils.step import MicrogridStep
+from pymgrid.utils.eq import verbose_eq
+from pymgrid.utils.logger import ModularLogger
 from pymgrid.utils.serialize import add_numpy_pandas_representers, add_numpy_pandas_constructors, dump_data
 from pymgrid.utils.space import MicrogridSpace
 
+
 class Microgrid(yaml.YAMLObject):
     """
     Microgrid class, used to define and simulate an environment with a variety of modules.
 
     Parameters
     ----------
     modules : List[Union[Tuple[str, BaseMicrogridModule], BaseMicrogridModule]]
@@ -107,18 +109,17 @@
 
         self._modules = self._get_module_container(modules,
                                                    add_unbalanced_module,
                                                    loss_load_cost,
                                                    overgeneration_cost)
 
         # TODO (ahalev) transform envs to wrappers, and remove microgrid from attr names)
-        self.microgrid_action_space = MicrogridSpace(
-            self._modules.get_attrs('action_space', 'module_type', as_pandas=False), 'act'
-        )
-        self.microgrid_observation_space = MicrogridSpace(
+        self.microgrid_action_space = MicrogridSpace.from_module_spaces(
+            self._modules.get_attrs('action_space', 'module_type', as_pandas=False), 'act')
+        self.microgrid_observation_space = MicrogridSpace.from_module_spaces(
             self._modules.get_attrs('observation_space', as_pandas=False), 'obs'
         )
 
         self._initial_step = self._get_module_initial_step()
         self._final_step = self._get_module_final_step()
 
         self.reward_shaping_func = reward_shaping_func
@@ -473,20 +474,40 @@
                     _log_dict[(name, j, key)] = value
 
         _log_dict = dict(sorted(_log_dict.items(), key=lambda k: k[0]))
 
         for key, value in self._balance_logger.to_dict().items():
             _log_dict[('balance', 0, key)] = value
 
+        pad = (0, '')
+
         for key, value in self._microgrid_logger.items():
-            _log_dict[(key, 0, '')] = value
+            key = key if pd.api.types.is_list_like(key) else [key]
+            _log_dict[(*key, *pad[len(key)-1:])] = value
 
         col_names = ['module_name', 'module_number', 'field']
 
-        df = pd.DataFrame(_log_dict, index=pd.RangeIndex(start=self.initial_step, stop=self.current_step))
+        initial_step = self._modules.get_attrs('initial_step', unique=True)
+
+        try:
+            df = pd.DataFrame(_log_dict, index=pd.RangeIndex(start=initial_step, stop=self.current_step))
+        except ValueError as e:
+            if 'Length of values' in e.args[0]:
+                module_log_lengths = pd.Series([len(log_dict) for log_dict in _log_dict.values()])
+
+                msg = f"Length of module log dicts ({module_log_lengths.unique().item()}) " \
+                      f"do not match self.current_step-initial_step ({self.current_step-initial_step}). " \
+                      f"Did you set a trajectory attribute " \
+                      f"('initial_step', 'final_step', 'trajectory_func') without calling Microgrid.reset()?"
+
+                raise ValueError(msg)
+
+            else:
+                raise
+
         df.columns = pd.MultiIndex.from_tuples(df.columns.to_list(), names=col_names)
 
         if drop_forecasts:
             df = df.drop(columns=df.columns[df.columns.get_level_values(-1).str.contains('forecast')])
 
         if drop_singleton_key:
             cols = df.columns
@@ -635,15 +656,15 @@
         Current step of underlying modules.
 
         Returns
         -------
         current_step : int
             Current step.
         """
-        return self._modules.get_attrs('current_step', unique=True).item()
+        return self._modules.get_attrs('current_step', unique=True)
 
     @property
     def initial_step(self):
         """
         Initial step at which to start underlying timeseries data.
 
         The step to which :attr:`.current_step` is reset to when calling :meth:`.reset`.
@@ -652,20 +673,18 @@
         -------
         initial_step : int
             Initial step.
         """
         return self._initial_step
 
     def _get_module_initial_step(self):
-        initial_step = self.modules.get_attrs('initial_step', unique=True)
         try:
-            return initial_step.item()
-        except ValueError:
-            if initial_step.empty:
-                return 0
+            return self.modules.get_attrs('initial_step', unique=True)
+        except AttributeError:
+            return 0
 
     @initial_step.setter
     def initial_step(self, value):
         self._set_initial_step(value)
 
     def _set_initial_step(self, value, modules_only=False):
         self.set_module_attrs(initial_step=value)
@@ -681,20 +700,18 @@
         -------
         final_step : int
             Final step.
         """
         return self._final_step
 
     def _get_module_final_step(self):
-        final_step = self.modules.get_attrs('final_step', unique=True)
         try:
-            return final_step.item()
-        except ValueError:
-            if final_step.empty:
-                return np.inf
+            return self.modules.get_attrs('final_step', unique=True)
+        except AttributeError:
+            return np.inf
 
     @final_step.setter
     def final_step(self, value):
         self._set_final_step(value)
 
     def _set_final_step(self, value, modules_only=False):
         self.set_module_attrs(final_step=value)
@@ -710,33 +727,43 @@
         -------
         modules : :class:`pymgrid.modules.module_container.ModuleContainer`
             View of the container.
 
         """
         return self._modules
 
-    def state_dict(self, normalized=False):
+    def state_dict(self, normalized=False, as_run_output=False):
         """
         State of the microgrid as a dict.
 
         Keys are module names and values are lists of state dicts for all modules with said name.
 
         Parameters
         ----------
         normalized : bool, default False
             Whether to return a dict of normalized values.
 
+        as_run_output : bool, default False
+            Whether to return output in the same format as the output of :meth:`Microgrid.run`.
+            Inner values are numpy arrays and not dict in this case.
+
+
         Returns
         -------
-        state_dict : dict[str, list[dict]]
+        state_dict : dict[str, list[dict]] or dict[str[list[np.ndarray]]]
             State of the microgrid as a nested dict.
 
         """
+        def as_run_output_f(state_dict):
+            if as_run_output:
+                return np.array(list(state_dict.values()))
+            return state_dict
+
         return {name: [
-            module.state_dict(normalized=normalized) for module in modules
+            as_run_output_f(module.state_dict(normalized=normalized)) for module in modules
         ] for name, modules in self._modules.iterdict()}
 
     @property
     def log(self):
         """
         Microgrid's log as a DataFrame.
 
@@ -1003,14 +1030,17 @@
 
     def _dir_additions(self):
         return {
             x for x in dir(self._modules) if
             not x.startswith('_') and not callable(getattr(self._modules, x)) and x in self._modules
         }
 
+    def verbose_eq(self, other, indent=0):
+        verbose_eq(self, other, ('_balance_logger', 'trajectory_func', *self._modules.names()), indent=indent)
+
     def __dir__(self):
         rv = set(super().__dir__())
         rv = rv | self._dir_additions()
         return sorted(rv)
 
     def __getnewargs__(self):
         return (self.modules.to_tuples(), )
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/microgrid/modular_microgrid_sandbox.py` & `python-microgrid-1.4.0/src/pymgrid/microgrid/modular_microgrid_sandbox.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/microgrid/reward_shaping/base.py` & `python-microgrid-1.4.0/src/pymgrid/microgrid/reward_shaping/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,12 +12,12 @@
         try:
             module_info = info[module_name]
             return sum([d[module_attr] for d in module_info])
         except KeyError:
             return 0.0
 
     @abstractmethod
-    def __call__(self, step_info, cost_info):
+    def __call__(self, original_reward, step_info, cost_info):
         pass
 
     def __repr__(self):
         return f'{self.__class__.__name__}()'
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/microgrid/reward_shaping/battery_discharge_shaper.py` & `python-microgrid-1.4.0/src/pymgrid/microgrid/reward_shaping/battery_discharge_shaper.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     microgrid:
         attributes:
             reward_shaping_func: !BatteryDischargeShaper {}
 
     """
     yaml_tag = u"!BatteryDischargeShaper"
 
-    def __call__(self, step_info, cost_info):
+    def __call__(self, original_reward, step_info, cost_info):
         battery_discharge = self.sum_module_val(step_info, 'battery', 'provided_energy')
         load = self.sum_module_val(step_info, 'load', 'absorbed_energy')
         loss_load = self.sum_module_val(step_info, 'unbalanced_energy', 'provided_energy')
 
         # battery_discharge is in [0, load-loss_load]; loss_load is in [0, load].
         try:
             percent_battery = (battery_discharge - loss_load) / load
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/microgrid/trajectory/base.py` & `python-microgrid-1.4.0/src/pymgrid/microgrid/trajectory/base.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/microgrid/trajectory/stochastic.py` & `python-microgrid-1.4.0/src/pymgrid/microgrid/trajectory/stochastic.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/microgrid/utils/step.py` & `python-microgrid-1.4.0/src/pymgrid/microgrid/utils/step.py`

 * *Files 13% similar despite different names*

```diff
@@ -35,19 +35,22 @@
         absorbed_energy = np.sum(self._info['absorbed_energy'])
         return provided_energy, absorbed_energy, self._reward, self.shaped_reward()
 
     def output(self):
         return self._obs, self.shaped_reward(), self._done, self._output_info()
 
     def shaped_reward(self):
-        if self._reward_shaping_func is not None:
-            assert isinstance(self.cost_info, dict)
-            return self._reward_shaping_func(self._output_info(), self.cost_info)
+        if self._reward_shaping_func is None:
+            return self._reward
+        elif not callable(self._reward_shaping_func):
+            raise TypeError(f'reward_shaping_func {self._reward_shaping_func} is not callable.')
+
+        assert isinstance(self.cost_info, dict)
+        return self._reward_shaping_func(self._reward, self._output_info(), self.cost_info)
 
-        return self._reward
 
     def _output_info(self):
         return {k: v for k, v in self._info.items() if k not in ('absorbed_energy', 'provided_energy')}
 
     @property
     def obs(self):
         return self._obs
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/modules/base/base_module.py` & `python-microgrid-1.4.0/src/pymgrid/modules/base/base_module.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import inspect
 import logging
 import yaml
 import numpy as np
 
 from warnings import warn
 
+from pymgrid.utils.eq import verbose_eq
 from pymgrid.utils.logger import ModularLogger
 from pymgrid.utils.space import ModuleSpace
 from pymgrid.utils.serialize import add_numpy_pandas_representers, add_numpy_pandas_constructors, dump_data
 
 
 script_logger = logging.getLogger(__name__)
 
@@ -33,32 +34,34 @@
     """
 
     _energy_pos = 0
 
     def __init__(self,
                  raise_errors,
                  initial_step=0,
+                 normalized_action_bounds=(0, 1),
                  provided_energy_name='provided_energy',
                  absorbed_energy_name='absorbed_energy'
                  ):
 
         self.raise_errors = raise_errors
         self.initial_step = initial_step
         self._current_step = initial_step
-        self._action_space = self._get_action_spaces()
+        self._action_space = self._get_action_spaces(normalized_action_bounds)
         self._observation_space = self._get_observation_spaces()
         self.provided_energy_name, self.absorbed_energy_name = provided_energy_name, absorbed_energy_name
         self._logger = ModularLogger()
-        self.name = (None, None)  # set by ModularMicrogrid
+        self.name = None  # set by ModularMicrogrid
 
-    def _get_action_spaces(self):
+    def _get_action_spaces(self, normalized_bounds):
         unnormalized_low = self.min_act if isinstance(self.min_act, np.ndarray) else np.array([self.min_act])
         unnormalized_high = self.max_act if isinstance(self.max_act, np.ndarray) else np.array([self.max_act])
         return ModuleSpace(unnormalized_low=unnormalized_low,
-                           unnormalized_high=unnormalized_high)
+                           unnormalized_high=unnormalized_high,
+                           normalized_bounds=normalized_bounds)
 
     def _get_observation_spaces(self):
         unnormalized_low = self.min_obs if isinstance(self.min_obs, np.ndarray) else np.array([self.min_obs])
         unnormalized_high = self.max_obs if isinstance(self.max_obs, np.ndarray) else np.array([self.max_obs])
         return ModuleSpace(unnormalized_low=unnormalized_low,
                            unnormalized_high=unnormalized_high)
 
@@ -199,17 +202,14 @@
         ------
         AssertionError
             If ``energy_demand<0`` or the module is not a source.
 
         """
 
         assert energy_demand >= 0
-        assert self.is_source, f'step() was called with positive energy (source) for module {self} but ' \
-                               f'module is not a source and ' \
-                               f'can only be called with negative energy.'
 
         if self.module_type[-1] == 'fixed':
             return self.update(None, as_source=True)
 
         if energy_demand > self.max_production:
             if self.raise_errors:
                 self._raise_error(energy_demand, self.max_production, as_source=True)
@@ -298,16 +298,16 @@
     @abstractmethod
     def update(self, external_energy_change, as_source=False, as_sink=False):
         """
         Update the state of the module given an energy request.
 
         Parameters
         ----------
-        external_energy_change : float or None
-            Amount of energy to provide or absorb.
+        external_energy_change : float >= 0 or None
+            Amount of energy to provide or absorb. A non-negative number.
         as_source : bool
             Whether the module is acting as a source.
         as_sink
             Whether the module is acting as a sink.
 
         Returns
         -------
@@ -401,14 +401,33 @@
         """
         assert act + obs == 1, 'One of act or obs must be True but not both.'
         if act:
             return self._action_space.denormalize(value)
         if obs:
             return self._observation_space.denormalize(value)
 
+    def dynamic_action_space(self):
+        """
+        An action space bounded by the current step's maximum consumption and production.
+
+        This is useful for checking if an action satisfies production or consumption limits in a given step.
+        It can also be used for clipping actions to these bounds by using :meth:`.ModuleSpace.clip`.
+
+        Returns
+        -------
+
+        action_space : :class:`.ModuleSpace`
+            A space with bounds for the current step.
+
+        """
+        return ModuleSpace(unnormalized_low=-1*self.max_consumption,
+                           unnormalized_high=self.max_production,
+                           normalized_bounds=self.normalized_action_bounds,
+                           shape=self._action_space.shape)
+
     def log_dict(self):
         """
         Module's log as a dict.
 
         Returns
         -------
         dict
@@ -620,37 +639,35 @@
 
     @property
     def max_production(self):
         """
         Maximum amount of production at the current time step.
 
         Must be defined in any child class that is a source.
-        If the module is not a source, this value is irrelevant.
 
         Returns
         -------
         float
 
         """
-        return NotImplemented
+        return 0.0
 
     @property
     def max_consumption(self):
         """
         Maximum amount of consumption at the current time step.
 
         Must be defined in any child class that is a sink.
-        If the module is not a sink, this value is irrelevant.
 
         Returns
         -------
         float
 
         """
-        return NotImplemented
+        return 0.0
 
     @property
     def marginal_cost(self):
         """
         Average marginal cost of producing with the module.
 
         Returns
@@ -694,14 +711,57 @@
         -------
         observation_space : :class:`ModuleSpace <pymgrid.utils.space.ModuleSpace>`
             The observation space.
         """
         return self._observation_space
 
     @property
+    def normalized_action_bounds(self):
+        """
+        Bounds that actions are normalized to in the action space.
+
+        This property is necessary for serialization.
+
+        :meta private:
+
+        Returns
+        -------
+        normalized_action_bounds : tuple
+            Normalized bounds
+        """
+
+        low = np.unique(self._action_space.normalized.low)
+        high = np.unique(self._action_space.normalized.high)
+
+        try:
+            low = low.item()
+            high = high.item()
+        except ValueError:
+            if not self._action_space.shape == (0, ):
+                raise
+            low, high = 0, 1
+
+        if isinstance(low, float) and low.is_integer():
+            low = int(low)
+
+        if isinstance(high, float) and high.is_integer():
+            high = int(high)
+
+        return low, high
+
+    @normalized_action_bounds.setter
+    def normalized_action_bounds(self, value):
+        if len(value) != 2:
+            raise TypeError('Invalid number of components.')
+        if value[0] > value[1]:
+            raise ValueError('Low value cannot be greater than high value.')
+
+        self._action_space = self._get_action_spaces(value)
+
+    @property
     def is_source(self):
         """
         Whether the module is a source.
 
         Returns
         -------
         bool
@@ -952,20 +1012,38 @@
             except KeyError:
                 raise KeyError(f"Missing key {attr_name} in deserialized dict.")
 
         if len(serialized_dict):
             warn(f"Unused keys in serialized_dict: {list(serialized_dict.keys())}")
         return self
 
+    def verbose_eq(self, other, indent=0):
+        return verbose_eq(self, other, self.__dict__.keys(), indent=indent)
+
     def __eq__(self, other):
         if type(self) != type(other):
             return NotImplemented
 
-        diff = [(k1, v1, v2) for (k1, v1), (k2, v2) in zip(self.__dict__.items(), other.__dict__.items()) if
-                ((hasattr(v1, "any") and not np.allclose(v1, v2)) or (not hasattr(v1, "any") and v1 != v2))]
+        def are_equal(v1, v2):
+            try:
+                _are_equal = bool(v1 == v2)
+                if _are_equal:
+                    return True
+            except ValueError:
+                pass
+
+            try:
+                return np.allclose(v1, v2)
+            except (ValueError, TypeError):
+                return False
+
+        diff = [
+            (k1, v1, v2) for (k1, v1), (k2, v2) in zip(self.__dict__.items(), other.__dict__.items())
+            if not are_equal(v1, v2)
+        ]
 
         return len(diff) == 0
 
     def __repr__(self):
         param_repr = {p: getattr(self, p) for p in inspect.signature(self.__init__).parameters}
         param_repr = [f'{p}={type(v) if hasattr(v, "__len__") and not isinstance(v, str) else v}' for p, v in param_repr.items()]
         param_repr = ', '.join(param_repr)
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/modules/base/timeseries/base_timeseries_module.py` & `python-microgrid-1.4.0/src/pymgrid/modules/base/timeseries/base_timeseries_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
                  raise_errors,
                  forecaster=None,
                  forecast_horizon=DEFAULT_HORIZON,
                  forecaster_increase_uncertainty=False,
                  forecaster_relative_noise=False,
                  initial_step=0,
                  final_step=-1,
+                 normalized_action_bounds=(0, 1),
                  provided_energy_name='provided_energy',
                  absorbed_energy_name='absorbed_energy',
                  normalize_pos=...):
 
         self._time_series = self._set_time_series(time_series)
         self._min_obs, self._max_obs, self._min_act, self._max_act = self._get_bounds()
 
@@ -46,14 +47,15 @@
                                           increase_uncertainty=forecaster_increase_uncertainty,
                                           relative_noise=forecaster_relative_noise)
 
         self._state_dict_keys = self._set_state_dict_keys()
 
         super().__init__(raise_errors,
                          initial_step=initial_step,
+                         normalized_action_bounds=normalized_action_bounds,
                          provided_energy_name=provided_energy_name,
                          absorbed_energy_name=absorbed_energy_name)
 
         self._current_forecast = self.forecast()
 
     def _set_time_series(self, time_series):
         _time_series = np.array(time_series)
@@ -152,15 +154,15 @@
         """
         return self._time_series
 
     @time_series.setter
     def time_series(self, value):
         self._time_series = self._set_time_series(value)
         self._min_obs, self._max_obs, self._min_act, self._max_act = self._get_bounds()
-        self._action_space = self._get_action_spaces()
+        self._action_space = self._get_action_spaces(self.normalized_action_bounds)
         self._observation_space = self._get_observation_spaces()
 
     @property
     def min_obs(self):
         # TODO find a better solution
         return np.repeat(np.array(self._min_obs).reshape((-1, 1)), 1+self._forecast_horizon, axis=1).T.reshape(-1)
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/modules/battery/battery_module.py` & `python-microgrid-1.4.0/src/pymgrid/modules/battery/battery_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,31 +84,32 @@
                  max_discharge,
                  efficiency,
                  battery_cost_cycle=0.0,
                  battery_transition_model=None,
                  init_charge=None,
                  init_soc=None,
                  initial_step=0,
+                 normalized_action_bounds=(0, 1),
                  raise_errors=False):
         assert 0 < efficiency <= 1
         self.min_capacity = min_capacity
         self.max_capacity = max_capacity
         self.max_charge = max_charge
         self.max_discharge = max_discharge
         self.efficiency = efficiency
         self.battery_cost_cycle = battery_cost_cycle
         self.battery_transition_model = battery_transition_model
         self.min_soc, self.max_soc = min_capacity/max_capacity, 1
         self.init_charge, self.init_soc = init_charge, init_soc
         self._current_charge, self._soc = self._init_battery(init_charge, init_soc)
         self._min_act, self._max_act = self._set_min_max_act()
-        self.name = ('battery', None)
 
         super().__init__(raise_errors,
                          initial_step=initial_step,
+                         normalized_action_bounds=normalized_action_bounds,
                          provided_energy_name='discharge_amount',
                          absorbed_energy_name='charge_amount')
 
     def _init_battery(self, init_charge, init_soc):
         if init_charge is not None:
             if init_soc is not None:
                 warn('Passed both init_capacity and init_soc. Using init_charge and ignoring init_soc')
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/modules/battery/transition_models/biased_transition_model.py` & `python-microgrid-1.4.0/src/pymgrid/modules/battery/transition_models/biased_transition_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,9 +21,7 @@
         else:
             self.efficiency = self.true_efficiency
 
     def transition(self, external_energy_change, efficiency, **kwargs):
         self._set_efficiency(efficiency)
         return super().transition(external_energy_change=external_energy_change,
                                   efficiency=self.efficiency)
-
-# Can do this: yaml.safe_load('!BiasedTransitionModel {true_efficiency: 0.5}')
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/modules/battery/transition_models/decay_transition_model.py` & `python-microgrid-1.4.0/src/pymgrid/modules/battery/transition_models/decay_transition_model.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/modules/battery/transition_models/transition_model.py` & `python-microgrid-1.4.0/src/pymgrid/modules/battery/transition_models/transition_model.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/modules/genset_module.py` & `python-microgrid-1.4.0/src/pymgrid/modules/genset_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,14 +65,15 @@
                  co2_per_unit=0.0,
                  cost_per_unit_co2=0.0,
                  start_up_time=0,
                  wind_down_time=0,
                  allow_abortion=True,
                  init_start_up=True,
                  initial_step=0,
+                 normalized_action_bounds=(0, 1),
                  raise_errors=False,
                  provided_energy_name='genset_production'):
 
         if running_min_production > running_max_production:
             raise ValueError('parameter min_production must not be greater than parameter max_production.')
 
         if not allow_abortion:
@@ -86,18 +87,18 @@
         self.start_up_time = start_up_time
         self.wind_down_time = wind_down_time
         self.allow_abortion = allow_abortion
         self.init_start_up = init_start_up
 
         self._current_status, self._goal_status = int(init_start_up), int(init_start_up)
         self._steps_until_up, self._steps_until_down = self._reset_up_down_times()
-        self.name = ('genset', None)
 
         super().__init__(raise_errors,
                          initial_step=initial_step,
+                         normalized_action_bounds=normalized_action_bounds,
                          provided_energy_name=provided_energy_name,
                          absorbed_energy_name=None)
 
     def step(self, action, normalized=True):
         """
         Take one step in the module, attempting to draw a certain amount of energy from the genset.
 
@@ -139,18 +140,24 @@
             Whether the module terminates.
         info : dict
             Additional information from this step.
             Will include either `provided_energy` or `absorbed_energy` as a key, denoting the amount of energy
             this module provided to or absorbed from the microgrid.
 
         """
-        goal_status = action[0]
+        if normalized:
+            denormalized = self._action_space.denormalize(action)
+        else:
+            denormalized = action
+
+        goal_status = denormalized[0]
+
         assert 0 <= goal_status <= 1
         self.update_status(goal_status)
-        return super().step(action, normalized=normalized)
+        return super().step(denormalized, normalized=False)
 
     def get_co2(self, production):
         """
         Carbon dioxide emissions of energy production.
 
         Parameters
         ----------
@@ -201,15 +208,17 @@
         cost : float
             Total cost.
 
         """
         return self._get_fuel_cost(production) + self.get_co2_cost(production)
 
     def update(self, external_energy_change, as_source=False, as_sink=False):
-        assert as_source, 'This module may only act as a source.'
+        assert as_source or external_energy_change == 0.0, f'step() was called with negative energy (sink) for ' \
+                                                           f'module {self} but module is not a sink and ' \
+                                                           f'can only be called with positive energy.'
 
         reward = -1.0 * self.get_cost(external_energy_change)
         info = {'provided_energy': external_energy_change,
                 'co2_production': self.get_co2(external_energy_change)}
 
         return reward, False, info
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/modules/grid_module.py` & `python-microgrid-1.4.0/src/pymgrid/modules/grid_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,29 +77,31 @@
                  forecaster=None,
                  forecast_horizon=DEFAULT_HORIZON,
                  forecaster_increase_uncertainty=False,
                  forecaster_relative_noise=False,
                  initial_step=0,
                  final_step=-1,
                  cost_per_unit_co2=0.0,
+                 normalized_action_bounds=(0, 1),
                  raise_errors=False):
 
         time_series = self._check_params(max_import, max_export, time_series)
         self.max_import, self.max_export = max_import, max_export
         self.cost_per_unit_co2 = cost_per_unit_co2
-        self.name = ('grid', None)
+
         super().__init__(
             time_series,
             raise_errors,
             forecaster=forecaster,
             forecast_horizon=forecast_horizon,
             forecaster_increase_uncertainty=forecaster_increase_uncertainty,
             forecaster_relative_noise=forecaster_relative_noise,
             initial_step=initial_step,
             final_step=final_step,
+            normalized_action_bounds=normalized_action_bounds,
             provided_energy_name='grid_import',
             absorbed_energy_name='grid_export'
         )
 
     def _check_params(self, max_import, max_export, time_series):
         if max_import < 0:
             raise ValueError('parameter max_import must be non-negative.')
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/modules/load_module.py` & `python-microgrid-1.4.0/src/pymgrid/modules/load_module.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,36 +59,38 @@
                  time_series,
                  forecaster=None,
                  forecast_horizon=DEFAULT_HORIZON,
                  forecaster_increase_uncertainty=False,
                  forecaster_relative_noise=False,
                  initial_step=0,
                  final_step=-1,
+                 normalized_action_bounds=(0, 1),
                  raise_errors=False):
         super().__init__(
             time_series,
             raise_errors=raise_errors,
             forecaster=forecaster,
             forecast_horizon=forecast_horizon,
             forecaster_increase_uncertainty=forecaster_increase_uncertainty,
             forecaster_relative_noise=forecaster_relative_noise,
             initial_step=initial_step,
             final_step=final_step,
+            normalized_action_bounds=normalized_action_bounds,
             provided_energy_name=None,
             absorbed_energy_name='load_met'
         )
 
-        self.name = ('load', None)
-
     def _get_bounds(self):
         _min_obs, _max_obs, _, _ = super()._get_bounds()
         return _min_obs, _max_obs, np.array([]), np.array([])
 
     def update(self, external_energy_change, as_source=False, as_sink=False):
-        assert as_sink, f'Class {self.__class__.__name__} is a sink.'
+        assert as_sink or external_energy_change == 0.0, f'step() was called with positive energy (source) for ' \
+                                                           f'module {self} but module is not a source and ' \
+                                                           f'can only be called with negative energy.'
 
         info = {'absorbed_energy': self.current_load}
 
         return 0.0, self._done(), info
 
     def sample_action(self, strict_bound=False):
         return np.array([])
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/modules/module_container.py` & `python-microgrid-1.4.0/src/pymgrid/modules/module_container.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import json
 import pandas as pd
 
 from collections import UserDict, UserList
+import warnings
+
 from pymgrid.modules.base import BaseMicrogridModule
+from pymgrid.utils.eq import verbose_eq
 
 
 class Container(UserDict):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.dir_additions = self.dir_additions()
 
@@ -33,27 +36,48 @@
 
         """
         l = []
         for _, raw_container in self.containers.items():
             l.extend(raw_container.to_list())
         return l
 
-    def to_dict(self):
+    def to_dict(self, orient='list'):
         """
         Get the modules as a dictionary.
 
         Returns
         -------
         d : dict[str, list[module]]
             Dictionary with module names as keys, modules as values.
 
         """
+
+        def _dict_update_vals(raw_container):
+            if orient == 'list':
+                return raw_container
+            elif orient == 'records':
+                return {(name, n): module for name, mod_list in raw_container.items() for n, module in
+                        enumerate(mod_list)}
+
+        def _list_update_vals(key, raw_container):
+            if orient == 'list':
+                return {key: raw_container}
+            elif orient == 'records':
+                return {(key, n): module for n, module in enumerate(raw_container)}
+
+            raise ValueError(f"Unrecognized orient '{orient}'")
+
         d = dict()
+
         for k, raw_container in self.containers.items():
-            d.update(raw_container)
+            if isinstance(raw_container, ModuleList):
+                d.update(_list_update_vals(k, raw_container))
+            else:
+                d.update(_dict_update_vals(raw_container))
+
         return d
 
     def to_tuples(self):
         """
         Get the modules in (name, module) pairs.
 
         Returns
@@ -90,15 +114,19 @@
         iter : generator
             Iterator of (name, module) pairs.
 
         """
         for name, modules in self.to_dict().items():
             yield name, modules
 
-    def get_attrs(self, *attrs, unique=False, as_pandas=True):
+    def iteritems(self):
+        for name, module in self.to_dict(orient='records').items():
+            yield name, module
+
+    def get_attrs(self, *attrs, unique=False, as_pandas=True, drop_attr_names=False):
         """
         Get module attributes as a dictionary or pandas object.
 
         If ``unique``, checks that the value is unique for all modules and returns only the unique value.
         Otherwise, returns the values for all modules.
 
         If ``as_pandas``, returns either a pd.Series (if ``unique``) or pd.DataFrame of attributes.
@@ -119,14 +147,17 @@
 
         .. note::
             If only some modules have a particular attribute, ``get_attrs`` will not raise an error.
 
             If ``unique``, the unique value of the modules containing the value will be returned.
             Otherwise, ``NotImplemented`` will fill in missing values.
 
+        drop_attr_names : bool, default False
+            Whether to drop attribute names. Ignored if ``unique`` and ``len(attrs) == 1``.
+
         Returns
         -------
         d : dict or pd.DataFrame or pd.Series
             * Returns dict if ``as_pandas`` is False.
 
             * Otherwise, returns a pd.Series if ``unique`` and a pd.DataFrame otherwise.
 
@@ -142,61 +173,74 @@
             .. warning::
             This check is not performed if both ``unique`` and ``as_pandas`` are False.
 
         """
         if not attrs:
             raise ValueError('Missing attrs to get.')
 
+        if unique:
+            return self._get_unique_attrs(attrs, as_pandas, drop_attr_names)
+
+        def getattr_func(module, _attrs):
+            if drop_attr_names:
+                return [getattr(module, attr, NotImplemented) for attr in _attrs]
+            return {attr: getattr(module, attr, NotImplemented) for attr in _attrs}
+
         d = dict()
         for k, raw_container in self.containers.items():
             d.update({
-                name: [{attr: getattr(module, attr, NotImplemented) for attr in attrs} for module in module_list]
+                name: [getattr_func(module, attrs) for module in module_list]
                 for name, module_list in raw_container.items()
             })
 
-        if not (unique or as_pandas):
+        if not as_pandas:
             return d
 
         d_df = pd.DataFrame({(name, num): subdict for name, module_list in d.items()
                             for num, subdict in enumerate(module_list)}).T
 
-        bad_keys = []
-        uniques, nonuniques = {}, []
+        all_not_implemented = d_df.columns[(d_df == NotImplemented).all()]
 
-        for k, v in d_df.items():
-            not_notimplemented = v[v != NotImplemented]
-            unique_items = not_notimplemented.drop_duplicates().values
+        if len(all_not_implemented):
+            raise AttributeError(f'No values found for key(s) {all_not_implemented.tolist()}')
 
-            try:
-                unique_item = unique_items.item()
-            except ValueError:
-                if len(unique_items) == 0:
-                    # Only values were NotImplemented
-                    bad_keys.append(k)
-                else:
-                    nonuniques.append(k)
-            else:
-                uniques[k] = unique_item
+        return d_df
 
-        if len(bad_keys):
-            raise AttributeError(f'No values found for key(s) {bad_keys}')
+    def _get_unique_attrs(self, attrs, as_pandas, drop_attr_names):
+        if len(attrs) == 1:
+            return self._get_single_unique_attr(attrs[0])
 
-        if unique:
-            if len(nonuniques):
-                raise ValueError(f"Attribute(s) {nonuniques} have non-unique values, cannot return single unique value.")
+        if not drop_attr_names:
+            unique_attrs = {attr: self._get_single_unique_attr(attr) for attr in attrs}
+        else:
+            unique_attrs = [self._get_single_unique_attr(attr) for attr in attrs]
 
-            if not as_pandas:
-                return uniques
+        if as_pandas:
+            return pd.Series(unique_attrs)
 
-            return pd.Series(uniques, dtype=None if len(uniques) else float)
+        return unique_attrs
 
-        if as_pandas:
-            return d_df
+    def _get_single_unique_attr(self, attr):
+        val = NotImplemented
+        for module in self.iterlist():
+            try:
+                module_val = getattr(module, attr)
+            except AttributeError:
+                continue
 
-        return d
+            if val is NotImplemented:
+                val = module_val
+            elif module_val != val:
+                msg = f"Attribute [{attr}] has non-unique values, cannot return single unique value."
+                raise ValueError(msg)
+
+        if val is NotImplemented:
+            raise AttributeError(f'No values found for key {attr}.')
+
+        return val
 
     def set_attrs(self, attr_dict=None, **attrs):
         """
         Set the value of an attribute in all modules containing that attribute.
 
         Does nothing in modules not already containing the attribute.
 
@@ -256,15 +300,18 @@
     def __getitem__(self, item):
         if item == 'data' or item == 'module_dict':
             raise KeyError(item)
         try:
             return self.data[item]
         except KeyError:
             try:
-                return self.to_dict()[item]
+                if isinstance(item, tuple):
+                    return self.to_dict(orient='records')[item]
+                else:
+                    return self.to_dict()[item]
             except KeyError:
                 raise KeyError(item)
 
     def __getattr__(self, item):
         if item == 'data' or item.startswith('__') or item not in dir(self):
             raise AttributeError(item)
         try:
@@ -325,22 +372,22 @@
         container.big_battery
             Modules passed with custom name big_battery
 
         Each level can be iterated on, both by calling .items() or by iterating through the modules directly with .iterlist()
         For example, container.sinks.iterlist() returns an iterator of all the sinks, without their names.
 
     """
-    def __init__(self, modules):
+    def __init__(self, modules, set_names=True):
         """
 
         :param modules: list-like. List of _modules or tuples. Latter case: tup(str, Module); str to define name of module
             and second element is the module.
 
         """
-        self._containers = get_subcontainers(modules)
+        self._containers = get_subcontainers(modules, set_names=set_names)
         midlevels = self._set_midlevel()
         self._types_by_name = self._get_types_by_name()
         super().__init__(**midlevels)
 
     def _get_types_by_name(self):
         return {name: container_type for container_type, container in self._containers.items() for name in container}
 
@@ -394,16 +441,19 @@
         :meta private:
 
         Function to be compatible with Container API.
 
         """
         return self
 
+    def verbose_eq(self, other, indent=0):
+        verbose_eq(self, other, list(range(len(self))), indent=indent)
+
 
-def get_subcontainers(modules):
+def get_subcontainers(modules, set_names=True):
     """
     :meta private:
     """
     source_sink_keys = ('sources', 'sinks', 'source_and_sinks')
     fixed = {k: dict() for k in source_sink_keys}
     flex = {k: dict() for k in source_sink_keys}
     controllable = {k: dict() for k in source_sink_keys}
@@ -443,15 +493,22 @@
                 f'Attempted to add module {module_name} of type {(fixed_flex_controllable, source_sink_both)}, '
                 f'but there is an identically named module of type {module_names[module_name]}.')
 
         try:
             d[source_sink_both][module_name].append(module)
         except KeyError:
             d[source_sink_both][module_name] = ModuleList([module])
-        module.name = (module_name, len(d[source_sink_both][module_name]) - 1)
+
+        if set_names:
+            name = (module_name, len(d[source_sink_both][module_name]) - 1)
+
+            if name != module.name and module.name is not None:
+                warnings.warn(f"Overwriting module name '{module.name}' with name '{name}'.")
+
+            module.name = name
 
     modules_dict = dict(fixed=fixed,
                         flex=flex,
                         controllable=controllable)
 
     containers = {(ffs, source_sink_both): Container(modules_dict[ffs][source_sink_both])
                   for ffs in ('fixed', 'flex', 'controllable')
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/modules/renewable_module.py` & `python-microgrid-1.4.0/src/pymgrid/modules/renewable_module.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,30 +63,30 @@
                  raise_errors=False,
                  forecaster=None,
                  forecast_horizon=DEFAULT_HORIZON,
                  forecaster_increase_uncertainty=False,
                  forecaster_relative_noise=False,
                  initial_step=0,
                  final_step=-1,
+                 normalized_action_bounds=(0, 1),
                  provided_energy_name='renewable_used'):
         super().__init__(
             time_series,
             raise_errors,
             forecaster=forecaster,
             forecast_horizon=forecast_horizon,
             forecaster_increase_uncertainty=forecaster_increase_uncertainty,
             forecaster_relative_noise=forecaster_relative_noise,
             initial_step=initial_step,
             final_step=final_step,
+            normalized_action_bounds=normalized_action_bounds,
             provided_energy_name=provided_energy_name,
             absorbed_energy_name=None
         )
 
-        self.name = ('renewable', None)
-
     def update(self, external_energy_change, as_source=False, as_sink=False):
         assert as_source, f'Class {self.__class__.__name__} can only be used as a source.'
         assert external_energy_change <= self.current_renewable, f'Cannot provide more than {self.current_renewable}'
 
         info = {'provided_energy': external_energy_change,
                 'curtailment': self.current_renewable-external_energy_change}
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/modules/unbalanced_energy_module.py` & `python-microgrid-1.4.0/src/pymgrid/modules/unbalanced_energy_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,24 +10,25 @@
     yaml_dumper = yaml.SafeDumper
     yaml_loader = yaml.SafeLoader
 
     def __init__(self,
                  raise_errors,
                  initial_step=0,
                  loss_load_cost=10,
-                 overgeneration_cost=2.0
-                 ):
+                 overgeneration_cost=2.0,
+                 normalized_action_bounds = (0, 1)
+    ):
 
         super().__init__(raise_errors,
                          initial_step=initial_step,
+                         normalized_action_bounds=normalized_action_bounds,
                          provided_energy_name='loss_load',
                          absorbed_energy_name='overgeneration')
 
         self.loss_load_cost, self.overgeneration_cost = loss_load_cost, overgeneration_cost
-        self.name = ('unbalanced_energy', None)
 
     def update(self, external_energy_change, as_source=False, as_sink=False):
         assert as_source + as_sink == 1, 'Must act as either source or sink but not both or neither.'
 
         info_key = 'provided_energy' if as_source else 'absorbed_energy'
         reward = -1.0 * self.get_cost(external_energy_change, as_source, as_sink)
         assert reward <= 0
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/utils/DataGenerator.py` & `python-microgrid-1.4.0/src/pymgrid/utils/DataGenerator.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/utils/logger.py` & `python-microgrid-1.4.0/src/pymgrid/utils/logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,23 +11,31 @@
 
     def flush(self):
         d = self.data.copy()
         self.clear()
         self._log_length = 0
         return d
 
-    def log(self, **log_dict):
+    def log(self, log_dict=None, **log_items):
+        if log_items:
+            if log_dict:
+                raise TypeError('Cannot pass both positional and keyword arguments.')
+
+            log_dict = log_items
+
         for key, value in log_dict.items():
+            if key not in self:
+                self[key] = []
+
             try:
                 self[key].append(value.item())
             except AttributeError:
                 self[key].append(value)
-            except KeyError:
-                self[key] = [np.nan]*self._log_length
-                self[key].append(value)
+            except ValueError:
+                raise ValueError('Only scalar values can be logged.')
 
         self._log_length += 1
 
     def to_dict(self):
         return self.data.copy()
 
     def raw(self):
```

### Comparing `python-microgrid-1.3.0/src/pymgrid/utils/ray.py` & `python-microgrid-1.4.0/src/pymgrid/utils/ray.py`

 * *Files identical despite different names*

### Comparing `python-microgrid-1.3.0/src/pymgrid/utils/serialize.py` & `python-microgrid-1.4.0/src/pymgrid/utils/serialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,16 @@
         DeterministicTrajectory,
         StochasticTrajectory,
         FixedLengthStochasticTrajectory
     )
 
     from pymgrid.microgrid.reward_shaping import (
         PVCurtailmentShaper,
-        BatteryDischargeShaper
+        BatteryDischargeShaper,
+        RescaleShaper
     )
 
     from pymgrid.modules.battery.transition_models import (
         BatteryTransitionModel,
         BiasedTransitionModel,
         DecayTransitionModel
     )
```

### Comparing `python-microgrid-1.3.0/src/python_microgrid.egg-info/PKG-INFO` & `python-microgrid-1.4.0/src/python_microgrid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: python-microgrid
-Version: 1.3.0
+Version: 1.4.0
 Summary: A simulator for tertiary control of electrical microgrids
-Download-URL: https://github.com/Total-RD/pymgrid/archive/refs/tags/v1.3.0.tar.gz
+Download-URL: https://github.com/ahalev/python-microgrid/archive/refs/tags/v1.4.0.tar.gz
 Maintainer: Avishai Halev
 Maintainer-email: avishaihalev@gmail.com
 License: GNU LGPL 3.0
 Project-URL: Source Code, https://github.com/ahalev/python-microgrid
 Project-URL: Documentation, https://python-microgrid.readthedocs.io/
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -14,15 +14,15 @@
 Provides-Extra: dev
 Provides-Extra: rtd
 Provides-Extra: all
 License-File: LICENSE
 
 # python-microgrid
 
-![Build](https://github.com/Total-RD/pymgrid/workflows/build/badge.svg?dummy=unused)
+![Build](https://github.com/ahalev/python-microgrid/workflows/build/badge.svg?dummy=unused)
 
 *python-microgrid* is a python library to generate and simulate a large number of microgrids. It is an extension of TotalEnergies' [*pymgrid*](https://github.com/Total-RD/pymgrid).
 
 For more context, please see the [presentation](https://www.climatechange.ai/papers/neurips2020/3) done at Climate Change AI
 and the [documentation](https://python-microgrid.readthedocs.io/).
 
 ## Installation
```

### Comparing `python-microgrid-1.3.0/src/python_microgrid.egg-info/SOURCES.txt` & `python-microgrid-1.4.0/src/python_microgrid.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -145,17 +145,20 @@
 src/pymgrid/forecast/forecaster.py
 src/pymgrid/microgrid/__init__.py
 src/pymgrid/microgrid/convert_scenario_sandbox.py
 src/pymgrid/microgrid/microgrid.py
 src/pymgrid/microgrid/modular_microgrid_sandbox.py
 src/pymgrid/microgrid/serialization_sandbox.py
 src/pymgrid/microgrid/reward_shaping/__init__.py
+src/pymgrid/microgrid/reward_shaping/analyze_shaper.py
 src/pymgrid/microgrid/reward_shaping/base.py
+src/pymgrid/microgrid/reward_shaping/baseline_shaper.py
 src/pymgrid/microgrid/reward_shaping/battery_discharge_shaper.py
 src/pymgrid/microgrid/reward_shaping/pv_curtailment_shaper.py
+src/pymgrid/microgrid/reward_shaping/rescale_shaper.py
 src/pymgrid/microgrid/trajectory/__init__.py
 src/pymgrid/microgrid/trajectory/base.py
 src/pymgrid/microgrid/trajectory/deterministic.py
 src/pymgrid/microgrid/trajectory/stochastic.py
 src/pymgrid/microgrid/utils/__init__.py
 src/pymgrid/microgrid/utils/step.py
 src/pymgrid/modules/__init__.py
@@ -174,16 +177,21 @@
 src/pymgrid/modules/battery/transition_models/__init__.py
 src/pymgrid/modules/battery/transition_models/biased_transition_model.py
 src/pymgrid/modules/battery/transition_models/decay_transition_model.py
 src/pymgrid/modules/battery/transition_models/transition_model.py
 src/pymgrid/utils/DataGenerator.py
 src/pymgrid/utils/__init__.py
 src/pymgrid/utils/dry_run.py
+src/pymgrid/utils/eq.py
 src/pymgrid/utils/logger.py
 src/pymgrid/utils/ray.py
 src/pymgrid/utils/serialize.py
-src/pymgrid/utils/space.py
+src/pymgrid/utils/space/__init__.py
+src/pymgrid/utils/space/space.py
+src/pymgrid/utils/space/utils.py
 src/python_microgrid.egg-info/PKG-INFO
 src/python_microgrid.egg-info/SOURCES.txt
 src/python_microgrid.egg-info/dependency_links.txt
 src/python_microgrid.egg-info/requires.txt
-src/python_microgrid.egg-info/top_level.txt
+src/python_microgrid.egg-info/top_level.txt
+tests/test_microgridgenerator.py
+tests/test_nonmodular_microgrid.py
```

